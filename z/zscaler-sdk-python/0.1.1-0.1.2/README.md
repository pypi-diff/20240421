# Comparing `tmp/zscaler-sdk-python-0.1.1.tar.gz` & `tmp/zscaler-sdk-python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zscaler-sdk-python-0.1.1.tar", last modified: Fri Apr 19 06:21:36 2024, max compression
+gzip compressed data, was "zscaler-sdk-python-0.1.2.tar", last modified: Sat Apr 20 22:57:24 2024, max compression
```

## Comparing `zscaler-sdk-python-0.1.1.tar` & `zscaler-sdk-python-0.1.2.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.465035 zscaler-sdk-python-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-04-19 06:21:36.465035 zscaler-sdk-python-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.437035 zscaler-sdk-python-0.1.1/docsrc/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.437035 zscaler-sdk-python-0.1.1/docsrc/zs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.437035 zscaler-sdk-python-0.1.1/docsrc/zs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/guides/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/guides/support.rst
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/guides/troubleshooting.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.441035 zscaler-sdk-python-0.1.1/docsrc/zs/zia/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/activate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/admin_and_role_management.rst
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/apptotal.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/audit_logs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/authentication_settings.rst
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/cloud_apps.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/device_management.rst
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/dlp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/firewall.rst
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/forwarding_control.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/isolation_profile.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/locations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/rule_labels.rst
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/sandbox.rst
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/security.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/ssl_inspection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/traffic.rst
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/url_categories.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/url_filtering.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/users.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/web_dlp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/workload_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zia/zpa_gateway.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.445035 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/app_segments.rst
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/app_segments_inspection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/app_segments_pra.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/certificates.rst
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/cloud_connector_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/connectors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/emergency_access.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/idp.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/inspection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/isolation_profile.rst
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/lss.rst
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/machine_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/policies.rst
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/posture_profiles.rst
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/privileged_remote_access.rst
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/provisioning.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/saml_attributes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/scim_attributes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/scim_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/segment_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/server_groups.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/servers.rst
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/service_edges.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/docsrc/zs/zpa/trusted_networks.rst
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 06:21:36.469035 zscaler-sdk-python-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1750 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.445035 zscaler-sdk-python-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.437035 zscaler-sdk-python-0.1.1/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.449035 zscaler-sdk-python-0.1.1/tests/integration/zia/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_admin_and_role_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_authentication_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_cloud_firewall_ip_destination_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_cloud_firewall_ip_source_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_cloud_firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_engines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_icap_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_idm_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_incident_receiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_web_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_location_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    14311 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_location_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_rule_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_security.py
--rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_traffic_gre_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_traffic_static_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_traffic_vpn_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_url_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_url_filtering_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zia/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.453035 zscaler-sdk-python-0.1.1/tests/integration/zpa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_access_policy_forwarding_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_access_policy_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_access_policy_timeout_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_app_connector_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_application_segment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_application_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_ba_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_enrolment_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_idp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_machine_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_posture_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_pra_approval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_pra_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_pra_portal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_provisioning_key_app_connector_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_provisioning_key_service_edge_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_saml_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_scim_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_scim_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_segment_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_server_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_service_edge_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/integration/zpa/test_trusted_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.457035 zscaler-sdk-python-0.1.1/zscaler/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.457035 zscaler-sdk-python-0.1.1/zscaler/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/cache/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/cache/no_op_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/cache/zscaler_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.457035 zscaler-sdk-python-0.1.1/zscaler/errors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/errors/http_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/errors/zscaler_api_error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.457035 zscaler-sdk-python-0.1.1/zscaler/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.457035 zscaler-sdk-python-0.1.1/zscaler/ratelimiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/ratelimiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/ratelimiter/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    19443 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.461035 zscaler-sdk-python-0.1.1/zscaler/zia/
--rw-r--r--   0 runner    (1001) docker     (127)    22024 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/activate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/admin_and_role_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/apptotal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/authentication_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18549 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/cloud_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/device_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    27588 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/dlp.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    40386 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/forwarding_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)    30972 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/ssl_inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    31279 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/traffic.py
--rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/url_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/url_filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/web_dlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/workload_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zia/zpa_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.465035 zscaler-sdk-python-0.1.1/zscaler/zpa/
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    24790 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/app_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12657 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/app_segments_inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/app_segments_pra.py
--rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/cloud_connector_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    20602 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/connectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/emergency_access.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/idp.py
--rw-r--r--   0 runner    (1001) docker     (127)    34889 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/inspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/isolation_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/lss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/machine_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    30654 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/posture_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    32581 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/privileged_remote_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/provisioning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/saml_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/scim_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/scim_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/segment_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/server_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/servers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15606 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/service_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-19 06:21:28.000000 zscaler-sdk-python-0.1.1/zscaler/zpa/trusted_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 06:21:36.465035 zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-04-19 06:21:36.000000 zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-19 06:21:36.000000 zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 06:21:36.000000 zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-19 06:21:36.000000 zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 06:21:36.000000 zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.284349 zscaler-sdk-python-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-04-20 22:57:24.284349 zscaler-sdk-python-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15600 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.252349 zscaler-sdk-python-0.1.2/docsrc/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.252349 zscaler-sdk-python-0.1.2/docsrc/zs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.256349 zscaler-sdk-python-0.1.2/docsrc/zs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/guides/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/guides/support.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/guides/troubleshooting.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.260349 zscaler-sdk-python-0.1.2/docsrc/zs/zia/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/activate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/admin_and_role_management.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/apptotal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/audit_logs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/authentication_settings.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/cloud_apps.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/device_management.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/dlp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/firewall.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/forwarding_control.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/isolation_profile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/locations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/rule_labels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/sandbox.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/security.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/ssl_inspection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/traffic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/url_categories.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/url_filtering.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/users.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/web_dlp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/workload_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zia/zpa_gateway.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.264349 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/app_segments.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/app_segments_inspection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/app_segments_pra.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/certificates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/cloud_connector_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/connectors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/emergency_access.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/idp.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/inspection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/isolation_profile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/lss.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/machine_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/policies.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/posture_profiles.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/privileged_remote_access.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/provisioning.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/saml_attributes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/scim_attributes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/scim_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/segment_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/server_groups.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/servers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/service_edges.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/docsrc/zs/zpa/trusted_networks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-20 22:57:24.284349 zscaler-sdk-python-0.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1750 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.264349 zscaler-sdk-python-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.252349 zscaler-sdk-python-0.1.2/tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.268349 zscaler-sdk-python-0.1.2/tests/integration/zia/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_admin_and_role_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_authentication_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_cloud_firewall_ip_destination_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_cloud_firewall_ip_source_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_cloud_firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_engines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_icap_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_idm_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_incident_receiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_web_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_isolation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_location_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14311 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_location_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_rule_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15623 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_traffic_gre_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_traffic_static_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_traffic_vpn_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9141 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_url_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_url_filtering_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zia/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.272349 zscaler-sdk-python-0.1.2/tests/integration/zpa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_access_policy_forwarding_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_access_policy_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_access_policy_timeout_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_app_connector_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_application_segment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_application_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_ba_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_enrolment_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_idp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_isolation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_machine_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_posture_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_pra_approval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_pra_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_pra_portal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_provisioning_key_app_connector_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_provisioning_key_service_edge_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_saml_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_scim_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_scim_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_segment_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_server_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_service_edge_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/integration/zpa/test_trusted_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.272349 zscaler-sdk-python-0.1.2/zscaler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.272349 zscaler-sdk-python-0.1.2/zscaler/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/cache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/cache/no_op_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/cache/zscaler_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.272349 zscaler-sdk-python-0.1.2/zscaler/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/errors/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/errors/zscaler_api_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.272349 zscaler-sdk-python-0.1.2/zscaler/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.272349 zscaler-sdk-python-0.1.2/zscaler/ratelimiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/ratelimiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/ratelimiter/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19443 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.280349 zscaler-sdk-python-0.1.2/zscaler/zia/
+-rw-r--r--   0 runner    (1001) docker     (127)    22024 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/activate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/admin_and_role_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/apptotal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/authentication_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18549 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/cloud_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/device_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27797 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/dlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40386 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/forwarding_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/isolation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30972 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/ssl_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31149 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/traffic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14744 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/url_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/url_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/web_dlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/workload_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zia/zpa_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.284349 zscaler-sdk-python-0.1.2/zscaler/zpa/
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    24790 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13393 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/app_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12657 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/app_segments_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12217 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/app_segments_pra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/cloud_connector_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20602 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/emergency_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/idp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34889 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/isolation_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21471 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/lss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/machine_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30654 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/posture_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32581 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/privileged_remote_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/provisioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/saml_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/scim_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/scim_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/segment_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/server_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15606 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/service_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4399 2024-04-20 22:57:18.000000 zscaler-sdk-python-0.1.2/zscaler/zpa/trusted_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 22:57:24.284349 zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-04-20 22:57:24.000000 zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-20 22:57:24.000000 zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 22:57:24.000000 zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-20 22:57:24.000000 zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 22:57:24.000000 zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/top_level.txt
```

### Comparing `zscaler-sdk-python-0.1.1/LICENSE.md` & `zscaler-sdk-python-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/PKG-INFO` & `zscaler-sdk-python-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler-sdk-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: Official Python SDK for the Zscaler Products (Beta)
 Home-page: https://zscaler-sdk-python.readthedocs.io
 Author: Zscaler, Inc.
 Author-email: devrel@zscaler.com
 Keywords: zscaler,sdk,zpa,zia,zdx,zcc,zcon
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `zscaler-sdk-python-0.1.1/README.md` & `zscaler-sdk-python-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/docsrc/Makefile` & `zscaler-sdk-python-0.1.2/docsrc/Makefile`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/docsrc/conf.py` & `zscaler-sdk-python-0.1.2/docsrc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
 project = "Zscaler SDK Python"
 copyright = "2023, Zscaler Inc."
 author = "Zscaler Technology Alliances"
 html_title = ""
 
 # The short X.Y version
