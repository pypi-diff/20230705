# Comparing `tmp/extremecloudiq-api-23.3.2.1.tar.gz` & `tmp/extremecloudiq-api-23.4.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/lib/jenkins/workspace/Build-Promotions/UploadtoPyPi/dist/tmph7dyjgtd/extremecloudiq-api-23.3.2.1.tar", last modified: Fri Jun 16 04:33:44 2023, max compression
+gzip compressed data, was "/var/lib/jenkins/workspace/Build-Promotions/UploadtoPyPi/dist/tmpwk8bufox/extremecloudiq-api-23.4.0.41.tar", last modified: Wed Jul  5 16:10:55 2023, max compression
```

## Comparing `extremecloudiq-api-23.3.2.1.tar` & `extremecloudiq-api-23.4.0.41.tar`

### file list

```diff
@@ -1,822 +1,846 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/
--rw-r--r--   0 root         (0) root         (0)     1588 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32862 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/account_api.py
--rw-r--r--   0 root         (0) root         (0)    16606 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/alert_api.py
--rw-r--r--   0 root         (0) root         (0)    24695 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/application_api.py
--rw-r--r--   0 root         (0) root         (0)    11074 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/authentication_api.py
--rw-r--r--   0 root         (0) root         (0)    26154 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/authorization_api.py
--rw-r--r--   0 root         (0) root         (0)    47343 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/client_api.py
--rw-r--r--   0 root         (0) root         (0)   171864 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___authentication_api.py
--rw-r--r--   0 root         (0) root         (0)    34019 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___basic_api.py
--rw-r--r--   0 root         (0) root         (0)     7035 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___certificate_api.py
--rw-r--r--   0 root         (0) root         (0)    16187 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___deployment_api.py
--rw-r--r--   0 root         (0) root         (0)   292852 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___policy_api.py
--rw-r--r--   0 root         (0) root         (0)   133457 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___user_management_api.py
--rw-r--r--   0 root         (0) root         (0)    79847 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/copilot___anomalies_api.py
--rw-r--r--   0 root         (0) root         (0)    96668 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/copilot___connectivity_experience_api.py
--rw-r--r--   0 root         (0) root         (0)   261167 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/device_api.py
--rw-r--r--   0 root         (0) root         (0)    56014 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/hiq_api.py
--rw-r--r--   0 root         (0) root         (0)    67517 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/location_api.py
--rw-r--r--   0 root         (0) root         (0)    45961 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/log_api.py
--rw-r--r--   0 root         (0) root         (0)    49086 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/network_policy_api.py
--rw-r--r--   0 root         (0) root         (0)    15844 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/notification_api.py
--rw-r--r--   0 root         (0) root         (0)    16818 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/operation_api.py
--rw-r--r--   0 root         (0) root         (0)    59447 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api/user_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/
--rw-r--r--   0 root         (0) root         (0)    32173 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3761 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/inline_object.py
--rw-r--r--   0 root         (0) root         (0)     7332 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)     7548 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     7116 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     7197 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     7170 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     7467 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     7143 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     7413 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     7683 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     7521 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     7332 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     7062 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     7143 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     7494 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_digital_twin_products.py
--rw-r--r--   0 root         (0) root         (0)     7197 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)     7170 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     7521 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     7305 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)     7521 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)     7521 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     7251 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     7332 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     7305 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     7467 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     7386 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     7143 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     7089 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     7089 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_user.py
--rw-r--r--   0 root         (0) root         (0)     7224 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     7413 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)    14243 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_account.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_account_mode.py
--rw-r--r--   0 root         (0) root         (0)     2909 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_account_type.py
--rw-r--r--   0 root         (0) root         (0)    30788 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)    21693 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     2937 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py
--rw-r--r--   0 root         (0) root         (0)    10199 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     2986 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_category.py
--rw-r--r--   0 root         (0) root         (0)     2913 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_group_query.py
--rw-r--r--   0 root         (0) root         (0)     2884 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_severity.py
--rw-r--r--   0 root         (0) root         (0)     5055 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_source.py
--rw-r--r--   0 root         (0) root         (0)     2859 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_source_type.py
--rw-r--r--   0 root         (0) root         (0)    10206 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomalies_count_vo_entity.py
--rw-r--r--   0 root         (0) root         (0)    14366 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_device_entity.py
--rw-r--r--   0 root         (0) root         (0)     4637 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py
--rw-r--r--   0 root         (0) root         (0)     2909 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_health_type.py
--rw-r--r--   0 root         (0) root         (0)    12034 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     2898 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_severity.py
--rw-r--r--   0 root         (0) root         (0)     2899 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     3107 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_type.py
--rw-r--r--   0 root         (0) root         (0)    11006 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_api_token_info.py
--rw-r--r--   0 root         (0) root         (0)    11340 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_detection_protocol.py
--rw-r--r--   0 root         (0) root         (0)     5032 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_detection_rule.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_detection_type.py
--rw-r--r--   0 root         (0) root         (0)     2879 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     7296 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_top_clients_usage.py
--rw-r--r--   0 root         (0) root         (0)     4721 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assign_devices_country_code_request.py
--rw-r--r--   0 root         (0) root         (0)     4787 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assign_devices_location_request.py
--rw-r--r--   0 root         (0) root         (0)     4917 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assign_devices_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     5033 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assurance_scans_overview_response.py
--rw-r--r--   0 root         (0) root         (0)     6190 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_device_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     4743 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_device_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     8777 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_packet_counts_entity.py
--rw-r--r--   0 root         (0) root         (0)     4776 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_packet_counts_response.py
--rw-r--r--   0 root         (0) root         (0)     9991 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     2992 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_audit_log_category.py
--rw-r--r--   0 root         (0) root         (0)     2846 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_audit_log_sort_field.py
--rw-r--r--   0 root         (0) root         (0)    15660 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     5199 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_data.py
--rw-r--r--   0 root         (0) root         (0)     4359 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_operation_result.py
--rw-r--r--   0 root         (0) root         (0)     5672 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_request.py
--rw-r--r--   0 root         (0) root         (0)     3452 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_response.py
--rw-r--r--   0 root         (0) root         (0)     8802 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_building.py
--rw-r--r--   0 root         (0) root         (0)     9739 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     2844 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_certificate_type.py
--rw-r--r--   0 root         (0) root         (0)    10480 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_change_devices_ibeacon_request.py
--rw-r--r--   0 root         (0) root         (0)     5520 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_change_devices_os_mode_request.py
--rw-r--r--   0 root         (0) root         (0)     4512 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_check_permission_request.py
--rw-r--r--   0 root         (0) root         (0)     4715 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_check_permission_response.py
--rw-r--r--   0 root         (0) root         (0)    10384 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_classification.py
--rw-r--r--   0 root         (0) root         (0)     9146 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     3030 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_classification_type.py
--rw-r--r--   0 root         (0) root         (0)     5159 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cli_output.py
--rw-r--r--   0 root         (0) root         (0)     3849 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cli_response_code.py
--rw-r--r--   0 root         (0) root         (0)    36438 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     4736 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_field.py
--rw-r--r--   0 root         (0) root         (0)     3459 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_sort_field.py
--rw-r--r--   0 root         (0) root         (0)    10029 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     5121 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_summary.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_usage.py
--rw-r--r--   0 root         (0) root         (0)     2980 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_view.py
--rw-r--r--   0 root         (0) root         (0)    13089 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     8577 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     2937 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_connectivity_experience_view_type.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     3006 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     8601 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_wired_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)    10452 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)     8903 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_country_code.py
--rw-r--r--   0 root         (0) root         (0)     5500 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_building_request.py
--rw-r--r--   0 root         (0) root         (0)     6857 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     5416 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)    13024 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)    11802 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)    11599 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_floor_request.py
--rw-r--r--   0 root         (0) root         (0)    32292 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     3786 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)    19020 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     4576 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_location_request.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     4469 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_organization_request.py
--rw-r--r--   0 root         (0) root         (0)    18199 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     5564 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_client.py
--rw-r--r--   0 root         (0) root         (0)    15073 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     5735 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)    13169 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)     7342 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)    15879 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     4740 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     7691 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_user_request.py
--rw-r--r--   0 root         (0) root         (0)     5112 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     7192 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6670 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_webhook_subscription_request.py
--rw-r--r--   0 root         (0) root         (0)     6440 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     6706 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     4292 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_data_point.py
--rw-r--r--   0 root         (0) root         (0)     7368 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_date_time_type.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_date_time_unit_type.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_default_device_password.py
--rw-r--r--   0 root         (0) root         (0)     3766 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     4587 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_delivery_settings.py
--rw-r--r--   0 root         (0) root         (0)     3661 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dell_devices.py
--rw-r--r--   0 root         (0) root         (0)     5048 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_overview.py
--rw-r--r--   0 root         (0) root         (0)     6912 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_policy.py
--rw-r--r--   0 root         (0) root         (0)     4442 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_request.py
--rw-r--r--   0 root         (0) root         (0)     3464 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_response.py
--rw-r--r--   0 root         (0) root         (0)     8691 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)    29776 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     2965 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_admin_state.py
--rw-r--r--   0 root         (0) root         (0)     8198 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     5362 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_cpu_memory_usage.py
--rw-r--r--   0 root         (0) root         (0)     4313 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_field.py
--rw-r--r--   0 root         (0) root         (0)     3376 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_filter.py
--rw-r--r--   0 root         (0) root         (0)     3236 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_function.py
--rw-r--r--   0 root         (0) root         (0)     9175 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_ibeacon.py
--rw-r--r--   0 root         (0) root         (0)    11914 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_installation_report.py
--rw-r--r--   0 root         (0) root         (0)     5439 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_level_ssid.py
--rw-r--r--   0 root         (0) root         (0)     4957 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_lldp_cdp_info.py
--rw-r--r--   0 root         (0) root         (0)    14406 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_location.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_location_assignment.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_null_field.py
--rw-r--r--   0 root         (0) root         (0)     2838 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     5418 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_stats.py
--rw-r--r--   0 root         (0) root         (0)    10017 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     2890 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_type.py
--rw-r--r--   0 root         (0) root         (0)     2956 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_view.py
--rw-r--r--   0 root         (0) root         (0)    29252 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_wifi_interface.py
--rw-r--r--   0 root         (0) root         (0)     4432 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_channel_changes_entity.py
--rw-r--r--   0 root         (0) root         (0)     4606 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_channel_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     5837 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     4872 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     8069 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_device.py
--rw-r--r--   0 root         (0) root         (0)     3511 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_devices.py
--rw-r--r--   0 root         (0) root         (0)     3025 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_feat_license.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_make.py
--rw-r--r--   0 root         (0) root         (0)     4452 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_model.py
--rw-r--r--   0 root         (0) root         (0)     6349 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_products.py
--rw-r--r--   0 root         (0) root         (0)     3081 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_vim_module.py
--rw-r--r--   0 root         (0) root         (0)     5411 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_duplex_data_rate_entity.py
--rw-r--r--   0 root         (0) root         (0)     8665 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)    13080 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_email_template.py
--rw-r--r--   0 root         (0) root         (0)    19288 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_entitlement_type.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_error.py
--rw-r--r--   0 root         (0) root         (0)     3521 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_exos_devices.py
--rw-r--r--   0 root         (0) root         (0)     2918 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_expiration_action_type.py
--rw-r--r--   0 root         (0) root         (0)     8372 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_expiration_settings.py
--rw-r--r--   0 root         (0) root         (0)     3011 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_expiration_type.py
--rw-r--r--   0 root         (0) root         (0)     9135 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_account.py
--rw-r--r--   0 root         (0) root         (0)    13975 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     8959 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)    15642 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user_directory.py
--rw-r--r--   0 root         (0) root         (0)     5339 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user_directory_entry.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user_directory_type.py
--rw-r--r--   0 root         (0) root         (0)     3545 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_extreme_devices.py
--rw-r--r--   0 root         (0) root         (0)     6249 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_firmware_activate_option.py
--rw-r--r--   0 root         (0) root         (0)     5507 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_firmware_upgrade_policy.py
--rw-r--r--   0 root         (0) root         (0)     6362 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_flap_count_entity.py
--rw-r--r--   0 root         (0) root         (0)    15299 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_floor.py
--rw-r--r--   0 root         (0) root         (0)     3089 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_forensic_bucket.py
--rw-r--r--   0 root         (0) root         (0)     5813 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_generate_api_token_request.py
--rw-r--r--   0 root         (0) root         (0)     9829 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_generate_api_token_response.py
--rw-r--r--   0 root         (0) root         (0)     6336 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_get_port_assignment_details_response.py
--rw-r--r--   0 root         (0) root         (0)     6608 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_grant_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)     5021 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_hiq_context.py
--rw-r--r--   0 root         (0) root         (0)     3580 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_hiq_status.py
--rw-r--r--   0 root         (0) root         (0)     5920 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     4703 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_initialize_location_request.py
--rw-r--r--   0 root         (0) root         (0)     9687 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)    34396 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     3013 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     3180 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py
--rw-r--r--   0 root         (0) root         (0)    10730 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_key_based_pcg.py
--rw-r--r--   0 root         (0) root         (0)     9190 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_key_based_pcg_user.py
--rw-r--r--   0 root         (0) root         (0)     5806 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py
--rw-r--r--   0 root         (0) root         (0)     7343 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_l3_address_profile.py
--rw-r--r--   0 root         (0) root         (0)     2890 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_l3_address_type.py
--rw-r--r--   0 root         (0) root         (0)     2854 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ldap_protocol_type.py
--rw-r--r--   0 root         (0) root         (0)    18839 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     2921 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ldap_server_verification_mode.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_license_mode.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_license_status.py
--rw-r--r--   0 root         (0) root         (0)    11042 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_location.py
--rw-r--r--   0 root         (0) root         (0)     4025 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_location_legend.py
--rw-r--r--   0 root         (0) root         (0)     2874 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_location_type.py
--rw-r--r--   0 root         (0) root         (0)     4525 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_login_request.py
--rw-r--r--   0 root         (0) root         (0)     5818 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_login_response.py
--rw-r--r--   0 root         (0) root         (0)     2853 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_measurement_unit.py
--rw-r--r--   0 root         (0) root         (0)     9804 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     3084 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy_field.py
--rw-r--r--   0 root         (0) root         (0)     3377 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy_type.py
--rw-r--r--   0 root         (0) root         (0)     2858 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy_view.py
--rw-r--r--   0 root         (0) root         (0)     6713 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_onboard_device_request.py
--rw-r--r--   0 root         (0) root         (0)     5597 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py
--rw-r--r--   0 root         (0) root         (0)    12063 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_operation_metadata.py
--rw-r--r--   0 root         (0) root         (0)     6798 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_operation_object.py
--rw-r--r--   0 root         (0) root         (0)     3009 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_operation_status.py
--rw-r--r--   0 root         (0) root         (0)     8614 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_organization.py
--rw-r--r--   0 root         (0) root         (0)     2869 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_organization_type.py
--rw-r--r--   0 root         (0) root         (0)     3135 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_character_type.py
--rw-r--r--   0 root         (0) root         (0)     2865 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_db_location.py
--rw-r--r--   0 root         (0) root         (0)    10247 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_settings.py
--rw-r--r--   0 root         (0) root         (0)     2841 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_type.py
--rw-r--r--   0 root         (0) root         (0)     3937 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_assign_ports_request.py
--rw-r--r--   0 root         (0) root         (0)     6201 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_assign_ports_response.py
--rw-r--r--   0 root         (0) root         (0)     6696 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment.py
--rw-r--r--   0 root         (0) root         (0)    10512 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry.py
--rw-r--r--   0 root         (0) root         (0)     9628 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py
--rw-r--r--   0 root         (0) root         (0)     9870 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py
--rw-r--r--   0 root         (0) root         (0)    11649 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_type.py
--rw-r--r--   0 root         (0) root         (0)     5441 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_permission.py
--rw-r--r--   0 root         (0) root         (0)     4632 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_poe_flapping_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     4001 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     4010 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_port_efficiency_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     7189 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_post_expiration_action.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_psk_generation_method.py
--rw-r--r--   0 root         (0) root         (0)     2985 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radio_mode.py
--rw-r--r--   0 root         (0) root         (0)    24026 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     6103 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client.py
--rw-r--r--   0 root         (0) root         (0)    17440 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     6148 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client_object_entry.py
--rw-r--r--   0 root         (0) root         (0)     3058 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client_object_type.py
--rw-r--r--   0 root         (0) root         (0)    13996 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     2907 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_proxy_format_type.py
--rw-r--r--   0 root         (0) root         (0)     6300 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_server_type.py
--rw-r--r--   0 root         (0) root         (0)     3812 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_regenerate_end_user_password_response.py
--rw-r--r--   0 root         (0) root         (0)     3200 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rf_environment_type.py
--rw-r--r--   0 root         (0) root         (0)    31139 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_channel_selection.py
--rw-r--r--   0 root         (0) root         (0)    11298 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     8919 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_miscellaneous_settings.py
--rw-r--r--   0 root         (0) root         (0)    12893 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_neighborhood_analysis.py
--rw-r--r--   0 root         (0) root         (0)    50567 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_radio_usage_optimization.py
--rw-r--r--   0 root         (0) root         (0)     8500 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_sensor_scan_settings.py
--rw-r--r--   0 root         (0) root         (0)    12157 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_wmm_qos_settings.py
--rw-r--r--   0 root         (0) root         (0)     4444 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_send_cli_request.py
--rw-r--r--   0 root         (0) root         (0)     3772 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_send_cli_response.py
--rw-r--r--   0 root         (0) root         (0)     2911 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_server_role.py
--rw-r--r--   0 root         (0) root         (0)     6742 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sessions_data_entity.py
--rw-r--r--   0 root         (0) root         (0)     9305 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py
--rw-r--r--   0 root         (0) root         (0)    13068 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py
--rw-r--r--   0 root         (0) root         (0)    10196 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py
--rw-r--r--   0 root         (0) root         (0)    14920 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py
--rw-r--r--   0 root         (0) root         (0)    11002 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     2916 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sms_log_status.py
--rw-r--r--   0 root         (0) root         (0)    10606 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sms_template.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     2820 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sort_order.py
--rw-r--r--   0 root         (0) root         (0)     5339 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_speed_duplex_entity.py
--rw-r--r--   0 root         (0) root         (0)     9632 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     2971 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     2992 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_dot1x_key_management.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_key_type.py
--rw-r--r--   0 root         (0) root         (0)     2928 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_ppsk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     2933 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_psk_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     2960 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_psk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     2850 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_sae_group.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     2921 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_default_key.py
--rw-r--r--   0 root         (0) root         (0)     2888 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     2879 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_key_management.py
--rw-r--r--   0 root         (0) root         (0)     3176 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_subscription_data_type.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_subscription_message_type.py
--rw-r--r--   0 root         (0) root         (0)     2880 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_subscription_status.py
--rw-r--r--   0 root         (0) root         (0)     6384 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_top_applications_usage.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_trend_indicator.py
--rw-r--r--   0 root         (0) root         (0)     5030 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_building_request.py
--rw-r--r--   0 root         (0) root         (0)     6859 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     5906 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     5262 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)     6260 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)    10732 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)    10501 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     5312 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)    10458 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_floor_request.py
--rw-r--r--   0 root         (0) root         (0)    29854 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     3786 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)    16311 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     4263 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_location_request.py
--rw-r--r--   0 root         (0) root         (0)     5087 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)    18045 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_client.py
--rw-r--r--   0 root         (0) root         (0)    13978 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     6534 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)    11162 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)    31686 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_channel_selection_request.py
--rw-r--r--   0 root         (0) root         (0)     7033 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     5656 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py
--rw-r--r--   0 root         (0) root         (0)    10883 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py
--rw-r--r--   0 root         (0) root         (0)    58065 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py
--rw-r--r--   0 root         (0) root         (0)     5907 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py
--rw-r--r--   0 root         (0) root         (0)    11171 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py
--rw-r--r--   0 root         (0) root         (0)    15879 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     4421 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     6940 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_user_request.py
--rw-r--r--   0 root         (0) root         (0)     5112 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     7192 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)    14729 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user.py
--rw-r--r--   0 root         (0) root         (0)    19133 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     3137 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user_role.py
--rw-r--r--   0 root         (0) root         (0)     7243 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_daily_settings.py
--rw-r--r--   0 root         (0) root         (0)     5799 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_during_date_settings.py
--rw-r--r--   0 root         (0) root         (0)     6383 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_for_time_period_settings.py
--rw-r--r--   0 root         (0) root         (0)     7741 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_time_period_after_first_login.py
--rw-r--r--   0 root         (0) root         (0)     5242 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py
--rw-r--r--   0 root         (0) root         (0)     2925 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_time_period_after_type.py
--rw-r--r--   0 root         (0) root         (0)     7920 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_viq.py
--rw-r--r--   0 root         (0) root         (0)    13203 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_viq_license.py
--rw-r--r--   0 root         (0) root         (0)     8961 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_vlan_object_classified_entry.py
--rw-r--r--   0 root         (0) root         (0)    10998 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_vlan_profile_filter.py
--rw-r--r--   0 root         (0) root         (0)     3521 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_voss_devices.py
--rw-r--r--   0 root         (0) root         (0)    11214 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_webhook_subscription.py
--rw-r--r--   0 root         (0) root         (0)     3863 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wifi_capacity_client_list_response.py
--rw-r--r--   0 root         (0) root         (0)     3707 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wifi_capacity_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     3959 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wifi_efficiency_client_list_response.py
--rw-r--r--   0 root         (0) root         (0)     5723 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wifi_efficiency_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     3682 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wing_devices.py
--rw-r--r--   0 root         (0) root         (0)     8402 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)     7173 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_hardware_entity.py
--rw-r--r--   0 root         (0) root         (0)     3853 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_hardware_response.py
--rw-r--r--   0 root         (0) root         (0)     4583 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)     2827 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_view_type.py
--rw-r--r--   0 root         (0) root         (0)     7144 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_apps_response.py
--rw-r--r--   0 root         (0) root         (0)     4027 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py
--rw-r--r--   0 root         (0) root         (0)     8513 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_event_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_if_name.py
--rw-r--r--   0 root         (0) root         (0)     9193 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_performance_entity.py
--rw-r--r--   0 root         (0) root         (0)     5556 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_performance_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     5774 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)    13565 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py
--rw-r--r--   0 root         (0) root         (0)     3957 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_time_to_connect_response.py
--rw-r--r--   0 root         (0) root         (0)     2865 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_views_list_type.py
--rw-r--r--   0 root         (0) root         (0)     3834 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_views_type_response.py
--rw-r--r--   0 root         (0) root         (0)    34113 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26259 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/api_client.py
--rw-r--r--   0 root         (0) root         (0)    12883 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/configuration.py
--rw-r--r--   0 root         (0) root         (0)     3801 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    12333 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/extremecloudiq/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      375 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    36636 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/test/
--rw-r--r--   0 root         (0) root         (0)     1912 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_account_api.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_alert_api.py
--rw-r--r--   0 root         (0) root         (0)     1294 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_application_api.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_authentication_api.py
--rw-r--r--   0 root         (0) root         (0)     1572 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_authorization_api.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_client_api.py
--rw-r--r--   0 root         (0) root         (0)     6221 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_configuration___authentication_api.py
--rw-r--r--   0 root         (0) root         (0)     1736 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_configuration___basic_api.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_configuration___certificate_api.py
--rw-r--r--   0 root         (0) root         (0)     1339 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_configuration___deployment_api.py
--rw-r--r--   0 root         (0) root         (0)     9450 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_configuration___policy_api.py
--rw-r--r--   0 root         (0) root         (0)     4801 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_configuration___user_management_api.py
--rw-r--r--   0 root         (0) root         (0)     2581 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_copilot___anomalies_api.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_copilot___connectivity_experience_api.py
--rw-r--r--   0 root         (0) root         (0)     8485 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_device_api.py
--rw-r--r--   0 root         (0) root         (0)     2467 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_hiq_api.py
--rw-r--r--   0 root         (0) root         (0)     1449 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_inline_object.py
--rw-r--r--   0 root         (0) root         (0)     2472 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_location_api.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_log_api.py
--rw-r--r--   0 root         (0) root         (0)     2138 2023-06-08 21:13:45.000000 extremecloudiq-api-23.3.2.1/test/test_network_policy_api.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/test/test_notification_api.py
--rw-r--r--   0 root         (0) root         (0)     1250 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/test/test_operation_api.py
--rw-r--r--   0 root         (0) root         (0)     3344 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)     3019 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     2681 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     2491 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     2301 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     3024 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     4077 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     2599 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     2484 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     2729 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     2045 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     3937 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     2120 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_digital_twin_products.py
--rw-r--r--   0 root         (0) root         (0)     2110 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     2346 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)     2393 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)     4635 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     2793 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     2320 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     3042 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     3197 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     2459 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     2210 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     2653 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_user.py
--rw-r--r--   0 root         (0) root         (0)     6281 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     4818 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     4284 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     2200 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_paged_xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/test/test_user_api.py
--rw-r--r--   0 root         (0) root         (0)     2380 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_account.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_account_mode.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_account_type.py
--rw-r--r--   0 root         (0) root         (0)     2669 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_accounting_log.py
--rw-r--r--   0 root         (0) root         (0)     2647 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_active_directory_server.py
--rw-r--r--   0 root         (0) root         (0)     1681 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_active_directory_server_base_dn_fetch_mode.py
--rw-r--r--   0 root         (0) root         (0)     2160 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_alert.py
--rw-r--r--   0 root         (0) root         (0)     1418 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_alert_category.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_alert_group_query.py
--rw-r--r--   0 root         (0) root         (0)     1418 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_alert_severity.py
--rw-r--r--   0 root         (0) root         (0)     1505 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_alert_source.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_alert_source_type.py
--rw-r--r--   0 root         (0) root         (0)     1852 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomalies_count_vo_entity.py
--rw-r--r--   0 root         (0) root         (0)     1986 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_device_entity.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_devices_by_location_response.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_health_type.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_severity.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_type.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_api_token_info.py
--rw-r--r--   0 root         (0) root         (0)     2371 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_application.py
--rw-r--r--   0 root         (0) root         (0)     1585 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_application_detection_protocol.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_application_detection_rule.py
--rw-r--r--   0 root         (0) root         (0)     1541 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_application_detection_type.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_application_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_application_top_clients_usage.py
--rw-r--r--   0 root         (0) root         (0)     2523 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_assign_devices_location_request.py
--rw-r--r--   0 root         (0) root         (0)     2054 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_assign_devices_country_code_request.py
--rw-r--r--   0 root         (0) root         (0)     2060 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_assign_devices_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     2182 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_assurance_scans_overview_response.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_atp_device_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     1893 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_atp_device_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1803 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_atp_packet_counts_entity.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_atp_packet_counts_response.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_audit_log_category.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_audit_log_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_auth_log.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_data.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_operation_result.py
--rw-r--r--   0 root         (0) root         (0)     1642 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_request.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_response.py
--rw-r--r--   0 root         (0) root         (0)     2059 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_building.py
--rw-r--r--   0 root         (0) root         (0)     2141 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_certificate.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_certificate_type.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_change_devices_ibeacon_request.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_change_devices_os_mode_request.py
--rw-r--r--   0 root         (0) root         (0)     1633 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_check_permission_request.py
--rw-r--r--   0 root         (0) root         (0)     2176 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_check_permission_response.py
--rw-r--r--   0 root         (0) root         (0)     2242 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_classification.py
--rw-r--r--   0 root         (0) root         (0)     2711 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_classification_rule.py
--rw-r--r--   0 root         (0) root         (0)     1473 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_classification_type.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_cli_output.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_cli_response_code.py
--rw-r--r--   0 root         (0) root         (0)     3521 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client_field.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1778 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client_summary.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client_usage.py
--rw-r--r--   0 root         (0) root         (0)     1385 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_client_view.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_cloud_config_group.py
--rw-r--r--   0 root         (0) root         (0)     2261 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_connectivity_experience_data.py
--rw-r--r--   0 root         (0) root         (0)     1609 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_connectivity_experience_view_type.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_events_wired_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_events_wireless_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     2608 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_wired_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)     2218 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_wireless_event.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_wireless_events_score_type.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_country_code.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_building_request.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     2398 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     1769 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     2099 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_floor_request.py
--rw-r--r--   0 root         (0) root         (0)     5096 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     2499 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_location_request.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     1637 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_organization_request.py
--rw-r--r--   0 root         (0) root         (0)     2040 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_client.py
--rw-r--r--   0 root         (0) root         (0)     2939 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     3015 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)     1816 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     8503 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     2002 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_create_webhook_subscription_request.py
--rw-r--r--   0 root         (0) root         (0)     1594 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_credential_log.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_cwp.py
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_data_point.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_date_time_type.py
--rw-r--r--   0 root         (0) root         (0)     1455 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_date_time_unit_type.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_default_device_password.py
--rw-r--r--   0 root         (0) root         (0)     1751 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_delete_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     1529 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_delivery_settings.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_dell_devices.py
--rw-r--r--   0 root         (0) root         (0)     1631 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_overview.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_policy.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_request.py
--rw-r--r--   0 root         (0) root         (0)     1505 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_response.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_status.py
--rw-r--r--   0 root         (0) root         (0)     3429 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_admin_state.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_alarm.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_cpu_memory_usage.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_field.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-06-08 21:13:42.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_filter.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_function.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_ibeacon.py
--rw-r--r--   0 root         (0) root         (0)     1969 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_installation_report.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_level_ssid.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_lldp_cdp_info.py
--rw-r--r--   0 root         (0) root         (0)     2366 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_location.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_location_assignment.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_null_field.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1526 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_stats.py
--rw-r--r--   0 root         (0) root         (0)     1798 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     1385 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_type.py
--rw-r--r--   0 root         (0) root         (0)     1385 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_view.py
--rw-r--r--   0 root         (0) root         (0)     2593 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_device_wifi_interface.py
--rw-r--r--   0 root         (0) root         (0)     1624 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_channel_changes_entity.py
--rw-r--r--   0 root         (0) root         (0)     1611 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_channel_stats_entity.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_recurence_channel_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_recurence_count_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1918 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_device.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_devices.py
--rw-r--r--   0 root         (0) root         (0)     1521 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_feat_license.py
--rw-r--r--   0 root         (0) root         (0)     1442 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_make.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_model.py
--rw-r--r--   0 root         (0) root         (0)     1791 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_products.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_vim_module.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_duplex_data_rate_entity.py
--rw-r--r--   0 root         (0) root         (0)     1645 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_email_log.py
--rw-r--r--   0 root         (0) root         (0)     2314 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_email_template.py
--rw-r--r--   0 root         (0) root         (0)     2673 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_end_user.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_entitlement_type.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_error.py
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_exos_devices.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_expiration_action_type.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_expiration_settings.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_expiration_type.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_external_account.py
--rw-r--r--   0 root         (0) root         (0)     2482 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_external_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     2160 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_external_user.py
--rw-r--r--   0 root         (0) root         (0)     2716 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_external_user_directory.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_external_user_directory_entry.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_external_user_directory_type.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_extreme_devices.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_firmware_activate_option.py
--rw-r--r--   0 root         (0) root         (0)     1704 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_firmware_upgrade_policy.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_flap_count_entity.py
--rw-r--r--   0 root         (0) root         (0)     2504 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_floor.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_forensic_bucket.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_generate_api_token_request.py
--rw-r--r--   0 root         (0) root         (0)     2271 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_generate_api_token_response.py
--rw-r--r--   0 root         (0) root         (0)     5132 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_get_port_assignment_details_response.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_grant_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_hiq_context.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_hiq_status.py
--rw-r--r--   0 root         (0) root         (0)     2359 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_init_key_based_pcg_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_initialize_location_request.py
--rw-r--r--   0 root         (0) root         (0)     2241 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_device.py
--rw-r--r--   0 root         (0) root         (0)     5512 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_server.py
--rw-r--r--   0 root         (0) root         (0)     1721 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_server_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     1778 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_server_authentication_method_group.py
--rw-r--r--   0 root         (0) root         (0)     2744 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_key_based_pcg.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_key_based_pcg_user.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_key_based_pcg_user_base_info.py
--rw-r--r--   0 root         (0) root         (0)     2084 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_l3_address_profile.py
--rw-r--r--   0 root         (0) root         (0)     1420 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_l3_address_type.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ldap_protocol_type.py
--rw-r--r--   0 root         (0) root         (0)     2488 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ldap_server.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ldap_server_verification_mode.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_license_mode.py
--rw-r--r--   0 root         (0) root         (0)     1418 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_license_status.py
--rw-r--r--   0 root         (0) root         (0)     3474 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_location.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_location_legend.py
--rw-r--r--   0 root         (0) root         (0)     1407 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_location_type.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_login_request.py
--rw-r--r--   0 root         (0) root         (0)     1352 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_type.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_login_response.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_measurement_unit.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy_field.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy_type.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy_view.py
--rw-r--r--   0 root         (0) root         (0)     3058 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_onboard_device_request.py
--rw-r--r--   0 root         (0) root         (0)     1837 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_onboard_key_based_pcg_request.py
--rw-r--r--   0 root         (0) root         (0)     2381 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_operation_metadata.py
--rw-r--r--   0 root         (0) root         (0)     3238 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_operation_object.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_operation_status.py
--rw-r--r--   0 root         (0) root         (0)     2074 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_organization.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_organization_type.py
--rw-r--r--   0 root         (0) root         (0)     1508 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_password_character_type.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_password_db_location.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_password_settings.py
--rw-r--r--   0 root         (0) root         (0)     1407 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_password_type.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_assign_ports_request.py
--rw-r--r--   0 root         (0) root         (0)     2956 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_assign_ports_response.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry.py
--rw-r--r--   0 root         (0) root         (0)     4618 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry_detail.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry_device_meta.py
--rw-r--r--   0 root         (0) root         (0)     2576 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py
--rw-r--r--   0 root         (0) root         (0)     1574 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_permission.py
--rw-r--r--   0 root         (0) root         (0)     1910 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_poe_flapping_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_port_efficiency_speed_duplex_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1869 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_port_efficiency_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_post_expiration_action.py
--rw-r--r--   0 root         (0) root         (0)     1486 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_psk_generation_method.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radio_mode.py
--rw-r--r--   0 root         (0) root         (0)     2681 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radio_profile.py
--rw-r--r--   0 root         (0) root         (0)     1550 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client.py
--rw-r--r--   0 root         (0) root         (0)     3277 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client_object.py
--rw-r--r--   0 root         (0) root         (0)     1805 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client_object_entry.py
--rw-r--r--   0 root         (0) root         (0)     1521 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client_object_type.py
--rw-r--r--   0 root         (0) root         (0)     2806 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_proxy.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_proxy_format_type.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_radius_server_type.py
--rw-r--r--   0 root         (0) root         (0)     1707 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_regenerate_end_user_password_response.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rf_environment_type.py
--rw-r--r--   0 root         (0) root         (0)     2986 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_channel_selection.py
--rw-r--r--   0 root         (0) root         (0)     2178 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_mac_oui_profile.py
--rw-r--r--   0 root         (0) root         (0)     2833 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_miscellaneous_settings.py
--rw-r--r--   0 root         (0) root         (0)     2306 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_neighborhood_analysis.py
--rw-r--r--   0 root         (0) root         (0)     4357 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_radio_usage_optimization.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_sensor_scan_settings.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_rp_wmm_qos_settings.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_send_cli_request.py
--rw-r--r--   0 root         (0) root         (0)     1778 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_send_cli_response.py
--rw-r--r--   0 root         (0) root         (0)     1385 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_server_role.py
--rw-r--r--   0 root         (0) root         (0)     1672 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_sessions_data_entity.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_dot1x_request.py
--rw-r--r--   0 root         (0) root         (0)     2169 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_ppsk_request.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_psk_request.py
--rw-r--r--   0 root         (0) root         (0)     2031 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_wep_request.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_sms_log.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_sms_log_status.py
--rw-r--r--   0 root         (0) root         (0)     2186 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_sms_template.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_sort_field.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_sort_order.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_speed_duplex_entity.py
--rw-r--r--   0 root         (0) root         (0)     2071 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_dot1x_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     1521 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_dot1x_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_key_type.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_ppsk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_psk_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_psk_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_sae_group.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_authentication_method.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_default_key.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_encryption_method.py
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_key_management.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_subscription_data_type.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_subscription_message_type.py
--rw-r--r--   0 root         (0) root         (0)     1473 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_subscription_status.py
--rw-r--r--   0 root         (0) root         (0)     1639 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_top_applications_usage.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_trend_indicator.py
--rw-r--r--   0 root         (0) root         (0)     1600 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_building_request.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_classification_request.py
--rw-r--r--   0 root         (0) root         (0)     1953 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_device_level_ssid_status.py
--rw-r--r--   0 root         (0) root         (0)     2398 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_classification_rule_request.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_cloud_config_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_end_user_request.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_external_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_external_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1830 2023-06-08 21:13:43.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_floor_request.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_internal_radius_server_request.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_key_based_pcg_users_request.py
--rw-r--r--   0 root         (0) root         (0)     2077 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_ldap_server_request.py
--rw-r--r--   0 root         (0) root         (0)     1568 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_location_request.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_network_policy_request.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_radio_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1618 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_client.py
--rw-r--r--   0 root         (0) root         (0)     2306 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_client_object_request.py
--rw-r--r--   0 root         (0) root         (0)     1670 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_proxy_realm.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_proxy_request.py
--rw-r--r--   0 root         (0) root         (0)     2646 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_channel_selection_request.py
--rw-r--r--   0 root         (0) root         (0)     1759 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_mac_oui_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1756 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_miscellaneous_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_neighborhood_analysis_request.py
--rw-r--r--   0 root         (0) root         (0)     3371 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_radio_usage_optimization_request.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_sensor_scan_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     1831 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_wmm_qos_settings_request.py
--rw-r--r--   0 root         (0) root         (0)     8503 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_user_group_request.py
--rw-r--r--   0 root         (0) root         (0)     1609 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_user_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     1696 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_user_request.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_vlan_object_classified_entry_request.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_update_vlan_profile_request.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_user.py
--rw-r--r--   0 root         (0) root         (0)     9059 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_user_group.py
--rw-r--r--   0 root         (0) root         (0)     4351 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_user_profile.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_user_role.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_valid_daily_settings.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_valid_during_date_settings.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_valid_for_time_period_settings.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_valid_time_period_after_first_login.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_valid_time_period_after_id_creation.py
--rw-r--r--   0 root         (0) root         (0)     1545 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_valid_time_period_after_type.py
--rw-r--r--   0 root         (0) root         (0)     2484 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_viq.py
--rw-r--r--   0 root         (0) root         (0)     2374 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_viq_license.py
--rw-r--r--   0 root         (0) root         (0)     3275 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_vlan_object_classified_entry.py
--rw-r--r--   0 root         (0) root         (0)     3940 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_vlan_profile.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_vlan_profile_filter.py
--rw-r--r--   0 root         (0) root         (0)     1537 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_voss_devices.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_webhook_subscription.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wifi_capacity_client_list_response.py
--rw-r--r--   0 root         (0) root         (0)     2058 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wifi_capacity_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     2174 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wifi_efficiency_client_list_response.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wifi_efficiency_stats_response.py
--rw-r--r--   0 root         (0) root         (0)     1565 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wing_devices.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wired_event_entity.py
--rw-r--r--   0 root         (0) root         (0)     1697 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wired_hardware_entity.py
--rw-r--r--   0 root         (0) root         (0)     1884 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wired_hardware_response.py
--rw-r--r--   0 root         (0) root         (0)     1627 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wired_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)     1420 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wired_view_type.py
--rw-r--r--   0 root         (0) root         (0)     1682 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_apps_response.py
--rw-r--r--   0 root         (0) root         (0)     2438 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_connectivity_performance_response.py
--rw-r--r--   0 root         (0) root         (0)     1809 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_event_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     1431 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_if_name.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_performance_entity.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_performance_retries_entity.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_quality_index_response.py
--rw-r--r--   0 root         (0) root         (0)     2043 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_time_to_connect_entity.py
--rw-r--r--   0 root         (0) root         (0)     2296 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_time_to_connect_response.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_views_list_type.py
--rw-r--r--   0 root         (0) root         (0)     1640 2023-06-08 21:13:44.000000 extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_views_type_response.py
--rw-r--r--   0 root         (0) root         (0)    69227 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1123 2023-06-08 21:13:46.000000 extremecloudiq-api-23.3.2.1/setup.py
--rw-r--r--   0 root         (0) root         (0)      375 2023-06-16 04:33:44.000000 extremecloudiq-api-23.3.2.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:10:55.000000 extremecloudiq-api-23.4.0.41/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:10:55.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:10:55.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32863 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/account_api.py
+-rw-r--r--   0 root         (0) root         (0)    16607 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/alert_api.py
+-rw-r--r--   0 root         (0) root         (0)    24696 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/application_api.py
+-rw-r--r--   0 root         (0) root         (0)    11075 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)    26155 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/authorization_api.py
+-rw-r--r--   0 root         (0) root         (0)    53081 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/client_api.py
+-rw-r--r--   0 root         (0) root         (0)   171865 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/configuration___authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)    34020 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/configuration___basic_api.py
+-rw-r--r--   0 root         (0) root         (0)     7036 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/configuration___certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)    16188 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/configuration___deployment_api.py
+-rw-r--r--   0 root         (0) root         (0)   292853 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/configuration___policy_api.py
+-rw-r--r--   0 root         (0) root         (0)   133458 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/configuration___user_management_api.py
+-rw-r--r--   0 root         (0) root         (0)    79848 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/copilot___anomalies_api.py
+-rw-r--r--   0 root         (0) root         (0)    96669 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/copilot___connectivity_experience_api.py
+-rw-r--r--   0 root         (0) root         (0)   268481 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/device_api.py
+-rw-r--r--   0 root         (0) root         (0)    56015 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/hiq_api.py
+-rw-r--r--   0 root         (0) root         (0)    67518 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/location_api.py
+-rw-r--r--   0 root         (0) root         (0)    46740 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/log_api.py
+-rw-r--r--   0 root         (0) root         (0)    49087 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/network_policy_api.py
+-rw-r--r--   0 root         (0) root         (0)    15845 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/notification_api.py
+-rw-r--r--   0 root         (0) root         (0)    16819 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/operation_api.py
+-rw-r--r--   0 root         (0) root         (0)    59448 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api/user_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:10:55.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/
+-rw-r--r--   0 root         (0) root         (0)    33126 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3762 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/inline_object.py
+-rw-r--r--   0 root         (0) root         (0)     7333 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)     7549 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     7117 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     7198 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     7171 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     7414 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     7684 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     7333 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     7495 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_digital_twin_products.py
+-rw-r--r--   0 root         (0) root         (0)     7198 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)     7171 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     7306 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)     7522 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     7252 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     7333 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     7306 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7468 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     7387 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7144 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     7090 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     7090 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)     7225 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     7414 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)    14244 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_account.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_account_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_account_type.py
+-rw-r--r--   0 root         (0) root         (0)    30789 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)    21694 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py
+-rw-r--r--   0 root         (0) root         (0)     8513 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_advanced_onboard_device_request.py
+-rw-r--r--   0 root         (0) root         (0)     4854 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_advanced_onboard_device_response.py
+-rw-r--r--   0 root         (0) root         (0)    10200 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     2987 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_alert_category.py
+-rw-r--r--   0 root         (0) root         (0)     2914 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_alert_group_query.py
+-rw-r--r--   0 root         (0) root         (0)     2885 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_alert_severity.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_alert_source.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_alert_source_type.py
+-rw-r--r--   0 root         (0) root         (0)    10207 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomalies_count_vo_entity.py
+-rw-r--r--   0 root         (0) root         (0)    14367 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_device_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4638 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_health_type.py
+-rw-r--r--   0 root         (0) root         (0)    12035 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2899 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_severity.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_type.py
+-rw-r--r--   0 root         (0) root         (0)    11007 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_api_token_info.py
+-rw-r--r--   0 root         (0) root         (0)    11341 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_application_detection_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     5033 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_application_detection_rule.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_application_detection_type.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_application_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     7297 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_application_top_clients_usage.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_assign_devices_country_code_request.py
+-rw-r--r--   0 root         (0) root         (0)     4788 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_assign_devices_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     4918 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_assign_devices_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     5034 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_assurance_scans_overview_response.py
+-rw-r--r--   0 root         (0) root         (0)     6191 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_atp_device_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4744 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_atp_device_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     8778 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_atp_packet_counts_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4777 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_atp_packet_counts_response.py
+-rw-r--r--   0 root         (0) root         (0)     9992 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     2993 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_audit_log_category.py
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_audit_log_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)    15661 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     5200 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_bounce_device_port_data.py
+-rw-r--r--   0 root         (0) root         (0)     4360 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_bounce_device_port_operation_result.py
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_bounce_device_port_request.py
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_bounce_device_port_response.py
+-rw-r--r--   0 root         (0) root         (0)     8803 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_building.py
+-rw-r--r--   0 root         (0) root         (0)     9740 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     2845 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_certificate_type.py
+-rw-r--r--   0 root         (0) root         (0)    10481 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_change_devices_ibeacon_request.py
+-rw-r--r--   0 root         (0) root         (0)     5521 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_change_devices_os_mode_request.py
+-rw-r--r--   0 root         (0) root         (0)     4513 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_check_permission_request.py
+-rw-r--r--   0 root         (0) root         (0)     4716 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_check_permission_response.py
+-rw-r--r--   0 root         (0) root         (0)    10385 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_classification.py
+-rw-r--r--   0 root         (0) root         (0)     9147 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     3031 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_classification_type.py
+-rw-r--r--   0 root         (0) root         (0)     6707 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     5160 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_cli_output.py
+-rw-r--r--   0 root         (0) root         (0)     3850 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_cli_response_code.py
+-rw-r--r--   0 root         (0) root         (0)    37116 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client_field.py
+-rw-r--r--   0 root         (0) root         (0)     5513 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client_mac_address_alias.py
+-rw-r--r--   0 root         (0) root         (0)     3460 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)    10030 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5122 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client_summary.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2981 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client_view.py
+-rw-r--r--   0 root         (0) root         (0)    13090 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     8578 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_connectivity_experience_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     3007 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_copilot_wired_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)    10453 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)     8904 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_country_code.py
+-rw-r--r--   0 root         (0) root         (0)     5501 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     6858 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     5895 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     5417 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)    13025 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    11803 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)    11600 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)    32293 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)    19021 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     4577 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     5396 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     4470 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_organization_request.py
+-rw-r--r--   0 root         (0) root         (0)    18200 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)    15074 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     5736 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)    13170 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)     7343 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)    15880 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     4741 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     7692 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     5113 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     7193 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     6671 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_webhook_subscription_request.py
+-rw-r--r--   0 root         (0) root         (0)     6441 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     7369 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_date_time_type.py
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_date_time_unit_type.py
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_default_device_password.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_delivery_settings.py
+-rw-r--r--   0 root         (0) root         (0)     7081 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_dell_device.py
+-rw-r--r--   0 root         (0) root         (0)     3662 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_dell_devices.py
+-rw-r--r--   0 root         (0) root         (0)     5049 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_deployment_overview.py
+-rw-r--r--   0 root         (0) root         (0)     6913 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_deployment_policy.py
+-rw-r--r--   0 root         (0) root         (0)     4443 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_deployment_request.py
+-rw-r--r--   0 root         (0) root         (0)     3465 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_deployment_response.py
+-rw-r--r--   0 root         (0) root         (0)     8692 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)    29777 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_admin_state.py
+-rw-r--r--   0 root         (0) root         (0)     8199 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     5363 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_cpu_memory_usage.py
+-rw-r--r--   0 root         (0) root         (0)     4314 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_field.py
+-rw-r--r--   0 root         (0) root         (0)     3377 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_function.py
+-rw-r--r--   0 root         (0) root         (0)     9176 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_ibeacon.py
+-rw-r--r--   0 root         (0) root         (0)    11915 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_installation_report.py
+-rw-r--r--   0 root         (0) root         (0)     5440 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_level_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     4958 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)     5970 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_lldp_cdp_info.py
+-rw-r--r--   0 root         (0) root         (0)    14407 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_location.py
+-rw-r--r--   0 root         (0) root         (0)     6912 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_location_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_null_field.py
+-rw-r--r--   0 root         (0) root         (0)     2839 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     5419 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_stats.py
+-rw-r--r--   0 root         (0) root         (0)    10018 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_type.py
+-rw-r--r--   0 root         (0) root         (0)     2957 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_view.py
+-rw-r--r--   0 root         (0) root         (0)    29253 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_wifi_interface.py
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_dfs_channel_changes_entity.py
+-rw-r--r--   0 root         (0) root         (0)     4607 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_dfs_channel_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5838 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     8070 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_device.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_devices.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_feat_license.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_make.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_model.py
+-rw-r--r--   0 root         (0) root         (0)     6500 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_onboard_device.py
+-rw-r--r--   0 root         (0) root         (0)     6350 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_products.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_vim_module.py
+-rw-r--r--   0 root         (0) root         (0)     5412 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_duplex_data_rate_entity.py
+-rw-r--r--   0 root         (0) root         (0)     8666 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)    13081 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_email_template.py
+-rw-r--r--   0 root         (0) root         (0)    19289 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     2941 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_entitlement_type.py
+-rw-r--r--   0 root         (0) root         (0)     5520 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_error.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_exos_device.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_exos_devices.py
+-rw-r--r--   0 root         (0) root         (0)     2919 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_expiration_action_type.py
+-rw-r--r--   0 root         (0) root         (0)     8373 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_expiration_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3012 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_expiration_type.py
+-rw-r--r--   0 root         (0) root         (0)     9136 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_external_account.py
+-rw-r--r--   0 root         (0) root         (0)    13976 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     8960 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)    15643 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_external_user_directory.py
+-rw-r--r--   0 root         (0) root         (0)     5340 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_external_user_directory_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_external_user_directory_type.py
+-rw-r--r--   0 root         (0) root         (0)     6183 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_extreme_device.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_extreme_devices.py
+-rw-r--r--   0 root         (0) root         (0)     4461 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_failure_onboard_device.py
+-rw-r--r--   0 root         (0) root         (0)     6250 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_firmware_activate_option.py
+-rw-r--r--   0 root         (0) root         (0)     5508 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_firmware_upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)     6363 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_flap_count_entity.py
+-rw-r--r--   0 root         (0) root         (0)    15300 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_floor.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_forensic_bucket.py
+-rw-r--r--   0 root         (0) root         (0)     5814 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_generate_api_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     9830 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_generate_api_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_get_port_assignment_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     6609 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_grant_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     5022 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_hiq_context.py
+-rw-r--r--   0 root         (0) root         (0)     3581 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_hiq_status.py
+-rw-r--r--   0 root         (0) root         (0)     5921 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     4704 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_initialize_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     9688 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)    34397 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     3181 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py
+-rw-r--r--   0 root         (0) root         (0)    10731 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_key_based_pcg.py
+-rw-r--r--   0 root         (0) root         (0)     9191 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_key_based_pcg_user.py
+-rw-r--r--   0 root         (0) root         (0)     5807 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py
+-rw-r--r--   0 root         (0) root         (0)     7344 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_l3_address_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_l3_address_type.py
+-rw-r--r--   0 root         (0) root         (0)     2855 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ldap_protocol_type.py
+-rw-r--r--   0 root         (0) root         (0)    18840 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ldap_server_verification_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_license_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_license_status.py
+-rw-r--r--   0 root         (0) root         (0)    11043 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_location.py
+-rw-r--r--   0 root         (0) root         (0)     4026 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_location_legend.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_location_type.py
+-rw-r--r--   0 root         (0) root         (0)     4526 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_login_request.py
+-rw-r--r--   0 root         (0) root         (0)     5819 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_login_response.py
+-rw-r--r--   0 root         (0) root         (0)     2854 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_measurement_unit.py
+-rw-r--r--   0 root         (0) root         (0)     9805 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_network_policy_field.py
+-rw-r--r--   0 root         (0) root         (0)     3378 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_network_policy_type.py
+-rw-r--r--   0 root         (0) root         (0)     2859 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_network_policy_view.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_onboard_device_request.py
+-rw-r--r--   0 root         (0) root         (0)     6139 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_onboard_error.py
+-rw-r--r--   0 root         (0) root         (0)     5598 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py
+-rw-r--r--   0 root         (0) root         (0)    12064 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_operation_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     6799 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_operation_object.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_operation_status.py
+-rw-r--r--   0 root         (0) root         (0)     8615 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_organization.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_organization_type.py
+-rw-r--r--   0 root         (0) root         (0)     3136 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_password_character_type.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_password_db_location.py
+-rw-r--r--   0 root         (0) root         (0)    10248 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_password_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_password_type.py
+-rw-r--r--   0 root         (0) root         (0)     3938 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_assign_ports_request.py
+-rw-r--r--   0 root         (0) root         (0)     6202 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_assign_ports_response.py
+-rw-r--r--   0 root         (0) root         (0)     6697 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_port_assignment.py
+-rw-r--r--   0 root         (0) root         (0)    10513 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_port_assignment_entry.py
+-rw-r--r--   0 root         (0) root         (0)     9629 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py
+-rw-r--r--   0 root         (0) root         (0)     9871 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2843 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_type.py
+-rw-r--r--   0 root         (0) root         (0)     5442 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_permission.py
+-rw-r--r--   0 root         (0) root         (0)     4633 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_poe_flapping_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     4002 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_port_efficiency_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     7190 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_post_expiration_action.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_psk_generation_method.py
+-rw-r--r--   0 root         (0) root         (0)     2986 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radio_mode.py
+-rw-r--r--   0 root         (0) root         (0)    24027 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     6104 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)    17441 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     6149 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_client_object_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_client_object_type.py
+-rw-r--r--   0 root         (0) root         (0)    13997 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     2908 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_proxy_format_type.py
+-rw-r--r--   0 root         (0) root         (0)     6301 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_server_type.py
+-rw-r--r--   0 root         (0) root         (0)     3813 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_regenerate_end_user_password_response.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rf_environment_type.py
+-rw-r--r--   0 root         (0) root         (0)    31140 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_channel_selection.py
+-rw-r--r--   0 root         (0) root         (0)    11299 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     8920 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_miscellaneous_settings.py
+-rw-r--r--   0 root         (0) root         (0)    12894 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_neighborhood_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    50568 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_radio_usage_optimization.py
+-rw-r--r--   0 root         (0) root         (0)     8501 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_sensor_scan_settings.py
+-rw-r--r--   0 root         (0) root         (0)    12158 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_wmm_qos_settings.py
+-rw-r--r--   0 root         (0) root         (0)     4445 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_send_cli_request.py
+-rw-r--r--   0 root         (0) root         (0)     3773 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_send_cli_response.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_server_role.py
+-rw-r--r--   0 root         (0) root         (0)     6743 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_sessions_data_entity.py
+-rw-r--r--   0 root         (0) root         (0)     9306 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py
+-rw-r--r--   0 root         (0) root         (0)    13069 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py
+-rw-r--r--   0 root         (0) root         (0)    10197 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py
+-rw-r--r--   0 root         (0) root         (0)    14921 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py
+-rw-r--r--   0 root         (0) root         (0)    11003 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_sms_log_status.py
+-rw-r--r--   0 root         (0) root         (0)    10607 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_sms_template.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     2821 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_sort_order.py
+-rw-r--r--   0 root         (0) root         (0)     5340 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_speed_duplex_entity.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     2993 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_dot1x_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_key_type.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_ppsk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_psk_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_psk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_sae_group.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_wep_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_wep_default_key.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_wep_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_wep_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     3177 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_subscription_data_type.py
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_subscription_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     2881 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_subscription_status.py
+-rw-r--r--   0 root         (0) root         (0)     4736 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_success_onboard_device.py
+-rw-r--r--   0 root         (0) root         (0)     6385 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_top_applications_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_trend_indicator.py
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     6860 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     5907 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     5263 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     6261 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)    10733 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    10502 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     5313 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    10459 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)    29855 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)    16312 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     4264 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)    18046 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     6338 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)    13979 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     6535 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)    11163 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)    31687 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_channel_selection_request.py
+-rw-r--r--   0 root         (0) root         (0)     7034 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     5657 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)    10884 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py
+-rw-r--r--   0 root         (0) root         (0)    58066 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py
+-rw-r--r--   0 root         (0) root         (0)     5908 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)    11172 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)    15880 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     4422 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     6941 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     5113 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     7193 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)    14730 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)    19134 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     7058 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_user_role.py
+-rw-r--r--   0 root         (0) root         (0)     7244 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_valid_daily_settings.py
+-rw-r--r--   0 root         (0) root         (0)     5800 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_valid_during_date_settings.py
+-rw-r--r--   0 root         (0) root         (0)     6384 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_valid_for_time_period_settings.py
+-rw-r--r--   0 root         (0) root         (0)     7742 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_valid_time_period_after_first_login.py
+-rw-r--r--   0 root         (0) root         (0)     5243 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_valid_time_period_after_type.py
+-rw-r--r--   0 root         (0) root         (0)     7921 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_viq.py
+-rw-r--r--   0 root         (0) root         (0)    13204 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_viq_license.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_vlan_object_classified_entry.py
+-rw-r--r--   0 root         (0) root         (0)    10999 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_vlan_profile_filter.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_voss_device.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_voss_devices.py
+-rw-r--r--   0 root         (0) root         (0)    11215 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_webhook_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     3864 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wifi_capacity_client_list_response.py
+-rw-r--r--   0 root         (0) root         (0)     3708 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wifi_capacity_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     3960 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wifi_efficiency_client_list_response.py
+-rw-r--r--   0 root         (0) root         (0)     5724 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wifi_efficiency_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     7081 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wing_device.py
+-rw-r--r--   0 root         (0) root         (0)     3683 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wing_devices.py
+-rw-r--r--   0 root         (0) root         (0)     8403 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)     7174 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wired_hardware_entity.py
+-rw-r--r--   0 root         (0) root         (0)     3854 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wired_hardware_response.py
+-rw-r--r--   0 root         (0) root         (0)     4584 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wired_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wired_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     7145 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_apps_response.py
+-rw-r--r--   0 root         (0) root         (0)     4028 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py
+-rw-r--r--   0 root         (0) root         (0)     8514 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_event_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_if_name.py
+-rw-r--r--   0 root         (0) root         (0)     9194 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_performance_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_performance_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     5775 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)    13566 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py
+-rw-r--r--   0 root         (0) root         (0)     3958 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_time_to_connect_response.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_views_list_type.py
+-rw-r--r--   0 root         (0) root         (0)     3835 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_views_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    35067 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26261 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    12886 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3802 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12334 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/extremecloudiq/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:10:55.000000 extremecloudiq-api-23.4.0.41/extremecloudiq_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      376 2023-07-05 16:10:55.000000 extremecloudiq-api-23.4.0.41/extremecloudiq_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    37670 2023-07-05 16:10:55.000000 extremecloudiq-api-23.4.0.41/extremecloudiq_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 16:10:55.000000 extremecloudiq-api-23.4.0.41/extremecloudiq_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-07-05 16:10:55.000000 extremecloudiq-api-23.4.0.41/extremecloudiq_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-05 16:10:55.000000 extremecloudiq-api-23.4.0.41/extremecloudiq_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 16:10:55.000000 extremecloudiq-api-23.4.0.41/test/
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_account_api.py
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_alert_api.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_application_api.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_authorization_api.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_client_api.py
+-rw-r--r--   0 root         (0) root         (0)     6222 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_configuration___authentication_api.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_configuration___basic_api.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_configuration___certificate_api.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_configuration___deployment_api.py
+-rw-r--r--   0 root         (0) root         (0)     9451 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_configuration___policy_api.py
+-rw-r--r--   0 root         (0) root         (0)     4802 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_configuration___user_management_api.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_copilot___anomalies_api.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_copilot___connectivity_experience_api.py
+-rw-r--r--   0 root         (0) root         (0)     8661 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_device_api.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_hiq_api.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_inline_object.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_location_api.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_log_api.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_network_policy_api.py
+-rw-r--r--   0 root         (0) root         (0)     1226 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_notification_api.py
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_operation_api.py
+-rw-r--r--   0 root         (0) root         (0)     3345 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)     3020 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     2190 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     2730 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     2063 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     3938 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_digital_twin_products.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     2794 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)     6282 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     4819 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     4285 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_paged_xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/test/test_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2381 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_account.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_account_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_account_type.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_accounting_log.py
+-rw-r--r--   0 root         (0) root         (0)     2648 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_active_directory_server.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_active_directory_server_base_dn_fetch_mode.py
+-rw-r--r--   0 root         (0) root         (0)     5882 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_advanced_onboard_device_request.py
+-rw-r--r--   0 root         (0) root         (0)     2084 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_advanced_onboard_device_response.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_alert.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_alert_category.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_alert_group_query.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-06-19 21:31:04.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_alert_severity.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_alert_source.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_alert_source_type.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_anomalies_count_vo_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_device_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_devices_by_location_response.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_health_type.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_severity.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_type.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_api_token_info.py
+-rw-r--r--   0 root         (0) root         (0)     2372 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_application.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_application_detection_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_application_detection_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1542 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_application_detection_type.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_application_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_application_top_clients_usage.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_assign_devices_country_code_request.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_assign_devices_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     2061 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_assign_devices_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     2183 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_assurance_scans_overview_response.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_atp_device_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_atp_device_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_atp_packet_counts_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_atp_packet_counts_response.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_audit_log_category.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_audit_log_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_auth_log.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_bounce_device_port_data.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_bounce_device_port_operation_result.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_bounce_device_port_request.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_bounce_device_port_response.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_building.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_certificate_type.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_change_devices_ibeacon_request.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_change_devices_os_mode_request.py
+-rw-r--r--   0 root         (0) root         (0)     1634 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_check_permission_request.py
+-rw-r--r--   0 root         (0) root         (0)     2177 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_check_permission_response.py
+-rw-r--r--   0 root         (0) root         (0)     2243 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_classification_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_classification_type.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_cli_output.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_cli_response_code.py
+-rw-r--r--   0 root         (0) root         (0)     3552 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_client.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_client_field.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_client_mac_address_alias.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_client_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_client_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_client_summary.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_client_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_client_view.py
+-rw-r--r--   0 root         (0) root         (0)     2349 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_cloud_config_group.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_connectivity_experience_data.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_connectivity_experience_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_copilot_events_wired_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_copilot_events_wireless_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_copilot_wired_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_copilot_wireless_event.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_copilot_wireless_events_score_type.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_country_code.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)     5097 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_organization_request.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1593 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     8504 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     2003 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_create_webhook_subscription_request.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_credential_log.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_cwp.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_data_point.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_date_time_type.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_date_time_unit_type.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_dell_device.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_default_device_password.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_delete_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_delivery_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_dell_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1632 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_deployment_overview.py
+-rw-r--r--   0 root         (0) root         (0)     2081 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_deployment_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_deployment_request.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_deployment_response.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_deployment_status.py
+-rw-r--r--   0 root         (0) root         (0)     3430 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_admin_state.py
+-rw-r--r--   0 root         (0) root         (0)     1633 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_alarm.py
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_cpu_memory_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_field.py
+-rw-r--r--   0 root         (0) root         (0)     1477 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_function.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_ibeacon.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_installation_report.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_level_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_lldp_cdp_info.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_location.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_location_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_null_field.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1799 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_type.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_view.py
+-rw-r--r--   0 root         (0) root         (0)     2594 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_device_wifi_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_dfs_channel_changes_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_dfs_channel_stats_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_dfs_recurence_channel_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_dfs_recurence_count_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_device.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_feat_license.py
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_make.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_model.py
+-rw-r--r--   0 root         (0) root         (0)     2885 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_onboard_device.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_products.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_vim_module.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_duplex_data_rate_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_email_log.py
+-rw-r--r--   0 root         (0) root         (0)     2315 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_email_template.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_end_user.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_entitlement_type.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_error.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_exos_device.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_exos_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_expiration_action_type.py
+-rw-r--r--   0 root         (0) root         (0)     3768 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_expiration_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_expiration_type.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_external_account.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_external_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_external_user.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_external_user_directory.py
+-rw-r--r--   0 root         (0) root         (0)     1728 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_external_user_directory_entry.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_external_user_directory_type.py
+-rw-r--r--   0 root         (0) root         (0)     1860 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_extreme_device.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_extreme_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_failure_onboard_device.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_firmware_activate_option.py
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_firmware_upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_flap_count_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2505 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_floor.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_forensic_bucket.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_generate_api_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_generate_api_token_response.py
+-rw-r--r--   0 root         (0) root         (0)     5133 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_get_port_assignment_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     1812 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_grant_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_hiq_context.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_hiq_status.py
+-rw-r--r--   0 root         (0) root         (0)     2360 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_init_key_based_pcg_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_initialize_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_internal_radius_device.py
+-rw-r--r--   0 root         (0) root         (0)     5513 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_internal_radius_server.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_internal_radius_server_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_internal_radius_server_authentication_method_group.py
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_key_based_pcg.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_key_based_pcg_user.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_key_based_pcg_user_base_info.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_l3_address_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-06-19 21:31:05.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_l3_address_type.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ldap_protocol_type.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ldap_server.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ldap_server_verification_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_license_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_license_status.py
+-rw-r--r--   0 root         (0) root         (0)     3475 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_location.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_location_legend.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_location_type.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_login_request.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_login_response.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_measurement_unit.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_network_policy_field.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_network_policy_type.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_network_policy_view.py
+-rw-r--r--   0 root         (0) root         (0)     3059 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_onboard_device_request.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_onboard_error.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_onboard_key_based_pcg_request.py
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_operation_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3239 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_operation_object.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_operation_status.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_organization.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_organization_type.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_password_character_type.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_password_db_location.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_password_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_password_type.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_assign_ports_request.py
+-rw-r--r--   0 root         (0) root         (0)     2957 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_assign_ports_response.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_port_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     2208 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_port_assignment_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_port_assignment_entry_detail.py
+-rw-r--r--   0 root         (0) root         (0)     2368 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_port_assignment_entry_device_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_type.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_permission.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_poe_flapping_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_port_efficiency_speed_duplex_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_port_efficiency_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_post_expiration_action.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_psk_generation_method.py
+-rw-r--r--   0 root         (0) root         (0)     1375 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_radio_mode.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_radio_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_radius_client_object.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_radius_client_object_entry.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_radius_client_object_type.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_radius_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_radius_proxy_format_type.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     1454 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_radius_server_type.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_regenerate_end_user_password_response.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_rf_environment_type.py
+-rw-r--r--   0 root         (0) root         (0)     2987 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_rp_channel_selection.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_rp_mac_oui_profile.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_rp_miscellaneous_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_rp_neighborhood_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     4358 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_rp_radio_usage_optimization.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_rp_sensor_scan_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2214 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_rp_wmm_qos_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_send_cli_request.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_send_cli_response.py
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_server_role.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_sessions_data_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_set_ssid_mode_dot1x_request.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_set_ssid_mode_ppsk_request.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_set_ssid_mode_psk_request.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_set_ssid_mode_wep_request.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_sms_log.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_sms_log_status.py
+-rw-r--r--   0 root         (0) root         (0)     2187 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_sms_template.py
+-rw-r--r--   0 root         (0) root         (0)     1375 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_sort_field.py
+-rw-r--r--   0 root         (0) root         (0)     1375 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_sort_order.py
+-rw-r--r--   0 root         (0) root         (0)     1599 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_speed_duplex_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ssid.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_dot1x_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_dot1x_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_key_type.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_ppsk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_psk_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_psk_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_sae_group.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_wep_authentication_method.py
+-rw-r--r--   0 root         (0) root         (0)     1467 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_wep_default_key.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_wep_encryption_method.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_wep_key_management.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_subscription_data_type.py
+-rw-r--r--   0 root         (0) root         (0)     1531 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_subscription_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_subscription_status.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_success_onboard_device.py
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_top_applications_usage.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_trend_indicator.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_building_request.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_classification_request.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_classification_rule_request.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_cloud_config_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_device_level_ssid_status.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_end_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     2036 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_external_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_external_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_floor_request.py
+-rw-r--r--   0 root         (0) root         (0)     3387 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_internal_radius_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_key_based_pcg_users_request.py
+-rw-r--r--   0 root         (0) root         (0)     2078 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_ldap_server_request.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_location_request.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_network_policy_request.py
+-rw-r--r--   0 root         (0) root         (0)     2013 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_radio_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1619 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_radius_client.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_radius_client_object_request.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_radius_proxy_realm.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_radius_proxy_request.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_channel_selection_request.py
+-rw-r--r--   0 root         (0) root         (0)     1760 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_mac_oui_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_miscellaneous_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     1968 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_neighborhood_analysis_request.py
+-rw-r--r--   0 root         (0) root         (0)     3372 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_radio_usage_optimization_request.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_sensor_scan_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_wmm_qos_settings_request.py
+-rw-r--r--   0 root         (0) root         (0)     8504 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_user_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     1610 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_user_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     1697 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_vlan_object_classified_entry_request.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_update_vlan_profile_request.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_user.py
+-rw-r--r--   0 root         (0) root         (0)     9060 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_user_group.py
+-rw-r--r--   0 root         (0) root         (0)     4352 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_user_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_user_role.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_valid_daily_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_valid_during_date_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_valid_for_time_period_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1984 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_valid_time_period_after_first_login.py
+-rw-r--r--   0 root         (0) root         (0)     1796 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_valid_time_period_after_id_creation.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_valid_time_period_after_type.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_viq.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_viq_license.py
+-rw-r--r--   0 root         (0) root         (0)     3276 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_vlan_object_classified_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3941 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_vlan_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_vlan_profile_filter.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_voss_device.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_voss_devices.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_webhook_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wifi_capacity_client_list_response.py
+-rw-r--r--   0 root         (0) root         (0)     2059 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wifi_capacity_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wifi_efficiency_client_list_response.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wifi_efficiency_stats_response.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wing_device.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wing_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wired_event_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wired_hardware_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1885 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wired_hardware_response.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wired_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wired_view_type.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_apps_response.py
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_connectivity_performance_response.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_event_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_if_name.py
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_performance_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_performance_retries_entity.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_quality_index_response.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_time_to_connect_entity.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_time_to_connect_response.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_views_list_type.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2023-06-19 21:31:06.000000 extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_views_type_response.py
+-rw-r--r--   0 root         (0) root         (0)    70210 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/README.md
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-05 16:10:55.000000 extremecloudiq-api-23.4.0.41/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-19 21:31:08.000000 extremecloudiq-api-23.4.0.41/setup.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-07-05 16:10:55.000000 extremecloudiq-api-23.4.0.41/PKG-INFO
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/__init__.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/__init__.py`

 * *Files identical despite different names*

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/account_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/account_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/alert_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/alert_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/application_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/application_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/authentication_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/authorization_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/authorization_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/client_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/client_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -923,7 +923,125 @@
             response_type='PagedXiqClient',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
+
+    def set_clients_aliases(self, xiq_client_mac_address_alias, **kwargs):  # noqa: E501
+        """Set the aliases for multiple clients  # noqa: E501
+
+        Bulk update the aliases for multiple clients based on the mac addresses. Empty or null alias value deletes the previous client alias.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.set_clients_aliases(xiq_client_mac_address_alias, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param list[XiqClientMacAddressAlias] xiq_client_mac_address_alias: A list of client mac addresses and aliases (required)
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.set_clients_aliases_with_http_info(xiq_client_mac_address_alias, **kwargs)  # noqa: E501
+
+    def set_clients_aliases_with_http_info(self, xiq_client_mac_address_alias, **kwargs):  # noqa: E501
+        """Set the aliases for multiple clients  # noqa: E501
+
+        Bulk update the aliases for multiple clients based on the mac addresses. Empty or null alias value deletes the previous client alias.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.set_clients_aliases_with_http_info(xiq_client_mac_address_alias, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param list[XiqClientMacAddressAlias] xiq_client_mac_address_alias: A list of client mac addresses and aliases (required)
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'xiq_client_mac_address_alias'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method set_clients_aliases" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'xiq_client_mac_address_alias' is set
+        if self.api_client.client_side_validation and ('xiq_client_mac_address_alias' not in local_var_params or  # noqa: E501
+                                                        local_var_params['xiq_client_mac_address_alias'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `xiq_client_mac_address_alias` when calling `set_clients_aliases`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'xiq_client_mac_address_alias' in local_var_params:
+            body_params = local_var_params['xiq_client_mac_address_alias']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/clients/alias', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___authentication_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/configuration___authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___basic_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/configuration___basic_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___certificate_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/configuration___certificate_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___deployment_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/configuration___deployment_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___policy_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/configuration___policy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/configuration___user_management_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/configuration___user_management_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/copilot___anomalies_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/copilot___anomalies_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/copilot___connectivity_experience_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/copilot___connectivity_experience_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/device_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/device_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -33,14 +33,137 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
+    def advanced_onboard_devices(self, xiq_advanced_onboard_device_request, **kwargs):  # noqa: E501
+        """[LRO] Advanced Onboard Devices  # noqa: E501
+
+        Advanced onboard devices for all devices, such as Extreme/Aerohive, EXOS, VOSS, WiNG, Dell, and Digital Twin. Advanced onboard devices will allow the user to set the device hostname, attach the device location, associate network policy, etc. in a single API request. To avoid API timeout when onboarding a large number of devices, please make sure to enable async mode (set async=true in query parameter) and use long-running operation API to query the result.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.advanced_onboard_devices(xiq_advanced_onboard_device_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param XiqAdvancedOnboardDeviceRequest xiq_advanced_onboard_device_request: (required)
+        :param bool _async: Whether to enable async mode
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: XiqAdvancedOnboardDeviceResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.advanced_onboard_devices_with_http_info(xiq_advanced_onboard_device_request, **kwargs)  # noqa: E501
+
+    def advanced_onboard_devices_with_http_info(self, xiq_advanced_onboard_device_request, **kwargs):  # noqa: E501
+        """[LRO] Advanced Onboard Devices  # noqa: E501
+
+        Advanced onboard devices for all devices, such as Extreme/Aerohive, EXOS, VOSS, WiNG, Dell, and Digital Twin. Advanced onboard devices will allow the user to set the device hostname, attach the device location, associate network policy, etc. in a single API request. To avoid API timeout when onboarding a large number of devices, please make sure to enable async mode (set async=true in query parameter) and use long-running operation API to query the result.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.advanced_onboard_devices_with_http_info(xiq_advanced_onboard_device_request, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool: execute request asynchronously
+        :param XiqAdvancedOnboardDeviceRequest xiq_advanced_onboard_device_request: (required)
+        :param bool _async: Whether to enable async mode
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: tuple(XiqAdvancedOnboardDeviceResponse, status_code(int), headers(HTTPHeaderDict))
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        local_var_params = locals()
+
+        all_params = [
+            'xiq_advanced_onboard_device_request',
+            '_async'
+        ]
+        all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout'
+            ]
+        )
+
+        for key, val in six.iteritems(local_var_params['kwargs']):
+            if key not in all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method advanced_onboard_devices" % key
+                )
+            local_var_params[key] = val
+        del local_var_params['kwargs']
+        # verify the required parameter 'xiq_advanced_onboard_device_request' is set
+        if self.api_client.client_side_validation and ('xiq_advanced_onboard_device_request' not in local_var_params or  # noqa: E501
+                                                        local_var_params['xiq_advanced_onboard_device_request'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `xiq_advanced_onboard_device_request` when calling `advanced_onboard_devices`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if '_async' in local_var_params and local_var_params['_async'] is not None:  # noqa: E501
+            query_params.append(('async', local_var_params['_async']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'xiq_advanced_onboard_device_request' in local_var_params:
+            body_params = local_var_params['xiq_advanced_onboard_device_request']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/devices/:advanced-onboard', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='XiqAdvancedOnboardDeviceResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=local_var_params.get('async_req'),
+            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=local_var_params.get('_preload_content', True),
+            _request_timeout=local_var_params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def assign_device_location(self, id, xiq_device_location_assignment, **kwargs):  # noqa: E501
         """Assign location to a device  # noqa: E501
 
         Assign a location to a specific device with extra map and geographical properties.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.assign_device_location(id, xiq_device_location_assignment, async_req=True)
@@ -3447,16 +3570,17 @@
         :param list[str] sns: The device serial numbers
         :param list[str] hostnames: The device host names
         :param XiqDeviceSortField sort_field: The sort field
         :param XiqSortOrder order: The sort order (ascending by default)
         :param list[XiqDeviceView] views: The views to return device fields (Check fields for each view at XiqDeviceView schema)
         :param list[XiqDeviceField] fields: The device fields to return
         :param list[XiqDeviceType] device_types: The device types to return
-        :param bool _async: Whether to enable async mode
         :param XiqDeviceNullField null_field: The device empty field, only returns the selected field that is null
+        :param list[int] location_ids: The location IDs
+        :param bool _async: Whether to enable async mode
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -3486,16 +3610,17 @@
         :param list[str] sns: The device serial numbers
         :param list[str] hostnames: The device host names
         :param XiqDeviceSortField sort_field: The sort field
         :param XiqSortOrder order: The sort order (ascending by default)
         :param list[XiqDeviceView] views: The views to return device fields (Check fields for each view at XiqDeviceView schema)
         :param list[XiqDeviceField] fields: The device fields to return
         :param list[XiqDeviceType] device_types: The device types to return
-        :param bool _async: Whether to enable async mode
         :param XiqDeviceNullField null_field: The device empty field, only returns the selected field that is null
+        :param list[int] location_ids: The location IDs
+        :param bool _async: Whether to enable async mode
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -3518,16 +3643,17 @@
             'sns',
             'hostnames',
             'sort_field',
             'order',
             'views',
             'fields',
             'device_types',
-            '_async',
-            'null_field'
+            'null_field',
+            'location_ids',
+            '_async'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -3583,18 +3709,21 @@
             collection_formats['views'] = 'multi'  # noqa: E501
         if 'fields' in local_var_params and local_var_params['fields'] is not None:  # noqa: E501
             query_params.append(('fields', local_var_params['fields']))  # noqa: E501
             collection_formats['fields'] = 'multi'  # noqa: E501
         if 'device_types' in local_var_params and local_var_params['device_types'] is not None:  # noqa: E501
             query_params.append(('deviceTypes', local_var_params['device_types']))  # noqa: E501
             collection_formats['deviceTypes'] = 'multi'  # noqa: E501
-        if '_async' in local_var_params and local_var_params['_async'] is not None:  # noqa: E501
-            query_params.append(('async', local_var_params['_async']))  # noqa: E501
         if 'null_field' in local_var_params and local_var_params['null_field'] is not None:  # noqa: E501
             query_params.append(('nullField', local_var_params['null_field']))  # noqa: E501
+        if 'location_ids' in local_var_params and local_var_params['location_ids'] is not None:  # noqa: E501
+            query_params.append(('locationIds', local_var_params['location_ids']))  # noqa: E501
+            collection_formats['locationIds'] = 'multi'  # noqa: E501
+        if '_async' in local_var_params and local_var_params['_async'] is not None:  # noqa: E501
+            query_params.append(('async', local_var_params['_async']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/hiq_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/hiq_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/location_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/location_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/log_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/log_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -174,65 +174,65 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def list_audit_logs(self, **kwargs):  # noqa: E501
+    def list_audit_logs(self, start_time, end_time, **kwargs):  # noqa: E501
         """List audit logs  # noqa: E501
 
         List a page of audit logs.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.list_audit_logs(async_req=True)
+        >>> thread = api.list_audit_logs(start_time, end_time, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param int start_time: The start time to query, epoch time in milliseconds since 1/1/1970 (required)
+        :param int end_time: The end time to query, epoch time in milliseconds since 1/1/1970. Note: endTime - startTime must be no greater than 2592000000 (30 days) (required)
         :param int page: Page number, min = 1
         :param int limit: Page Size, min = 1, max = 100
         :param XiqAuditLogSortField sort_field: The field for sorting
         :param XiqSortOrder sort_order: The sorting order
         :param list[XiqAuditLogCategory] categories: Audit category
         :param str username: The user login name
-        :param int start_time: The start time to query, epoch time in milliseconds since 1/1/1970, default is 0 if not specified or is negative
-        :param int end_time: The end time to query, epoch time in milliseconds since 1/1/1970, default is now if not specified or is negative, endTime - startTime must be no greater than 2592000000 (30 days)
         :param str keyword: The case-insensitive keyword to search in description
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: PagedXiqAuditLog
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_audit_logs_with_http_info(**kwargs)  # noqa: E501
+        return self.list_audit_logs_with_http_info(start_time, end_time, **kwargs)  # noqa: E501
 
-    def list_audit_logs_with_http_info(self, **kwargs):  # noqa: E501
+    def list_audit_logs_with_http_info(self, start_time, end_time, **kwargs):  # noqa: E501
         """List audit logs  # noqa: E501
 
         List a page of audit logs.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.list_audit_logs_with_http_info(async_req=True)
+        >>> thread = api.list_audit_logs_with_http_info(start_time, end_time, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool: execute request asynchronously
+        :param int start_time: The start time to query, epoch time in milliseconds since 1/1/1970 (required)
+        :param int end_time: The end time to query, epoch time in milliseconds since 1/1/1970. Note: endTime - startTime must be no greater than 2592000000 (30 days) (required)
         :param int page: Page number, min = 1
         :param int limit: Page Size, min = 1, max = 100
         :param XiqAuditLogSortField sort_field: The field for sorting
         :param XiqSortOrder sort_order: The sorting order
         :param list[XiqAuditLogCategory] categories: Audit category
         :param str username: The user login name
-        :param int start_time: The start time to query, epoch time in milliseconds since 1/1/1970, default is 0 if not specified or is negative
-        :param int end_time: The end time to query, epoch time in milliseconds since 1/1/1970, default is now if not specified or is negative, endTime - startTime must be no greater than 2592000000 (30 days)
         :param str keyword: The case-insensitive keyword to search in description
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -243,22 +243,22 @@
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
+            'start_time',
+            'end_time',
             'page',
             'limit',
             'sort_field',
             'sort_order',
             'categories',
             'username',
-            'start_time',
-            'end_time',
             'keyword'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -270,14 +270,22 @@
             if key not in all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
                     " to method list_audit_logs" % key
                 )
             local_var_params[key] = val
         del local_var_params['kwargs']
+        # verify the required parameter 'start_time' is set
+        if self.api_client.client_side_validation and ('start_time' not in local_var_params or  # noqa: E501
+                                                        local_var_params['start_time'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `start_time` when calling `list_audit_logs`")  # noqa: E501
+        # verify the required parameter 'end_time' is set
+        if self.api_client.client_side_validation and ('end_time' not in local_var_params or  # noqa: E501
+                                                        local_var_params['end_time'] is None):  # noqa: E501
+            raise ApiValueError("Missing the required parameter `end_time` when calling `list_audit_logs`")  # noqa: E501
 
         if self.api_client.client_side_validation and 'page' in local_var_params and local_var_params['page'] < 1:  # noqa: E501
             raise ApiValueError("Invalid value for parameter `page` when calling `list_audit_logs`, must be a value greater than or equal to `1`")  # noqa: E501
         if self.api_client.client_side_validation and 'limit' in local_var_params and local_var_params['limit'] > 100:  # noqa: E501
             raise ApiValueError("Invalid value for parameter `limit` when calling `list_audit_logs`, must be a value less than or equal to `100`")  # noqa: E501
         if self.api_client.client_side_validation and 'limit' in local_var_params and local_var_params['limit'] < 1:  # noqa: E501
             raise ApiValueError("Invalid value for parameter `limit` when calling `list_audit_logs`, must be a value greater than or equal to `1`")  # noqa: E501
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/network_policy_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/network_policy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/notification_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/notification_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/operation_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/operation_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api/user_api.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/__init__.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -54,14 +54,16 @@
 from extremecloudiq.models.paged_xiq_wired_event_entity import PagedXiqWiredEventEntity
 from extremecloudiq.models.xiq_account import XiqAccount
 from extremecloudiq.models.xiq_account_mode import XiqAccountMode
 from extremecloudiq.models.xiq_account_type import XiqAccountType
 from extremecloudiq.models.xiq_accounting_log import XiqAccountingLog
 from extremecloudiq.models.xiq_active_directory_server import XiqActiveDirectoryServer
 from extremecloudiq.models.xiq_active_directory_server_base_dn_fetch_mode import XiqActiveDirectoryServerBaseDnFetchMode
+from extremecloudiq.models.xiq_advanced_onboard_device_request import XiqAdvancedOnboardDeviceRequest
+from extremecloudiq.models.xiq_advanced_onboard_device_response import XiqAdvancedOnboardDeviceResponse
 from extremecloudiq.models.xiq_alert import XiqAlert
 from extremecloudiq.models.xiq_alert_category import XiqAlertCategory
 from extremecloudiq.models.xiq_alert_group_query import XiqAlertGroupQuery
 from extremecloudiq.models.xiq_alert_severity import XiqAlertSeverity
 from extremecloudiq.models.xiq_alert_source import XiqAlertSource
 from extremecloudiq.models.xiq_alert_source_type import XiqAlertSourceType
 from extremecloudiq.models.xiq_anomalies_count_vo_entity import XiqAnomaliesCountVoEntity
@@ -105,14 +107,15 @@
 from extremecloudiq.models.xiq_classification import XiqClassification
 from extremecloudiq.models.xiq_classification_rule import XiqClassificationRule
 from extremecloudiq.models.xiq_classification_type import XiqClassificationType
 from extremecloudiq.models.xiq_cli_output import XiqCliOutput
 from extremecloudiq.models.xiq_cli_response_code import XiqCliResponseCode
 from extremecloudiq.models.xiq_client import XiqClient
 from extremecloudiq.models.xiq_client_field import XiqClientField
+from extremecloudiq.models.xiq_client_mac_address_alias import XiqClientMacAddressAlias
 from extremecloudiq.models.xiq_client_sort_field import XiqClientSortField
 from extremecloudiq.models.xiq_client_stats_entity import XiqClientStatsEntity
 from extremecloudiq.models.xiq_client_summary import XiqClientSummary
 from extremecloudiq.models.xiq_client_usage import XiqClientUsage
 from extremecloudiq.models.xiq_client_view import XiqClientView
 from extremecloudiq.models.xiq_cloud_config_group import XiqCloudConfigGroup
 from extremecloudiq.models.xiq_connectivity_experience_data import XiqConnectivityExperienceData
@@ -153,14 +156,15 @@
 from extremecloudiq.models.xiq_cwp import XiqCwp
 from extremecloudiq.models.xiq_data_point import XiqDataPoint
 from extremecloudiq.models.xiq_date_time_type import XiqDateTimeType
 from extremecloudiq.models.xiq_date_time_unit_type import XiqDateTimeUnitType
 from extremecloudiq.models.xiq_default_device_password import XiqDefaultDevicePassword
 from extremecloudiq.models.xiq_delete_key_based_pcg_users_request import XiqDeleteKeyBasedPcgUsersRequest
 from extremecloudiq.models.xiq_delivery_settings import XiqDeliverySettings
+from extremecloudiq.models.xiq_dell_device import XiqDellDevice
 from extremecloudiq.models.xiq_dell_devices import XiqDellDevices
 from extremecloudiq.models.xiq_deployment_overview import XiqDeploymentOverview
 from extremecloudiq.models.xiq_deployment_policy import XiqDeploymentPolicy
 from extremecloudiq.models.xiq_deployment_request import XiqDeploymentRequest
 from extremecloudiq.models.xiq_deployment_response import XiqDeploymentResponse
 from extremecloudiq.models.xiq_deployment_status import XiqDeploymentStatus
 from extremecloudiq.models.xiq_device import XiqDevice
@@ -189,33 +193,37 @@
 from extremecloudiq.models.xiq_dfs_recurence_channel_stats_response import XiqDfsRecurenceChannelStatsResponse
 from extremecloudiq.models.xiq_dfs_recurence_count_stats_response import XiqDfsRecurenceCountStatsResponse
 from extremecloudiq.models.xiq_digital_twin_device import XiqDigitalTwinDevice
 from extremecloudiq.models.xiq_digital_twin_devices import XiqDigitalTwinDevices
 from extremecloudiq.models.xiq_digital_twin_feat_license import XiqDigitalTwinFeatLicense
 from extremecloudiq.models.xiq_digital_twin_make import XiqDigitalTwinMake
 from extremecloudiq.models.xiq_digital_twin_model import XiqDigitalTwinModel
+from extremecloudiq.models.xiq_digital_twin_onboard_device import XiqDigitalTwinOnboardDevice
 from extremecloudiq.models.xiq_digital_twin_products import XiqDigitalTwinProducts
 from extremecloudiq.models.xiq_digital_twin_vim_module import XiqDigitalTwinVimModule
 from extremecloudiq.models.xiq_duplex_data_rate_entity import XiqDuplexDataRateEntity
 from extremecloudiq.models.xiq_email_log import XiqEmailLog
 from extremecloudiq.models.xiq_email_template import XiqEmailTemplate
 from extremecloudiq.models.xiq_end_user import XiqEndUser
 from extremecloudiq.models.xiq_entitlement_type import XiqEntitlementType
 from extremecloudiq.models.xiq_error import XiqError
+from extremecloudiq.models.xiq_exos_device import XiqExosDevice
 from extremecloudiq.models.xiq_exos_devices import XiqExosDevices
 from extremecloudiq.models.xiq_expiration_action_type import XiqExpirationActionType
 from extremecloudiq.models.xiq_expiration_settings import XiqExpirationSettings
 from extremecloudiq.models.xiq_expiration_type import XiqExpirationType
 from extremecloudiq.models.xiq_external_account import XiqExternalAccount
 from extremecloudiq.models.xiq_external_radius_server import XiqExternalRadiusServer
 from extremecloudiq.models.xiq_external_user import XiqExternalUser
 from extremecloudiq.models.xiq_external_user_directory import XiqExternalUserDirectory
 from extremecloudiq.models.xiq_external_user_directory_entry import XiqExternalUserDirectoryEntry
 from extremecloudiq.models.xiq_external_user_directory_type import XiqExternalUserDirectoryType
+from extremecloudiq.models.xiq_extreme_device import XiqExtremeDevice
 from extremecloudiq.models.xiq_extreme_devices import XiqExtremeDevices
+from extremecloudiq.models.xiq_failure_onboard_device import XiqFailureOnboardDevice
 from extremecloudiq.models.xiq_firmware_activate_option import XiqFirmwareActivateOption
 from extremecloudiq.models.xiq_firmware_upgrade_policy import XiqFirmwareUpgradePolicy
 from extremecloudiq.models.xiq_flap_count_entity import XiqFlapCountEntity
 from extremecloudiq.models.xiq_floor import XiqFloor
 from extremecloudiq.models.xiq_forensic_bucket import XiqForensicBucket
 from extremecloudiq.models.xiq_generate_api_token_request import XiqGenerateApiTokenRequest
 from extremecloudiq.models.xiq_generate_api_token_response import XiqGenerateApiTokenResponse
@@ -246,14 +254,15 @@
 from extremecloudiq.models.xiq_login_response import XiqLoginResponse
 from extremecloudiq.models.xiq_measurement_unit import XiqMeasurementUnit
 from extremecloudiq.models.xiq_network_policy import XiqNetworkPolicy
 from extremecloudiq.models.xiq_network_policy_field import XiqNetworkPolicyField
 from extremecloudiq.models.xiq_network_policy_type import XiqNetworkPolicyType
 from extremecloudiq.models.xiq_network_policy_view import XiqNetworkPolicyView
 from extremecloudiq.models.xiq_onboard_device_request import XiqOnboardDeviceRequest
+from extremecloudiq.models.xiq_onboard_error import XiqOnboardError
 from extremecloudiq.models.xiq_onboard_key_based_pcg_request import XiqOnboardKeyBasedPcgRequest
 from extremecloudiq.models.xiq_operation_metadata import XiqOperationMetadata
 from extremecloudiq.models.xiq_operation_object import XiqOperationObject
 from extremecloudiq.models.xiq_operation_status import XiqOperationStatus
 from extremecloudiq.models.xiq_organization import XiqOrganization
 from extremecloudiq.models.xiq_organization_type import XiqOrganizationType
 from extremecloudiq.models.xiq_password_character_type import XiqPasswordCharacterType
@@ -318,14 +327,15 @@
 from extremecloudiq.models.xiq_ssid_wep_authentication_method import XiqSsidWepAuthenticationMethod
 from extremecloudiq.models.xiq_ssid_wep_default_key import XiqSsidWepDefaultKey
 from extremecloudiq.models.xiq_ssid_wep_encryption_method import XiqSsidWepEncryptionMethod
 from extremecloudiq.models.xiq_ssid_wep_key_management import XiqSsidWepKeyManagement
 from extremecloudiq.models.xiq_subscription_data_type import XiqSubscriptionDataType
 from extremecloudiq.models.xiq_subscription_message_type import XiqSubscriptionMessageType
 from extremecloudiq.models.xiq_subscription_status import XiqSubscriptionStatus
+from extremecloudiq.models.xiq_success_onboard_device import XiqSuccessOnboardDevice
 from extremecloudiq.models.xiq_top_applications_usage import XiqTopApplicationsUsage
 from extremecloudiq.models.xiq_trend_indicator import XiqTrendIndicator
 from extremecloudiq.models.xiq_update_building_request import XiqUpdateBuildingRequest
 from extremecloudiq.models.xiq_update_classification_request import XiqUpdateClassificationRequest
 from extremecloudiq.models.xiq_update_classification_rule_request import XiqUpdateClassificationRuleRequest
 from extremecloudiq.models.xiq_update_cloud_config_group_request import XiqUpdateCloudConfigGroupRequest
 from extremecloudiq.models.xiq_update_device_level_ssid_status import XiqUpdateDeviceLevelSsidStatus
@@ -366,20 +376,22 @@
 from extremecloudiq.models.xiq_valid_time_period_after_id_creation import XiqValidTimePeriodAfterIdCreation
 from extremecloudiq.models.xiq_valid_time_period_after_type import XiqValidTimePeriodAfterType
 from extremecloudiq.models.xiq_viq import XiqViq
 from extremecloudiq.models.xiq_viq_license import XiqViqLicense
 from extremecloudiq.models.xiq_vlan_object_classified_entry import XiqVlanObjectClassifiedEntry
 from extremecloudiq.models.xiq_vlan_profile import XiqVlanProfile
 from extremecloudiq.models.xiq_vlan_profile_filter import XiqVlanProfileFilter
+from extremecloudiq.models.xiq_voss_device import XiqVossDevice
 from extremecloudiq.models.xiq_voss_devices import XiqVossDevices
 from extremecloudiq.models.xiq_webhook_subscription import XiqWebhookSubscription
 from extremecloudiq.models.xiq_wifi_capacity_client_list_response import XiqWifiCapacityClientListResponse
 from extremecloudiq.models.xiq_wifi_capacity_stats_response import XiqWifiCapacityStatsResponse
 from extremecloudiq.models.xiq_wifi_efficiency_client_list_response import XiqWifiEfficiencyClientListResponse
 from extremecloudiq.models.xiq_wifi_efficiency_stats_response import XiqWifiEfficiencyStatsResponse
+from extremecloudiq.models.xiq_wing_device import XiqWingDevice
 from extremecloudiq.models.xiq_wing_devices import XiqWingDevices
 from extremecloudiq.models.xiq_wired_event_entity import XiqWiredEventEntity
 from extremecloudiq.models.xiq_wired_hardware_entity import XiqWiredHardwareEntity
 from extremecloudiq.models.xiq_wired_hardware_response import XiqWiredHardwareResponse
 from extremecloudiq.models.xiq_wired_quality_index_response import XiqWiredQualityIndexResponse
 from extremecloudiq.models.xiq_wired_view_type import XiqWiredViewType
 from extremecloudiq.models.xiq_wireless_apps_response import XiqWirelessAppsResponse
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/inline_object.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/inline_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_accounting_log.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_accounting_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_active_directory_server.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_active_directory_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_alert.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_alert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_application.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_application.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_audit_log.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_audit_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_auth_log.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_auth_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_certificate.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_classification_rule.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_classification_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_client.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_cloud_config_group.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_cloud_config_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_connectivity_experience_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_copilot_wireless_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_credential_log.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_credential_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_cwp.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_cwp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_device.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_device_alarm.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_device_alarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_digital_twin_products.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_digital_twin_products.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_email_log.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_email_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_end_user.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_end_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_external_radius_server.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_external_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_external_user.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_external_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_internal_radius_device.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_internal_radius_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_internal_radius_server.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_internal_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_ldap_server.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_ldap_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_network_policy.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_network_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_radio_profile.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_radio_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_radius_client_object.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_radius_client_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_radius_proxy.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_radius_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_rp_mac_oui_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_sms_log.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_sms_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_ssid.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_ssid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_user.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_user_group.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_user_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_user_profile.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_user_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_vlan_profile.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_vlan_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/paged_xiq_wired_event_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/paged_xiq_wired_event_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_account.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_account_mode.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_account_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_account_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_account_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_accounting_log.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_accounting_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_active_directory_server.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_active_directory_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_category.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_alert_category.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_group_query.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_alert_group_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_severity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_alert_severity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_source.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_alert_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_alert_source_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_alert_source_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomalies_count_vo_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomalies_count_vo_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_device_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_device_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_devices_by_location_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_health_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_health_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_location_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_severity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_severity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_sort_field.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_anomaly_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_anomaly_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_api_token_info.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_api_token_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_application.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_detection_protocol.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_application_detection_protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_detection_rule.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_application_detection_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_detection_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_application_detection_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_sort_field.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_application_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_application_top_clients_usage.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_application_top_clients_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assign_devices_country_code_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_assign_devices_country_code_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assign_devices_location_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_assign_devices_location_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assign_devices_network_policy_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_assign_devices_network_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_assurance_scans_overview_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_assurance_scans_overview_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_device_stats_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_atp_device_stats_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_device_stats_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_atp_device_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_packet_counts_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_atp_packet_counts_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_atp_packet_counts_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_atp_packet_counts_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_audit_log.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_audit_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_audit_log_category.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_audit_log_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_audit_log_sort_field.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_audit_log_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_auth_log.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_auth_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_data.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_bounce_device_port_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_operation_result.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_bounce_device_port_operation_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_bounce_device_port_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_bounce_device_port_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_bounce_device_port_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_building.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_building.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_certificate.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_certificate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_certificate_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_certificate_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_change_devices_ibeacon_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_change_devices_ibeacon_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_change_devices_os_mode_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_change_devices_os_mode_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_check_permission_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_check_permission_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_check_permission_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_check_permission_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_classification.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_classification_rule.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_classification_rule.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_classification_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_classification_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cli_output.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_cli_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cli_response_code.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_cli_response_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -72,15 +72,16 @@
         'snr': 'int',
         'description': 'str',
         'category': 'str',
         'mobility': 'str',
         'port_type_name': 'str',
         'wing_ap': 'bool',
         'vendor': 'str',
-        'locations': 'list[XiqLocationLegend]'
+        'locations': 'list[XiqLocationLegend]',
+        'alias': 'str'
     }
 
     attribute_map = {
         'id': 'id',
         'create_time': 'create_time',
         'update_time': 'update_time',
         'org_id': 'org_id',
@@ -118,18 +119,19 @@
         'snr': 'snr',
         'description': 'description',
         'category': 'category',
         'mobility': 'mobility',
         'port_type_name': 'port_type_name',
         'wing_ap': 'wing_ap',
         'vendor': 'vendor',
-        'locations': 'locations'
+        'locations': 'locations',
+        'alias': 'alias'
     }
 
-    def __init__(self, id=None, create_time=None, update_time=None, org_id=None, location_id=None, device_id=None, hostname=None, mac_address=None, ip_address=None, ipv6_address=None, os_type=None, username=None, user_profile_name=None, connected=None, online_time=None, offline_time=None, vlan=None, connection_type=None, ssid=None, port=None, org_name=None, device_function=None, device_mac_address=None, device_name=None, auth=None, channel=None, client_health=None, application_health=None, radio_health=None, network_health=None, radio_type=None, encryption_method=None, interface_name=None, bssid=None, rssi=None, snr=None, description=None, category=None, mobility=None, port_type_name=None, wing_ap=None, vendor=None, locations=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, create_time=None, update_time=None, org_id=None, location_id=None, device_id=None, hostname=None, mac_address=None, ip_address=None, ipv6_address=None, os_type=None, username=None, user_profile_name=None, connected=None, online_time=None, offline_time=None, vlan=None, connection_type=None, ssid=None, port=None, org_name=None, device_function=None, device_mac_address=None, device_name=None, auth=None, channel=None, client_health=None, application_health=None, radio_health=None, network_health=None, radio_type=None, encryption_method=None, interface_name=None, bssid=None, rssi=None, snr=None, description=None, category=None, mobility=None, port_type_name=None, wing_ap=None, vendor=None, locations=None, alias=None, local_vars_configuration=None):  # noqa: E501
         """XiqClient - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._create_time = None
@@ -170,14 +172,15 @@
         self._description = None
         self._category = None
         self._mobility = None
         self._port_type_name = None
         self._wing_ap = None
         self._vendor = None
         self._locations = None
+        self._alias = None
         self.discriminator = None
 
         self.id = id
         self.create_time = create_time
         self.update_time = update_time
         if org_id is not None:
             self.org_id = org_id
@@ -255,14 +258,16 @@
             self.port_type_name = port_type_name
         if wing_ap is not None:
             self.wing_ap = wing_ap
         if vendor is not None:
             self.vendor = vendor
         if locations is not None:
             self.locations = locations
+        if alias is not None:
+            self.alias = alias
 
     @property
     def id(self):
         """Gets the id of this XiqClient.  # noqa: E501
 
         The unique identifier  # noqa: E501
 
@@ -1251,14 +1256,37 @@
 
         :param locations: The locations of this XiqClient.  # noqa: E501
         :type: list[XiqLocationLegend]
         """
 
         self._locations = locations
 
+    @property
+    def alias(self):
+        """Gets the alias of this XiqClient.  # noqa: E501
+
+        The alias of the client  # noqa: E501
+
+        :return: The alias of this XiqClient.  # noqa: E501
+        :rtype: str
+        """
+        return self._alias
+
+    @alias.setter
+    def alias(self, alias):
+        """Sets the alias of this XiqClient.
+
+        The alias of the client  # noqa: E501
+
+        :param alias: The alias of this XiqClient.  # noqa: E501
+        :type: str
+        """
+
+        self._alias = alias
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_field.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -71,16 +71,17 @@
     RADIO_TYPE = "RADIO_TYPE"
     WING_AP = "WING_AP"
     VENDOR = "VENDOR"
     MOBILITY = "MOBILITY"
     CATEGORY = "CATEGORY"
     DESCRIPTION = "DESCRIPTION"
     DEVICE_MAC_ADDRESS = "DEVICE_MAC_ADDRESS"
+    ALIAS = "ALIAS"
 
-    allowable_values = [ID, CREATE_TIME, UPDATE_TIME, ORG_ID, ORG_NAME, LOCATION_ID, LOCATIONS, HOSTNAME, MAC_ADDRESS, IP_ADDRESS, IPV6_ADDRESS, OS_TYPE, DEVICE_ID, DEVICE_FUNCTION, DEVICE_NAME, USERNAME, USER_PROFILE_NAME, CONNECTED, ONLINE_TIME, OFFLINE_TIME, VLAN, CONNECTION_TYPE, SSID, PORT, BSSID, PORT_TYPE_NAME, INTERFACE_NAME, AUTH, ENCRYPTION_METHOD, CHANNEL, CLIENT_HEALTH, APPLICATION_HEALTH, NETWORK_HEALTH, RADIO_HEALTH, HEALTH_UPDATE_TIME, RSSI, RSSI_UPDATE_TIME, SNR, SNR_UPDATE_TIME, RADIO_TYPE, WING_AP, VENDOR, MOBILITY, CATEGORY, DESCRIPTION, DEVICE_MAC_ADDRESS]  # noqa: E501
+    allowable_values = [ID, CREATE_TIME, UPDATE_TIME, ORG_ID, ORG_NAME, LOCATION_ID, LOCATIONS, HOSTNAME, MAC_ADDRESS, IP_ADDRESS, IPV6_ADDRESS, OS_TYPE, DEVICE_ID, DEVICE_FUNCTION, DEVICE_NAME, USERNAME, USER_PROFILE_NAME, CONNECTED, ONLINE_TIME, OFFLINE_TIME, VLAN, CONNECTION_TYPE, SSID, PORT, BSSID, PORT_TYPE_NAME, INTERFACE_NAME, AUTH, ENCRYPTION_METHOD, CHANNEL, CLIENT_HEALTH, APPLICATION_HEALTH, NETWORK_HEALTH, RADIO_HEALTH, HEALTH_UPDATE_TIME, RSSI, RSSI_UPDATE_TIME, SNR, SNR_UPDATE_TIME, RADIO_TYPE, WING_AP, VENDOR, MOBILITY, CATEGORY, DESCRIPTION, DEVICE_MAC_ADDRESS, ALIAS]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_sort_field.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_stats_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client_stats_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_summary.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_usage.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_client_view.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_client_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cloud_config_group.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_cloud_config_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_connectivity_experience_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_connectivity_experience_view_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_connectivity_experience_view_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_copilot_events_wired_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_copilot_events_wireless_sort_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_copilot_paged_xiq_anomaly_location_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_wired_events_score_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_copilot_wired_events_score_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_copilot_wireless_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_copilot_wireless_events_score_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_country_code.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_country_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_building_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_building_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_classification_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_classification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_classification_rule_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_classification_rule_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_cloud_config_group_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_cloud_config_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_end_user_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_end_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_external_radius_server_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_external_radius_server_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_floor_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_floor_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_internal_radius_server_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_internal_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_key_based_pcg_users_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_ldap_server_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_ldap_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_location_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_location_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_network_policy_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_network_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_organization_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_organization_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radio_profile_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_radio_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_client.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_radius_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_client_object_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_radius_client_object_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_proxy_realm.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_radius_proxy_realm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_radius_proxy_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_radius_proxy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_rp_mac_oui_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_user_group_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_user_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_user_profile_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_user_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_user_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_vlan_object_classified_entry_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_vlan_profile_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_vlan_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_create_webhook_subscription_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_create_webhook_subscription_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_credential_log.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_credential_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_cwp.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_cwp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_data_point.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_data_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_date_time_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_date_time_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_date_time_unit_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_date_time_unit_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_default_device_password.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_default_device_password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_delivery_settings.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_delivery_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dell_devices.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_dell_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_overview.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_deployment_overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_policy.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_deployment_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_deployment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_deployment_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_deployment_status.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_deployment_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_admin_state.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_admin_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_alarm.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_alarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_cpu_memory_usage.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_cpu_memory_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_field.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_filter.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_function.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_ibeacon.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_ibeacon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_installation_report.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_installation_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_level_ssid.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_level_ssid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_level_ssid_status.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_level_ssid_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_lldp_cdp_info.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_lldp_cdp_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_location.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_location_assignment.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_location_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_null_field.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_null_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_sort_field.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_sort_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_stats.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_stats_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_stats_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_view.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_device_wifi_interface.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_device_wifi_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_channel_changes_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_dfs_channel_changes_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_channel_stats_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_dfs_channel_stats_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_device.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_devices.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_feat_license.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_feat_license.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -29,16 +29,17 @@
     """
     allowed enum values
     """
     _5000_PRMR = "PRD_5000_PRMR"
     _5000_MACSEC = "PRD_5000_MACSEC"
     _5320_10G_4P = "PRD_5320_10G_4P"
     _5320_10G_8P = "PRD_5320_10G_8P"
+    _7000_PRMR = "PRD_7000_PRMR"
 
-    allowable_values = [_5000_PRMR, _5000_MACSEC, _5320_10G_4P, _5320_10G_8P]  # noqa: E501
+    allowable_values = [_5000_PRMR, _5000_MACSEC, _5320_10G_4P, _5320_10G_8P, _7000_PRMR]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_make.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_make.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_model.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
@@ -56,16 +56,19 @@
     _5520_48SE = "DT_5520_48SE"
     _5520_48T = "DT_5520_48T"
     _5520_48W = "DT_5520_48W"
     _5720_24MW = "DT_5720_24MW"
     _5720_24MXW = "DT_5720_24MXW"
     _5720_48MW = "DT_5720_48MW"
     _5720_48MXW = "DT_5720_48MXW"
+    _7520_48XT_6C = "DT_7520_48XT_6C"
+    _7520_48Y_8C = "DT_7520_48Y_8C"
+    _7720_32C = "DT_7720_32C"
 
-    allowable_values = [_5320_16P_4XE, _5320_16P_4XE_DC, _5320_24P_8XE, _5320_24T_8XE, _5320_48P_8XE, _5320_48T_8XE, _5420F_16MW_32P_4XE, _5420F_16W_32P_4XE, _5420F_24P_4XE, _5420F_24S_4XE, _5420F_24T_4XE, _5420F_48P_4XE, _5420F_48P_4XL, _5420F_48T_4XE, _5420F_8W_16P_4XE, _5420M_16MW_32P_4YE, _5420M_24T_4YE, _5420M_24W_4YE, _5420M_48T_4YE, _5420M_48W_4YE, _5520_12MW_36W, _5520_24T, _5520_24W, _5520_24X, _5520_48SE, _5520_48T, _5520_48W, _5720_24MW, _5720_24MXW, _5720_48MW, _5720_48MXW]  # noqa: E501
+    allowable_values = [_5320_16P_4XE, _5320_16P_4XE_DC, _5320_24P_8XE, _5320_24T_8XE, _5320_48P_8XE, _5320_48T_8XE, _5420F_16MW_32P_4XE, _5420F_16W_32P_4XE, _5420F_24P_4XE, _5420F_24S_4XE, _5420F_24T_4XE, _5420F_48P_4XE, _5420F_48P_4XL, _5420F_48T_4XE, _5420F_8W_16P_4XE, _5420M_16MW_32P_4YE, _5420M_24T_4YE, _5420M_24W_4YE, _5420M_48T_4YE, _5420M_48W_4YE, _5520_12MW_36W, _5520_24T, _5520_24W, _5520_24X, _5520_48SE, _5520_48T, _5520_48W, _5720_24MW, _5720_24MXW, _5720_48MW, _5720_48MXW, _7520_48XT_6C, _7520_48Y_8C, _7720_32C]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_products.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_products.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_digital_twin_vim_module.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_digital_twin_vim_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_duplex_data_rate_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_duplex_data_rate_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_email_log.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_email_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_email_template.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_email_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_end_user.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_end_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_entitlement_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_entitlement_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_error.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_exos_devices.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_exos_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_expiration_action_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_expiration_action_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_expiration_settings.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_expiration_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_expiration_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_expiration_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_account.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_external_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_radius_server.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_external_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_external_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user_directory.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_external_user_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user_directory_entry.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_external_user_directory_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_external_user_directory_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_external_user_directory_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_extreme_devices.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_extreme_devices.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_firmware_activate_option.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_firmware_activate_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_firmware_upgrade_policy.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_firmware_upgrade_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_flap_count_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_flap_count_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_floor.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_floor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_forensic_bucket.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_forensic_bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_generate_api_token_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_generate_api_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_generate_api_token_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_generate_api_token_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_get_port_assignment_details_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_get_port_assignment_details_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_grant_external_user_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_grant_external_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_hiq_context.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_hiq_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_hiq_status.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_hiq_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_init_key_based_pcg_network_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_initialize_location_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_initialize_location_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_device.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_internal_radius_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_server.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_internal_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_internal_radius_server_authentication_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_internal_radius_server_authentication_method_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_key_based_pcg.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_key_based_pcg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_key_based_pcg_user.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_key_based_pcg_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_key_based_pcg_user_base_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_l3_address_profile.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_l3_address_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_l3_address_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_l3_address_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ldap_protocol_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ldap_protocol_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ldap_server.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ldap_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ldap_server_verification_mode.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ldap_server_verification_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_license_mode.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_license_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_license_status.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_license_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_location.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_location_legend.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_location_legend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_location_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_location_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_login_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_login_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_login_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_login_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_measurement_unit.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_measurement_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_network_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy_field.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_network_policy_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_network_policy_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_network_policy_view.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_network_policy_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_onboard_device_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_onboard_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_onboard_key_based_pcg_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_operation_metadata.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_operation_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_operation_object.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_operation_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_operation_status.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_operation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_organization.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_organization_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_organization_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_character_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_password_character_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_db_location.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_password_db_location.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_settings.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_password_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_password_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_password_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_assign_ports_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_assign_ports_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_assign_ports_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_assign_ports_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_port_assignment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_port_assignment_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_port_assignment_entry_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_port_assignment_entry_device_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_port_assignment_entry_eth_user_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_pcg_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_sms_log_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqPcgType(object):
+class XiqSmsLogStatus(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    AP_BASED = "AP_BASED"
-    KEY_BASED = "KEY_BASED"
+    SEND_OUT = "SEND_OUT"
+    COMPLETE = "COMPLETE"
+    SUCCESS = "SUCCESS"
+    FAIL = "FAIL"
 
-    allowable_values = [AP_BASED, KEY_BASED]  # noqa: E501
+    allowable_values = [SEND_OUT, COMPLETE, SUCCESS, FAIL]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +46,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqPcgType - a model defined in OpenAPI"""  # noqa: E501
+        """XiqSmsLogStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +86,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqPcgType):
+        if not isinstance(other, XiqSmsLogStatus):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqPcgType):
+        if not isinstance(other, XiqSmsLogStatus):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_permission.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_poe_flapping_stats_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_poe_flapping_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_port_efficiency_speed_duplex_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_port_efficiency_stats_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_port_efficiency_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_post_expiration_action.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_post_expiration_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_psk_generation_method.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_psk_generation_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radio_mode.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radio_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radio_profile.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radio_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client_object.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_client_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client_object_entry.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_client_object_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_client_object_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_client_object_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_proxy.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_proxy_format_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_proxy_format_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_proxy_realm.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_radius_server_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_radius_server_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_regenerate_end_user_password_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_regenerate_end_user_password_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rf_environment_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rf_environment_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_channel_selection.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_channel_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_mac_oui_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_miscellaneous_settings.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_miscellaneous_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_neighborhood_analysis.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_neighborhood_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_radio_usage_optimization.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_radio_usage_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_sensor_scan_settings.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_sensor_scan_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_rp_wmm_qos_settings.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_rp_wmm_qos_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_send_cli_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_send_cli_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_send_cli_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_send_cli_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_server_role.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_server_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sessions_data_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_sessions_data_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_set_ssid_mode_dot1x_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_set_ssid_mode_ppsk_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_set_ssid_mode_psk_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_set_ssid_mode_wep_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sms_log.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_sms_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sms_log_status.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_subscription_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqSmsLogStatus(object):
+class XiqSubscriptionStatus(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    SEND_OUT = "SEND_OUT"
-    COMPLETE = "COMPLETE"
-    SUCCESS = "SUCCESS"
-    FAIL = "FAIL"
+    ENABLED = "ENABLED"
+    DISABLED = "DISABLED"
 
-    allowable_values = [SEND_OUT, COMPLETE, SUCCESS, FAIL]  # noqa: E501
+    allowable_values = [ENABLED, DISABLED]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -46,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqSmsLogStatus - a model defined in OpenAPI"""  # noqa: E501
+        """XiqSubscriptionStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -86,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqSmsLogStatus):
+        if not isinstance(other, XiqSubscriptionStatus):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqSmsLogStatus):
+        if not isinstance(other, XiqSubscriptionStatus):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sms_template.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_sms_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sort_field.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_sort_order.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_sort_order.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_speed_duplex_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_speed_duplex_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_dot1x_encryption_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_dot1x_key_management.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_dot1x_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_key_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_key_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_ppsk_key_management.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_ppsk_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_psk_encryption_method.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_psk_encryption_method.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_psk_key_management.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_psk_key_management.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_sae_group.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_sae_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_authentication_method.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_wep_authentication_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_default_key.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_wep_default_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_encryption_method.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_wep_encryption_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_ssid_wep_key_management.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_ssid_wep_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_subscription_data_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_subscription_data_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_subscription_message_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_subscription_message_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_subscription_status.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_trend_indicator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqSubscriptionStatus(object):
+class XiqTrendIndicator(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    ENABLED = "ENABLED"
-    DISABLED = "DISABLED"
+    UP = "UP"
+    DOWN = "DOWN"
+    EQUAL = "EQUAL"
 
-    allowable_values = [ENABLED, DISABLED]  # noqa: E501
+    allowable_values = [UP, DOWN, EQUAL]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +45,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqSubscriptionStatus - a model defined in OpenAPI"""  # noqa: E501
+        """XiqTrendIndicator - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +85,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqSubscriptionStatus):
+        if not isinstance(other, XiqTrendIndicator):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqSubscriptionStatus):
+        if not isinstance(other, XiqTrendIndicator):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_top_applications_usage.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_top_applications_usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_trend_indicator.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_views_list_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqTrendIndicator(object):
+class XiqWirelessViewsListType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UP = "UP"
-    DOWN = "DOWN"
-    EQUAL = "EQUAL"
+    SSID = "SSID"
+    OS = "OS"
 
-    allowable_values = [UP, DOWN, EQUAL]  # noqa: E501
+    allowable_values = [SSID, OS]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -45,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqTrendIndicator - a model defined in OpenAPI"""  # noqa: E501
+        """XiqWirelessViewsListType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -85,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqTrendIndicator):
+        if not isinstance(other, XiqWirelessViewsListType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqTrendIndicator):
+        if not isinstance(other, XiqWirelessViewsListType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_building_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_building_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_classification_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_classification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_classification_rule_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_classification_rule_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_cloud_config_group_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_cloud_config_group_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_device_level_ssid_status.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_device_level_ssid_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_end_user_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_end_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_external_radius_server_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_external_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_external_user_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_external_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_floor_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_floor_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_internal_radius_server_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_internal_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_key_based_pcg_users_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_ldap_server_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_ldap_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_location_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_network_policy_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_network_policy_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radio_profile_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_radio_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_client.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_radius_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_client_object_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_radius_client_object_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_proxy_realm.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_radius_proxy_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_radius_proxy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_channel_selection_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_channel_selection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_mac_oui_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_miscellaneous_settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_neighborhood_analysis_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_radio_usage_optimization_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_sensor_scan_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_rp_wmm_qos_settings_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_user_group_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_user_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_user_profile_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_user_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_user_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_vlan_object_classified_entry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_update_vlan_profile_request.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_update_vlan_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user_group.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_user_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user_profile.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_user_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_user_role.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_user_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_daily_settings.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_valid_daily_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_during_date_settings.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_valid_during_date_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_for_time_period_settings.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_valid_for_time_period_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_time_period_after_first_login.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_valid_time_period_after_first_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_valid_time_period_after_id_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_valid_time_period_after_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_valid_time_period_after_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_viq.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_viq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_viq_license.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_viq_license.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_vlan_object_classified_entry.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_vlan_object_classified_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_vlan_profile.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_vlan_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_vlan_profile_filter.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_vlan_profile_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_voss_devices.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_voss_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_webhook_subscription.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_webhook_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wifi_capacity_client_list_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wifi_capacity_client_list_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wifi_capacity_stats_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wifi_capacity_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wifi_efficiency_client_list_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wifi_efficiency_client_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wifi_efficiency_stats_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wifi_efficiency_stats_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wing_devices.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wing_devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_event_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wired_event_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_hardware_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wired_hardware_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_hardware_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wired_hardware_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_quality_index_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wired_quality_index_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wired_view_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wired_view_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_apps_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_apps_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_connectivity_performance_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_event_retries_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_event_retries_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_if_name.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_if_name.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_performance_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_performance_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_performance_retries_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_performance_retries_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_quality_index_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_quality_index_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_time_to_connect_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_time_to_connect_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_time_to_connect_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_views_list_type.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_pcg_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
 from extremecloudiq.configuration import Configuration
 
 
-class XiqWirelessViewsListType(object):
+class XiqPcgType(object):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    SSID = "SSID"
-    OS = "OS"
+    AP_BASED = "AP_BASED"
+    KEY_BASED = "KEY_BASED"
 
-    allowable_values = [SSID, OS]  # noqa: E501
+    allowable_values = [AP_BASED, KEY_BASED]  # noqa: E501
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -44,15 +44,15 @@
     openapi_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, local_vars_configuration=None):  # noqa: E501
-        """XiqWirelessViewsListType - a model defined in OpenAPI"""  # noqa: E501
+        """XiqPcgType - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -84,18 +84,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, XiqWirelessViewsListType):
+        if not isinstance(other, XiqPcgType):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, XiqWirelessViewsListType):
+        if not isinstance(other, XiqPcgType):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/models/xiq_wireless_views_type_response.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/models/xiq_wireless_views_type_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/__init__.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "23.3.2.1"
+__version__ = "23.4.0.41"
 
 # import apis into sdk package
 from extremecloudiq.api.account_api import AccountApi
 from extremecloudiq.api.alert_api import AlertApi
 from extremecloudiq.api.application_api import ApplicationApi
 from extremecloudiq.api.authentication_api import AuthenticationApi
 from extremecloudiq.api.authorization_api import AuthorizationApi
@@ -89,14 +89,16 @@
 from extremecloudiq.models.paged_xiq_wired_event_entity import PagedXiqWiredEventEntity
 from extremecloudiq.models.xiq_account import XiqAccount
 from extremecloudiq.models.xiq_account_mode import XiqAccountMode
 from extremecloudiq.models.xiq_account_type import XiqAccountType
 from extremecloudiq.models.xiq_accounting_log import XiqAccountingLog
 from extremecloudiq.models.xiq_active_directory_server import XiqActiveDirectoryServer
 from extremecloudiq.models.xiq_active_directory_server_base_dn_fetch_mode import XiqActiveDirectoryServerBaseDnFetchMode
+from extremecloudiq.models.xiq_advanced_onboard_device_request import XiqAdvancedOnboardDeviceRequest
+from extremecloudiq.models.xiq_advanced_onboard_device_response import XiqAdvancedOnboardDeviceResponse
 from extremecloudiq.models.xiq_alert import XiqAlert
 from extremecloudiq.models.xiq_alert_category import XiqAlertCategory
 from extremecloudiq.models.xiq_alert_group_query import XiqAlertGroupQuery
 from extremecloudiq.models.xiq_alert_severity import XiqAlertSeverity
 from extremecloudiq.models.xiq_alert_source import XiqAlertSource
 from extremecloudiq.models.xiq_alert_source_type import XiqAlertSourceType
 from extremecloudiq.models.xiq_anomalies_count_vo_entity import XiqAnomaliesCountVoEntity
@@ -140,14 +142,15 @@
 from extremecloudiq.models.xiq_classification import XiqClassification
 from extremecloudiq.models.xiq_classification_rule import XiqClassificationRule
 from extremecloudiq.models.xiq_classification_type import XiqClassificationType
 from extremecloudiq.models.xiq_cli_output import XiqCliOutput
 from extremecloudiq.models.xiq_cli_response_code import XiqCliResponseCode
 from extremecloudiq.models.xiq_client import XiqClient
 from extremecloudiq.models.xiq_client_field import XiqClientField
+from extremecloudiq.models.xiq_client_mac_address_alias import XiqClientMacAddressAlias
 from extremecloudiq.models.xiq_client_sort_field import XiqClientSortField
 from extremecloudiq.models.xiq_client_stats_entity import XiqClientStatsEntity
 from extremecloudiq.models.xiq_client_summary import XiqClientSummary
 from extremecloudiq.models.xiq_client_usage import XiqClientUsage
 from extremecloudiq.models.xiq_client_view import XiqClientView
 from extremecloudiq.models.xiq_cloud_config_group import XiqCloudConfigGroup
 from extremecloudiq.models.xiq_connectivity_experience_data import XiqConnectivityExperienceData
@@ -188,14 +191,15 @@
 from extremecloudiq.models.xiq_cwp import XiqCwp
 from extremecloudiq.models.xiq_data_point import XiqDataPoint
 from extremecloudiq.models.xiq_date_time_type import XiqDateTimeType
 from extremecloudiq.models.xiq_date_time_unit_type import XiqDateTimeUnitType
 from extremecloudiq.models.xiq_default_device_password import XiqDefaultDevicePassword
 from extremecloudiq.models.xiq_delete_key_based_pcg_users_request import XiqDeleteKeyBasedPcgUsersRequest
 from extremecloudiq.models.xiq_delivery_settings import XiqDeliverySettings
+from extremecloudiq.models.xiq_dell_device import XiqDellDevice
 from extremecloudiq.models.xiq_dell_devices import XiqDellDevices
 from extremecloudiq.models.xiq_deployment_overview import XiqDeploymentOverview
 from extremecloudiq.models.xiq_deployment_policy import XiqDeploymentPolicy
 from extremecloudiq.models.xiq_deployment_request import XiqDeploymentRequest
 from extremecloudiq.models.xiq_deployment_response import XiqDeploymentResponse
 from extremecloudiq.models.xiq_deployment_status import XiqDeploymentStatus
 from extremecloudiq.models.xiq_device import XiqDevice
@@ -224,33 +228,37 @@
 from extremecloudiq.models.xiq_dfs_recurence_channel_stats_response import XiqDfsRecurenceChannelStatsResponse
 from extremecloudiq.models.xiq_dfs_recurence_count_stats_response import XiqDfsRecurenceCountStatsResponse
 from extremecloudiq.models.xiq_digital_twin_device import XiqDigitalTwinDevice
 from extremecloudiq.models.xiq_digital_twin_devices import XiqDigitalTwinDevices
 from extremecloudiq.models.xiq_digital_twin_feat_license import XiqDigitalTwinFeatLicense
 from extremecloudiq.models.xiq_digital_twin_make import XiqDigitalTwinMake
 from extremecloudiq.models.xiq_digital_twin_model import XiqDigitalTwinModel
+from extremecloudiq.models.xiq_digital_twin_onboard_device import XiqDigitalTwinOnboardDevice
 from extremecloudiq.models.xiq_digital_twin_products import XiqDigitalTwinProducts
 from extremecloudiq.models.xiq_digital_twin_vim_module import XiqDigitalTwinVimModule
 from extremecloudiq.models.xiq_duplex_data_rate_entity import XiqDuplexDataRateEntity
 from extremecloudiq.models.xiq_email_log import XiqEmailLog
 from extremecloudiq.models.xiq_email_template import XiqEmailTemplate
 from extremecloudiq.models.xiq_end_user import XiqEndUser
 from extremecloudiq.models.xiq_entitlement_type import XiqEntitlementType
 from extremecloudiq.models.xiq_error import XiqError
+from extremecloudiq.models.xiq_exos_device import XiqExosDevice
 from extremecloudiq.models.xiq_exos_devices import XiqExosDevices
 from extremecloudiq.models.xiq_expiration_action_type import XiqExpirationActionType
 from extremecloudiq.models.xiq_expiration_settings import XiqExpirationSettings
 from extremecloudiq.models.xiq_expiration_type import XiqExpirationType
 from extremecloudiq.models.xiq_external_account import XiqExternalAccount
 from extremecloudiq.models.xiq_external_radius_server import XiqExternalRadiusServer
 from extremecloudiq.models.xiq_external_user import XiqExternalUser
 from extremecloudiq.models.xiq_external_user_directory import XiqExternalUserDirectory
 from extremecloudiq.models.xiq_external_user_directory_entry import XiqExternalUserDirectoryEntry
 from extremecloudiq.models.xiq_external_user_directory_type import XiqExternalUserDirectoryType
+from extremecloudiq.models.xiq_extreme_device import XiqExtremeDevice
 from extremecloudiq.models.xiq_extreme_devices import XiqExtremeDevices
+from extremecloudiq.models.xiq_failure_onboard_device import XiqFailureOnboardDevice
 from extremecloudiq.models.xiq_firmware_activate_option import XiqFirmwareActivateOption
 from extremecloudiq.models.xiq_firmware_upgrade_policy import XiqFirmwareUpgradePolicy
 from extremecloudiq.models.xiq_flap_count_entity import XiqFlapCountEntity
 from extremecloudiq.models.xiq_floor import XiqFloor
 from extremecloudiq.models.xiq_forensic_bucket import XiqForensicBucket
 from extremecloudiq.models.xiq_generate_api_token_request import XiqGenerateApiTokenRequest
 from extremecloudiq.models.xiq_generate_api_token_response import XiqGenerateApiTokenResponse
@@ -281,14 +289,15 @@
 from extremecloudiq.models.xiq_login_response import XiqLoginResponse
 from extremecloudiq.models.xiq_measurement_unit import XiqMeasurementUnit
 from extremecloudiq.models.xiq_network_policy import XiqNetworkPolicy
 from extremecloudiq.models.xiq_network_policy_field import XiqNetworkPolicyField
 from extremecloudiq.models.xiq_network_policy_type import XiqNetworkPolicyType
 from extremecloudiq.models.xiq_network_policy_view import XiqNetworkPolicyView
 from extremecloudiq.models.xiq_onboard_device_request import XiqOnboardDeviceRequest
+from extremecloudiq.models.xiq_onboard_error import XiqOnboardError
 from extremecloudiq.models.xiq_onboard_key_based_pcg_request import XiqOnboardKeyBasedPcgRequest
 from extremecloudiq.models.xiq_operation_metadata import XiqOperationMetadata
 from extremecloudiq.models.xiq_operation_object import XiqOperationObject
 from extremecloudiq.models.xiq_operation_status import XiqOperationStatus
 from extremecloudiq.models.xiq_organization import XiqOrganization
 from extremecloudiq.models.xiq_organization_type import XiqOrganizationType
 from extremecloudiq.models.xiq_password_character_type import XiqPasswordCharacterType
@@ -353,14 +362,15 @@
 from extremecloudiq.models.xiq_ssid_wep_authentication_method import XiqSsidWepAuthenticationMethod
 from extremecloudiq.models.xiq_ssid_wep_default_key import XiqSsidWepDefaultKey
 from extremecloudiq.models.xiq_ssid_wep_encryption_method import XiqSsidWepEncryptionMethod
 from extremecloudiq.models.xiq_ssid_wep_key_management import XiqSsidWepKeyManagement
 from extremecloudiq.models.xiq_subscription_data_type import XiqSubscriptionDataType
 from extremecloudiq.models.xiq_subscription_message_type import XiqSubscriptionMessageType
 from extremecloudiq.models.xiq_subscription_status import XiqSubscriptionStatus
+from extremecloudiq.models.xiq_success_onboard_device import XiqSuccessOnboardDevice
 from extremecloudiq.models.xiq_top_applications_usage import XiqTopApplicationsUsage
 from extremecloudiq.models.xiq_trend_indicator import XiqTrendIndicator
 from extremecloudiq.models.xiq_update_building_request import XiqUpdateBuildingRequest
 from extremecloudiq.models.xiq_update_classification_request import XiqUpdateClassificationRequest
 from extremecloudiq.models.xiq_update_classification_rule_request import XiqUpdateClassificationRuleRequest
 from extremecloudiq.models.xiq_update_cloud_config_group_request import XiqUpdateCloudConfigGroupRequest
 from extremecloudiq.models.xiq_update_device_level_ssid_status import XiqUpdateDeviceLevelSsidStatus
@@ -401,20 +411,22 @@
 from extremecloudiq.models.xiq_valid_time_period_after_id_creation import XiqValidTimePeriodAfterIdCreation
 from extremecloudiq.models.xiq_valid_time_period_after_type import XiqValidTimePeriodAfterType
 from extremecloudiq.models.xiq_viq import XiqViq
 from extremecloudiq.models.xiq_viq_license import XiqViqLicense
 from extremecloudiq.models.xiq_vlan_object_classified_entry import XiqVlanObjectClassifiedEntry
 from extremecloudiq.models.xiq_vlan_profile import XiqVlanProfile
 from extremecloudiq.models.xiq_vlan_profile_filter import XiqVlanProfileFilter
+from extremecloudiq.models.xiq_voss_device import XiqVossDevice
 from extremecloudiq.models.xiq_voss_devices import XiqVossDevices
 from extremecloudiq.models.xiq_webhook_subscription import XiqWebhookSubscription
 from extremecloudiq.models.xiq_wifi_capacity_client_list_response import XiqWifiCapacityClientListResponse
 from extremecloudiq.models.xiq_wifi_capacity_stats_response import XiqWifiCapacityStatsResponse
 from extremecloudiq.models.xiq_wifi_efficiency_client_list_response import XiqWifiEfficiencyClientListResponse
 from extremecloudiq.models.xiq_wifi_efficiency_stats_response import XiqWifiEfficiencyStatsResponse
+from extremecloudiq.models.xiq_wing_device import XiqWingDevice
 from extremecloudiq.models.xiq_wing_devices import XiqWingDevices
 from extremecloudiq.models.xiq_wired_event_entity import XiqWiredEventEntity
 from extremecloudiq.models.xiq_wired_hardware_entity import XiqWiredHardwareEntity
 from extremecloudiq.models.xiq_wired_hardware_response import XiqWiredHardwareResponse
 from extremecloudiq.models.xiq_wired_quality_index_response import XiqWiredQualityIndexResponse
 from extremecloudiq.models.xiq_wired_view_type import XiqWiredViewType
 from extremecloudiq.models.xiq_wireless_apps_response import XiqWirelessAppsResponse
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/api_client.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/23.3.2.1/python'
+        self.user_agent = 'OpenAPI-Generator/23.4.0.41/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/configuration.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -333,16 +333,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 23.3.2.1\n"\
-               "SDK Package Version: 23.3.2.1".\
+               "Version of the API: 23.4.0.41\n"\
+               "SDK Package Version: 23.4.0.41".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/exceptions.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq/rest.py` & `extremecloudiq-api-23.4.0.41/extremecloudiq/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/extremecloudiq_api.egg-info/SOURCES.txt` & `extremecloudiq-api-23.4.0.41/extremecloudiq_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 extremecloudiq/models/paged_xiq_wired_event_entity.py
 extremecloudiq/models/xiq_account.py
 extremecloudiq/models/xiq_account_mode.py
 extremecloudiq/models/xiq_account_type.py
 extremecloudiq/models/xiq_accounting_log.py
 extremecloudiq/models/xiq_active_directory_server.py
 extremecloudiq/models/xiq_active_directory_server_base_dn_fetch_mode.py
+extremecloudiq/models/xiq_advanced_onboard_device_request.py
+extremecloudiq/models/xiq_advanced_onboard_device_response.py
 extremecloudiq/models/xiq_alert.py
 extremecloudiq/models/xiq_alert_category.py
 extremecloudiq/models/xiq_alert_group_query.py
 extremecloudiq/models/xiq_alert_severity.py
 extremecloudiq/models/xiq_alert_source.py
 extremecloudiq/models/xiq_alert_source_type.py
 extremecloudiq/models/xiq_anomalies_count_vo_entity.py
@@ -120,14 +122,15 @@
 extremecloudiq/models/xiq_classification.py
 extremecloudiq/models/xiq_classification_rule.py
 extremecloudiq/models/xiq_classification_type.py
 extremecloudiq/models/xiq_cli_output.py
 extremecloudiq/models/xiq_cli_response_code.py
 extremecloudiq/models/xiq_client.py
 extremecloudiq/models/xiq_client_field.py
+extremecloudiq/models/xiq_client_mac_address_alias.py
 extremecloudiq/models/xiq_client_sort_field.py
 extremecloudiq/models/xiq_client_stats_entity.py
 extremecloudiq/models/xiq_client_summary.py
 extremecloudiq/models/xiq_client_usage.py
 extremecloudiq/models/xiq_client_view.py
 extremecloudiq/models/xiq_cloud_config_group.py
 extremecloudiq/models/xiq_connectivity_experience_data.py
@@ -168,14 +171,15 @@
 extremecloudiq/models/xiq_cwp.py
 extremecloudiq/models/xiq_data_point.py
 extremecloudiq/models/xiq_date_time_type.py
 extremecloudiq/models/xiq_date_time_unit_type.py
 extremecloudiq/models/xiq_default_device_password.py
 extremecloudiq/models/xiq_delete_key_based_pcg_users_request.py
 extremecloudiq/models/xiq_delivery_settings.py
+extremecloudiq/models/xiq_dell_device.py
 extremecloudiq/models/xiq_dell_devices.py
 extremecloudiq/models/xiq_deployment_overview.py
 extremecloudiq/models/xiq_deployment_policy.py
 extremecloudiq/models/xiq_deployment_request.py
 extremecloudiq/models/xiq_deployment_response.py
 extremecloudiq/models/xiq_deployment_status.py
 extremecloudiq/models/xiq_device.py
@@ -204,33 +208,37 @@
 extremecloudiq/models/xiq_dfs_recurence_channel_stats_response.py
 extremecloudiq/models/xiq_dfs_recurence_count_stats_response.py
 extremecloudiq/models/xiq_digital_twin_device.py
 extremecloudiq/models/xiq_digital_twin_devices.py
 extremecloudiq/models/xiq_digital_twin_feat_license.py
 extremecloudiq/models/xiq_digital_twin_make.py
 extremecloudiq/models/xiq_digital_twin_model.py
+extremecloudiq/models/xiq_digital_twin_onboard_device.py
 extremecloudiq/models/xiq_digital_twin_products.py
 extremecloudiq/models/xiq_digital_twin_vim_module.py
 extremecloudiq/models/xiq_duplex_data_rate_entity.py
 extremecloudiq/models/xiq_email_log.py
 extremecloudiq/models/xiq_email_template.py
 extremecloudiq/models/xiq_end_user.py
 extremecloudiq/models/xiq_entitlement_type.py
 extremecloudiq/models/xiq_error.py
+extremecloudiq/models/xiq_exos_device.py
 extremecloudiq/models/xiq_exos_devices.py
 extremecloudiq/models/xiq_expiration_action_type.py
 extremecloudiq/models/xiq_expiration_settings.py
 extremecloudiq/models/xiq_expiration_type.py
 extremecloudiq/models/xiq_external_account.py
 extremecloudiq/models/xiq_external_radius_server.py
 extremecloudiq/models/xiq_external_user.py
 extremecloudiq/models/xiq_external_user_directory.py
 extremecloudiq/models/xiq_external_user_directory_entry.py
 extremecloudiq/models/xiq_external_user_directory_type.py
+extremecloudiq/models/xiq_extreme_device.py
 extremecloudiq/models/xiq_extreme_devices.py
+extremecloudiq/models/xiq_failure_onboard_device.py
 extremecloudiq/models/xiq_firmware_activate_option.py
 extremecloudiq/models/xiq_firmware_upgrade_policy.py
 extremecloudiq/models/xiq_flap_count_entity.py
 extremecloudiq/models/xiq_floor.py
 extremecloudiq/models/xiq_forensic_bucket.py
 extremecloudiq/models/xiq_generate_api_token_request.py
 extremecloudiq/models/xiq_generate_api_token_response.py
@@ -261,14 +269,15 @@
 extremecloudiq/models/xiq_login_response.py
 extremecloudiq/models/xiq_measurement_unit.py
 extremecloudiq/models/xiq_network_policy.py
 extremecloudiq/models/xiq_network_policy_field.py
 extremecloudiq/models/xiq_network_policy_type.py
 extremecloudiq/models/xiq_network_policy_view.py
 extremecloudiq/models/xiq_onboard_device_request.py
+extremecloudiq/models/xiq_onboard_error.py
 extremecloudiq/models/xiq_onboard_key_based_pcg_request.py
 extremecloudiq/models/xiq_operation_metadata.py
 extremecloudiq/models/xiq_operation_object.py
 extremecloudiq/models/xiq_operation_status.py
 extremecloudiq/models/xiq_organization.py
 extremecloudiq/models/xiq_organization_type.py
 extremecloudiq/models/xiq_password_character_type.py
@@ -333,14 +342,15 @@
 extremecloudiq/models/xiq_ssid_wep_authentication_method.py
 extremecloudiq/models/xiq_ssid_wep_default_key.py
 extremecloudiq/models/xiq_ssid_wep_encryption_method.py
 extremecloudiq/models/xiq_ssid_wep_key_management.py
 extremecloudiq/models/xiq_subscription_data_type.py
 extremecloudiq/models/xiq_subscription_message_type.py
 extremecloudiq/models/xiq_subscription_status.py
+extremecloudiq/models/xiq_success_onboard_device.py
 extremecloudiq/models/xiq_top_applications_usage.py
 extremecloudiq/models/xiq_trend_indicator.py
 extremecloudiq/models/xiq_update_building_request.py
 extremecloudiq/models/xiq_update_classification_request.py
 extremecloudiq/models/xiq_update_classification_rule_request.py
 extremecloudiq/models/xiq_update_cloud_config_group_request.py
 extremecloudiq/models/xiq_update_device_level_ssid_status.py
@@ -381,20 +391,22 @@
 extremecloudiq/models/xiq_valid_time_period_after_id_creation.py
 extremecloudiq/models/xiq_valid_time_period_after_type.py
 extremecloudiq/models/xiq_viq.py
 extremecloudiq/models/xiq_viq_license.py
 extremecloudiq/models/xiq_vlan_object_classified_entry.py
 extremecloudiq/models/xiq_vlan_profile.py
 extremecloudiq/models/xiq_vlan_profile_filter.py
+extremecloudiq/models/xiq_voss_device.py
 extremecloudiq/models/xiq_voss_devices.py
 extremecloudiq/models/xiq_webhook_subscription.py
 extremecloudiq/models/xiq_wifi_capacity_client_list_response.py
 extremecloudiq/models/xiq_wifi_capacity_stats_response.py
 extremecloudiq/models/xiq_wifi_efficiency_client_list_response.py
 extremecloudiq/models/xiq_wifi_efficiency_stats_response.py
+extremecloudiq/models/xiq_wing_device.py
 extremecloudiq/models/xiq_wing_devices.py
 extremecloudiq/models/xiq_wired_event_entity.py
 extremecloudiq/models/xiq_wired_hardware_entity.py
 extremecloudiq/models/xiq_wired_hardware_response.py
 extremecloudiq/models/xiq_wired_quality_index_response.py
 extremecloudiq/models/xiq_wired_view_type.py
 extremecloudiq/models/xiq_wireless_apps_response.py
@@ -474,14 +486,16 @@
 test/test_user_api.py
 test/test_xiq_account.py
 test/test_xiq_account_mode.py
 test/test_xiq_account_type.py
 test/test_xiq_accounting_log.py
 test/test_xiq_active_directory_server.py
 test/test_xiq_active_directory_server_base_dn_fetch_mode.py
+test/test_xiq_advanced_onboard_device_request.py
+test/test_xiq_advanced_onboard_device_response.py
 test/test_xiq_alert.py
 test/test_xiq_alert_category.py
 test/test_xiq_alert_group_query.py
 test/test_xiq_alert_severity.py
 test/test_xiq_alert_source.py
 test/test_xiq_alert_source_type.py
 test/test_xiq_anomalies_count_vo_entity.py
@@ -525,14 +539,15 @@
 test/test_xiq_classification.py
 test/test_xiq_classification_rule.py
 test/test_xiq_classification_type.py
 test/test_xiq_cli_output.py
 test/test_xiq_cli_response_code.py
 test/test_xiq_client.py
 test/test_xiq_client_field.py
+test/test_xiq_client_mac_address_alias.py
 test/test_xiq_client_sort_field.py
 test/test_xiq_client_stats_entity.py
 test/test_xiq_client_summary.py
 test/test_xiq_client_usage.py
 test/test_xiq_client_view.py
 test/test_xiq_cloud_config_group.py
 test/test_xiq_connectivity_experience_data.py
@@ -573,14 +588,15 @@
 test/test_xiq_cwp.py
 test/test_xiq_data_point.py
 test/test_xiq_date_time_type.py
 test/test_xiq_date_time_unit_type.py
 test/test_xiq_default_device_password.py
 test/test_xiq_delete_key_based_pcg_users_request.py
 test/test_xiq_delivery_settings.py
+test/test_xiq_dell_device.py
 test/test_xiq_dell_devices.py
 test/test_xiq_deployment_overview.py
 test/test_xiq_deployment_policy.py
 test/test_xiq_deployment_request.py
 test/test_xiq_deployment_response.py
 test/test_xiq_deployment_status.py
 test/test_xiq_device.py
@@ -609,33 +625,37 @@
 test/test_xiq_dfs_recurence_channel_stats_response.py
 test/test_xiq_dfs_recurence_count_stats_response.py
 test/test_xiq_digital_twin_device.py
 test/test_xiq_digital_twin_devices.py
 test/test_xiq_digital_twin_feat_license.py
 test/test_xiq_digital_twin_make.py
 test/test_xiq_digital_twin_model.py
+test/test_xiq_digital_twin_onboard_device.py
 test/test_xiq_digital_twin_products.py
 test/test_xiq_digital_twin_vim_module.py
 test/test_xiq_duplex_data_rate_entity.py
 test/test_xiq_email_log.py
 test/test_xiq_email_template.py
 test/test_xiq_end_user.py
 test/test_xiq_entitlement_type.py
 test/test_xiq_error.py
+test/test_xiq_exos_device.py
 test/test_xiq_exos_devices.py
 test/test_xiq_expiration_action_type.py
 test/test_xiq_expiration_settings.py
 test/test_xiq_expiration_type.py
 test/test_xiq_external_account.py
 test/test_xiq_external_radius_server.py
 test/test_xiq_external_user.py
 test/test_xiq_external_user_directory.py
 test/test_xiq_external_user_directory_entry.py
 test/test_xiq_external_user_directory_type.py
+test/test_xiq_extreme_device.py
 test/test_xiq_extreme_devices.py
+test/test_xiq_failure_onboard_device.py
 test/test_xiq_firmware_activate_option.py
 test/test_xiq_firmware_upgrade_policy.py
 test/test_xiq_flap_count_entity.py
 test/test_xiq_floor.py
 test/test_xiq_forensic_bucket.py
 test/test_xiq_generate_api_token_request.py
 test/test_xiq_generate_api_token_response.py
@@ -666,14 +686,15 @@
 test/test_xiq_login_response.py
 test/test_xiq_measurement_unit.py
 test/test_xiq_network_policy.py
 test/test_xiq_network_policy_field.py
 test/test_xiq_network_policy_type.py
 test/test_xiq_network_policy_view.py
 test/test_xiq_onboard_device_request.py
+test/test_xiq_onboard_error.py
 test/test_xiq_onboard_key_based_pcg_request.py
 test/test_xiq_operation_metadata.py
 test/test_xiq_operation_object.py
 test/test_xiq_operation_status.py
 test/test_xiq_organization.py
 test/test_xiq_organization_type.py
 test/test_xiq_password_character_type.py
@@ -738,14 +759,15 @@
 test/test_xiq_ssid_wep_authentication_method.py
 test/test_xiq_ssid_wep_default_key.py
 test/test_xiq_ssid_wep_encryption_method.py
 test/test_xiq_ssid_wep_key_management.py
 test/test_xiq_subscription_data_type.py
 test/test_xiq_subscription_message_type.py
 test/test_xiq_subscription_status.py
+test/test_xiq_success_onboard_device.py
 test/test_xiq_top_applications_usage.py
 test/test_xiq_trend_indicator.py
 test/test_xiq_update_building_request.py
 test/test_xiq_update_classification_request.py
 test/test_xiq_update_classification_rule_request.py
 test/test_xiq_update_cloud_config_group_request.py
 test/test_xiq_update_device_level_ssid_status.py
@@ -786,20 +808,22 @@
 test/test_xiq_valid_time_period_after_id_creation.py
 test/test_xiq_valid_time_period_after_type.py
 test/test_xiq_viq.py
 test/test_xiq_viq_license.py
 test/test_xiq_vlan_object_classified_entry.py
 test/test_xiq_vlan_profile.py
 test/test_xiq_vlan_profile_filter.py
+test/test_xiq_voss_device.py
 test/test_xiq_voss_devices.py
 test/test_xiq_webhook_subscription.py
 test/test_xiq_wifi_capacity_client_list_response.py
 test/test_xiq_wifi_capacity_stats_response.py
 test/test_xiq_wifi_efficiency_client_list_response.py
 test/test_xiq_wifi_efficiency_stats_response.py
+test/test_xiq_wing_device.py
 test/test_xiq_wing_devices.py
 test/test_xiq_wired_event_entity.py
 test/test_xiq_wired_hardware_entity.py
 test/test_xiq_wired_hardware_response.py
 test/test_xiq_wired_quality_index_response.py
 test/test_xiq_wired_view_type.py
 test/test_xiq_wireless_apps_response.py
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_account_api.py` & `extremecloudiq-api-23.4.0.41/test/test_account_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_alert_api.py` & `extremecloudiq-api-23.4.0.41/test/test_alert_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_application_api.py` & `extremecloudiq-api-23.4.0.41/test/test_application_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_authentication_api.py` & `extremecloudiq-api-23.4.0.41/test/test_authentication_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_authorization_api.py` & `extremecloudiq-api-23.4.0.41/test/test_authorization_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_client_api.py` & `extremecloudiq-api-23.4.0.41/test/test_client_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -67,10 +67,17 @@
     def test_list_active_clients(self):
         """Test case for list_active_clients
 
         List active clients  # noqa: E501
         """
         pass
 
+    def test_set_clients_aliases(self):
+        """Test case for set_clients_aliases
+
+        Set the aliases for multiple clients  # noqa: E501
+        """
+        pass
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_configuration___authentication_api.py` & `extremecloudiq-api-23.4.0.41/test/test_configuration___authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_configuration___basic_api.py` & `extremecloudiq-api-23.4.0.41/test/test_configuration___basic_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_configuration___certificate_api.py` & `extremecloudiq-api-23.4.0.41/test/test_configuration___certificate_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_configuration___deployment_api.py` & `extremecloudiq-api-23.4.0.41/test/test_configuration___deployment_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_configuration___policy_api.py` & `extremecloudiq-api-23.4.0.41/test/test_configuration___policy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_configuration___user_management_api.py` & `extremecloudiq-api-23.4.0.41/test/test_configuration___user_management_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_copilot___anomalies_api.py` & `extremecloudiq-api-23.4.0.41/test/test_copilot___anomalies_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_copilot___connectivity_experience_api.py` & `extremecloudiq-api-23.4.0.41/test/test_copilot___connectivity_experience_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_device_api.py` & `extremecloudiq-api-23.4.0.41/test/test_device_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -25,14 +25,21 @@
 
     def setUp(self):
         self.api = extremecloudiq.api.device_api.DeviceApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
+    def test_advanced_onboard_devices(self):
+        """Test case for advanced_onboard_devices
+
+        [LRO] Advanced Onboard Devices  # noqa: E501
+        """
+        pass
+
     def test_assign_device_location(self):
         """Test case for assign_device_location
 
         Assign location to a device  # noqa: E501
         """
         pass
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_hiq_api.py` & `extremecloudiq-api-23.4.0.41/test/test_hiq_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_inline_object.py` & `extremecloudiq-api-23.4.0.41/test/test_inline_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_location_api.py` & `extremecloudiq-api-23.4.0.41/test/test_location_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_log_api.py` & `extremecloudiq-api-23.4.0.41/test/test_log_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_network_policy_api.py` & `extremecloudiq-api-23.4.0.41/test/test_network_policy_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_notification_api.py` & `extremecloudiq-api-23.4.0.41/test/test_notification_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_operation_api.py` & `extremecloudiq-api-23.4.0.41/test/test_operation_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_accounting_log.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_accounting_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_active_directory_server.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_active_directory_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_alert.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_application.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_application.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_audit_log.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_audit_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_auth_log.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_auth_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_certificate.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_certificate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_classification_rule.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_classification_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_client.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -85,15 +85,16 @@
                         port_type_name = '0', 
                         wing_ap = True, 
                         vendor = '0', 
                         locations = [
                             extremecloudiq.models.xiq_location_legend.XiqLocationLegend(
                                 id = 56, 
                                 name = '0', )
-                            ], )
+                            ], 
+                        alias = '0', )
                     ]
             )
         else :
             return PagedXiqClient(
                 page = 56,
                 count = 56,
                 total_pages = 56,
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_cloud_config_group.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_cloud_config_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_connectivity_experience_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_copilot_wireless_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_credential_log.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_credential_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_cwp.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_cwp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_device.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_device_alarm.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_device_alarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_digital_twin_products.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_digital_twin_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_email_log.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_email_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_end_user.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_end_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_external_radius_server.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_external_radius_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_external_user.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_external_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_internal_radius_device.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_internal_radius_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_internal_radius_server.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_internal_radius_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_ldap_server.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_ldap_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_network_policy.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_network_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_radio_profile.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_radio_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_radius_client_object.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_radius_client_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_radius_proxy.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_radius_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_rp_mac_oui_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_sms_log.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_sms_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_ssid.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_ssid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_user.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_user_group.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_user_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_user_profile.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_user_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_vlan_profile.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_vlan_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_paged_xiq_wired_event_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_paged_xiq_wired_event_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_user_api.py` & `extremecloudiq-api-23.4.0.41/test/test_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_account.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_account_mode.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_account_mode.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_account_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_account_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_accounting_log.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_accounting_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_active_directory_server.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_active_directory_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_active_directory_server_base_dn_fetch_mode.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_active_directory_server_base_dn_fetch_mode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_alert.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_alert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_alert_category.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_date_time_unit_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_alert_category import XiqAlertCategory  # noqa: E501
+from extremecloudiq.models.xiq_date_time_unit_type import XiqDateTimeUnitType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqAlertCategory(unittest.TestCase):
-    """XiqAlertCategory unit test stubs"""
+class TestXiqDateTimeUnitType(unittest.TestCase):
+    """XiqDateTimeUnitType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqAlertCategory
+        """Test XiqDateTimeUnitType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_alert_category.XiqAlertCategory()  # noqa: E501
+        # model = extremecloudiq.models.xiq_date_time_unit_type.XiqDateTimeUnitType()  # noqa: E501
         if include_optional :
-            return XiqAlertCategory(
+            return XiqDateTimeUnitType(
             )
         else :
-            return XiqAlertCategory(
+            return XiqDateTimeUnitType(
         )
 
-    def testXiqAlertCategory(self):
-        """Test XiqAlertCategory"""
+    def testXiqDateTimeUnitType(self):
+        """Test XiqDateTimeUnitType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_alert_group_query.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_alert_group_query.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_alert_severity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_alert_severity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_alert_source.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_alert_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_alert_source_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_alert_source_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_anomalies_count_vo_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_anomalies_count_vo_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_device_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_device_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_devices_by_location_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_devices_by_location_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_health_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_sort_field.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_anomaly_health_type import XiqAnomalyHealthType  # noqa: E501
+from extremecloudiq.models.xiq_anomaly_sort_field import XiqAnomalySortField  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqAnomalyHealthType(unittest.TestCase):
-    """XiqAnomalyHealthType unit test stubs"""
+class TestXiqAnomalySortField(unittest.TestCase):
+    """XiqAnomalySortField unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqAnomalyHealthType
+        """Test XiqAnomalySortField
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_anomaly_health_type.XiqAnomalyHealthType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_anomaly_sort_field.XiqAnomalySortField()  # noqa: E501
         if include_optional :
-            return XiqAnomalyHealthType(
+            return XiqAnomalySortField(
             )
         else :
-            return XiqAnomalyHealthType(
+            return XiqAnomalySortField(
         )
 
-    def testXiqAnomalyHealthType(self):
-        """Test XiqAnomalyHealthType"""
+    def testXiqAnomalySortField(self):
+        """Test XiqAnomalySortField"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_location_entity.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_severity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_severity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_sort_field.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_anomaly_sort_field import XiqAnomalySortField  # noqa: E501
+from extremecloudiq.models.xiq_anomaly_type import XiqAnomalyType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqAnomalySortField(unittest.TestCase):
-    """XiqAnomalySortField unit test stubs"""
+class TestXiqAnomalyType(unittest.TestCase):
+    """XiqAnomalyType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqAnomalySortField
+        """Test XiqAnomalyType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_anomaly_sort_field.XiqAnomalySortField()  # noqa: E501
+        # model = extremecloudiq.models.xiq_anomaly_type.XiqAnomalyType()  # noqa: E501
         if include_optional :
-            return XiqAnomalySortField(
+            return XiqAnomalyType(
             )
         else :
-            return XiqAnomalySortField(
+            return XiqAnomalyType(
         )
 
-    def testXiqAnomalySortField(self):
-        """Test XiqAnomalySortField"""
+    def testXiqAnomalyType(self):
+        """Test XiqAnomalyType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_anomaly_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_country_code.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_anomaly_type import XiqAnomalyType  # noqa: E501
+from extremecloudiq.models.xiq_country_code import XiqCountryCode  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqAnomalyType(unittest.TestCase):
-    """XiqAnomalyType unit test stubs"""
+class TestXiqCountryCode(unittest.TestCase):
+    """XiqCountryCode unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqAnomalyType
+        """Test XiqCountryCode
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_anomaly_type.XiqAnomalyType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_country_code.XiqCountryCode()  # noqa: E501
         if include_optional :
-            return XiqAnomalyType(
+            return XiqCountryCode(
             )
         else :
-            return XiqAnomalyType(
+            return XiqCountryCode(
         )
 
-    def testXiqAnomalyType(self):
-        """Test XiqAnomalyType"""
+    def testXiqCountryCode(self):
+        """Test XiqCountryCode"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_api_token_info.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_api_token_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_application.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_application.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_application_detection_protocol.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_application_detection_protocol.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_application_detection_rule.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_application_detection_rule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_application_detection_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_application_detection_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_application_sort_field.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_application_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_application_top_clients_usage.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_application_top_clients_usage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_assign_devices_location_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_assign_devices_location_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_assign_devices_country_code_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_assign_devices_country_code_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_assign_devices_network_policy_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_assign_devices_network_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_assurance_scans_overview_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_assurance_scans_overview_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_atp_device_stats_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_atp_device_stats_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_atp_device_stats_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_atp_device_stats_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_atp_packet_counts_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_atp_packet_counts_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_atp_packet_counts_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_atp_packet_counts_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_audit_log.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_audit_log.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_audit_log_category.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_audit_log_category.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_audit_log_sort_field.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_audit_log_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_auth_log.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_auth_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_data.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_bounce_device_port_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_operation_result.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_bounce_device_port_operation_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_bounce_device_port_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_bounce_device_port_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_bounce_device_port_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_building.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_building.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_certificate.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_certificate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_certificate_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_certificate_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_change_devices_ibeacon_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_change_devices_ibeacon_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_change_devices_os_mode_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_change_devices_os_mode_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_check_permission_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_check_permission_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_check_permission_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_check_permission_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_classification.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_classification.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_classification_rule.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_classification_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_classification_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_classification_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_cli_output.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_cli_output.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_cli_response_code.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_cli_response_code.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_client.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -79,15 +79,16 @@
                 port_type_name = '0', 
                 wing_ap = True, 
                 vendor = '0', 
                 locations = [
                     extremecloudiq.models.xiq_location_legend.XiqLocationLegend(
                         id = 56, 
                         name = '0', )
-                    ]
+                    ], 
+                alias = '0'
             )
         else :
             return XiqClient(
                 id = 56,
                 create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
         )
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_client_field.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_client_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_client_sort_field.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_client_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_client_stats_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_client_stats_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_client_summary.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_client_summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_client_usage.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_client_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_client_view.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_view.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_client_view import XiqClientView  # noqa: E501
+from extremecloudiq.models.xiq_device_view import XiqDeviceView  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqClientView(unittest.TestCase):
-    """XiqClientView unit test stubs"""
+class TestXiqDeviceView(unittest.TestCase):
+    """XiqDeviceView unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqClientView
+        """Test XiqDeviceView
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_client_view.XiqClientView()  # noqa: E501
+        # model = extremecloudiq.models.xiq_device_view.XiqDeviceView()  # noqa: E501
         if include_optional :
-            return XiqClientView(
+            return XiqDeviceView(
             )
         else :
-            return XiqClientView(
+            return XiqDeviceView(
         )
 
-    def testXiqClientView(self):
-        """Test XiqClientView"""
+    def testXiqDeviceView(self):
+        """Test XiqDeviceView"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_cloud_config_group.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_cloud_config_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_connectivity_experience_data.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_connectivity_experience_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_connectivity_experience_view_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_connectivity_experience_view_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_events_wired_sort_field.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_copilot_events_wired_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_events_wireless_sort_field.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_copilot_events_wireless_sort_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_copilot_paged_xiq_anomaly_location_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_wired_events_score_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_copilot_wired_events_score_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_wireless_event.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_copilot_wireless_event.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_copilot_wireless_events_score_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_copilot_wireless_events_score_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_country_code.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_server_role.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_country_code import XiqCountryCode  # noqa: E501
+from extremecloudiq.models.xiq_server_role import XiqServerRole  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqCountryCode(unittest.TestCase):
-    """XiqCountryCode unit test stubs"""
+class TestXiqServerRole(unittest.TestCase):
+    """XiqServerRole unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqCountryCode
+        """Test XiqServerRole
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_country_code.XiqCountryCode()  # noqa: E501
+        # model = extremecloudiq.models.xiq_server_role.XiqServerRole()  # noqa: E501
         if include_optional :
-            return XiqCountryCode(
+            return XiqServerRole(
             )
         else :
-            return XiqCountryCode(
+            return XiqServerRole(
         )
 
-    def testXiqCountryCode(self):
-        """Test XiqCountryCode"""
+    def testXiqServerRole(self):
+        """Test XiqServerRole"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_building_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_building_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_classification_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_classification_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_classification_rule_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_classification_rule_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_cloud_config_group_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_cloud_config_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_end_user_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_end_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_external_radius_server_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_external_radius_server_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_floor_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_floor_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_internal_radius_server_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_internal_radius_server_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_key_based_pcg_users_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_key_based_pcg_users_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_ldap_server_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_ldap_server_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_location_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_location_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_network_policy_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_network_policy_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_organization_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_organization_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_radio_profile_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_radio_profile_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_client.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_radius_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_client_object_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_radius_client_object_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_proxy_realm.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_radius_proxy_realm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_radius_proxy_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_radius_proxy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_rp_mac_oui_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_user_group_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_user_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_user_profile_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_user_profile_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_user_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_vlan_object_classified_entry_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_vlan_profile_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_vlan_profile_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_create_webhook_subscription_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_create_webhook_subscription_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_credential_log.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_credential_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_cwp.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_cwp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_data_point.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_data_point.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_date_time_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_date_time_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_date_time_unit_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_function.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_date_time_unit_type import XiqDateTimeUnitType  # noqa: E501
+from extremecloudiq.models.xiq_device_function import XiqDeviceFunction  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqDateTimeUnitType(unittest.TestCase):
-    """XiqDateTimeUnitType unit test stubs"""
+class TestXiqDeviceFunction(unittest.TestCase):
+    """XiqDeviceFunction unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqDateTimeUnitType
+        """Test XiqDeviceFunction
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_date_time_unit_type.XiqDateTimeUnitType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_device_function.XiqDeviceFunction()  # noqa: E501
         if include_optional :
-            return XiqDateTimeUnitType(
+            return XiqDeviceFunction(
             )
         else :
-            return XiqDateTimeUnitType(
+            return XiqDeviceFunction(
         )
 
-    def testXiqDateTimeUnitType(self):
-        """Test XiqDateTimeUnitType"""
+    def testXiqDeviceFunction(self):
+        """Test XiqDeviceFunction"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_default_device_password.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_default_device_password.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_delete_key_based_pcg_users_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_delete_key_based_pcg_users_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_delivery_settings.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_delivery_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_dell_devices.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_dell_devices.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_overview.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_deployment_overview.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_policy.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_deployment_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_deployment_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_deployment_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_deployment_status.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_deployment_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_admin_state.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_admin_state.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_alarm.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_alarm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_cpu_memory_usage.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_cpu_memory_usage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_field.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_filter.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_function.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_vlan_profile_filter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_device_function import XiqDeviceFunction  # noqa: E501
+from extremecloudiq.models.xiq_vlan_profile_filter import XiqVlanProfileFilter  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqDeviceFunction(unittest.TestCase):
-    """XiqDeviceFunction unit test stubs"""
+class TestXiqVlanProfileFilter(unittest.TestCase):
+    """XiqVlanProfileFilter unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqDeviceFunction
+        """Test XiqVlanProfileFilter
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_device_function.XiqDeviceFunction()  # noqa: E501
+        # model = extremecloudiq.models.xiq_vlan_profile_filter.XiqVlanProfileFilter()  # noqa: E501
         if include_optional :
-            return XiqDeviceFunction(
+            return XiqVlanProfileFilter(
+                ids = [
+                    56
+                    ]
             )
         else :
-            return XiqDeviceFunction(
+            return XiqVlanProfileFilter(
         )
 
-    def testXiqDeviceFunction(self):
-        """Test XiqDeviceFunction"""
+    def testXiqVlanProfileFilter(self):
+        """Test XiqVlanProfileFilter"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_ibeacon.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_ibeacon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_installation_report.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_installation_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_level_ssid.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_level_ssid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_level_ssid_status.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_level_ssid_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_lldp_cdp_info.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_lldp_cdp_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_location.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_location.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_location_assignment.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_location_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_null_field.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_null_field.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_sort_field.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_stats.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_stats_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_stats_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_view.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_expiration_type.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_device_view import XiqDeviceView  # noqa: E501
+from extremecloudiq.models.xiq_expiration_type import XiqExpirationType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqDeviceView(unittest.TestCase):
-    """XiqDeviceView unit test stubs"""
+class TestXiqExpirationType(unittest.TestCase):
+    """XiqExpirationType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqDeviceView
+        """Test XiqExpirationType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_device_view.XiqDeviceView()  # noqa: E501
+        # model = extremecloudiq.models.xiq_expiration_type.XiqExpirationType()  # noqa: E501
         if include_optional :
-            return XiqDeviceView(
+            return XiqExpirationType(
             )
         else :
-            return XiqDeviceView(
+            return XiqExpirationType(
         )
 
-    def testXiqDeviceView(self):
-        """Test XiqDeviceView"""
+    def testXiqExpirationType(self):
+        """Test XiqExpirationType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_device_wifi_interface.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_device_wifi_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_channel_changes_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_dfs_channel_changes_entity.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_channel_stats_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_dfs_channel_stats_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_recurence_channel_stats_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_dfs_recurence_channel_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_dfs_recurence_count_stats_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_dfs_recurence_count_stats_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_device.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_devices.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_devices.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_feat_license.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_feat_license.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_make.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_make.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_model.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_products.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_products.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_digital_twin_vim_module.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_digital_twin_vim_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_duplex_data_rate_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_duplex_data_rate_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_email_log.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_email_log.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_email_template.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_email_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_end_user.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_end_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_entitlement_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_entitlement_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_error.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_exos_devices.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_exos_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_expiration_action_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_expiration_action_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_expiration_settings.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_expiration_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_expiration_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_generate_api_token_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_expiration_type import XiqExpirationType  # noqa: E501
+from extremecloudiq.models.xiq_generate_api_token_request import XiqGenerateApiTokenRequest  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqExpirationType(unittest.TestCase):
-    """XiqExpirationType unit test stubs"""
+class TestXiqGenerateApiTokenRequest(unittest.TestCase):
+    """XiqGenerateApiTokenRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqExpirationType
+        """Test XiqGenerateApiTokenRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_expiration_type.XiqExpirationType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_generate_api_token_request.XiqGenerateApiTokenRequest()  # noqa: E501
         if include_optional :
-            return XiqExpirationType(
+            return XiqGenerateApiTokenRequest(
+                expire_time = 56, 
+                description = '0', 
+                permissions = [
+                    '0'
+                    ]
             )
         else :
-            return XiqExpirationType(
+            return XiqGenerateApiTokenRequest(
+                permissions = [
+                    '0'
+                    ],
         )
 
-    def testXiqExpirationType(self):
-        """Test XiqExpirationType"""
+    def testXiqGenerateApiTokenRequest(self):
+        """Test XiqGenerateApiTokenRequest"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_external_account.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_external_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_external_radius_server.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_external_radius_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_external_user.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_external_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_external_user_directory.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_external_user_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_external_user_directory_entry.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_external_user_directory_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_external_user_directory_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_external_user_directory_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_extreme_devices.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_extreme_devices.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_firmware_activate_option.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_firmware_activate_option.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_firmware_upgrade_policy.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_firmware_upgrade_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_flap_count_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_flap_count_entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_floor.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_floor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_forensic_bucket.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_forensic_bucket.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_generate_api_token_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_generate_api_token_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,68 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_generate_api_token_request import XiqGenerateApiTokenRequest  # noqa: E501
+from extremecloudiq.models.xiq_generate_api_token_response import XiqGenerateApiTokenResponse  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqGenerateApiTokenRequest(unittest.TestCase):
-    """XiqGenerateApiTokenRequest unit test stubs"""
+class TestXiqGenerateApiTokenResponse(unittest.TestCase):
+    """XiqGenerateApiTokenResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqGenerateApiTokenRequest
+        """Test XiqGenerateApiTokenResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_generate_api_token_request.XiqGenerateApiTokenRequest()  # noqa: E501
+        # model = extremecloudiq.models.xiq_generate_api_token_response.XiqGenerateApiTokenResponse()  # noqa: E501
         if include_optional :
-            return XiqGenerateApiTokenRequest(
-                expire_time = 56, 
+            return XiqGenerateApiTokenResponse(
+                access_token = '0', 
+                create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                expire_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                creator_id = 56, 
+                customer_id = 56, 
                 description = '0', 
                 permissions = [
                     '0'
                     ]
             )
         else :
-            return XiqGenerateApiTokenRequest(
+            return XiqGenerateApiTokenResponse(
+                access_token = '0',
+                create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                creator_id = 56,
+                customer_id = 56,
                 permissions = [
                     '0'
                     ],
         )
 
-    def testXiqGenerateApiTokenRequest(self):
-        """Test XiqGenerateApiTokenRequest"""
+    def testXiqGenerateApiTokenResponse(self):
+        """Test XiqGenerateApiTokenResponse"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_generate_api_token_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ssid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,66 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_generate_api_token_response import XiqGenerateApiTokenResponse  # noqa: E501
+from extremecloudiq.models.xiq_ssid import XiqSsid  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqGenerateApiTokenResponse(unittest.TestCase):
-    """XiqGenerateApiTokenResponse unit test stubs"""
+class TestXiqSsid(unittest.TestCase):
+    """XiqSsid unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqGenerateApiTokenResponse
+        """Test XiqSsid
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_generate_api_token_response.XiqGenerateApiTokenResponse()  # noqa: E501
+        # model = extremecloudiq.models.xiq_ssid.XiqSsid()  # noqa: E501
         if include_optional :
-            return XiqGenerateApiTokenResponse(
-                access_token = '0', 
+            return XiqSsid(
+                id = 56, 
                 create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                expire_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                creator_id = 56, 
-                customer_id = 56, 
+                update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                org_id = 56, 
+                name = '0', 
+                broadcast_name = '0', 
                 description = '0', 
-                permissions = [
-                    '0'
-                    ]
+                predefined = True
             )
         else :
-            return XiqGenerateApiTokenResponse(
-                access_token = '0',
+            return XiqSsid(
+                id = 56,
                 create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                creator_id = 56,
-                customer_id = 56,
-                permissions = [
-                    '0'
-                    ],
+                update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                name = '0',
+                broadcast_name = '0',
+                predefined = True,
         )
 
-    def testXiqGenerateApiTokenResponse(self):
-        """Test XiqGenerateApiTokenResponse"""
+    def testXiqSsid(self):
+        """Test XiqSsid"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_get_port_assignment_details_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_get_port_assignment_details_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_grant_external_user_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_grant_external_user_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_hiq_context.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_hiq_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_hiq_status.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_hiq_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_init_key_based_pcg_network_policy_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_init_key_based_pcg_network_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_initialize_location_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_initialize_location_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_device.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_internal_radius_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_server.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_internal_radius_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_server_authentication_method.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_internal_radius_server_authentication_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_internal_radius_server_authentication_method_group.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_internal_radius_server_authentication_method_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_key_based_pcg.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_key_based_pcg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_key_based_pcg_user.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_key_based_pcg_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_key_based_pcg_user_base_info.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_key_based_pcg_user_base_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_l3_address_profile.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_l3_address_profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_l3_address_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_l3_address_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ldap_protocol_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ldap_protocol_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ldap_server.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ldap_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ldap_server_verification_mode.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ldap_server_verification_mode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_license_mode.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_license_mode.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_license_status.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_license_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_location.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_location.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_location_legend.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_location_legend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_location_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_location_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_login_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_login_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_login_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_login_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_measurement_unit.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_measurement_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_network_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy_field.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_network_policy_field.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_network_policy_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_network_policy_view.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_network_policy_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_onboard_device_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_onboard_device_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_onboard_key_based_pcg_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_onboard_key_based_pcg_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_operation_metadata.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_operation_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_operation_object.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_operation_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_operation_status.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_operation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_organization.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_organization_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_organization_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_password_character_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_password_character_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_password_db_location.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_password_db_location.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_password_settings.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_password_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_password_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_radius_proxy_format_type.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_password_type import XiqPasswordType  # noqa: E501
+from extremecloudiq.models.xiq_radius_proxy_format_type import XiqRadiusProxyFormatType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqPasswordType(unittest.TestCase):
-    """XiqPasswordType unit test stubs"""
+class TestXiqRadiusProxyFormatType(unittest.TestCase):
+    """XiqRadiusProxyFormatType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqPasswordType
+        """Test XiqRadiusProxyFormatType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_password_type.XiqPasswordType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_radius_proxy_format_type.XiqRadiusProxyFormatType()  # noqa: E501
         if include_optional :
-            return XiqPasswordType(
+            return XiqRadiusProxyFormatType(
             )
         else :
-            return XiqPasswordType(
+            return XiqRadiusProxyFormatType(
         )
 
-    def testXiqPasswordType(self):
-        """Test XiqPasswordType"""
+    def testXiqRadiusProxyFormatType(self):
+        """Test XiqRadiusProxyFormatType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_assign_ports_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_assign_ports_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_assign_ports_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_assign_ports_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_port_assignment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_port_assignment_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry_detail.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_port_assignment_entry_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry_device_meta.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_port_assignment_entry_device_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_pcg_port_assignment_entry_eth_user_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_permission.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_permission.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_poe_flapping_stats_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_poe_flapping_stats_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_port_efficiency_speed_duplex_stats_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_port_efficiency_speed_duplex_stats_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_port_efficiency_stats_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_port_efficiency_stats_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_post_expiration_action.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_post_expiration_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_psk_generation_method.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_psk_generation_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_radio_mode.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_sort_order.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_radio_mode import XiqRadioMode  # noqa: E501
+from extremecloudiq.models.xiq_sort_order import XiqSortOrder  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqRadioMode(unittest.TestCase):
-    """XiqRadioMode unit test stubs"""
+class TestXiqSortOrder(unittest.TestCase):
+    """XiqSortOrder unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqRadioMode
+        """Test XiqSortOrder
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_radio_mode.XiqRadioMode()  # noqa: E501
+        # model = extremecloudiq.models.xiq_sort_order.XiqSortOrder()  # noqa: E501
         if include_optional :
-            return XiqRadioMode(
+            return XiqSortOrder(
             )
         else :
-            return XiqRadioMode(
+            return XiqSortOrder(
         )
 
-    def testXiqRadioMode(self):
-        """Test XiqRadioMode"""
+    def testXiqSortOrder(self):
+        """Test XiqSortOrder"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_radio_profile.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_radio_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_radius_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client_object.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_radius_client_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client_object_entry.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_radius_client_object_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_client_object_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_radius_client_object_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_proxy.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_radius_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_proxy_format_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wired_view_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_radius_proxy_format_type import XiqRadiusProxyFormatType  # noqa: E501
+from extremecloudiq.models.xiq_wired_view_type import XiqWiredViewType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqRadiusProxyFormatType(unittest.TestCase):
-    """XiqRadiusProxyFormatType unit test stubs"""
+class TestXiqWiredViewType(unittest.TestCase):
+    """XiqWiredViewType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqRadiusProxyFormatType
+        """Test XiqWiredViewType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_radius_proxy_format_type.XiqRadiusProxyFormatType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_wired_view_type.XiqWiredViewType()  # noqa: E501
         if include_optional :
-            return XiqRadiusProxyFormatType(
+            return XiqWiredViewType(
             )
         else :
-            return XiqRadiusProxyFormatType(
+            return XiqWiredViewType(
         )
 
-    def testXiqRadiusProxyFormatType(self):
-        """Test XiqRadiusProxyFormatType"""
+    def testXiqWiredViewType(self):
+        """Test XiqWiredViewType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_proxy_realm.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_radius_server_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_radius_server_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_regenerate_end_user_password_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_regenerate_end_user_password_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_rf_environment_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_rf_environment_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_channel_selection.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_rp_channel_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_mac_oui_profile.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_rp_mac_oui_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_miscellaneous_settings.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_rp_miscellaneous_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_neighborhood_analysis.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_rp_neighborhood_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_radio_usage_optimization.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_rp_radio_usage_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_sensor_scan_settings.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_rp_sensor_scan_settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_rp_wmm_qos_settings.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_rp_wmm_qos_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_send_cli_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_send_cli_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_send_cli_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_send_cli_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_server_role.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_user_role.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_server_role import XiqServerRole  # noqa: E501
+from extremecloudiq.models.xiq_user_role import XiqUserRole  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqServerRole(unittest.TestCase):
-    """XiqServerRole unit test stubs"""
+class TestXiqUserRole(unittest.TestCase):
+    """XiqUserRole unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqServerRole
+        """Test XiqUserRole
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_server_role.XiqServerRole()  # noqa: E501
+        # model = extremecloudiq.models.xiq_user_role.XiqUserRole()  # noqa: E501
         if include_optional :
-            return XiqServerRole(
+            return XiqUserRole(
             )
         else :
-            return XiqServerRole(
+            return XiqUserRole(
         )
 
-    def testXiqServerRole(self):
-        """Test XiqServerRole"""
+    def testXiqUserRole(self):
+        """Test XiqUserRole"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_sessions_data_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_sessions_data_entity.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_dot1x_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_set_ssid_mode_dot1x_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_ppsk_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_set_ssid_mode_ppsk_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_psk_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_set_ssid_mode_psk_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_set_ssid_mode_wep_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_set_ssid_mode_wep_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_sms_log.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_sms_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_sms_log_status.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_sms_log_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_sms_template.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_sms_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_sort_field.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_sort_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_sort_order.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_speed_duplex_entity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_sort_order import XiqSortOrder  # noqa: E501
+from extremecloudiq.models.xiq_speed_duplex_entity import XiqSpeedDuplexEntity  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqSortOrder(unittest.TestCase):
-    """XiqSortOrder unit test stubs"""
+class TestXiqSpeedDuplexEntity(unittest.TestCase):
+    """XiqSpeedDuplexEntity unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqSortOrder
+        """Test XiqSpeedDuplexEntity
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_sort_order.XiqSortOrder()  # noqa: E501
+        # model = extremecloudiq.models.xiq_speed_duplex_entity.XiqSpeedDuplexEntity()  # noqa: E501
         if include_optional :
-            return XiqSortOrder(
+            return XiqSpeedDuplexEntity(
+                timestamp = 56, 
+                speed_value = 56, 
+                duplex_value = 56
             )
         else :
-            return XiqSortOrder(
+            return XiqSpeedDuplexEntity(
+                timestamp = 56,
         )
 
-    def testXiqSortOrder(self):
-        """Test XiqSortOrder"""
+    def testXiqSpeedDuplexEntity(self):
+        """Test XiqSpeedDuplexEntity"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_speed_duplex_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wing_device.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,64 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_speed_duplex_entity import XiqSpeedDuplexEntity  # noqa: E501
+from extremecloudiq.models.xiq_wing_device import XiqWingDevice  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqSpeedDuplexEntity(unittest.TestCase):
-    """XiqSpeedDuplexEntity unit test stubs"""
+class TestXiqWingDevice(unittest.TestCase):
+    """XiqWingDevice unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqSpeedDuplexEntity
+        """Test XiqWingDevice
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_speed_duplex_entity.XiqSpeedDuplexEntity()  # noqa: E501
+        # model = extremecloudiq.models.xiq_wing_device.XiqWingDevice()  # noqa: E501
         if include_optional :
-            return XiqSpeedDuplexEntity(
-                timestamp = 56, 
-                speed_value = 56, 
-                duplex_value = 56
+            return XiqWingDevice(
+                serial_number = '0', 
+                mac_address = '0', 
+                location = extremecloudiq.models.xiq_device_location_assignment.XiqDeviceLocationAssignment(
+                    location_id = 56, 
+                    x = 1.337, 
+                    y = 1.337, 
+                    latitude = 1.337, 
+                    longitude = 1.337, ), 
+                network_policy_id = 56, 
+                hostname = '0'
             )
         else :
-            return XiqSpeedDuplexEntity(
-                timestamp = 56,
+            return XiqWingDevice(
+                serial_number = '0',
+                mac_address = '0',
         )
 
-    def testXiqSpeedDuplexEntity(self):
-        """Test XiqSpeedDuplexEntity"""
+    def testXiqWingDevice(self):
+        """Test XiqWingDevice"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_viq_license.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_ssid import XiqSsid  # noqa: E501
+from extremecloudiq.models.xiq_viq_license import XiqViqLicense  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqSsid(unittest.TestCase):
-    """XiqSsid unit test stubs"""
+class TestXiqViqLicense(unittest.TestCase):
+    """XiqViqLicense unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqSsid
+        """Test XiqViqLicense
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_ssid.XiqSsid()  # noqa: E501
+        # model = extremecloudiq.models.xiq_viq_license.XiqViqLicense()  # noqa: E501
         if include_optional :
-            return XiqSsid(
+            return XiqViqLicense(
                 id = 56, 
                 create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                 update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                org_id = 56, 
-                name = '0', 
-                broadcast_name = '0', 
-                description = '0', 
-                predefined = True
+                status = 'BUY', 
+                active_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                expire_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                entitlement_key = '0', 
+                entitlement_type = 'EVALUATION', 
+                mode = 'BUY', 
+                devices = 56, 
+                activated = 56, 
+                available = 56, 
+                license_type = '0'
             )
         else :
-            return XiqSsid(
+            return XiqViqLicense(
                 id = 56,
                 create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
                 update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                name = '0',
-                broadcast_name = '0',
-                predefined = True,
         )
 
-    def testXiqSsid(self):
-        """Test XiqSsid"""
+    def testXiqViqLicense(self):
+        """Test XiqViqLicense"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_dot1x_encryption_method.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_dot1x_encryption_method.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_dot1x_key_management.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_dot1x_key_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_key_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_key_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_ppsk_key_management.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_ppsk_key_management.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_psk_encryption_method.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_psk_encryption_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_psk_key_management.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_psk_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_sae_group.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_sae_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_authentication_method.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_wep_authentication_method.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_default_key.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_wep_default_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_encryption_method.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_wep_encryption_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_ssid_wep_key_management.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_ssid_wep_key_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_subscription_data_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_subscription_data_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_subscription_message_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_subscription_message_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_subscription_status.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_subscription_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_top_applications_usage.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_top_applications_usage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_trend_indicator.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_trend_indicator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_building_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_building_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_classification_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_classification_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_device_level_ssid_status.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_device_level_ssid_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_classification_rule_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_classification_rule_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_cloud_config_group_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_cloud_config_group_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_end_user_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_end_user_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_external_radius_server_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_external_radius_server_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_external_user_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_external_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_floor_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_floor_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_internal_radius_server_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_internal_radius_server_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_key_based_pcg_users_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_key_based_pcg_users_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_ldap_server_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_ldap_server_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_location_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_location_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_network_policy_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_network_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_radio_profile_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_radio_profile_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_client.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_radius_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_client_object_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_radius_client_object_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_proxy_realm.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_radius_proxy_realm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_radius_proxy_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_radius_proxy_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_channel_selection_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_channel_selection_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_mac_oui_profile_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_mac_oui_profile_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_miscellaneous_settings_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_miscellaneous_settings_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_neighborhood_analysis_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_neighborhood_analysis_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_radio_usage_optimization_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_radio_usage_optimization_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_sensor_scan_settings_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_sensor_scan_settings_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_rp_wmm_qos_settings_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_rp_wmm_qos_settings_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_user_group_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_user_group_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_user_profile_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_user_profile_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_user_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_user_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_vlan_object_classified_entry_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_vlan_object_classified_entry_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_update_vlan_profile_request.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_update_vlan_profile_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_user.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_user_group.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_user_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_user_profile.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_user_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_user_role.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_alert_category.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_user_role import XiqUserRole  # noqa: E501
+from extremecloudiq.models.xiq_alert_category import XiqAlertCategory  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqUserRole(unittest.TestCase):
-    """XiqUserRole unit test stubs"""
+class TestXiqAlertCategory(unittest.TestCase):
+    """XiqAlertCategory unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqUserRole
+        """Test XiqAlertCategory
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_user_role.XiqUserRole()  # noqa: E501
+        # model = extremecloudiq.models.xiq_alert_category.XiqAlertCategory()  # noqa: E501
         if include_optional :
-            return XiqUserRole(
+            return XiqAlertCategory(
             )
         else :
-            return XiqUserRole(
+            return XiqAlertCategory(
         )
 
-    def testXiqUserRole(self):
-        """Test XiqUserRole"""
+    def testXiqAlertCategory(self):
+        """Test XiqAlertCategory"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_valid_daily_settings.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_valid_daily_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_valid_during_date_settings.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_valid_during_date_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_valid_for_time_period_settings.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_valid_for_time_period_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_valid_time_period_after_first_login.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_valid_time_period_after_first_login.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_valid_time_period_after_id_creation.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_valid_time_period_after_id_creation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_valid_time_period_after_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_valid_time_period_after_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_viq.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_viq.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_viq_license.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_failure_onboard_device.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,55 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_viq_license import XiqViqLicense  # noqa: E501
+from extremecloudiq.models.xiq_failure_onboard_device import XiqFailureOnboardDevice  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqViqLicense(unittest.TestCase):
-    """XiqViqLicense unit test stubs"""
+class TestXiqFailureOnboardDevice(unittest.TestCase):
+    """XiqFailureOnboardDevice unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqViqLicense
+        """Test XiqFailureOnboardDevice
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_viq_license.XiqViqLicense()  # noqa: E501
+        # model = extremecloudiq.models.xiq_failure_onboard_device.XiqFailureOnboardDevice()  # noqa: E501
         if include_optional :
-            return XiqViqLicense(
-                id = 56, 
-                create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                status = 'BUY', 
-                active_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                expire_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                entitlement_key = '0', 
-                entitlement_type = 'EVALUATION', 
-                mode = 'BUY', 
-                devices = 56, 
-                activated = 56, 
-                available = 56, 
-                license_type = '0'
+            return XiqFailureOnboardDevice(
+                serial_number = '0', 
+                error = 'UNKNOWN'
             )
         else :
-            return XiqViqLicense(
-                id = 56,
-                create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                update_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+            return XiqFailureOnboardDevice(
+                serial_number = '0',
         )
 
-    def testXiqViqLicense(self):
-        """Test XiqViqLicense"""
+    def testXiqFailureOnboardDevice(self):
+        """Test XiqFailureOnboardDevice"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_vlan_object_classified_entry.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_vlan_object_classified_entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_vlan_profile.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_vlan_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_vlan_profile_filter.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_password_type.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_vlan_profile_filter import XiqVlanProfileFilter  # noqa: E501
+from extremecloudiq.models.xiq_password_type import XiqPasswordType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqVlanProfileFilter(unittest.TestCase):
-    """XiqVlanProfileFilter unit test stubs"""
+class TestXiqPasswordType(unittest.TestCase):
+    """XiqPasswordType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqVlanProfileFilter
+        """Test XiqPasswordType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_vlan_profile_filter.XiqVlanProfileFilter()  # noqa: E501
+        # model = extremecloudiq.models.xiq_password_type.XiqPasswordType()  # noqa: E501
         if include_optional :
-            return XiqVlanProfileFilter(
-                ids = [
-                    56
-                    ]
+            return XiqPasswordType(
             )
         else :
-            return XiqVlanProfileFilter(
+            return XiqPasswordType(
         )
 
-    def testXiqVlanProfileFilter(self):
-        """Test XiqVlanProfileFilter"""
+    def testXiqPasswordType(self):
+        """Test XiqPasswordType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_voss_devices.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_voss_devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_webhook_subscription.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_webhook_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wifi_capacity_client_list_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wifi_capacity_client_list_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wifi_capacity_stats_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wifi_capacity_stats_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wifi_efficiency_client_list_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wifi_efficiency_client_list_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wifi_efficiency_stats_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wifi_efficiency_stats_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wing_devices.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wing_devices.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wired_event_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wired_event_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wired_hardware_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wired_hardware_entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wired_hardware_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wired_hardware_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wired_quality_index_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wired_quality_index_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wired_view_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_anomaly_health_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import extremecloudiq
-from extremecloudiq.models.xiq_wired_view_type import XiqWiredViewType  # noqa: E501
+from extremecloudiq.models.xiq_anomaly_health_type import XiqAnomalyHealthType  # noqa: E501
 from extremecloudiq.rest import ApiException
 
-class TestXiqWiredViewType(unittest.TestCase):
-    """XiqWiredViewType unit test stubs"""
+class TestXiqAnomalyHealthType(unittest.TestCase):
+    """XiqAnomalyHealthType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test XiqWiredViewType
+        """Test XiqAnomalyHealthType
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # model = extremecloudiq.models.xiq_wired_view_type.XiqWiredViewType()  # noqa: E501
+        # model = extremecloudiq.models.xiq_anomaly_health_type.XiqAnomalyHealthType()  # noqa: E501
         if include_optional :
-            return XiqWiredViewType(
+            return XiqAnomalyHealthType(
             )
         else :
-            return XiqWiredViewType(
+            return XiqAnomalyHealthType(
         )
 
-    def testXiqWiredViewType(self):
-        """Test XiqWiredViewType"""
+    def testXiqAnomalyHealthType(self):
+        """Test XiqAnomalyHealthType"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_apps_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_apps_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_connectivity_performance_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_connectivity_performance_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_event_retries_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_event_retries_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_if_name.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_if_name.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_performance_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_performance_entity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_performance_retries_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_performance_retries_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_quality_index_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_quality_index_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_time_to_connect_entity.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_time_to_connect_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_time_to_connect_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_time_to_connect_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_views_list_type.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_views_list_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/test/test_xiq_wireless_views_type_response.py` & `extremecloudiq-api-23.4.0.41/test/test_xiq_wireless_views_type_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `extremecloudiq-api-23.3.2.1/README.md` & `extremecloudiq-api-23.4.0.41/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # extremecloudiq-api
 ExtremeCloud IQ RESTful API for external and internal applications.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 23.3.2.1
