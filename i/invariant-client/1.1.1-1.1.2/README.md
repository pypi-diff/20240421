# Comparing `tmp/invariant_client-1.1.1.tar.gz` & `tmp/invariant_client-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invariant_client-1.1.1.tar", max compression
+gzip compressed data, was "invariant_client-1.1.2.tar", max compression
```

## Comparing `invariant_client-1.1.1.tar` & `invariant_client-1.1.2.tar`

### file list

```diff
@@ -1,127 +1,128 @@
--rw-r--r--   0        0        0     1069 2024-03-21 00:30:36.351086 invariant_client-1.1.1/LICENSE
--rw-r--r--   0        0        0     1234 2024-03-21 00:30:36.357508 invariant_client-1.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-21 00:30:36.359660 invariant_client-1.1.1/invariant_client/__init__.py
--rw-r--r--   0        0        0       67 2024-03-21 00:30:36.360236 invariant_client-1.1.1/invariant_client/__main__.py
--rw-r--r--   0        0        0      169 2024-03-21 00:30:36.361091 invariant_client-1.1.1/invariant_client/auth/__init__.py
--rw-r--r--   0        0        0     4213 2024-03-21 00:30:36.361681 invariant_client-1.1.1/invariant_client/auth/auth.py
--rw-r--r--   0        0        0      162 2024-03-21 00:30:36.363015 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/__init__.py
--rw-r--r--   0        0        0       47 2024-03-21 00:30:36.367999 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 00:30:36.369171 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/__init__.py
--rw-r--r--   0        0        0     6126 2024-03-21 00:30:36.372095 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/create_integration_organization_name_api_v_1_integrations_post.py
--rw-r--r--   0        0        0     5813 2024-03-21 00:30:36.379085 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/create_token_organization_name_api_v_1_token_post.py
--rw-r--r--   0        0        0     5527 2024-03-21 00:30:36.381799 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/get_report_download_organization_name_api_v_1_reports_report_id_download_get.py
--rw-r--r--   0        0        0     5488 2024-03-21 00:30:36.383656 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/get_report_organization_name_api_v_1_reports_report_id_get.py
--rw-r--r--   0        0        0     6052 2024-03-21 00:30:36.384219 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/get_report_summary_organization_name_api_v_1_reports_report_id_summary_get.py
--rw-r--r--   0        0        0     6763 2024-03-21 00:30:36.384713 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/get_report_text_summary_organization_name_api_v_1_reports_report_id_text_get.py
--rw-r--r--   0        0        0     6298 2024-03-21 00:30:36.385250 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/invite_user_organization_name_api_v_1_user_invite_post.py
--rw-r--r--   0        0        0     5825 2024-03-21 00:30:36.385842 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/list_integrations_organization_name_api_v_1_integrations_get.py
--rw-r--r--   0        0        0     5582 2024-03-21 00:30:36.386317 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/list_reports_organization_name_api_v_1_reports_get.py
--rw-r--r--   0        0        0     5794 2024-03-21 00:30:36.387333 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/list_tokens_organization_name_api_v_1_token_get.py
--rw-r--r--   0        0        0     5584 2024-03-21 00:30:36.388666 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/refresh_integration_organization_name_api_v_1_integrations_integration_uuid_refresh_post.py
--rw-r--r--   0        0        0     5753 2024-03-21 00:30:36.389169 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/refresh_organization_name_api_v1_refresh_post.py
--rw-r--r--   0        0        0     5838 2024-03-21 00:30:36.389676 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/set_ui_status_organization_name_api_v_1_ui_post.py
--rw-r--r--   0        0        0     5303 2024-03-21 00:30:36.390137 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/ui_status_organization_name_api_v_1_ui_get.py
--rw-r--r--   0        0        0     7002 2024-03-21 00:30:36.390608 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_organization_name_api_v_1_uploadsnapshot_post.py
--rw-r--r--   0        0        0     6131 2024-03-21 00:30:36.391012 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_status_organization_name_api_v_1_uploadsnapshot_status_get.py
--rw-r--r--   0        0        0        0 2024-03-21 00:30:36.391595 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/static_css_js/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 00:30:36.392361 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/static_html/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 00:30:36.393121 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/static_images/__init__.py
--rw-r--r--   0        0        0     3588 2024-03-21 00:30:36.393638 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/static_images/favicon_favicon_ico_get.py
--rw-r--r--   0        0        0    12209 2024-03-21 00:30:36.394293 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/client.py
--rw-r--r--   0        0        0      470 2024-03-21 00:30:36.395547 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/errors.py
--rw-r--r--   0        0        0     4051 2024-03-21 00:30:36.397229 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/__init__.py
--rw-r--r--   0        0        0     3027 2024-03-21 00:30:36.400050 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/base_error_response.py
--rw-r--r--   0        0        0     3710 2024-03-21 00:30:36.412986 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/body_upload_snapshot_organization_name_api_v1_uploadsnapshot_post.py
--rw-r--r--   0        0        0     3944 2024-03-21 00:30:36.415344 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/challenge_response.py
--rw-r--r--   0        0        0      261 2024-03-21 00:30:36.416564 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/challenge_response_challenge.py
--rw-r--r--   0        0        0     2654 2024-03-21 00:30:36.419896 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata.py
--rw-r--r--   0        0        0     1304 2024-03-21 00:30:36.422795 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata_files.py
--rw-r--r--   0        0        0     2579 2024-03-21 00:30:36.429419 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation.py
--rw-r--r--   0        0        0     2269 2024-03-21 00:30:36.454867 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation_data.py
--rw-r--r--   0        0        0     2164 2024-03-21 00:30:36.459025 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/create_token_request.py
--rw-r--r--   0        0        0     3580 2024-03-21 00:30:36.461604 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/external_status_data_integration.py
--rw-r--r--   0        0        0     2682 2024-03-21 00:30:36.469382 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/external_status_integration.py
--rw-r--r--   0        0        0      151 2024-03-21 00:30:36.470460 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/generic_state.py
--rw-r--r--   0        0        0     2723 2024-03-21 00:30:36.473213 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response.py
--rw-r--r--   0        0        0     1335 2024-03-21 00:30:36.475897 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_status.py
--rw-r--r--   0        0        0     1340 2024-03-21 00:30:36.476599 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_summary.py
--rw-r--r--   0        0        0     2788 2024-03-21 00:30:36.477601 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/integration.py
--rw-r--r--   0        0        0     2434 2024-03-21 00:30:36.478447 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation.py
--rw-r--r--   0        0        0     3335 2024-03-21 00:30:36.481711 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data.py
--rw-r--r--   0        0        0     1416 2024-03-21 00:30:36.482807 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data_extra.py
--rw-r--r--   0        0        0     2193 2024-03-21 00:30:36.483518 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/integration_with_status.py
--rw-r--r--   0        0        0     1481 2024-03-21 00:30:36.484333 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/invite_user_request.py
--rw-r--r--   0        0        0     2004 2024-03-21 00:30:36.487204 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/list_reports_response.py
--rw-r--r--   0        0        0     1572 2024-03-21 00:30:36.493383 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/metadata.py
--rw-r--r--   0        0        0     2709 2024-03-21 00:30:36.504663 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/organization.py
--rw-r--r--   0        0        0     2621 2024-03-21 00:30:36.505620 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/poc_report_data.py
--rw-r--r--   0        0        0     2352 2024-03-21 00:30:36.506364 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/refresh_response.py
--rw-r--r--   0        0        0     3375 2024-03-21 00:30:36.506739 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/report.py
--rw-r--r--   0        0        0     1914 2024-03-21 00:30:36.507977 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/report_text_summary_request.py
--rw-r--r--   0        0        0     2256 2024-03-21 00:30:36.508309 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/report_text_summary_response.py
--rw-r--r--   0        0        0     4949 2024-03-21 00:30:36.508679 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data.py
--rw-r--r--   0        0        0     1297 2024-03-21 00:30:36.509128 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data_files.py
--rw-r--r--   0        0        0     4420 2024-03-21 00:30:36.509679 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/tab_info.py
--rw-r--r--   0        0        0     2821 2024-03-21 00:30:36.510194 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/tab_info_parameters_type_0.py
--rw-r--r--   0        0        0     1270 2024-03-21 00:30:36.510795 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/tab_info_state_type_0.py
--rw-r--r--   0        0        0     3093 2024-03-21 00:30:36.511490 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/ui_status_response.py
--rw-r--r--   0        0        0     1546 2024-03-21 00:30:36.513314 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_response.py
--rw-r--r--   0        0        0     1795 2024-03-21 00:30:36.513965 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_status_response.py
--rw-r--r--   0        0        0     4555 2024-03-21 00:30:36.514599 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/user.py
--rw-r--r--   0        0        0     1525 2024-03-21 00:30:36.514975 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/user_metadata.py
--rw-r--r--   0        0        0     1922 2024-03-21 00:30:36.515601 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/user_tabs_config.py
--rw-r--r--   0        0        0     3945 2024-03-21 00:30:36.515947 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/validation_error_response.py
--rw-r--r--   0        0        0     1850 2024-03-21 00:30:36.516410 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/validation_error_response_part.py
--rw-r--r--   0        0        0      968 2024-03-21 00:30:36.516801 invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/types.py
--rw-r--r--   0        0        0      159 2024-03-21 00:30:36.517530 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/__init__.py
--rw-r--r--   0        0        0       47 2024-03-21 00:30:36.518148 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 00:30:36.519325 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/client_login/__init__.py
--rw-r--r--   0        0        0     4700 2024-03-21 00:30:36.519862 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/client_login/consume_client_login_api_v1_client_login_consume_post.py
--rw-r--r--   0        0        0     5770 2024-03-21 00:30:36.520678 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/client_login/fulfill_client_login_api_v1_fulfill_client_login_post.py
--rw-r--r--   0        0        0     4590 2024-03-21 00:30:36.521573 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/client_login/init_client_login_api_v1_client_login_post.py
--rw-r--r--   0        0        0        0 2024-03-21 00:30:36.522692 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/__init__.py
--rw-r--r--   0        0        0     5085 2024-03-21 00:30:36.524556 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/active_login_exists_for_email_api_v1_login_exists_post.py
--rw-r--r--   0        0        0     7153 2024-03-21 00:30:36.525109 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/check_invite_api_v1_login_check_invite_post.py
--rw-r--r--   0        0        0     4746 2024-03-21 00:30:36.526157 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/get_instances_api_v1_login_get_instances_post.py
--rw-r--r--   0        0        0     3948 2024-03-21 00:30:36.526821 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/get_version_api_v1_login_version_get.py
--rw-r--r--   0        0        0    14437 2024-03-21 00:30:36.527526 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/init_login_api_v1_login_post.py
--rw-r--r--   0        0        0     4470 2024-03-21 00:30:36.527930 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/refresh_api_v1_login_refresh_post.py
--rw-r--r--   0        0        0     5473 2024-03-21 00:30:36.528646 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/register_api_v1_login_register_post.py
--rw-r--r--   0        0        0     4492 2024-03-21 00:30:36.529045 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/resend_validation_pin_api_v1_login_resend_validation_pin_post.py
--rw-r--r--   0        0        0        0 2024-03-21 00:30:36.529654 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/static/__init__.py
--rw-r--r--   0        0        0     4042 2024-03-21 00:30:36.530136 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/static/static_urlpath_get.py
--rw-r--r--   0        0        0        0 2024-03-21 00:30:36.530702 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/webhooks/__init__.py
--rw-r--r--   0        0        0     4347 2024-03-21 00:30:36.534994 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/webhooks/github_webhook_recv_api_v1_github_webhook_post.py
--rw-r--r--   0        0        0    12209 2024-03-21 00:30:36.538851 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/client.py
--rw-r--r--   0        0        0      470 2024-03-21 00:30:36.542306 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/errors.py
--rw-r--r--   0        0        0     1900 2024-03-21 00:30:36.565240 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/__init__.py
--rw-r--r--   0        0        0     3027 2024-03-21 00:30:36.570381 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/base_error_response.py
--rw-r--r--   0        0        0     3944 2024-03-21 00:30:36.572465 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/challenge_response.py
--rw-r--r--   0        0        0      261 2024-03-21 00:30:36.573804 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/challenge_response_challenge.py
--rw-r--r--   0        0        0     2241 2024-03-21 00:30:36.576191 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/check_invite_response.py
--rw-r--r--   0        0        0     3324 2024-03-21 00:30:36.578894 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/consume_client_login_session_response.py
--rw-r--r--   0        0        0     2708 2024-03-21 00:30:36.584325 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/create_client_login_session_response.py
--rw-r--r--   0        0        0     1481 2024-03-21 00:30:36.585034 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/email_check_request.py
--rw-r--r--   0        0        0     1668 2024-03-21 00:30:36.585578 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/email_password_login.py
--rw-r--r--   0        0        0     1776 2024-03-21 00:30:36.586158 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/fulfill_client_login_request.py
--rw-r--r--   0        0        0     1506 2024-03-21 00:30:36.586640 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/get_version_response.py
--rw-r--r--   0        0        0     1557 2024-03-21 00:30:36.589679 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/login.py
--rw-r--r--   0        0        0    10565 2024-03-21 00:30:36.592772 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/login_request.py
--rw-r--r--   0        0        0     2461 2024-03-21 00:30:36.593850 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/new_password_request.py
--rw-r--r--   0        0        0      168 2024-03-21 00:30:36.594631 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/new_password_request_authn_type.py
--rw-r--r--   0        0        0     2220 2024-03-21 00:30:36.595695 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/organization.py
--rw-r--r--   0        0        0     1786 2024-03-21 00:30:36.602489 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/register_organization_request_body.py
--rw-r--r--   0        0        0     1603 2024-03-21 00:30:36.603187 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/reset_pin_request.py
--rw-r--r--   0        0        0     1453 2024-03-21 00:30:36.604096 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/reset_request.py
--rw-r--r--   0        0        0     2678 2024-03-21 00:30:36.605963 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/user.py
--rw-r--r--   0        0        0     3945 2024-03-21 00:30:36.610324 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/validation_error_response.py
--rw-r--r--   0        0        0     1850 2024-03-21 00:30:36.615041 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/validation_error_response_part.py
--rw-r--r--   0        0        0     1458 2024-03-21 00:30:36.618777 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/validation_request.py
--rw-r--r--   0        0        0      968 2024-03-21 00:30:36.621828 invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/types.py
--rw-r--r--   0        0        0    15895 2024-03-21 00:30:36.626672 invariant_client-1.1.1/invariant_client/cli.py
--rw-r--r--   0        0        0     3010 2024-03-21 00:30:36.655168 invariant_client-1.1.1/invariant_client/display.py
--rw-r--r--   0        0        0    18041 2024-03-21 00:30:36.667483 invariant_client-1.1.1/invariant_client/pysdk.py
--rw-r--r--   0        0        0     1616 2024-03-21 00:30:36.670011 invariant_client-1.1.1/invariant_client/version.py
--rw-r--r--   0        0        0     2481 2024-03-21 00:30:36.684494 invariant_client-1.1.1/invariant_client/zip_util.py
--rw-r--r--   0        0        0      772 2024-03-21 00:30:36.775423 invariant_client-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 invariant_client-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-20 17:20:31.942692 invariant_client-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1262 2024-04-20 17:20:31.942785 invariant_client-1.1.2/README.md
+-rw-r--r--   0        0        0     6148 2024-04-20 17:21:49.048467 invariant_client-1.1.2/invariant_client/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-20 17:20:31.942933 invariant_client-1.1.2/invariant_client/__init__.py
+-rw-r--r--   0        0        0       67 2024-04-20 17:20:31.943029 invariant_client-1.1.2/invariant_client/__main__.py
+-rw-r--r--   0        0        0      169 2024-04-20 17:20:31.943153 invariant_client-1.1.2/invariant_client/auth/__init__.py
+-rw-r--r--   0        0        0     4213 2024-04-20 17:20:31.943252 invariant_client-1.1.2/invariant_client/auth/auth.py
+-rw-r--r--   0        0        0      162 2024-04-20 17:20:31.943422 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-20 17:20:31.943537 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:20:31.943620 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/__init__.py
+-rw-r--r--   0        0        0     6126 2024-04-20 17:20:31.943790 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/create_integration_organization_name_api_v_1_integrations_post.py
+-rw-r--r--   0        0        0     5813 2024-04-20 17:20:31.943953 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/create_token_organization_name_api_v_1_token_post.py
+-rw-r--r--   0        0        0     5527 2024-04-20 17:20:31.944096 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_download_organization_name_api_v_1_reports_report_id_download_get.py
+-rw-r--r--   0        0        0     5488 2024-04-20 17:20:31.944189 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_organization_name_api_v_1_reports_report_id_get.py
+-rw-r--r--   0        0        0     6052 2024-04-20 17:20:31.944302 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_summary_organization_name_api_v_1_reports_report_id_summary_get.py
+-rw-r--r--   0        0        0     6763 2024-04-20 17:20:31.944389 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_text_summary_organization_name_api_v_1_reports_report_id_text_get.py
+-rw-r--r--   0        0        0     6298 2024-04-20 17:20:31.944542 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/invite_user_organization_name_api_v_1_user_invite_post.py
+-rw-r--r--   0        0        0     5825 2024-04-20 17:20:31.944639 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/list_integrations_organization_name_api_v_1_integrations_get.py
+-rw-r--r--   0        0        0     5582 2024-04-20 17:20:31.944739 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/list_reports_organization_name_api_v_1_reports_get.py
+-rw-r--r--   0        0        0     5794 2024-04-20 17:20:31.944850 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/list_tokens_organization_name_api_v_1_token_get.py
+-rw-r--r--   0        0        0     5584 2024-04-20 17:20:31.944995 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/refresh_integration_organization_name_api_v_1_integrations_integration_uuid_refresh_post.py
+-rw-r--r--   0        0        0     5753 2024-04-20 17:20:31.945105 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/refresh_organization_name_api_v1_refresh_post.py
+-rw-r--r--   0        0        0     5838 2024-04-20 17:20:31.945212 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/set_ui_status_organization_name_api_v_1_ui_post.py
+-rw-r--r--   0        0        0     5303 2024-04-20 17:20:31.945318 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/ui_status_organization_name_api_v_1_ui_get.py
+-rw-r--r--   0        0        0     7002 2024-04-20 17:20:31.945428 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_organization_name_api_v_1_uploadsnapshot_post.py
+-rw-r--r--   0        0        0     6131 2024-04-20 17:20:31.945554 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_status_organization_name_api_v_1_uploadsnapshot_status_get.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:20:31.945670 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/static_css_js/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:20:31.945787 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/static_html/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:20:31.945910 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/static_images/__init__.py
+-rw-r--r--   0        0        0     3588 2024-04-20 17:20:31.946019 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/static_images/favicon_favicon_ico_get.py
+-rw-r--r--   0        0        0    12209 2024-04-20 17:20:31.946149 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/client.py
+-rw-r--r--   0        0        0      470 2024-04-20 17:20:31.946241 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/errors.py
+-rw-r--r--   0        0        0     4051 2024-04-20 17:20:31.946396 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/__init__.py
+-rw-r--r--   0        0        0     3027 2024-04-20 17:20:31.946507 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/base_error_response.py
+-rw-r--r--   0        0        0     3710 2024-04-20 17:20:31.946630 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/body_upload_snapshot_organization_name_api_v1_uploadsnapshot_post.py
+-rw-r--r--   0        0        0     3944 2024-04-20 17:20:31.946762 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/challenge_response.py
+-rw-r--r--   0        0        0      261 2024-04-20 17:20:31.946878 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/challenge_response_challenge.py
+-rw-r--r--   0        0        0     2654 2024-04-20 17:20:31.947013 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata.py
+-rw-r--r--   0        0        0     1304 2024-04-20 17:20:31.947125 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata_files.py
+-rw-r--r--   0        0        0     2579 2024-04-20 17:20:31.947265 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation.py
+-rw-r--r--   0        0        0     2269 2024-04-20 17:20:31.947387 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation_data.py
+-rw-r--r--   0        0        0     2164 2024-04-20 17:20:31.947507 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/create_token_request.py
+-rw-r--r--   0        0        0     3580 2024-04-20 17:20:31.947595 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/external_status_data_integration.py
+-rw-r--r--   0        0        0     2682 2024-04-20 17:20:31.947679 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/external_status_integration.py
+-rw-r--r--   0        0        0      151 2024-04-20 17:20:31.947757 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/generic_state.py
+-rw-r--r--   0        0        0     2723 2024-04-20 17:20:31.947851 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response.py
+-rw-r--r--   0        0        0     1335 2024-04-20 17:20:31.947930 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_status.py
+-rw-r--r--   0        0        0     1340 2024-04-20 17:20:31.948014 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_summary.py
+-rw-r--r--   0        0        0     2788 2024-04-20 17:20:31.948090 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration.py
+-rw-r--r--   0        0        0     2434 2024-04-20 17:20:31.948168 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation.py
+-rw-r--r--   0        0        0     3335 2024-04-20 17:20:31.948241 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data.py
+-rw-r--r--   0        0        0     1416 2024-04-20 17:20:31.948309 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data_extra.py
+-rw-r--r--   0        0        0     2193 2024-04-20 17:20:31.948381 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_with_status.py
+-rw-r--r--   0        0        0     1481 2024-04-20 17:20:31.948476 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/invite_user_request.py
+-rw-r--r--   0        0        0     2004 2024-04-20 17:20:31.948566 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/list_reports_response.py
+-rw-r--r--   0        0        0     1572 2024-04-20 17:20:31.948656 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/metadata.py
+-rw-r--r--   0        0        0     2709 2024-04-20 17:20:31.948753 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/organization.py
+-rw-r--r--   0        0        0     2621 2024-04-20 17:20:31.948876 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/poc_report_data.py
+-rw-r--r--   0        0        0     2352 2024-04-20 17:20:31.948966 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/refresh_response.py
+-rw-r--r--   0        0        0     3375 2024-04-20 17:20:31.949030 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/report.py
+-rw-r--r--   0        0        0     1914 2024-04-20 17:20:31.949118 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/report_text_summary_request.py
+-rw-r--r--   0        0        0     2256 2024-04-20 17:20:31.949199 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/report_text_summary_response.py
+-rw-r--r--   0        0        0     4949 2024-04-20 17:20:31.949275 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data.py
+-rw-r--r--   0        0        0     1297 2024-04-20 17:20:31.949345 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data_files.py
+-rw-r--r--   0        0        0     4420 2024-04-20 17:20:31.949430 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/tab_info.py
+-rw-r--r--   0        0        0     2821 2024-04-20 17:20:31.949517 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/tab_info_parameters_type_0.py
+-rw-r--r--   0        0        0     1270 2024-04-20 17:20:31.949584 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/tab_info_state_type_0.py
+-rw-r--r--   0        0        0     3093 2024-04-20 17:20:31.949661 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/ui_status_response.py
+-rw-r--r--   0        0        0     1546 2024-04-20 17:20:31.949728 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_response.py
+-rw-r--r--   0        0        0     1795 2024-04-20 17:20:31.949807 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_status_response.py
+-rw-r--r--   0        0        0     4555 2024-04-20 17:20:31.949876 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/user.py
+-rw-r--r--   0        0        0     1525 2024-04-20 17:20:31.949952 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/user_metadata.py
+-rw-r--r--   0        0        0     1922 2024-04-20 17:20:31.950031 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/user_tabs_config.py
+-rw-r--r--   0        0        0     3945 2024-04-20 17:20:31.950114 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/validation_error_response.py
+-rw-r--r--   0        0        0     1850 2024-04-20 17:20:31.950209 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/validation_error_response_part.py
+-rw-r--r--   0        0        0      968 2024-04-20 17:20:31.950282 invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/types.py
+-rw-r--r--   0        0        0      159 2024-04-20 17:20:31.950405 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-20 17:20:31.950508 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:20:31.950584 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/__init__.py
+-rw-r--r--   0        0        0     4700 2024-04-20 17:20:31.950675 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/consume_client_login_api_v1_client_login_consume_post.py
+-rw-r--r--   0        0        0     5770 2024-04-20 17:20:31.950772 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/fulfill_client_login_api_v1_fulfill_client_login_post.py
+-rw-r--r--   0        0        0     4590 2024-04-20 17:20:31.950852 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/init_client_login_api_v1_client_login_post.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:20:31.950928 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/__init__.py
+-rw-r--r--   0        0        0     5085 2024-04-20 17:20:31.951007 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/active_login_exists_for_email_api_v1_login_exists_post.py
+-rw-r--r--   0        0        0     7153 2024-04-20 17:20:31.951092 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/check_invite_api_v1_login_check_invite_post.py
+-rw-r--r--   0        0        0     4746 2024-04-20 17:20:31.951178 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/get_instances_api_v1_login_get_instances_post.py
+-rw-r--r--   0        0        0     3948 2024-04-20 17:20:31.951263 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/get_version_api_v1_login_version_get.py
+-rw-r--r--   0        0        0    14437 2024-04-20 17:20:31.951340 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/init_login_api_v1_login_post.py
+-rw-r--r--   0        0        0     4470 2024-04-20 17:20:31.951418 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/refresh_api_v1_login_refresh_post.py
+-rw-r--r--   0        0        0     5473 2024-04-20 17:20:31.951497 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/register_api_v1_login_register_post.py
+-rw-r--r--   0        0        0     4492 2024-04-20 17:20:31.951579 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/resend_validation_pin_api_v1_login_resend_validation_pin_post.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:20:31.951659 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/static/__init__.py
+-rw-r--r--   0        0        0     4042 2024-04-20 17:20:31.951744 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/static/static_urlpath_get.py
+-rw-r--r--   0        0        0        0 2024-04-20 17:20:31.951818 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/webhooks/__init__.py
+-rw-r--r--   0        0        0     4347 2024-04-20 17:20:31.951910 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/webhooks/github_webhook_recv_api_v1_github_webhook_post.py
+-rw-r--r--   0        0        0    12209 2024-04-20 17:20:31.952005 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/client.py
+-rw-r--r--   0        0        0      470 2024-04-20 17:20:31.952082 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/errors.py
+-rw-r--r--   0        0        0     1900 2024-04-20 17:20:31.952192 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/__init__.py
+-rw-r--r--   0        0        0     3027 2024-04-20 17:20:31.952282 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/base_error_response.py
+-rw-r--r--   0        0        0     3944 2024-04-20 17:20:31.952344 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/challenge_response.py
+-rw-r--r--   0        0        0      261 2024-04-20 17:20:31.952411 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/challenge_response_challenge.py
+-rw-r--r--   0        0        0     2241 2024-04-20 17:20:31.952479 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/check_invite_response.py
+-rw-r--r--   0        0        0     3324 2024-04-20 17:20:31.952549 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/consume_client_login_session_response.py
+-rw-r--r--   0        0        0     2708 2024-04-20 17:20:31.952613 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/create_client_login_session_response.py
+-rw-r--r--   0        0        0     1481 2024-04-20 17:20:31.952673 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/email_check_request.py
+-rw-r--r--   0        0        0     1668 2024-04-20 17:20:31.952742 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/email_password_login.py
+-rw-r--r--   0        0        0     1776 2024-04-20 17:20:31.952803 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/fulfill_client_login_request.py
+-rw-r--r--   0        0        0     1506 2024-04-20 17:20:31.952865 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/get_version_response.py
+-rw-r--r--   0        0        0     1557 2024-04-20 17:20:31.952932 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/login.py
+-rw-r--r--   0        0        0    10565 2024-04-20 17:20:31.953000 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/login_request.py
+-rw-r--r--   0        0        0     2461 2024-04-20 17:20:31.953068 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/new_password_request.py
+-rw-r--r--   0        0        0      168 2024-04-20 17:20:31.953142 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/new_password_request_authn_type.py
+-rw-r--r--   0        0        0     2220 2024-04-20 17:20:31.953210 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/organization.py
+-rw-r--r--   0        0        0     1786 2024-04-20 17:20:31.953289 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/register_organization_request_body.py
+-rw-r--r--   0        0        0     1603 2024-04-20 17:20:31.953351 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/reset_pin_request.py
+-rw-r--r--   0        0        0     1453 2024-04-20 17:20:31.953410 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/reset_request.py
+-rw-r--r--   0        0        0     2678 2024-04-20 17:20:31.953472 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/user.py
+-rw-r--r--   0        0        0     3945 2024-04-20 17:20:31.953536 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/validation_error_response.py
+-rw-r--r--   0        0        0     1850 2024-04-20 17:20:31.953604 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/validation_error_response_part.py
+-rw-r--r--   0        0        0     1458 2024-04-20 17:20:31.953667 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/validation_request.py
+-rw-r--r--   0        0        0      968 2024-04-20 17:20:31.953734 invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/types.py
+-rw-r--r--   0        0        0    15895 2024-04-20 17:20:31.953883 invariant_client-1.1.2/invariant_client/cli.py
+-rw-r--r--   0        0        0     3010 2024-04-20 17:20:31.953974 invariant_client-1.1.2/invariant_client/display.py
+-rw-r--r--   0        0        0    18041 2024-04-20 17:20:31.954113 invariant_client-1.1.2/invariant_client/pysdk.py
+-rw-r--r--   0        0        0     1616 2024-04-20 17:20:31.954189 invariant_client-1.1.2/invariant_client/version.py
+-rw-r--r--   0        0        0     2481 2024-04-20 17:20:31.954277 invariant_client-1.1.2/invariant_client/zip_util.py
+-rw-r--r--   0        0        0      800 2024-04-20 23:49:40.609789 invariant_client-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 invariant_client-1.1.2/PKG-INFO
```

### Comparing `invariant_client-1.1.1/LICENSE` & `invariant_client-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/README.md` & `invariant_client-1.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # Invariant CLI and Python SDK
 
 ## Installation
 
 The Invariant client is available as a Python package. You can install it through pip or pipx like so:
 
 ```bash
-pip install invariant
+pip install invariant-client
 
 # Or using pipx
-pipx install invariant
+pipx install invariant-client
 ```
 
 The Invariant CLI can be used to run Invariant from your test automation workflow. This example shows one way to install it for Github Actions:
 
 ```yaml
 steps:
 - uses: actions/checkout@v4
 - uses: actions/setup-python@v4
   with:
     python-version: '3.11'
     cache: 'pip'
 - name: Install dependencies
-  run: python -m pip install --upgrade pip invariant
+  run: python -m pip install --upgrade pip invariant-client
 - name: Evaluate current directory using Invariant
   run: |
-    python -m invariant run
+    python -m invariant-client run
 ```
 
 ## Usage: Command Line Interface
 
 The Invariant CLI can analyize local changes to network configuration files.
 
 ```bash
 $ invariant login
 Open this link in your browser to log in:
-https://invariant.test/login?code=320664
+https://invariant.tech/login?code=320664
 Login successful.
 
 $ invariant run
 Uploading snapshot...
 Processing... (51643c3e-9a08-47b9-968e-1d2d7e2ca42e)
 Analysis complete.
```