-version = '0.1.1'
+version = '0.1.2'
 # The full version, including alpha/beta/rc tags
-release = '0.1.1'
+release = '0.1.2'
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `zscaler-sdk-python-0.1.1/docsrc/index.rst` & `zscaler-sdk-python-0.1.2/docsrc/index.rst`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/docsrc/zs/guides/examples.rst` & `zscaler-sdk-python-0.1.2/docsrc/zs/guides/examples.rst`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/docsrc/zs/guides/support.rst` & `zscaler-sdk-python-0.1.2/docsrc/zs/guides/support.rst`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/docsrc/zs/zia/url_categories.rst` & `zscaler-sdk-python-0.1.2/docsrc/zs/zia/url_categories.rst`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/setup.py` & `zscaler-sdk-python-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "zscaler.zia",
     "zscaler.zpa",
 ]
 
 package_data = {"": ["*"]}
 
 setup(name="zscaler-sdk-python",
-      version='0.1.1',
+      version='0.1.2',
       packages=find_packages(exclude=["tests", "*tests.*", "*tests"]),
       package_data=package_data,
       python_requires=">=3.8,<4.0",
       install_requires=["arrow", "certifi", "charset-normalizer", "idna", "python-box",
         "python-dateutil", "requests", "responses", "restfly", "six",
         "urllib3", "flatdict", "pyyaml", "xmltodict", "yarl",
         "pycryptodomex", "aenum", "pydash", "flake8", "pytz"],
```