-- Package version: 23.3.2.1
+- API version: 23.4.0.41
+- Package version: 23.4.0.41
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.extremenetworks.com/support](https://www.extremenetworks.com/support)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -110,14 +110,15 @@
 *AuthorizationApi* | [**validate_api_token**](docs/AuthorizationApi.md#validate_api_token) | **POST** /auth/apitoken/:validate | Validate API token
 *ClientApi* | [**disconnect_client**](docs/ClientApi.md#disconnect_client) | **DELETE** /clients/byMac/{clientMac} | Disconnect the client
 *ClientApi* | [**get_active_clients_count**](docs/ClientApi.md#get_active_clients_count) | **GET** /clients/active/count | Get active clients count
 *ClientApi* | [**get_client**](docs/ClientApi.md#get_client) | **GET** /clients/{id} | Get client info
 *ClientApi* | [**get_client_summary**](docs/ClientApi.md#get_client_summary) | **GET** /clients/summary | Get client summary metrics
 *ClientApi* | [**get_client_usage**](docs/ClientApi.md#get_client_usage) | **GET** /clients/usage | Get usage per client
 *ClientApi* | [**list_active_clients**](docs/ClientApi.md#list_active_clients) | **GET** /clients/active | List active clients
+*ClientApi* | [**set_clients_aliases**](docs/ClientApi.md#set_clients_aliases) | **PUT** /clients/alias | Set the aliases for multiple clients
 *ConfigurationAuthenticationApi* | [**create_external_radius_server**](docs/ConfigurationAuthenticationApi.md#create_external_radius_server) | **POST** /radius-servers/external | Create external RADIUS server configuration
 *ConfigurationAuthenticationApi* | [**create_internal_radius_server**](docs/ConfigurationAuthenticationApi.md#create_internal_radius_server) | **POST** /radius-servers/internal | Create internal RADIUS server configuration
 *ConfigurationAuthenticationApi* | [**create_ldap_server**](docs/ConfigurationAuthenticationApi.md#create_ldap_server) | **POST** /ldap-servers | Create LDAP server
 *ConfigurationAuthenticationApi* | [**create_radius_client_object**](docs/ConfigurationAuthenticationApi.md#create_radius_client_object) | **POST** /radius-client-objects | Create RADIUS client object configuration
 *ConfigurationAuthenticationApi* | [**create_radius_proxy**](docs/ConfigurationAuthenticationApi.md#create_radius_proxy) | **POST** /radius-proxies | Create RADIUS proxy configuration
 *ConfigurationAuthenticationApi* | [**delete_bulk_internal_radius_server**](docs/ConfigurationAuthenticationApi.md#delete_bulk_internal_radius_server) | **DELETE** /radius-servers/internal | [LRO] Delete internal RADIUS server configuration
 *ConfigurationAuthenticationApi* | [**delete_external_radius_server**](docs/ConfigurationAuthenticationApi.md#delete_external_radius_server) | **DELETE** /radius-servers/external/{id} | Delete external RADIUS server configuration
@@ -249,14 +250,15 @@
 *CopilotConnectivityExperienceApi* | [**get_wireless_apps**](docs/CopilotConnectivityExperienceApi.md#get_wireless_apps) | **GET** /copilot/connectivity/wireless/apps | 
 *CopilotConnectivityExperienceApi* | [**get_wireless_connectivity_experience**](docs/CopilotConnectivityExperienceApi.md#get_wireless_connectivity_experience) | **GET** /copilot/connectivity/wireless/experience | 
 *CopilotConnectivityExperienceApi* | [**get_wireless_events**](docs/CopilotConnectivityExperienceApi.md#get_wireless_events) | **GET** /copilot/connectivity/wireless/events | 
 *CopilotConnectivityExperienceApi* | [**get_wireless_performance**](docs/CopilotConnectivityExperienceApi.md#get_wireless_performance) | **GET** /copilot/connectivity/wireless/performance | 
 *CopilotConnectivityExperienceApi* | [**get_wireless_quality_index**](docs/CopilotConnectivityExperienceApi.md#get_wireless_quality_index) | **GET** /copilot/connectivity/wireless/quality-index | 
 *CopilotConnectivityExperienceApi* | [**get_wireless_time_to_connect**](docs/CopilotConnectivityExperienceApi.md#get_wireless_time_to_connect) | **GET** /copilot/connectivity/wireless/time-to-connect | 
 *CopilotConnectivityExperienceApi* | [**get_wireless_views**](docs/CopilotConnectivityExperienceApi.md#get_wireless_views) | **GET** /copilot/connectivity/wireless/views | 
+*DeviceApi* | [**advanced_onboard_devices**](docs/DeviceApi.md#advanced_onboard_devices) | **POST** /devices/:advanced-onboard | [LRO] Advanced Onboard Devices
 *DeviceApi* | [**assign_device_location**](docs/DeviceApi.md#assign_device_location) | **PUT** /devices/{id}/location | Assign location to a device
 *DeviceApi* | [**assign_device_network_policy**](docs/DeviceApi.md#assign_device_network_policy) | **PUT** /devices/{id}/network-policy | Assign network policy to a device
 *DeviceApi* | [**assign_devices_country_code**](docs/DeviceApi.md#assign_devices_country_code) | **POST** /devices/country-code/:assign | Assign a country code to devices
 *DeviceApi* | [**assign_devices_location**](docs/DeviceApi.md#assign_devices_location) | **POST** /devices/location/:assign | Assign location to multiple devices
 *DeviceApi* | [**assign_devices_network_policy**](docs/DeviceApi.md#assign_devices_network_policy) | **POST** /devices/network-policy/:assign | Assign network policy to multiple devices
 *DeviceApi* | [**assign_devices_radius_proxy**](docs/DeviceApi.md#assign_devices_radius_proxy) | **PUT** /devices/radius-proxy/:assign | Assign RADIUS proxy to devices
 *DeviceApi* | [**bounce_device_port**](docs/DeviceApi.md#bounce_device_port) | **POST** /devices/{id}/bounce-port | Bounce port of a device (EXOS, VOSS and SR Switches
@@ -395,14 +397,16 @@
  - [PagedXiqWiredEventEntity](docs/PagedXiqWiredEventEntity.md)
  - [XiqAccount](docs/XiqAccount.md)
  - [XiqAccountMode](docs/XiqAccountMode.md)
  - [XiqAccountType](docs/XiqAccountType.md)
  - [XiqAccountingLog](docs/XiqAccountingLog.md)
  - [XiqActiveDirectoryServer](docs/XiqActiveDirectoryServer.md)
  - [XiqActiveDirectoryServerBaseDnFetchMode](docs/XiqActiveDirectoryServerBaseDnFetchMode.md)
+ - [XiqAdvancedOnboardDeviceRequest](docs/XiqAdvancedOnboardDeviceRequest.md)
+ - [XiqAdvancedOnboardDeviceResponse](docs/XiqAdvancedOnboardDeviceResponse.md)
  - [XiqAlert](docs/XiqAlert.md)
  - [XiqAlertCategory](docs/XiqAlertCategory.md)
  - [XiqAlertGroupQuery](docs/XiqAlertGroupQuery.md)
  - [XiqAlertSeverity](docs/XiqAlertSeverity.md)
  - [XiqAlertSource](docs/XiqAlertSource.md)
  - [XiqAlertSourceType](docs/XiqAlertSourceType.md)
  - [XiqAnomaliesCountVoEntity](docs/XiqAnomaliesCountVoEntity.md)
@@ -446,14 +450,15 @@
  - [XiqClassification](docs/XiqClassification.md)
  - [XiqClassificationRule](docs/XiqClassificationRule.md)
  - [XiqClassificationType](docs/XiqClassificationType.md)
  - [XiqCliOutput](docs/XiqCliOutput.md)
  - [XiqCliResponseCode](docs/XiqCliResponseCode.md)
  - [XiqClient](docs/XiqClient.md)
  - [XiqClientField](docs/XiqClientField.md)
+ - [XiqClientMacAddressAlias](docs/XiqClientMacAddressAlias.md)
  - [XiqClientSortField](docs/XiqClientSortField.md)
  - [XiqClientStatsEntity](docs/XiqClientStatsEntity.md)
  - [XiqClientSummary](docs/XiqClientSummary.md)
  - [XiqClientUsage](docs/XiqClientUsage.md)
  - [XiqClientView](docs/XiqClientView.md)
  - [XiqCloudConfigGroup](docs/XiqCloudConfigGroup.md)
  - [XiqConnectivityExperienceData](docs/XiqConnectivityExperienceData.md)
@@ -494,14 +499,15 @@
  - [XiqCwp](docs/XiqCwp.md)
  - [XiqDataPoint](docs/XiqDataPoint.md)
  - [XiqDateTimeType](docs/XiqDateTimeType.md)
  - [XiqDateTimeUnitType](docs/XiqDateTimeUnitType.md)
  - [XiqDefaultDevicePassword](docs/XiqDefaultDevicePassword.md)
  - [XiqDeleteKeyBasedPcgUsersRequest](docs/XiqDeleteKeyBasedPcgUsersRequest.md)
  - [XiqDeliverySettings](docs/XiqDeliverySettings.md)
+ - [XiqDellDevice](docs/XiqDellDevice.md)
  - [XiqDellDevices](docs/XiqDellDevices.md)
  - [XiqDeploymentOverview](docs/XiqDeploymentOverview.md)
  - [XiqDeploymentPolicy](docs/XiqDeploymentPolicy.md)
  - [XiqDeploymentRequest](docs/XiqDeploymentRequest.md)
  - [XiqDeploymentResponse](docs/XiqDeploymentResponse.md)
  - [XiqDeploymentStatus](docs/XiqDeploymentStatus.md)
  - [XiqDevice](docs/XiqDevice.md)
@@ -530,33 +536,37 @@
  - [XiqDfsRecurenceChannelStatsResponse](docs/XiqDfsRecurenceChannelStatsResponse.md)
  - [XiqDfsRecurenceCountStatsResponse](docs/XiqDfsRecurenceCountStatsResponse.md)
  - [XiqDigitalTwinDevice](docs/XiqDigitalTwinDevice.md)
  - [XiqDigitalTwinDevices](docs/XiqDigitalTwinDevices.md)
  - [XiqDigitalTwinFeatLicense](docs/XiqDigitalTwinFeatLicense.md)
  - [XiqDigitalTwinMake](docs/XiqDigitalTwinMake.md)
  - [XiqDigitalTwinModel](docs/XiqDigitalTwinModel.md)
+ - [XiqDigitalTwinOnboardDevice](docs/XiqDigitalTwinOnboardDevice.md)
  - [XiqDigitalTwinProducts](docs/XiqDigitalTwinProducts.md)
  - [XiqDigitalTwinVimModule](docs/XiqDigitalTwinVimModule.md)
  - [XiqDuplexDataRateEntity](docs/XiqDuplexDataRateEntity.md)
  - [XiqEmailLog](docs/XiqEmailLog.md)
  - [XiqEmailTemplate](docs/XiqEmailTemplate.md)
  - [XiqEndUser](docs/XiqEndUser.md)
  - [XiqEntitlementType](docs/XiqEntitlementType.md)
  - [XiqError](docs/XiqError.md)
+ - [XiqExosDevice](docs/XiqExosDevice.md)
  - [XiqExosDevices](docs/XiqExosDevices.md)
  - [XiqExpirationActionType](docs/XiqExpirationActionType.md)
  - [XiqExpirationSettings](docs/XiqExpirationSettings.md)
  - [XiqExpirationType](docs/XiqExpirationType.md)
  - [XiqExternalAccount](docs/XiqExternalAccount.md)
  - [XiqExternalRadiusServer](docs/XiqExternalRadiusServer.md)
  - [XiqExternalUser](docs/XiqExternalUser.md)
  - [XiqExternalUserDirectory](docs/XiqExternalUserDirectory.md)
  - [XiqExternalUserDirectoryEntry](docs/XiqExternalUserDirectoryEntry.md)
  - [XiqExternalUserDirectoryType](docs/XiqExternalUserDirectoryType.md)
+ - [XiqExtremeDevice](docs/XiqExtremeDevice.md)
  - [XiqExtremeDevices](docs/XiqExtremeDevices.md)
+ - [XiqFailureOnboardDevice](docs/XiqFailureOnboardDevice.md)
  - [XiqFirmwareActivateOption](docs/XiqFirmwareActivateOption.md)
  - [XiqFirmwareUpgradePolicy](docs/XiqFirmwareUpgradePolicy.md)
  - [XiqFlapCountEntity](docs/XiqFlapCountEntity.md)
  - [XiqFloor](docs/XiqFloor.md)
  - [XiqForensicBucket](docs/XiqForensicBucket.md)
  - [XiqGenerateApiTokenRequest](docs/XiqGenerateApiTokenRequest.md)
  - [XiqGenerateApiTokenResponse](docs/XiqGenerateApiTokenResponse.md)
@@ -587,14 +597,15 @@
  - [XiqLoginResponse](docs/XiqLoginResponse.md)
  - [XiqMeasurementUnit](docs/XiqMeasurementUnit.md)
  - [XiqNetworkPolicy](docs/XiqNetworkPolicy.md)
  - [XiqNetworkPolicyField](docs/XiqNetworkPolicyField.md)
  - [XiqNetworkPolicyType](docs/XiqNetworkPolicyType.md)
  - [XiqNetworkPolicyView](docs/XiqNetworkPolicyView.md)
  - [XiqOnboardDeviceRequest](docs/XiqOnboardDeviceRequest.md)
+ - [XiqOnboardError](docs/XiqOnboardError.md)
  - [XiqOnboardKeyBasedPcgRequest](docs/XiqOnboardKeyBasedPcgRequest.md)
  - [XiqOperationMetadata](docs/XiqOperationMetadata.md)
  - [XiqOperationObject](docs/XiqOperationObject.md)
  - [XiqOperationStatus](docs/XiqOperationStatus.md)
  - [XiqOrganization](docs/XiqOrganization.md)
  - [XiqOrganizationType](docs/XiqOrganizationType.md)
  - [XiqPasswordCharacterType](docs/XiqPasswordCharacterType.md)
@@ -659,14 +670,15 @@
  - [XiqSsidWepAuthenticationMethod](docs/XiqSsidWepAuthenticationMethod.md)
  - [XiqSsidWepDefaultKey](docs/XiqSsidWepDefaultKey.md)
  - [XiqSsidWepEncryptionMethod](docs/XiqSsidWepEncryptionMethod.md)
  - [XiqSsidWepKeyManagement](docs/XiqSsidWepKeyManagement.md)
  - [XiqSubscriptionDataType](docs/XiqSubscriptionDataType.md)
  - [XiqSubscriptionMessageType](docs/XiqSubscriptionMessageType.md)
  - [XiqSubscriptionStatus](docs/XiqSubscriptionStatus.md)
+ - [XiqSuccessOnboardDevice](docs/XiqSuccessOnboardDevice.md)
  - [XiqTopApplicationsUsage](docs/XiqTopApplicationsUsage.md)
  - [XiqTrendIndicator](docs/XiqTrendIndicator.md)
  - [XiqUpdateBuildingRequest](docs/XiqUpdateBuildingRequest.md)
  - [XiqUpdateClassificationRequest](docs/XiqUpdateClassificationRequest.md)
  - [XiqUpdateClassificationRuleRequest](docs/XiqUpdateClassificationRuleRequest.md)
  - [XiqUpdateCloudConfigGroupRequest](docs/XiqUpdateCloudConfigGroupRequest.md)
  - [XiqUpdateDeviceLevelSsidStatus](docs/XiqUpdateDeviceLevelSsidStatus.md)
@@ -707,20 +719,22 @@
  - [XiqValidTimePeriodAfterIdCreation](docs/XiqValidTimePeriodAfterIdCreation.md)
  - [XiqValidTimePeriodAfterType](docs/XiqValidTimePeriodAfterType.md)
  - [XiqViq](docs/XiqViq.md)
  - [XiqViqLicense](docs/XiqViqLicense.md)
  - [XiqVlanObjectClassifiedEntry](docs/XiqVlanObjectClassifiedEntry.md)
  - [XiqVlanProfile](docs/XiqVlanProfile.md)
  - [XiqVlanProfileFilter](docs/XiqVlanProfileFilter.md)
+ - [XiqVossDevice](docs/XiqVossDevice.md)
  - [XiqVossDevices](docs/XiqVossDevices.md)
  - [XiqWebhookSubscription](docs/XiqWebhookSubscription.md)
  - [XiqWifiCapacityClientListResponse](docs/XiqWifiCapacityClientListResponse.md)
  - [XiqWifiCapacityStatsResponse](docs/XiqWifiCapacityStatsResponse.md)
  - [XiqWifiEfficiencyClientListResponse](docs/XiqWifiEfficiencyClientListResponse.md)
  - [XiqWifiEfficiencyStatsResponse](docs/XiqWifiEfficiencyStatsResponse.md)
+ - [XiqWingDevice](docs/XiqWingDevice.md)
  - [XiqWingDevices](docs/XiqWingDevices.md)
  - [XiqWiredEventEntity](docs/XiqWiredEventEntity.md)
  - [XiqWiredHardwareEntity](docs/XiqWiredHardwareEntity.md)
  - [XiqWiredHardwareResponse](docs/XiqWiredHardwareResponse.md)
  - [XiqWiredQualityIndexResponse](docs/XiqWiredQualityIndexResponse.md)
  - [XiqWiredViewType](docs/XiqWiredViewType.md)
  - [XiqWirelessAppsResponse](docs/XiqWirelessAppsResponse.md)
```

### Comparing `extremecloudiq-api-23.3.2.1/setup.py` & `extremecloudiq-api-23.4.0.41/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 """
     ExtremeCloud IQ API
 
     ExtremeCloud IQ RESTful API for external and internal applications.  # noqa: E501
 
-    The version of the OpenAPI document: 23.3.2.1
+    The version of the OpenAPI document: 23.4.0.41
     Contact: support@extremenetworks.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "extremecloudiq-api"
-VERSION = "23.3.2.1"
+VERSION = "23.4.0.41"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