### Comparing `invariant_client-1.1.1/invariant_client/auth/auth.py` & `invariant_client-1.1.2/invariant_client/auth/auth.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/create_integration_organization_name_api_v_1_integrations_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/create_integration_organization_name_api_v_1_integrations_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/create_token_organization_name_api_v_1_token_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/create_token_organization_name_api_v_1_token_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/get_report_download_organization_name_api_v_1_reports_report_id_download_get.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_download_organization_name_api_v_1_reports_report_id_download_get.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/get_report_organization_name_api_v_1_reports_report_id_get.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_organization_name_api_v_1_reports_report_id_get.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/get_report_summary_organization_name_api_v_1_reports_report_id_summary_get.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_summary_organization_name_api_v_1_reports_report_id_summary_get.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/get_report_text_summary_organization_name_api_v_1_reports_report_id_text_get.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/get_report_text_summary_organization_name_api_v_1_reports_report_id_text_get.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/invite_user_organization_name_api_v_1_user_invite_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/invite_user_organization_name_api_v_1_user_invite_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/list_integrations_organization_name_api_v_1_integrations_get.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/list_integrations_organization_name_api_v_1_integrations_get.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/list_reports_organization_name_api_v_1_reports_get.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/list_reports_organization_name_api_v_1_reports_get.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/list_tokens_organization_name_api_v_1_token_get.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/list_tokens_organization_name_api_v_1_token_get.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/refresh_integration_organization_name_api_v_1_integrations_integration_uuid_refresh_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/refresh_integration_organization_name_api_v_1_integrations_integration_uuid_refresh_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/refresh_organization_name_api_v1_refresh_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/refresh_organization_name_api_v1_refresh_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/set_ui_status_organization_name_api_v_1_ui_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/set_ui_status_organization_name_api_v_1_ui_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/ui_status_organization_name_api_v_1_ui_get.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/ui_status_organization_name_api_v_1_ui_get.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_organization_name_api_v_1_uploadsnapshot_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_organization_name_api_v_1_uploadsnapshot_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_status_organization_name_api_v_1_uploadsnapshot_status_get.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/organization/upload_snapshot_status_organization_name_api_v_1_uploadsnapshot_status_get.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/api/static_images/favicon_favicon_ico_get.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/api/static_images/favicon_favicon_ico_get.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/client.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/client.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/__init__.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/base_error_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/base_error_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/body_upload_snapshot_organization_name_api_v1_uploadsnapshot_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/body_upload_snapshot_organization_name_api_v1_uploadsnapshot_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/challenge_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/challenge_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata_files.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/comparison_reportdata_files.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation_data.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/create_integration_request_github_app_installation_data.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/create_token_request.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/create_token_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/external_status_data_integration.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/external_status_data_integration.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/external_status_integration.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/external_status_integration.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_status.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_status.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_summary.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/get_report_summary_response_summary.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/integration.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data_extra.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_data_github_app_installation_data_extra.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/integration_with_status.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/integration_with_status.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/invite_user_request.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/invite_user_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/list_reports_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/list_reports_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/metadata.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/metadata.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/organization.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/poc_report_data.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/poc_report_data.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/refresh_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/refresh_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/report.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/report.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/report_text_summary_request.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/report_text_summary_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/report_text_summary_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/report_text_summary_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data_files.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/snapshot_report_data_files.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/tab_info.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/tab_info.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/tab_info_parameters_type_0.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/tab_info_parameters_type_0.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/tab_info_state_type_0.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/tab_info_state_type_0.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/ui_status_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/ui_status_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_status_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/upload_snapshot_status_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/user.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/user.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/user_metadata.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/user_metadata.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/user_tabs_config.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/user_tabs_config.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/validation_error_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/validation_error_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/models/validation_error_response_part.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/models/validation_error_response_part.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_instance_client/types.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_instance_client/types.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/client_login/consume_client_login_api_v1_client_login_consume_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/consume_client_login_api_v1_client_login_consume_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/client_login/fulfill_client_login_api_v1_fulfill_client_login_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/fulfill_client_login_api_v1_fulfill_client_login_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/client_login/init_client_login_api_v1_client_login_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/client_login/init_client_login_api_v1_client_login_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/active_login_exists_for_email_api_v1_login_exists_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/active_login_exists_for_email_api_v1_login_exists_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/check_invite_api_v1_login_check_invite_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/check_invite_api_v1_login_check_invite_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/get_instances_api_v1_login_get_instances_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/get_instances_api_v1_login_get_instances_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/get_version_api_v1_login_version_get.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/get_version_api_v1_login_version_get.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/init_login_api_v1_login_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/init_login_api_v1_login_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/refresh_api_v1_login_refresh_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/refresh_api_v1_login_refresh_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/register_api_v1_login_register_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/register_api_v1_login_register_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/login/resend_validation_pin_api_v1_login_resend_validation_pin_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/login/resend_validation_pin_api_v1_login_resend_validation_pin_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/static/static_urlpath_get.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/static/static_urlpath_get.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/api/webhooks/github_webhook_recv_api_v1_github_webhook_post.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/api/webhooks/github_webhook_recv_api_v1_github_webhook_post.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/client.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/client.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/__init__.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/base_error_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/base_error_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/challenge_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/challenge_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/check_invite_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/check_invite_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/consume_client_login_session_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/consume_client_login_session_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/create_client_login_session_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/create_client_login_session_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/email_check_request.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/email_check_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/email_password_login.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/email_password_login.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/fulfill_client_login_request.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/fulfill_client_login_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/get_version_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/get_version_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/login.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/login.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/login_request.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/login_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/new_password_request.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/new_password_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/organization.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/register_organization_request_body.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/register_organization_request_body.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/reset_pin_request.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/reset_pin_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/reset_request.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/reset_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/user.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/user.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/validation_error_response.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/validation_error_response.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/validation_error_response_part.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/validation_error_response_part.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/models/validation_request.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/models/validation_request.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/bindings/invariant_login_client/types.py` & `invariant_client-1.1.2/invariant_client/bindings/invariant_login_client/types.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/cli.py` & `invariant_client-1.1.2/invariant_client/cli.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/display.py` & `invariant_client-1.1.2/invariant_client/display.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/pysdk.py` & `invariant_client-1.1.2/invariant_client/pysdk.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/version.py` & `invariant_client-1.1.2/invariant_client/version.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/invariant_client/zip_util.py` & `invariant_client-1.1.2/invariant_client/zip_util.py`

 * *Files identical despite different names*