### Comparing `zscaler-sdk-python-0.1.1/tests/conftest.py` & `zscaler-sdk-python-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/conftest.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/conftest.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_activation.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_activation.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_admin_and_role_management.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_admin_and_role_management.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_authentication_settings.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_authentication_settings.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_cloud_firewall_ip_destination_groups.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_cloud_firewall_ip_destination_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_cloud_firewall_ip_source_groups.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_cloud_firewall_ip_source_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_cloud_firewall_rule.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_cloud_firewall_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_dictionary.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_dictionary.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_engines.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_engines.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_icap_server.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_icap_server.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_idm_profile.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_idm_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_incident_receiver.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_saml_attributes.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,65 +13,77 @@
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 
 import pytest
 
-from tests.integration.zia.conftest import MockZIAClient
+from tests.integration.zpa.conftest import MockZPAClient
 
 
 @pytest.fixture
 def fs():
     yield
 
 
-class TestDLPIncidentReceiver:
+class TestSamlAttributes:
     """
-    Integration Tests for the DLP Incident Receiver
+    Integration Tests for the SAML attributes
     """
 
-    def test_dlp_incident_receiver(self, fs):
-        client = MockZIAClient(fs)
+    def test_saml_attributes_operations(self, fs):
+        client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
-            # List all receivers
-            receivers = client.dlp.list_dlp_incident_receiver()
-            assert isinstance(receivers, list), "Expected a list of receivers"
-            if receivers:  # If there are any receivers
-                # Select the first receiver for further testing
-                first_receiver = receivers[0]
-                receiver_id = first_receiver.get("id")
-
-                # Fetch the selected receiver by its ID
-                try:
-                    fetched_receiver = client.dlp.get_dlp_incident_receiver(receiver_id)
-                    assert (
-                        fetched_receiver is not None
-                    ), "Expected a valid receiver object"
-                    assert (
-                        fetched_receiver.get("id") == receiver_id
-                    ), "Mismatch in receiver ID"
-                except Exception as exc:
-                    errors.append(f"Fetching receiver by ID failed: {exc}")
-
-                # Attempt to retrieve the receiver by name
-                try:
-                    receiver_name = first_receiver.dlp("name")
-                    receiver_by_name = client.dlp.get_dlp_incident_receiver_by_name(
-                        receiver_name
-                    )
-                    assert (
-                        receiver_by_name is not None
-                    ), "Expected a valid receiver object when searching by name"
-                    assert (
-                        receiver_by_name.get("id") == receiver_id
-                    ), "Mismatch in receiver ID when searching by name"
-                except Exception as exc:
-                    errors.append(f"Fetching receiver by name failed: {exc}")
+            # Test listing all SAML attributes
+            resp = client.saml_attributes.list_attributes()
+            assert isinstance(
+                resp, list
+            ), "Response is not in the expected list format."
+            assert len(resp) > 0, "No SAML attributes were found."
+        except Exception as exc:
+            errors.append(f"Listing all SAML attributes failed: {exc}")
 
+        try:
+            # Test listing SAML attributes by IDP
+            idps = client.idp.list_idps()
+            user_idp = next(
+                (idp for idp in idps if "USER" in idp.get("sso_type", [])), None
+            )
+            assert user_idp is not None, "No IdP with sso_type 'USER' found."
+
+            user_idp_id = user_idp["id"]
+            resp = client.saml_attributes.list_attributes_by_idp(user_idp_id)
+            assert isinstance(
+                resp, list
+            ), "Response is not in the expected list format for IDP."
+            assert (
+                len(resp) > 0
+            ), "No SAML attributes were found for the specified IdP by ID."
+        except Exception as exc:
+            errors.append(f"Listing SAML attributes by IDP failed: {exc}")
+
+        try:
+            # Test getting a specific SAML attribute
+            attributes = client.saml_attributes.list_attributes_by_idp(user_idp["id"])
+            assert (
+                len(attributes) > 0
+            ), "No SAML attributes found for the specified IdP."
+
+            first_attribute_id = attributes[0][
+                "id"
+            ]  # Assuming attributes is a list of dicts
+            resp = client.saml_attributes.get_attribute(first_attribute_id)
+            assert isinstance(
+                resp, dict
+            ), "Response is not in the expected dict format."
+            assert (
+                resp["id"] == first_attribute_id
+            ), "Retrieved SAML attribute ID does not match the requested ID."
         except Exception as exc:
-            errors.append(f"Listing receivers failed: {exc}")
+            errors.append(f"Getting a specific SAML attribute failed: {exc}")
 
         # Assert that no errors occurred during the test