### Comparing `invariant_client-1.1.1/pyproject.toml` & `invariant_client-1.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "invariant-client"
-version = "1.1.1"
-description = "Invariant Website"
+version = "1.1.2"
+description = "Invariant: manage ACLs in an entirely new way"
 authors = ["Rob Ankeny <ankenyr@gmail.com>", "Jason Benterou <jason.benterou@invariant.tech>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 invariant = "invariant_client.cli:EntryPoint"
 
 [tool.poetry.dependencies]
```

### Comparing `invariant_client-1.1.1/PKG-INFO` & `invariant_client-1.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: invariant-client
-Version: 1.1.1
-Summary: Invariant Website
+Version: 1.1.2
+Summary: Invariant: manage ACLs in an entirely new way
 Author: Rob Ankeny
 Author-email: ankenyr@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: attrs (>=21.3.0)
 Requires-Dist: httpx (>=0.20.0,<0.26.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pyarrow (>=13.0.0,<14.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
@@ -22,44 +21,44 @@
 # Invariant CLI and Python SDK
 
 ## Installation
 
 The Invariant client is available as a Python package. You can install it through pip or pipx like so:
 
 ```bash
-pip install invariant
+pip install invariant-client
 
 # Or using pipx
-pipx install invariant
+pipx install invariant-client
 ```
 
 The Invariant CLI can be used to run Invariant from your test automation workflow. This example shows one way to install it for Github Actions:
 
 ```yaml
 steps:
 - uses: actions/checkout@v4
 - uses: actions/setup-python@v4
   with:
     python-version: '3.11'
     cache: 'pip'
 - name: Install dependencies
-  run: python -m pip install --upgrade pip invariant
+  run: python -m pip install --upgrade pip invariant-client
 - name: Evaluate current directory using Invariant
   run: |
-    python -m invariant run
+    python -m invariant-client run
 ```
 
 ## Usage: Command Line Interface
 
 The Invariant CLI can analyize local changes to network configuration files.
 
 ```bash
 $ invariant login
 Open this link in your browser to log in:
-https://invariant.test/login?code=320664
+https://invariant.tech/login?code=320664
 Login successful.
 
 $ invariant run
 Uploading snapshot...
 Processing... (51643c3e-9a08-47b9-968e-1d2d7e2ca42e)
 Analysis complete.
```