-        assert len(errors) == 0, f"Errors occurred during receivers test: {errors}"
+        assert (
+            len(errors) == 0
+        ), f"Errors occurred during SAML attributes operations test: {errors}"
```

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_dlp_web_rule.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_dlp_web_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_isolation_profile.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_location_group.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_location_group.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_location_management.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_location_management.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_rule_labels.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_rule_labels.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_sandbox.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_sandbox.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_security.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_security.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_traffic_gre_tunnel.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_traffic_gre_tunnel.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_traffic_static_ip.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_traffic_static_ip.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_traffic_vpn_credential.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_traffic_vpn_credential.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_url_categories.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_url_categories.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_url_filtering_rule.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_url_filtering_rule.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zia/test_users.py` & `zscaler-sdk-python-0.1.2/tests/integration/zia/test_users.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/conftest.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/conftest.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_access_policy_forwarding_rules.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_access_policy_forwarding_rules.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_access_policy_rules.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_access_policy_rules.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_access_policy_timeout_rules.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_access_policy_timeout_rules.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_app_connector_groups.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_app_connector_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_application_segment.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_application_segment.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_application_servers.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_application_servers.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_ba_certificates.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_ba_certificates.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_enrolment_certificates.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_enrolment_certificates.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_idp.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_idp.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_isolation_profile.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_machine_groups.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_machine_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_posture_profiles.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_posture_profiles.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_pra_approval.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_pra_approval.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_pra_credential.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_pra_credential.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_pra_portal.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_pra_portal.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_provisioning_key_app_connector_group.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_provisioning_key_app_connector_group.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_provisioning_key_service_edge_group.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_provisioning_key_service_edge_group.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_saml_attributes.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_scim_attributes.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,69 +21,57 @@
 
 
 @pytest.fixture
 def fs():
     yield
 
 
-class TestSamlAttributes:
+class TestScimAttributes:
     """
-    Integration Tests for the SAML attributes
+    Integration Tests for the SCIM attributes
     """
 
-    def test_saml_attributes_operations(self, fs):
+    def test_scim_attributes_operations(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
-            # Test listing all SAML attributes
-            resp = client.saml_attributes.list_attributes()
-            assert isinstance(
-                resp, list
-            ), "Response is not in the expected list format."
-            assert len(resp) > 0, "No SAML attributes were found."
-        except Exception as exc:
-            errors.append(f"Listing all SAML attributes failed: {exc}")
-
-        try:
-            # Test listing SAML attributes by IDP
+            # Test listing SCIM attributes by IDP
             idps = client.idp.list_idps()
             user_idp = next(
                 (idp for idp in idps if "USER" in idp.get("sso_type", [])), None
             )
             assert user_idp is not None, "No IdP with sso_type 'USER' found."
 
             user_idp_id = user_idp["id"]
-            resp = client.saml_attributes.list_attributes_by_idp(user_idp_id)
+            resp = client.scim_attributes.list_attributes_by_idp(user_idp_id)
             assert isinstance(
                 resp, list
-            ), "Response is not in the expected list format for IDP."
-            assert (
-                len(resp) > 0
-            ), "No SAML attributes were found for the specified IdP by ID."
+            ), "Response is not in the expected list format."
+            assert len(resp) > 0, "No SCIM groups were found for the specified IdP."
         except Exception as exc:
-            errors.append(f"Listing SAML attributes by IDP failed: {exc}")
+            errors.append(f"Listing SCIM attributes by IDP failed: {exc}")
 
         try:
-            # Test getting a specific SAML attribute
-            attributes = client.saml_attributes.list_attributes_by_idp(user_idp["id"])
+            # Test getting a specific SCIM attribute
+            attributes = client.scim_attributes.list_attributes_by_idp(user_idp_id)
             assert (
                 len(attributes) > 0
-            ), "No SAML attributes found for the specified IdP."
+            ), "No SCIM attributes found for the specified IdP."
 
             first_attribute_id = attributes[0][
                 "id"
             ]  # Assuming attributes is a list of dicts
-            resp = client.saml_attributes.get_attribute(first_attribute_id)
+            resp = client.scim_attributes.get_attribute(user_idp_id, first_attribute_id)
             assert isinstance(
                 resp, dict
             ), "Response is not in the expected dict format."
             assert (
                 resp["id"] == first_attribute_id
-            ), "Retrieved SAML attribute ID does not match the requested ID."
+            ), "Retrieved SCIM attribute ID does not match the requested ID."
         except Exception as exc:
-            errors.append(f"Getting a specific SAML attribute failed: {exc}")
+            errors.append(f"Getting a specific SCIM attribute failed: {exc}")
 
         # Assert that no errors occurred during the test
         assert (
             len(errors) == 0
-        ), f"Errors occurred during SAML attributes operations test: {errors}"
+        ), f"Errors occurred during SCIM attributes operations test: {errors}"
```

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_scim_attributes.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_scim_groups.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,57 +21,55 @@
 
 
 @pytest.fixture
 def fs():
     yield
 
 
-class TestScimAttributes:
+class TestScimGroups:
     """
-    Integration Tests for the SCIM attributes
+    Integration Tests for the SCIM Groups
     """
 
-    def test_scim_attributes_operations(self, fs):
+    def test_scim_groups_operations(self, fs):
         client = MockZPAClient(fs)
         errors = []  # Initialize an empty list to collect errors
 
         try:
-            # Test listing SCIM attributes by IDP
+            # Test listing SCIM groups
             idps = client.idp.list_idps()
             user_idp = next(
                 (idp for idp in idps if "USER" in idp.get("sso_type", [])), None
             )
             assert user_idp is not None, "No IdP with sso_type 'USER' found."
 
             user_idp_id = user_idp["id"]
-            resp = client.scim_attributes.list_attributes_by_idp(user_idp_id)
+            resp = client.scim_groups.list_groups(user_idp_id)
             assert isinstance(
                 resp, list
             ), "Response is not in the expected list format."
             assert len(resp) > 0, "No SCIM groups were found for the specified IdP."
         except Exception as exc:
-            errors.append(f"Listing SCIM attributes by IDP failed: {exc}")
+            errors.append(f"Listing SCIM groups failed: {exc}")
 
         try:
-            # Test getting a specific SCIM attribute
-            attributes = client.scim_attributes.list_attributes_by_idp(user_idp_id)
-            assert (
-                len(attributes) > 0
-            ), "No SCIM attributes found for the specified IdP."
+            # Test getting a specific SCIM group
+            scim_groups = client.scim_groups.list_groups(user_idp_id)
+            assert len(scim_groups) > 0, "No SCIM groups found for the specified IdP."
 
-            first_attribute_id = attributes[0][
+            first_group_id = scim_groups[0][
                 "id"
-            ]  # Assuming attributes is a list of dicts
-            resp = client.scim_attributes.get_attribute(user_idp_id, first_attribute_id)
+            ]  # Assuming scim_groups is a list of dicts
+            resp = client.scim_groups.get_group(first_group_id)
             assert isinstance(
                 resp, dict
             ), "Response is not in the expected dict format."
             assert (
-                resp["id"] == first_attribute_id
-            ), "Retrieved SCIM attribute ID does not match the requested ID."
+                resp["id"] == first_group_id
+            ), "Retrieved SCIM group ID does not match the requested ID."
         except Exception as exc:
-            errors.append(f"Getting a specific SCIM attribute failed: {exc}")
+            errors.append(f"Getting a specific SCIM group failed: {exc}")
 
         # Assert that no errors occurred during the test
         assert (
             len(errors) == 0
-        ), f"Errors occurred during SCIM attributes operations test: {errors}"
+        ), f"Errors occurred during SCIM groups operations test: {errors}"
```

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_segment_groups.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_segment_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_server_groups.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_server_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_service_edge_groups.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_service_edge_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/integration/zpa/test_trusted_networks.py` & `zscaler-sdk-python-0.1.2/tests/integration/zpa/test_trusted_networks.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/tests/test_utils.py` & `zscaler-sdk-python-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/__init__.py` & `zscaler-sdk-python-0.1.2/zscaler/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,11 +16,11 @@
 
 __author__ = "Zscaler Inc"
 __email__ = "devrel@zscaler.com"
 __license__ = "MIT"
 __contributors__ = [
     "William Guilherme",
 ]
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 from zscaler.zia import ZIAClientHelper  # noqa
 from zscaler.zpa import ZPAClientHelper  # noqa
```

### Comparing `zscaler-sdk-python-0.1.1/zscaler/cache/cache.py` & `zscaler-sdk-python-0.1.2/zscaler/cache/cache.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/cache/no_op_cache.py` & `zscaler-sdk-python-0.1.2/zscaler/cache/no_op_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/cache/zscaler_cache.py` & `zscaler-sdk-python-0.1.2/zscaler/cache/zscaler_cache.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/constants.py` & `zscaler-sdk-python-0.1.2/zscaler/constants.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/errors/http_error.py` & `zscaler-sdk-python-0.1.2/zscaler/errors/http_error.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/errors/zscaler_api_error.py` & `zscaler-sdk-python-0.1.2/zscaler/errors/zscaler_api_error.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/exceptions/exceptions.py` & `zscaler-sdk-python-0.1.2/zscaler/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/logger.py` & `zscaler-sdk-python-0.1.2/zscaler/logger.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/ratelimiter/ratelimiter.py` & `zscaler-sdk-python-0.1.2/zscaler/ratelimiter/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/user_agent.py` & `zscaler-sdk-python-0.1.2/zscaler/user_agent.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/utils.py` & `zscaler-sdk-python-0.1.2/zscaler/utils.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/__init__.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/activate.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/activate.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/admin_and_role_management.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/admin_and_role_management.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/apptotal.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/apptotal.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/audit_logs.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/audit_logs.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/authentication_settings.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/authentication_settings.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/client.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/client.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/cloud_apps.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/cloud_apps.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/device_management.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/device_management.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/dlp.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/dlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -462,19 +462,23 @@
             ...    pprint(icap)
 
             Print icaps that match the name or description 'ZS_ICAP'
 
             >>> pprint(zia.dlp.list_dlp_icap_servers('ZS_ICAP'))
 
         """
-        payload = {"search": query}
-        list = self.rest.get(path="/icapServers", params=payload)
-        if isinstance(list, Response):
+        response = self.rest.get("/icapServers")
+        if isinstance(response, Response):
             return None
-        return list
+        return response
+        # payload = {"search": query}
+        # list = self.rest.get(path="/icapServers", params=payload)
+        # if isinstance(list, Response):
+        #     return None
+        # return list
 
     def get_dlp_icap_servers(self, icap_server_id: str) -> Box:
         """
         Returns the dlp icap server details for a given DLP ICAP Server.
 
         Args:
             icap_server_id (str): The unique identifier for the DLP ICAP Server.
@@ -507,27 +511,26 @@
 
         Returns:
             :obj:`BoxList`: A list containing ZIA DLP Incident Receiver.
 
         Examples:
             Print all incident receivers
 
-            >>> for dlp incident receiver in zia.dlp.list_dlp_incident_receiver():
-            ...    pprint(receiver)
+            >>> for receiver in zia.dlp.list_dlp_incident_receiver():
+            ...    pprint(dlp)
 
             Print Incident Receiver that match the name or description 'ZS_INC_RECEIVER_01'
 
             >>> pprint(zia.dlp.list_dlp_incident_receiver('ZS_INC_RECEIVER_01'))
 
         """
-        payload = {"search": query}
-        response = self.rest.get(path="/incidentReceiverServers", params=payload)
-        if isinstance(response, Response) and response.ok:
-            return response.json()
-        return []  # Return an empty list in case of no data or error
+        response = self.rest.get("/incidentReceiverServers")
+        if isinstance(response, Response):
+            return None
+        return response
 
     def get_dlp_incident_receiver(self, receiver_id: str) -> Box:
         """
         Returns the dlp incident receiver details for a given DLP Incident Receiver.
 
         Args:
             receiver_id (str): The unique identifier for the DLP Incident Receiver.
@@ -541,21 +544,31 @@
         """
         response = self.rest.get("/incidentReceiverServers/%s" % (receiver_id))
         if isinstance(response, Response):
             return None
         return response
 
     def get_dlp_incident_receiver_by_name(self, name):
-        # Fetch all receivers (assuming the API doesn't support server-side filtering by name)
+        """
+        Retrieves a specific DLP Incident Receiver by its name.
+
+        Args:
+            name (str): The name of the dlp incident receiver to retrieve.
+
+        Returns:
+            :obj:`Box`: The incident receiver if found, otherwise None.
+
+        Examples:
+            >>> receiver = zia.dlp.get_dlp_incident_receiver_by_name('ZS_INC_RECEIVER_01')
+            ...    pprint(receiver)
+        """
         receivers = self.list_dlp_incident_receiver()
-        # Iterate through the receivers to find a match by name
         for receiver in receivers:
             if receiver.get("name") == name:
                 return receiver
-        # If no receiver matches the given name
         return None
 
     def list_dlp_idm_profiles(self, query: str = None) -> BoxList:
         """
         Returns the list of ZIA DLP IDM Profiles.
 
         Args:
```

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/errors.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/firewall.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/firewall.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/forwarding_control.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/forwarding_control.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/isolation_profile.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/labels.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/labels.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/locations.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/locations.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/sandbox.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/sandbox.py`

 * *Files 10% similar despite different names*

```diff
@@ -150,14 +150,35 @@
 
         Examples:
             >>> pprint(zia.sandbox.get_behavioral_analysis())
 
         """
         return self.rest.get("behavioralAnalysisAdvancedSettings")
 
+    def get_file_hash_count(self) -> Box:
+        """
+        Retrieves the Cloud Sandbox used and unused quota for blocking MD5 file hashes.
+
+        This method fetches the count of MD5 hashes currently blocked by the Sandbox and the remaining
+        quota available for blocking additional hashes.
+
+        Returns:
+            Box: A Box object containing the used and unused quotas for MD5 hash blocking.
+
+        Examples:
+            >>> file_hash_quota = zia.sandbox.get_file_hash_count()
+            >>> pprint(file_hash_quota)
+
+        The returned Box object contains the following keys:
+        - blocked_file_hashes_count: The number of unique MD5 file hashes that are currently blocked.
+        - remaining_file_hashes: The remaining quota available for blocking additional MD5 file hashes.
+        """
+        response = self.rest.get("behavioralAnalysisAdvancedSettings/fileHashCount")
+        return response
+
     def add_hash_to_custom_list(self, file_hashes_to_be_blocked: list) -> Box:
         """
         Updates the custom list of MD5 file hashes that are blocked by Sandbox.
 
         Args:
             file_hashes_to_be_blocked (:obj:`list` of :obj:`str`):
                 The list of MD5 Hashes to be added. Pass an empty list to clear the blocklist.
```

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/security.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/security.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/ssl_inspection.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/ssl_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/traffic.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/traffic.py`

 * *Files 0% similar despite different names*

```diff
@@ -689,18 +689,14 @@
             location_id (str):
                 Associate the VPN credential with an existing location.
 
         Returns:
             :obj:`Box`: The newly created VPN credential resource record.
         """
 
-        # Generate a random PSK if not provided
-        if not pre_shared_key:
-            pre_shared_key = self.randomize_psk()
-
         payload = {
             "type": authentication_type,
             "preSharedKey": pre_shared_key,
         }
 
         # Add location ID to payload if specified.
         if kwargs.get("location_id"):
```

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/url_categories.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/url_categories.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/url_filtering.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/url_filtering.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/users.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/users.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/web_dlp.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/web_dlp.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/workload_groups.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/workload_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zia/zpa_gateway.py` & `zscaler-sdk-python-0.1.2/zscaler/zia/zpa_gateway.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/README.md` & `zscaler-sdk-python-0.1.2/zscaler/zpa/README.md`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/__init__.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/__init__.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/app_segments.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/app_segments.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/app_segments_inspection.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/app_segments_inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/app_segments_pra.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/app_segments_pra.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/certificates.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/certificates.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/client.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/client.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/cloud_connector_groups.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/cloud_connector_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/connectors.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/connectors.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/emergency_access.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/emergency_access.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/errors.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/errors.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/idp.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/idp.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/inspection.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/inspection.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/isolation_profile.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/isolation_profile.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/lss.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/lss.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/machine_groups.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/machine_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/policies.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/policies.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/posture_profiles.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/posture_profiles.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/privileged_remote_access.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/privileged_remote_access.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/provisioning.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/provisioning.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/saml_attributes.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/saml_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/scim_attributes.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/scim_attributes.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/scim_groups.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/scim_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/segment_groups.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/segment_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/server_groups.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/server_groups.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/servers.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/servers.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/service_edges.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/service_edges.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler/zpa/trusted_networks.py` & `zscaler-sdk-python-0.1.2/zscaler/zpa/trusted_networks.py`

 * *Files identical despite different names*

### Comparing `zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/PKG-INFO` & `zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zscaler-sdk-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: Official Python SDK for the Zscaler Products (Beta)
 Home-page: https://zscaler-sdk-python.readthedocs.io
 Author: Zscaler, Inc.
 Author-email: devrel@zscaler.com
 Keywords: zscaler,sdk,zpa,zia,zdx,zcc,zcon
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `zscaler-sdk-python-0.1.1/zscaler_sdk_python.egg-info/SOURCES.txt` & `zscaler-sdk-python-0.1.2/zscaler_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

