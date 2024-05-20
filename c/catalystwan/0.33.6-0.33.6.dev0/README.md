# Comparing `tmp/catalystwan-0.33.6.tar.gz` & `tmp/catalystwan-0.33.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystwan-0.33.6.tar", max compression
+gzip compressed data, was "catalystwan-0.33.6.dev0.tar", max compression
```

## Comparing `catalystwan-0.33.6.tar` & `catalystwan-0.33.6.dev0.tar`

### file list

```diff
@@ -1,344 +1,542 @@
--rw-r--r--   0        0        0    11375 2024-05-14 22:23:34.199131 catalystwan-0.33.6/LICENSE
--rw-r--r--   0        0        0    13654 2024-05-14 22:23:34.199131 catalystwan-0.33.6/README.md
--rw-r--r--   0        0        0     2524 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/__init__.py
--rw-r--r--   0        0        0     1533 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/abstractions.py
--rw-r--r--   0        0        0        0 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/__init__.py
--rw-r--r--   0        0        0     6689 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/admin_tech_api.py
--rw-r--r--   0        0        0    14935 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/administration.py
--rw-r--r--   0        0        0     6314 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/alarms_api.py
--rw-r--r--   0        0        0     3220 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/api_container.py
--rw-r--r--   0        0        0    11636 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/basic_api.py
--rw-r--r--   0        0        0     2053 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/config_device_inventory_api.py
--rw-r--r--   0        0        0     4301 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/config_group_api.py
--rw-r--r--   0        0        0     4645 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/configuration_groups/parcel.py
--rw-r--r--   0        0        0     1290 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/configuration_groups/parcels/cellular_controller.py
--rw-r--r--   0        0        0     7315 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/dashboard_api.py
--rw-r--r--   0        0        0     7360 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/device_action_api.py
--rw-r--r--   0        0        0    15767 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/feature_profile_api.py
--rw-r--r--   0        0        0     1919 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/logs_api.py
--rw-r--r--   0        0        0     2449 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/monitoring_status_api.py
--rw-r--r--   0        0        0     6036 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/mtt_aaa_api.py
--rw-r--r--   0        0        0     4394 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/omp_api.py
--rw-r--r--   0        0        0     5691 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/packet_capture_api.py
--rw-r--r--   0        0        0     1654 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/parcel_api.py
--rw-r--r--   0        0        0     5600 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/partition_manager_api.py
--rw-r--r--   0        0        0    28976 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/policy_api.py
--rw-r--r--   0        0        0     2284 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/resource_pool_api.py
--rw-r--r--   0        0        0    11320 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/software_action_api.py
--rw-r--r--   0        0        0     5473 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/speedtest_api.py
--rw-r--r--   0        0        0     7149 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/task_status_api.py
--rw-r--r--   0        0        0    29260 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/template_api.py
--rw-r--r--   0        0        0     3540 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/templates/README.md
--rw-r--r--   0        0        0      251 2024-05-14 22:23:34.199131 catalystwan-0.33.6/catalystwan/api/templates/bool_str.py
--rw-r--r--   0        0        0     7481 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/cli_template.py
--rw-r--r--   0        0        0     3107 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/device_template/device_template.py
--rw-r--r--   0        0        0      571 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/device_template/device_template_payload.json.j2
--rw-r--r--   0        0        0      137 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/device_variable.py
--rw-r--r--   0        0        0     5235 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/feature_template.py
--rw-r--r--   0        0        0     6576 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/feature_template_field.py
--rw-r--r--   0        0        0      661 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/feature_template_payload.py
--rw-r--r--   0        0        0     3244 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_aaa_model.py
--rw-r--r--   0        0        0      667 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_banner_model.py
--rw-r--r--   0        0        0     2180 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_bfd_model.py
--rw-r--r--   0        0        0    12522 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_bgp_model.py
--rw-r--r--   0        0        0     3436 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_logging_model.py
--rw-r--r--   0        0        0     1584 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_ntp_model.py
--rw-r--r--   0        0        0     3835 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_omp_model.py
--rw-r--r--   0        0        0     6749 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_ospf.py
--rw-r--r--   0        0        0    13901 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_ospfv3.py
--rw-r--r--   0        0        0     9589 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
--rw-r--r--   0        0        0     2581 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_snmp_model.py
--rw-r--r--   0        0        0     8986 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_system.py
--rw-r--r--   0        0        0    21665 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_vpn_interface_model.py
--rw-r--r--   0        0        0    15836 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cisco_vpn_model.py
--rw-r--r--   0        0        0      472 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/cli_template.py
--rw-r--r--   0        0        0     1835 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/omp_vsmart_model.py
--rw-r--r--   0        0        0      806 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/security_vsmart_model.py
--rw-r--r--   0        0        0     1882 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/supported.py
--rw-r--r--   0        0        0     2624 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/models/system_vsmart_model.py
--rw-r--r--   0        0        0     2261 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/aaa_model.py
--rw-r--r--   0        0        0    11178 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
--rw-r--r--   0        0        0     1041 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
--rw-r--r--   0        0        0     4264 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
--rw-r--r--   0        0        0     3735 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
--rw-r--r--   0        0        0     1999 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
--rw-r--r--   0        0        0     2558 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
--rw-r--r--   0        0        0     4547 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
--rw-r--r--   0        0        0     1843 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
--rw-r--r--   0        0        0     2247 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
--rw-r--r--   0        0        0     2098 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
--rw-r--r--   0        0        0      683 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
--rw-r--r--   0        0        0     7113 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/tenant/tenant.json.j2
--rw-r--r--   0        0        0     1460 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/templates/payloads/tenant/tenant_model.py
--rw-r--r--   0        0        0     5013 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/tenant_backup_restore_api.py
--rw-r--r--   0        0        0     4406 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/tenant_management_api.py
--rw-r--r--   0        0        0     5090 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/tenant_migration_api.py
--rw-r--r--   0        0        0    15887 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/versions_utils.py
--rw-r--r--   0        0        0     7715 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/api/virtual_image_action_api.py
--rw-r--r--   0        0        0    21802 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/dataclasses.py
--rw-r--r--   0        0        0    25866 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/__init__.py
--rw-r--r--   0        0        0    11938 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/administration_user_and_group.py
--rw-r--r--   0        0        0     6731 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/certificate_management_device.py
--rw-r--r--   0        0        0     1476 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/certificate_management_vmanage.py
--rw-r--r--   0        0        0     4035 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/client.py
--rw-r--r--   0        0        0     2722 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/cluster_management.py
--rw-r--r--   0        0        0      983 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/device/software_update.py
--rw-r--r--   0        0        0     9447 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/disaster_recovery.py
--rw-r--r--   0        0        0     4037 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
--rw-r--r--   0        0        0     2064 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
--rw-r--r--   0        0        0     4836 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
--rw-r--r--   0        0        0     2028 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
--rw-r--r--   0        0        0     2091 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
--rw-r--r--   0        0        0     2092 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/control.py
--rw-r--r--   0        0        0     2247 2024-05-14 22:23:34.203131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/device_access.py
--rw-r--r--   0        0        0     2324 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
--rw-r--r--   0        0        0     2174 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
--rw-r--r--   0        0        0     2032 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/mesh.py
--rw-r--r--   0        0        0     2073 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/qos_map.py
--rw-r--r--   0        0        0     2132 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/rewrite.py
--rw-r--r--   0        0        0     2039 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/rule_set.py
--rw-r--r--   0        0        0     2159 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/security_group.py
--rw-r--r--   0        0        0     2104 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
--rw-r--r--   0        0        0     2263 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
--rw-r--r--   0        0        0     2186 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
--rw-r--r--   0        0        0     1793 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/app.py
--rw-r--r--   0        0        0     1950 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/app_probe.py
--rw-r--r--   0        0        0     1848 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/as_path.py
--rw-r--r--   0        0        0     1870 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/class_map.py
--rw-r--r--   0        0        0     1827 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/color.py
--rw-r--r--   0        0        0     1911 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/community.py
--rw-r--r--   0        0        0     2016 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
--rw-r--r--   0        0        0     1932 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/data_prefix.py
--rw-r--r--   0        0        0     2079 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/expanded_community.py
--rw-r--r--   0        0        0     1806 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/fqdn.py
--rw-r--r--   0        0        0     1953 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/geo_location.py
--rw-r--r--   0        0        0     1974 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/ips_signature.py
--rw-r--r--   0        0        0     1932 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
--rw-r--r--   0        0        0     1890 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/local_app.py
--rw-r--r--   0        0        0     1953 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/local_domain.py
--rw-r--r--   0        0        0     1848 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/mirror.py
--rw-r--r--   0        0        0     1874 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/policer.py
--rw-r--r--   0        0        0     1806 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/port.py
--rw-r--r--   0        0        0     2115 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
--rw-r--r--   0        0        0     1848 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/prefix.py
--rw-r--r--   0        0        0     1974 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/protocol_name.py
--rw-r--r--   0        0        0     1781 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/region.py
--rw-r--r--   0        0        0     1946 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/site.py
--rw-r--r--   0        0        0     1845 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/sla.py
--rw-r--r--   0        0        0     1806 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/tloc.py
--rw-r--r--   0        0        0     1926 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
--rw-r--r--   0        0        0     1926 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/url_block_list.py
--rw-r--r--   0        0        0     1787 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/vpn.py
--rw-r--r--   0        0        0     1806 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/zone.py
--rw-r--r--   0        0        0     1782 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/security_template.py
--rw-r--r--   0        0        0     1738 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/vedge_template.py
--rw-r--r--   0        0        0     2974 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/vsmart_template.py
--rw-r--r--   0        0        0     8865 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration/software_actions.py
--rw-r--r--   0        0        0     6820 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_dashboard_status.py
--rw-r--r--   0        0        0    13587 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_device_actions.py
--rw-r--r--   0        0        0    13973 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_device_inventory.py
--rw-r--r--   0        0        0      881 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_device_template.py
--rw-r--r--   0        0        0     5277 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_feature_profile.py
--rw-r--r--   0        0        0     5158 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_group.py
--rw-r--r--   0        0        0    24950 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/configuration_settings.py
--rw-r--r--   0        0        0    14444 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/endpoints_container.py
--rw-r--r--   0        0        0      760 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/misc.py
--rw-r--r--   0        0        0     8272 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/monitoring/device_details.py
--rw-r--r--   0        0        0      400 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/monitoring/security_policy.py
--rw-r--r--   0        0        0      347 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/monitoring/server_info.py
--rw-r--r--   0        0        0     1929 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/monitoring/status.py
--rw-r--r--   0        0        0     1446 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/real_time_monitoring/reboot_history.py
--rw-r--r--   0        0        0     1419 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/sdavc_cloud_connector.py
--rw-r--r--   0        0        0     1047 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/tenant_backup_restore.py
--rw-r--r--   0        0        0     7648 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/tenant_management.py
--rw-r--r--   0        0        0     3582 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/tenant_migration.py
--rw-r--r--   0        0        0     3661 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
--rw-r--r--   0        0        0      802 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/endpoints/url_monitoring.py
--rw-r--r--   0        0        0     5714 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/exceptions.py
--rw-r--r--   0        0        0     1902 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/integration_tests/test_find_template_values.py
--rw-r--r--   0        0        0      676 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/logging.conf
--rw-r--r--   0        0        0     3079 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/common.py
--rw-r--r--   0        0        0      171 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/common.py
--rw-r--r--   0        0        0     1090 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/config_migration.py
--rw-r--r--   0        0        0    10043 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/README.md
--rw-r--r--   0        0        0      663 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/builder.py
--rw-r--r--   0        0        0     9117 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/common.py
--rw-r--r--   0        0        0     1086 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/management/vpn.py
--rw-r--r--   0        0        0     5553 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
--rw-r--r--   0        0        0     1342 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
--rw-r--r--   0        0        0     1121 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
--rw-r--r--   0        0        0      577 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
--rw-r--r--   0        0        0     1033 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
--rw-r--r--   0        0        0      885 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
--rw-r--r--   0        0        0      731 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
--rw-r--r--   0        0        0     1034 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
--rw-r--r--   0        0        0     1034 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
--rw-r--r--   0        0        0     1268 2024-05-14 22:23:34.207131 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py
--rw-r--r--   0        0        0     2867 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
--rw-r--r--   0        0        0     1028 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
--rw-r--r--   0        0        0     5197 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
--rw-r--r--   0        0        0      925 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
--rw-r--r--   0        0        0     1581 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
--rw-r--r--   0        0        0     1177 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
--rw-r--r--   0        0        0      759 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
--rw-r--r--   0        0        0      738 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
--rw-r--r--   0        0        0     1182 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
--rw-r--r--   0        0        0     1496 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
--rw-r--r--   0        0        0      801 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
--rw-r--r--   0        0        0      691 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
--rw-r--r--   0        0        0     1131 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
--rw-r--r--   0        0        0      883 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
--rw-r--r--   0        0        0     1384 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
--rw-r--r--   0        0        0    14665 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
--rw-r--r--   0        0        0     8961 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
--rw-r--r--   0        0        0    14020 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
--rw-r--r--   0        0        0     3448 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
--rw-r--r--   0        0        0     3835 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
--rw-r--r--   0        0        0     2777 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
--rw-r--r--   0        0        0    14424 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
--rw-r--r--   0        0        0     9128 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
--rw-r--r--   0        0        0     6575 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
--rw-r--r--   0        0        0     7971 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
--rw-r--r--   0        0        0    24489 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
--rw-r--r--   0        0        0    10081 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
--rw-r--r--   0        0        0     3294 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
--rw-r--r--   0        0        0     6725 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
--rw-r--r--   0        0        0    11900 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
--rw-r--r--   0        0        0     6391 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
--rw-r--r--   0        0        0     6993 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
--rw-r--r--   0        0        0     5179 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
--rw-r--r--   0        0        0     3790 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
--rw-r--r--   0        0        0     5294 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
--rw-r--r--   0        0        0    13826 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
--rw-r--r--   0        0        0     2179 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
--rw-r--r--   0        0        0      167 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/configuration/profile_type.py
--rw-r--r--   0        0        0     1041 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/device_inventory.py
--rw-r--r--   0        0        0      341 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/feature_profile_parcel.py
--rw-r--r--   0        0        0      785 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/misc/application_protocols.py
--rw-r--r--   0        0        0      346 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/monitoring/security_policy.py
--rw-r--r--   0        0        0      405 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/monitoring/server_info.py
--rw-r--r--   0        0        0     4567 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/__init__.py
--rw-r--r--   0        0        0     9426 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/centralized.py
--rw-r--r--   0        0        0     5540 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/access_control_list.py
--rw-r--r--   0        0        0     5726 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/access_control_list_ipv6.py
--rw-r--r--   0        0        0    11851 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/control.py
--rw-r--r--   0        0        0     3861 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/device_access.py
--rw-r--r--   0        0        0     3961 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/device_access_ipv6.py
--rw-r--r--   0        0        0     3004 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/hub_and_spoke.py
--rw-r--r--   0        0        0     1184 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/mesh.py
--rw-r--r--   0        0        0     3454 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/qos_map.py
--rw-r--r--   0        0        0     1193 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/rewrite.py
--rw-r--r--   0        0        0    12252 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/rule_set.py
--rw-r--r--   0        0        0     2948 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/security_group.py
--rw-r--r--   0        0        0    13309 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/traffic_data.py
--rw-r--r--   0        0        0     1074 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/vpn_membership.py
--rw-r--r--   0        0        0     9345 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/definitions/zone_based_firewall.py
--rw-r--r--   0        0        0    10893 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/lists.py
--rw-r--r--   0        0        0    14613 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/lists_entries.py
--rw-r--r--   0        0        0     5558 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/localized.py
--rw-r--r--   0        0        0     3553 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/policy.py
--rw-r--r--   0        0        0    31904 2024-05-14 22:23:34.211130 catalystwan-0.33.6/catalystwan/models/policy/policy_definition.py
--rw-r--r--   0        0        0     1274 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/models/policy/policy_list.py
--rw-r--r--   0        0        0     7100 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/models/policy/security.py
--rw-r--r--   0        0        0     5239 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/models/tenant.py
--rw-r--r--   0        0        0      924 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/models/url_monitoring.py
--rw-r--r--   0        0        0     9586 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/response.py
--rw-r--r--   0        0        0    19488 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/session.py
--rw-r--r--   0        0        0      401 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
--rw-r--r--   0        0        0      513 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/banner_1.json
--rw-r--r--   0        0        0      116 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/alias.json
--rw-r--r--   0        0        0      114 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/basic.json
--rw-r--r--   0        0        0      109 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/basic_no_value.json
--rw-r--r--   0        0        0      848 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/children.json
--rw-r--r--   0        0        0     2348 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/children_nested.json
--rw-r--r--   0        0        0     2348 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      274 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/data_path.json
--rw-r--r--   0        0        0     2973 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/cisco_bfd.json
--rw-r--r--   0        0        0    11100 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/complex_aaa.json
--rw-r--r--   0        0        0    41165 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
--rw-r--r--   0        0        0     5219 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/default_cisco_system.json
--rw-r--r--   0        0        0     5505 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/iuo.json
--rw-r--r--   0        0        0      249 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/omp_1.json
--rw-r--r--   0        0        0      875 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/omp_2.json
--rw-r--r--   0        0        0     1682 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/definitions/omp_3.json
--rw-r--r--   0        0        0      662 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/__init__.py
--rw-r--r--   0        0        0     2828 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_aaa.py
--rw-r--r--   0        0        0      303 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_banner.py
--rw-r--r--   0        0        0      587 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_bfd.py
--rw-r--r--   0        0        0      344 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_system.py
--rw-r--r--   0        0        0     8078 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_vpn.py
--rw-r--r--   0        0        0     1091 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/models/omp_vsmart.py
--rw-r--r--   0        0        0      605 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/alias.json
--rw-r--r--   0        0        0      574 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/basic.json
--rw-r--r--   0        0        0     1810 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/children.json
--rw-r--r--   0        0        0     4005 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/children_nested.json
--rw-r--r--   0        0        0     4005 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      731 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/data_path.json
--rw-r--r--   0        0        0    43436 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/cedge_aaa.json
--rw-r--r--   0        0        0     1200 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_banner.json
--rw-r--r--   0        0        0     9495 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_bfd.json
--rw-r--r--   0        0        0    99045 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_system.json
--rw-r--r--   0        0        0    87854 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_vpn.json
--rw-r--r--   0        0        0     5939 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/schemas/omp-vsmart.json
--rw-r--r--   0        0        0     1381 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/test_chose_model.py
--rw-r--r--   0        0        0     2598 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/test_deserialize_model.py
--rw-r--r--   0        0        0     4598 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/test_generate_payload.py
--rw-r--r--   0        0        0     1756 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/templates/test_serialize_model.py
--rw-r--r--   0        0        0     8145 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_admin_tech_api.py
--rw-r--r--   0        0        0    17792 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_administration.py
--rw-r--r--   0        0        0    11116 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_alarms_api.py
--rw-r--r--   0        0        0     8322 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_cli_template.py
--rw-r--r--   0        0        0     5494 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_creation_tools.py
--rw-r--r--   0        0        0     3981 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_device_action_api.py
--rw-r--r--   0        0        0    28159 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_devices_api.py
--rw-r--r--   0        0        0    33583 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_endpoints.py
--rw-r--r--   0        0        0      894 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_feature_template_field.py
--rw-r--r--   0        0        0     1545 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_logs_api.py
--rw-r--r--   0        0        0     2896 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_monitoring_security_policy.py
--rw-r--r--   0        0        0     1809 2024-05-14 22:23:34.215131 catalystwan-0.33.6/catalystwan/tests/test_monitoring_server_info.py
--rw-r--r--   0        0        0     5489 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_monitoring_status_api.py
--rw-r--r--   0        0        0    11026 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_mtt_aaa_api.py
--rw-r--r--   0        0        0    16472 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_omp_api.py
--rw-r--r--   0        0        0     5223 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_packet_capture.py
--rw-r--r--   0        0        0     5727 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_partition_manager_api.py
--rw-r--r--   0        0        0     7440 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_response.py
--rw-r--r--   0        0        0     6724 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_session.py
--rw-r--r--   0        0        0     7117 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_software_action_api.py
--rw-r--r--   0        0        0     6071 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_speed_test_api.py
--rw-r--r--   0        0        0    14926 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_task_status_api.py
--rw-r--r--   0        0        0    15050 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_templates.py
--rw-r--r--   0        0        0     3705 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_tenant_backup_restore_api.py
--rw-r--r--   0        0        0     6114 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_tenant_management_api.py
--rw-r--r--   0        0        0     4506 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_tenant_migration_api.py
--rw-r--r--   0        0        0    11346 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_typed_list.py
--rw-r--r--   0        0        0     3746 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_url_monitoring.py
--rw-r--r--   0        0        0     2968 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_version.py
--rw-r--r--   0        0        0    10377 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_version_utils.py
--rw-r--r--   0        0        0     3343 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/tests/test_vmanage_auth.py
--rw-r--r--   0        0        0     8547 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/typed_list.py
--rw-r--r--   0        0        0        0 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/__init__.py
--rw-r--r--   0        0        0      266 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/alarm_status.py
--rw-r--r--   0        0        0      253 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/certificate_status.py
--rw-r--r--   0        0        0      279 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/colors.py
--rw-r--r--   0        0        0      154 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/config_status.py
--rw-r--r--   0        0        0     4778 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/creation_tools.py
--rw-r--r--   0        0        0     7281 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/dashboard.py
--rw-r--r--   0        0        0     2863 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/device_model.py
--rw-r--r--   0        0        0     2110 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/dict.py
--rw-r--r--   0        0        0      953 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/feature_template/choose_model.py
--rw-r--r--   0        0        0     5066 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/feature_template/find_template_values.py
--rw-r--r--   0        0        0      584 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/operation_status.py
--rw-r--r--   0        0        0      196 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/personality.py
--rw-r--r--   0        0        0      360 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/pydantic_field.py
--rw-r--r--   0        0        0      172 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/reachability.py
--rw-r--r--   0        0        0      407 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/session_type.py
--rw-r--r--   0        0        0      149 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/template_type.py
--rw-r--r--   0        0        0    17168 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/timezone.py
--rw-r--r--   0        0        0     3930 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/upgrades_helper.py
--rw-r--r--   0        0        0      159 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/utils/validate_status.py
--rw-r--r--   0        0        0     3032 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/version.py
--rw-r--r--   0        0        0     5415 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/vmanage_auth.py
--rw-r--r--   0        0        0     9946 2024-05-14 22:23:34.219131 catalystwan-0.33.6/catalystwan/workflows/tenant_migration.py
--rw-r--r--   0        0        0      862 2024-05-14 22:23:34.219131 catalystwan-0.33.6/pyproject.toml
--rw-r--r--   0        0        0    17267 1970-01-01 00:00:00.000000 catalystwan-0.33.6/setup.py
--rw-r--r--   0        0        0    14781 1970-01-01 00:00:00.000000 catalystwan-0.33.6/PKG-INFO
+-rw-r--r--   0        0        0    11375 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/LICENSE
+-rw-r--r--   0        0        0    13533 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/README.md
+-rw-r--r--   0        0        0     2558 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/__init__.py
+-rw-r--r--   0        0        0     1532 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/abstractions.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/__init__.py
+-rw-r--r--   0        0        0     6689 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/admin_tech_api.py
+-rw-r--r--   0        0        0    14935 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/administration.py
+-rw-r--r--   0        0        0     6314 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/alarms_api.py
+-rw-r--r--   0        0        0     3293 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/api_container.py
+-rw-r--r--   0        0        0    11636 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/basic_api.py
+-rw-r--r--   0        0        0      386 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/builders/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/builders/feature_profiles/__init__.py
+-rw-r--r--   0        0        0     2017 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/builders/feature_profiles/builder_factory.py
+-rw-r--r--   0        0        0     2679 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/builders/feature_profiles/cli.py
+-rw-r--r--   0        0        0     2696 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/builders/feature_profiles/other.py
+-rw-r--r--   0        0        0     3146 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/builders/feature_profiles/report.py
+-rw-r--r--   0        0        0     5727 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/builders/feature_profiles/service.py
+-rw-r--r--   0        0        0     2768 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/builders/feature_profiles/system.py
+-rw-r--r--   0        0        0     4328 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/builders/feature_profiles/transport.py
+-rw-r--r--   0        0        0     2053 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/config_device_inventory_api.py
+-rw-r--r--   0        0        0     4760 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/config_group_api.py
+-rw-r--r--   0        0        0     6672 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/configuration_groups/parcel.py
+-rw-r--r--   0        0        0     7315 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/dashboard_api.py
+-rw-r--r--   0        0        0     7360 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/device_action_api.py
+-rw-r--r--   0        0        0    53269 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/feature_profile_api.py
+-rw-r--r--   0        0        0     1919 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/logs_api.py
+-rw-r--r--   0        0        0     2449 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/monitoring_status_api.py
+-rw-r--r--   0        0        0     6036 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/mtt_aaa_api.py
+-rw-r--r--   0        0        0     4394 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/omp_api.py
+-rw-r--r--   0        0        0     5691 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/packet_capture_api.py
+-rw-r--r--   0        0        0     1654 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/parcel_api.py
+-rw-r--r--   0        0        0     5600 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/partition_manager_api.py
+-rw-r--r--   0        0        0    35876 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/policy_api.py
+-rw-r--r--   0        0        0     2284 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/resource_pool_api.py
+-rw-r--r--   0        0        0    11320 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/software_action_api.py
+-rw-r--r--   0        0        0     5473 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/speedtest_api.py
+-rw-r--r--   0        0        0     7149 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/task_status_api.py
+-rw-r--r--   0        0        0    30133 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/template_api.py
+-rw-r--r--   0        0        0     3540 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/templates/README.md
+-rw-r--r--   0        0        0      251 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/templates/bool_str.py
+-rw-r--r--   0        0        0     7481 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/templates/cli_template.py
+-rw-r--r--   0        0        0     3425 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/templates/device_template/device_template.py
+-rw-r--r--   0        0        0      571 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/templates/device_template/device_template_payload.json.j2
+-rw-r--r--   0        0        0      137 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/templates/device_variable.py
+-rw-r--r--   0        0        0     5235 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/templates/feature_template.py
+-rw-r--r--   0        0        0     6576 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/templates/feature_template_field.py
+-rw-r--r--   0        0        0      661 2024-05-20 07:57:48.055061 catalystwan-0.33.6.dev0/catalystwan/api/templates/feature_template_payload.py
+-rw-r--r--   0        0        0     3244 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_aaa_model.py
+-rw-r--r--   0        0        0      667 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_banner_model.py
+-rw-r--r--   0        0        0     2180 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_bfd_model.py
+-rw-r--r--   0        0        0    12522 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_bgp_model.py
+-rw-r--r--   0        0        0     3436 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_logging_model.py
+-rw-r--r--   0        0        0     1584 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_ntp_model.py
+-rw-r--r--   0        0        0     3835 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_omp_model.py
+-rw-r--r--   0        0        0     6749 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_ospf.py
+-rw-r--r--   0        0        0    13901 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_ospfv3.py
+-rw-r--r--   0        0        0     9589 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
+-rw-r--r--   0        0        0     2581 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_snmp_model.py
+-rw-r--r--   0        0        0     8986 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_system.py
+-rw-r--r--   0        0        0    21665 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_vpn_interface_model.py
+-rw-r--r--   0        0        0    15836 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_vpn_model.py
+-rw-r--r--   0        0        0      472 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cli_template.py
+-rw-r--r--   0        0        0     1835 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/omp_vsmart_model.py
+-rw-r--r--   0        0        0      806 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/security_vsmart_model.py
+-rw-r--r--   0        0        0     1882 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/supported.py
+-rw-r--r--   0        0        0     2624 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/models/system_vsmart_model.py
+-rw-r--r--   0        0        0     2261 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/aaa/aaa_model.py
+-rw-r--r--   0        0        0    11178 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
+-rw-r--r--   0        0        0     1041 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
+-rw-r--r--   0        0        0     4264 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
+-rw-r--r--   0        0        0     3735 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
+-rw-r--r--   0        0        0     1999 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
+-rw-r--r--   0        0        0     2558 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
+-rw-r--r--   0        0        0     4547 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
+-rw-r--r--   0        0        0     1843 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
+-rw-r--r--   0        0        0     2247 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
+-rw-r--r--   0        0        0     2098 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
+-rw-r--r--   0        0        0      683 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
+-rw-r--r--   0        0        0     7113 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/tenant/tenant.json.j2
+-rw-r--r--   0        0        0     1460 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/tenant/tenant_model.py
+-rw-r--r--   0        0        0     5013 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     4406 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/tenant_management_api.py
+-rw-r--r--   0        0        0     5090 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/tenant_migration_api.py
+-rw-r--r--   0        0        0    13729 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/api/versions_utils.py
+-rw-r--r--   0        0        0    21802 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/dataclasses.py
+-rw-r--r--   0        0        0    27207 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/__init__.py
+-rw-r--r--   0        0        0    11938 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/administration_user_and_group.py
+-rw-r--r--   0        0        0     6731 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/certificate_management_device.py
+-rw-r--r--   0        0        0     1476 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/certificate_management_vmanage.py
+-rw-r--r--   0        0        0     4035 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/client.py
+-rw-r--r--   0        0        0     2722 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/cluster_management.py
+-rw-r--r--   0        0        0      983 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/device/software_update.py
+-rw-r--r--   0        0        0     9447 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/disaster_recovery.py
+-rw-r--r--   0        0        0     3876 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/application_priority.py
+-rw-r--r--   0        0        0     2406 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/cli.py
+-rw-r--r--   0        0        0     3557 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/dns_security.py
+-rw-r--r--   0        0        0     3735 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/embedded_security.py
+-rw-r--r--   0        0        0     2600 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py
+-rw-r--r--   0        0        0     4037 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
+-rw-r--r--   0        0        0     2747 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py
+-rw-r--r--   0        0        0     3315 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/sig_security.py
+-rw-r--r--   0        0        0    10040 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
+-rw-r--r--   0        0        0     3679 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/topology.py
+-rw-r--r--   0        0        0     6471 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
+-rw-r--r--   0        0        0     1361 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/abstractions.py
+-rw-r--r--   0        0        0     1969 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     2024 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2046 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/aip.py
+-rw-r--r--   0        0        0     2046 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/amp.py
+-rw-r--r--   0        0        0     1756 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/cflowd.py
+-rw-r--r--   0        0        0     2025 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/control.py
+-rw-r--r--   0        0        0     2170 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/device_access.py
+-rw-r--r--   0        0        0     2239 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     1853 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/dns_security.py
+-rw-r--r--   0        0        0     2099 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     1995 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/intrusion_prevention.py
+-rw-r--r--   0        0        0     1954 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/mesh.py
+-rw-r--r--   0        0        0     1991 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     2065 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/rewrite.py
+-rw-r--r--   0        0        0     1967 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     2092 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/security_group.py
+-rw-r--r--   0        0        0     1879 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/ssl_decryption.py
+-rw-r--r--   0        0        0     1985 2024-05-20 07:57:48.059061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/ssl_decryption_utd_profile.py
+-rw-r--r--   0        0        0     2029 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     1869 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/url_filtering.py
+-rw-r--r--   0        0        0     2184 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0     2111 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1740 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/app.py
+-rw-r--r--   0        0        0     1900 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/app_probe.py
+-rw-r--r--   0        0        0     1793 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/as_path.py
+-rw-r--r--   0        0        0     1813 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/class_map.py
+-rw-r--r--   0        0        0     1772 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/color.py
+-rw-r--r--   0        0        0     1854 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/community.py
+-rw-r--r--   0        0        0     1971 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0     1873 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/data_prefix.py
+-rw-r--r--   0        0        0     2023 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/expanded_community.py
+-rw-r--r--   0        0        0     1752 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1893 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/geo_location.py
+-rw-r--r--   0        0        0     1930 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1873 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0     1833 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/local_app.py
+-rw-r--r--   0        0        0     1893 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/local_domain.py
+-rw-r--r--   0        0        0     1792 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/mirror.py
+-rw-r--r--   0        0        0     1817 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/policer.py
+-rw-r--r--   0        0        0     1752 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/port.py
+-rw-r--r--   0        0        0     2065 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1852 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/prefix.py
+-rw-r--r--   0        0        0     1930 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1683 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/region.py
+-rw-r--r--   0        0        0     1892 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/site.py
+-rw-r--r--   0        0        0     1782 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/sla.py
+-rw-r--r--   0        0        0     1940 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py
+-rw-r--r--   0        0        0     1752 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/tloc.py
+-rw-r--r--   0        0        0     1872 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/trunkgroup.py
+-rw-r--r--   0        0        0     1930 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/umbrella_data.py
+-rw-r--r--   0        0        0     1863 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
+-rw-r--r--   0        0        0     1863 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/url_block_list.py
+-rw-r--r--   0        0        0     1734 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/vpn.py
+-rw-r--r--   0        0        0     1752 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/zone.py
+-rw-r--r--   0        0        0     1726 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/security_template.py
+-rw-r--r--   0        0        0     1738 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/vedge_template.py
+-rw-r--r--   0        0        0     2974 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/vsmart_template.py
+-rw-r--r--   0        0        0     8865 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/software_actions.py
+-rw-r--r--   0        0        0     6820 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_dashboard_status.py
+-rw-r--r--   0        0        0    10675 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_device_actions.py
+-rw-r--r--   0        0        0    13973 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_device_inventory.py
+-rw-r--r--   0        0        0      881 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_device_template.py
+-rw-r--r--   0        0        0     5277 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_feature_profile.py
+-rw-r--r--   0        0        0     6387 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_group.py
+-rw-r--r--   0        0        0    27565 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_settings.py
+-rw-r--r--   0        0        0    14794 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/endpoints_container.py
+-rw-r--r--   0        0        0      760 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/misc.py
+-rw-r--r--   0        0        0     8272 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/monitoring/device_details.py
+-rw-r--r--   0        0        0      347 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/monitoring/server_info.py
+-rw-r--r--   0        0        0     1929 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/monitoring/status.py
+-rw-r--r--   0        0        0     1446 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/real_time_monitoring/reboot_history.py
+-rw-r--r--   0        0        0     1419 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/sdavc_cloud_connector.py
+-rw-r--r--   0        0        0     1047 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/tenant_backup_restore.py
+-rw-r--r--   0        0        0     7648 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/tenant_management.py
+-rw-r--r--   0        0        0     3649 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/tenant_migration.py
+-rw-r--r--   0        0        0     3661 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
+-rw-r--r--   0        0        0     6246 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/exceptions.py
+-rw-r--r--   0        0        0     1340 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/integration_tests/feature_profile/sdwan/base.py
+-rw-r--r--   0        0        0     5165 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_application_priority.py
+-rw-r--r--   0        0        0     2364 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_cli.py
+-rw-r--r--   0        0        0     4587 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_dns_security.py
+-rw-r--r--   0        0        0     1834 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_other.py
+-rw-r--r--   0        0        0    28479 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_service.py
+-rw-r--r--   0        0        0    14507 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_sig_security.py
+-rw-r--r--   0        0        0     9901 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_system.py
+-rw-r--r--   0        0        0    57995 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py
+-rw-r--r--   0        0        0     4124 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/integration_tests/feature_profile/sdwan/topology/test_topology.py
+-rw-r--r--   0        0        0     1078 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/integration_tests/test_config_migration.py
+-rw-r--r--   0        0        0     1902 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/integration_tests/test_find_template_values.py
+-rw-r--r--   0        0        0      676 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/logging.conf
+-rw-r--r--   0        0        0    15611 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/models/common.py
+-rw-r--r--   0        0        0      194 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/common.py
+-rw-r--r--   0        0        0    12357 2024-05-20 07:57:48.063061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/config_migration.py
+-rw-r--r--   0        0        0       89 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/docs/README.md
+-rw-r--r--   0        0        0   142336 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/docs/diagram.png
+-rw-r--r--   0        0        0    10043 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/README.md
+-rw-r--r--   0        0        0      663 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/builder.py
+-rw-r--r--   0        0        0    25595 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/common.py
+-rw-r--r--   0        0        0     5065 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/parcel.py
+-rw-r--r--   0        0        0      661 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/application_priority/__init__.py
+-rw-r--r--   0        0        0     1385 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/application_priority/policy_settings.py
+-rw-r--r--   0        0        0     1554 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/application_priority/qos_policy.py
+-rw-r--r--   0        0        0      292 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/cli/__init__.py
+-rw-r--r--   0        0        0      480 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/cli/config.py
+-rw-r--r--   0        0        0      275 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/dns_security/__init__.py
+-rw-r--r--   0        0        0     2787 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/dns_security/dns.py
+-rw-r--r--   0        0        0      507 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/__init__.py
+-rw-r--r--   0        0        0    16716 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/ngfirewall.py
+-rw-r--r--   0        0        0     4103 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/policy.py
+-rw-r--r--   0        0        0      420 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/other/__init__.py
+-rw-r--r--   0        0        0     4750 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py
+-rw-r--r--   0        0        0     3950 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py
+-rw-r--r--   0        0        0     5256 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
+-rw-r--r--   0        0        0     1426 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
+-rw-r--r--   0        0        0     1203 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
+-rw-r--r--   0        0        0      825 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py
+-rw-r--r--   0        0        0      653 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
+-rw-r--r--   0        0        0     1244 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
+-rw-r--r--   0        0        0     1034 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
+-rw-r--r--   0        0        0      807 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
+-rw-r--r--   0        0        0     1152 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
+-rw-r--r--   0        0        0     1706 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
+-rw-r--r--   0        0        0      737 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py
+-rw-r--r--   0        0        0     1332 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py
+-rw-r--r--   0        0        0     2995 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
+-rw-r--r--   0        0        0     1106 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
+-rw-r--r--   0        0        0     5272 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
+-rw-r--r--   0        0        0     1215 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
+-rw-r--r--   0        0        0     1641 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
+-rw-r--r--   0        0        0     1442 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py
+-rw-r--r--   0        0        0     1898 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py
+-rw-r--r--   0        0        0     1277 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
+-rw-r--r--   0        0        0      871 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
+-rw-r--r--   0        0        0      830 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
+-rw-r--r--   0        0        0     1288 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
+-rw-r--r--   0        0        0     1398 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py
+-rw-r--r--   0        0        0     1604 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
+-rw-r--r--   0        0        0      907 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
+-rw-r--r--   0        0        0      799 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
+-rw-r--r--   0        0        0     1408 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
+-rw-r--r--   0        0        0     3388 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py
+-rw-r--r--   0        0        0     3935 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py
+-rw-r--r--   0        0        0     1079 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
+-rw-r--r--   0        0        0     3679 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py
+-rw-r--r--   0        0        0     1461 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
+-rw-r--r--   0        0        0     2255 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py
+-rw-r--r--   0        0        0    14507 2024-05-20 07:57:48.067062 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
+-rw-r--r--   0        0        0    10235 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
+-rw-r--r--   0        0        0    14485 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
+-rw-r--r--   0        0        0     5289 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
+-rw-r--r--   0        0        0     4001 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
+-rw-r--r--   0        0        0     1349 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
+-rw-r--r--   0        0        0    12626 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
+-rw-r--r--   0        0        0     6938 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
+-rw-r--r--   0        0        0     6350 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
+-rw-r--r--   0        0        0     5349 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/multilink.py
+-rw-r--r--   0        0        0     8633 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
+-rw-r--r--   0        0        0    24934 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
+-rw-r--r--   0        0        0    10821 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
+-rw-r--r--   0        0        0     3291 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
+-rw-r--r--   0        0        0     7362 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
+-rw-r--r--   0        0        0    12770 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
+-rw-r--r--   0        0        0     9187 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
+-rw-r--r--   0        0        0     6966 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
+-rw-r--r--   0        0        0     5161 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
+-rw-r--r--   0        0        0     3705 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
+-rw-r--r--   0        0        0     5706 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
+-rw-r--r--   0        0        0      297 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/sig_security/__init__.py
+-rw-r--r--   0        0        0    16817 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/sig_security/sig_security.py
+-rw-r--r--   0        0        0     1058 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py
+-rw-r--r--   0        0        0    15484 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
+-rw-r--r--   0        0        0      977 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py
+-rw-r--r--   0        0        0    10457 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py
+-rw-r--r--   0        0        0     2623 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py
+-rw-r--r--   0        0        0     6396 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py
+-rw-r--r--   0        0        0     6355 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py
+-rw-r--r--   0        0        0     2935 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py
+-rw-r--r--   0        0        0     3932 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py
+-rw-r--r--   0        0        0     5166 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py
+-rw-r--r--   0        0        0     6653 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/security.py
+-rw-r--r--   0        0        0     6841 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py
+-rw-r--r--   0        0        0      726 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/topology/__init__.py
+-rw-r--r--   0        0        0    12828 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/topology/custom_control.py
+-rw-r--r--   0        0        0     2162 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/topology/hubspoke.py
+-rw-r--r--   0        0        0      799 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/topology/mesh.py
+-rw-r--r--   0        0        0     2255 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py
+-rw-r--r--   0        0        0    26093 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/bgp.py
+-rw-r--r--   0        0        0     2276 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
+-rw-r--r--   0        0        0     2668 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_profile.py
+-rw-r--r--   0        0        0     1579 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/gps.py
+-rw-r--r--   0        0        0     4400 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/t1e1controller.py
+-rw-r--r--   0        0        0    12662 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn.py
+-rw-r--r--   0        0        0     9090 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/cellular.py
+-rw-r--r--   0        0        0    13993 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ethernet.py
+-rw-r--r--   0        0        0     2169 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/gre.py
+-rw-r--r--   0        0        0     5137 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ipsec.py
+-rw-r--r--   0        0        0    11421 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/multilink.py
+-rw-r--r--   0        0        0    16558 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/protocol_over.py
+-rw-r--r--   0        0        0     8889 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/t1e1serial.py
+-rw-r--r--   0        0        0      157 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/profile_type.py
+-rw-r--r--   0        0        0      378 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/configuration/topology_group.py
+-rw-r--r--   0        0        0     1041 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/device_inventory.py
+-rw-r--r--   0        0        0      341 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/feature_profile_parcel.py
+-rw-r--r--   0        0        0      785 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/misc/application_protocols.py
+-rw-r--r--   0        0        0      405 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/monitoring/server_info.py
+-rw-r--r--   0        0        0    10244 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/policy/__init__.py
+-rw-r--r--   0        0        0     8738 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/policy/centralized.py
+-rw-r--r--   0        0        0     5777 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     5979 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2204 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/aip.py
+-rw-r--r--   0        0        0     2598 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/amp.py
+-rw-r--r--   0        0        0     3159 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/cflowd.py
+-rw-r--r--   0        0        0    12236 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/control.py
+-rw-r--r--   0        0        0     4134 2024-05-20 07:57:48.071061 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/device_access.py
+-rw-r--r--   0        0        0     4250 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     4585 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/dns_security.py
+-rw-r--r--   0        0        0     3251 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     2139 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/intrusion_prevention.py
+-rw-r--r--   0        0        0     1403 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/mesh.py
+-rw-r--r--   0        0        0     3520 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     1410 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/rewrite.py
+-rw-r--r--   0        0        0    12381 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     3187 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/security_group.py
+-rw-r--r--   0        0        0     7992 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/ssl_decryption.py
+-rw-r--r--   0        0        0     3539 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/ssl_decryption_utd_profile.py
+-rw-r--r--   0        0        0    14006 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     2684 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/url_filtering.py
+-rw-r--r--   0        0        0     1329 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0    10584 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1094 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/app.py
+-rw-r--r--   0        0        0     1295 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/app_probe.py
+-rw-r--r--   0        0        0      651 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/as_path.py
+-rw-r--r--   0        0        0      789 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/class_map.py
+-rw-r--r--   0        0        0      661 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/color.py
+-rw-r--r--   0        0        0     1378 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/communities.py
+-rw-r--r--   0        0        0      918 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0      860 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/data_prefix.py
+-rw-r--r--   0        0        0      495 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1055 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/geo_location.py
+-rw-r--r--   0        0        0      817 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1111 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0      990 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/local_app.py
+-rw-r--r--   0        0        0      923 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/local_domain.py
+-rw-r--r--   0        0        0      714 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/mirror.py
+-rw-r--r--   0        0        0     1127 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/policer.py
+-rw-r--r--   0        0        0      771 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/port.py
+-rw-r--r--   0        0        0     3196 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1055 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/prefix.py
+-rw-r--r--   0        0        0      723 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1325 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/region.py
+-rw-r--r--   0        0        0      942 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/site.py
+-rw-r--r--   0        0        0     6864 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/sla.py
+-rw-r--r--   0        0        0      970 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/threat_grid_api_key.py
+-rw-r--r--   0        0        0      960 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/tloc.py
+-rw-r--r--   0        0        0     2111 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/trunkgroup.py
+-rw-r--r--   0        0        0      824 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/umbrella_data.py
+-rw-r--r--   0        0        0      856 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/url.py
+-rw-r--r--   0        0        0     1071 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/vpn.py
+-rw-r--r--   0        0        0     1405 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/list/zone.py
+-rw-r--r--   0        0        0     6204 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/localized.py
+-rw-r--r--   0        0        0     3752 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/policy.py
+-rw-r--r--   0        0        0    33009 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/policy_definition.py
+-rw-r--r--   0        0        0     1557 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/policy_list.py
+-rw-r--r--   0        0        0     9385 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/policy/security.py
+-rw-r--r--   0        0        0     2437 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/templates.py
+-rw-r--r--   0        0        0     5239 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/models/tenant.py
+-rw-r--r--   0        0        0     9586 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/response.py
+-rw-r--r--   0        0        0    19513 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/session.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/config_migration/__init__.py
+-rw-r--r--   0        0        0     1236 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/config_migration/test_converter_chooser.py
+-rw-r--r--   0        0        0      467 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/config_migration/test_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/config_migration/test_data/feature_templates/__init__.py
+-rw-r--r--   0        0        0    10804 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/config_migration/test_data/feature_templates/interface.py
+-rw-r--r--   0        0        0      519 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/config_migration/test_data/feature_templates/malformed.py
+-rw-r--r--   0        0        0     3185 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/config_migration/test_data/feature_templates/vpn.py
+-rw-r--r--   0        0        0     3583 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/config_migration/test_device_template_with_info.py
+-rw-r--r--   0        0        0     6139 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/config_migration/test_merge_parcels.py
+-rw-r--r--   0        0        0     4288 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/config_migration/test_normalizer.py
+-rw-r--r--   0        0        0    10094 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/config_migration/test_transform.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/models/__init__.py
+-rw-r--r--   0        0        0      401 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
+-rw-r--r--   0        0        0      513 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/banner_1.json
+-rw-r--r--   0        0        0      116 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/basic/alias.json
+-rw-r--r--   0        0        0      114 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/basic/basic.json
+-rw-r--r--   0        0        0      109 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/basic/basic_no_value.json
+-rw-r--r--   0        0        0      848 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/basic/children.json
+-rw-r--r--   0        0        0     2348 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/basic/children_nested.json
+-rw-r--r--   0        0        0     2348 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      274 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/basic/data_path.json
+-rw-r--r--   0        0        0     2973 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/cisco_bfd.json
+-rw-r--r--   0        0        0    11100 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/complex_aaa.json
+-rw-r--r--   0        0        0    41165 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
+-rw-r--r--   0        0        0     5219 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/default_cisco_system.json
+-rw-r--r--   0        0        0     5505 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/iuo.json
+-rw-r--r--   0        0        0      249 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/omp_1.json
+-rw-r--r--   0        0        0      875 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/omp_2.json
+-rw-r--r--   0        0        0     1682 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/omp_3.json
+-rw-r--r--   0        0        0      662 2024-05-20 07:57:48.075062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/models/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/models/cisco_aaa.py
+-rw-r--r--   0        0        0      303 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/models/cisco_banner.py
+-rw-r--r--   0        0        0      587 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/models/cisco_bfd.py
+-rw-r--r--   0        0        0      344 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/models/cisco_system.py
+-rw-r--r--   0        0        0     8078 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/models/cisco_vpn.py
+-rw-r--r--   0        0        0     1091 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/models/omp_vsmart.py
+-rw-r--r--   0        0        0      605 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/basic/alias.json
+-rw-r--r--   0        0        0      574 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/basic/basic.json
+-rw-r--r--   0        0        0     1810 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/basic/children.json
+-rw-r--r--   0        0        0     4005 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/basic/children_nested.json
+-rw-r--r--   0        0        0     4005 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      731 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/basic/data_path.json
+-rw-r--r--   0        0        0    43436 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/cedge_aaa.json
+-rw-r--r--   0        0        0     1200 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/cisco_banner.json
+-rw-r--r--   0        0        0     9495 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/cisco_bfd.json
+-rw-r--r--   0        0        0    99045 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/cisco_system.json
+-rw-r--r--   0        0        0    87854 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/cisco_vpn.json
+-rw-r--r--   0        0        0     5939 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/omp-vsmart.json
+-rw-r--r--   0        0        0     1381 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/test_chose_model.py
+-rw-r--r--   0        0        0     2598 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/test_deserialize_model.py
+-rw-r--r--   0        0        0     4598 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/test_generate_payload.py
+-rw-r--r--   0        0        0     1755 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/templates/test_serialize_model.py
+-rw-r--r--   0        0        0     8145 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_admin_tech_api.py
+-rw-r--r--   0        0        0    17792 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_administration.py
+-rw-r--r--   0        0        0    11116 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_alarms_api.py
+-rw-r--r--   0        0        0     8322 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_cli_template.py
+-rw-r--r--   0        0        0     5494 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_creation_tools.py
+-rw-r--r--   0        0        0     3981 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_device_action_api.py
+-rw-r--r--   0        0        0    28159 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_devices_api.py
+-rw-r--r--   0        0        0    34864 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_endpoints.py
+-rw-r--r--   0        0        0    10585 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_feature_profile_api.py
+-rw-r--r--   0        0        0      894 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_feature_template_field.py
+-rw-r--r--   0        0        0     1545 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_logs_api.py
+-rw-r--r--   0        0        0     1899 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_models_common.py
+-rw-r--r--   0        0        0     1809 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_monitoring_server_info.py
+-rw-r--r--   0        0        0     5489 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_monitoring_status_api.py
+-rw-r--r--   0        0        0    11026 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_mtt_aaa_api.py
+-rw-r--r--   0        0        0     9562 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_normalize_to_model_definition.py
+-rw-r--r--   0        0        0    16472 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_omp_api.py
+-rw-r--r--   0        0        0     5223 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_packet_capture.py
+-rw-r--r--   0        0        0     5727 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_partition_manager_api.py
+-rw-r--r--   0        0        0     7483 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_response.py
+-rw-r--r--   0        0        0     6724 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_session.py
+-rw-r--r--   0        0        0     7117 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_software_action_api.py
+-rw-r--r--   0        0        0     6071 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_speed_test_api.py
+-rw-r--r--   0        0        0    14926 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_task_status_api.py
+-rw-r--r--   0        0        0    15055 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_templates.py
+-rw-r--r--   0        0        0     3705 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     6114 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_tenant_management_api.py
+-rw-r--r--   0        0        0     4506 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_tenant_migration_api.py
+-rw-r--r--   0        0        0    12377 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_typed_list.py
+-rw-r--r--   0        0        0     2968 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_version.py
+-rw-r--r--   0        0        0    10377 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_version_utils.py
+-rw-r--r--   0        0        0     3343 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/tests/test_vmanage_auth.py
+-rw-r--r--   0        0        0     9379 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/typed_list.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/utils/__init__.py
+-rw-r--r--   0        0        0      266 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/utils/alarm_status.py
+-rw-r--r--   0        0        0      253 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/utils/certificate_status.py
+-rw-r--r--   0        0        0      279 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/utils/colors.py
+-rw-r--r--   0        0        0      239 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/exceptions.py
+-rw-r--r--   0        0        0      328 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/__init__.py
+-rw-r--r--   0        0        0     3433 2024-05-20 07:57:48.079062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/aaa.py
+-rw-r--r--   0        0        0     5810 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/appqoe.py
+-rw-r--r--   0        0        0      784 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/banner.py
+-rw-r--r--   0        0        0      268 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/base.py
+-rw-r--r--   0        0        0     2991 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/basic.py
+-rw-r--r--   0        0        0      898 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/bfd.py
+-rw-r--r--   0        0        0     4357 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/bgp.py
+-rw-r--r--   0        0        0     1520 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/cellular_controller.py
+-rw-r--r--   0        0        0     3269 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/cellular_profile.py
+-rw-r--r--   0        0        0      756 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/cli.py
+-rw-r--r--   0        0        0     1932 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/cloud_credentials.py
+-rw-r--r--   0        0        0     4387 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/dhcp.py
+-rw-r--r--   0        0        0     5349 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/eigrp.py
+-rw-r--r--   0        0        0      578 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/global_.py
+-rw-r--r--   0        0        0     1573 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/gps.py
+-rw-r--r--   0        0        0      331 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/helpers.py
+-rw-r--r--   0        0        0    12692 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/lan/ethernet.py
+-rw-r--r--   0        0        0     5619 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/lan/gre.py
+-rw-r--r--   0        0        0     5331 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/lan/ipsec.py
+-rw-r--r--   0        0        0     9349 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/lan/multilink.py
+-rw-r--r--   0        0        0     7411 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/lan/svi.py
+-rw-r--r--   0        0        0     1963 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/logging_.py
+-rw-r--r--   0        0        0     4720 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/model_definition_normalizer.py
+-rw-r--r--   0        0        0    13085 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/multicast.py
+-rw-r--r--   0        0        0     5149 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/normalizer.py
+-rw-r--r--   0        0        0     2295 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/ntp.py
+-rw-r--r--   0        0        0     1475 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/omp.py
+-rw-r--r--   0        0        0     5520 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/ospf.py
+-rw-r--r--   0        0        0    11012 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py
+-rw-r--r--   0        0        0     6289 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py
+-rw-r--r--   0        0        0     1568 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/security.py
+-rw-r--r--   0        0        0     9336 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/sig.py
+-rw-r--r--   0        0        0     2240 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/snmp.py
+-rw-r--r--   0        0        0     9032 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/switchport.py
+-rw-r--r--   0        0        0     2776 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py
+-rw-r--r--   0        0        0     2250 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/ucse.py
+-rw-r--r--   0        0        0    32939 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/vpn.py
+-rw-r--r--   0        0        0     5742 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/cellular.py
+-rw-r--r--   0        0        0    13285 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/ethernet.py
+-rw-r--r--   0        0        0     4844 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/gre.py
+-rw-r--r--   0        0        0     6866 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/ipsec.py
+-rw-r--r--   0        0        0    14360 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/multilink.py
+-rw-r--r--   0        0        0    18190 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/protocol_over.py
+-rw-r--r--   0        0        0     5344 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/wan/t1e1serial.py
+-rw-r--r--   0        0        0     8057 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py
+-rw-r--r--   0        0        0     2540 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/policy/policy_definitions.py
+-rw-r--r--   0        0        0     9564 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/converters/policy/policy_lists.py
+-rw-r--r--   0        0        0     6038 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/creators/config_pusher.py
+-rw-r--r--   0        0        0     5570 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/creators/strategy/parcels.py
+-rw-r--r--   0        0        0     1686 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/factories/feature_profile_api.py
+-rw-r--r--   0        0        0     1257 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/factories/parcel_pusher.py
+-rw-r--r--   0        0        0     1671 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/reverters/config_reverter.py
+-rw-r--r--   0        0        0        0 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/steps/__init__.py
+-rw-r--r--   0        0        0     2914 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/steps/constants.py
+-rw-r--r--   0        0        0     5853 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_migration/steps/transform.py
+-rw-r--r--   0        0        0      154 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/config_status.py
+-rw-r--r--   0        0        0     4778 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/creation_tools.py
+-rw-r--r--   0        0        0     7281 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/dashboard.py
+-rw-r--r--   0        0        0     2863 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/device_model.py
+-rw-r--r--   0        0        0     2110 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/dict.py
+-rw-r--r--   0        0        0      953 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/feature_template/choose_model.py
+-rw-r--r--   0        0        0     5144 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/feature_template/find_template_values.py
+-rw-r--r--   0        0        0      584 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/operation_status.py
+-rw-r--r--   0        0        0      196 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/personality.py
+-rw-r--r--   0        0        0      360 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/pydantic_field.py
+-rw-r--r--   0        0        0      172 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/reachability.py
+-rw-r--r--   0        0        0      407 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/session_type.py
+-rw-r--r--   0        0        0      149 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/template_type.py
+-rw-r--r--   0        0        0     9825 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/timezone.py
+-rw-r--r--   0        0        0     3930 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/upgrades_helper.py
+-rw-r--r--   0        0        0      159 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/utils/validate_status.py
+-rw-r--r--   0        0        0     3032 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/version.py
+-rw-r--r--   0        0        0     5415 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/vmanage_auth.py
+-rw-r--r--   0        0        0    15724 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/workflows/config_migration.py
+-rw-r--r--   0        0        0     9946 2024-05-20 07:57:48.083062 catalystwan-0.33.6.dev0/catalystwan/workflows/tenant_migration.py
+-rw-r--r--   0        0        0      866 2024-05-20 07:57:48.087062 catalystwan-0.33.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0    18637 1970-01-01 00:00:00.000000 catalystwan-0.33.6.dev0/setup.py
+-rw-r--r--   0        0        0    14665 1970-01-01 00:00:00.000000 catalystwan-0.33.6.dev0/PKG-INFO
```

### Comparing `catalystwan-0.33.6/LICENSE` & `catalystwan-0.33.6.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/README.md` & `catalystwan-0.33.6.dev0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -178,30 +178,28 @@
 n = 24
 alarms_from_n_hours = session.api.alarms.get(from_time=n)
 ```
 
 To get all critical alarms from past `n` hours:
 
 ```python
-from catalystwan.utils.alarm_status import Severity
 n = 48
 critical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)
 ```
 
 </details>
 
 <details>
     <summary> <b>Users</b> <i>(click to expand)</i></summary>
 
 ```python
 # Get all users
 session.api.users.get()
 
 # Create user
-from catalystwan.endpoints.administration_user_and_group import User
 new_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")
 session.api.users.create(new_user)
 
 # Update user data
 new_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")
 session.api.users.update(new_user_update)
```

#### html2text {}

```diff
@@ -72,20 +72,18 @@
 session.api.repository.upload_image(image) # Install software install_task =
 session.api.software.install(devices=vsmarts, image=image) # Check action
 status install_task.wait_for_completed() ``` GGeett aallaarrmmss (click to expand) To
 get all alarms: ```python alarms = session.api.alarms.get() ``` To get all not
 viewed alarms: ```python not_viewed_alarms = session.api.alarms.get().filter
 (viewed=False) ``` To get all alarms from past `n` hours: ```python n = 24
 alarms_from_n_hours = session.api.alarms.get(from_time=n) ``` To get all
-critical alarms from past `n` hours: ```python from
-catalystwan.utils.alarm_status import Severity n = 48 critical_alarms =
+critical alarms from past `n` hours: ```python n = 48 critical_alarms =
 session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL) ```
 UUsseerrss (click to expand) ```python # Get all users session.api.users.get() #
-Create user from catalystwan.endpoints.administration_user_and_group import
-User new_user = User(username="new_user", password="new_user", group=
+Create user new_user = User(username="new_user", password="new_user", group=
 ["netadmin"], description="new user") session.api.users.create(new_user) #
 Update user data new_user_update = UserUpdateRequest(username="new_user",
 group=["netadmin", "netops"], locale="en_US", description="updated-new_user-
 description") session.api.users.update(new_user_update) # Update user password
 session.api.users.update_password("new_user", "n3W-P4s$w0rd") # Reset user
 session.api.users.reset("new_user") # Delete user session.api.users.delete
 ("new_user") # Get current user authentication type and role
```

### Comparing `catalystwan-0.33.6/catalystwan/__init__.py` & `catalystwan-0.33.6.dev0/catalystwan/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from os import environ
 from pathlib import Path
 from traceback import FrameSummary, StackSummary, extract_stack
 from typing import Callable, Final, List, Optional
 
 import urllib3
 
-USER_AGENT = f"{__package__}/{metadata.version(__package__)}"
+PACKAGE_VERSION = metadata.version(__package__)
+USER_AGENT = f"{__package__}/{PACKAGE_VERSION}"
 
 
 def with_proc_info_header(method: Callable[..., str]) -> Callable[..., str]:
     """
     Adds process ID and external caller information before first line of returned string
     """
```

### Comparing `catalystwan-0.33.6/catalystwan/abstractions.py` & `catalystwan-0.33.6.dev0/catalystwan/abstractions.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,9 +50,9 @@
         ...
 
     @property
     def session_type(self) -> Optional[SessionType]:
         ...
 
     @property
-    def validate_responses(self) -> bool:
+    def validate_response(self) -> bool:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/api/admin_tech_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/administration.py` & `catalystwan-0.33.6.dev0/catalystwan/api/administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/alarms_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/api_container.py` & `catalystwan-0.33.6.dev0/catalystwan/api/api_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,32 +11,32 @@
     ResourceGroupsAPI,
     SessionsAPI,
     UserGroupsAPI,
     UsersAPI,
 )
 from catalystwan.api.alarms_api import AlarmsAPI
 from catalystwan.api.basic_api import DevicesAPI, DeviceStateAPI
+from catalystwan.api.builders import BuilderAPI
 from catalystwan.api.config_device_inventory_api import ConfigurationDeviceInventoryAPI
 from catalystwan.api.config_group_api import ConfigGroupAPI
 from catalystwan.api.dashboard_api import DashboardAPI
-from catalystwan.api.feature_profile_api import SDRoutingFeatureProfilesAPI
+from catalystwan.api.feature_profile_api import SDRoutingFeatureProfilesAPI, SDWANFeatureProfilesAPI
 from catalystwan.api.logs_api import LogsAPI
 from catalystwan.api.omp_api import OmpAPI
 from catalystwan.api.packet_capture_api import PacketCaptureAPI
 from catalystwan.api.partition_manager_api import PartitionManagerAPI
 from catalystwan.api.policy_api import PolicyAPI
 from catalystwan.api.resource_pool_api import ResourcePoolAPI
 from catalystwan.api.software_action_api import SoftwareActionAPI
 from catalystwan.api.speedtest_api import SpeedtestAPI
 from catalystwan.api.template_api import TemplatesAPI
 from catalystwan.api.tenant_backup_restore_api import TenantBackupRestoreAPI
 from catalystwan.api.tenant_management_api import TenantManagementAPI
 from catalystwan.api.tenant_migration_api import TenantMigrationAPI
 from catalystwan.api.versions_utils import RepositoryAPI
-from catalystwan.api.virtual_image_action_api import LxcActionAPI
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
 
 class APIContainer:
     def __init__(self, session: ManagerSession):
@@ -55,16 +55,17 @@
         self.speedtest = SpeedtestAPI(session)
         self.templates = TemplatesAPI(session)
         self.tenant_backup = TenantBackupRestoreAPI(session)
         self.tenant_migration = TenantMigrationAPI(session)
         self.repository = RepositoryAPI(session)
         self.resource_pool = ResourcePoolAPI(session)
         self.software = SoftwareActionAPI(session)
-        self.lxcsoftware = LxcActionAPI(session)
         self.partition = PartitionManagerAPI(session)
         self.users = UsersAPI(session)
         self.cluster_management = ClusterManagementAPI(session)
         self.user_groups = UserGroupsAPI(session)
         self.resource_groups = ResourceGroupsAPI(session)
         self.sessions = SessionsAPI(session)
         self.policy = PolicyAPI(session)
         self.sd_routing_feature_profiles = SDRoutingFeatureProfilesAPI(session)
+        self.sdwan_feature_profiles = SDWANFeatureProfilesAPI(session)
+        self.builders = BuilderAPI(session)
```

### Comparing `catalystwan-0.33.6/catalystwan/api/basic_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/basic_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/config_device_inventory_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/config_device_inventory_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/config_group_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/config_group_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,125 +1,139 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Optional, overload
+from uuid import UUID
+
+from catalystwan.typed_list import DataSequence
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
 from catalystwan.endpoints.configuration_group import (
+    ConfigGroup,
     ConfigGroupAssociatePayload,
     ConfigGroupCreationPayload,
     ConfigGroupCreationResponse,
     ConfigGroupDeployPayload,
     ConfigGroupDeployResponse,
     ConfigGroupDisassociateResponse,
     ConfigGroupEditPayload,
     ConfigGroupEditResponse,
-    ConfigGroupResponsePayload,
     ConfigGroupVariablesCreatePayload,
     ConfigGroupVariablesCreateResponse,
     ConfigGroupVariablesEditPayload,
     ConfigurationGroup,
     DeviceId,
     ProfileId,
     Solution,
 )
 
 
 class ConfigGroupAPI:
     def __init__(self, session: ManagerSession):
-        self.session = session
-        self.endpoint = ConfigurationGroup(session)
+        self._session = session
+        self._endpoints = ConfigurationGroup(session)
 
     def associate(self, cg_id: str, device_ids: list) -> None:
         """
         Associates given config-group to specified list of devices
         """
         devices = []
 
         for device_id in device_ids:
             devices.append(DeviceId(id=device_id))
 
         payload = ConfigGroupAssociatePayload(devices=devices)
 
-        self.endpoint.associate(config_group_id=cg_id, payload=payload)
+        self._endpoints.associate(config_group_id=cg_id, payload=payload)
 
     def create(self, name: str, description: str, solution: Solution, profile_ids: list) -> ConfigGroupCreationResponse:
         """
         Creates new config-group
         """
         profiles = []
 
         for profile_id in profile_ids:
             profiles.append(ProfileId(id=profile_id))
         cg_payload = ConfigGroupCreationPayload(
             name=name, description=description, solution=solution, profiles=profiles
         )
 
-        return self.endpoint.create_config_group(cg_payload)
+        return self._endpoints.create_config_group(cg_payload)
 
     def create_variables(
         self, cg_id: str, device_ids: list, suggestions: bool = True
     ) -> ConfigGroupVariablesCreateResponse:
         """
         Creates device specific variable data in given config-group
         """
         payload = ConfigGroupVariablesCreatePayload(deviceIds=device_ids, suggestions=suggestions)
-        return self.endpoint.create_variables(config_group_id=cg_id, payload=payload)
+        return self._endpoints.create_variables(config_group_id=cg_id, payload=payload)
 
-    def delete(self, cg_id: str) -> None:
+    def delete(self, cg_id: UUID) -> None:
         """
         Deletes existing config-group with given ID
         """
-        self.endpoint.delete_config_group(cg_id)
+        self._endpoints.delete_config_group(cg_id)
 
     def deploy(self, cg_id: str, device_ids: list) -> ConfigGroupDeployResponse:
         """
         Deploys specified config-group config to given list of devices
         """
         devices = []
         for device_id in device_ids:
             devices.append(DeviceId(id=device_id))
 
         payload = ConfigGroupDeployPayload(devices=devices)
-        return self.endpoint.deploy(config_group_id=cg_id, payload=payload)
+        return self._endpoints.deploy(config_group_id=cg_id, payload=payload)
 
     def disassociate(self, cg_id: str, device_ids: list) -> ConfigGroupDisassociateResponse:
         """
         Disassociates given list of devices from the specified config-group
         """
         devices = []
         for device_id in device_ids:
             devices.append(DeviceId(id=device_id))
 
         payload = ConfigGroupAssociatePayload(devices=devices)
-        return self.endpoint.disassociate(config_group_id=cg_id, payload=payload)
+        return self._endpoints.disassociate(config_group_id=cg_id, payload=payload)
 
     def edit(
         self, cg_id: str, name: str, description: str, solution: Solution, profile_ids: list
     ) -> ConfigGroupEditResponse:
         """
         Modifies feature profiles in existing config-group
         """
         profiles = []
 
         for profile_id in profile_ids:
             profiles.append(ProfileId(id=profile_id))
         payload = ConfigGroupEditPayload(name=name, description=description, solution=solution, profiles=profiles)
 
-        return self.endpoint.edit_config_group(config_group_id=cg_id, payload=payload)
+        return self._endpoints.edit_config_group(config_group_id=cg_id, payload=payload)
+
+    @overload
+    def get(self) -> DataSequence[ConfigGroup]:
+        ...
+
+    @overload
+    def get(self, group_id: UUID) -> ConfigGroup:
+        ...
 
-    def get(self) -> ConfigGroupResponsePayload:
+    def get(self, group_id: Optional[UUID] = None) -> Any:
         """
-        Gets list of existing config-groups
+        Gets list of existing config-groups or single config-group with given ID
+        If given ID is not correct return None
         """
-        return self.endpoint.get()
+        if group_id is None:
+            return self._endpoints.get()
+        return self._endpoints.get().filter(id=group_id).single_or_default()
 
     def update_variables(self, cg_id: str, solution: Solution, device_variables: list) -> None:
         """
         Updates device specific variable data in given config-group
         """
         payload = ConfigGroupVariablesEditPayload(solution=solution, devices=device_variables)
 
-        self.endpoint.update_variables(config_group_id=cg_id, payload=payload)
+        self._endpoints.update_variables(config_group_id=cg_id, payload=payload)
```

### Comparing `catalystwan-0.33.6/catalystwan/api/configuration_groups/parcel.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,139 +1,112 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from enum import Enum
-from typing import Any, Dict, Generic, Literal, Optional, TypeVar, get_origin
+from typing import List, Literal, Optional, Union
 
-from pydantic import AliasPath, BaseModel, ConfigDict, Field, PrivateAttr, model_serializer
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-T = TypeVar("T")
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default
+from catalystwan.models.common import Duplex, Speed
 
 
-class _ParcelBase(BaseModel):
-    model_config = ConfigDict(extra="forbid", arbitrary_types_allowed=True, populate_by_name=True)
-    parcel_name: str = Field(
-        min_length=1,
-        max_length=128,
-        pattern=r'^[^&<>! "]+$',
-        serialization_alias="name",
-        validation_alias="name",
-    )
-    parcel_description: Optional[str] = Field(
-        default=None,
-        serialization_alias="description",
-        validation_alias="description",
-        description="Set the parcel description",
-    )
-    data: Optional[Any] = None
-    _parcel_data_key: str = PrivateAttr(default="data")
-
-    @model_serializer(mode="wrap")
-    def envelope_parcel_data(self, handler) -> Dict[str, Any]:
-        model_dict = handler(self)
-        model_dict[self._parcel_data_key] = {}
-        remove_keys = []
-
-        for key in model_dict.keys():
-            field_info = self.model_fields.get(key)
-            if field_info and isinstance(field_info.validation_alias, AliasPath):
-                aliases = field_info.validation_alias.convert_to_aliases()
-                if aliases and aliases[0] == self._parcel_data_key and len(aliases) == 2:
-                    model_dict[self._parcel_data_key][aliases[1]] = model_dict[key]
-                    remove_keys.append(key)
-        for key in remove_keys:
-            del model_dict[key]
-        return model_dict
-
+class StaticMacAddress(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-class OptionType(str, Enum):
-    GLOBAL = "global"
-    DEFAULT = "default"
-    VARIABLE = "variable"
-
-
-class ParcelAttribute(BaseModel):
-    model_config = ConfigDict(extra="forbid")
-    option_type: OptionType = Field(serialization_alias="optionType", validation_alias="optionType")
-
-
-# https://github.com/pydantic/pydantic/discussions/6090
-# Usage: Global[str](value="test")
-class Global(ParcelAttribute, Generic[T]):
-    option_type: OptionType = Field(
-        default=OptionType.GLOBAL, serialization_alias="optionType", validation_alias="optionType"
+    mac_address: Union[Global[str], Variable] = Field(serialization_alias="macaddr", validation_alias="macaddr")
+    vlan: Union[Global[int], Variable]
+    interface_name: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="ifName", validation_alias="ifName", default=None
     )
-    value: T
-
-    def __len__(self) -> int:
-        if isinstance(self.value, (str, list)):
-            return len(self.value)
-        return -1
 
-    def __ge__(self, other: Any) -> bool:
-        if isinstance(self.value, int):
-            return self.value >= other
-        return False
 
-    def __le__(self, other: Any) -> bool:
-        if isinstance(self.value, int):
-            return self.value <= other
-        return False
-
-
-class Variable(ParcelAttribute):
-    option_type: OptionType = Field(
-        default=OptionType.VARIABLE, serialization_alias="optionType", validation_alias="optionType"
+SwitchportMode = Literal[
+    "access",
+    "trunk",
+]
+
+
+PortControl = Literal[
+    "auto",
+    "force-unauthorized",
+    "force-authorized",
+]
+
+HostMode = Literal[
+    "single-host",
+    "multi-auth",
+    "multi-host",
+    "multi-domain",
+]
+
+ControlDirection = Literal[
+    "both",
+    "in",
+]
+
+
+class SwitchportInterface(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    interface_name: Union[Global[str], Variable] = Field(serialization_alias="ifName", validation_alias="ifName")
+    mode: Global[SwitchportMode] = as_default("access", SwitchportMode)
+    shutdown: Union[Global[bool], Variable, Default[bool]] = Default[bool](value=True)
+    speed: Union[Global[Speed], Variable, Default[None]] = Default[None](value=None)
+    duplex: Union[Global[Duplex], Variable, Default[None]] = Default[None](value=None)
+    switchport_access_vlan: Union[Global[int], Variable, Default[None]] = Field(
+        serialization_alias="switchportAccessVlan",
+        validation_alias="switchportAccessVlan",
+        default=Default[None](value=None),
     )
-    value: str = Field(pattern=r"^\{\{[.\/\[\]a-zA-Z0-9_-]+\}\}$", min_length=1, max_length=64)
-
-
-class Default(ParcelAttribute, Generic[T]):
-    option_type: OptionType = Field(
-        default=OptionType.DEFAULT, serialization_alias="optionType", validation_alias="optionType"
+    switchport_trunk_allowed_vlans: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="switchportTrunkAllowedVlans", validation_alias="switchportTrunkAllowedVlans", default=None
+    )
+    switchport_trunk_native_vlan: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="switchportTrunkNativeVlan", validation_alias="switchportTrunkNativeVlan", default=None
+    )
+    port_control: Optional[Union[Global[PortControl], Variable, Default[None]]] = Field(
+        serialization_alias="portControl", validation_alias="portControl", default=None
+    )
+    voice_vlan: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="voiceVlan", validation_alias="voiceVlan", default=None
+    )
+    pae_enable: Optional[Union[Global[bool], Variable, Default[None]]] = Field(
+        serialization_alias="paeEnable", validation_alias="paeEnable", default=None
+    )
+    mac_authentication_bypass: Optional[Union[Global[bool], Variable, Default[None]]] = Field(
+        serialization_alias="macAuthenticationBypass", validation_alias="macAuthenticationBypass", default=None
+    )
+    host_mode: Optional[Union[Global[HostMode], Variable, Default[None]]] = Field(
+        serialization_alias="hostMode", validation_alias="hostMode", default=None
+    )
+    enable_periodic_reauth: Optional[Union[Global[bool], Variable, Default[None]]] = Field(
+        serialization_alias="enablePeriodicReauth", validation_alias="enablePeriodicReauth", default=None
+    )
+    inactivity: Union[Global[int], Variable, Default[None]] = Default[None](value=None)
+    reauthentication: Union[Global[int], Variable, Default[int]] = as_default(3600)
+    control_direction: Optional[Union[Global[ControlDirection], Variable, Default[None]]] = Field(
+        serialization_alias="controlDirection", validation_alias="controlDirection", default=None
+    )
+    restricted_vlan: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="restrictedVlan", validation_alias="restrictedVlan", default=None
+    )
+    guest_vlan: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="guestVlan", validation_alias="guestVlan", default=None
+    )
+    critical_vlan: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="criticalVlan", validation_alias="criticalVlan", default=None
+    )
+    enable_voice: Optional[Union[Global[bool], Variable, Default[None]]] = Field(
+        serialization_alias="enableVoice", validation_alias="enableVoice", default=None
     )
-    value: Any
-
-
-def as_global(value: Any, generic_alias: Any = None):
-    """Produces Global object given only value (type is induced from value)
-
-    Args:
-        value (Any): value of Global object to be produced
-        generic_alias (Any, optional): specify alias type like Literal. Defaults to None.
-
-    Returns:
-        Global[Any]: global option type object
-    """
-    if generic_alias is None:
-        return Global[type(value)](value=value)  # type: ignore
-    elif get_origin(generic_alias) is Literal:
-        return Global[generic_alias](value=value)  # type: ignore
-    TypeError("Inappropriate type for argument generic_alias")
-
-
-def as_variable(value: str):
-    """Produces Variable object from variable name string
-
-    Args:
-        value (str): value of Variable object to be produced
-
-    Returns:
-        Variable: variable option type object
-    """
-    return Variable(value=value)
-
-
-def as_default(value: Any, generic_alias: Any = None):
-    """Produces Default object given only value (type is induced from value)
 
-    Args:
-        value (Any): value of Default object to be produced
-        generic_alias (Any, optional): specify alias type like Literal. Defaults to None.
 
-    Returns:
-        Default[Any]: default option type object
-    """
-    if generic_alias is None:
-        return Default[type(value)](value=value)  # type: ignore
-    elif get_origin(generic_alias) is Literal:
-        return Default[generic_alias](value=value)  # type: ignore
-    TypeError("Inappropriate type for argument generic_alias")
+class SwitchportParcel(_ParcelBase):
+    type_: Literal["switchport"] = Field(default="switchport", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    interface: List[SwitchportInterface] = Field(default_factory=list, validation_alias=AliasPath("data", "interface"))
+    age_time: Union[Global[int], Variable, Default[int]] = Field(
+        default=Default[int](value=300), validation_alias=AliasPath("data", "ageTime")
+    )
+    static_mac_address: List[StaticMacAddress] = Field(
+        default_factory=list, validation_alias=AliasPath("data", "staticMacAddress")
+    )
```

### Comparing `catalystwan-0.33.6/catalystwan/api/dashboard_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/dashboard_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/device_action_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/logs_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/monitoring_status_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/mtt_aaa_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/omp_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/packet_capture_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/packet_capture_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/parcel_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/parcel_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/partition_manager_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/policy_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/policy_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,117 +1,71 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Type, overload
+from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Tuple, Type, overload
 from uuid import UUID
 
 from catalystwan.api.task_status_api import Task
-from catalystwan.endpoints.configuration.policy.definition.access_control_list import (
-    AclPolicyGetResponse,
-    ConfigurationPolicyAclDefinition,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints, PolicyListEndpoints
+from catalystwan.endpoints.configuration.policy.definition.access_control_list import ConfigurationPolicyAclDefinition
 from catalystwan.endpoints.configuration.policy.definition.access_control_list_ipv6 import (
-    AclIPv6PolicyGetResponse,
     ConfigurationPolicyAclIPv6Definition,
 )
-from catalystwan.endpoints.configuration.policy.definition.control import (
-    ConfigurationPolicyControlDefinition,
-    ControlPolicyGetResponse,
-)
+from catalystwan.endpoints.configuration.policy.definition.aip import ConfigurationPolicyAIPDefinition
+from catalystwan.endpoints.configuration.policy.definition.amp import ConfigurationPolicyAMPDefinition
+from catalystwan.endpoints.configuration.policy.definition.cflowd import ConfigurationPolicyCflowdDefinition
+from catalystwan.endpoints.configuration.policy.definition.control import ConfigurationPolicyControlDefinition
 from catalystwan.endpoints.configuration.policy.definition.device_access import (
     ConfigurationPolicyDeviceAccessDefinition,
-    DeviceAccessPolicyGetResponse,
 )
 from catalystwan.endpoints.configuration.policy.definition.device_access_ipv6 import (
     ConfigurationPolicyDeviceAccessIPv6Definition,
-    DeviceAccessIPv6PolicyGetResponse,
-)
-from catalystwan.endpoints.configuration.policy.definition.hub_and_spoke import (
-    ConfigurationPolicyHubAndSpokeDefinition,
-    HubAndSpokePolicyGetResponse,
-)
-from catalystwan.endpoints.configuration.policy.definition.mesh import (
-    ConfigurationPolicyMeshDefinition,
-    MeshPolicyGetResponse,
-)
-from catalystwan.endpoints.configuration.policy.definition.qos_map import (
-    ConfigurationPolicyQoSMapDefinition,
-    QoSMapPolicyGetResponse,
-)
-from catalystwan.endpoints.configuration.policy.definition.rewrite import (
-    ConfigurationPolicyRewriteRuleDefinition,
-    RewritePolicyGetResponse,
-)
-from catalystwan.endpoints.configuration.policy.definition.rule_set import (
-    ConfigurationPolicyRuleSetDefinition,
-    RuleSetGetResponse,
 )
+from catalystwan.endpoints.configuration.policy.definition.dns_security import ConfigurationPolicyDnsSecurityDefinition
+from catalystwan.endpoints.configuration.policy.definition.hub_and_spoke import ConfigurationPolicyHubAndSpokeDefinition
+from catalystwan.endpoints.configuration.policy.definition.intrusion_prevention import (
+    ConfigurationPolicyIntrusionPreventionDefinition,
+)
+from catalystwan.endpoints.configuration.policy.definition.mesh import ConfigurationPolicyMeshDefinition
+from catalystwan.endpoints.configuration.policy.definition.qos_map import ConfigurationPolicyQoSMapDefinition
+from catalystwan.endpoints.configuration.policy.definition.rewrite import ConfigurationPolicyRewriteRuleDefinition
+from catalystwan.endpoints.configuration.policy.definition.rule_set import ConfigurationPolicyRuleSetDefinition
 from catalystwan.endpoints.configuration.policy.definition.security_group import (
     ConfigurationPolicySecurityGroupDefinition,
-    SecurityGroupGetResponse,
 )
-from catalystwan.endpoints.configuration.policy.definition.traffic_data import (
-    ConfigurationPolicyDataDefinition,
-    TrafficDataPolicy,
-    TrafficDataPolicyGetResponse,
+from catalystwan.endpoints.configuration.policy.definition.ssl_decryption import ConfigurationSslDecryptionDefinition
+from catalystwan.endpoints.configuration.policy.definition.ssl_decryption_utd_profile import (
+    ConfigurationSslDecryptionUtdProfileDefinition,
+)
+from catalystwan.endpoints.configuration.policy.definition.traffic_data import ConfigurationPolicyDataDefinition
+from catalystwan.endpoints.configuration.policy.definition.url_filtering import (
+    ConfigurationPolicyUrlFilteringDefinition,
 )
 from catalystwan.endpoints.configuration.policy.definition.vpn_membership import (
     ConfigurationPolicyVPNMembershipGroupDefinition,
-    VPNMembershipPolicyGetResponse,
 )
 from catalystwan.endpoints.configuration.policy.definition.zone_based_firewall import (
     ConfigurationPolicyZoneBasedFirewallDefinition,
-    ZoneBasedFWPolicyGetResponse,
 )
 from catalystwan.endpoints.configuration.policy.list.app import AppListInfo, ConfigurationPolicyApplicationList
-from catalystwan.endpoints.configuration.policy.list.app_probe import (
-    AppProbeClassListInfo,
-    ConfigurationPolicyAppProbeClassList,
-)
+from catalystwan.endpoints.configuration.policy.list.app_probe import ConfigurationPolicyAppProbeClassList
 from catalystwan.endpoints.configuration.policy.list.as_path import ASPathListInfo, ConfigurationPolicyASPathList
-from catalystwan.endpoints.configuration.policy.list.class_map import (
-    ClassMapListInfo,
-    ConfigurationPolicyForwardingClassList,
-)
+from catalystwan.endpoints.configuration.policy.list.class_map import ConfigurationPolicyForwardingClassList
 from catalystwan.endpoints.configuration.policy.list.color import ColorListInfo, ConfigurationPolicyColorList
-from catalystwan.endpoints.configuration.policy.list.community import (
-    CommunityListInfo,
-    ConfigurationPolicyCommunityList,
-)
-from catalystwan.endpoints.configuration.policy.list.data_ipv6_prefix import (
-    ConfigurationPolicyDataIPv6PrefixList,
-    DataIPv6PrefixListInfo,
-)
-from catalystwan.endpoints.configuration.policy.list.data_prefix import (
-    ConfigurationPolicyDataPrefixList,
-    DataPrefixListInfo,
-)
-from catalystwan.endpoints.configuration.policy.list.expanded_community import (
-    ConfigurationPolicyExpandedCommunityList,
-    ExpandedCommunityListInfo,
-)
+from catalystwan.endpoints.configuration.policy.list.community import ConfigurationPolicyCommunityList
+from catalystwan.endpoints.configuration.policy.list.data_ipv6_prefix import ConfigurationPolicyDataIPv6PrefixList
+from catalystwan.endpoints.configuration.policy.list.data_prefix import ConfigurationPolicyDataPrefixList
+from catalystwan.endpoints.configuration.policy.list.expanded_community import ConfigurationPolicyExpandedCommunityList
 from catalystwan.endpoints.configuration.policy.list.fqdn import ConfigurationPolicyFQDNList, FQDNListInfo
-from catalystwan.endpoints.configuration.policy.list.geo_location import (
-    ConfigurationPolicyGeoLocationList,
-    GeoLocationListInfo,
-)
-from catalystwan.endpoints.configuration.policy.list.ips_signature import (
-    ConfigurationPolicyIPSSignatureList,
-    IPSSignatureListInfo,
-)
-from catalystwan.endpoints.configuration.policy.list.ipv6_prefix import (
-    ConfigurationPolicyIPv6PrefixList,
-    IPv6PrefixListInfo,
-)
+from catalystwan.endpoints.configuration.policy.list.geo_location import ConfigurationPolicyGeoLocationList
+from catalystwan.endpoints.configuration.policy.list.ips_signature import ConfigurationPolicyIPSSignatureList
+from catalystwan.endpoints.configuration.policy.list.ipv6_prefix import ConfigurationPolicyIPv6PrefixList
 from catalystwan.endpoints.configuration.policy.list.local_app import ConfigurationPolicyLocalAppList, LocalAppListInfo
-from catalystwan.endpoints.configuration.policy.list.local_domain import (
-    ConfigurationPolicyLocalDomainList,
-    LocalDomainListInfo,
-)
+from catalystwan.endpoints.configuration.policy.list.local_domain import ConfigurationPolicyLocalDomainList
 from catalystwan.endpoints.configuration.policy.list.mirror import ConfigurationPolicyMirrorList, MirrorListInfo
 from catalystwan.endpoints.configuration.policy.list.policer import ConfigurationPolicyPolicerClassList, PolicerListInfo
 from catalystwan.endpoints.configuration.policy.list.port import ConfigurationPolicyPortList, PortListInfo
 from catalystwan.endpoints.configuration.policy.list.preferred_color_group import (
     ConfigurationPreferredColorGroupList,
     PreferredColorGroupListInfo,
 )
@@ -119,15 +73,18 @@
 from catalystwan.endpoints.configuration.policy.list.protocol_name import (
     ConfigurationPolicyProtocolNameList,
     ProtocolNameListInfo,
 )
 from catalystwan.endpoints.configuration.policy.list.region import ConfigurationPolicyRegionList, RegionListInfo
 from catalystwan.endpoints.configuration.policy.list.site import ConfigurationPolicySiteList, SiteListInfo
 from catalystwan.endpoints.configuration.policy.list.sla import ConfigurationPolicySLAClassList, SLAClassListInfo
+from catalystwan.endpoints.configuration.policy.list.threat_grid_api_key import ConfigurationPolicyThreatGridApiKeyList
 from catalystwan.endpoints.configuration.policy.list.tloc import ConfigurationPolicyTLOCList, TLOCListInfo
+from catalystwan.endpoints.configuration.policy.list.trunkgroup import ConfigurationPolicyTrunkGroupList
+from catalystwan.endpoints.configuration.policy.list.umbrella_data import ConfigurationPolicyUmbrellaDataList
 from catalystwan.endpoints.configuration.policy.list.url_allow_list import (
     ConfigurationPolicyURLAllowList,
     URLAllowListInfo,
 )
 from catalystwan.endpoints.configuration.policy.list.url_block_list import (
     ConfigurationPolicyURLBlockList,
     URLBlockListInfo,
@@ -137,30 +94,17 @@
 from catalystwan.endpoints.configuration.policy.security_template import ConfigurationSecurityTemplatePolicy
 from catalystwan.endpoints.configuration.policy.vedge_template import ConfigurationVEdgeTemplatePolicy
 from catalystwan.endpoints.configuration.policy.vsmart_template import (
     ConfigurationVSmartTemplatePolicy,
     VSmartConnectivityStatus,
 )
 from catalystwan.models.misc.application_protocols import ApplicationProtocol
-from catalystwan.models.policy import AnyPolicyDefinition, AnyPolicyList
-from catalystwan.models.policy.centralized import CentralizedPolicy, CentralizedPolicyEditPayload, CentralizedPolicyInfo
-from catalystwan.models.policy.definitions.access_control_list import AclPolicy
-from catalystwan.models.policy.definitions.access_control_list_ipv6 import AclIPv6Policy
-from catalystwan.models.policy.definitions.control import ControlPolicy
-from catalystwan.models.policy.definitions.device_access import DeviceAccessPolicy
-from catalystwan.models.policy.definitions.device_access_ipv6 import DeviceAccessIPv6Policy
-from catalystwan.models.policy.definitions.hub_and_spoke import HubAndSpokePolicy
-from catalystwan.models.policy.definitions.mesh import MeshPolicy
-from catalystwan.models.policy.definitions.qos_map import QoSMapPolicy
-from catalystwan.models.policy.definitions.rewrite import RewritePolicy
-from catalystwan.models.policy.definitions.rule_set import RuleSet
-from catalystwan.models.policy.definitions.security_group import SecurityGroup
-from catalystwan.models.policy.definitions.vpn_membership import VPNMembershipPolicy
-from catalystwan.models.policy.definitions.zone_based_firewall import ZoneBasedFWPolicy
-from catalystwan.models.policy.lists import (
+from catalystwan.models.policy import (
+    AnyPolicyDefinition,
+    AnyPolicyList,
     AppList,
     AppProbeClassList,
     ASPathList,
     ClassMapList,
     ColorList,
     CommunityList,
     DataIPv6PrefixList,
@@ -170,44 +114,92 @@
     GeoLocationList,
     IPSSignatureList,
     IPv6PrefixList,
     LocalAppList,
     LocalDomainList,
     MirrorList,
     PolicerList,
-    PolicyListBase,
     PortList,
     PreferredColorGroupList,
     PrefixList,
     ProtocolNameList,
     RegionList,
     SiteList,
     SLAClassList,
     TLOCList,
     URLAllowList,
     URLBlockList,
     VPNList,
     ZoneList,
 )
+from catalystwan.models.policy.centralized import CentralizedPolicy, CentralizedPolicyEditPayload, CentralizedPolicyInfo
+from catalystwan.models.policy.definition.access_control_list import AclPolicy, AclPolicyGetResponse
+from catalystwan.models.policy.definition.access_control_list_ipv6 import AclIPv6Policy, AclIPv6PolicyGetResponse
+from catalystwan.models.policy.definition.aip import (
+    AdvancedInspectionProfilePolicy,
+    AdvancedInspectionProfilePolicyGetResponse,
+)
+from catalystwan.models.policy.definition.amp import (
+    AdvancedMalwareProtectionPolicy,
+    AdvancedMalwareProtectionPolicyGetResponse,
+)
+from catalystwan.models.policy.definition.cflowd import CflowdPolicy, CflowdPolicyGetResponse
+from catalystwan.models.policy.definition.control import ControlPolicy, ControlPolicyGetResponse
+from catalystwan.models.policy.definition.device_access import DeviceAccessPolicy, DeviceAccessPolicyGetResponse
+from catalystwan.models.policy.definition.device_access_ipv6 import (
+    DeviceAccessIPv6Policy,
+    DeviceAccessIPv6PolicyGetResponse,
+)
+from catalystwan.models.policy.definition.dns_security import DnsSecurityPolicy, DnsSecurityPolicyGetResponse
+from catalystwan.models.policy.definition.hub_and_spoke import HubAndSpokePolicy, HubAndSpokePolicyGetResponse
+from catalystwan.models.policy.definition.intrusion_prevention import (
+    IntrusionPreventionPolicy,
+    IntrusionPreventionPolicyGetResponse,
+)
+from catalystwan.models.policy.definition.mesh import MeshPolicy, MeshPolicyGetResponse
+from catalystwan.models.policy.definition.qos_map import QoSMapPolicy, QoSMapPolicyGetResponse
+from catalystwan.models.policy.definition.rewrite import RewritePolicy, RewritePolicyGetResponse
+from catalystwan.models.policy.definition.rule_set import RuleSet, RuleSetGetResponse
+from catalystwan.models.policy.definition.security_group import SecurityGroup, SecurityGroupGetResponse
+from catalystwan.models.policy.definition.ssl_decryption import SslDecryptionPolicy, SslDecryptionPolicyGetResponse
+from catalystwan.models.policy.definition.ssl_decryption_utd_profile import (
+    SslDecryptionUtdProfilePolicy,
+    SslDecryptionUtdProfilePolicyGetResponse,
+)
+from catalystwan.models.policy.definition.traffic_data import TrafficDataPolicy, TrafficDataPolicyGetResponse
+from catalystwan.models.policy.definition.url_filtering import UrlFilteringPolicy, UrlFilteringPolicyGetResponse
+from catalystwan.models.policy.definition.vpn_membership import VPNMembershipPolicy, VPNMembershipPolicyGetResponse
+from catalystwan.models.policy.definition.zone_based_firewall import ZoneBasedFWPolicy, ZoneBasedFWPolicyGetResponse
+from catalystwan.models.policy.list.app_probe import AppProbeClassListInfo
+from catalystwan.models.policy.list.class_map import ClassMapListInfo
+from catalystwan.models.policy.list.communities import CommunityListInfo, ExpandedCommunityListInfo
+from catalystwan.models.policy.list.data_ipv6_prefix import DataIPv6PrefixListInfo
+from catalystwan.models.policy.list.data_prefix import DataPrefixListInfo
+from catalystwan.models.policy.list.geo_location import GeoLocationListInfo
+from catalystwan.models.policy.list.ips_signature import IPSSignatureListInfo
+from catalystwan.models.policy.list.ipv6_prefix import IPv6PrefixListInfo
+from catalystwan.models.policy.list.local_domain import LocalDomainListInfo
+from catalystwan.models.policy.list.threat_grid_api_key import ThreatGridApiKeyList, ThreatGridApiKeyListInfo
+from catalystwan.models.policy.list.trunkgroup import TrunkGroupList, TrunkGroupListInfo
+from catalystwan.models.policy.list.umbrella_data import UmbrellaDataList, UmbrellaDataListInfo
 from catalystwan.models.policy.localized import (
     LocalizedPolicy,
     LocalizedPolicyDeviceInfo,
     LocalizedPolicyEditResponse,
     LocalizedPolicyInfo,
 )
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionBase,
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
     PolicyDefinitionInfo,
 )
-from catalystwan.models.policy.policy_list import PolicyListEndpoints
+from catalystwan.models.policy.policy_list import PolicyListBase
 from catalystwan.models.policy.security import (
     AnySecurityPolicy,
-    AnySecurityPolicyInfo,
+    AnySecurityPolicyInfoList,
     SecurityPolicy,
     SecurityPolicyEditResponse,
     UnifiedSecurityPolicy,
 )
 from catalystwan.typed_list import DataSequence
 
 if TYPE_CHECKING:
@@ -235,15 +227,18 @@
     PortList: ConfigurationPolicyPortList,
     PreferredColorGroupList: ConfigurationPreferredColorGroupList,
     PrefixList: ConfigurationPolicyPrefixList,
     ProtocolNameList: ConfigurationPolicyProtocolNameList,
     RegionList: ConfigurationPolicyRegionList,
     SiteList: ConfigurationPolicySiteList,
     SLAClassList: ConfigurationPolicySLAClassList,
+    ThreatGridApiKeyList: ConfigurationPolicyThreatGridApiKeyList,
     TLOCList: ConfigurationPolicyTLOCList,
+    TrunkGroupList: ConfigurationPolicyTrunkGroupList,
+    UmbrellaDataList: ConfigurationPolicyUmbrellaDataList,
     URLBlockList: ConfigurationPolicyURLBlockList,
     URLAllowList: ConfigurationPolicyURLAllowList,
     VPNList: ConfigurationPolicyVPNList,
     ZoneList: ConfigurationPolicyZoneList,
 }
 
 POLICY_DEFINITION_ENDPOINTS_MAP: Mapping[type, type] = {
@@ -257,14 +252,22 @@
     VPNMembershipPolicy: ConfigurationPolicyVPNMembershipGroupDefinition,
     HubAndSpokePolicy: ConfigurationPolicyHubAndSpokeDefinition,
     MeshPolicy: ConfigurationPolicyMeshDefinition,
     AclPolicy: ConfigurationPolicyAclDefinition,
     AclIPv6Policy: ConfigurationPolicyAclIPv6Definition,
     DeviceAccessPolicy: ConfigurationPolicyDeviceAccessDefinition,
     DeviceAccessIPv6Policy: ConfigurationPolicyDeviceAccessIPv6Definition,
+    AdvancedInspectionProfilePolicy: ConfigurationPolicyAIPDefinition,
+    AdvancedMalwareProtectionPolicy: ConfigurationPolicyAMPDefinition,
+    IntrusionPreventionPolicy: ConfigurationPolicyIntrusionPreventionDefinition,
+    SslDecryptionPolicy: ConfigurationSslDecryptionDefinition,
+    SslDecryptionUtdProfilePolicy: ConfigurationSslDecryptionUtdProfileDefinition,
+    UrlFilteringPolicy: ConfigurationPolicyUrlFilteringDefinition,
+    DnsSecurityPolicy: ConfigurationPolicyDnsSecurityDefinition,
+    CflowdPolicy: ConfigurationPolicyCflowdDefinition,
 }
 
 
 class CentralizedPolicyAPI:
     def __init__(self, session: ManagerSession):
         self._session = session
         self._endpoints = ConfigurationVSmartTemplatePolicy(session)
@@ -360,25 +363,25 @@
     def edit(self, id: UUID, policy: AnySecurityPolicy) -> SecurityPolicyEditResponse:
         return self._endpoints.edit_security_template(id, policy)
 
     def delete(self, id: UUID) -> None:
         self._endpoints.delete_security_template(id)
 
     @overload
-    def get(self) -> List[AnySecurityPolicyInfo]:
+    def get(self) -> AnySecurityPolicyInfoList:
         ...
 
     @overload
     def get(self, id: UUID) -> AnySecurityPolicy:
         ...
 
     def get(self, id: Optional[UUID] = None) -> Any:
         if id is not None:
             return self._endpoints.get_security_template(id).root
-        return [info.root for info in self._endpoints.generate_security_template_list()]
+        return self._endpoints.generate_security_template_list()
 
 
 class PolicyListsAPI:
     def __init__(self, session: ManagerSession):
         self._session = session
 
     def __get_list_endpoints_instance(self, payload_type: type) -> PolicyListEndpoints:
@@ -492,18 +495,30 @@
         ...
 
     @overload
     def get(self, type: Type[SLAClassList]) -> DataSequence[SLAClassListInfo]:
         ...
 
     @overload
+    def get(self, type: Type[ThreatGridApiKeyList]) -> DataSequence[ThreatGridApiKeyListInfo]:
+        ...
+
+    @overload
     def get(self, type: Type[TLOCList]) -> DataSequence[TLOCListInfo]:
         ...
 
     @overload
+    def get(self, type: Type[TrunkGroupList]) -> DataSequence[TrunkGroupListInfo]:
+        ...
+
+    @overload
+    def get(self, type: Type[UmbrellaDataList]) -> DataSequence[UmbrellaDataListInfo]:
+        ...
+
+    @overload
     def get(self, type: Type[URLBlockList]) -> DataSequence[URLBlockListInfo]:
         ...
 
     @overload
     def get(self, type: Type[URLAllowList]) -> DataSequence[URLAllowListInfo]:
         ...
 
@@ -610,18 +625,30 @@
         ...
 
     @overload
     def get(self, type: Type[SLAClassList], id: UUID) -> SLAClassListInfo:
         ...
 
     @overload
+    def get(self, type: Type[ThreatGridApiKeyList], id: UUID) -> ThreatGridApiKeyListInfo:
+        ...
+
+    @overload
     def get(self, type: Type[TLOCList], id: UUID) -> TLOCListInfo:
         ...
 
     @overload
+    def get(self, type: Type[TrunkGroupList], id: UUID) -> TrunkGroupListInfo:
+        ...
+
+    @overload
+    def get(self, type: Type[UmbrellaDataList], id: UUID) -> UmbrellaDataListInfo:
+        ...
+
+    @overload
     def get(self, type: Type[URLBlockList], id: UUID) -> URLBlockListInfo:
         ...
 
     @overload
     def get(self, type: Type[URLAllowList], id: UUID) -> URLAllowListInfo:
         ...
 
@@ -635,14 +662,20 @@
 
     def get(self, type: Type[AnyPolicyList], id: Optional[UUID] = None) -> Any:
         endpoints = self.__get_list_endpoints_instance(type)
         if id is not None:
             return endpoints.get_lists_by_id(id=id)
         return endpoints.get_policy_lists()
 
+    def get_all(self) -> List[AnyPolicyList]:
+        infos: List[AnyPolicyList] = []
+        for list_type, _ in POLICY_LIST_ENDPOINTS_MAP.items():
+            infos.extend(self.get(list_type))
+        return infos
+
 
 class PolicyDefinitionsAPI:
     def __init__(self, session: ManagerSession):
         self._session = session
 
     def __get_definition_endpoints_instance(self, payload_type: type) -> PolicyDefinitionEndpoints:
         endpoints_class = POLICY_DEFINITION_ENDPOINTS_MAP.get(payload_type)
@@ -659,26 +692,58 @@
         return endpoints.edit_policy_definition(id=id, payload=policy_definition)
 
     def delete(self, type: Type[AnyPolicyDefinition], id: UUID) -> None:
         endpoints = self.__get_definition_endpoints_instance(type)
         endpoints.delete_policy_definition(id=id)
 
     @overload
+    def get(self, type: Type[IntrusionPreventionPolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
     def get(self, type: Type[TrafficDataPolicy]) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
     @overload
+    def get(self, type: Type[UrlFilteringPolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
+    def get(self, type: Type[AdvancedInspectionProfilePolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
+    def get(self, type: Type[AdvancedMalwareProtectionPolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
+    def get(self, type: Type[CflowdPolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
+    def get(self, type: Type[DnsSecurityPolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
     def get(self, type: Type[RuleSet]) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
     @overload
     def get(self, type: Type[SecurityGroup]) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
     @overload
+    def get(self, type: Type[SslDecryptionPolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
+    def get(self, type: Type[SslDecryptionUtdProfilePolicy]) -> DataSequence[PolicyDefinitionInfo]:
+        ...
+
+    @overload
     def get(self, type: Type[ZoneBasedFWPolicy]) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
     @overload
     def get(self, type: Type[QoSMapPolicy]) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
@@ -715,28 +780,59 @@
         ...
 
     @overload
     def get(self, type: Type[DeviceAccessIPv6Policy]) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
     # get by id
+    @overload
+    def get(self, type: Type[IntrusionPreventionPolicy], id: UUID) -> IntrusionPreventionPolicyGetResponse:
+        ...
 
     @overload
     def get(self, type: Type[TrafficDataPolicy], id: UUID) -> TrafficDataPolicyGetResponse:
         ...
 
     @overload
+    def get(self, type: Type[UrlFilteringPolicy], id: UUID) -> UrlFilteringPolicyGetResponse:
+        ...
+
+    @overload
+    def get(self, type: Type[AdvancedInspectionProfilePolicy], id: UUID) -> AdvancedInspectionProfilePolicyGetResponse:
+        ...
+
+    @overload
+    def get(self, type: Type[AdvancedMalwareProtectionPolicy], id: UUID) -> AdvancedMalwareProtectionPolicyGetResponse:
+        ...
+
+    @overload
+    def get(self, type: Type[CflowdPolicy], id: UUID) -> CflowdPolicyGetResponse:
+        ...
+
+    @overload
+    def get(self, type: Type[DnsSecurityPolicy], id: UUID) -> DnsSecurityPolicyGetResponse:
+        ...
+
+    @overload
     def get(self, type: Type[RuleSet], id: UUID) -> RuleSetGetResponse:
         ...
 
     @overload
     def get(self, type: Type[SecurityGroup], id: UUID) -> SecurityGroupGetResponse:
         ...
 
     @overload
+    def get(self, type: Type[SslDecryptionPolicy], id: UUID) -> SslDecryptionPolicyGetResponse:
+        ...
+
+    @overload
+    def get(self, type: Type[SslDecryptionUtdProfilePolicy], id: UUID) -> SslDecryptionUtdProfilePolicyGetResponse:
+        ...
+
+    @overload
     def get(self, type: Type[ZoneBasedFWPolicy], id: UUID) -> ZoneBasedFWPolicyGetResponse:
         ...
 
     @overload
     def get(self, type: Type[QoSMapPolicy], id: UUID) -> QoSMapPolicyGetResponse:
         ...
 
@@ -778,14 +874,20 @@
 
     def get(self, type: Type[AnyPolicyDefinition], id: Optional[UUID] = None) -> Any:
         endpoints = self.__get_definition_endpoints_instance(type)
         if id is not None:
             return endpoints.get_policy_definition(id=id)
         return endpoints.get_definitions()
 
+    def get_all(self) -> List[Tuple[type, PolicyDefinitionInfo]]:
+        all_items: List[Tuple[type, PolicyDefinitionInfo]] = []
+        for definition_type, _ in POLICY_DEFINITION_ENDPOINTS_MAP.items():
+            all_items.extend([(definition_type, info) for info in self.get(definition_type)])
+        return all_items
+
 
 class PolicyAPI:
     """This is exposing so called 'UX 1.0' API"""
 
     def __init__(self, session: ManagerSession):
         self._session = session
         self.centralized = CentralizedPolicyAPI(session)
```

### Comparing `catalystwan-0.33.6/catalystwan/api/resource_pool_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/resource_pool_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/software_action_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/speedtest_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/speedtest_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/task_status_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/template_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/template_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from catalystwan.api.templates.models.cli_template import CliTemplateModel
 from catalystwan.api.templates.models.omp_vsmart_model import OMPvSmart
 from catalystwan.api.templates.models.security_vsmart_model import SecurityvSmart
 from catalystwan.api.templates.models.system_vsmart_model import SystemVsmart
 from catalystwan.dataclasses import Device, DeviceTemplateInfo, FeatureTemplateInfo, FeatureTemplatesTypes, TemplateInfo
 from catalystwan.endpoints.configuration_device_template import FeatureToCLIPayload
 from catalystwan.exceptions import AttachedError, TemplateNotFoundError
+from catalystwan.models.templates import DeviceTemplateInformation, FeatureTemplateInformation
 from catalystwan.response import ManagerResponse
 from catalystwan.typed_list import DataSequence
 from catalystwan.utils.device_model import DeviceModel
 from catalystwan.utils.dict import merge
 from catalystwan.utils.pydantic_field import get_extra_field
 from catalystwan.utils.template_type import TemplateType
 
@@ -694,7 +695,23 @@
         """
         encoded_uuid = device.uuid.replace("/", "%2F")
         endpoint = f"/dataservice/template/config/running/{encoded_uuid}"
         response = self.session.get_json(endpoint)
         config = CiscoConfParse(response["config"].splitlines())
         logger.debug(f"Template loaded from {device.hostname}.")
         return config
+
+    def get_feature_templates(self) -> DataSequence[FeatureTemplateInformation]:
+        endpoint = "/dataservice/template/feature"
+        fr_templates = self.session.get(endpoint)
+        return fr_templates.dataseq(FeatureTemplateInformation)
+
+    def get_device_templates(self) -> DataSequence[DeviceTemplateInformation]:
+        endpoint = "/dataservice/template/device"
+        params = {"feature": "all"}
+        templates = self.session.get(url=endpoint, params=params)
+        return templates.dataseq(DeviceTemplateInformation)
+
+    def get_device_template(self, template_id: str) -> DeviceTemplate:
+        endpoint = f"/dataservice/template/device/object/{template_id}"
+        response = self.session.get(endpoint)
+        return DeviceTemplate(**response.json())
```

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/README.md` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/cli_template.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/device_template/device_template.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/device_template/device_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
 import logging
 from pathlib import Path
-from typing import TYPE_CHECKING, Final, List
+from typing import TYPE_CHECKING, ClassVar, List
 
 from jinja2 import DebugUndefined, Environment, FileSystemLoader, meta  # type: ignore
 from pydantic import BaseModel, ConfigDict, Field, field_validator
 
-from catalystwan.utils.device_model import DeviceModel
-
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
 logger = logging.getLogger(__name__)
 
 
 class GeneralTemplate(BaseModel):
@@ -40,21 +38,25 @@
             template_name="python",
             template_description="python",
             general_templates=templates
         )
     >>> session.api.templates.create(device_template)
     """
 
-    template_name: str = Field(alias="templateName")
-    template_description: str = Field(alias="templateDescription")
-    general_templates: List[GeneralTemplate] = Field(alias="generalTemplates")
-    device_role: str = Field(default="sdwan-edge", alias="deviceRole")
-    device_type: DeviceModel = Field(alias="deviceType")
-    security_policy_id: str = Field(default="", alias="securityPolicyId")
-    policy_id: str = Field(default="", alias="policyId")
+    template_name: str = Field(serialization_alias="templateName", validation_alias="templateName")
+    template_description: str = Field(serialization_alias="templateDescription", validation_alias="templateDescription")
+    general_templates: List[GeneralTemplate] = Field(
+        default=[], serialization_alias="generalTemplates", validation_alias="generalTemplates"
+    )
+    device_role: str = Field(default="sdwan-edge", serialization_alias="deviceRole", validation_alias="deviceRole")
+    device_type: str = Field(serialization_alias="deviceType", validation_alias="deviceType")
+    security_policy_id: str = Field(
+        default="", serialization_alias="securityPolicyId", validation_alias="securityPolicyId"
+    )
+    policy_id: str = Field(default="", serialization_alias="policyId", validation_alias="policyId")
 
     def generate_payload(self) -> str:
         env = Environment(
             loader=FileSystemLoader(self.payload_path.parent),
             trim_blocks=True,
             lstrip_blocks=True,
             undefined=DebugUndefined,
@@ -75,15 +77,15 @@
         for template in value:
             if isinstance(template, str):
                 output.append(GeneralTemplate(name=template))
             else:
                 output.append(template)
         return output
 
-    payload_path: Final[Path] = Path(__file__).parent / "device_template_payload.json.j2"
+    payload_path: ClassVar[Path] = Path(__file__).parent / "device_template_payload.json.j2"
 
     @classmethod
     def get(self, name: str, session: ManagerSession) -> DeviceTemplate:
         device_template = session.api.templates.get(DeviceTemplate).filter(name=name).single_or_default()
         resp = session.get(f"dataservice/template/device/object/{device_template.id}").json()
         return DeviceTemplate(**resp)
```

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/device_template/device_template_payload.json.j2` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/device_template/device_template_payload.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/feature_template.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/feature_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/feature_template_field.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/feature_template_payload.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/feature_template_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_aaa_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_banner_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_banner_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_bfd_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_bfd_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_bgp_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_bgp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_logging_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_logging_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_ntp_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_ntp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_omp_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_omp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_ospf.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_ospfv3.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_secure_internet_gateway.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_secure_internet_gateway.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_snmp_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_snmp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_system.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_vpn_interface_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_vpn_interface_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/cisco_vpn_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/omp_vsmart_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/omp_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/security_vsmart_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/security_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/supported.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/supported.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/models/system_vsmart_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/models/system_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/aaa_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/aaa/aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/aaa/feature/user.json.j2` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/aaa/feature/user.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/tenant/tenant.json.j2` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/tenant/tenant.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/templates/payloads/tenant/tenant_model.py` & `catalystwan-0.33.6.dev0/catalystwan/api/templates/payloads/tenant/tenant_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/tenant_backup_restore_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/tenant_management_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/tenant_migration_api.py` & `catalystwan-0.33.6.dev0/catalystwan/api/tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/api/versions_utils.py` & `catalystwan-0.33.6.dev0/catalystwan/api/versions_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,15 @@
 import logging
 from pathlib import PurePath
 from typing import TYPE_CHECKING, Dict, List, Union
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from catalystwan.endpoints.configuration.software_actions import SoftwareImageDetails
-from catalystwan.endpoints.configuration_device_actions import (
-    InstallLxcImage,
-    LxcActivateDevice,
-    LxcUpgradeDevice,
-    PartitionDevice,
-)
+from catalystwan.endpoints.configuration_device_actions import PartitionDevice
 from catalystwan.endpoints.configuration_device_inventory import DeviceDetailsResponse
 from catalystwan.exceptions import ImageNotInRepositoryError
 from catalystwan.typed_list import DataSequence
 from catalystwan.utils.upgrades_helper import SoftwarePackageUploadPayload
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
@@ -68,26 +63,14 @@
 
         Returns:
             list: software images list
         """
         software_images = self.session.endpoints.configuration_software_actions.get_list_of_all_images()
         return software_images
 
-    def get_all_virtual_images(self) -> DataSequence[SoftwareImageDetails]:
-        """
-        Get all info about all software images stored in Vmanage repository
-
-        Returns:
-            list: software images list
-        """
-        software_images = self.session.endpoints.configuration_software_actions.get_list_of_all_images(
-            "imageType=virtualmachine"
-        )
-        return software_images
-
     def get_devices_versions_repository(self) -> Dict[str, DeviceSoftwareRepository]:
         """
         Create DeviceSoftwareRepository dataclass,
         which cointains information about all possible version types for certain devices
 
         Returns:
             Dict[str, DeviceSoftwareRepository]: Dictionary containing all versions
@@ -222,62 +205,14 @@
             if not device.uuid or not device.local_system_ip:
                 raise ValueError(
                     f"Provided device '{device.host_name}' doesn't include required fields for this operation:"
                     f"device.uuid (current value: {device.uuid})"
                     f"device.device_ip (current value: {device.device_ip})"
                 )
 
-    def get_lxcactivate_device_list(
-        self,
-        version_to_set_up: str,
-        devices: DataSequence[DeviceDetailsResponse],
-    ) -> DataSequence[LxcActivateDevice]:
-        self._validate_devices_required_fields(devices)
-        install_image_payload = [
-            InstallLxcImage(
-                network_function_type="app-hosting",
-                version_name=version_to_set_up,
-                version_type_name="UTD-Snort-Feature",
-            )
-        ]
-        devices_payload = DataSequence(
-            LxcActivateDevice,
-            [
-                LxcActivateDevice(
-                    device_id=str(device.uuid),
-                    device_ip=str(device.local_system_ip),
-                    install_images=install_image_payload,
-                )
-                for device in devices
-            ],  # type: ignore
-        )
-
-        return devices_payload
-
-    def get_lxcupgrade_device_list(
-        self,
-        version_to_set_up: str,
-        devices: DataSequence[DeviceDetailsResponse],
-    ) -> DataSequence[LxcUpgradeDevice]:
-        self._validate_devices_required_fields(devices)
-        install_image_payload = [InstallLxcImage(version_name=version_to_set_up)]
-        devices_payload = DataSequence(
-            LxcUpgradeDevice,
-            [
-                LxcUpgradeDevice(
-                    device_id=str(device.uuid),
-                    device_ip=str(device.local_system_ip),
-                    install_images=install_image_payload,
-                )
-                for device in devices
-            ],  # type: ignore
-        )
-
-        return devices_payload
-
     def _get_device_list_in(
         self, version_to_set_up: str, devices: DataSequence[DeviceDetailsResponse], version_type: str
     ) -> DataSequence[PartitionDevice]:
         """
         Create devices payload list included requested version, if requested version
         is in specified version type
 
@@ -288,18 +223,16 @@
 
         Returns:
             list : list of devices
         """
         self._validate_devices_required_fields(devices)
         devices_payload = DataSequence(
             PartitionDevice,
-            [PartitionDevice(device_id=str(device.uuid), device_ip=str(device.local_system_ip)) for device in devices],
-            # type: ignore
+            [PartitionDevice(device_id=device.uuid, device_ip=device.device_ip) for device in devices],  # type: ignore
         )
-
         all_dev_versions = self.repository.get_devices_versions_repository()
         for device in devices_payload:
             device_versions = getattr(all_dev_versions[device.device_id], version_type)
             try:
                 for version in device_versions:
                     if version_to_set_up in version:
                         device.version = version
@@ -358,18 +291,17 @@
         Returns:
             list : list of devices
         """
         self._validate_devices_required_fields(devices)
 
         devices_payload = DataSequence(
             PartitionDevice,
-            [
-                PartitionDevice(device_id=device.uuid, device_ip=device.local_system_ip)  # type: ignore
-                for device in devices
-            ],  # type: ignore
+            [PartitionDevice(
+                device_id=device.uuid, device_ip=device.local_system_ip  # type: ignore
+            ) for device in devices],  # type: ignore
         )
         all_dev_versions = self.repository.get_devices_versions_repository()
         for device in devices_payload:
             device.version = getattr(all_dev_versions[device.device_id], version_type)
         return devices_payload
 
     def get_devices_current_version(
```

### Comparing `catalystwan-0.33.6/catalystwan/dataclasses.py` & `catalystwan-0.33.6.dev0/catalystwan/dataclasses.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/__init__.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     Literal,
     Mapping,
     Optional,
     Protocol,
     Sequence,
     Set,
     Tuple,
+    Type,
     TypeVar,
     Union,
     runtime_checkable,
 )
 from uuid import UUID
 
 from packaging.specifiers import SpecifierSet  # type: ignore
@@ -109,14 +110,53 @@
     def json(cls) -> TypeSpecifier:
         return TypeSpecifier(present=True, is_json=True)
 
     @classmethod
     def model_union(cls, models: Sequence[type]) -> TypeSpecifier:
         return TypeSpecifier(present=True, payload_union_model_types=models)
 
+    @classmethod
+    def resolve_nested_base_model_unions(
+        cls, annotation: Any, models_types: List[Type[BaseModel]]
+    ) -> List[Type[BaseModel]]:
+        type_origin = get_origin(annotation)
+        if isclass(annotation):
+            try:
+                if issubclass(annotation, BaseModel):
+                    return [annotation]
+                raise APIEndpointError(f"Expected: {PayloadType}")
+            except TypeError:
+                raise APIEndpointError(f"Expected: {PayloadType}")
+        # Check if Annnotated[Union[PayloadModelType, ...]], only unions of pydantic models allowed
+        elif type_origin == Annotated:
+            if annotated_origin := get_args(annotation):
+                if (len(annotated_origin) >= 1) and get_origin(annotated_origin[0]) == Union:
+                    type_args = get_args(annotated_origin[0])
+                    if all(isclass(t) for t in type_args) and all(issubclass(t, BaseModel) for t in type_args):
+                        models_types.extend(list(type_args))
+                        return models_types
+                    else:
+                        non_models = [t for t in type_args if not isclass(t)]
+                        for non_model in non_models:
+                            models_types.extend(cls.resolve_nested_base_model_unions(non_model, models_types))
+                        return models_types
+
+        # Check if Union[PayloadModelType, ...], only unions of pydantic models allowed
+        elif type_origin == Union:
+            type_args = get_args(annotation)
+            if all(isclass(t) for t in type_args) and all(issubclass(t, BaseModel) for t in type_args):
+                models_types.extend(list(type_args))
+                return models_types
+            else:
+                non_models = [t for t in type_args if not isclass(t)]
+                for non_model in non_models:
+                    models_types.extend(cls.resolve_nested_base_model_unions(non_model, models_types))
+                return models_types
+        raise APIEndpointError(f"Expected: {PayloadType}")
+
 
 @dataclass
 class APIEndpointRequestMeta:
     """Holds data for endpoints exctracted during decorating. Used for documentation"""
 
     func: Any
     http_request: str
@@ -157,51 +197,54 @@
     """
     Class to be used as base for all API endpoints.
     Injects BASE_PATH url prefix as it is common for all known vManage API endpoints.
     Introduces special keyword argument 'payload' in request call and handles sending of such object.
     """
 
     @classmethod
-    def _prepare_payload(cls, payload: PayloadType, force_json: bool = False) -> PreparedPayload:
+    def _prepare_payload(
+        cls, payload: PayloadType, force_json: bool = False, context: Dict[str, Any] = {}
+    ) -> PreparedPayload:
         """Helper method to prepare data for sending based on type"""
         if force_json or isinstance(payload, dict):
             return PreparedPayload(data=json.dumps(payload), headers={"content-type": "application/json"})
         if isinstance(payload, (str, bytes)):
             return PreparedPayload(data=payload)
         elif isinstance(payload, (BaseModel)):
-            return cls._prepare_basemodel_payload(payload)
+            return cls._prepare_basemodel_payload(payload, context)
         elif isinstance(payload, Sequence) and not isinstance(payload, (str, bytes)):
-            return cls._prepare_sequence_payload(payload)  # type: ignore[arg-type]
+            return cls._prepare_sequence_payload(payload, context)  # type: ignore[arg-type]
             # offender is List[JSON] which is also a Sequence can be ignored as long as force_json is passed correctly
         elif isinstance(payload, CustomPayloadType):
             return payload.prepared()
         else:
             raise APIRequestPayloadTypeError(payload)
 
     @classmethod
-    def _prepare_basemodel_payload(cls, payload: BaseModel) -> PreparedPayload:
+    def _prepare_basemodel_payload(cls, payload: BaseModel, context: Dict[str, Any] = {}) -> PreparedPayload:
         """Helper method to prepare BaseModel instance for sending"""
         return PreparedPayload(
-            data=payload.model_dump_json(exclude_none=True, by_alias=True), headers={"content-type": "application/json"}
+            data=payload.model_dump_json(exclude_none=True, by_alias=True, context=context),
+            headers={"content-type": "application/json"},
         )
 
     @classmethod
-    def _prepare_sequence_payload(cls, payload: Iterable[BaseModel]) -> PreparedPayload:
+    def _prepare_sequence_payload(cls, payload: Iterable[BaseModel], context: Dict[str, Any] = {}) -> PreparedPayload:
         """Helper method to prepare sequences for sending"""
         items = []
         for item in payload:
-            items.append(item.model_dump(exclude_none=True, by_alias=True))
+            items.append(item.model_dump(exclude_none=True, by_alias=True, context=context))
         data = json.dumps(items)
         return PreparedPayload(data=data, headers={"content-type": "application/json"})
 
     @classmethod
-    def _prepare_params(cls, params: RequestParamsType) -> Dict[str, Any]:
+    def _prepare_params(cls, params: RequestParamsType, context: Dict[str, Any] = {}) -> Dict[str, Any]:
         """Helper method to prepare params for sending"""
         if isinstance(params, BaseModel):
-            return params.model_dump(exclude_none=True, by_alias=True)
+            return params.model_dump(exclude_none=True, by_alias=True, context=context)
         return params
 
     def __init__(self, client: APIEndpointClient):
         self._client = client
         self._basepath = BASE_PATH
 
     def _request(
@@ -211,18 +254,19 @@
         payload: Optional[ModelPayloadType] = None,
         params: Optional[RequestParamsType] = None,
         force_json_payload: bool = False,
         **kwargs,
     ) -> APIEndpointClientResponse:
         """Prepares and sends request using client protocol"""
         _kwargs = dict(kwargs)
+        context = dict(api_version=self._api_version)
         if payload is not None:
-            _kwargs.update(self._prepare_payload(payload, force_json_payload).asdict())
+            _kwargs.update(self._prepare_payload(payload, force_json_payload, context).asdict())
         if params is not None:
-            _kwargs.update({"params": self._prepare_params(params)})
+            _kwargs.update({"params": self._prepare_params(params, context)})
         return self._client.request(method, self._basepath + url, **_kwargs)
 
     @property
     def _api_version(self) -> Optional[Version]:
         return self._client.api_version
 
     @property
@@ -437,35 +481,18 @@
                 if (
                     (type_args := get_args(annotation))
                     and (len(type_args) == 1)
                     and isclass(type_args[0])
                     and issubclass(type_args[0], BaseModel)
                 ):
                     return TypeSpecifier(True, type_origin, type_args[0], None, False, is_optional)
-            # Check if Annnotated[Union[PayloadModelType, ...]], only unions of pydantic models allowed
-            elif type_origin == Annotated:
-                if annotated_origin := get_args(annotation):
-                    if (len(annotated_origin) >= 1) and get_origin(annotated_origin[0]) == Union:
-                        if (
-                            (type_args := get_args(annotated_origin[0]))
-                            and all(isclass(t) for t in type_args)
-                            and all(issubclass(t, BaseModel) for t in type_args)
-                        ):
-                            return TypeSpecifier.model_union(models=list(type_args))
-            # Check if Union[PayloadModelType, ...], only unions of pydantic models allowed
-            elif type_origin == Union:
-                if (
-                    (type_args := get_args(annotation))
-                    and all(isclass(t) for t in type_args)
-                    and all(issubclass(t, BaseModel) for t in type_args)
-                ):
-                    return TypeSpecifier.model_union(models=list(type_args))
-            raise APIEndpointError(f"Expected: {PayloadType} but found payload {annotation}")
-        else:
-            raise APIEndpointError(f"Expected: {PayloadType} but found payload {annotation}")
+            else:
+                models = TypeSpecifier.resolve_nested_base_model_unions(annotation, [])
+                return TypeSpecifier.model_union(models)
+        raise APIEndpointError(f"'payload' param must be annotated with supported type: {PayloadType}")
 
     def check_params(self):
         """Checks params in decorated method definition
 
         Raises:
             APIEndpointError: when decorated params not matching specification
         """
@@ -564,19 +591,19 @@
                 if self.return_spec.payload_type is None:
                     pass
                 elif issubclass(self.return_spec.payload_type, BaseModel):
                     if self.return_spec.sequence_type == DataSequence:
                         return response.dataseq(
                             cls=self.return_spec.payload_type,
                             sourcekey=self.resp_json_key,
-                            validate=_self._client.validate_responses,
+                            validate=_self._client.validate_response,
                         )
                     else:
                         return response.dataobj(
-                            self.return_spec.payload_type, self.resp_json_key, validate=_self._client.validate_responses
+                            self.return_spec.payload_type, self.resp_json_key, validate=_self._client.validate_response
                         )
                 elif issubclass(self.return_spec.payload_type, str):
                     return response.text
                 elif issubclass(self.return_spec.payload_type, bytes):
                     return response.content
                 elif issubclass(self.return_spec.payload_type, dict):
                     return response.json()
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/administration_user_and_group.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/administration_user_and_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/certificate_management_device.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/certificate_management_device.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/certificate_management_vmanage.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/certificate_management_vmanage.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/client.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/client.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/cluster_management.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/cluster_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/device/software_update.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/device/software_update.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/disaster_recovery.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/disaster_recovery.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
-from catalystwan.models.configuration.feature_profile.common import Parcel, ParcelCreationResponse
+from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse
 from catalystwan.models.configuration.feature_profile.sdwan.policy_object import AnyPolicyObjectParcel
 from catalystwan.typed_list import DataSequence
 
 
 class PolicyObjectFeatureProfile(APIEndpoints):
     @versions(supported_versions=(">=20.13"), raises=False)
     @post("/v1/feature-profile/sdwan/policy-object/{profile_id}/{policy_object_list_type}")
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,62 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from typing import Optional
+from uuid import UUID
 
 from catalystwan.api.configuration_groups.parcel import _ParcelBase
-from catalystwan.endpoints import JSON, APIEndpoints, delete, get, post, put, versions
+from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileInfo,
     GetFeatureProfilesPayload,
-    ParcelId,
-    SchemaTypeQuery,
 )
+from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelId
 from catalystwan.typed_list import DataSequence
 
 
-class SystemFeatureProfile(APIEndpoints):
+class OtherFeatureProfile(APIEndpoints):
     @versions(supported_versions=(">=20.9"), raises=False)
-    @get("/v1/feature-profile/sdwan/system/aaa/schema", resp_json_key="request")
-    def get_sdwan_system_aaa_parcel_schema(self, params: SchemaTypeQuery) -> JSON:
-        ...
-
-    @versions(supported_versions=(">=20.9"), raises=False)
-    @get("/v1/feature-profile/sdwan/system")
-    def get_sdwan_system_feature_profiles(
+    @get("/v1/feature-profile/sdwan/other")
+    def get_sdwan_other_feature_profiles(
         self, payload: Optional[GetFeatureProfilesPayload]
     ) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
-    @post("/v1/feature-profile/sdwan/system")
-    def create_sdwan_system_feature_profile(
+    @post("/v1/feature-profile/sdwan/other")
+    def create_sdwan_other_feature_profile(
         self, payload: FeatureProfileCreationPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
-    @delete("/v1/feature-profile/sdwan/system/{system_id}")
-    def delete_sdwan_system_feature_profile(self, system_id: str) -> None:
+    @delete("/v1/feature-profile/sdwan/other/{profile_id}")
+    def delete_sdwan_other_feature_profile(self, profile_id: UUID) -> None:
+        ...
+
+    @versions(supported_versions=(">=20.9"), raises=False)
+    @get("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}")
+    def get_all(self, profile_id: UUID, parcel_type: UUID) -> DataSequence[Parcel]:
+        ...
+
+    @versions(supported_versions=(">=20.9"), raises=False)
+    @get("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}/{parcel_id}")
+    def get_by_id(self, profile_id: UUID, parcel_type: str, parcel_id: UUID) -> Parcel:
+        ...
+
+    @versions(supported_versions=(">=20.9"), raises=False)
+    @put("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}/{parcel_id}")
+    def update(self, profile_id: UUID, parcel_type: str, parcel_id: UUID, payload: _ParcelBase) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
-    @post("/v1/feature-profile/sdwan/system/{system_id}/aaa")
-    def create_aaa_profile_parcel_for_system(self, system_id: str, payload: _ParcelBase) -> ParcelId:
+    @delete("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}/{parcel_id}")
+    def delete(self, profile_id: UUID, parcel_type: str, parcel_id: UUID) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
-    @put("/v1/feature-profile/sdwan/system/{system_id}/aaa/{parcel_id}")
-    def edit_aaa_profile_parcel_for_system(self, system_id: str, parcel_id: str, payload: _ParcelBase) -> ParcelId:
+    @post("/v1/feature-profile/sdwan/other/{profile_id}/{parcel_type}")
+    def create(self, profile_id: UUID, parcel_type: str, payload: _ParcelBase) -> ParcelId:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from typing import Optional
+from uuid import UUID
 
 from catalystwan.api.configuration_groups.parcel import _ParcelBase
 from catalystwan.endpoints import JSON, APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileDetail,
     FeatureProfileEditPayload,
     FeatureProfileInfo,
     GetFeatureProfilesPayload,
-    ParcelCreationResponse,
-    ParcelId,
     SchemaTypeQuery,
 )
-from catalystwan.models.configuration.feature_profile.sdwan.management.vpn import ManagementVPN
-from catalystwan.models.configuration.feature_profile.sdwan.transport.cellular_controller import CellularController
+from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse, ParcelId
+from catalystwan.models.configuration.feature_profile.sdwan.transport import (
+    AnyTransportParcel,
+    CellularControllerParcel,
+)
+from catalystwan.models.configuration.feature_profile.sdwan.transport.vpn import ManagementVpnParcel
 from catalystwan.typed_list import DataSequence
 
 
 class TransportFeatureProfile(APIEndpoints):
     @versions(supported_versions=(">=20.13"), raises=False)
     @post("/v1/feature-profile/sdwan/transport")
     def create_transport_feature_profile(
@@ -32,57 +35,90 @@
     @versions(supported_versions=(">=20.13"), raises=False)
     @get("/v1/feature-profile/sdwan/transport")
     def get_transport_feature_profiles(self, params: GetFeatureProfilesPayload) -> DataSequence[FeatureProfileInfo]:
         ...
 
     @versions(supported_versions=(">=20.13"), raises=False)
     @get("/v1/feature-profile/sdwan/transport/{profile_id}")
-    def get_transport_feature_profile(self, profile_id: str, params: GetFeatureProfilesPayload) -> FeatureProfileDetail:
+    def get_transport_feature_profile(
+        self, profile_id: UUID, params: GetFeatureProfilesPayload
+    ) -> FeatureProfileDetail:
         ...
 
     @versions(supported_versions=(">=20.13"), raises=False)
     @put("/v1/feature-profile/sdwan/transport/{profile_id}")
     def edit_transport_feature_profile(
-        self, profile_id: str, payload: FeatureProfileEditPayload
+        self, profile_id: UUID, payload: FeatureProfileEditPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
     @versions(supported_versions=(">=20.13"), raises=False)
     @delete("/v1/feature-profile/sdwan/transport/{profile_id}")
-    def delete_transport_feature_profile(self, profile_id: str) -> None:
+    def delete_transport_feature_profile(self, profile_id: UUID) -> None:
+        ...
+
+    @versions(supported_versions=(">=20.13"), raises=False)
+    @post("/v1/feature-profile/sdwan/transport/{profile_id}/{parcel_type}")
+    def create_transport_parcel(
+        self, profile_id: UUID, parcel_type: str, payload: _ParcelBase
+    ) -> ParcelCreationResponse:
+        ...
+
+    @versions(supported_versions=(">=20.13"), raises=False)
+    @post("/v1/feature-profile/sdwan/transport/{profile_id}/wan/vpn/{vpn_id}/{parcel_type}")
+    def create_transport_vpn_sub_parcel(
+        self, profile_id: UUID, vpn_id: UUID, parcel_type: str, payload: _ParcelBase
+    ) -> ParcelCreationResponse:
+        ...
+
+    @versions(supported_versions=(">=20.13"), raises=False)
+    @post("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn/{vpn_id}/{parcel_type}")
+    def create_management_vpn_sub_parcel(
+        self, profile_id: UUID, vpn_id: UUID, parcel_type: str, payload: _ParcelBase
+    ) -> ParcelCreationResponse:
+        ...
+
+    @versions(supported_versions=(">=20.13"), raises=False)
+    @get("/v1/feature-profile/sdwan/transport/{profile_id}/{parcel_type}")
+    def get_transport_parcels(self, profile_id: UUID, parcel_type: str) -> DataSequence[Parcel[AnyTransportParcel]]:
+        ...
+
+    @versions(supported_versions=(">=20.13"), raises=False)
+    @get("/v1/feature-profile/sdwan/transport/{profile_id}/{parcel_type}/{parcel_id}")
+    def get_transport_parcel(self, profile_id: UUID, parcel_type: str, parcel_id: UUID) -> Parcel[AnyTransportParcel]:
         ...
 
     #
     # ManagementVPN parcel
     #
     @versions(supported_versions=(">=20.13"), raises=False)
     @post("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn")
-    def create_management_vpn_parcel(self, profile_id: str, payload: _ParcelBase) -> ParcelCreationResponse:
+    def create_management_vpn_parcel(self, profile_id: UUID, payload: _ParcelBase) -> ParcelCreationResponse:
         ...
 
     # @versions(supported_versions=(">=20.13"), raises=False)
     # @get("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn")
-    # def get_management_vpn_parcels(self, profile_id: str) -> ParcelSequence[ManagementVPN]:
+    # def get_management_vpn_parcels(self, profile_id: UUID) -> ParcelSequence[ManagementVPN]:
     #     ...
 
     # @versions(supported_versions=(">=20.13"), raises=False)
     # @get("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn/{parcel_id}")
-    # def get_management_vpn_parcel(self, profile_id: str, parcel_id: str) -> Parcel[ManagementVPN]:
+    # def get_management_vpn_parcel(self, profile_id: UUID, parcel_id: str) -> Parcel[ManagementVPN]:
     #     ...
 
     @versions(supported_versions=(">=20.13"), raises=False)
     @put("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn/{parcel_id}")
     def edit_management_vpn_parcel(
-        self, profile_id: str, parcel_id: str, payload: ManagementVPN
+        self, profile_id: UUID, parcel_id: str, payload: ManagementVpnParcel
     ) -> ParcelCreationResponse:
         ...
 
     @versions(supported_versions=(">=20.13"), raises=False)
     @delete("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn/{parcel_id}")
-    def delete_management_vpn_parcel(self, profile_id: str, parcel_id: str) -> None:
+    def delete_management_vpn_parcel(self, profile_id: UUID, parcel_id: str) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @get("/v1/feature-profile/sdwan/transport")
     def get_sdwan_transport_feature_profiles(
         self, payload: Optional[GetFeatureProfilesPayload]
     ) -> DataSequence[FeatureProfileInfo]:
@@ -104,10 +140,10 @@
     @delete("/v1/feature-profile/sdwan/transport/{transport_id}")
     def delete_sdwan_transport_feature_profile(self, transport_id: str) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @post("/v1/feature-profile/sdwan/transport/{transport_id}/cellular-controller")
     def create_cellular_controller_profile_parcel_for_transport(
-        self, transport_id: str, payload: CellularController
+        self, transport_id: str, payload: CellularControllerParcel
     ) -> ParcelId:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/access_control_list.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/qos_map.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,53 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.access_control_list import AclPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.qos_map import QoSMapPolicy, QoSMapPolicyEditPayload, QoSMapPolicyGetResponse
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class AclPolicyEditPayload(AclPolicy, PolicyDefinitionId):
-    pass
-
-
-class AclPolicyGetResponse(AclPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyAclDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/acl")
-    def create_policy_definition(self, payload: AclPolicy) -> PolicyDefinitionId:
+class ConfigurationPolicyQoSMapDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/qosmap")
+    def create_policy_definition(self, payload: QoSMapPolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/acl/{id}")
+    @delete("/template/policy/definition/qosmap/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/acl/multiple/{id}
+        # PUT /template/policy/definition/qosmap/multiple/{id}
         ...
 
-    @put("/template/policy/definition/acl/{id}")
-    def edit_policy_definition(self, id: UUID, payload: AclPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/qosmap/{id}")
+    def edit_policy_definition(self, id: UUID, payload: QoSMapPolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/acl", "data")
+    @get("/template/policy/definition/qosmap", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/acl/{id}")
-    def get_policy_definition(self, id: UUID) -> AclPolicyGetResponse:
+    @get("/template/policy/definition/qosmap/{id}")
+    def get_policy_definition(self, id: UUID) -> QoSMapPolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/acl/preview")
-    def preview_policy_definition(self, payload: AclPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/qosmap/preview")
+    def preview_policy_definition(self, payload: QoSMapPolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/acl/preview/{id}")
+    @get("/template/policy/definition/qosmap/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/acl/bulk
+        # PUT /template/policy/definition/qosmap/bulk
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.access_control_list_ipv6 import AclIPv6Policy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.access_control_list_ipv6 import (
+    AclIPv6Policy,
+    AclIPv6PolicyEditPayload,
+    AclIPv6PolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class AclIPv6PolicyEditPayload(AclIPv6Policy, PolicyDefinitionId):
-    pass
-
-
-class AclIPv6PolicyGetResponse(AclIPv6Policy, PolicyDefinitionGetResponse):
-    pass
-
-
 class ConfigurationPolicyAclIPv6Definition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/aclv6")
     def create_policy_definition(self, payload: AclIPv6Policy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/aclv6/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/control.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/access_control_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.control import ControlPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.access_control_list import (
+    AclPolicy,
+    AclPolicyEditPayload,
+    AclPolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class ControlPolicyEditPayload(ControlPolicy, PolicyDefinitionId):
-    pass
-
-
-class ControlPolicyGetResponse(ControlPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyControlDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/control")
-    def create_policy_definition(self, payload: ControlPolicy) -> PolicyDefinitionId:
+class ConfigurationPolicyAclDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/acl")
+    def create_policy_definition(self, payload: AclPolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/control/{id}")
+    @delete("/template/policy/definition/acl/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/control/multiple/{id}
+        # PUT /template/policy/definition/acl/multiple/{id}
         ...
 
-    @put("/template/policy/definition/control/{id}")
-    def edit_policy_definition(self, id: UUID, payload: ControlPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/acl/{id}")
+    def edit_policy_definition(self, id: UUID, payload: AclPolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/control", "data")
+    @get("/template/policy/definition/acl", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/control/{id}")
-    def get_policy_definition(self, id: UUID) -> ControlPolicyGetResponse:
+    @get("/template/policy/definition/acl/{id}")
+    def get_policy_definition(self, id: UUID) -> AclPolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/control/preview")
-    def preview_policy_definition(self, payload: ControlPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/acl/preview")
+    def preview_policy_definition(self, payload: AclPolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/control/preview/{id}")
+    @get("/template/policy/definition/acl/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/control/bulk
+        # PUT /template/policy/definition/acl/bulk
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/device_access.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/device_access.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.device_access import DeviceAccessPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.device_access import (
+    DeviceAccessPolicy,
+    DeviceAccessPolicyEditPayload,
+    DeviceAccessPolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class DeviceAccessPolicyEditPayload(DeviceAccessPolicy, PolicyDefinitionId):
-    pass
-
-
-class DeviceAccessPolicyGetResponse(DeviceAccessPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
 class ConfigurationPolicyDeviceAccessDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/deviceaccesspolicy")
     def create_policy_definition(self, payload: DeviceAccessPolicy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/deviceaccesspolicy/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/rewrite.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,57 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.device_access_ipv6 import DeviceAccessIPv6Policy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.rewrite import (
+    RewritePolicy,
+    RewritePolicyEditPayload,
+    RewritePolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class DeviceAccessIPv6PolicyEditPayload(DeviceAccessIPv6Policy, PolicyDefinitionId):
-    pass
-
-
-class DeviceAccessIPv6PolicyGetResponse(DeviceAccessIPv6Policy, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyDeviceAccessIPv6Definition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/deviceaccesspolicyv6")
-    def create_policy_definition(self, payload: DeviceAccessIPv6Policy) -> PolicyDefinitionId:
+class ConfigurationPolicyRewriteRuleDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/rewriterule")
+    def create_policy_definition(self, payload: RewritePolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/deviceaccesspolicyv6/{id}")
+    @delete("/template/policy/definition/rewriterule/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/deviceaccesspolicyv6/multiple/{id}
+        # PUT /template/policy/definition/rewriterule/multiple/{id}
         ...
 
-    @put("/template/policy/definition/deviceaccesspolicyv6/{id}")
-    def edit_policy_definition(
-        self, id: UUID, payload: DeviceAccessIPv6PolicyEditPayload
-    ) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/rewriterule/{id}")
+    def edit_policy_definition(self, id: UUID, payload: RewritePolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/deviceaccesspolicyv6", "data")
+    @get("/template/policy/definition/rewriterule", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/deviceaccesspolicyv6/{id}")
-    def get_policy_definition(self, id: UUID) -> DeviceAccessIPv6PolicyGetResponse:
+    @get("/template/policy/definition/rewriterule/{id}")
+    def get_policy_definition(self, id: UUID) -> RewritePolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/deviceaccesspolicyv6/preview")
-    def preview_policy_definition(self, payload: DeviceAccessIPv6Policy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/rewriterule/preview")
+    def preview_policy_definition(self, payload: RewritePolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/deviceaccesspolicyv6/preview/{id}")
+    @get("/template/policy/definition/rewriterule/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/deviceaccesspolicyv6/bulk
+        # PUT /template/policy/definition/rewriterule/bulk
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.hub_and_spoke import HubAndSpokePolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.hub_and_spoke import (
+    HubAndSpokePolicy,
+    HubAndSpokePolicyEditPayload,
+    HubAndSpokePolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class HubAndSpokePolicyEditPayload(HubAndSpokePolicy, PolicyDefinitionId):
-    pass
-
-
-class HubAndSpokePolicyGetResponse(HubAndSpokePolicy, PolicyDefinitionGetResponse):
-    pass
-
-
 class ConfigurationPolicyHubAndSpokeDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/hubandspoke")
     def create_policy_definition(self, payload: HubAndSpokePolicy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/hubandspoke/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/mesh.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/mesh.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.mesh import MeshPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.mesh import MeshPolicy, MeshPolicyEditPayload, MeshPolicyGetResponse
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class MeshPolicyEditPayload(MeshPolicy, PolicyDefinitionId):
-    pass
-
-
-class MeshPolicyGetResponse(MeshPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
 class ConfigurationPolicyMeshDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/mesh")
     def create_policy_definition(self, payload: MeshPolicy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/mesh/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/qos_map.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.qos_map import QoSMapPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.zone_based_firewall import (
+    ZoneBasedFWPolicy,
+    ZoneBasedFWPolicyEditPayload,
+    ZoneBasedFWPolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class QoSMapPolicyEditPayload(QoSMapPolicy, PolicyDefinitionId):
-    pass
-
-
-class QoSMapPolicyGetResponse(QoSMapPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyQoSMapDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/qosmap")
-    def create_policy_definition(self, payload: QoSMapPolicy) -> PolicyDefinitionId:
+class ConfigurationPolicyZoneBasedFirewallDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/zonebasedfw")
+    def create_policy_definition(self, payload: ZoneBasedFWPolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/qosmap/{id}")
+    @delete("/template/policy/definition/zonebasedfw/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/qosmap/multiple/{id}
+        # PUT /template/policy/definition/zonebasedfw/multiple/{id}
         ...
 
-    @put("/template/policy/definition/qosmap/{id}")
-    def edit_policy_definition(self, id: UUID, payload: QoSMapPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/zonebasedfw/{id}")
+    def edit_policy_definition(self, id: UUID, payload: ZoneBasedFWPolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/qosmap", "data")
+    @get("/template/policy/definition/zonebasedfw", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/qosmap/{id}")
-    def get_policy_definition(self, id: UUID) -> QoSMapPolicyGetResponse:
+    @get("/template/policy/definition/zonebasedfw/{id}")
+    def get_policy_definition(self, id: UUID) -> ZoneBasedFWPolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/qosmap/preview")
-    def preview_policy_definition(self, payload: QoSMapPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/zonebasedfw/preview")
+    def preview_policy_definition(self, payload: ZoneBasedFWPolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/qosmap/preview/{id}")
+    @get("/template/policy/definition/zonebasedfw/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/qosmap/bulk
+        # PUT /template/policy/definition/zonebasedfw/bulk
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/rule_set.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,59 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.rule_set import RuleSet
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.device_access_ipv6 import (
+    DeviceAccessIPv6Policy,
+    DeviceAccessIPv6PolicyEditPayload,
+    DeviceAccessIPv6PolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class RuleSetEditPayload(RuleSet, PolicyDefinitionId):
-    pass
-
-
-class RuleSetGetResponse(RuleSet, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyRuleSetDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/ruleset")
-    def create_policy_definition(self, payload: RuleSet) -> PolicyDefinitionId:
+class ConfigurationPolicyDeviceAccessIPv6Definition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/deviceaccesspolicyv6")
+    def create_policy_definition(self, payload: DeviceAccessIPv6Policy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/ruleset/{id}")
+    @delete("/template/policy/definition/deviceaccesspolicyv6/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/ruleset/multiple/{id}
+        # PUT /template/policy/definition/deviceaccesspolicyv6/multiple/{id}
         ...
 
-    @put("/template/policy/definition/ruleset/{id}")
-    def edit_policy_definition(self, id: UUID, payload: RuleSetEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/deviceaccesspolicyv6/{id}")
+    def edit_policy_definition(
+        self, id: UUID, payload: DeviceAccessIPv6PolicyEditPayload
+    ) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/ruleset", "data")
+    @get("/template/policy/definition/deviceaccesspolicyv6", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/ruleset/{id}")
-    def get_policy_definition(self, id: UUID) -> RuleSetGetResponse:
+    @get("/template/policy/definition/deviceaccesspolicyv6/{id}")
+    def get_policy_definition(self, id: UUID) -> DeviceAccessIPv6PolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/ruleset/preview")
-    def preview_policy_definition(self, payload: RuleSet) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/deviceaccesspolicyv6/preview")
+    def preview_policy_definition(self, payload: DeviceAccessIPv6Policy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/ruleset/preview/{id}")
+    @get("/template/policy/definition/deviceaccesspolicyv6/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/ruleset/bulk
+        # PUT /template/policy/definition/deviceaccesspolicyv6/bulk
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/security_group.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/security_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.security_group import SecurityGroup
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.security_group import (
+    SecurityGroup,
+    SecurityGroupEditPayload,
+    SecurityGroupGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class SecurityGroupEditPayload(SecurityGroup, PolicyDefinitionId):
-    pass
-
-
-class SecurityGroupGetResponse(SecurityGroup, PolicyDefinitionGetResponse):
-    pass
-
-
 class ConfigurationPolicySecurityGroupDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/securitygroup")
     def create_policy_definition(self, payload: SecurityGroup) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/securitygroup/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/traffic_data.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/traffic_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.traffic_data import TrafficDataPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.traffic_data import (
+    TrafficDataPolicy,
+    TrafficDataPolicyEditPayload,
+    TrafficDataPolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class TrafficDataPolicyEditPayload(TrafficDataPolicy, PolicyDefinitionId):
-    pass
-
-
-class TrafficDataPolicyGetResponse(TrafficDataPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
 class ConfigurationPolicyDataDefinition(APIEndpoints, PolicyDefinitionEndpoints):
     @post("/template/policy/definition/data")
     def create_policy_definition(self, payload: TrafficDataPolicy) -> PolicyDefinitionId:
         ...
 
     @delete("/template/policy/definition/data/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/rule_set.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,53 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.vpn_membership import VPNMembershipPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.rule_set import RuleSet, RuleSetEditPayload, RuleSetGetResponse
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class VPNMembershipPolicyEditPayload(VPNMembershipPolicy, PolicyDefinitionId):
-    pass
-
-
-class VPNMembershipPolicyGetResponse(VPNMembershipPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyVPNMembershipGroupDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/vpnmembershipgroup")
-    def create_policy_definition(self, payload: VPNMembershipPolicy) -> PolicyDefinitionId:
+class ConfigurationPolicyRuleSetDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/ruleset")
+    def create_policy_definition(self, payload: RuleSet) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/vpnmembershipgroup/{id}")
+    @delete("/template/policy/definition/ruleset/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
     def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/vpnmembershipgroup/multiple/{id}
+        # PUT /template/policy/definition/ruleset/multiple/{id}
         ...
 
-    @put("/template/policy/definition/vpnmembershipgroup/{id}")
-    def edit_policy_definition(self, id: UUID, payload: VPNMembershipPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/ruleset/{id}")
+    def edit_policy_definition(self, id: UUID, payload: RuleSetEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/vpnmembershipgroup", "data")
+    @get("/template/policy/definition/ruleset", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/vpnmembershipgroup/{id}")
-    def get_policy_definition(self, id: UUID) -> VPNMembershipPolicyGetResponse:
+    @get("/template/policy/definition/ruleset/{id}")
+    def get_policy_definition(self, id: UUID) -> RuleSetGetResponse:
         ...
 
-    @post("/template/policy/definition/vpnmembershipgroup/preview")
-    def preview_policy_definition(self, payload: VPNMembershipPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/ruleset/preview")
+    def preview_policy_definition(self, payload: RuleSet) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/vpnmembershipgroup/preview/{id}")
+    @get("/template/policy/definition/ruleset/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
 
     def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/vpnmembershipgroup/bulk
+        # PUT /template/policy/definition/ruleset/bulk
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/definition/dns_security.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,50 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
+
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.definitions.zone_based_firewall import ZoneBasedFWPolicy
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyDefinitionEndpoints
+from catalystwan.models.policy.definition.dns_security import (
+    DnsSecurityPolicy,
+    DnsSecurityPolicyEditPayload,
+    DnsSecurityPolicyGetResponse,
+)
 from catalystwan.models.policy.policy_definition import (
     PolicyDefinitionEditResponse,
-    PolicyDefinitionEndpoints,
-    PolicyDefinitionGetResponse,
     PolicyDefinitionId,
     PolicyDefinitionInfo,
     PolicyDefinitionPreview,
 )
 from catalystwan.typed_list import DataSequence
 
 
-class ZoneBasedFWPolicyEditPayload(ZoneBasedFWPolicy, PolicyDefinitionId):
-    pass
-
-
-class ZoneBasedFWPolicyGetResponse(ZoneBasedFWPolicy, PolicyDefinitionGetResponse):
-    pass
-
-
-class ConfigurationPolicyZoneBasedFirewallDefinition(APIEndpoints, PolicyDefinitionEndpoints):
-    @post("/template/policy/definition/zonebasedfw")
-    def create_policy_definition(self, payload: ZoneBasedFWPolicy) -> PolicyDefinitionId:
+class ConfigurationPolicyDnsSecurityDefinition(APIEndpoints, PolicyDefinitionEndpoints):
+    @post("/template/policy/definition/dnssecurity")
+    def create_policy_definition(self, payload: DnsSecurityPolicy) -> PolicyDefinitionId:
         ...
 
-    @delete("/template/policy/definition/zonebasedfw/{id}")
+    @delete("/template/policy/definition/dnssecurity/{id}")
     def delete_policy_definition(self, id: UUID) -> None:
         ...
 
-    def edit_multiple_policy_definition(self):
-        # PUT /template/policy/definition/zonebasedfw/multiple/{id}
-        ...
-
-    @put("/template/policy/definition/zonebasedfw/{id}")
-    def edit_policy_definition(self, id: UUID, payload: ZoneBasedFWPolicyEditPayload) -> PolicyDefinitionEditResponse:
+    @put("/template/policy/definition/dnssecurity/{id}")
+    def edit_policy_definition(self, id: UUID, payload: DnsSecurityPolicyEditPayload) -> PolicyDefinitionEditResponse:
         ...
 
-    @get("/template/policy/definition/zonebasedfw", "data")
+    @get("/template/policy/definition/dnssecurity", "data")
     def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
         ...
 
-    @get("/template/policy/definition/zonebasedfw/{id}")
-    def get_policy_definition(self, id: UUID) -> ZoneBasedFWPolicyGetResponse:
+    @get("/template/policy/definition/dnssecurity/{id}")
+    def get_policy_definition(self, id: UUID) -> DnsSecurityPolicyGetResponse:
         ...
 
-    @post("/template/policy/definition/zonebasedfw/preview")
-    def preview_policy_definition(self, payload: ZoneBasedFWPolicy) -> PolicyDefinitionPreview:
+    @post("/template/policy/definition/dnssecurity/preview")
+    def preview_policy_definition(self, payload: DnsSecurityPolicy) -> PolicyDefinitionPreview:
         ...
 
-    @get("/template/policy/definition/zonebasedfw/preview/{id}")
+    @get("/template/policy/definition/dnssecurity/preview/{id}")
     def preview_policy_definition_by_id(self, id: UUID) -> PolicyDefinitionPreview:
         ...
-
-    def save_policy_definition_in_bulk(self):
-        # PUT /template/policy/definition/zonebasedfw/bulk
-        ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/app.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/port.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import AppList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.port import PortList, PortListEditPayload, PortListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class AppListEditPayload(AppList, PolicyListId):
-    pass
-
-
-class AppListInfo(AppList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyApplicationList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/app")
-    def create_policy_list(self, payload: AppList) -> PolicyListId:
+class ConfigurationPolicyPortList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/port")
+    def create_policy_list(self, payload: PortList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/app/{id}")
+    @delete("/template/policy/list/port/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/app")
+    @delete("/template/policy/list/port")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/app/{id}")
-    def edit_policy_list(self, id: UUID, payload: AppListEditPayload) -> None:
+    @put("/template/policy/list/port/{id}")
+    def edit_policy_list(self, id: UUID, payload: PortListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/app/{id}")
-    def get_lists_by_id(self, id: UUID) -> AppListInfo:
+    @get("/template/policy/list/port/{id}")
+    def get_lists_by_id(self, id: UUID) -> PortListInfo:
         ...
 
-    @get("/template/policy/list/app", "data")
-    def get_policy_lists(self) -> DataSequence[AppListInfo]:
+    @get("/template/policy/list/port", "data")
+    def get_policy_lists(self) -> DataSequence[PortListInfo]:
         ...
 
-    @get("/template/policy/list/app/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[AppListInfo]:
+    @get("/template/policy/list/port/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[PortListInfo]:
         ...
 
-    @post("/template/policy/list/app/preview")
-    def preview_policy_list(self, payload: AppList) -> PolicyListPreview:
+    @post("/template/policy/list/port/preview")
+    def preview_policy_list(self, payload: PortList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/app/preview/{id}")
+    @get("/template/policy/list/port/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/app_probe.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/app_probe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import AppProbeClassList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.app_probe import (
+    AppProbeClassList,
+    AppProbeClassListEditPayload,
+    AppProbeClassListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class AppProbeClassListEditPayload(AppProbeClassList, PolicyListId):
-    pass
-
-
-class AppProbeClassListInfo(AppProbeClassList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyAppProbeClassList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/appprobe")
     def create_policy_list(self, payload: AppProbeClassList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/appprobe/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/as_path.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/as_path.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import ASPathList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.as_path import ASPathList, ASPathListEditPayload, ASPathListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class ASPathListEditPayload(ASPathList, PolicyListId):
-    pass
-
-
-class ASPathListInfo(ASPathList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyASPathList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/aspath")
     def create_policy_list(self, payload: ASPathList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/aspath/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/class_map.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/site.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,52 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import ClassMapList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.site import SiteList, SiteListEditPayload, SiteListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class ClassMapListEditPayload(ClassMapList, PolicyListId):
-    pass
-
-
-class ClassMapListInfo(ClassMapList, PolicyListInfo):
-    pass
-
+class ConfigurationPolicySiteList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/site/defaultsite")
+    def create_default_site_list(self, payload: SiteList) -> PolicyListId:
+        ...
 
-class ConfigurationPolicyForwardingClassList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/class")
-    def create_policy_list(self, payload: ClassMapList) -> PolicyListId:
+    @post("/template/policy/list/site")
+    def create_policy_list(self, payload: SiteList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/class/{id}")
+    @delete("/template/policy/list/site/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/class")
+    @delete("/template/policy/list/site")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/class/{id}")
-    def edit_policy_list(self, id: UUID, payload: ClassMapListEditPayload) -> None:
+    @put("/template/policy/list/site/{id}")
+    def edit_policy_list(self, id: UUID, payload: SiteListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/class/{id}")
-    def get_lists_by_id(self, id: UUID) -> ClassMapListInfo:
+    @get("/template/policy/list/site/{id}")
+    def get_lists_by_id(self, id: UUID) -> SiteListInfo:
         ...
 
-    @get("/template/policy/list/class", "data")
-    def get_policy_lists(self) -> DataSequence[ClassMapListInfo]:
+    @get("/template/policy/list/site", "data")
+    def get_policy_lists(self) -> DataSequence[SiteListInfo]:
         ...
 
-    @get("/template/policy/list/class/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[ClassMapListInfo]:
+    @get("/template/policy/list/site/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[SiteListInfo]:
         ...
 
-    @post("/template/policy/list/class/preview")
-    def preview_policy_list(self, payload: ClassMapList) -> PolicyListPreview:
+    @post("/template/policy/list/site/preview")
+    def preview_policy_list(self, payload: SiteList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/class/preview/{id}")
+    @get("/template/policy/list/site/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/color.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/color.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import ColorList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.color import ColorList, ColorListEditPayload, ColorListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class ColorListEditPayload(ColorList, PolicyListId):
-    pass
-
-
-class ColorListInfo(ColorList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyColorList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/color")
     def create_policy_list(self, payload: ColorList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/color/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/community.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/community.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import CommunityList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.communities import CommunityList, CommunityListEditPayload, CommunityListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class CommunityListEditPayload(CommunityList, PolicyListId):
-    pass
-
-
-class CommunityListInfo(CommunityList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyCommunityList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/community")
     def create_policy_list(self, payload: CommunityList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/community/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import DataIPv6PrefixList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.data_ipv6_prefix import (
+    DataIPv6PrefixList,
+    DataIPv6PrefixListEditPayload,
+    DataIPv6PrefixListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class DataIPv6PrefixListEditPayload(DataIPv6PrefixList, PolicyListId):
-    pass
-
-
-class DataIPv6PrefixListInfo(DataIPv6PrefixList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyDataIPv6PrefixList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/dataipv6prefix")
     def create_policy_list(self, payload: DataIPv6PrefixList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/dataipv6prefix/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/data_prefix.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/data_prefix.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import DataPrefixList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.data_prefix import DataPrefixList, DataPrefixListEditPayload, DataPrefixListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class DataPrefixListEditPayload(DataPrefixList, PolicyListId):
-    pass
-
-
-class DataPrefixListInfo(DataPrefixList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyDataPrefixList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/dataprefix")
     def create_policy_list(self, payload: DataPrefixList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/dataprefix/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/expanded_community.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/expanded_community.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import ExpandedCommunityList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.communities import (
+    ExpandedCommunityList,
+    ExpandedCommunityListEditPayload,
+    ExpandedCommunityListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class ExpandedCommunityListEditPayload(ExpandedCommunityList, PolicyListId):
-    pass
-
-
-class ExpandedCommunityListInfo(ExpandedCommunityList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyExpandedCommunityList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/expandedcommunity")
     def create_policy_list(self, payload: ExpandedCommunityList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/expandedcommunity/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/fqdn.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/fqdn.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import FQDNList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.fqdn import FQDNList, FQDNListEditPayload, FQDNListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class FQDNListEditPayload(FQDNList, PolicyListId):
-    pass
-
-
-class FQDNListInfo(FQDNList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyFQDNList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/fqdn")
     def create_policy_list(self, payload: FQDNList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/fqdn/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/geo_location.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/url_block_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import GeoLocationList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.url import URLBlockList, URLBlockListEditPayload, URLBlockListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class GeoLocationListEditPayload(GeoLocationList, PolicyListId):
-    pass
-
-
-class GeoLocationListInfo(GeoLocationList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyGeoLocationList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/geolocation")
-    def create_policy_list(self, payload: GeoLocationList) -> PolicyListId:
+class ConfigurationPolicyURLBlockList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/urlblacklist")
+    def create_policy_list(self, payload: URLBlockList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/geolocation/{id}")
+    @delete("/template/policy/list/urlblacklist/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/geolocation")
+    @delete("/template/policy/list/urlblacklist")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/geolocation/{id}")
-    def edit_policy_list(self, id: UUID, payload: GeoLocationListEditPayload) -> None:
+    @put("/template/policy/list/urlblacklist/{id}")
+    def edit_policy_list(self, id: UUID, payload: URLBlockListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/geolocation/{id}")
-    def get_lists_by_id(self, id: UUID) -> GeoLocationListInfo:
+    @get("/template/policy/list/urlblacklist/{id}")
+    def get_lists_by_id(self, id: UUID) -> URLBlockListInfo:
         ...
 
-    @get("/template/policy/list/geolocation", "data")
-    def get_policy_lists(self) -> DataSequence[GeoLocationListInfo]:
+    @get("/template/policy/list/urlblacklist", "data")
+    def get_policy_lists(self) -> DataSequence[URLBlockListInfo]:
         ...
 
-    @get("/template/policy/list/geolocation/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[GeoLocationListInfo]:
+    @get("/template/policy/list/urlblacklist/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[URLBlockListInfo]:
         ...
 
-    @post("/template/policy/list/geolocation/preview")
-    def preview_policy_list(self, payload: GeoLocationList) -> PolicyListPreview:
+    @post("/template/policy/list/urlblacklist/preview")
+    def preview_policy_list(self, payload: URLBlockList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/geolocation/preview/{id}")
+    @get("/template/policy/list/urlblacklist/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/ips_signature.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/ips_signature.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import IPSSignatureList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.ips_signature import (
+    IPSSignatureList,
+    IPSSignatureListEditPayload,
+    IPSSignatureListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class IPSSignatureListEditPayload(IPSSignatureList, PolicyListId):
-    pass
-
-
-class IPSSignatureListInfo(IPSSignatureList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyIPSSignatureList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/ipssignature")
     def create_policy_list(self, payload: IPSSignatureList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/ipssignature/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/zone.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import IPv6PrefixList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.zone import ZoneList, ZoneListEditPayload, ZoneListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class IPv6PrefixListEditPayload(IPv6PrefixList, PolicyListId):
-    pass
-
-
-class IPv6PrefixListInfo(IPv6PrefixList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyIPv6PrefixList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/ipv6prefix")
-    def create_policy_list(self, payload: IPv6PrefixList) -> PolicyListId:
+class ConfigurationPolicyZoneList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/zone")
+    def create_policy_list(self, payload: ZoneList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/ipv6prefix/{id}")
+    @delete("/template/policy/list/zone/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/ipv6prefix")
+    @delete("/template/policy/list/zone")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/ipv6prefix/{id}")
-    def edit_policy_list(self, id: UUID, payload: IPv6PrefixListEditPayload) -> None:
+    @put("/template/policy/list/zone/{id}")
+    def edit_policy_list(self, id: UUID, payload: ZoneListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/ipv6prefix/{id}")
-    def get_lists_by_id(self, id: UUID) -> IPv6PrefixListInfo:
+    @get("/template/policy/list/zone/{id}")
+    def get_lists_by_id(self, id: UUID) -> ZoneListInfo:
         ...
 
-    @get("/template/policy/list/ipv6prefix", "data")
-    def get_policy_lists(self) -> DataSequence[IPv6PrefixListInfo]:
+    @get("/template/policy/list/zone", "data")
+    def get_policy_lists(self) -> DataSequence[ZoneListInfo]:
         ...
 
-    @get("/template/policy/list/ipv6prefix/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[IPv6PrefixListInfo]:
+    @get("/template/policy/list/zone/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[ZoneListInfo]:
         ...
 
-    @post("/template/policy/list/ipv6prefix/preview")
-    def preview_policy_list(self, payload: IPv6PrefixList) -> PolicyListPreview:
+    @post("/template/policy/list/zone/preview")
+    def preview_policy_list(self, payload: ZoneList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/ipv6prefix/preview/{id}")
+    @get("/template/policy/list/zone/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/local_app.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/local_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import LocalAppList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.local_app import LocalAppList, LocalAppListEditPayload, LocalAppListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class LocalAppListEditPayload(LocalAppList, PolicyListId):
-    pass
-
-
-class LocalAppListInfo(LocalAppList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyLocalAppList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/localapp")
     def create_policy_list(self, payload: LocalAppList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/localapp/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/local_domain.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/local_domain.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import LocalDomainList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.local_domain import LocalDomainList, LocalDomainListEditPayload, LocalDomainListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class LocalDomainListEditPayload(LocalDomainList, PolicyListId):
-    pass
-
-
-class LocalDomainListInfo(LocalDomainList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyLocalDomainList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/localdomain")
     def create_policy_list(self, payload: LocalDomainList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/localdomain/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/mirror.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/mirror.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import MirrorList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.mirror import MirrorList, MirrorListEditPayload, MirrorListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class MirrorListEditPayload(MirrorList, PolicyListId):
-    pass
-
-
-class MirrorListInfo(MirrorList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyMirrorList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/mirror")
     def create_policy_list(self, payload: MirrorList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/mirror/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/policer.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/policer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import PolicerList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.policer import PolicerList, PolicerListEditPayload, PolicerListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class PolicerListEditPayload(PolicerList, PolicyListId):
-    pass
-
-
-class PolicerListInfo(PolicerList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyPolicerClassList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/policer")
     def create_policy_list(self, payload: PolicerList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/policer/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/port.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/tloc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import PortList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.tloc import TLOCList, TLOCListEditPayload, TLOCListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class PortListEditPayload(PortList, PolicyListId):
-    pass
-
-
-class PortListInfo(PortList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyPortList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/port")
-    def create_policy_list(self, payload: PortList) -> PolicyListId:
+class ConfigurationPolicyTLOCList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/tloc")
+    def create_policy_list(self, payload: TLOCList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/port/{id}")
+    @delete("/template/policy/list/tloc/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/port")
+    @delete("/template/policy/list/tloc")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/port/{id}")
-    def edit_policy_list(self, id: UUID, payload: PortListEditPayload) -> None:
+    @put("/template/policy/list/tloc/{id}")
+    def edit_policy_list(self, id: UUID, payload: TLOCListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/port/{id}")
-    def get_lists_by_id(self, id: UUID) -> PortListInfo:
+    @get("/template/policy/list/tloc/{id}")
+    def get_lists_by_id(self, id: UUID) -> TLOCListInfo:
         ...
 
-    @get("/template/policy/list/port", "data")
-    def get_policy_lists(self) -> DataSequence[PortListInfo]:
+    @get("/template/policy/list/tloc", "data")
+    def get_policy_lists(self) -> DataSequence[TLOCListInfo]:
         ...
 
-    @get("/template/policy/list/port/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[PortListInfo]:
+    @get("/template/policy/list/tloc/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[TLOCListInfo]:
         ...
 
-    @post("/template/policy/list/port/preview")
-    def preview_policy_list(self, payload: PortList) -> PolicyListPreview:
+    @post("/template/policy/list/tloc/preview")
+    def preview_policy_list(self, payload: TLOCList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/port/preview/{id}")
+    @get("/template/policy/list/tloc/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import PreferredColorGroupList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.preferred_color_group import (
+    PreferredColorGroupList,
+    PreferredColorGroupListEditPayload,
+    PreferredColorGroupListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class PreferredColorGroupListEditPayload(PreferredColorGroupList, PolicyListId):
-    pass
-
-
-class PreferredColorGroupListInfo(PreferredColorGroupList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPreferredColorGroupList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/preferredcolorgroup")
     def create_policy_list(self, payload: PreferredColorGroupList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/preferredcolorgroup/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/prefix.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/prefix.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,20 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
+from catalystwan.api.templates.models.cisco_vpn_model import PrefixList
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import PrefixList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.prefix import PrefixListEditPayload, PrefixListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class PrefixListEditPayload(PrefixList, PolicyListId):
-    pass
-
-
-class PrefixListInfo(PrefixList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyPrefixList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/prefix")
     def create_policy_list(self, payload: PrefixList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/prefix/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/protocol_name.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/protocol_name.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import ProtocolNameList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.protocol_name import (
+    ProtocolNameList,
+    ProtocolNameListEditPayload,
+    ProtocolNameListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class ProtocolNameListEditPayload(ProtocolNameList, PolicyListId):
-    pass
-
-
-class ProtocolNameListInfo(ProtocolNameList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyProtocolNameList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/protocolname")
     def create_policy_list(self, payload: ProtocolNameList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/protocolname/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/region.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/region.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import RegionList
-from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListInfo, PolicyListPreview
+from catalystwan.models.policy.list.region import RegionList, RegionListEditPayload, RegionListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class RegionListEditPayload(RegionList, PolicyListId):
-    pass
-
-
-class RegionListInfo(RegionList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyRegionList(APIEndpoints):
     @post("/template/policy/list/region")
     def create_policy_list(self, payload: RegionList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/region/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/site.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/sla.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import SiteList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.sla import SLAClassList, SLAClassListEditPayload, SLAClassListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class SiteListEditPayload(SiteList, PolicyListId):
-    pass
-
-
-class SiteListInfo(SiteList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicySiteList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/site/defaultsite")
-    def create_default_site_list(self, payload: SiteList) -> PolicyListId:
-        ...
-
-    @post("/template/policy/list/site")
-    def create_policy_list(self, payload: SiteList) -> PolicyListId:
+class ConfigurationPolicySLAClassList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/sla")
+    def create_policy_list(self, payload: SLAClassList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/site/{id}")
+    @delete("/template/policy/list/sla/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/site")
+    @delete("/template/policy/list/sla")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/site/{id}")
-    def edit_policy_list(self, id: UUID, payload: SiteListEditPayload) -> None:
+    @put("/template/policy/list/sla/{id}")
+    def edit_policy_list(self, id: UUID, payload: SLAClassListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/site/{id}")
-    def get_lists_by_id(self, id: UUID) -> SiteListInfo:
+    @get("/template/policy/list/sla/{id}")
+    def get_lists_by_id(self, id: UUID) -> SLAClassListInfo:
         ...
 
-    @get("/template/policy/list/site", "data")
-    def get_policy_lists(self) -> DataSequence[SiteListInfo]:
+    @get("/template/policy/list/sla", "data")
+    def get_policy_lists(self) -> DataSequence[SLAClassListInfo]:
         ...
 
-    @get("/template/policy/list/site/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[SiteListInfo]:
+    @get("/template/policy/list/sla/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[SLAClassListInfo]:
         ...
 
-    @post("/template/policy/list/site/preview")
-    def preview_policy_list(self, payload: SiteList) -> PolicyListPreview:
+    @post("/template/policy/list/sla/preview")
+    def preview_policy_list(self, payload: SLAClassList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/site/preview/{id}")
+    @get("/template/policy/list/sla/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/sla.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/trunkgroup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,48 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import SLAClassList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.trunkgroup import TrunkGroupList, TrunkGroupListEditPayload, TrunkGroupListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class SLAClassListEditPayload(SLAClassList, PolicyListId):
-    pass
-
-
-class SLAClassListInfo(SLAClassList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicySLAClassList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/sla")
-    def create_policy_list(self, payload: SLAClassList) -> PolicyListId:
+class ConfigurationPolicyTrunkGroupList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/trunkgroup")
+    def create_policy_list(self, payload: TrunkGroupList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/sla/{id}")
+    @delete("/template/policy/list/trunkgroup/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/sla")
+    @delete("/template/policy/list/trunkgroup")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/sla/{id}")
-    def edit_policy_list(self, id: UUID, payload: SLAClassListEditPayload) -> None:
+    @put("/template/policy/list/trunkgroup/{id}")
+    def edit_policy_list(self, id: UUID, payload: TrunkGroupListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/sla/{id}")
-    def get_lists_by_id(self, id: UUID) -> SLAClassListInfo:
+    @get("/template/policy/list/trunkgroup/{id}")
+    def get_lists_by_id(self, id: UUID) -> TrunkGroupListInfo:
         ...
 
-    @get("/template/policy/list/sla", "data")
-    def get_policy_lists(self) -> DataSequence[SLAClassListInfo]:
+    @get("/template/policy/list/trunkgroup", "data")
+    def get_policy_lists(self) -> DataSequence[TrunkGroupListInfo]:
         ...
 
-    @get("/template/policy/list/sla/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[SLAClassListInfo]:
+    @get("/template/policy/list/trunkgroup/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[TrunkGroupListInfo]:
         ...
 
-    @post("/template/policy/list/sla/preview")
-    def preview_policy_list(self, payload: SLAClassList) -> PolicyListPreview:
+    @post("/template/policy/list/trunkgroup/preview")
+    def preview_policy_list(self, payload: TrunkGroupList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/sla/preview/{id}")
+    @get("/template/policy/list/trunkgroup/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/tloc.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import TLOCList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.ipv6_prefix import IPv6PrefixList, IPv6PrefixListEditPayload, IPv6PrefixListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class TLOCListEditPayload(TLOCList, PolicyListId):
-    pass
-
-
-class TLOCListInfo(TLOCList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyTLOCList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/tloc")
-    def create_policy_list(self, payload: TLOCList) -> PolicyListId:
+class ConfigurationPolicyIPv6PrefixList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/ipv6prefix")
+    def create_policy_list(self, payload: IPv6PrefixList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/tloc/{id}")
+    @delete("/template/policy/list/ipv6prefix/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/tloc")
+    @delete("/template/policy/list/ipv6prefix")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/tloc/{id}")
-    def edit_policy_list(self, id: UUID, payload: TLOCListEditPayload) -> None:
+    @put("/template/policy/list/ipv6prefix/{id}")
+    def edit_policy_list(self, id: UUID, payload: IPv6PrefixListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/tloc/{id}")
-    def get_lists_by_id(self, id: UUID) -> TLOCListInfo:
+    @get("/template/policy/list/ipv6prefix/{id}")
+    def get_lists_by_id(self, id: UUID) -> IPv6PrefixListInfo:
         ...
 
-    @get("/template/policy/list/tloc", "data")
-    def get_policy_lists(self) -> DataSequence[TLOCListInfo]:
+    @get("/template/policy/list/ipv6prefix", "data")
+    def get_policy_lists(self) -> DataSequence[IPv6PrefixListInfo]:
         ...
 
-    @get("/template/policy/list/tloc/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[TLOCListInfo]:
+    @get("/template/policy/list/ipv6prefix/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[IPv6PrefixListInfo]:
         ...
 
-    @post("/template/policy/list/tloc/preview")
-    def preview_policy_list(self, payload: TLOCList) -> PolicyListPreview:
+    @post("/template/policy/list/ipv6prefix/preview")
+    def preview_policy_list(self, payload: IPv6PrefixList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/tloc/preview/{id}")
+    @get("/template/policy/list/ipv6prefix/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/url_allow_list.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/url_allow_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,19 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import URLAllowList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.url import URLAllowList, URLAllowListEditPayload, URLAllowListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class URLAllowListEditPayload(URLAllowList, PolicyListId):
-    pass
-
-
-class URLAllowListInfo(URLAllowList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyURLAllowList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/urlwhitelist")
     def create_policy_list(self, payload: URLAllowList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/urlwhitelist/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/url_block_list.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/app.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,48 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import URLBlockList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.app import AppList, AppListEditPayload, AppListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class URLBlockListEditPayload(URLBlockList, PolicyListId):
-    pass
-
-
-class URLBlockListInfo(URLBlockList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyURLBlockList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/urlblacklist")
-    def create_policy_list(self, payload: URLBlockList) -> PolicyListId:
+class ConfigurationPolicyApplicationList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/app")
+    def create_policy_list(self, payload: AppList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/urlblacklist/{id}")
+    @delete("/template/policy/list/app/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/urlblacklist")
+    @delete("/template/policy/list/app")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/urlblacklist/{id}")
-    def edit_policy_list(self, id: UUID, payload: URLBlockListEditPayload) -> None:
+    @put("/template/policy/list/app/{id}")
+    def edit_policy_list(self, id: UUID, payload: AppListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/urlblacklist/{id}")
-    def get_lists_by_id(self, id: UUID) -> URLBlockListInfo:
+    @get("/template/policy/list/app/{id}")
+    def get_lists_by_id(self, id: UUID) -> AppListInfo:
         ...
 
-    @get("/template/policy/list/urlblacklist", "data")
-    def get_policy_lists(self) -> DataSequence[URLBlockListInfo]:
+    @get("/template/policy/list/app", "data")
+    def get_policy_lists(self) -> DataSequence[AppListInfo]:
         ...
 
-    @get("/template/policy/list/urlblacklist/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[URLBlockListInfo]:
+    @get("/template/policy/list/app/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[AppListInfo]:
         ...
 
-    @post("/template/policy/list/urlblacklist/preview")
-    def preview_policy_list(self, payload: URLBlockList) -> PolicyListPreview:
+    @post("/template/policy/list/app/preview")
+    def preview_policy_list(self, payload: AppList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/urlblacklist/preview/{id}")
+    @get("/template/policy/list/app/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/vpn.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/vpn.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,20 @@
 
 # mypy: disable-error-code="empty-body"
 
 
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import VPNList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
-)
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.vpn import VPNList, VPNListEditPayload, VPNListInfo
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class VPNListEditPayload(VPNList, PolicyListId):
-    pass
-
-
-class VPNListInfo(VPNList, PolicyListInfo):
-    pass
-
-
 class ConfigurationPolicyVPNList(APIEndpoints, PolicyListEndpoints):
     @post("/template/policy/list/vpn")
     def create_policy_list(self, payload: VPNList) -> PolicyListId:
         ...
 
     @delete("/template/policy/list/vpn/{id}")
     def delete_policy_list(self, id: UUID) -> None:
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/list/zone.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,52 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put
-from catalystwan.models.policy.lists import ZoneList
-from catalystwan.models.policy.policy_list import (
-    InfoTag,
-    PolicyListEndpoints,
-    PolicyListId,
-    PolicyListInfo,
-    PolicyListPreview,
+from catalystwan.endpoints.configuration.policy.abstractions import PolicyListEndpoints
+from catalystwan.models.policy.list.threat_grid_api_key import (
+    ThreatGridApiKeyList,
+    ThreatGridApiKeyListEditPayload,
+    ThreatGridApiKeyListInfo,
 )
+from catalystwan.models.policy.policy_list import InfoTag, PolicyListId, PolicyListPreview
 from catalystwan.typed_list import DataSequence
 
 
-class ZoneListEditPayload(ZoneList, PolicyListId):
-    pass
-
-
-class ZoneListInfo(ZoneList, PolicyListInfo):
-    pass
-
-
-class ConfigurationPolicyZoneList(APIEndpoints, PolicyListEndpoints):
-    @post("/template/policy/list/zone")
-    def create_policy_list(self, payload: ZoneList) -> PolicyListId:
+class ConfigurationPolicyThreatGridApiKeyList(APIEndpoints, PolicyListEndpoints):
+    @post("/template/policy/list/tgapikey")
+    def create_policy_list(self, payload: ThreatGridApiKeyList) -> PolicyListId:
         ...
 
-    @delete("/template/policy/list/zone/{id}")
+    @delete("/template/policy/list/tgapikey/{id}")
     def delete_policy_list(self, id: UUID) -> None:
         ...
 
-    @delete("/template/policy/list/zone")
+    @delete("/template/policy/list/tgapikey")
     def delete_policy_lists_with_info_tag(self, params: InfoTag) -> None:
         ...
 
-    @put("/template/policy/list/zone/{id}")
-    def edit_policy_list(self, id: UUID, payload: ZoneListEditPayload) -> None:
+    @put("/template/policy/list/tgapikey/{id}")
+    def edit_policy_list(self, id: UUID, payload: ThreatGridApiKeyListEditPayload) -> None:
         ...
 
-    @get("/template/policy/list/zone/{id}")
-    def get_lists_by_id(self, id: UUID) -> ZoneListInfo:
+    @get("/template/policy/list/tgapikey/{id}")
+    def get_lists_by_id(self, id: UUID) -> ThreatGridApiKeyListInfo:
         ...
 
-    @get("/template/policy/list/zone", "data")
-    def get_policy_lists(self) -> DataSequence[ZoneListInfo]:
+    @get("/template/policy/list/tgapikey", "data")
+    def get_policy_lists(self) -> DataSequence[ThreatGridApiKeyListInfo]:
         ...
 
-    @get("/template/policy/list/zone/filtered", "data")
-    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[ZoneListInfo]:
+    @get("/template/policy/list/tgapikey/filtered", "data")
+    def get_policy_lists_with_info_tag(self, params: InfoTag) -> DataSequence[ThreatGridApiKeyListInfo]:
         ...
 
-    @post("/template/policy/list/zone/preview")
-    def preview_policy_list(self, payload: ZoneList) -> PolicyListPreview:
+    @post("/template/policy/list/tgapikey/preview")
+    def preview_policy_list(self, payload: ThreatGridApiKeyList) -> PolicyListPreview:
         ...
 
-    @get("/template/policy/list/zone/preview/{id}")
+    @get("/template/policy/list/tgapikey/preview/{id}")
     def preview_policy_list_by_id(self, id: UUID) -> PolicyListPreview:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/security_template.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/security_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import JSON, APIEndpoints, delete, get, post, put
 from catalystwan.models.policy.security import (
     AnySecurityPolicy,
+    AnySecurityPolicyInfoList,
     SecurityPolicyEditResponse,
-    SecurityPolicyInfoRoot,
     SecurityPolicyRoot,
 )
-from catalystwan.typed_list import DataSequence
 
 
 class ConfigurationSecurityTemplatePolicy(APIEndpoints):
     @post("/template/policy/security")
     def create_security_template(self, payload: AnySecurityPolicy) -> None:
         ...
 
@@ -32,15 +31,15 @@
         ...
 
     def generate_security_policy_summary(self):
         # GET /template/policy/security/summary
         ...
 
     @get("/template/policy/security", "data")
-    def generate_security_template_list(self) -> DataSequence[SecurityPolicyInfoRoot]:
+    def generate_security_template_list(self) -> AnySecurityPolicyInfoList:
         ...
 
     def get_device_list_by_id(self):
         # GET /template/policy/security/devices/{policyId}
         ...
 
     def get_security_policy_device_list(self):
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/vedge_template.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/vedge_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/policy/vsmart_template.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/policy/vsmart_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration/software_actions.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration/software_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration_dashboard_status.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_dashboard_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration_device_actions.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_device_actions.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 
 DeviceType = Literal["vedge", "controller", "vmanage"]
 
 VersionType = Literal["vmanage", "remote"]
 
 PartitionActionType = Literal["removepartition", "defaultpartition", "changepartition"]
-LxcActionType = Literal["lxc_activate", "lxc_upgrade", "lxc_delete"]
 
 
 class ActionId(BaseModel):
     id: str
 
 
 class GroupId(BaseModel):
@@ -47,44 +46,14 @@
     device_ip: str = Field(serialization_alias="deviceIP", validation_alias="deviceIP")
     version: Union[str, List[str]] = Field(default="")
 
 
 VersionList = Annotated[Union[str, List[str]], BeforeValidator(convert_to_list)]
 
 
-class InstallLxcImage(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    network_function_type: str = Field(
-        default="app-hosting", serialization_alias="networkFunctionType", validation_alias="networkFunctionType"
-    )
-    version_name: str = Field(serialization_alias="versionName", validation_alias="versionName")
-    version_type_name: str = Field(
-        default="UTD-Snort-Feature", serialization_alias="versionTypeName", validation_alias="versionTypeName"
-    )
-
-
-class LxcActivateDevice(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    device_id: str = Field(serialization_alias="deviceId", validation_alias="deviceId")
-    device_ip: str = Field(serialization_alias="deviceIP", validation_alias="deviceIP")
-    install_images: List[InstallLxcImage] = Field(serialization_alias="installImages", validation_alias="installImages")
-    vedge_vpn: str = Field(default="0", serialization_alias="vEdgeVPN", validation_alias="vEdgeVPN")
-    version_type: str = Field(default="vmanage", serialization_alias="versionType", validation_alias="versionType")
-
-
-class LxcUpgradeDevice(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    device_id: str = Field(serialization_alias="deviceId", validation_alias="deviceId")
-    device_ip: str = Field(serialization_alias="deviceIP", validation_alias="deviceIP")
-    install_images: List[InstallLxcImage] = Field(serialization_alias="installImages", validation_alias="installImages")
-
-
 class RemovePartitionDevice(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
 
     device_id: str = Field(serialization_alias="deviceId", validation_alias="deviceId")
     device_ip: str = Field(serialization_alias="deviceIP", validation_alias="deviceIP")
     version: VersionList
 
@@ -93,47 +62,14 @@
     model_config = ConfigDict(populate_by_name=True)
 
     action: PartitionActionType
     device_type: str = Field(serialization_alias="deviceType", validation_alias="deviceType")
     devices: List[PartitionDevice]
 
 
-class LxcInstallInput(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    v_edge_vpn: str = Field(serialization_alias="vEdgeVPN", validation_alias="vEdgeVPN")
-    version_type: VersionType = Field(serialization_alias="versionType", validation_alias="versionType")
-
-
-class LxcImageActivatePayload(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    action: LxcActionType
-    device_type: str = Field(serialization_alias="deviceType", validation_alias="deviceType")
-    devices: List[LxcActivateDevice]
-    input: LxcInstallInput
-
-
-class LxcImageUpgradePayload(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    action: LxcActionType
-    device_type: str = Field(serialization_alias="deviceType", validation_alias="deviceType")
-    devices: List[LxcUpgradeDevice]
-    input: LxcInstallInput
-
-
-class LxcImageDeletePayload(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    action: LxcActionType
-    device_type: str = Field(serialization_alias="deviceType", validation_alias="deviceType")
-    devices: List[LxcUpgradeDevice]
-
-
 class RemovePartitionActionPayload(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
 
     action: PartitionActionType
     device_type: str = Field(serialization_alias="deviceType", validation_alias="deviceType")
     devices: List[RemovePartitionDevice]
 
@@ -309,21 +245,19 @@
         # DELETE /device/action/security/amp/apikey/{uuid}
         ...
 
     @post("/device/action/install")
     def process_install_operation(self, payload: InstallActionPayload) -> ActionId:
         ...
 
-    @post("/device/action/lxcactivate")
-    def process_lxc_activate(self, payload: PartitionActionPayload) -> ActionId:
+    def process_lxc_activate(self):
         # POST /device/action/lxcactivate
         ...
 
-    @post("/device/action/lxcdelete")
-    def process_lxc_delete(self, payload: PartitionActionPayload) -> ActionId:
+    def process_lxc_delete(self):
         # POST /device/action/lxcdelete
         ...
 
     def process_lxc_install(self):
         # POST /device/action/lxcinstall
         ...
 
@@ -331,16 +265,15 @@
         # POST /device/action/lxcreload
         ...
 
     def process_lxc_reset(self):
         # POST /device/action/lxcreset
         ...
 
-    @post("/device/action/lxcupgrade")
-    def process_lxc_upgrade(self, payload: PartitionActionPayload) -> ActionId:
+    def process_lxc_upgrade(self):
         # POST /device/action/lxcupgrade
         ...
 
     def process_reboot(self):
         # POST /device/action/reboot
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration_device_inventory.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration_device_template.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_device_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration_feature_profile.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_feature_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration_group.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_group.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from datetime import datetime
-from typing import List, Optional
+from typing import Any, List, Optional, Union
+from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.common import Solution
 from catalystwan.models.configuration.feature_profile.common import ProfileType
 from catalystwan.typed_list import DataSequence
 
 
 class ProfileId(BaseModel):
-    id: str
+    id: UUID
 
 
 # TODO Get mode from schema
 class ConfigGroupCreationPayload(BaseModel):
     name: str
     description: str
     solution: Solution
@@ -34,18 +35,37 @@
     created_by: str = Field(serialization_alias="createdBy", validation_alias="createdBy")
     last_updated_by: str = Field(serialization_alias="lastUpdatedBy", validation_alias="lastUpdatedBy")
     created_on: datetime = Field(serialization_alias="createdOn", validation_alias="createdOn")
     last_updated_on: datetime = Field(serialization_alias="lastUpdatedOn", validation_alias="lastUpdatedOn")
 
 
 class ConfigGroup(BaseModel):
+    model_config = ConfigDict(populate_by_name=True)
+    id: UUID
     name: str
     description: Optional[str]
     solution: Solution
     profiles: Optional[List[FeatureProfile]]
+    source: Optional[str] = None
+    state: Optional[str] = None
+    devices: Optional[List] = Field(default=[])
+    created_by: Optional[str] = Field(serialization_alias="createdBy", validation_alias="createdBy")
+    last_updated_by: Optional[str] = Field(serialization_alias="lastUpdatedBy", validation_alias="lastUpdatedBy")
+    created_on: Optional[datetime] = Field(serialization_alias="createdOn", validation_alias="createdOn")
+    last_updated_on: Optional[datetime] = Field(serialization_alias="lastUpdatedOn", validation_alias="lastUpdatedOn")
+    version: int
+    number_of_devices: int = Field(serialization_alias="numberOfDevices", validation_alias="numberOfDevices")
+    number_of_devices_up_to_date: int = Field(
+        serialization_alias="numberOfDevicesUpToDate", validation_alias="numberOfDevicesUpToDate"
+    )
+    origin: Optional[str] = None
+    topology: Any = None
+    full_config_cli: Optional[bool] = Field(
+        default=None, serialization_alias="fullConfigCli", validation_alias="fullConfigCli"
+    )
 
 
 class ConfigGroupResponsePayload(BaseModel):
     config_groups: List[ConfigGroup]
 
 
 class ConfigGroupEditPayload(BaseModel):
@@ -64,17 +84,20 @@
 
 
 class ConfigGroupVariablesCreatePayload(BaseModel):
     deviceIds: List[str]
     suggestions: bool = True
 
 
+VariableType = Union[str, int, bool, List[Union[str, int, bool]]]
+
+
 class VariableData(BaseModel):
     name: str
-    value: str
+    value: Optional[VariableType] = None
 
 
 class DeviceVariables(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     device_id: str = Field(serialization_alias="device-id", validation_alias="device-id")
     variables: List[VariableData]
 
@@ -107,15 +130,15 @@
 
 
 class ConfigGroupDisassociateResponse(BaseModel):
     parentTaskId: str
 
 
 class ConfigGroupCreationResponse(BaseModel):
-    id: str
+    id: UUID
 
 
 class EditedProfileId(BaseModel):
     profileId: str
 
 
 class ConfigGroupEditResponse(BaseModel):
@@ -139,15 +162,15 @@
     def create_variables(
         self, config_group_id: str, payload: ConfigGroupVariablesCreatePayload
     ) -> ConfigGroupVariablesCreateResponse:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @delete("/v1/config-group/{config_group_id}")
-    def delete_config_group(self, config_group_id: str) -> None:
+    def delete_config_group(self, config_group_id: UUID) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @post("/v1/config-group/{config_group_id}/device/deploy")
     def deploy(self, config_group_id: str, payload: ConfigGroupDeployPayload) -> ConfigGroupDeployResponse:
         ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/configuration_settings.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/configuration_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -331,14 +331,60 @@
     def check_vpn(cls, vpn_str: str):
         vpn = int(vpn_str)
         if vpn < 0 or vpn > 65530:
             raise ValueError("vpn should be in range 0-65530")
         return vpn_str
 
 
+class CloudCredentials(BaseModel):
+    model_config = ConfigDict(populate_by_name=True)
+
+    umbrella_org_id: Optional[str] = Field(
+        default=None, validation_alias="umbrellaOrgId", serialization_alias="umbrellaOrgId"
+    )
+    umbrella_sig_auth_key: Optional[str] = Field(
+        default=None, validation_alias="umbrellaSIGAuthKey", serialization_alias="umbrellaSIGAuthKey"
+    )
+    umbrella_sig_auth_secret: Optional[str] = Field(
+        default=None, validation_alias="umbrellaSIGAuthSecret", serialization_alias="umbrellaSIGAuthSecret"
+    )
+    umbrella_dns_auth_key: Optional[str] = Field(
+        default=None, validation_alias="umbrellaDNSAuthKey", serialization_alias="umbrellaDNSAuthKey"
+    )
+    umbrella_dns_auth_secret: Optional[str] = Field(
+        default=None, validation_alias="umbrellaDNSAuthSecret", serialization_alias="umbrellaDNSAuthSecret"
+    )
+
+    zscaler_organization: Optional[str] = Field(
+        default=None, validation_alias="zscalerOrganization", serialization_alias="zscalerOrganization"
+    )
+    zscaler_partner_base_uri: Optional[str] = Field(
+        default=None, validation_alias="zscalerPartnerBaseUri", serialization_alias="zscalerPartnerBaseUri"
+    )
+    zscaler_partner_key: Optional[str] = Field(
+        default=None, validation_alias="zscalerPartnerKey", serialization_alias="zscalerPartnerKey"
+    )
+    zscaler_username: Optional[str] = Field(
+        default=None, validation_alias="zscalerUsername", serialization_alias="zscalerUsername"
+    )
+    zscaler_password: Optional[str] = Field(
+        default=None, validation_alias="zscalerPassword", serialization_alias="zscalerPassword"
+    )
+
+    cisco_sse_org_id: Optional[str] = Field(
+        default=None, validation_alias="ciscoSSEOrgId", serialization_alias="ciscoSSEOrgId"
+    )
+    cisco_sse_auth_key: Optional[str] = Field(
+        default=None, validation_alias="ciscoSSEAuthKey", serialization_alias="ciscoSSEAuthKey"
+    )
+    cisco_sse_auth_secret: Optional[str] = Field(
+        default=None, validation_alias="ciscoSSEAuthSecret", serialization_alias="ciscoSSEAuthSecret"
+    )
+
+
 class ConfigurationSettings(APIEndpoints):
     def create_analytics_data_file(self):
         # POST /settings/configuration/analytics/dca
         ...
 
     def edit_cert_configuration(self):
         # PUT /settings/configuration/certificate/{settingType}
@@ -498,14 +544,18 @@
         ...
 
     @view({SingleTenantView, ProviderView})
     @get("/settings/configuration/smartLicensing", "data")
     def get_smart_licensing_settings(self) -> DataSequence[SmartLicensingSetting]:
         ...
 
+    @get("/settings/configuration/cloudProviderSetting", "data")
+    def get_cloud_credentials(self) -> DataSequence[CloudCredentials]:
+        ...
+
     def new_cert_configuration(self):
         # POST /settings/configuration/certificate/{settingType}
         ...
 
     def new_configuration(self):
         # POST /settings/configuration/{settingType}
         ...
@@ -654,7 +704,15 @@
     def edit_walkme(self, payload: WalkMe) -> DataSequence[WalkMe]:
         ...
 
     @view({SingleTenantView, ProviderView})
     @put("/settings/configuration/smartLicensing", "data")
     def edit_smart_licensing_settings(self, payload: SmartLicensingSetting) -> DataSequence[SmartLicensingSetting]:
         ...
+
+    @put("/settings/configuration/cloudProviderSetting", "data")
+    def edit_cloud_credentials(self, payload: CloudCredentials) -> DataSequence[CloudCredentials]:
+        ...
+
+    @post("/settings/configuration/cloudProviderSetting", "data")
+    def create_cloud_credentials(self, payload: CloudCredentials) -> DataSequence[CloudCredentials]:
+        ...
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/endpoints_container.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/endpoints_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 from catalystwan.endpoints.administration_user_and_group import AdministrationUserAndGroup
 from catalystwan.endpoints.certificate_management_device import CertificateManagementDevice
 from catalystwan.endpoints.certificate_management_vmanage import CertificateManagementVManage
 from catalystwan.endpoints.client import Client
 from catalystwan.endpoints.cluster_management import ClusterManagement
 from catalystwan.endpoints.configuration.device.software_update import ConfigurationDeviceSoftwareUpdate
 from catalystwan.endpoints.configuration.disaster_recovery import ConfigurationDisasterRecovery
+from catalystwan.endpoints.configuration.feature_profile.sdwan.cli import CliFeatureProfile
+from catalystwan.endpoints.configuration.feature_profile.sdwan.sig_security import SIGSecurity
 from catalystwan.endpoints.configuration.feature_profile.sdwan.system import SystemFeatureProfile
+from catalystwan.endpoints.configuration.feature_profile.sdwan.topology import TopologyFeatureProfile
 from catalystwan.endpoints.configuration.feature_profile.sdwan.transport import TransportFeatureProfile
 from catalystwan.endpoints.configuration.policy.definition.access_control_list import ConfigurationPolicyAclDefinition
 from catalystwan.endpoints.configuration.policy.definition.access_control_list_ipv6 import (
     ConfigurationPolicyAclIPv6Definition,
 )
 from catalystwan.endpoints.configuration.policy.definition.control import ConfigurationPolicyControlDefinition
 from catalystwan.endpoints.configuration.policy.definition.device_access import (
@@ -60,14 +63,15 @@
 from catalystwan.endpoints.configuration.policy.list.preferred_color_group import ConfigurationPreferredColorGroupList
 from catalystwan.endpoints.configuration.policy.list.prefix import ConfigurationPolicyPrefixList
 from catalystwan.endpoints.configuration.policy.list.protocol_name import ConfigurationPolicyProtocolNameList
 from catalystwan.endpoints.configuration.policy.list.region import ConfigurationPolicyRegionList
 from catalystwan.endpoints.configuration.policy.list.site import ConfigurationPolicySiteList
 from catalystwan.endpoints.configuration.policy.list.sla import ConfigurationPolicySLAClassList
 from catalystwan.endpoints.configuration.policy.list.tloc import ConfigurationPolicyTLOCList
+from catalystwan.endpoints.configuration.policy.list.trunkgroup import ConfigurationPolicyTrunkGroupList
 from catalystwan.endpoints.configuration.policy.list.url_allow_list import ConfigurationPolicyURLAllowList
 from catalystwan.endpoints.configuration.policy.list.url_block_list import ConfigurationPolicyURLBlockList
 from catalystwan.endpoints.configuration.policy.list.vpn import ConfigurationPolicyVPNList
 from catalystwan.endpoints.configuration.policy.list.zone import ConfigurationPolicyZoneList
 from catalystwan.endpoints.configuration.policy.security_template import ConfigurationSecurityTemplatePolicy
 from catalystwan.endpoints.configuration.policy.vedge_template import ConfigurationVEdgeTemplatePolicy
 from catalystwan.endpoints.configuration.policy.vsmart_template import ConfigurationVSmartTemplatePolicy
@@ -80,24 +84,22 @@
     ConfigurationFeatureProfile,
     SDRoutingConfigurationFeatureProfile,
 )
 from catalystwan.endpoints.configuration_group import ConfigurationGroup
 from catalystwan.endpoints.configuration_settings import ConfigurationSettings
 from catalystwan.endpoints.misc import MiscellaneousEndpoints
 from catalystwan.endpoints.monitoring.device_details import MonitoringDeviceDetails
-from catalystwan.endpoints.monitoring.security_policy import MonitoringSecurityPolicy
 from catalystwan.endpoints.monitoring.server_info import ServerInfo
 from catalystwan.endpoints.monitoring.status import MonitoringStatus
 from catalystwan.endpoints.real_time_monitoring.reboot_history import RealTimeMonitoringRebootHistory
 from catalystwan.endpoints.sdavc_cloud_connector import SDAVCCloudConnector
 from catalystwan.endpoints.tenant_backup_restore import TenantBackupRestore
 from catalystwan.endpoints.tenant_management import TenantManagement
 from catalystwan.endpoints.tenant_migration import TenantMigration
 from catalystwan.endpoints.troubleshooting_tools.device_connectivity import TroubleshootingToolsDeviceConnectivity
-from catalystwan.endpoints.url_monitoring import UrlMonitoring
 
 if TYPE_CHECKING:
     from catalystwan.session import ManagerSession
 
 
 class ConfigurationPolicyListContainer:
     def __init__(self, session: ManagerSession):
@@ -122,14 +124,15 @@
         self.preferred_color_group = ConfigurationPreferredColorGroupList(session)
         self.prefix = ConfigurationPolicyPrefixList(session)
         self.protocol_name = ConfigurationPolicyProtocolNameList(session)
         self.region = ConfigurationPolicyRegionList(session)
         self.site = ConfigurationPolicySiteList(session)
         self.sla = ConfigurationPolicySLAClassList(session)
         self.tloc = ConfigurationPolicyTLOCList(session)
+        self.trunkgroup = ConfigurationPolicyTrunkGroupList(session)
         self.url_block_list = ConfigurationPolicyURLBlockList(session)
         self.url_allow_list = ConfigurationPolicyURLAllowList(session)
         self.vpn = ConfigurationPolicyVPNList(session)
         self.zone = ConfigurationPolicyZoneList(session)
 
 
 class ConfigurationPolicyDefinitionContainer:
@@ -159,14 +162,16 @@
         self.security_template = ConfigurationSecurityTemplatePolicy(session)
 
 
 class ConfigurationSDWANFeatureProfileContainer:
     def __init__(self, session: ManagerSession):
         self.transport = TransportFeatureProfile(client=session)
         self.system = SystemFeatureProfile(client=session)
+        self.cli = CliFeatureProfile(client=session)
+        self.topology = TopologyFeatureProfile(client=session)
 
 
 class ConfigurationFeatureProfileContainer:
     def __init__(self, session: ManagerSession):
         self.sdwan = ConfigurationSDWANFeatureProfileContainer(session=session)
 
 
@@ -197,23 +202,22 @@
         self.configuration_device_actions = ConfigurationDeviceActions(session)
         self.configuration_device_software_update = ConfigurationDeviceSoftwareUpdate(session)
         self.configuration_device_template = ConfigurationDeviceTemplate(session)
         self.configuration_settings = ConfigurationSettings(session)
         self.configuration_software_actions = ConfigurationSoftwareActions(session)
         self.configuration_disaster_recovery = ConfigurationDisasterRecovery(session)
         self.monitoring_device_details = MonitoringDeviceDetails(session)
-        self.monitoring_security_policy = MonitoringSecurityPolicy(session)
         self.monitoring_server_info = ServerInfo(session)
         self.monitoring_status = MonitoringStatus(session)
         self.sdavc_cloud_connector = SDAVCCloudConnector(session)
         self.tenant_backup_restore = TenantBackupRestore(session)
         self.tenant_management = TenantManagement(session)
         self.tenant_migration = TenantMigration(session)
         self.configuration_feature_profile = ConfigurationFeatureProfile(session)
         self.configuration_group = ConfigurationGroup(session)
         self.sd_routing_configuration_feature_profile = SDRoutingConfigurationFeatureProfile(session)
         self.configuration_device_inventory = ConfigurationDeviceInventory(session)
         self.troubleshooting_tools = TroubleshootingToolsContainer(session)
         self.misc = MiscellaneousEndpoints(session)
         self.real_time_monitoring = RealTimeMonitoringContainer(session)
         self.certificate_management_device = CertificateManagementDevice(session)
-        self.url_monitoring = UrlMonitoring(session)
+        self.sig_security = SIGSecurity(session)
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/misc.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/monitoring/device_details.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/monitoring/device_details.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/monitoring/status.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/monitoring/status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/real_time_monitoring/reboot_history.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/real_time_monitoring/reboot_history.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/sdavc_cloud_connector.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/sdavc_cloud_connector.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/tenant_backup_restore.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/tenant_backup_restore.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/tenant_management.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/tenant_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/tenant_migration.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/tenant_migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 class MigrationTokenQueryParams(BaseModel):
     model_config = ConfigDict(populate_by_name=True, extra="allow")
     migration_id: str = Field(serialization_alias="migrationId", validation_alias="migrationId")
 
     @model_validator(mode="before")
     @classmethod
     def single_migration_id_required(cls, values: Any):
+        if not isinstance(values, dict):
+            return values
         migration_id = values.get("migrationId")
         if isinstance(migration_id, list) and len(migration_id) == 1:
             values["migrationId"] = migration_id[0]
         return values
 
 
 class ExportInfo(BaseModel):
```

### Comparing `catalystwan-0.33.6/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py` & `catalystwan-0.33.6.dev0/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/exceptions.py` & `catalystwan-0.33.6.dev0/catalystwan/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import Union
 
 from pydantic import BaseModel
 from requests import HTTPError, RequestException
 
 
 class ManagerErrorInfo(BaseModel):
-    message: Union[str, None]
-    details: Union[str, None]
-    code: Union[str, None]
+    message: Union[str, None] = None
+    details: Union[str, None] = None
+    code: Union[str, None] = None
 
 
 class CatalystwanException(Exception):
     """Superclass of all catalystwan SDK exception types."""
 
 
 class ManagerRequestException(RequestException, CatalystwanException):
@@ -28,14 +28,25 @@
         _args = args
         if not _args:
             _args = (info_str,)
         else:
             _args = (str(_args[0]) + "\n" + info_str,) + _args[1:]
         super().__init__(*_args, **kwargs)
 
+    def __str__(self):
+        error_info_str = str(self.info) if self.info else "No error information"
+        request_str = (
+            f"Request: Method: {self.request.method}, URL: {self.request.url},"
+            f"Headers: {self.request.headers}, Body: {self.request.body}"
+        )
+        response_str = (
+            f"Response: {str(self.response.json())}" if self.response else "Response: No response information"
+        )
+        return f"{error_info_str}\n\n {request_str}\n\n {response_str}"
+
 
 class DefaultPasswordError(CatalystwanException):
     """Default password for SDWAN Manager user was detected and needs to be changed."""
 
     pass
```

### Comparing `catalystwan-0.33.6/catalystwan/integration_tests/test_find_template_values.py` & `catalystwan-0.33.6.dev0/catalystwan/integration_tests/test_find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/logging.conf` & `catalystwan-0.33.6.dev0/catalystwan/logging.conf`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/README.md` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/builder.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/builder.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,133 +1,123 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Mapping, Union
+from typing import List, Union
 
 from pydantic import Field
 from typing_extensions import Annotated
 
 from .policy.app_probe import AppProbeMapItem, AppProbeParcel
 from .policy.application_list import ApplicationFamilyListEntry, ApplicationListEntry, ApplicationListParcel
+from .policy.as_path import AsPathParcel
 from .policy.color_list import ColorEntry, ColorParcel
 from .policy.data_prefix import DataPrefixEntry, DataPrefixParcel
 from .policy.expanded_community_list import ExpandedCommunityParcel
 from .policy.fowarding_class import FowardingClassParcel, FowardingClassQueueEntry
 from .policy.ipv6_data_prefix import IPv6DataPrefixEntry, IPv6DataPrefixParcel
 from .policy.ipv6_prefix_list import IPv6PrefixListEntry, IPv6PrefixListParcel
-from .policy.policier import PolicierEntry, PolicierParcel
+from .policy.mirror import MirrorParcel
+from .policy.policer import PolicerEntry, PolicerParcel
 from .policy.prefered_group_color import Preference, PreferredColorGroupEntry, PreferredColorGroupParcel
 from .policy.prefix_list import PrefixListEntry, PrefixListParcel
 from .policy.sla_class import FallbackBestTunnel, SLAAppProbeClass, SLAClassCriteria, SLAClassListEntry, SLAClassParcel
 from .policy.standard_community import StandardCommunityEntry, StandardCommunityParcel
 from .policy.tloc_list import TlocEntry, TlocParcel
+from .security.aip import AdvancedInspectionProfileParcel
+from .security.amp import AdvancedMalwareProtectionParcel
 from .security.application_list import (
     SecurityApplicationFamilyListEntry,
     SecurityApplicationListEntry,
     SecurityApplicationListParcel,
 )
 from .security.data_prefix import SecurityDataPrefixEntry, SecurityDataPrefixParcel
 from .security.fqdn import FQDNDomainParcel, FQDNListEntry
 from .security.geolocation_list import GeoLocationListEntry, GeoLocationListParcel
+from .security.intrusion_prevention import IntrusionPreventionParcel
 from .security.ips_signature import IPSSignatureListEntry, IPSSignatureParcel
 from .security.local_domain import LocalDomainListEntry, LocalDomainParcel
 from .security.protocol_list import ProtocolListEntry, ProtocolListParcel
 from .security.security_port import SecurityPortListEntry, SecurityPortParcel
-from .security.url import BaseURLListEntry, URLAllowParcel, URLBlockParcel
+from .security.ssl_decryption import SslDecryptionParcel
+from .security.ssl_decryption_profile import SslDecryptionProfileParcel
+from .security.url import BaseURLListEntry, URLAllowParcel, URLBlockParcel, URLParcel
 from .security.zone import SecurityZoneListEntry, SecurityZoneListParcel
 
 AnyPolicyObjectParcel = Annotated[
     Union[
-        AppProbeParcel,
+        AdvancedInspectionProfileParcel,
+        AdvancedMalwareProtectionParcel,
+        URLParcel,
         ApplicationListParcel,
+        AppProbeParcel,
+        AsPathParcel,
         ColorParcel,
         DataPrefixParcel,
         ExpandedCommunityParcel,
         FowardingClassParcel,
+        FQDNDomainParcel,
+        GeoLocationListParcel,
+        IntrusionPreventionParcel,
+        IPSSignatureParcel,
         IPv6DataPrefixParcel,
         IPv6PrefixListParcel,
-        PrefixListParcel,
-        PolicierParcel,
-        PreferredColorGroupParcel,
-        SLAClassParcel,
-        TlocParcel,
-        StandardCommunityParcel,
         LocalDomainParcel,
-        FQDNDomainParcel,
-        IPSSignatureParcel,
-        URLAllowParcel,
-        URLBlockParcel,
-        SecurityPortParcel,
+        MirrorParcel,
+        PolicerParcel,
+        PreferredColorGroupParcel,
+        PrefixListParcel,
         ProtocolListParcel,
-        GeoLocationListParcel,
-        SecurityZoneListParcel,
         SecurityApplicationListParcel,
         SecurityDataPrefixParcel,
+        SecurityPortParcel,
+        SecurityZoneListParcel,
+        SLAClassParcel,
+        SslDecryptionParcel,
+        SslDecryptionProfileParcel,
+        StandardCommunityParcel,
+        TlocParcel,
     ],
-    Field(discriminator="type"),
+    Field(discriminator="type_"),
 ]
 
-POLICY_OBJECT_PAYLOAD_ENDPOINT_MAPPING: Mapping[type, str] = {
-    AppProbeParcel: "app-probe",
-    ApplicationListParcel: "app-list",
-    ColorParcel: "color",
-    DataPrefixParcel: "data-prefix",
-    ExpandedCommunityParcel: "expanded-community",
-    FowardingClassParcel: "class",
-    IPv6DataPrefixParcel: "data-ipv6-prefix",
-    IPv6PrefixListParcel: "ipv6-prefix",
-    PrefixListParcel: "prefix",
-    PolicierParcel: "policer",
-    PreferredColorGroupParcel: "preferred-color-group",
-    SLAClassParcel: "sla-class",
-    TlocParcel: "tloc",
-    StandardCommunityParcel: "standard-community",
-    LocalDomainParcel: "security-localdomain",
-    FQDNDomainParcel: "security-fqdn",
-    IPSSignatureParcel: "security-ipssignature",
-    URLAllowParcel: "security-urllist",
-    URLBlockParcel: "security-urllist",
-    SecurityPortParcel: "security-port",
-    ProtocolListParcel: "security-protocolname",
-    GeoLocationListParcel: "security-geolocation",
-    SecurityZoneListParcel: "security-zone",
-    SecurityApplicationListParcel: "security-localapp",
-    SecurityDataPrefixParcel: "security-data-ip-prefix",
-}
-
 __all__ = (
+    "AdvancedInspectionProfileParcel",
+    "AdvancedMalwareProtectionParcel",
     "AnyPolicyObjectParcel",
     "ApplicationFamilyListEntry",
     "ApplicationListEntry",
     "ApplicationListParcel",
     "AppProbeEntry",
     "AppProbeMapItem",
     "AppProbeParcel",
+    "AsPathParcel",
     "BaseURLListEntry",
     "ColorEntry",
     "ColorParcel",
     "DataPrefixEntry",
     "DataPrefixParcel",
     "ExpandedCommunityParcel",
     "FallbackBestTunnel",
     "FowardingClassParcel",
     "FowardingClassQueueEntry",
     "FQDNDomainParcel",
     "FQDNListEntry",
     "GeoLocationListEntry",
     "GeoLocationListParcel",
+    "IntrusionPreventionParcel",
     "IPSSignatureListEntry",
     "IPSSignatureParcel",
     "IPv6DataPrefixEntry",
     "IPv6DataPrefixParcel",
     "IPv6PrefixListEntry",
     "IPv6PrefixListParcel",
     "LocalDomainListEntry",
     "LocalDomainParcel",
-    "PolicierEntry",
-    "PolicierParcel",
+    "MirrorParcel",
+    "PolicerEntry",
+    "PolicerParcel",
     "Preference",
     "PreferredColorGroupEntry",
     "PreferredColorGroupParcel",
     "PrefixListEntry",
     "PrefixListParcel",
     "ProtocolListEntry",
     "ProtocolListParcel",
@@ -140,18 +130,21 @@
     "SecurityPortParcel",
     "SecurityZoneListEntry",
     "SecurityZoneListParcel",
     "SLAAppProbeClass",
     "SLAClassCriteria",
     "SLAClassListEntry",
     "SLAClassParcel",
+    "SslDecryptionParcel",
+    "SslDecryptionProfileParcel",
     "StandardCommunityEntry",
     "StandardCommunityParcel",
     "TlocEntry",
     "TlocParcel",
+    "URLParcel",
     "URLAllowParcel",
     "URLBlockParcel",
 )
 
 
 def __dir__() -> "List[str]":
     return list(__all__)
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import TLOCColor
 
 
@@ -24,14 +24,15 @@
     map: List[AppProbeMapItem] = Field(default=[])
     forwarding_class_name: Global[str] = Field(
         serialization_alias="forwardingClass", validation_alias="forwardingClass"
     )
 
 
 class AppProbeParcel(_ParcelBase):
+    type_: Literal["app-probe"] = Field(default="app-probe", exclude=True)
     entries: List[AppProbeEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_fowarding_class(self, forwarding_class_name: str):
         self.entries.append(
             AppProbeEntry(
                 forwarding_class_name=as_global(forwarding_class_name),
             )
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Union
+from typing import List, Literal, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class ApplicationListEntry(BaseModel):
@@ -14,14 +14,15 @@
 
 class ApplicationFamilyListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     app_list_family: Global[str] = Field(serialization_alias="appFamily", validation_alias="appFamily")
 
 
 class ApplicationListParcel(_ParcelBase):
+    type_: Literal["app-list"] = Field(default="app-list", exclude=True)
     entries: List[Union[ApplicationListEntry, ApplicationFamilyListEntry]] = Field(
         default=[], validation_alias=AliasPath("data", "entries")
     )
 
     def add_application(self, application: str):
         self.entries.append(ApplicationListEntry(app_list=as_global(application)))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from ipaddress import IPv4Address, IPv4Network
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class DataPrefixEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     ipv4_address: Global[IPv4Address] = Field(serialization_alias="ipv4Address", validation_alias="ipv4Address")
     ipv4_prefix_length: Global[int] = Field(serialization_alias="ipv4PrefixLength", validation_alias="ipv4PrefixLength")
 
+    @staticmethod
+    def from_ipv4_network(ipv4_network: IPv4Network) -> "DataPrefixEntry":
+        return DataPrefixEntry(
+            ipv4_address=as_global(ipv4_network.network_address),
+            ipv4_prefix_length=as_global(ipv4_network.prefixlen),
+        )
+
 
 class DataPrefixParcel(_ParcelBase):
+    type_: Literal["data-prefix"] = Field(default="data-prefix", exclude=True)
     entries: List[DataPrefixEntry] = Field(default_factory=list, validation_alias=AliasPath("data", "entries"))
 
     def add_data_prefix(self, ipv4_network: IPv4Network):
-        self.entries.append(
-            DataPrefixEntry(
-                ipv4_address=as_global(ipv4_network.network_address),
-                ipv4_prefix_length=as_global(ipv4_network.prefixlen),
-            )
-        )
+        self.entries.append(DataPrefixEntry.from_ipv4_network(ipv4_network))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from typing import List, Literal
+
 from pydantic import AliasPath, ConfigDict, Field, field_validator
 
-from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
+from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase
 
 
 class ExpandedCommunityParcel(_ParcelBase):
+    type_: Literal["expanded-community"] = Field(default="expanded-community", exclude=True)
     model_config = ConfigDict(populate_by_name=True)
-    expandedCommunityList: Global[list] = Field(
-        default=as_global([]),
+    expanded_community_list: Global[List[str]] = Field(
+        default=Global[List[str]](value=list()),
         serialization_alias="expandedCommunityList",
         validation_alias=AliasPath("data", "expandedCommunityList"),
     )
 
     def add_community(self, expanded_community: str):
-        self.expandedCommunityList.value.append(expanded_community)
+        self.expanded_community_list.value.append(expanded_community)
 
-    @field_validator("expandedCommunityList")
+    @field_validator("expanded_community_list")
     @classmethod
-    def check_rate(cls, expanded_community_list: Global):
+    def check_list_str(cls, expanded_community_list: Global):
         assert all([isinstance(ec, str) for ec in expanded_community_list.value])
         return expanded_community_list
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class FowardingClassQueueEntry(BaseModel):
@@ -14,11 +14,12 @@
     @classmethod
     def check_burst(cls, queue: Global):
         assert 0 <= int(queue.value) <= 7
         return queue
 
 
 class FowardingClassParcel(_ParcelBase):
+    type_: Literal["class"] = Field(default="class", exclude=True)
     entries: List[FowardingClassQueueEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_queue(self, queue: int):
         self.entries.append(FowardingClassQueueEntry(queue=as_global(str(queue))))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from ipaddress import IPv6Address, IPv6Network
-from typing import List
+from ipaddress import IPv6Address, IPv6Interface
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class IPv6DataPrefixEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     ipv6_address: Global[IPv6Address] = Field(serialization_alias="ipv6Address", validation_alias="ipv6Address")
     ipv6_prefix_length: Global[int] = Field(serialization_alias="ipv6PrefixLength", validation_alias="ipv6PrefixLength")
 
 
 class IPv6DataPrefixParcel(_ParcelBase):
+    type_: Literal["data-ipv6-prefix"] = Field(default="data-ipv6-prefix", exclude=True)
     entries: List[IPv6DataPrefixEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
-    def add_prefix(self, ipv6_network: IPv6Network):
+    def add_prefix(self, ipv6_network: IPv6Interface):
         self.entries.append(
             IPv6DataPrefixEntry(
-                ipv6_address=as_global(ipv6_network.network_address),
-                ipv6_prefix_length=as_global(ipv6_network.prefixlen),
+                ipv6_address=as_global(ipv6_network.network.network_address),
+                ipv6_prefix_length=as_global(ipv6_network.network.prefixlen),
             )
         )
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from ipaddress import IPv6Address, IPv6Network
-from typing import List
+from ipaddress import IPv4Address, IPv4Network
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
-class IPv6PrefixListEntry(BaseModel):
+class PrefixListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    ipv6_address: Global[IPv6Address] = Field(serialization_alias="ipv6Address", validation_alias="ipv6Address")
-    ipv6_prefix_length: Global[int] = Field(serialization_alias="ipv6PrefixLength", validation_alias="ipv6PrefixLength")
+    ipv4_address: Global[IPv4Address] = Field(serialization_alias="ipv4Address", validation_alias="ipv4Address")
+    ipv4_prefix_length: Global[int] = Field(serialization_alias="ipv4PrefixLength", validation_alias="ipv4PrefixLength")
 
 
-class IPv6PrefixListParcel(_ParcelBase):
-    entries: List[IPv6PrefixListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
+class PrefixListParcel(_ParcelBase):
+    type_: Literal["prefix"] = Field(default="prefix", exclude=True)
+    entries: List[PrefixListEntry] = Field(default_factory=list, validation_alias=AliasPath("data", "entries"))
 
-    def add_prefix(self, ipv6_network: IPv6Network):
+    def add_prefix(self, ipv4_network: IPv4Network):
         self.entries.append(
-            IPv6PrefixListEntry(
-                ipv6_address=as_global(ipv6_network.network_address),
-                ipv6_prefix_length=as_global(ipv6_network.prefixlen),
+            PrefixListEntry(
+                ipv4_address=as_global(ipv4_network.network_address),
+                ipv4_prefix_length=as_global(ipv4_network.prefixlen),
             )
         )
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policier.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
-from catalystwan.models.policy.lists_entries import PolicerExceedAction
 
+PolicerExceedAction = Literal[
+    "drop",
+    "remark",
+]
 
-class PolicierEntry(BaseModel):
+
+class PolicerEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     burst: Global[int]
     exceed: Global[PolicerExceedAction]
     rate: Global[int]
 
     @field_validator("burst")
     @classmethod
@@ -23,18 +27,19 @@
     @field_validator("rate")
     @classmethod
     def check_rate(cls, rate_str: Global):
         assert 8 <= rate_str.value <= 100_000_000_000
         return rate_str
 
 
-class PolicierParcel(_ParcelBase):
-    entries: List[PolicierEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
+class PolicerParcel(_ParcelBase):
+    type_: Literal["policer"] = Field(default="policer", exclude=True)
+    entries: List[PolicerEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_entry(self, burst: int, exceed: PolicerExceedAction, rate: int):
         self.entries.append(
-            PolicierEntry(
+            PolicerEntry(
                 burst=as_global(burst),
                 exceed=as_global(exceed, PolicerExceedAction),
                 rate=as_global(rate),
             )
         )
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Optional
+from typing import List, Literal, Optional
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, model_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import TLOCColor
-from catalystwan.models.policy.lists_entries import PathPreference
+
+PathPreference = Literal[
+    "direct-path",
+    "multi-hop-path",
+    "all-paths",
+]
 
 
 class Preference(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     color_preference: Global[list] = Field(serialization_alias="colorPreference", validation_alias="colorPreference")
     path_preference: Global[PathPreference] = Field(
         serialization_alias="pathPreference", validation_alias="pathPreference"
@@ -33,14 +38,15 @@
     def check_passwords_match(self) -> "PreferredColorGroupEntry":
         if not self.secondary_preference and self.tertiary_preference:
             raise ValueError("Preference Entry has to have a secondary prefrence when assigning tertiary preference.")
         return self
 
 
 class PreferredColorGroupParcel(_ParcelBase):
+    type_: Literal["preferred-color-group"] = Field(default="preferred-color-group", exclude=True)
     entries: List[PreferredColorGroupEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_primary(self, color_preference: List[TLOCColor], path_preference: PathPreference):
         self.entries.append(
             PreferredColorGroupEntry(
                 primary_preference=Preference(
                     color_preference=as_global(color_preference),
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from ipaddress import IPv4Address, IPv4Network
-from typing import List
+from typing import List, Literal, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
-class PrefixListEntry(BaseModel):
+class SecurityApplicationListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    ipv4_address: Global[IPv4Address] = Field(serialization_alias="ipv4Address", validation_alias="ipv4Address")
-    ipv4_prefix_length: Global[int] = Field(serialization_alias="ipv4PrefixLength", validation_alias="ipv4PrefixLength")
+    app_list: Global[str] = Field(serialization_alias="app", validation_alias="app")
 
 
-class PrefixListParcel(_ParcelBase):
-    entries: List[PrefixListEntry] = Field(default_factory=list, validation_alias=AliasPath("data", "entries"))
+class SecurityApplicationFamilyListEntry(BaseModel):
+    model_config = ConfigDict(populate_by_name=True)
+    app_list_family: Global[str] = Field(serialization_alias="appFamily", validation_alias="appFamily")
+
+
+class SecurityApplicationListParcel(_ParcelBase):
+    type_: Literal["security-localapp"] = Field(default="security-localapp", exclude=True)
+    entries: List[Union[SecurityApplicationFamilyListEntry, SecurityApplicationListEntry]] = Field(
+        default=[], validation_alias=AliasPath("data", "entries")
+    )
+
+    def add_application(self, application: str):
+        self.entries.append(SecurityApplicationListEntry(app_list=as_global(application)))
 
-    def add_prefix(self, ipv4_network: IPv4Network):
-        self.entries.append(
-            PrefixListEntry(
-                ipv4_address=as_global(ipv4_network.network_address),
-                ipv4_prefix_length=as_global(ipv4_network.prefixlen),
-            )
-        )
+    def add_application_family(self, application_family: str):
+        self.entries.append(SecurityApplicationFamilyListEntry(app_list_family=as_global(application_family)))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     # validators
     _jitter_validator = field_validator("jitter")(check_jitter_ms)
     _latency_validator = field_validator("latency")(check_latency_ms)
     _loss_validator = field_validator("loss")(check_loss_percent)
 
 
 class SLAClassParcel(_ParcelBase):
+    type_: Literal["sla-class"] = Field(default="sla-class", exclude=True)
     entries: List[SLAClassListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_entry(
         self,
         app_probe_class_id: UUID,
         loss: Optional[int] = None,
         jitter: Optional[int] = None,
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import WellKnownBGPCommunities
 
 
 class StandardCommunityEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    standard_community: Global[WellKnownBGPCommunities] = Field(
+    standard_community: Global[str] = Field(
         serialization_alias="standardCommunity", validation_alias="standardCommunity"
     )
 
 
 class StandardCommunityParcel(_ParcelBase):
+    type_: Literal["standard-community"] = Field(default="standard-community", exclude=True)
     entries: List[StandardCommunityEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
-    def add_community(self, standard_community: WellKnownBGPCommunities):
-        self.entries.append(
-            StandardCommunityEntry(standard_community=as_global(standard_community, WellKnownBGPCommunities))
-        )
+    def _add_community(self, standard_community: str):
+        self.entries.append(StandardCommunityEntry(standard_community=as_global(standard_community)))
+
+    def add_well_known_community(self, standard_community: WellKnownBGPCommunities):
+        self._add_community(standard_community)
+
+    def add_community(self, as_number: int, community_number: int) -> None:
+        self._add_community(f"{as_number}:{community_number}")
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from ipaddress import IPv4Address
-from typing import List, Optional
+from typing import List, Literal, Optional
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import TLOCColor
-from catalystwan.models.policy.lists_entries import EncapType
+
+EncapType = Literal[
+    "ipsec",
+    "gre",
+]
 
 
 class TlocEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     tloc: Global[IPv4Address]
     color: Global[TLOCColor]
     encapsulation: Global[EncapType] = Field(serialization_alias="encap", validation_alias="encap")
@@ -24,14 +28,15 @@
             return v
         if not (0 <= int(v.value) < 4_294_967_295):
             raise ValueError('"preference" not in range 0 - 4 294 967 295 (2 ** 32 - 1)')
         return v
 
 
 class TlocParcel(_ParcelBase):
+    type_: Literal["tloc"] = Field(default="tloc", exclude=True)
     entries: List[TlocEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_entry(
         self, tloc: IPv4Address, color: TLOCColor, encapsulation: EncapType, preference: Optional[str] = None
     ):
         self.entries.append(
             TlocEntry(
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from ipaddress import IPv4Network
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
-class SecurityDataPrefixEntry(BaseModel):
+class AsPathEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    ip_prefix: Global[IPv4Network] = Field(serialization_alias="ipPrefix", validation_alias="ipPrefix")
+    as_path: Global[str] = Field(validation_alias="asPath", serialization_alias="asPath")
 
 
-class SecurityDataPrefixParcel(_ParcelBase):
-    entries: List[SecurityDataPrefixEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
+class AsPathParcel(_ParcelBase):
+    type_: Literal["as-path"] = Field(default="as-path", exclude=True)
+    as_path_list_num: Global[int] = Field(validation_alias=AliasPath("data", "asPathListNum"))
+    entries: List[AsPathEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
-    def add_prefix(self, ip_prefix: IPv4Network):
-        self.entries.append(SecurityDataPrefixEntry(ip_prefix=as_global(ip_prefix)))
+    def add_as_path(self, as_path: str):
+        self.entries.append(AsPathEntry(as_path=as_global(as_path)))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
+from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase
 
 
-class FQDNListEntry(BaseModel):
+class MirrorEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    pattern: Global[str] = Field(
-        description="Ex: cisco.com, .*cisco.com, .*.cisco.com. Should not start with '*' or '+'"
-    )
+    remote_dest_ip: Global[str] = Field(validation_alias="remoteDestIp", serialization_alias="remoteDestIp")
+    source_ip: Global[str] = Field(validation_alias="sourceIp", serialization_alias="sourceIp")
 
 
-class FQDNDomainParcel(_ParcelBase):
-    entries: List[FQDNListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
-
-    def from_fqdns(self, fqdns: List[str]):
-        for fqdn in fqdns:
-            self.entries.append(FQDNListEntry(pattern=as_global(fqdn)))
+class MirrorParcel(_ParcelBase):
+    type_: Literal["mirror"] = Field(default="mirror", exclude=True)
+    entries: List[MirrorEntry] = Field(validation_alias=AliasPath("data", "entries"), min_length=1, max_length=1)
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Optional
+from typing import List, Literal, Optional
 
 from pydantic import AliasPath, BaseModel, Field, model_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import check_fields_exclusive
 
 
@@ -17,14 +17,15 @@
     @model_validator(mode="after")
     def check_country_xor_continent(self):
         check_fields_exclusive(self.__dict__, {"country", "continent"}, True)
         return self
 
 
 class GeoLocationListParcel(_ParcelBase):
+    type_: Literal["security-geolocation"] = Field(default="security-geolocation", exclude=True)
     entries: List[GeoLocationListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_country(self, country: str):
         self.entries.append(GeoLocationListEntry(country=as_global(country)))
 
     def add_continent(self, continent: str):
         self.entries.append(GeoLocationListEntry(continent=as_global(continent)))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class IPSSignatureListEntry(BaseModel):
@@ -26,14 +26,15 @@
     @classmethod
     def check_signature_id(cls, signature_id: Global):
         assert 0 <= int(signature_id.value) <= 4294967295
         return signature_id
 
 
 class IPSSignatureParcel(_ParcelBase):
+    type_: Literal["security-ipssignature"] = Field(default="security-ipssignature", exclude=True)
     entries: List[IPSSignatureListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_signature(self, signature: str):
         generator_id, signature_id = signature.split(":")
         self.entries.append(
             IPSSignatureListEntry(
                 generator_id=as_global(generator_id),
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class LocalDomainListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     name_server: Global[str] = Field(
         serialization_alias="nameServer", validation_alias="nameServer", description="Ex: cisco.com, *.cisco.com"
     )
 
 
 class LocalDomainParcel(_ParcelBase):
+    type_: Literal["security-localdomain"] = Field(default="security-localdomain", exclude=True)
     entries: List[LocalDomainListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def from_local_domains(self, domains: List[str]):
         for domain in domains:
             self.entries.append(LocalDomainListEntry(name_server=as_global(domain)))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class ProtocolListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     protocol: Global[str] = Field(serialization_alias="protocolName", validation_alias="protocolName")
 
 
 class ProtocolListParcel(_ParcelBase):
+    type_: Literal["security-protocolname"] = Field(default="security-protocolname", exclude=True)
     entries: List[ProtocolListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_protocol(self, protocol: str):
         self.entries.append(ProtocolListEntry(protocol=as_global(protocol)))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List
+from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class BaseURLListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     pattern: Global[str]
 
 
-class BaseURLParcel(_ParcelBase):
+class URLParcel(_ParcelBase):
+    type_: Literal["security-urllist"] = Field(default="security-urllist", exclude=True)
+    type: Literal["urlallowed", "urlblocked"]
     entries: List[BaseURLListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_url(self, pattern: str):
         self.entries.append(BaseURLListEntry(pattern=as_global(pattern)))
 
 
-class URLAllowParcel(BaseURLParcel):
-    parcel_type: str = Field(default="urlallowed", validation_alias="type", serialization_alias="type")
+class URLAllowParcel(URLParcel):
+    type_: Literal["security-urllist"] = Field(default="security-urllist", exclude=True)
+    type: Literal["urlallowed"] = "urlallowed"
 
 
-class URLBlockParcel(BaseURLParcel):
-    parcel_type: str = Field(default="urlblocked", validation_alias="type", serialization_alias="type")
+class URLBlockParcel(URLParcel):
+    type_: Literal["security-urllist"] = Field(default="security-urllist", exclude=True)
+    type: Literal["urlblocked"] = "urlblocked"
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Optional
+from typing import List, Literal, Optional
 
 from pydantic import AliasPath, BaseModel, Field, field_validator, model_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 from catalystwan.models.common import InterfaceType, check_fields_exclusive
 
 
@@ -21,22 +21,23 @@
     @model_validator(mode="after")
     def check_vpn_xor_interface(self):
         check_fields_exclusive(self.__dict__, {"vpn", "interface"}, True)
         return self
 
 
 class SecurityZoneListParcel(_ParcelBase):
+    type_: Literal["security-zone"] = Field(default="security-zone", exclude=True)
     entries: List[SecurityZoneListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_interface(self, interface: InterfaceType):
         self.entries.append(
             SecurityZoneListEntry(
                 interface=as_global(interface, InterfaceType),
             )
         )
 
     def add_vpn(self, vpn: str):
         self.entries.append(
             SecurityZoneListEntry(
-                vpn=as_global(vpn, InterfaceType),
+                vpn=as_global(vpn),
             )
         )
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,20 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
+from __future__ import annotations
 
+from ipaddress import IPv4Address, IPv6Address, IPv6Interface
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field, model_validator
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.common import ServiceChainNumber
+from catalystwan.api.configuration_groups.parcel import Default, Global, _ParcelBase, as_default
 
-Action = Literal[
-    "drop",
-    "accept",
-]
-
-IcmpMessage = Literal[
-    "administratively-prohibited",
-    "dod-host-prohibited",
-    "dod-net-prohibited",
-    "echo",
-    "echo-reply",
-    "echo-reply-no-error",
-    "extended-echo",
-    "extended-echo-reply",
-    "general-parameter-problem",
-    "host-isolated",
-    "host-precedence-unreachable",
-    "host-redirect",
-    "host-tos-redirect",
-    "host-tos-unreachable",
-    "host-unknown",
-    "host-unreachable",
-    "interface-error",
-    "malformed-query",
-    "multiple-interface-match",
-    "net-redirect",
-    "net-tos-redirect",
-    "net-tos-unreachable",
-    "net-unreachable",
-    "network-unknown",
-    "no-room-for-option",
-    "option-missing",
-    "packet-too-big",
-    "parameter-problem",
-    "photuris",
-    "port-unreachable",
-    "precedence-unreachable",
-    "protocol-unreachable",
-    "reassembly-timeout",
-    "redirect",
-    "router-advertisement",
-    "router-solicitation",
-    "source-route-failed",
-    "table-entry-error",
-    "time-exceeded",
-    "timestamp-reply",
-    "timestamp-request",
-    "ttl-exceeded",
-    "unreachable",
-]
-
-Icmp6Message = Literal[
+Action = Literal["drop", "accept"]
+Icmp6Msg = Literal[
     "beyond-scope",
     "cp-advertisement",
     "cp-solicitation",
     "destination-unreachable",
     "dhaad-reply",
     "dhaad-request",
     "echo-reply",
@@ -109,301 +60,383 @@
     "router-solicitation",
     "rpl-control",
     "source-policy",
     "source-route-header",
     "time-exceeded",
     "unreachable",
 ]
+IcmpMsg = Literal[
+    "administratively-prohibited",
+    "dod-host-prohibited",
+    "dod-net-prohibited",
+    "echo",
+    "echo-reply",
+    "echo-reply-no-error",
+    "extended-echo",
+    "extended-echo-reply",
+    "general-parameter-problem",
+    "host-isolated",
+    "host-precedence-unreachable",
+    "host-redirect",
+    "host-tos-redirect",
+    "host-tos-unreachable",
+    "host-unknown",
+    "host-unreachable",
+    "interface-error",
+    "malformed-query",
+    "multiple-interface-match",
+    "net-redirect",
+    "net-tos-redirect",
+    "net-tos-unreachable",
+    "net-unreachable",
+    "network-unknown",
+    "no-room-for-option",
+    "option-missing",
+    "packet-too-big",
+    "parameter-problem",
+    "photuris",
+    "port-unreachable",
+    "precedence-unreachable",
+    "protocol-unreachable",
+    "reassembly-timeout",
+    "redirect",
+    "router-advertisement",
+    "router-solicitation",
+    "source-route-failed",
+    "table-entry-error",
+    "time-exceeded",
+    "timestamp-reply",
+    "timestamp-request",
+    "ttl-exceeded",
+    "unreachable",
+]
+Tcp = Literal["syn"]
 
 
-class SourceDataIPv4Prefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    source_ip_prefix: Union[Global[str], Variable] = Field(
-        serialization_alias="sourceIpPrefix", validation_alias="sourceIpPrefix"
+class ReferenceId(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
+    ref_id: Global[UUID] = Field(..., serialization_alias="refId", validation_alias="refId")
 
 
-class SourceDataIPv6Prefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    source_ip_prefix: Union[Global[str], Variable] = Field(
-        serialization_alias="sourceIpPrefix", validation_alias="sourceIpPrefix"
+class SourceDataPrefixListReference(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-
-
-class SourceDataIPv4PrefixParcel(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    source_data_prefix_list: Global[UUID] = Field(
-        serialization_alias="sourceDataPrefixList", validation_alias="sourceDataPrefixList"
+    source_data_prefix_list: ReferenceId = Field(
+        ...,
+        serialization_alias="sourceDataPrefixList",
+        validation_alias="sourceDataPrefixList",
+        description="Source Data Prefix Parcel",
     )
 
 
-class SourceDataIPv6PrefixParcel(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    source_data_prefix_list: Global[UUID] = Field(
-        serialization_alias="sourceDataPrefixList", validation_alias="sourceDataPrefixList"
+class SourceDataPrefixIp(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    source_ip_prefix: Global[str] = Field(
+        ...,
+        serialization_alias="sourceIpPrefix",
+        validation_alias="sourceIpPrefix",
+        description="Source Data IP Prefix",
     )
 
 
 class SourcePort(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    source_port: Global[int] = Field(serialization_alias="sourcePort", validation_alias="sourcePort")
-
-
-class DestinationDataIPv4Prefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    destination_ip_prefix: Union[Global[str], Variable] = Field(
-        serialization_alias="destinationIpPrefix", validation_alias="destinationIpPrefix"
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-
-
-class DestinationDataIPv6Prefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    destination_ip_prefix: Union[Global[str], Variable] = Field(
-        serialization_alias="destinationIpPrefix", validation_alias="destinationIpPrefix"
+    source_port: Union[Global[int], Global[str]] = Field(
+        ...,
+        serialization_alias="sourcePort",
+        validation_alias="sourcePort",
+        description="source port range or individual port number",
     )
 
 
-class DestinationDataIPv4PrefixParcel(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    destination_data_prefix_list: Global[UUID] = Field(
-        serialization_alias="destinationDataPrefixList", validation_alias="destinationDataPrefixList"
+class DestinationDataPrefixListReference(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    destination_data_prefix_list: ReferenceId = Field(
+        ...,
+        serialization_alias="destinationDataPrefixList",
+        validation_alias="destinationDataPrefixList",
+        description="Destination Data Prefix Parcel",
     )
 
 
-class DestinationDataIPv6PrefixParcel(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    destination_data_prefix_list: Global[UUID] = Field(
-        serialization_alias="destinationDataPrefixList", validation_alias="destinationDataPrefixList"
+class DestinationDataPrefixIp(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    destination_ip_prefix: Global[IPv6Interface] = Field(
+        ...,
+        serialization_alias="destinationIpPrefix",
+        validation_alias="destinationIpPrefix",
+        description="Destination Data IP Prefix",
     )
 
 
 class DestinationPort(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    destination_port: Global[int] = Field(serialization_alias="destinationPort", validation_alias="destinationPort")
-
-
-TcpState = Literal["syn"]
-
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    destination_port: Union[Global[int], Global[str]] = Field(
+        ...,
+        serialization_alias="destinationPort",
+        validation_alias="destinationPort",
+        description="destination port range or individual port number",
+    )
 
-class IPv4Match(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    dscp: Optional[Global[List[int]]] = None
-    packet_length: Optional[Global[int]] = Field(
-        serialization_alias="packetLength", validation_alias="packetLength", default=None
+class Ipv4MatchEntry(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    dscp: Optional[Global[List[int]]] = Field(default=None, description="DSCP number")
+    packet_length: Optional[Union[Global[int], Global[str]]] = Field(
+        default=None, serialization_alias="packetLength", validation_alias="packetLength", description="Packet Length"
     )
-    protocol: Optional[Global[List[int]]] = None
-    icmp_message: Optional[Global[List[IcmpMessage]]] = Field(
-        serialization_alias="icmpMsg", validation_alias="icmpMsg", default=None
+    protocol: Optional[Global[List[int]]] = Field(
+        default=None, description="protocol number list with at least one item"
     )
-    source_data_prefix: Optional[Union[SourceDataIPv4Prefix, SourceDataIPv4PrefixParcel]] = Field(
-        serialization_alias="sourceDataPrefix", validation_alias="sourceDataPrefix", default=None
+    icmp_msg: Optional[IcmpMsg] = Field(
+        default=None, serialization_alias="icmpMsg", validation_alias="icmpMsg", description="ICMP Message"
+    )
+    source_data_prefix: Optional[Union[SourceDataPrefixListReference, SourceDataPrefixIp]] = Field(
+        default=None, serialization_alias="sourceDataPrefix", validation_alias="sourceDataPrefix"
     )
     source_ports: Optional[List[SourcePort]] = Field(
-        serialization_alias="sourcePorts", validation_alias="sourcePorts", default=None
+        default=None, serialization_alias="sourcePorts", validation_alias="sourcePorts", description="Source Port List"
     )
-    destination_data_prefix: Optional[Union[DestinationDataIPv4Prefix, DestinationDataIPv4PrefixParcel]] = Field(
-        serialization_alias="destinationDataPrefix", validation_alias="destinationDataPrefix", default=None
+    destination_data_prefix: Optional[Union[DestinationDataPrefixListReference, DestinationDataPrefixIp]] = Field(
+        default=None, serialization_alias="destinationDataPrefix", validation_alias="destinationDataPrefix"
     )
     destination_ports: Optional[List[DestinationPort]] = Field(
-        serialization_alias="destinationPorts", validation_alias="destinationPorts", default=None
-    )
-    tcp: Optional[Global[TcpState]] = None
+        default=None,
+        serialization_alias="destinationPorts",
+        validation_alias="destinationPorts",
+        description="Destination Port List",
+    )
+    tcp: Optional[Tcp] = Field(default=None, description="TCP States")
 
 
-class IPv6Match(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
+class Ipv6MatchEntry(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
     next_header: Optional[Global[int]] = Field(
-        serialization_alias="nextHeader", validation_alias="nextHeader", default=None
+        default=None, serialization_alias="nextHeader", validation_alias="nextHeader", description="next header number"
     )
-    packet_length: Optional[Global[int]] = Field(
-        serialization_alias="packetLength", validation_alias="packetLength", default=None
+    packet_length: Optional[Union[Global[int], Global[str]]] = Field(
+        default=None, serialization_alias="packetLength", validation_alias="packetLength", description="Packet Length"
     )
-    source_data_prefix: Optional[Union[SourceDataIPv6Prefix, SourceDataIPv6PrefixParcel]] = Field(
-        serialization_alias="sourceDataPrefix", validation_alias="sourceDataPrefix", default=None
+    source_data_prefix: Optional[Union[SourceDataPrefixListReference, SourceDataPrefixIp]] = Field(
+        default=None, serialization_alias="sourceDataPrefix", validation_alias="sourceDataPrefix"
     )
     source_ports: Optional[List[SourcePort]] = Field(
-        serialization_alias="sourcePorts", validation_alias="sourcePorts", default=None
+        default=None, serialization_alias="sourcePorts", validation_alias="sourcePorts", description="Source Port List"
     )
-    destination_data_prefix: Optional[Union[DestinationDataIPv6Prefix, DestinationDataIPv6PrefixParcel]] = Field(
-        serialization_alias="destinationDataPrefix", validation_alias="destinationDataPrefix", default=None
+    destination_data_prefix: Optional[Union[DestinationDataPrefixListReference, DestinationDataPrefixIp]] = Field(
+        default=None, serialization_alias="destinationDataPrefix", validation_alias="destinationDataPrefix"
     )
     destination_ports: Optional[List[DestinationPort]] = Field(
-        serialization_alias="destinationPorts", validation_alias="destinationPorts", default=None
-    )
-    tcp: Optional[Global[TcpState]] = None
-    traffic_class: Optional[Global[int]] = None
-    icmp6_message: Optional[Global[List[Icmp6Message]]] = Field(
-        serialization_alias="icmpMsg", validation_alias="icmpMsg", default=None
+        default=None,
+        serialization_alias="destinationPorts",
+        validation_alias="destinationPorts",
+        description="Destination Port List",
+    )
+    tcp: Optional[Global[Tcp]] = Field(default=None, description="TCP States")
+    traffic_class: Optional[Global[List[int]]] = Field(
+        default=None,
+        serialization_alias="trafficClass",
+        validation_alias="trafficClass",
+        description="Select Traffic Class",
+    )
+    icmp6_msg: Optional[Global[List[Icmp6Msg]]] = Field(
+        default=None, serialization_alias="icmp6Msg", validation_alias="icmp6Msg", description="ICMP6 Message"
     )
 
 
-class ServiceChain(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    service_chain_number: Union[Global[ServiceChainNumber], Variable] = Field(
-        serialization_alias="serviceChainNumber", validation_alias="serviceChainNumber"
+class Ipv4AcceptAction(BaseModel):
+    """
+    Accept Action
+    """
+
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    vpn: Optional[Union[Global[int], Variable]] = None
-    fallback: Optional[Union[Global[bool], Variable, Default[bool]]] = None
-
-
-class AcceptActionIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    set_dscp: Optional[Global[int]] = Field(serialization_alias="setDscp", validation_alias="setDscp", default=None)
-    counter_name: Optional[Global[str]] = Field(
-        serialization_alias="counterName", validation_alias="counterName", default=None
+    set_dscp: Optional[Global[int]] = Field(
+        default=None, serialization_alias="setDscp", validation_alias="setDscp", description="DSCP number"
     )
-    log: Optional[Union[Global[bool], Default[bool]]] = None
-    set_next_hop: Optional[Global[str]] = Field(
-        serialization_alias="setNextHop", validation_alias="setNextHop", default=None
+    counter_name: Optional[Global[str]] = Field(
+        default=None, serialization_alias="counterName", validation_alias="counterName", description="Counter Name"
     )
-    set_service_chain: Optional[ServiceChain] = Field(
-        serialization_alias="setServiceChain", validation_alias="setServiceChain", default=None
+    log: Union[Global[bool], Default[bool]] = Field(default=as_default(False), description="Enable log")
+    set_next_hop: Optional[Global[IPv4Address]] = Field(
+        default=None,
+        serialization_alias="setNextHop",
+        validation_alias="setNextHop",
+        description="Set Next Hop (IPV4 address)",
+    )
+    mirror: Optional[ReferenceId] = Field(default=None, description="Select a Mirror Parcel UUID")
+    policer: Optional[ReferenceId] = Field(default=None, description="Select a Policer Parcel")
+
+
+class Ipv6AcceptAction(BaseModel):
+    """
+    Accept Action
+    """
+
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    mirror: Optional[Global[UUID]] = None
-    policer: Optional[Global[UUID]] = None
-
-
-class AcceptActionIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
     counter_name: Optional[Global[str]] = Field(
-        serialization_alias="counterName", validation_alias="counterName", default=None
-    )
-    log: Optional[Union[Global[bool], Default[bool]]] = None
-    set_next_hop: Optional[Global[str]] = Field(
-        serialization_alias="setNextHop", validation_alias="setNextHop", default=None
+        default=None, serialization_alias="counterName", validation_alias="counterName", description="Counter Name"
     )
-    set_service_chain: Optional[ServiceChain] = Field(
-        serialization_alias="setServiceChain", validation_alias="setServiceChain", default=None
+    log: Union[Global[bool], Default[bool]] = Field(default=as_default(False), description="Enable log")
+    set_next_hop: Optional[Global[IPv6Address]] = Field(
+        default=None,
+        serialization_alias="setNextHop",
+        validation_alias="setNextHop",
+        description="Set Next Hop (IPV6 address)",
     )
     set_traffic_class: Optional[Global[int]] = Field(
-        serialization_alias="setTrafficClass", validation_alias="setTrafficClass", default=None
+        default=None,
+        serialization_alias="setTrafficClass",
+        validation_alias="setTrafficClass",
+        description="set traffic class number",
     )
-    mirror: Optional[Global[UUID]] = None
-    policer: Optional[Global[UUID]] = None
+    mirror: Optional[ReferenceId] = Field(default=None, description="Select a Mirror Parcel UUID")
+    policer: Optional[ReferenceId] = Field(default=None, description="Select a Policer Parcel")
 
 
-class DropAction(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    counter_name: Optional[Global[str]] = Field(
-        serialization_alias="counterName", validation_alias="counterName", default=None
+class Ipv4AcceptActions(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    log: Optional[Union[Global[bool], Default[bool]]] = None
-
-
-class AcceptActionsIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    accept: AcceptActionIPv4
-
-
-class AcceptActionsIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    accept: AcceptActionIPv6
-
-
-class DropActions(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    accept: Ipv4AcceptAction = Field(..., description="Accept Action")
 
-    drop: DropAction
 
+class Ipv6AcceptActions(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    accept: Ipv6AcceptAction = Field(..., description="Accept Action")
 
-class IPv4SequenceBaseAction(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    sequence_id: Global[int] = Field(serialization_alias="sequenceId", validation_alias="sequenceId")
-    sequence_name: Global[str] = Field(serialization_alias="sequenceName", validation_alias="sequenceName")
-    base_action: Union[Global[Action], Default[Action]] = Field(
-        serialization_alias="baseAction", validation_alias="baseAction", default=Default[Action](value="accept")
+class DropAction(BaseModel):
+    """
+    Drop Action
+    """
+
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    match_entries: Optional[List[IPv4Match]] = Field(
-        serialization_alias="matchEntries", validation_alias="matchEntries", default=None
+    counter_name: Optional[Global[str]] = Field(
+        default=None, serialization_alias="counterName", validation_alias="counterName", description="Counter Name"
     )
+    log: Union[Global[bool], Default[bool]] = Field(default=as_default(False), description="Enable log")
 
 
-class IPv6SequenceBaseAction(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    sequence_id: Global[int] = Field(serialization_alias="sequenceId", validation_alias="sequenceId")
-    sequence_name: Global[str] = Field(serialization_alias="sequenceName", validation_alias="sequenceName")
-    base_action: Union[Global[Action], Default[Action]] = Field(
-        serialization_alias="baseAction", validation_alias="baseAction", default=Default[Action](value="accept")
-    )
-    match_entries: Optional[List[IPv6Match]] = Field(
-        serialization_alias="matchEntries", validation_alias="matchEntries", default=None
+class DropActions(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
+    drop: DropAction = Field(..., description="Drop Action")
 
 
-class IPv4SequenceActions(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    sequence_id: Global[int] = Field(serialization_alias="sequenceId", validation_alias="sequenceId")
-    sequence_name: Global[str] = Field(serialization_alias="sequenceName", validation_alias="sequenceName")
-    actions: List[Union[AcceptActionsIPv4, DropActions]] = Field(
-        serialization_alias="actions", validation_alias="actions"
+class Sequences(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    match_entries: Optional[List[IPv4Match]] = Field(
-        serialization_alias="matchEntries", validation_alias="matchEntries", default=None
+    sequence_id: Global[int] = Field(
+        ..., serialization_alias="sequenceId", validation_alias="sequenceId", description="Sequence Id"
     )
-
-
-class IPv6SequenceActions(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    sequence_id: Global[int] = Field(serialization_alias="sequenceId", validation_alias="sequenceId")
-    sequence_name: Global[str] = Field(serialization_alias="sequenceName", validation_alias="sequenceName")
-    actions: List[Union[AcceptActionsIPv6, DropActions]] = Field(
-        serialization_alias="actions", validation_alias="actions"
+    sequence_name: Global[str] = Field(
+        ..., serialization_alias="sequenceName", validation_alias="sequenceName", description="Sequence Name"
     )
-    match_entries: Optional[List[IPv6Match]] = Field(
-        serialization_alias="matchEntries", validation_alias="matchEntries", default=None
+    base_action: Optional[Union[Global[Action], Default[Action]]] = Field(
+        default=None, serialization_alias="baseAction", validation_alias="baseAction", description="Base Action"
+    )
+    match_entries: Optional[List[Ipv6MatchEntry]] = Field(
+        default=None,
+        serialization_alias="matchEntries",
+        validation_alias="matchEntries",
+        description="Define match conditions",
+        max_length=1,
+        min_length=1,
     )
 
+    @model_validator(mode="after")
+    def check_fields_at_least_one_assigned(self):
+        """There are two Sequence models in schema,
+        one with set base_action and empty actions,
+        and one with set actions and empty base_action,
+        so we combine two models into one model with check if
+        at least one field assigned
+        """
+        if self.base_action is None and self.actions is None:
+            self.base_action = as_default("accept", Action)
 
-class IPv4AclData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    defautl_action: Union[Global[Action], Default[Action]] = Field(
-        serialization_alias="defaultAction", validation_alias="defaultAction", default=Default[Action](value="drop")
+class Ipv6Sequences(Sequences):
+    actions: Optional[List[Union[Ipv6AcceptActions, DropActions]]] = Field(
+        default=None, description="Define list of actions", max_length=1, min_length=1
     )
-    sequences: List[Union[IPv4SequenceBaseAction, IPv4SequenceActions]]
-
-
-class IPv4AclCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    name: str
-    description: Optional[str] = None
-    data: IPv4AclData
 
+class Ipv4Sequences(Sequences):
+    actions: Optional[List[Union[Ipv4AcceptActions, DropActions]]] = Field(
+        default=None, description="Define list of actions", max_length=1, min_length=1
+    )
 
-class IPv6AclData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    defautl_action: Union[Global[Action], Default[Action]] = Field(
-        serialization_alias="defaultAction", validation_alias="defaultAction", default=Default[Action](value="drop")
+class Ipv4AclParcel(_ParcelBase):
+    type_: Literal["ipv4-acl"] = Field(default="ipv4-acl", exclude=True)
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    default_action: Union[Global[Action], Global[Action]] = Field(
+        as_default("drop", Action),
+        validation_alias=AliasPath("data", "defaultAction"),
+        description="Default Action",
+    )
+    sequences: List[Union[Ipv4Sequences]] = Field(
+        default_factory=list, validation_alias=AliasPath("data", "sequences"), description="Access Control List"
     )
-    sequences: List[Union[IPv6SequenceBaseAction, IPv6SequenceActions]]
-
 
-class IPv6AclCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    name: str
-    description: Optional[str] = None
-    data: IPv6AclData
+class Ipv6AclParcel(_ParcelBase):
+    type_: Literal["ipv6-acl"] = Field(default="ipv6-acl", exclude=True)
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    default_action: Union[Global[Action], Global[Action]] = Field(
+        as_default("drop", Action),
+        validation_alias=AliasPath("data", "defaultAction"),
+        description="Default Action",
+    )
+    sequences: List[Union[Ipv6Sequences]] = Field(
+        default_factory=list, validation_alias=AliasPath("data", "sequences"), description="Access Control List"
+    )
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,235 +1,172 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Address, IPv6Interface
 from typing import List, Literal, Optional, Union
+from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.configuration.feature_profile.common import Arp, StaticIPv4Address, StaticIPv6Address
+from catalystwan.models.configuration.feature_profile.sdwan.service.lan.common import (
+    VrrpIPv6Address,
+    VrrpTrackingObject,
+)
 
-VirtualApplicationType = Literal["dreopt"]
 
-ResourceProfile = Literal[
-    "small",
-    "medium",
-    "large",
-    "extra-large",
-    "default",
-]
+class VrrpIPv4SecondaryAddress(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-AppqoeDeviceRole = Literal[
-    "forwarder",
-    "forwarderAndServiceNode",
-    "serviceNode",
-    "serviceNodeWithDre",
-    "forwarderAndServiceNodeWithDre",
-]
+    address: Union[Variable, Global[str]]
 
-AppnavControllerGroupName = Literal["ACG-APPQOE"]
-ServiceNodeGroupName = Literal["SNG-APPQOE"]
-ForwarderAndServiceNodeAddress = Literal["192.168.2.2"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
-ForwarderAndServiceNodeControllerAddress = Literal[
-    "192.168.2.1"
-]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
-ServiceNodeExternalAddress = Literal["192.168.2.2"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
-ServiceNodeExternalVpgIp = Literal["192.168.2.1/24"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
 
+class VrrpIPv6SecondaryAddress(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-class VirtualApplication(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    prefix: Union[Global[str], Global[IPv6Interface], Variable]
 
-    instance_id: Global[int] = Field(
-        default=Global(value=1), serialization_alias="instanceId", validation_alias="instanceId"
+
+class VrrpIPv4(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    group_id: Union[Variable, Global[int]] = Field(serialization_alias="groupId", validation_alias="groupId")
+    priority: Union[Variable, Global[int], Default[int]] = Default[int](value=100)
+    timer: Union[Variable, Global[int], Default[int]] = Default[int](value=1000)
+    track_omp: Union[Global[bool], Default[bool]] = Field(
+        serialization_alias="trackOmp", validation_alias="trackOmp", default=Default[bool](value=False)
     )
-    application_type: Global[VirtualApplicationType] = Field(
-        default=Global[VirtualApplicationType](value="dreopt"),
-        serialization_alias="applicationType",
-        validation_alias="applicationType",
+    ip_address: Union[Global[str], Global[IPv4Address], Variable] = Field(
+        serialization_alias="ipAddress", validation_alias="ipAddress"
     )
-    resource_profile: Union[Global[ResourceProfile], Default[str]] = Field(
-        default=Global[ResourceProfile](value="default"),
-        serialization_alias="resourceProfile",
-        validation_alias="resourceProfile",
+    ip_address_secondary: Optional[List[VrrpIPv4SecondaryAddress]] = Field(
+        serialization_alias="ipAddressSecondary", validation_alias="ipAddressSecondary", default=None
     )
-
-
-class Appqoe(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: Default[str] = Default(value="/1")
-    appnav_controller_group: Global[AppnavControllerGroupName] = Field(
-        default=Global[AppnavControllerGroupName](value="ACG-APPQOE"),
-        serialization_alias="appnavControllerGroup",
-        validation_alias="appnavControllerGroup",
+    tloc_pref_change: Union[Global[bool], Default[bool]] = Field(
+        serialization_alias="tlocPrefChange", validation_alias="tlocPrefChange", default=Default[bool](value=False)
     )
-    service_node_group: Global[ServiceNodeGroupName] = Field(
-        default=Global[ServiceNodeGroupName](value="SNG-APPQOE"),
-        serialization_alias="serviceNodeGroup",
-        validation_alias="serviceNodeGroup",
+    tloc_pref_change_value: Optional[Union[Global[int], Variable]] = Field(
+        serialization_alias="tlocPrefChangeValue", validation_alias="tlocPrefChangeValue", default=None
     )
-    service_node_groups: List[Global[ServiceNodeGroupName]] = Field(
-        default=[Global[ServiceNodeGroupName](value="SNG-APPQOE")],
-        serialization_alias="serviceNodeGroups",
-        validation_alias="serviceNodeGroups",
+    tracking_object: Optional[List[VrrpTrackingObject]] = Field(
+        serialization_alias="trackingObject", validation_alias="trackingObject", default=None
     )
-    enable: Global[bool] = Global[bool](value=True)
-    vpn: Union[Global[int], Default[None], Variable] = Field(default=Global[int](value=0))
 
+    prefix_list: Optional[Union[Global[str], Variable, Default[None]]] = Default[None](value=None)
 
-class ServiceContext(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True)
-    appqoe: List[Appqoe]
 
+class VrrpIPv6(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-# Frowarder
-
-
-class ServiceNodeInformation(BaseModel):
-    address: Global[str]
+    group_id: Union[Variable, Global[int]] = Field(serialization_alias="groupId", validation_alias="groupId")
+    priority: Union[Variable, Global[int], Default[int]] = Default[int](value=100)
+    timer: Union[Variable, Global[int], Default[int]] = Default[int](value=1000)
+    track_omp: Union[Global[bool], Default[bool]] = Field(
+        serialization_alias="trackOmp", validation_alias="trackOmp", default=Default[bool](value=False)
+    )
+    track_prefix_list: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="trackPrefixList", validation_alias="trackPrefixList"
+    )
+    ipv6: List[VrrpIPv6Address]
+    ipv6_secondary: Optional[List[VrrpIPv6SecondaryAddress]]
 
 
-class ForwarderController(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class Dhcpv6Helper(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    address: Union[Global[str], Variable]
-    vpn: Global[int] = Global[int](value=1)
+    address: Union[Global[str], Variable] = Field(serialization_alias="address", validation_alias="address")
+    vpn: Optional[Union[Global[int], Variable, Default[None]]] = None
 
 
-class ForwarderAppnavControllerGroup(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class AdvancedSviAttributes(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    group_name: Default[AppnavControllerGroupName] = Field(
-        default=Default(value="ACG-APPQOE"), serialization_alias="groupName", validation_alias="groupName"
+    tcp_mss: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="tcpMss", validation_alias="tcpMss", default=Default[None](value=None)
     )
-    appnav_controllers: List[ForwarderController] = Field(
-        serialization_alias="appnavControllers", validation_alias="appnavControllers"
+    arp_timeout: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="arpTimeout", validation_alias="arpTimeout", default=Default[int](value=1200)
     )
-
-
-class ForwarderNodeGroup(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: Union[Global[str], Default[ServiceNodeGroupName]]
-    internal: Default[bool] = Default[bool](value=False)
-    service_node: List[ServiceNodeInformation] = Field(
-        serialization_alias="serviceNode", validation_alias="serviceNode"
+    ip_directed_broadcast: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="ipDirectedBroadcast",
+        validation_alias="ipDirectedBroadcast",
+        default=Default[bool](value=False),
+    )
+    icmp_redirect_disable: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="icmpRedirectDisable",
+        validation_alias="icmpRedirectDisable",
+        default=Default[bool](value=True),
     )
 
 
-class ForwarderRole(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class IPv4AddressConfiguration(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    appnav_controller_group: List[ForwarderAppnavControllerGroup] = Field(
-        serialization_alias="appnavControllerGroup", validation_alias="appnavControllerGroup"
+    address: StaticIPv4Address = Field(serialization_alias="addressV4", validation_alias="addressV4")
+    secondary_address: Optional[List[StaticIPv4Address]] = Field(
+        serialization_alias="secondaryAddressV4", validation_alias="secondaryAddressV4", default=None
     )
-    service_node_group: List[ForwarderNodeGroup] = Field(
-        serialization_alias="serviceNodeGroup", validation_alias="serviceNodeGroup"
+    dhcp_helper: Optional[Union[Global[List[str]], Variable, Default[None]]] = Field(
+        serialization_alias="dhcpHelperV4", validation_alias="dhcpHelperV4", default=None
     )
-    service_context: ServiceContext = Field(serialization_alias="serviceContext", validation_alias="serviceContext")
-
-
-# Forwarder and Service
 
 
-class ServiceNodeInformationDefault(BaseModel):
-    address: Default[ForwarderAndServiceNodeAddress] = Default[ForwarderAndServiceNodeAddress](value="192.168.2.2")
+class IPv6AddressConfiguration(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-
-class ForwarderAndServiceNodeController(BaseModel):
-    address: Default[ForwarderAndServiceNodeControllerAddress] = Default[ForwarderAndServiceNodeControllerAddress](
-        value="192.168.2.1"
+    address: Union[Global[str], Global[IPv6Interface], Variable, Default[None]] = Field(
+        serialization_alias="addressV6", validation_alias="addressV6"
     )
-
-
-class ForwarderAndServiceNodeAppnavControllerGroup(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    group_name: Default[AppnavControllerGroupName] = Field(
-        default=Default[AppnavControllerGroupName](value="ACG-APPQOE"),
-        serialization_alias="groupName",
-        validation_alias="groupName",
+    secondary_address: Optional[List[StaticIPv6Address]] = Field(
+        serialization_alias="secondaryAddressV6", validation_alias="secondaryAddressV6", default=None
     )
-    appnav_controllers: List[ForwarderAndServiceNodeController] = Field(
-        serialization_alias="appnavControllers", validation_alias="appnavControllers"
+    dhcp_helper: Optional[List[Dhcpv6Helper]] = Field(
+        serialization_alias="dhcpHelperV6", validation_alias="dhcpHelperV6", default=None
     )
 
 
-class ForwarderAndServiceNodeGroup(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class AclQos(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    name: Default[ServiceNodeGroupName] = Default[ServiceNodeGroupName](value="SNG-APPQOE")
-    internal: Default[bool] = Default[bool](value=True)
-    service_node: List[ServiceNodeInformationDefault] = Field(
-        serialization_alias="serviceNode", validation_alias="serviceNode"
+    ipv4_acl_egress: Optional[Global[UUID]] = Field(
+        serialization_alias="ipv4AclEgress", validation_alias="ipv4AclEgress", default=None
     )
-
-
-class ForwarderAndServiceNodeRole(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    appnav_controller_group: List[ForwarderAndServiceNodeAppnavControllerGroup] = Field(
-        serialization_alias="appnavControllerGroup", validation_alias="appnavControllerGroup"
+    ipv4_acl_ingress: Optional[Global[UUID]] = Field(
+        serialization_alias="ipv4AclIngress", validation_alias="ipv4AclIngress", default=None
     )
-    service_node_group: List[ForwarderAndServiceNodeGroup] = Field(
-        serialization_alias="serviceNodeGroup", validation_alias="serviceNodeGroup"
+    ipv6_acl_egress: Optional[Global[UUID]] = Field(
+        serialization_alias="ipv6AclEgress", validation_alias="ipv6AclEgress", default=None
     )
-
-    service_context: ServiceContext = Field(serialization_alias="serviceContext", validation_alias="serviceContext")
-
-
-# Service
-
-
-class ServiceNodeInformationExternal(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    address: Default[ServiceNodeExternalAddress] = Default[ServiceNodeExternalAddress](value="192.168.2.2")
-    vpg_ip: Default[ServiceNodeExternalVpgIp] = Field(
-        default=Default[ServiceNodeExternalVpgIp](value="192.168.2.1"),
-        serialization_alias="vpgIp",
-        validation_alias="vpgIp",
+    ipv6_acl_ingress: Optional[Global[UUID]] = Field(
+        serialization_alias="ipv6AclIngress", validation_alias="ipv6AclIngress", default=None
     )
 
 
-class ServiceNodeGroup(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class InterfaceSviParcel(_ParcelBase):
+    type_: Literal["lan/vpn/interface/svi"] = Field(default="lan/vpn/interface/svi", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    name: Default[ServiceNodeGroupName] = Default[ServiceNodeGroupName](value="SNG-APPQOE")
-    external_node: Default[bool] = Field(
-        default=Default[bool](value=True), serialization_alias="externalNode", validation_alias="externalNode"
+    shutdown: Union[Global[bool], Variable, Default[bool]] = Field(
+        default=Default[bool](value=True), validation_alias=AliasPath("data", "shutdown")
     )
-    service_node: List[ServiceNodeInformationExternal] = Field(
-        default=[ServiceNodeInformationExternal()], serialization_alias="serviceNode", validation_alias="serviceNode"
+    interface_name: Union[Global[str], Variable] = Field(validation_alias=AliasPath("data", "interfaceName"))
+    svi_description: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        default=Default[None](value=None), validation_alias=AliasPath("data", "description")
     )
-
-
-class ServiceNodeRole(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    service_node_group: List[ServiceNodeGroup] = Field(
-        default=[ServiceNodeGroup()], serialization_alias="serviceNodeGroup", validation_alias="serviceNodeGroup"
+    interface_mtu: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "ifMtu"), default=Default[int](value=1500)
     )
-
-
-class AppqoeData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    dreopt: Optional[Union[Global[bool], Default[bool]]] = Default[bool](value=False)
-    virtual_application: Optional[List[VirtualApplication]] = Field(
-        serialization_alias="virtualApplication", validation_alias="virtualApplication"
+    ip_mtu: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "ipMtu"), default=Default[int](value=1500)
     )
-    appqoe_device_role: Global[str] = Field(
-        default=Global(value="forwarder"), serialization_alias="appqoeDeviceRole", validation_alias="appqoeDeviceRole"
+    ipv4: Optional[IPv4AddressConfiguration] = Field(default=None, validation_alias=AliasPath("data", "ipv4"))
+    ipv6: Optional[IPv6AddressConfiguration] = Field(default=None, validation_alias=AliasPath("data", "ipv6"))
+    acl_qos: Optional[AclQos] = Field(validation_alias=AliasPath("data", "aclQos"), default=None)
+    arp: Optional[List[Arp]] = Field(default=None, validation_alias=AliasPath("data", "arp"))
+    vrrp: Optional[List[VrrpIPv4]] = Field(default=None, validation_alias=AliasPath("data", "vrrp"))
+    vrrp_ipv6: Optional[List[VrrpIPv6]] = Field(validation_alias=AliasPath("data", "vrrpIpv6"), default=None)
+    dhcp_client_v6: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        validation_alias=AliasPath("data", "dhcpClientV6"), default=Default[bool](value=False)
     )
-
-    forwarder: Optional[ForwarderRole]
-    forwarder_and_service_node: Optional[ForwarderAndServiceNodeRole] = Field(
-        serialization_alias="forwarderAndServiceNode", validation_alias="forwarderAndServiceNode"
+    advanced: AdvancedSviAttributes = Field(
+        default_factory=AdvancedSviAttributes, validation_alias=AliasPath("data", "advanced")
     )
-    service_node: Optional[ServiceNodeRole] = Field(serialization_alias="serviceNode", validation_alias="serviceNode")
-
-
-class AppqoeCreationPayload(BaseModel):
-    name: str
-    description: Optional[str] = None
-    data: AppqoeData
-    metadata: Optional[dict] = None
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.common import Prefix
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask
 
 
 class AggregatePrefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    prefix: Prefix
+    prefix: AddressWithMask
     as_set: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="asSet", validation_alias="asSet", default=Default[bool](value=False)
     )
     summary_only: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="summaryOnly", validation_alias="summaryOnly", default=Default[bool](value=False)
     )
 
 
 class AggregatePrefixIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     prefix: Union[Global[str], Variable]
     as_set: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="asSet", validation_alias="asSet", default=Default[bool](value=False)
     )
     summary_only: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="summaryOnly", validation_alias="summaryOnly", default=Default[bool](value=False)
     )
 
 
 class NetworkPrefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    prefix: Prefix
+    prefix: AddressWithMask
 
 
 class NetworkPrefixIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     prefix: Union[Global[str], Variable]
 
 
 RedistributeProtocol = Literal[
     "static",
     "connected",
@@ -61,70 +61,70 @@
     "connected",
     "omp",
     "ospf",
 ]
 
 
 class RedistributedRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     protocol: Union[Global[RedistributeProtocol], Variable]
     route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="routePolicy", validation_alias="routePolicy"
     )
 
 
 class RedistributedRouteIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     protocol: Union[Global[RedistributeProtocolIPv6], Variable]
     route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="routePolicy", validation_alias="routePolicy"
     )
 
 
 class AddressFamilyIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     aggregate_address: Optional[List[AggregatePrefix]] = Field(
         serialization_alias="aggregateAddress", validation_alias="aggregateAddress"
     )
     network: Optional[List[NetworkPrefix]] = None
     paths: Optional[Union[Global[int], Variable, Default[None]]] = None
     originate: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     name: Optional[Union[Default[None], Global[UUID]]] = None
     filter: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     redistribute: Optional[List[RedistributedRoute]] = None
 
 
 class PolicyType(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     policy_type: Global[str] = Field(serialization_alias="policyType", validation_alias="policyType")
 
 
 class PolicyTypeWithThreshold(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     policy_type: Global[str] = Field(serialization_alias="policyType", validation_alias="policyType")
     prefix_number: Union[Global[int], Variable] = Field(serialization_alias="prefixNum", validation_alias="prefixNum")
     threshold: Union[Global[int], Variable, Default[int]] = Default[int](value=75)
 
 
 class PolicyTypeWithRestart(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     policy_type: Global[str] = Field(serialization_alias="policyType", validation_alias="policyType")
     prefix_number: Union[Global[int], Variable] = Field(serialization_alias="prefixNum", validation_alias="prefixNum")
     threshold: Union[Global[int], Variable, Default[int]] = Default[int](value=75)
     restart_interval: Union[Global[int], Variable]
 
 
 class AddressFamilyIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     aggregate_address: Optional[List[AggregatePrefixIPv6]] = Field(
         serialization_alias="ipv6AggregateAddress", validation_alias="ipv6AggregateAddress"
     )
     network: Optional[List[NetworkPrefixIPv6]] = Field(
         serialization_alias="ipv6Network", validation_alias="ipv6Network"
     )
@@ -132,30 +132,30 @@
     originate: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     name: Optional[Union[Default[None], Global[UUID]]] = None
     filter: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     redistribute: Optional[List[RedistributedRouteIPv6]] = None
 
 
 class BgpAddressFamily(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     family_type: Global[str] = Field(serialization_alias="familyType", validation_alias="familyType")
     max_prefix_config: Optional[Union[PolicyType, PolicyTypeWithRestart, PolicyTypeWithThreshold]] = Field(
         serialization_alias="maxPrefixConfig", validation_alias="maxPrefixConfig"
     )
     in_route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="inRoutePolicy", validation_alias="inRoutePolicy"
     )
     out_route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="outRoutePolicy", validation_alias="outRoutePolicy"
     )
 
 
 class BgpIPv4Neighbor(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     address: Union[Global[str], Variable]
     description: Optional[Union[Global[str], Variable, Default[None]]] = None
     shutdown: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     remote_as: Union[Global[int], Variable] = Field(serialization_alias="remoteAs", validation_alias="remoteAs")
     local_as: Union[Global[int], Variable] = Field(
         serialization_alias="localAs", validation_alias="localAs", default=None
@@ -189,15 +189,15 @@
     )
     address_family: Optional[BgpAddressFamily] = Field(
         serialization_alias="addressFamily", validation_alias="addressFamily"
     )
 
 
 class BgpIPv6Neighbor(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     address: Union[Global[str], Variable]
     description: Optional[Union[Global[str], Variable, Default[None]]] = None
     shutdown: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     remote_as: Union[Global[int], Variable] = Field(serialization_alias="remoteAs", validation_alias="remoteAs")
     local_as: Union[Global[int], Variable] = Field(
         serialization_alias="localAs", validation_alias="localAs", default=None
@@ -230,59 +230,61 @@
         serialization_alias="asNumber", validation_alias="asNumber", default=None
     )
     address_family: Optional[BgpAddressFamily] = Field(
         serialization_alias="addressFamily", validation_alias="addressFamily"
     )
 
 
-class BgpData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    as_num: Union[Global[int], Variable] = Field(serialization_alias="asNum", validation_alias="asNum")
+class BgpParcel(_ParcelBase):
+    type_: Literal["routing/bgp"] = Field(default="routing/bgp", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+    as_num: Union[Global[int], Variable] = Field(validation_alias=AliasPath("data", "asNum"))
     router_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="routerId", validation_alias="routerId", default=None
+        validation_alias=AliasPath("data", "routerId"), default=None
     )
     propagate_aspath: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="propagateAspath", validation_alias="propagateAspath", default=Default[bool](value=False)
+        validation_alias=AliasPath("data", "propagateAspath"), default=Default[bool](value=False)
     )
     propagate_community: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="propagateCommunity",
-        validation_alias="propagateCommunity",
+        validation_alias=AliasPath("data", "propagateCommunity"),
         default=Default[bool](value=False),
     )
-    external: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=20)
-    internal: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=200)
-    local: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=20)
-    keepalive: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=60)
-    holdtime: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=180)
+    external: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "external"), default=Default[int](value=20)
+    )
+    internal: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "internal"), default=Default[int](value=200)
+    )
+    local: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "local"), default=Default[int](value=20)
+    )
+    keepalive: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "keepalive"), default=Default[int](value=60)
+    )
+    holdtime: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "holdtime"), default=Default[int](value=180)
+    )
     always_compare: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="alwaysCompare", validation_alias="alwaysCompare", default=Default[bool](value=False)
+        validation_alias=AliasPath("data", "alwaysCompare"), default=Default[bool](value=False)
+    )
+    deterministic: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        validation_alias=AliasPath("data", "deterministic"), default=Default[bool](value=False)
     )
-    deterministic: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
     missing_as_worst: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="missingAsWorst", validation_alias="missingAsWorst", default=Default[bool](value=False)
+        validation_alias=AliasPath("data", "missingAsWorst"), default=Default[bool](value=False)
     )
     compare_router_id: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="compareRouterId", validation_alias="compareRouterId", default=Default[bool](value=False)
+        validation_alias=AliasPath("data", "compareRouterId"), default=Default[bool](value=False)
     )
     multipath_relax: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="multipathRelax", validation_alias="multipathRelax", default=Default[bool](value=False)
+        validation_alias=AliasPath("data", "multipathRelax"), default=Default[bool](value=False)
     )
-    neighbor: Optional[List[BgpIPv4Neighbor]] = None
+    neighbor: Optional[List[BgpIPv4Neighbor]] = Field(validation_alias=AliasPath("data", "neighbor"), default=None)
     ipv6_neighbor: Optional[List[BgpIPv6Neighbor]] = Field(
-        serialization_alias="ipv6Neighbor", validation_alias="ipv6Neighbor", default=None
+        validation_alias=AliasPath("data", "ipv6Neighbor"), default=None
     )
     address_family: Optional[AddressFamilyIPv4] = Field(
-        serialization_alias="addressFamily", validation_alias="addressFamily", default=None
+        validation_alias=AliasPath("data", "addressFamily"), default=None
     )
     ipv6_address_family: Optional[AddressFamilyIPv6] = Field(
-        serialization_alias="ipv6AddressFamily", validation_alias="ipv6AddressFamily", default=None
+        validation_alias=AliasPath("data", "ipv6AddressFamily"), default=None
     )
-
-
-class BgpCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: BgpData
-    metadata: Optional[dict] = None
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,74 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
+from __future__ import annotations
 
-from typing import List, Optional, Union
+from typing import List, Literal, Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default
 
+EnableMrfMigration = Literal["enabled", "enabled-from-bgp-core"]
+Role = Literal["edge-router", "border-router"]
 
-class OptionCodeAscii(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    code: Union[Global[int], Variable]
-    ascii: Union[Global[str], Variable]
-
-
-class OptionCodeHex(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    code: Union[Global[int], Variable]
-    hex: Union[Global[str], Variable]
-
-
-class OptionCodeIP(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    code: Union[Global[int], Variable]
-    ip: Union[Global[List[str]], Variable]
-
-
-class StaticLease(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    mac_address: Union[Global[str], Variable] = Field(serialization_alias="macAddress", validation_alias="macAddress")
-    ip: Union[Global[str], Variable]
-
-
-class DhcpAddressPool(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    network_address: Union[Global[str], Variable] = Field(
-        serialization_alias="networkAddress", validation_alias="networkAddress"
+class ManagementRegion(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    vrf_id: Union[Global[int], Default[None], Variable] = Field(
+        default=Default[None](value=None),
+        serialization_alias="vrfId",
+        validation_alias="vrfId",
+        description="VRF name for management region",
+    )
+    gateway_preference: Optional[Union[Global[List[int]], Default[None], Variable]] = Field(
+        default=Default[None](value=None),
+        serialization_alias="gatewayPreference",
+        validation_alias="gatewayPreference",
+        description="List of affinity group preferences for VRF",
+    )
+    management_gateway: Union[Global[bool], Default[bool], Variable] = Field(
+        default=as_default(False),
+        serialization_alias="managementGateway",
+        validation_alias="managementGateway",
+        description="Enable management gateway",
     )
-    subnet_mask: Union[Global[str], Variable] = Field(serialization_alias="subnetMask", validation_alias="subnetMask")
 
 
-class DhcpServerData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class MRFParcel(_ParcelBase):
+    type_: Literal["mrf"] = Field(default="mrf", exclude=True)
 
-    address_pool: DhcpAddressPool = Field(serialization_alias="addressPool", validation_alias="addressPool")
-    exclude: Optional[Union[Global[List[str]], Variable, Default[None]]] = None
-    lease_time: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="leaseTime", validation_alias="leaseTime", default=Default[int](value=86400)
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    interface_mtu: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="interfaceMtu", validation_alias="interfaceMtu", default=None
+    secondary_region: Union[Global[int], Variable, Default[None]] = Field(
+        default=Default[None](value=None),
+        validation_alias=AliasPath("data", "secondaryRegion"),
+        description="Set secondary region ID",
     )
-    domain_name: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="domainName", validation_alias="domainName", default=None
+    role: Union[Global[Role], Variable, Default[None]] = Field(
+        default=Default[None](value=None),
+        validation_alias=AliasPath("data", "role"),
+        description="Set the role for router",
     )
-    default_gateway: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="defaultGateway", validation_alias="defaultGateway", default=None
+    enable_mrf_migration: Union[Global[EnableMrfMigration], Default[None]] = Field(
+        default=Default[None](value=None),
+        validation_alias=AliasPath("data", "enableMrfMigration"),
+        description="Enable migration mode to Multi-Region Fabric",
     )
-    dns_servers: Optional[Union[Global[List[str]], Variable, Default[None]]] = Field(
-        serialization_alias="dnsServers", validation_alias="dnsServers", default=None
+    migration_bgp_community: Optional[Union[Global[int], Default[None]]] = Field(
+        default=Default[None](value=None),
+        validation_alias=AliasPath("data", "migrationBgpCommunity"),
+        description="Set BGP community during migration from BGP-core based network",
     )
-    tftp_servers: Optional[Union[Global[List[str]], Variable, Default[None]]] = Field(
-        serialization_alias="tftpServers", validation_alias="tftpServers", default=None
+    enable_management_region: Union[Global[bool], Default[bool], Variable] = Field(
+        default=as_default(False),
+        validation_alias=AliasPath("data", "enableManagementRegion"),
+        description="Enable management region",
     )
-    static_lease: Optional[List[StaticLease]] = Field(
-        serialization_alias="staticLease", validation_alias="staticLease", default=None
+    management_region: ManagementRegion = Field(
+        default_factory=ManagementRegion,
+        validation_alias=AliasPath("data", "managementRegion"),
+        description="Management Region",
     )
-    option_code: Optional[List[Union[OptionCodeAscii, OptionCodeHex, OptionCodeIP]]] = Field(
-        serialization_alias="optionCode", validation_alias="optionCode", default=None
-    )
-
-
-class DhcpSeverCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: DhcpServerData
-    metadata: Optional[dict] = None
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.common import Prefix
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask
 
 EigrpAuthType = Literal[
     "md5",
     "hmac-sha-256",
 ]
 
 
@@ -22,85 +22,81 @@
     "ospf",
     "ospfv3",
     "static",
 ]
 
 
 class KeychainDetails(BaseModel):
-    key_id: Union[Global[int], Variable, Default[None]] = Field(serialization_alias="keyId", validation_alias="keyId")
-    keystring: Union[Global[str], Variable, Default[None]]
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    key_id: Union[Global[int], Variable, Default[None]] = Field(
+        default=Default[None](value=None), serialization_alias="keyId", validation_alias="keyId"
+    )
+    keystring: Union[Global[str], Variable, Default[None]] = Field(default=Default[None](value=None))
 
 
 class EigrpAuthentication(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    auth_type: Union[Global[EigrpAuthType], Variable, Default[None]] = Field(
-        serialization_alias="type", validation_alias="type"
-    )
+    auth_type: Union[Global[EigrpAuthType], Variable, Default[None]] = Default[None](value=None)
     auth_key: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="authKey", validation_alias="authKey"
+        serialization_alias="authKey", validation_alias="authKey", default=Default[None](value=None)
     )
-    key: Optional[List[KeychainDetails]] = Field(serialization_alias="key", validation_alias="key")
+    key: Optional[List[KeychainDetails]] = None
 
 
 class TableMap(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     name: Optional[Union[Default[None], Global[UUID]]] = Default[None](value=None)
     filter: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
 
 
 class SummaryAddress(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    prefix: Prefix
+    prefix: AddressWithMask
 
 
 class IPv4StaticRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     name: Union[Global[str], Variable]
-    shutdown: Optional[Union[Global[int], Variable, Default[bool]]] = Default[bool](value=False)
-    summary_address: Optional[List[SummaryAddress]] = Field(
-        serialization_alias="summaryAddress", validation_alias="summaryAddress"
+    shutdown: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
+    summary_address: List[SummaryAddress] = Field(
+        serialization_alias="summaryAddress", validation_alias="summaryAddress", default_factory=list
     )
 
 
 class RedistributeIntoEigrp(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     protocol: Union[Global[RedistributeProtocol], Variable]
     route_policy: Optional[Union[Default[None], Global[UUID]]] = Default[None](value=None)
 
 
 class AddressFamily(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     redistribute: Optional[List[RedistributeIntoEigrp]] = None
-    network: List[SummaryAddress]
+    network: List[SummaryAddress] = Field(min_length=1)
 
 
-class EigrpData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class EigrpParcel(_ParcelBase):
+    type_: Literal["routing/eigrp"] = Field(default="routing/eigrp", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    as_number: Union[Global[int], Variable] = Field(serialization_alias="asNum", validation_alias="asNum")
-    address_family: AddressFamily = Field(serialization_alias="addressFamily", validation_alias="addressFamily")
+    as_number: Union[Global[int], Variable] = Field(validation_alias=AliasPath("data", "asNum"))
+    address_family: AddressFamily = Field(validation_alias=AliasPath("data", "addressFamily"))
     hello_interval: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="helloInterval", validation_alias="helloInterval", default=Default[int](value=5)
+        validation_alias=AliasPath("data", "helloInterval"), default=Default[int](value=5)
     )
     hold_time: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="holdTime", validation_alias="holdTime", default=Default[int](value=15)
+        validation_alias=AliasPath("data", "holdTime"), default=Default[int](value=15)
+    )
+    authentication: Optional[EigrpAuthentication] = Field(
+        validation_alias=AliasPath("data", "authentication"), default=None
     )
-    authentication: Optional[EigrpAuthentication] = None
     af_interface: Optional[List[IPv4StaticRoute]] = Field(
-        serialization_alias="afInterface", validation_alias="afInterface", default=None
+        validation_alias=AliasPath("data", "afInterface"), default=None
     )
-    table_map: TableMap = Field(serialization_alias="tableMap", validation_alias="tableMap", default=TableMap())
-
-
-class EigrpCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: EigrpData
-    metadata: Optional[dict] = None
+    table_map: TableMap = Field(validation_alias=AliasPath("data", "tableMap"), default=TableMap())
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,114 +1,84 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import Literal, Optional, Union
+from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
 
-IkeMode = Literal[
-    "main",
-    "aggresive",
+ObjectTrackerType = Literal[
+    "Interface",
+    "SIG",
+    "Route",
 ]
 
-IkeCiphersuite = Literal[
-    "aes256-cbc-sha1",
-    "aes256-cbc-sha2",
-    "aes128-cbc-sha1",
-    "aes128-cbc-sha2",
-]
 
-IkeGroup = Literal[
-    "2",
-    "14",
-    "15",
-    "16",
-    "19",
-    "20",
-    "21",
-    "24",
+Criteria = Literal[
+    "and",
+    "or",
 ]
 
-IpsecCiphersuite = Literal[
-    "aes256-cbc-sha1",
-    "aes256-cbc-sha384",
-    "aes256-cbc-sha256",
-    "aes256-cbc-sha512",
-    "aes256-gcm",
-    "null-sha1",
-    "null-sha384",
-    "null-sha256",
-    "null-sha512",
-]
 
-PfsGroup = Literal[
-    "group-1",
-    "group-2",
-    "group-5",
-    "group-14",
-    "group-15",
-    "group-16",
-    "group-19",
-    "group-20",
-    "group-21",
-    "group-24",
-    "none",
-]
+class SigTracker(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-TunnelApplication = Literal[
-    "none",
-    "sig",
-]
-
-VrrpTrackerAction = Literal[
-    "Decrement",
-    "Shutdown",
-]
+    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
+    object_tracker_type: Global[ObjectTrackerType] = Field(
+        serialization_alias="objectTrackerType",
+        validation_alias="objectTrackerType",
+        default=Global[ObjectTrackerType](value="SIG"),
+    )
 
 
-class Arp(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class InterfaceTracker(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    ip_address: Union[Variable, Global[str], Default[None]]
-    mac_address: Union[Global[str], Variable]
+    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
+    object_tracker_type: Global[ObjectTrackerType] = Field(
+        serialization_alias="objectTrackerType",
+        validation_alias="objectTrackerType",
+        default=Global[ObjectTrackerType](value="Interface"),
+    )
+    interface: Union[Global[str], Variable]
 
 
-class VrrpTrackingObject(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class RouteTracker(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    tracker_id: Union[Default[None], Global[UUID]] = Field(
-        serialization_alias="trackerId", validation_alias="trackerId"
-    )
-    tracker_action: Union[Global[VrrpTrackerAction], Variable] = Field(
-        serialization_alias="trackerAction", validation_alias="trackerAction"
+    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
+    object_tracker_type: Global[ObjectTrackerType] = Field(
+        serialization_alias="objectTrackerType",
+        validation_alias="objectTrackerType",
+        default=Global[ObjectTrackerType](value="Route"),
     )
-    decrement_value: Optional[Union[Variable, Global[int]]] = Field(
-        serialization_alias="decrementValue", validation_alias="decrementValue", default=None
+    route_ip: Union[Global[str], Variable] = Field(serialization_alias="routeIp", validation_alias="routeIp")
+    route_mask: Union[Global[str], Variable, Default[str]] = Field(
+        serialization_alias="routeMask", validation_alias="routeMask"
     )
+    vpn: Union[Global[int], Variable, Default[None]] = Default[None](value=None)
 
 
-class VrrpIPv6Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ObjectTrackerCreationPayload(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    ipv6_link_local: Union[Global[str], Variable] = Field(
-        serialization_alias="ipv6LinkLocal", validation_alias="ipv6LinkLocal"
-    )
-    prefix: Optional[Union[Global[str], Variable, Default[None]]] = None
+    name: str
+    description: Optional[str] = None
+    data: Union[InterfaceTracker, RouteTracker, SigTracker]
 
 
-class StaticIPv4Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ObjectTrackerRef(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    ip_address: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="ipAddress", validation_alias="ipAddress"
-    )
-    subnet_mask: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="subnetMask", validation_alias="subnetMask"
-    )
+    tracker_ref: Global[UUID] = Field(serialization_alias="trackerRef", validation_alias="trackerRef")
 
 
-class StaticIPv6Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ObjectTrackerGroupParcel(_ParcelBase):
+    type_: Literal["trackergroup"] = Field(default="trackergroup", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    address: Union[Global[str], Variable]
+    object_id: Union[Global[int], Variable] = Field(validation_alias=AliasPath("data", "objectId"))
+    tracker_refs: List[ObjectTrackerRef] = Field(validation_alias=AliasPath("data", "trackerRefs"))
+    criteria: Union[Global[Criteria], Variable, Default[Criteria]] = Field(
+        validation_alias=AliasPath("data", "trackerRefs"), default=Default[Criteria](value="or")
+    )
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,175 +1,69 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Address
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.common import (
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.common import EthernetDuplexMode, MediaType
+from catalystwan.models.configuration.feature_profile.common import (
     Arp,
+    DynamicDhcpDistance,
+    EthernetNatAttributesIpv4,
+    InterfaceDynamicIPv4Address,
+    InterfaceDynamicIPv6Address,
+    InterfaceStaticIPv4Address,
     StaticIPv4Address,
+    StaticIPv4AddressConfig,
     StaticIPv6Address,
+)
+from catalystwan.models.configuration.feature_profile.sdwan.service.lan.common import (
     VrrpIPv6Address,
     VrrpTrackingObject,
 )
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.vpn import Direction
-
-NatType = Literal[
-    "pool",
-    "loopback",
-]
-
-DuplexMode = Literal[
-    "full",
-    "half",
-    "auto",
-]
-
-MediaType = Literal[
-    "auto-select",
-    "rj45",
-    "sfp",
-]
-
-
-class DynamicDhcpDistance(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    dynamic_dhcp_distance: Union[Variable, Global[int], Default[int]] = Default[int](value=1)
-
-
-class InterfaceDynamicIPv4Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    dynamic: DynamicDhcpDistance
-
-
-class StaticIPv4AddressConfig(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    primary_ip_address: StaticIPv4Address = Field(
-        serialization_alias="staticIpV4AddressPrimary", validation_alias="staticIpV4AddressPrimary"
-    )
-    secondary_ip_address: Optional[StaticIPv4Address] = Field(
-        serialization_alias="staticIpV4AddressSecondary", validation_alias="staticIpV4AddressSecondary", default=None
-    )
-
-
-class InterfaceStaticIPv4Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    static: StaticIPv4AddressConfig
-
-
-class DynamicIPv6Dhcp(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    dhcp_client: Global[dict] = Field(
-        serialization_alias="dhcpClient", validation_alias="dhcpClient", default=Global[dict](value={})
-    )
-    secondary_ipv6_address: Optional[List[StaticIPv6Address]] = Field(
-        serialization_alias="secondaryIpV6Address", validation_alias="secondaryIpV6Address"
-    )
-
-
-class InterfaceDynamicIPv6Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    dynamic: DynamicIPv6Dhcp
 
 
 class Dhcpv6Helper(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     ip_address: Union[Global[str], Variable] = Field(serialization_alias="ipAddress", validation_alias="ipAddress")
     vpn: Optional[Union[Global[int], Variable, Default[None]]] = None
 
 
 class StaticIPv6AddressConfig(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     primary_ip_address: StaticIPv6Address = Field(
         serialization_alias="staticIpV6AddressPrimary", validation_alias="staticIpV6AddressPrimary"
     )
     secondary_ip_address: Optional[List[StaticIPv6Address]] = Field(
         serialization_alias="staticIpV6AddressSecondary", validation_alias="staticIpV6AddressSecondary", default=None
     )
     dhcp_helper_v6: Optional[List[Dhcpv6Helper]] = Field(
         serialization_alias="dhcpHelperV6", validation_alias="dhcpHelperV6", default=None
     )
 
 
 class InterfaceStaticIPv6Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     static: StaticIPv6AddressConfig
 
 
-class NatPool(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    range_start: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="rangeStart", validation_alias="rangeStart"
-    )
-    range_end: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="rangeEnd", validation_alias="rangeEnd"
-    )
-    prefix_length: Union[Variable, Global[int], Default[None]] = Field(
-        serialization_alias="prefixLength", validation_alias="prefixLength"
-    )
-    overload: Union[Variable, Global[bool], Default[bool]] = Default[bool](value=True)
-
-
-class StaticNat(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    source_ip: Union[Global[str], Variable] = Field(serialization_alias="sourceIp", validation_alias="sourceIp")
-
-    translate_ip: Union[Global[str], Variable] = Field(
-        serialization_alias="translateIp", validation_alias="translateIp"
-    )
-    static_nat_direction: Union[Global[Direction], Default[Direction]] = Field(
-        serialization_alias="staticNatDirection",
-        validation_alias="staticNatDirection",
-        default=Default[Direction](value="inside"),
-    )
-    source_vpn: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="sourceVpn", validation_alias="sourceVpn", default=Default[int](value=0)
-    )
-
-
-class NatAttributesIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    nat_type: Union[Global[NatType], Variable] = Field(serialization_alias="natType", validation_alias="natType")
-    nat_pool: Optional[NatPool] = Field(serialization_alias="natPool", validation_alias="natPool", default=None)
-    nat_loopback: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="natLoopbakc", validation_alias="natLoopbakc", default=None
-    )
-    udp_timeout: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="udpTimeout", validation_alias="udpTimeout", default=Default[int](value=1)
-    )
-    tcp_timeout: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="tcpTimeout", validation_alias="tcpTimeout", default=Default[int](value=1)
-    )
-    new_static_nat: Optional[List[StaticNat]] = Field(
-        serialization_alias="newStaticNat", validation_alias="newStaticNat", default=None
-    )
-
-
 class NatAttributesIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     nat64: Optional[Union[Global[bool], Default[bool]]] = Default[bool](value=False)
 
 
 class AclQos(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     shaping_rate: Optional[Union[Global[int], Variable, Default[None]]] = Field(
         serialization_alias="shapingRate", validation_alias="shapingRate", default=None
     )
     ipv4_acl_egress: Optional[Global[UUID]] = Field(
         serialization_alias="ipv4AclEgress", validation_alias="ipv4AclEgress", default=None
     )
@@ -181,51 +75,55 @@
     )
     ipv6_acl_ingress: Optional[Global[UUID]] = Field(
         serialization_alias="ipv6AclIngress", validation_alias="ipv6AclIngress", default=None
     )
 
 
 class VrrpIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     group_id: Union[Variable, Global[int]] = Field(serialization_alias="groupId", validation_alias="groupId")
     priority: Union[Variable, Global[int], Default[int]] = Default[int](value=100)
     timer: Union[Variable, Global[int], Default[int]] = Default[int](value=1000)
     track_omp: Union[Global[bool], Default[bool]] = Field(
         serialization_alias="trackOmp", validation_alias="trackOmp", default=Default[bool](value=False)
     )
     ipv6: List[VrrpIPv6Address]
 
 
 class VrrpIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     group_id: Union[Variable, Global[int]] = Field(serialization_alias="groupId", validation_alias="groupId")
     priority: Union[Variable, Global[int], Default[int]] = Default[int](value=100)
     timer: Union[Variable, Global[int], Default[int]] = Default[int](value=1000)
     track_omp: Union[Global[bool], Default[bool]] = Field(
         serialization_alias="trackOmp", validation_alias="trackOmp", default=Default[bool](value=False)
     )
-    ip_address: Union[Global[str], Variable] = Field(serialization_alias="ipAddress", validation_alias="ipAddress")
+    ip_address: Union[Global[str], Global[IPv4Address], Variable] = Field(
+        serialization_alias="ipAddress", validation_alias="ipAddress"
+    )
     ip_address_secondary: Optional[List[StaticIPv4Address]] = Field(
-        serialization_alias="ipAddressSecondary", validation_alias="ipAddressSecondary"
+        serialization_alias="ipAddressSecondary",
+        validation_alias="ipAddressSecondary",
+        default=None,
     )
     tloc_pref_change: Union[Global[bool], Default[bool]] = Field(
         serialization_alias="tlocPrefChange", validation_alias="tlocPrefChange", default=Default[bool](value=False)
     )
     tloc_pref_change_value: Optional[Union[Global[int], Default[None]]] = Field(
         serialization_alias="tlocPrefChangeValue", validation_alias="tlocPrefChangeValue", default=None
     )
     tracking_object: Optional[List[VrrpTrackingObject]] = Field(
         serialization_alias="trackingObject", validation_alias="trackingObject", default=None
     )
 
 
 class Trustsec(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     enable_sgt_propagation: Union[Global[bool], Default[bool]] = Field(
         serialization_alias="enableSGTPropagation",
         validation_alias="enableSGTPropagation",
         default=Default[bool](value=False),
     )
     propagate: Optional[Union[Global[bool], Default[bool]]] = Default[bool](value=True)
@@ -236,18 +134,18 @@
         serialization_alias="enableEnforcedPropagation", validation_alias="enableEnforcedPropagation"
     )
     enforced_security_group_tag: Union[Global[int], Variable, Default[None]] = Field(
         serialization_alias="enforcedSecurityGroupTag", validation_alias="enforcedSecurityGroupTag"
     )
 
 
-class AdvancedAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class AdvancedEthernetAttributes(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    duplex: Optional[Union[Global[DuplexMode], Variable, Default[None]]] = None
+    duplex: Optional[Union[Global[EthernetDuplexMode], Variable, Default[None]]] = None
     mac_address: Optional[Union[Global[str], Variable, Default[None]]] = Field(
         serialization_alias="macAddress", validation_alias="macAddress", default=None
     )
     ip_mtu: Union[Global[int], Variable, Default[int]] = Field(
         serialization_alias="ipMtu", validation_alias="ipMtu", default=Default[int](value=1500)
     )
     interface_mtu: Optional[Union[Global[int], Variable, Default[int]]] = Field(
@@ -269,59 +167,86 @@
     )
     tracker: Optional[Union[Global[str], Variable, Default[None]]] = None
     icmp_redirect_disable: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="icmpRedirectDisable",
         validation_alias="icmpRedirectDisable",
         default=Default[bool](value=True),
     )
-    xconnect: Optional[Union[Global[str], Variable, Default[None]]] = None
+    xconnect: Optional[Union[Global[str], Global[IPv4Address], Variable, Default[None]]] = None
     ip_directed_broadcast: Union[Global[bool], Variable, Default[bool]] = Field(
         serialization_alias="ipDirectedBroadcast",
         validation_alias="ipDirectedBroadcast",
         default=Default[bool](value=False),
     )
 
 
-class InterfaceEthernetData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    shutdown: Union[Global[bool], Variable, Default[bool]] = Default[bool](value=True)
-    interface_name: Union[Global[str], Variable] = Field(
-        serialization_alias="interfaceName", validation_alias="interfaceName"
+class InterfaceEthernetParcel(_ParcelBase):
+    type_: Literal["lan/vpn/interface/ethernet"] = Field(default="lan/vpn/interface/ethernet", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    shutdown: Union[Global[bool], Variable, Default[bool]] = Field(
+        default=Default[bool](value=True), validation_alias=AliasPath("data", "shutdown")
+    )
+    interface_name: Union[Global[str], Variable] = Field(validation_alias=AliasPath("data", "interfaceName"))
+    ethernet_description: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        default=Default[None](value=None), validation_alias=AliasPath("data", "description")
     )
-    description: Optional[Union[Global[str], Variable, Default[None]]] = None
     interface_ip_address: Union[InterfaceDynamicIPv4Address, InterfaceStaticIPv4Address] = Field(
-        serialization_alias="intfIpAddress", validation_alias="intfIpAddress"
+        validation_alias=AliasPath("data", "intfIpAddress"), default_factory=InterfaceStaticIPv4Address
     )
     dhcp_helper: Optional[Union[Variable, Global[List[str]], Default[None]]] = Field(
-        serialization_alias="dhcpHelper", validation_alias="dhcpHelper", default=None
+        validation_alias=AliasPath("data", "dhcpHelper"), default=None
     )
     interface_ipv6_address: Optional[Union[InterfaceDynamicIPv6Address, InterfaceStaticIPv6Address]] = Field(
-        serialization_alias="intfIpV6Address", validation_alias="intfIpV6Address", default=None
+        validation_alias=AliasPath("data", "intfIpV6Address"), default=None
     )
-    nat: Union[Global[bool], Default[bool]] = Default[bool](value=False)
-    nat_attributes_ipv4: Optional[NatAttributesIPv4] = Field(
-        serialization_alias="natAttributesIpv4", validation_alias="natAttributesIpv4", default=None
+    nat: Union[Global[bool], Default[bool]] = Field(
+        validation_alias=AliasPath("data", "nat"), default=Default[bool](value=False)
+    )
+    nat_attributes_ipv4: Optional[EthernetNatAttributesIpv4] = Field(
+        validation_alias=AliasPath("data", "natAttributesIpv4"), default=None
     )
     nat_ipv6: Optional[Union[Global[bool], Default[bool]]] = Field(
-        serialization_alias="natIpv6", validation_alias="natIpv6", default=Default[bool](value=False)
+        validation_alias=AliasPath("data", "natIpv6"), default=Default[bool](value=False)
     )
     nat_attributes_ipv6: Optional[NatAttributesIPv6] = Field(
-        serialization_alias="natAttributesIpv6", validation_alias="natAttributesIpv6", default=None
-    )
-    acl_qos: Optional[AclQos] = Field(serialization_alias="aclQos", validation_alias="aclQos", default=None)
-    vrrp_ipv6: Optional[List[VrrpIPv6]] = Field(
-        serialization_alias="vrrpIpv6", validation_alias="vrrpIpv6", default=None
+        validation_alias=AliasPath("data", "natAttributesIpv6"), default=None
     )
-    vrrp: Optional[List[VrrpIPv4]] = None
-    arp: Optional[List[Arp]] = None
-    trustsec: Optional[Trustsec] = None
-    advanced: AdvancedAttributes = AdvancedAttributes()
-
-
-class InterfaceEthernetCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: InterfaceEthernetData
-    metadata: Optional[dict] = None
+    acl_qos: Optional[AclQos] = Field(validation_alias=AliasPath("data", "aclQos"), default=None)
+    vrrp_ipv6: Optional[List[VrrpIPv6]] = Field(validation_alias=AliasPath("data", "vrrpIpv6"), default=None)
+    vrrp: Optional[List[VrrpIPv4]] = Field(validation_alias=AliasPath("data", "vrrp"), default=None)
+    arp: Optional[List[Arp]] = Field(validation_alias=AliasPath("data", "arp"), default=None)
+    trustsec: Optional[Trustsec] = Field(validation_alias=AliasPath("data", "trustsec"), default=None)
+    advanced: AdvancedEthernetAttributes = Field(
+        validation_alias=AliasPath("data", "advanced"), default_factory=AdvancedEthernetAttributes
+    )
+
+    def set_dynamic_interface_ip_address(self, dhcp_distance: Union[Global[int], Variable]) -> None:
+        self.interface_ip_address = InterfaceDynamicIPv4Address(
+            dynamic=DynamicDhcpDistance(dynamic_dhcp_distance=dhcp_distance)
+        )
+
+    def set_static_primary_interface_ip_address(
+        self,
+        ip_address: Union[Global[str], Global[IPv4Address], Variable],
+        subnet_mask: Optional[Union[Global[str], Variable]] = None,
+    ) -> None:
+        if subnet_mask is None:
+            primary_ip_address = StaticIPv4Address(ip_address=ip_address)
+        else:
+            primary_ip_address = StaticIPv4Address(ip_address=ip_address, subnet_mask=subnet_mask)
+        self.interface_ip_address = InterfaceStaticIPv4Address(
+            static=StaticIPv4AddressConfig(primary_ip_address=primary_ip_address)
+        )
+
+    def add_static_secondary_interface_ip_address(
+        self, ip_address: Union[Global[str], Global[IPv4Address], Variable], subnet_mask: Union[Global[str], Variable]
+    ) -> None:
+        if self.interface_ip_address is None:
+            raise ValueError("Missing static primary IP Address")
+        if isinstance(self.interface_ip_address, InterfaceDynamicIPv4Address):
+            raise ValueError("Interface IP Address is already dynamic")
+
+        secondary_ip_address = StaticIPv4Address(ip_address=ip_address, subnet_mask=subnet_mask)
+        if self.interface_ip_address.static.secondary_ip_address is None:
+            self.interface_ip_address.static.secondary_ip_address = []
+        self.interface_ip_address.static.secondary_ip_address.append(secondary_ip_address)
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,206 +1,270 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import Literal, Optional, Union
+from ipaddress import IPv4Address
+from typing import List, Literal, Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.common import (
-    IkeCiphersuite,
-    IkeGroup,
-    IkeMode,
-    IpsecCiphersuite,
-    PfsGroup,
-    TunnelApplication,
-)
-
-GreTunnelMode = Literal[
-    "ipv4",
-    "ipv6",
-]
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default, as_global
 
+VirtualApplicationType = Literal["dreopt"]
 
-class GreAddress(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+ResourceProfile = Literal[
+    "small",
+    "medium",
+    "large",
+    "extra-large",
+    "default",
+]
 
-    address: Union[Variable, Global[str]]
-    mask: Union[Variable, Global[str]]
+AppqoeDeviceRole = Literal[
+    "forwarder",
+    "forwarderAndServiceNode",
+    "serviceNode",
+    "serviceNodeWithDre",
+    "forwarderAndServiceNodeWithDre",
+]
 
+AppnavControllerGroupName = Literal["ACG-APPQOE"]
+ServiceNodeGroupName = Literal["SNG-APPQOE"]
+ServiceNodeGroupsNames = Literal[
+    "SNG-APPQOE",
+    "SNG-APPQOE1",
+    "SNG-APPQOE2",
+    "SNG-APPQOE3",
+    "SNG-APPQOE4",
+    "SNG-APPQOE5",
+    "SNG-APPQOE6",
+    "SNG-APPQOE7",
+    "SNG-APPQOE8",
+    "SNG-APPQOE9",
+    "SNG-APPQOE10",
+    "SNG-APPQOE11",
+    "SNG-APPQOE12",
+    "SNG-APPQOE13",
+    "SNG-APPQOE14",
+    "SNG-APPQOE15",
+    "SNG-APPQOE16",
+    "SNG-APPQOE17",
+    "SNG-APPQOE18",
+    "SNG-APPQOE19",
+    "SNG-APPQOE20",
+    "SNG-APPQOE21",
+    "SNG-APPQOE22",
+    "SNG-APPQOE23",
+    "SNG-APPQOE24",
+    "SNG-APPQOE25",
+    "SNG-APPQOE26",
+    "SNG-APPQOE27",
+    "SNG-APPQOE28",
+    "SNG-APPQOE29",
+    "SNG-APPQOE30",
+    "SNG-APPQOE31",
+]
+ForwarderAndServiceNodeAddress = Literal["192.168.2.2"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
+ForwarderAndServiceNodeControllerAddress = Literal[
+    "192.168.2.1"
+]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
+ServiceNodeExternalAddress = Literal["192.168.2.2"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
+ServiceNodeExternalVpgIp = Literal["192.168.2.1/24"]  # TODO: 1.Is it really constant? 2.Use ipaddress.IPv4Address?
 
-class TunnelSourceIP(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    tunnel_source: Union[Global[str], Variable] = Field(
-        serialization_alias="tunnelSource", validation_alias="tunnelSource"
+class VirtualApplication(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    instance_id: Global[int] = Field(
+        default=Global(value=1), serialization_alias="instanceId", validation_alias="instanceId"
+    )
+    application_type: Global[VirtualApplicationType] = Field(
+        default=Global[VirtualApplicationType](value="dreopt"),
+        serialization_alias="applicationType",
+        validation_alias="applicationType",
     )
-    tunnel_route_via: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="tunnelRouteVia", validation_alias="tunnelRouteVia", default=None
+    resource_profile: Union[Global[ResourceProfile], Default[ResourceProfile]] = Field(
+        default=Default[ResourceProfile](value="default"),
+        serialization_alias="resourceProfile",
+        validation_alias="resourceProfile",
     )
 
 
-class TunnelSourceIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class Appqoe(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    tunnel_source_v6: Union[Global[str], Variable] = Field(
-        serialization_alias="tunnelSourceV6", validation_alias="tunnelSourceV6"
+    name: Default[str] = Default(value="/1")
+    appnav_controller_group: Global[AppnavControllerGroupName] = Field(
+        default=Global[AppnavControllerGroupName](value="ACG-APPQOE"),
+        serialization_alias="appnavControllerGroup",
+        validation_alias="appnavControllerGroup",
+    )
+    service_node_group: Global[ServiceNodeGroupName] = Field(
+        default=Global[ServiceNodeGroupName](value="SNG-APPQOE"),
+        serialization_alias="serviceNodeGroup",
+        validation_alias="serviceNodeGroup",
     )
-    tunnel_route_via: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="tunnelRouteVia", validation_alias="tunnelRouteVia", default=None
+    service_node_groups: List[Global[ServiceNodeGroupsNames]] = Field(
+        default=[Global[ServiceNodeGroupsNames](value="SNG-APPQOE")],
+        serialization_alias="serviceNodeGroups",
+        validation_alias="serviceNodeGroups",
     )
+    enable: Global[bool] = Global[bool](value=True)
+    vpn: Union[Global[int], Default[None], Variable] = Field(default=Global[int](value=0))
 
 
-class TunnelSourceInterface(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ServiceContext(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+    appqoe: List[Appqoe] = Field(default_factory=lambda: [Appqoe()])
 
-    tunnel_source_interface: Union[Global[str], Variable] = Field(
-        serialization_alias="tunnelSourceInterface", validation_alias="tunnelSourceInterface"
-    )
-    tunnel_route_via: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="tunnelRouteVia", validation_alias="tunnelRouteVia", default=None
-    )
 
+# Frowarder
 
-class GreSourceIp(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    source_ip: TunnelSourceIP = Field(serialization_alias="sourceIp", validation_alias="sourceIp")
+class ServiceNodeInformation(BaseModel):
+    address: Global[IPv4Address]
 
 
-class GreSourceNotLoopback(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ForwarderController(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    source_not_loopback: TunnelSourceInterface = Field(
-        serialization_alias="sourceNotLoopback", validation_alias="sourceNotLoopback"
+    address: Union[Global[str], Global[IPv4Address], Variable]
+    vpn: Global[int] = Field(
+        default=Global[int](value=1), description="This is field is a depended on the Service VPN value."
     )
 
 
-class GreSourceLoopback(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ForwarderAppnavControllerGroup(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    source_loopback: TunnelSourceInterface = Field(
-        serialization_alias="sourceLoopback", validation_alias="sourceLoopback"
+    group_name: Default[AppnavControllerGroupName] = Field(
+        default=Default(value="ACG-APPQOE"), serialization_alias="groupName", validation_alias="groupName"
+    )
+    appnav_controllers: List[ForwarderController] = Field(
+        serialization_alias="appnavControllers", validation_alias="appnavControllers"
     )
 
 
-class GreSourceIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ForwarderNodeGroup(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    source_ipv6: TunnelSourceIPv6 = Field(serialization_alias="sourceIpv6", validation_alias="sourceIpv6")
+    name: Union[Global[str], Default[ServiceNodeGroupName]] = Default[ServiceNodeGroupName](value="SNG-APPQOE")
+    internal: Union[Default[bool], Global[bool]] = Default[bool](value=False)
+    service_node: List[ServiceNodeInformation] = Field(
+        serialization_alias="serviceNode", validation_alias="serviceNode"
+    )
 
 
-class BasicGre(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ForwarderRole(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    interface_name: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="ifName", validation_alias="ifName", default=None
-    )
-    description: Optional[Union[Global[str], Variable, Default[None]]] = None
-    address: Optional[GreAddress] = None
-    ipv6_address: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="ipv6Address", validation_alias="ipv6Address", default=None
-    )
-    shutdown: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
-    tunnel_protection: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="tunnelProtection", validation_alias="tunnelProtection", default=Default[bool](value=False)
-    )
-    tunnel_mode: Optional[Union[Global[GreTunnelMode], Default[GreTunnelMode]]] = Field(
-        serialization_alias="tunnelMode",
-        validation_alias="tunnelMode",
-        default=Default[GreTunnelMode](value="ipv4"),
+    appnav_controller_group: List[ForwarderAppnavControllerGroup] = Field(
+        serialization_alias="appnavControllerGroup", validation_alias="appnavControllerGroup"
     )
-    tunnel_source_type: Optional[Union[GreSourceIp, GreSourceNotLoopback, GreSourceLoopback, GreSourceIPv6]] = Field(
-        serialization_alias="tunnelSourceType", validation_alias="tunnelSourceType", default=None
+    service_node_group: List[ForwarderNodeGroup] = Field(
+        serialization_alias="serviceNodeGroup", validation_alias="serviceNodeGroup"
     )
-    tunnel_destination: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="tunnelDestination", validation_alias="tunnelDestination", default=None
+    service_context: ServiceContext = Field(
+        default_factory=ServiceContext, serialization_alias="serviceContext", validation_alias="serviceContext"
     )
-    tunnel_destination_v6: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="tunnelDestinationV6", validation_alias="tunnelDestinationV6", default=None
-    )
-    mtu: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=1500)
-    mtu_v6: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="mtuV6", validation_alias="mtuV6", default=None
-    )
-    tcp_mss_adjust: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="tcpMssAdjust", validation_alias="tcpMssAdjust", default=None
-    )
-    tcp_mss_adjust_v6: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="tcpMssAdjustV6", validation_alias="tcpMssAdjustV6", default=None
-    )
-    clear_dont_fragment: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="clearDontFragment",
-        validation_alias="clearDontFragment",
-        default=Default[bool](value=False),
-    )
-    dpd_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="dpdInterval", validation_alias="dpdInterval", default=Default[int](value=10)
-    )
-    dpd_retries: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="dpdRetries", validation_alias="dpdRetries", default=Default[int](value=3)
-    )
-    ike_version: Optional[Union[Global[int], Default[int]]] = Field(
-        serialization_alias="ikeVersion", validation_alias="ikeVersion", default=Default[int](value=1)
-    )
-    ike_mode: Optional[Union[Global[IkeMode], Variable, Default[IkeMode]]] = Field(
-        serialization_alias="ikeMode", validation_alias="ikeMode", default=Default[IkeMode](value="main")
-    )
-    ike_rekey_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="ikeRekeyInterval", validation_alias="ikeRekeyInterval", default=Default[int](value=14400)
-    )
-    ike_ciphersuite: Optional[Union[Global[IkeCiphersuite], Variable, Default[IkeCiphersuite]]] = Field(
-        serialization_alias="ikeCiphersuite",
-        validation_alias="ikeCiphersuite",
-        default=Default[IkeCiphersuite](value="aes256-cbc-sha1"),
-    )
-    ike_group: Optional[Union[Global[IkeGroup], Variable, Default[IkeGroup]]] = Field(
-        serialization_alias="ikeGroup", validation_alias="ikeGroup", default=Default[IkeGroup](value="16")
-    )
-    pre_shared_secret: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="preSharedSecret", validation_alias="preSharedSecret", default=None
+
+
+# Forwarder and Service
+
+
+class ServiceNodeInformationDefault(BaseModel):
+    address: Default[ForwarderAndServiceNodeAddress] = Default[ForwarderAndServiceNodeAddress](value="192.168.2.2")
+
+
+class ForwarderAndServiceNodeController(BaseModel):
+    address: Default[ForwarderAndServiceNodeControllerAddress] = Default[ForwarderAndServiceNodeControllerAddress](
+        value="192.168.2.1"
     )
-    ike_local_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="ikeLocalId", validation_alias="ikeLocalId", default=None
+
+
+class ForwarderAndServiceNodeAppnavControllerGroup(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    group_name: Default[AppnavControllerGroupName] = Field(
+        default=Default[AppnavControllerGroupName](value="ACG-APPQOE"),
+        serialization_alias="groupName",
+        validation_alias="groupName",
     )
-    ike_remote_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="ikeRemoteId", validation_alias="ikeRemoteId", default=None
+    appnav_controllers: List[ForwarderAndServiceNodeController] = Field(
+        serialization_alias="appnavControllers", validation_alias="appnavControllers"
     )
-    ipsec_rekey_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="ipsecRekeyInterval",
-        validation_alias="ipsecRekeyInterval",
-        default=Default[int](value=3600),
+
+
+class ForwarderAndServiceNodeGroup(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    name: Default[ServiceNodeGroupName] = Default[ServiceNodeGroupName](value="SNG-APPQOE")
+    internal: Default[bool] = Default[bool](value=True)
+    service_node: List[ServiceNodeInformationDefault] = Field(
+        serialization_alias="serviceNode", validation_alias="serviceNode"
     )
-    ipsec_replay_window: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="ipsecReplayWindow", validation_alias="ipsecReplayWindow", default=Default[int](value=512)
+
+
+class ForwarderAndServiceNodeRole(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    appnav_controller_group: List[ForwarderAndServiceNodeAppnavControllerGroup] = Field(
+        serialization_alias="appnavControllerGroup", validation_alias="appnavControllerGroup"
     )
-    ipsec_ciphersuite: Optional[Union[Global[IpsecCiphersuite], Variable, Default[IpsecCiphersuite]]] = Field(
-        serialization_alias="ipsecCiphersuite",
-        validation_alias="ipsecCiphersuite",
-        default=Default[IpsecCiphersuite](value="aes256-gcm"),
+    service_node_group: List[ForwarderAndServiceNodeGroup] = Field(
+        serialization_alias="serviceNodeGroup", validation_alias="serviceNodeGroup"
     )
-    perfect_forward_secrecy: Optional[Union[Global[PfsGroup], Variable, Default[PfsGroup]]] = Field(
-        serialization_alias="perfectForwardSecrecy",
-        validation_alias="perfectForwardSecrecy",
-        default=Default[PfsGroup](value="group-16"),
+
+    service_context: ServiceContext = Field(serialization_alias="serviceContext", validation_alias="serviceContext")
+
+
+# Service
+
+
+class ServiceNodeInformationExternal(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    address: Default[ServiceNodeExternalAddress] = Default[ServiceNodeExternalAddress](value="192.168.2.2")
+    vpg_ip: Default[ServiceNodeExternalVpgIp] = Field(
+        default=Default[ServiceNodeExternalVpgIp](value="192.168.2.1/24"),
+        serialization_alias="vpgIp",
+        validation_alias="vpgIp",
     )
 
 
-class AdvancedGre(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ServiceNodeGroup(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    application: Optional[Union[Global[TunnelApplication], Variable]] = None
+    name: Default[ServiceNodeGroupName] = Default[ServiceNodeGroupName](value="SNG-APPQOE")
+    external_node: Default[bool] = Field(
+        default=Default[bool](value=True), serialization_alias="externalNode", validation_alias="externalNode"
+    )
+    service_node: List[ServiceNodeInformationExternal] = Field(
+        default=[ServiceNodeInformationExternal()], serialization_alias="serviceNode", validation_alias="serviceNode"
+    )
 
 
-class InterfaceGreData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ServiceNodeRole(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    service_node_group: List[ServiceNodeGroup] = Field(
+        default=[ServiceNodeGroup()], serialization_alias="serviceNodeGroup", validation_alias="serviceNodeGroup"
+    )
 
-    basic: BasicGre
-    advanced: Optional[AdvancedGre] = None
 
+class AppqoeParcel(_ParcelBase):
+    type_: Literal["appqoe"] = Field(default="appqoe", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-class InterfaceGreCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    dreopt: Optional[Union[Global[bool], Default[bool]]] = Field(
+        default=as_default(False), validation_alias=AliasPath("data", "dreopt")
+    )
+    virtual_application: Optional[List[VirtualApplication]] = Field(
+        default=None, validation_alias=AliasPath("data", "virtualApplication")
+    )
+    appqoe_device_role: Global[str] = Field(
+        default=as_global("forwarder"), validation_alias=AliasPath("data", "appqoeDeviceRole")
+    )
 
-    name: str
-    description: Optional[str] = None
-    data: InterfaceGreData
-    metadata: Optional[dict] = None
+    forwarder: Optional[ForwarderRole] = Field(default=None, validation_alias=AliasPath("data", "forwarder"))
+    forwarder_and_service_node: Optional[ForwarderAndServiceNodeRole] = Field(
+        default=None, validation_alias=AliasPath("data", "forwarderAndServiceNode")
+    )
+    service_node: Optional[ServiceNodeRole] = Field(default=None, validation_alias=AliasPath("data", "serviceNode"))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,138 +1,119 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Interface, IPv6Address, IPv6Interface
 from typing import Literal, Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.common import (
-    IkeCiphersuite,
-    IkeGroup,
-    IkeMode,
-    IpsecCiphersuite,
-    PfsGroup,
-    TunnelApplication,
-)
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.common import IkeCiphersuite, IkeGroup, IkeMode, IpsecCiphersuite, PfsGroup
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask, TunnelApplication
 
 IpsecTunnelMode = Literal[
     "ipv4",
     "ipv6",
     "ipv4-v6overlay",
 ]
 
 
-class IpsecAddress(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    address: Union[Variable, Global[str]]
-    mask: Union[Variable, Global[str]]
-
-
-class InterfaceIpsecData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    interface_name: Union[Global[str], Variable] = Field(serialization_alias="ifName", validation_alias="ifName")
-    shutdown: Union[Global[bool], Variable, Default[bool]] = Default[bool](value=True)
+class InterfaceIpsecParcel(_ParcelBase):
+    type_: Literal["lan/vpn/interface/ipsec"] = Field(default="lan/vpn/interface/ipsec", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    interface_name: Union[Global[str], Variable] = Field(validation_alias=AliasPath("data", "ifName"))
+    shutdown: Union[Global[bool], Variable, Default[bool]] = Field(
+        default=Default[bool](value=True), validation_alias=AliasPath("data", "shutdown")
+    )
     tunnel_mode: Optional[Union[Global[IpsecTunnelMode], Default[IpsecTunnelMode]]] = Field(
-        serialization_alias="tunnelMode",
-        validation_alias="tunnelMode",
-        default=Default[IpsecTunnelMode](value="ipv4"),
-    )
-    description: Union[Global[str], Variable, Default[None]] = Default[None](value=None)
-    address: Optional[IpsecAddress] = None
-    ipv6_address: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="ipv6Address", validation_alias="ipv6Address", default=None
+        validation_alias=AliasPath("data", "tunnelMode"),
+        default=None,
+    )
+    ipsec_description: Union[Global[str], Variable, Default[None]] = Field(
+        default=Default[None](value=None), validation_alias=AliasPath("data", "description")
     )
-    tunnel_source: Optional[IpsecAddress] = Field(
-        serialization_alias="tunnelSource", validation_alias="tunnelSource", default=None
+    address: Optional[AddressWithMask] = Field(default=None, validation_alias=AliasPath("data", "address"))
+    ipv6_address: Optional[Union[Global[str], Global[IPv6Interface], Variable]] = Field(
+        validation_alias=AliasPath("data", "ipv6Address"), default=None
     )
+    tunnel_source: Optional[AddressWithMask] = Field(validation_alias=AliasPath("data", "tunnelSource"), default=None)
     tunnel_source_v6: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="tunnelSourceV6", validation_alias="tunnelSourceV6", default=None
+        validation_alias=AliasPath("data", "tunnelSourceV6"), default=None
     )
-    tunnel_source_interface: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="tunnelSourceInterface", validation_alias="tunnelSourceInterface", default=None
+    tunnel_source_interface: Optional[Union[Global[str], Global[IPv4Interface], Variable]] = Field(
+        validation_alias=AliasPath("data", "tunnelSourceInterface"), default=None
     )
-    tunnel_destination: Optional[IpsecAddress] = Field(
-        serialization_alias="tunnelDestination", validation_alias="tunnelDestination", default=None
+    tunnel_destination: Optional[AddressWithMask] = Field(
+        validation_alias=AliasPath("data", "tunnelDestination"), default=None
     )
-    tunnel_destination_v6: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="tunnelDestinationV6", validation_alias="tunnelDestinationV6", default=None
+    tunnel_destination_v6: Optional[Union[Global[str], Global[IPv6Address], Variable]] = Field(
+        validation_alias=AliasPath("data", "tunnelDestinationV6"), default=None
     )
-    application: Union[Global[TunnelApplication], Variable]
+    application: Union[Global[TunnelApplication], Variable] = Field(validation_alias=AliasPath("data", "application"))
     tcp_mss_adjust: Union[Global[int], Variable, Default[None]] = Field(
-        serialization_alias="tcpMssAdjust", validation_alias="tcpMssAdjust", default=Default[None](value=None)
+        validation_alias=AliasPath("data", "tcpMssAdjust"), default=Default[None](value=None)
     )
-    tcp_mss_adjust_v6: Union[Global[int], Variable, Default[None]] = Field(
-        serialization_alias="tcpMssAdjustV6", validation_alias="tcpMssAdjustV6", default=Default[None](value=None)
+    tcp_mss_adjust_v6: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        validation_alias=AliasPath("data", "tcpMssAdjustV6"), default=None
     )
     clear_dont_fragment: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="clearDontFragment",
-        validation_alias="clearDontFragment",
+        validation_alias=AliasPath("data", "clearDontFragment"),
         default=Default[bool](value=False),
     )
-    mtu: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=1500)
+    mtu: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        default=Default[int](value=1500), validation_alias=AliasPath("data", "mtu")
+    )
     mtu_v6: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="mtuV6", validation_alias="mtuV6", default=None
+        validation_alias=AliasPath("data", "mtuV6"), default=None
     )
     dpd_interval: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="dpdInterval", validation_alias="dpdInterval", default=Default[int](value=10)
+        validation_alias=AliasPath("data", "dpdInterval"), default=Default[int](value=10)
     )
     dpd_retries: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="dpdRetries", validation_alias="dpdRetries", default=Default[int](value=3)
+        validation_alias=AliasPath("data", "dpdRetries"), default=Default[int](value=3)
     )
     ike_version: Union[Global[int], Default[int]] = Field(
-        serialization_alias="ikeVersion", validation_alias="ikeVersion", default=Default[int](value=1)
+        validation_alias=AliasPath("data", "ikeVersion"), default=Default[int](value=1)
     )
     ike_mode: Optional[Union[Global[IkeMode], Variable, Default[IkeMode]]] = Field(
-        serialization_alias="ikeMode", validation_alias="ikeMode", default=Default[IkeMode](value="main")
+        validation_alias=AliasPath("data", "ikeMode"), default=Default[IkeMode](value="main")
     )
     ike_rekey_interval: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="ikeRekeyInterval", validation_alias="ikeRekeyInterval", default=Default[int](value=14400)
+        validation_alias=AliasPath("data", "ikeRekeyInterval"), default=Default[int](value=14400)
     )
     ike_ciphersuite: Union[Global[IkeCiphersuite], Variable, Default[IkeCiphersuite]] = Field(
-        serialization_alias="ikeCiphersuite",
-        validation_alias="ikeCiphersuite",
+        validation_alias=AliasPath("data", "ikeCiphersuite"),
         default=Default[IkeCiphersuite](value="aes256-cbc-sha1"),
     )
     ike_group: Union[Global[IkeGroup], Variable, Default[IkeGroup]] = Field(
-        serialization_alias="ikeGroup", validation_alias="ikeGroup", default=Default[IkeGroup](value="16")
+        validation_alias=AliasPath("data", "ikeGroup"), default=Default[IkeGroup](value="16")
     )
     pre_shared_secret: Union[Global[str], Variable] = Field(
-        serialization_alias="preSharedSecret", validation_alias="preSharedSecret"
+        validation_alias=AliasPath("data", "preSharedSecret"),
     )
     ike_local_id: Union[Global[str], Variable, Default[None]] = Field(
-        serialization_alias="ikeLocalId", validation_alias="ikeLocalId"
+        validation_alias=AliasPath("data", "ikeLocalId"), default=Default[None](value=None)
     )
     ike_remote_id: Union[Global[str], Variable, Default[None]] = Field(
-        serialization_alias="ikeRemoteId", validation_alias="ikeRemoteId"
+        validation_alias=AliasPath("data", "ikeRemoteId"), default=Default[None](value=None)
     )
     ipsec_rekey_interval: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="ipsecRekeyInterval",
-        validation_alias="ipsecRekeyInterval",
+        validation_alias=AliasPath("data", "ipsecRekeyInterval"),
         default=Default[int](value=3600),
     )
     ipsec_replay_window: Union[Global[int], Variable, Default[int]] = Field(
-        serialization_alias="ipsecReplayWindow", validation_alias="ipsecReplayWindow", default=Default[int](value=512)
+        validation_alias=AliasPath("data", "ipsecReplayWindow"), default=Default[int](value=512)
     )
     ipsec_ciphersuite: Union[Global[IpsecCiphersuite], Variable, Default[IpsecCiphersuite]] = Field(
-        serialization_alias="ipsecCiphersuite",
-        validation_alias="ipsecCiphersuite",
+        validation_alias=AliasPath("data", "ipsecCiphersuite"),
         default=Default[IpsecCiphersuite](value="aes256-gcm"),
     )
     perfect_forward_secrecy: Union[Global[PfsGroup], Variable, Default[PfsGroup]] = Field(
-        serialization_alias="perfectForwardSecrecy",
-        validation_alias="perfectForwardSecrecy",
+        validation_alias=AliasPath("data", "perfectForwardSecrecy"),
         default=Default[PfsGroup](value="group-16"),
     )
-    tracker: Optional[Union[Global[str], Variable, Default[None]]] = None
+    tracker: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        default=None, validation_alias=AliasPath("data", "tracker")
+    )
     tunnel_route_via: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="tunnelRouteVia", validation_alias="tunnelRouteVia", default=None
+        validation_alias=AliasPath("data", "tunnelRouteVia"), default=None
     )
-
-
-class InterfaceIpsecCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: InterfaceIpsecData
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,177 +1,136 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Optional, Union
-from uuid import UUID
+from ipaddress import IPv4Address, IPv6Address, IPv6Interface
+from typing import Literal, Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.common import (
-    Arp,
-    StaticIPv4Address,
-    StaticIPv6Address,
-    VrrpIPv6Address,
-    VrrpTrackingObject,
-)
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.common import IkeCiphersuite, IkeGroup, IkeMode, IpsecCiphersuite, PfsGroup
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask, AdvancedGre, TunnelSourceType
 
+GreTunnelMode = Literal[
+    "ipv4",
+    "ipv6",
+]
 
-class VrrpIPv4SecondaryAddress(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    address: Union[Variable, Global[str]]
+class TunnelSourceIPv6(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
+    tunnel_source_v6: Union[Global[str], Global[IPv6Address], Variable] = Field(
+        serialization_alias="tunnelSourceV6", validation_alias="tunnelSourceV6"
+    )
+    tunnel_route_via: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="tunnelRouteVia", validation_alias="tunnelRouteVia", default=None
+    )
 
-class VrrpIPv6SecondaryAddress(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    prefix: Union[Global[str], Variable]
+class GreSourceIPv6(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
+    source_ipv6: TunnelSourceIPv6 = Field(serialization_alias="sourceIpv6", validation_alias="sourceIpv6")
 
-class VrrpIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    group_id: Union[Variable, Global[int]] = Field(serialization_alias="groupId", validation_alias="groupId")
-    priority: Union[Variable, Global[int], Default[int]] = Default[int](value=100)
-    timer: Union[Variable, Global[int], Default[int]] = Default[int](value=1000)
-    track_omp: Union[Global[bool], Default[bool]] = Field(
-        serialization_alias="trackOmp", validation_alias="trackOmp", default=Default[bool](value=False)
+class BasicGre(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    if_name: Union[Global[str], Variable] = Field(
+        serialization_alias="ifName", validation_alias="ifName", description="Minimum length of the value should be 4."
     )
-    ip_address: Union[Global[str], Variable] = Field(serialization_alias="ipAddress", validation_alias="ipAddress")
-    ip_address_secondary: Optional[List[VrrpIPv4SecondaryAddress]] = Field(
-        serialization_alias="ipAddressSecondary", validation_alias="ipAddressSecondary"
+    description: Union[Global[str], Variable, Default[None]] = Field(default=Default[None](value=None))
+    address: Optional[AddressWithMask] = None
+    ipv6_address: Optional[Union[Global[str], Global[IPv6Interface], Variable, Default[None]]] = Field(
+        serialization_alias="ipv6Address", validation_alias="ipv6Address", default=None
     )
-    tloc_pref_change: Union[Global[bool], Default[bool]] = Field(
-        serialization_alias="tlocPrefChange", validation_alias="tlocPrefChange", default=Default[bool](value=False)
+    shutdown: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
+    tunnel_protection: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="tunnelProtection", validation_alias="tunnelProtection", default=None
     )
-    tloc_pref_change_value: Optional[Union[Global[int], Variable]] = Field(
-        serialization_alias="tlocPrefChangeValue", validation_alias="tlocPrefChangeValue", default=None
+    tunnel_mode: Optional[Union[Global[GreTunnelMode], Default[GreTunnelMode]]] = Field(
+        default=None,
+        serialization_alias="tunnelMode",
+        validation_alias="tunnelMode",
     )
-    tracking_object: Optional[List[VrrpTrackingObject]] = Field(
-        serialization_alias="trackingObject", validation_alias="trackingObject", default=None
+    tunnel_source_type: Optional[Union[TunnelSourceType, GreSourceIPv6]] = Field(
+        serialization_alias="tunnelSourceType", validation_alias="tunnelSourceType", default=None
     )
-
-    prefix_list: Optional[Union[Global[str], Variable, Default[None]]] = Default[None](value=None)
-
-
-class VrrpIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    group_id: Union[Variable, Global[int]] = Field(serialization_alias="groupId", validation_alias="groupId")
-    priority: Union[Variable, Global[int], Default[int]] = Default[int](value=100)
-    timer: Union[Variable, Global[int], Default[int]] = Default[int](value=1000)
-    track_omp: Union[Global[bool], Default[bool]] = Field(
-        serialization_alias="trackOmp", validation_alias="trackOmp", default=Default[bool](value=False)
+    tunnel_destination: Union[Global[str], Global[IPv4Address], Variable] = Field(
+        serialization_alias="tunnelDestination", validation_alias="tunnelDestination"
     )
-    track_prefix_list: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="trackPrefixList", validation_alias="trackPrefixList"
+    tunnel_destination_v6: Optional[Union[Global[str], Global[IPv6Address], Variable]] = Field(
+        default=None, serialization_alias="tunnelDestinationV6", validation_alias="tunnelDestinationV6"
     )
-    ipv6: List[VrrpIPv6Address]
-    ipv6_secondary: Optional[List[VrrpIPv6SecondaryAddress]]
-
-
-class Dhcpv6Helper(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    address: Union[Global[str], Variable] = Field(serialization_alias="address", validation_alias="address")
-    vpn: Optional[Union[Global[int], Variable, Default[None]]] = None
-
-
-class AdvancedSviAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    tcp_mss: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="tcpMss", validation_alias="tcpMss", default=Default[None](value=None)
+    mtu: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=1500)
+    mtu_v6: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="mtuV6", validation_alias="mtuV6", default=None
     )
-    arp_timeout: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="arpTimeout", validation_alias="arpTimeout", default=Default[int](value=1200)
+    tcp_mss_adjust: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="tcpMssAdjust", validation_alias="tcpMssAdjust", default=None
     )
-    ip_directed_broadcast: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="ipDirectedBroadcast",
-        validation_alias="ipDirectedBroadcast",
-        default=Default[bool](value=False),
+    tcp_mss_adjust_v6: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        serialization_alias="tcpMssAdjustV6", validation_alias="tcpMssAdjustV6", default=None
     )
-    icmp_redirect_disable: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="icmpRedirectDisable",
-        validation_alias="icmpRedirectDisable",
-        default=Default[bool](value=True),
+    clear_dont_fragment: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="clearDontFragment",
+        validation_alias="clearDontFragment",
+        default=None,
     )
-
-
-class IPv4Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    address: StaticIPv4Address = Field(serialization_alias="addressV4", validation_alias="addressV4")
-    secondary_address: Optional[List[StaticIPv4Address]] = Field(
-        serialization_alias="secondaryAddressV4", validation_alias="secondaryAddressV4", default=None
+    dpd_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="dpdInterval", validation_alias="dpdInterval", default=None
     )
-    dhcp_helper: Optional[Union[Global[List[str]], Variable, Default[None]]] = Field(
-        serialization_alias="dhcpHelperV4", validation_alias="dhcpHelperV4", default=None
+    dpd_retries: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="dpdRetries", validation_alias="dpdRetries", default=None
     )
-
-
-class IPv6Address(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    address: Union[Global[str], Variable, Default[None]] = Field(
-        serialization_alias="addressV6", validation_alias="addressV6"
+    ike_version: Optional[Union[Global[int], Default[int]]] = Field(
+        serialization_alias="ikeVersion", validation_alias="ikeVersion", default=None
     )
-    secondary_address: Optional[List[StaticIPv6Address]] = Field(
-        serialization_alias="secondaryAddressV6", validation_alias="secondaryAddressV6", default=None
+    ike_mode: Optional[Union[Global[IkeMode], Variable, Default[IkeMode]]] = Field(
+        serialization_alias="ikeMode", validation_alias="ikeMode", default=None
     )
-    dhcp_helper: Optional[List[Dhcpv6Helper]] = Field(
-        serialization_alias="dhcpHelperV6", validation_alias="dhcpHelperV6", default=None
+    ike_rekey_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="ikeRekeyInterval", validation_alias="ikeRekeyInterval", default=None
     )
-
-
-class AclQos(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    ipv4_acl_egress: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv4AclEgress", validation_alias="ipv4AclEgress", default=None
+    ike_ciphersuite: Optional[Union[Global[IkeCiphersuite], Variable, Default[IkeCiphersuite]]] = Field(
+        serialization_alias="ikeCiphersuite",
+        validation_alias="ikeCiphersuite",
+        default=None,
     )
-    ipv4_acl_ingress: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv4AclIngress", validation_alias="ipv4AclIngress", default=None
+    ike_group: Optional[Union[Global[IkeGroup], Variable, Default[IkeGroup]]] = Field(
+        serialization_alias="ikeGroup", validation_alias="ikeGroup", default=None
     )
-    ipv6_acl_egress: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv6AclEgress", validation_alias="ipv6AclEgress", default=None
+    pre_shared_secret: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="preSharedSecret", validation_alias="preSharedSecret", default=None
     )
-    ipv6_acl_ingress: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv6AclIngress", validation_alias="ipv6AclIngress", default=None
+    ike_local_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="ikeLocalId", validation_alias="ikeLocalId", default=None
     )
-
-
-class InterfaceSviData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    shutdown: Union[Global[bool], Variable, Default[bool]] = Default[bool](value=True)
-    interface_name: Optional[Union[Global[str], Variable]] = Field(
-        serialization_alias="interfaceName", validation_alias="interfaceName"
+    ike_remote_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+        serialization_alias="ikeRemoteId", validation_alias="ikeRemoteId", default=None
     )
-    description: Optional[Union[Global[str], Variable, Default[None]]] = Default[None](value=None)
-    interface_mtu: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="ifMtu", validation_alias="ifMtu", default=Default[int](value=1500)
+    ipsec_rekey_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="ipsecRekeyInterval",
+        validation_alias="ipsecRekeyInterval",
+        default=None,
     )
-    ip_mtu: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="ipMtu", validation_alias="ipMtu", default=Default[int](value=1500)
+    ipsec_replay_window: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="ipsecReplayWindow", validation_alias="ipsecReplayWindow", default=None
     )
-    ipv4: Optional[IPv4Address] = None
-    ipv6: Optional[IPv6Address] = None
-    acl_qos: Optional[AclQos] = Field(serialization_alias="aclQos", validation_alias="aclQos", default=None)
-    arp: Optional[List[Arp]] = None
-    vrrp: Optional[List[VrrpIPv4]] = None
-    vrrp_ipv6: Optional[List[VrrpIPv6]] = Field(
-        serialization_alias="vrrpIpv6", validation_alias="vrrpIpv6", default=None
+    ipsec_ciphersuite: Optional[Union[Global[IpsecCiphersuite], Variable, Default[IpsecCiphersuite]]] = Field(
+        serialization_alias="ipsecCiphersuite",
+        validation_alias="ipsecCiphersuite",
+        default=None,
     )
-    dhcp_client_v6: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="dhcpClientV6", validation_alias="dhcpClientV6", default=Default[bool](value=False)
+    perfect_forward_secrecy: Optional[Union[Global[PfsGroup], Variable, Default[PfsGroup]]] = Field(
+        serialization_alias="perfectForwardSecrecy",
+        validation_alias="perfectForwardSecrecy",
+        default=None,
     )
-    advanced: AdvancedSviAttributes = AdvancedSviAttributes()
 
 
-class InterfaceSviCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class InterfaceGreParcel(_ParcelBase):
+    type_: Literal["lan/vpn/interface/gre"] = Field(default="lan/vpn/interface/gre", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    name: str
-    description: Optional[str] = None
-    data: InterfaceSviData
-    metadata: Optional[dict] = None
+    basic: BasicGre = Field(validation_alias=AliasPath("data", "basic"))
+    advanced: Optional[AdvancedGre] = Field(default=None, validation_alias=AliasPath("data", "advanced"))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Address, IPv6Address, IPv6Interface
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field, IPvAnyAddress
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.common import Prefix
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask
 
 ProtocolIPv4 = Literal[
     "bgp",
     "ospf",
     "opsfv3",
     "connected",
     "static",
@@ -93,18 +94,22 @@
 ]
 
 
 class DnsIPv4(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     primary_dns_address_ipv4: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="primaryDnsAddressIpv4", validation_alias="primaryDnsAddressIpv4"
+        default=Default[None](value=None),
+        serialization_alias="primaryDnsAddressIpv4",
+        validation_alias="primaryDnsAddressIpv4",
     )
     secondary_dns_address_ipv4: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="secondaryDnsAddressIpv4", validation_alias="secondaryDnsAddressIpv4"
+        default=Default[None](value=None),
+        serialization_alias="secondaryDnsAddressIpv4",
+        validation_alias="secondaryDnsAddressIpv4",
     )
 
 
 class DnsIPv6(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     primary_dns_address_ipv6: Union[Variable, Global[str], Default[None]] = Field(
@@ -115,40 +120,46 @@
     )
 
 
 class HostMapping(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     host_name: Union[Variable, Global[str]] = Field(serialization_alias="hostName", validation_alias="hostName")
-    list_of_ip: Union[Variable, Global[str]] = Field(serialization_alias="listOfIp", validation_alias="listOfIp")
+    list_of_ip: Union[Variable, Global[List[IPvAnyAddress]]] = Field(
+        serialization_alias="listOfIp", validation_alias="listOfIp"
+    )
 
 
 class RoutePrefix(BaseModel):
-    ip_address: Union[Variable, Global[str]] = Field(serialization_alias="ipAddress", validation_alias="ipAddress")
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+
+    ip_address: Union[Variable, Global[str], Global[IPv4Address], Global[IPv6Address]] = Field(
+        serialization_alias="ipAddress", validation_alias="ipAddress"
+    )
     subnet_mask: Union[Variable, Global[str]] = Field(serialization_alias="subnetMask", validation_alias="subnetMask")
 
 
 class IPv4Prefix(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    prefix: Prefix
+    prefix: AddressWithMask
     aggregate_only: Optional[Union[Global[bool], Default[bool]]] = Field(
         serialization_alias="aggregateOnly", validation_alias="aggregateOnly", default=None
     )
-    region: Optional[Union[Variable, Global[Region], Default[str]]] = None
+    region: Optional[Union[Variable, Global[Region], Default[Region]]] = None
 
 
 class IPv6Prefix(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    prefix: Union[Global[str], Variable]
+    prefix: Union[Global[str], Global[IPv6Interface], Variable]
     aggregate_only: Optional[Union[Global[bool], Default[bool]]] = Field(
         serialization_alias="aggregateOnly", validation_alias="aggregateOnly", default=None
     )
-    region: Optional[Union[Variable, Global[Region], Default[str]]] = None
+    region: Optional[Union[Variable, Global[Region], Default[Region]]] = None
 
 
 class OmpAdvertiseIPv4(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     omp_protocol: Union[Variable, Global[ProtocolIPv4]] = Field(
         serialization_alias="ompProtocol", validation_alias="ompProtocol"
@@ -170,15 +181,15 @@
     )
     prefix_list: Optional[List[IPv6Prefix]] = None
 
 
 class IPv4RouteGatewayNextHop(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    address: Union[Variable, Global[str]]
+    address: Union[Variable, Global[str], Global[IPv4Address]]
     distance: Union[Variable, Global[int], Default[int]] = Default[int](value=1)
 
 
 class IPv4RouteGatewayNextHopWithTracker(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     address: Union[Variable, Global[str]]
@@ -265,15 +276,15 @@
     address: Union[Variable, Global[str], Default[None]] = Default[None](value=None)
     distance: Union[Variable, Global[int], Default[int]] = Default[int](value=1)
 
 
 class NextHopInterfaceRouteIPv6(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    address: Union[Variable, Global[str], Default[None]] = Default[None](value=None)
+    address: Union[Variable, Global[str], Global[IPv6Address], Default[None]] = Default[None](value=None)
     distance: Union[Variable, Global[int], Default[int]] = Default[int](value=1)
 
 
 class IPStaticRouteInterface(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     interface_name: Union[Variable, Global[str]] = Field(
@@ -284,15 +295,17 @@
 
 class IPv6StaticRouteInterface(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     interface_name: Union[Variable, Global[str]] = Field(
         serialization_alias="interfaceName", validation_alias="interfaceName"
     )
-    next_hop: List[NextHopInterfaceRouteIPv6] = Field(serialization_alias="nextHop", validation_alias="nextHop")
+    interface_next_hop: List[NextHopInterfaceRouteIPv6] = Field(
+        serialization_alias="nextHop", validation_alias="nextHop"
+    )
 
 
 class InterfaceContainer(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     ip_static_route_interface: List[IPStaticRouteInterface] = Field(
         serialization_alias="ipStaticRouteInterface", validation_alias="ipStaticRouteInterface"
@@ -352,50 +365,54 @@
     )
     tracking: Union[Variable, Global[bool], Default[bool]] = Default[bool](value=True)
 
 
 class ServiceRoute(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    prefix: Prefix
+    prefix: AddressWithMask
     service: Union[Variable, Global[ServiceRouteType], Default[ServiceRouteType]] = Default[ServiceRouteType](
         value="SIG"
     )
     vpn: Global[int] = Global[int](value=0)
     sse_instance: Optional[Union[Variable, Global[str]]] = Field(
         serialization_alias="sseInstance", validation_alias="sseInstance", default=None
     )
 
 
 class StaticGreRouteIPv4(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    prefix: Prefix
-    interface: Union[Variable, Global[List[str]], Default[None]]
+    prefix: AddressWithMask
+    interface: Union[Variable, Global[List[str]], Default[None]] = Default[None](value=None)
     vpn: Global[int] = Global[int](value=0)
 
 
 class StaticIpsecRouteIPv4(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    prefix: Prefix
-    interface: Union[Variable, Global[List[str]], Default[None]]
+    prefix: AddressWithMask
+    interface: Union[Variable, Global[List[str]], Default[None]] = Default[None](value=None)
 
 
 class NatPool(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     nat_pool_name: Union[Variable, Global[int]] = Field(
         serialization_alias="natPoolName", validation_alias="natPoolName"
     )
     prefix_length: Union[Variable, Global[int]] = Field(
         serialization_alias="prefixLength", validation_alias="prefixLength"
     )
-    range_start: Union[Variable, Global[str]] = Field(serialization_alias="rangeStart", validation_alias="rangeStart")
-    range_end: Union[Variable, Global[str]] = Field(serialization_alias="rangeEnd", validation_alias="rangeEnd")
+    range_start: Union[Variable, Global[str], Global[IPv4Address]] = Field(
+        serialization_alias="rangeStart", validation_alias="rangeStart"
+    )
+    range_end: Union[Variable, Global[str], Global[IPv4Address]] = Field(
+        serialization_alias="rangeEnd", validation_alias="rangeEnd"
+    )
     overload: Union[Variable, Global[bool], Default[bool]] = Default[bool](value=True)
     direction: Union[Variable, Global[Direction]]
     tracking_object: Optional[dict] = Field(
         serialization_alias="trackingObject", validation_alias="trackingObject", default=None
     )
 
 
@@ -405,30 +422,34 @@
     nat_pool_name: Union[Variable, Global[int], Default[None]] = Field(
         serialization_alias="natPoolName", validation_alias="natPoolName"
     )
     source_port: Union[Variable, Global[int]] = Field(serialization_alias="sourcePort", validation_alias="sourcePort")
     translate_port: Union[Variable, Global[int]] = Field(
         serialization_alias="translatePort", validation_alias="translatePort"
     )
-    source_ip: Union[Variable, Global[str]] = Field(serialization_alias="sourceIp", validation_alias="sourceIp")
-    translated_source_ip: Union[Variable, Global[str]] = Field(
-        serialization_alias="TranslatedSourceIp", validation_alias="TranslatedSourceIp"
+    source_ip: Union[Variable, Global[str], Global[IPv4Address]] = Field(
+        serialization_alias="sourceIp", validation_alias="sourceIp"
+    )
+    translated_source_ip: Union[Variable, Global[str], Global[IPv4Address]] = Field(
+        serialization_alias="translatedSourceIp", validation_alias="translatedSourceIp"
     )
     protocol: Union[Variable, Global[NATPortForwardProtocol]]
 
 
 class StaticNat(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     nat_pool_name: Union[Variable, Global[int], Default[None]] = Field(
         serialization_alias="natPoolName", validation_alias="natPoolName"
     )
-    source_ip: Union[Variable, Global[str]] = Field(serialization_alias="sourceIp", validation_alias="sourceIp")
-    translated_source_ip: Union[Variable, Global[str]] = Field(
-        serialization_alias="TranslatedSourceIP", validation_alias="TranslatedSourceIP"
+    source_ip: Union[Variable, Global[str], Global[IPv4Address]] = Field(
+        serialization_alias="sourceIp", validation_alias="sourceIp"
+    )
+    translated_source_ip: Union[Variable, Global[str], Global[IPv4Address]] = Field(
+        serialization_alias="TranslatedSourceIp", validation_alias="TranslatedSourceIp"
     )
     static_nat_direction: Union[Variable, Global[Direction]] = Field(
         serialization_alias="staticNatDirection", validation_alias="staticNatDirection"
     )
     tracking_object: Optional[dict] = Field(
         serialization_alias="trackingObject", validation_alias="trackingObject", default=None
     )
@@ -437,15 +458,15 @@
 class StaticNatSubnet(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     source_ip_subnet: Union[Variable, Global[str]] = Field(
         serialization_alias="sourceIpSubnet", validation_alias="sourceIpSubnet"
     )
     translated_source_ip_subnet: Union[Variable, Global[str]] = Field(
-        serialization_alias="TranslatedSourceIpSubnet", validation_alias="TranslatedSourceIpSubnet"
+        serialization_alias="translatedSourceIpSubnet", validation_alias="translatedSourceIpSubnet"
     )
     prefix_length: Union[Variable, Global[int]] = Field(
         serialization_alias="prefixLength", validation_alias="prefixLength"
     )
     static_nat_direction: Union[Variable, Global[Direction]] = Field(
         serialization_alias="staticNatDirection", validation_alias="staticNatDirection"
     )
@@ -456,39 +477,39 @@
 
 class Nat64v4Pool(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     nat64_v4_pool_name: Union[Variable, Global[str]] = Field(
         serialization_alias="nat64V4PoolName", validation_alias="nat64V4PoolName"
     )
-    nat64_v4_pool_range_start: Union[Variable, Global[str]] = Field(
+    nat64_v4_pool_range_start: Union[Variable, Global[str], Global[IPv4Address]] = Field(
         serialization_alias="nat64V4PoolRangeStart", validation_alias="nat64V4PoolRangeStart"
     )
-    nat64_v4_pool_range_end: Union[Variable, Global[str]] = Field(
+    nat64_v4_pool_range_end: Union[Variable, Global[str], Global[IPv4Address]] = Field(
         serialization_alias="nat64V4PoolRangeEnd", validation_alias="nat64V4PoolRangeEnd"
     )
     nat64_v4_pool_overload: Union[Variable, Global[bool], Default[bool]] = Field(
         serialization_alias="nat64V4PoolOverload",
         validation_alias="nat64V4PoolOverload",
         default=Default[bool](value=False),
     )
 
 
 class RedistributeToService(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     protocol: Union[Variable, Global[RedistributeToServiceProtocol]]
-    policy: Union[Default[None], Global[UUID]]
+    policy: Union[Default[None], Global[UUID]] = Default[None](value=None)
 
 
 class RedistributeToGlobal(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     protocol: Union[Variable, Global[RedistributeToGlobalProtocol]]
-    policy: Union[Default[None], Global[UUID]]
+    policy: Union[Default[None], Global[UUID]] = Default[None](value=None)
 
 
 class RouteLeakFromGlobal(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     route_protocol: Union[Variable, Global[RouteLeakFromGlobalProtocol]] = Field(
         serialization_alias="routeProtocol", validation_alias="routeProtocol"
@@ -554,83 +575,69 @@
         serialization_alias="importRtList", validation_alias="importRtList", default=None
     )
     export_rt_list: Optional[List[RouteTarget]] = Field(
         serialization_alias="exportRtList", validation_alias="exportRtList", default=None
     )
 
 
-class LanVpnData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    vpn_id: Union[Variable, Global[int], Default[int]] = Field(serialization_alias="vpnId", validation_alias="vpnId")
-    name: Union[Variable, Global[str], Default[None]]
-    omp_admin_distance: Optional[Union[Variable, Global[int], Default[None]]] = Field(
-        serialization_alias="ompAdminDistance", validation_alias="ompAdminDistance", default=None
+class LanVpnParcel(_ParcelBase):
+    type_: Literal["lan/vpn"] = Field(default="lan/vpn", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    vpn_id: Union[Variable, Global[int]] = Field(validation_alias=AliasPath("data", "vpnId"))
+    vpn_name: Union[Variable, Global[str], Default[None]] = Field(
+        default=Default[None](value=None), validation_alias=AliasPath("data", "name")
+    )
+    omp_admin_distance_ipv4: Optional[Union[Variable, Global[int], Default[None]]] = Field(
+        validation_alias=AliasPath("data", "ompAdminDistance"), default=None
     )
     omp_admin_distance_ipv6: Optional[Union[Variable, Global[int], Default[None]]] = Field(
-        serialization_alias="ompAdminDistanceIpv6", validation_alias="ompAdminDistanceIpv6", default=None
+        validation_alias=AliasPath("data", "ompAdminDistanceIpv6"), default=None
     )
-    dns_ipv4: Optional[DnsIPv4] = Field(serialization_alias="dnsIpv4", validation_alias="dnsIpv4", default=None)
-    dns_ipv6: Optional[DnsIPv6] = Field(serialization_alias="dnsIpv6", validation_alias="dnsIpv6", default=None)
+    dns_ipv4: Optional[DnsIPv4] = Field(validation_alias=AliasPath("data", "dnsIpv4"), default=None)
+    dns_ipv6: Optional[DnsIPv6] = Field(validation_alias=AliasPath("data", "dnsIpv6"), default=None)
     new_host_mapping: Optional[List[HostMapping]] = Field(
-        serialization_alias="newHostMapping", validation_alias="newHostMapping", default=None
+        validation_alias=AliasPath("data", "newHostMapping"), default=None
     )
     omp_advertise_ipv4: Optional[List[OmpAdvertiseIPv4]] = Field(
-        serialization_alias="ompAdvertiseIpv4", validation_alias="ompAdvertiseIpv4", default=None
+        validation_alias=AliasPath("data", "ompAdvertiseIp4"), default=None  # API typo
     )
     omp_advertise_ipv6: Optional[List[OmpAdvertiseIPv6]] = Field(
-        serialization_alias="ompAdvertiseIpv6", validation_alias="ompAdvertiseIpv6", default=None
-    )
-    ipv4_route: Optional[List[StaticRouteIPv4]] = Field(
-        serialization_alias="ipv4Route", validation_alias="ipv4Route", default=None
-    )
-    ipv6_route: Optional[List[StaticRouteIPv6]] = Field(
-        serialization_alias="ipv6Route", validation_alias="ipv6Route", default=None
+        validation_alias=AliasPath("data", "ompAdvertiseIpv6"), default=None
     )
-    service: Optional[List[Service]] = None
+    ipv4_route: Optional[List[StaticRouteIPv4]] = Field(validation_alias=AliasPath("data", "ipv4Route"), default=None)
+    ipv6_route: Optional[List[StaticRouteIPv6]] = Field(validation_alias=AliasPath("data", "ipv6Route"), default=None)
+    service: Optional[List[Service]] = Field(default=None, validation_alias=AliasPath("data", "service"))
     service_route: Optional[List[ServiceRoute]] = Field(
-        serialization_alias="serviceRoute", validation_alias="serviceRoute", default=None
-    )
-    gre_route: Optional[List[StaticGreRouteIPv4]] = Field(
-        serialization_alias="greRoute", validation_alias="greRoute", default=None
+        validation_alias=AliasPath("data", "serviceRoute"), default=None
     )
+    gre_route: Optional[List[StaticGreRouteIPv4]] = Field(validation_alias=AliasPath("data", "greRoute"), default=None)
     ipsec_route: Optional[List[StaticIpsecRouteIPv4]] = Field(
-        serialization_alias="ipsecRoute", validation_alias="ipsecRoute", default=None
+        validation_alias=AliasPath("data", "ipsecRoute"), default=None
     )
-    nat_pool: Optional[List[NatPool]] = Field(serialization_alias="natPool", validation_alias="natPool", default=None)
+    nat_pool: Optional[List[NatPool]] = Field(validation_alias=AliasPath("data", "natPool"), default=None)
     nat_port_forwarding: Optional[List[NatPortForward]] = Field(
-        serialization_alias="natPortForwarding", validation_alias="natPortForwarding", default=None
-    )
-    static_nat: Optional[List[StaticNat]] = Field(
-        serialization_alias="staticNat", validation_alias="staticNat", default=None
+        validation_alias=AliasPath("data", "natPortForwarding"), default=None
     )
+    static_nat: Optional[List[StaticNat]] = Field(validation_alias=AliasPath("data", "staticNat"), default=None)
     static_nat_subnet: Optional[List[StaticNatSubnet]] = Field(
-        serialization_alias="staticNatSubnet", validation_alias="staticNatSubnet", default=None
-    )
-    nat64_v4_pool: Optional[List[Nat64v4Pool]] = Field(
-        serialization_alias="nat64V4Pool", validation_alias="nat64V4Pool", default=None
+        validation_alias=AliasPath("data", "staticNatSubnet"), default=None
     )
+    nat64_v4_pool: Optional[List[Nat64v4Pool]] = Field(validation_alias=AliasPath("data", "nat64V4Pool"), default=None)
     route_leak_from_global: Optional[List[RouteLeakFromGlobal]] = Field(
-        serialization_alias="routeLeakFromGlobal", validation_alias="routeLeakFromGlobal", default=None
+        validation_alias=AliasPath("data", "routeLeakFromGlobal"), default=None
     )
     route_leak_from_service: Optional[List[RouteLeakFromService]] = Field(
-        serialization_alias="routeLeakFromService", validation_alias="routeLeakFromService", default=None
+        validation_alias=AliasPath("data", "routeLeakFromService"), default=None
     )
     route_leak_between_services: Optional[List[RouteLeakBetweenServices]] = Field(
-        serialization_alias="routeLeakBetweenServices", validation_alias="routeLeakBetweenServices", default=None
+        validation_alias=AliasPath("data", "routeLeakBetweenServices"), default=None
     )
     mpls_vpn_ipv4_route_target: Optional[MplsVpnIPv4RouteTarget] = Field(
-        serialization_alias="mplsVpnIpv4RouteTarget", validation_alias="mplsVpnIpv4RouteTarget", default=None
+        validation_alias=AliasPath("data", "mplsVpnIpv4RouteTarget"), default=None
     )
     mpls_vpn_ipv6_route_target: Optional[MplsVpnIPv6RouteTarget] = Field(
-        serialization_alias="mplsVpnIpv6RouteTarget", validation_alias="mplsVpnIpv6RouteTarget", default=None
+        validation_alias=AliasPath("data", "mplsVpnIpv6RouteTarget"), default=None
     )
     enable_sdra: Optional[Union[Global[bool], Default[bool]]] = Field(
-        serialization_alias="enableSdra", validation_alias="enableSdra", default=None
+        validation_alias=AliasPath("data", "enableSdra"), default=None
     )
-
-
-class LanVpnCreationPayload(BaseModel):
-    name: str
-    description: Optional[str] = None
-    data: LanVpnData
-    metadata: Optional[dict] = None
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,243 +1,242 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Optional, Union
+from ipaddress import IPv4Address
+from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+
+SptThreshold = Literal["infinity", "0"]
 
 
 class LocalConfig(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     local: Union[Global[bool], Variable, Default[bool]] = Default[bool](value=False)
     threshold: Optional[Union[Global[int], Variable, Default[None]]] = Default[None](value=None)
 
 
 class MulticastBasicAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     spt_only: Union[Global[bool], Variable, Default[bool]] = Field(
         serialization_alias="sptOnly", validation_alias="sptOnly", default=Default[bool](value=False)
     )
     local_config: LocalConfig = Field(
         serialization_alias="localConfig", validation_alias="localConfig", default=LocalConfig()
     )
 
 
 class StaticJoin(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    group_address: Union[Global[str], Variable] = Field(
-        serialization_alias="groupAddress", validation_alias="groupAddress"
+    group_address: Union[Global[IPv4Address], Variable] = Field(
+        serialization_alias="groupAddress",
+        validation_alias="groupAddress",
+        description="Address range: 224.0.0.0 ~ 239.255.255.255",
     )
-    source_address: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+    source_address: Optional[Union[Global[IPv4Address], Variable, Default[None]]] = Field(
         serialization_alias="sourceAddress", validation_alias="sourceAddress", default=Default[None](value=None)
     )
 
 
 class IgmpInterfaceParameters(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     interface_name: Union[Global[str], Variable] = Field(
         serialization_alias="interfaceName", validation_alias="interfaceName"
     )
     version: Union[Global[int], Default[int]] = Default[int](value=2)
     join_group: Optional[List[StaticJoin]] = Field(
         serialization_alias="joinGroup", validation_alias="joinGroup", default=None
     )
 
 
 class IgmpAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     interface: List[IgmpInterfaceParameters]
 
 
-class SmmFlag(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    enable_ssm_flag: Global[bool] = Global[bool](value=True)
-    range: Optional[Union[Global[str], Variable, Default[None]]] = Default[None](value=None)
-
+class SsmFlag(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-class SptThreshold:
-    INFINITY = "infinity"
-    ZERO = "0"
+    enable_ssm_flag: Global[bool] = Field(
+        default=Global[bool](value=True), serialization_alias="enableSSMFlag", validation_alias="enableSSMFlag"
+    )
+    range: Union[Global[str], Variable, Default[None]] = Default[None](value=None)
 
 
-class SsmAttrubutes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class SsmAttributes(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    ssm_range_config: SmmFlag = Field(serialization_alias="ssmRangeConfig", validation_alias="ssmRangeConfig")
+    ssm_range_config: SsmFlag = Field(serialization_alias="ssmRangeConfig", validation_alias="ssmRangeConfig")
     spt_threshold: Optional[Union[Global[SptThreshold], Variable, Default[SptThreshold]]] = Field(
         serialization_alias="sptThreshold",
         validation_alias="sptThreshold",
-        default=Default[SptThreshold](value=SptThreshold.ZERO),
+        default=Default[SptThreshold](value="0"),
     )
 
 
 class PimInterfaceParameters(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     interface_name: Union[Global[str], Variable] = Field(
         serialization_alias="interfaceName", validation_alias="interfaceName"
     )
     query_interval: Union[Global[int], Variable, Default[int]] = Field(
         serialization_alias="queryInterval", validation_alias="queryInterval", default=Default[int](value=30)
     )
     join_prune_interval: Union[Global[int], Variable, Default[int]] = Field(
         serialization_alias="joinPruneInterval", validation_alias="joinPruneInterval", default=Default[int](value=60)
     )
 
 
 class StaticRpAddress(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    address: Union[Global[str], Variable]
+    address: Union[Global[IPv4Address], Variable]
     access_list: Union[Global[str], Variable] = Field(serialization_alias="accessList", validation_alias="accessList")
     override: Optional[Union[Global[bool], Variable, Default[bool]]] = Default[bool](value=False)
 
 
 class RPAnnounce(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     interface_name: Union[Global[str], Variable] = Field(
         serialization_alias="interfaceName", validation_alias="interfaceName"
     )
     scope: Union[Global[int], Variable]
 
 
 class AutoRpAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     enable_auto_rp_flag: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="enableAutoRPFlag", validation_alias="enableAutoRPFlag", default=Default[bool](value=False)
     )
     send_rp_announce_list: Optional[List[RPAnnounce]] = Field(
         serialization_alias="sendRpAnnounceList", validation_alias="sendRpAnnounceList", default=None
     )
     send_rp_discovery: Optional[List[RPAnnounce]] = Field(
         serialization_alias="sendRpDiscovery", validation_alias="sendRpDiscovery", default=None
     )
 
 
 class RpDiscoveryScope(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     interface_name: Union[Global[str], Variable] = Field(
         serialization_alias="interfaceName", validation_alias="interfaceName"
     )
     group_list: Optional[Union[Global[str], Variable, Default[None]]] = Field(
         serialization_alias="groupList", validation_alias="groupList", default=None
     )
     interval: Optional[Union[Global[int], Variable, Default[None]]] = None
     priority: Optional[Union[Global[int], Variable, Default[None]]] = None
 
 
 class BsrCandidateAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     interface_name: Union[Global[str], Variable] = Field(
         serialization_alias="interfaceName", validation_alias="interfaceName"
     )
     mask: Optional[Union[Global[int], Variable, Default[None]]] = None
     priority: Optional[Union[Global[int], Variable, Default[None]]] = None
     accept_rp_candidate: Optional[Union[Global[str], Variable, Default[None]]] = Field(
         serialization_alias="acceptRpCandidate", validation_alias="acceptRpCandidate", default=None
     )
 
 
 class PimBsrAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     rp_candidate: Optional[List[RpDiscoveryScope]] = Field(
         serialization_alias="rpCandidate", validation_alias="rpCandidate", default=None
     )
     bsr_candidate: Optional[List[BsrCandidateAttributes]] = Field(
-        serialization_alias="bsdCandidate", validation_alias="bsdCandidate", default=None
+        serialization_alias="bsrCandidate", validation_alias="bsrCandidate", default=None
     )
 
 
 class PimAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    ssm: SsmAttrubutes
+    ssm: SsmAttributes
     interface: Optional[List[PimInterfaceParameters]] = None
-    rp_addres: Optional[List[StaticRpAddress]] = Field(
+    rp_address: Optional[List[StaticRpAddress]] = Field(
         serialization_alias="rpAddr", validation_alias="rpAddr", default=None
     )
     auto_rp: Optional[AutoRpAttributes] = Field(serialization_alias="autoRp", validation_alias="autoRp", default=None)
     pim_bsr: Optional[PimBsrAttributes] = Field(serialization_alias="pimBsr", validation_alias="pimBsr", default=None)
 
 
 class DefaultMsdpPeer(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     default_peer: Union[Global[bool], Default[bool]]
     prefix_list: Optional[Global[UUID]] = None
 
 
 class MsdpPeerAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    peer_ip: Union[Global[str], Variable] = Field(serialization_alias="peerIp", validation_alias="peerIp")
+    peer_ip: Union[Global[IPv4Address], Variable] = Field(serialization_alias="peerIp", validation_alias="peerIp")
     connect_source_intf: Optional[Union[Global[str], Variable, Default[None]]] = Field(
         serialization_alias="connectSourceIntf", validation_alias="connectSourceIntf", default=None
     )
     remote_as: Optional[Union[Global[int], Variable, Default[None]]] = Field(
         serialization_alias="remoteAs", validation_alias="remoteAs", default=None
     )
     password: Optional[Union[Global[str], Variable, Default[None]]] = None
     keepalive_interval: Optional[Union[Global[int], Variable, Default[None]]] = Field(
         serialization_alias="keepaliveInterval", validation_alias="keepaliveInterval", default=None
     )
     keepalive_holdtime: Optional[Union[Global[int], Variable, Default[None]]] = Field(
-        serialization_alias="keepaliveHoldTime", validation_alias="keepaliveHoldTime", default=None
+        serialization_alias="keepaliveHoldTime",
+        validation_alias="keepaliveHoldTime",
+        default=None,
+        description="Hold-Time must be higher than Keep Alive",
     )
     sa_limit: Optional[Union[Global[int], Variable, Default[None]]] = Field(
         serialization_alias="saLimit", validation_alias="saLimit", default=None
     )
     default: Optional[DefaultMsdpPeer] = None
 
 
 class MsdpPeer(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     mesh_group: Optional[Union[Global[str], Variable, Default[None]]] = Field(
         serialization_alias="meshGroup", validation_alias="meshGroup", default=None
     )
     peer: List[MsdpPeerAttributes]
 
 
 class MsdpAttributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     msdp_list: Optional[List[MsdpPeer]] = Field(
         serialization_alias="msdpList", validation_alias="msdpList", default=None
     )
     originator_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
         serialization_alias="originatorId", validation_alias="originatorId", default=None
     )
     refresh_timer: Optional[Union[Global[int], Variable, Default[None]]] = Field(
         serialization_alias="refreshTimer", validation_alias="refreshTimer", default=None
     )
 
 
-class MulticastData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    basic: MulticastBasicAttributes = MulticastBasicAttributes()
-    igmp: Optional[IgmpAttributes] = None
-    pim: Optional[PimAttributes] = None
-    msdp: Optional[MsdpAttributes] = None
-
-
-class MulticastCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: MulticastData
-    metadata: Optional[dict] = None
+class MulticastParcel(_ParcelBase):
+    type_: Literal["routing/multicast"] = Field(default="routing/multicast", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    basic: MulticastBasicAttributes = Field(
+        validation_alias=AliasPath("data", "basic"), default_factory=MulticastBasicAttributes
+    )
+    igmp: Optional[IgmpAttributes] = Field(default=None, validation_alias=AliasPath("data", "igmp"))
+    pim: Optional[PimAttributes] = Field(default=None, validation_alias=AliasPath("data", "pim"))
+    msdp: Optional[MsdpAttributes] = Field(default=None, validation_alias=AliasPath("data", "msdp"))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
 
-ObjectTrackerType = Literal[
-    "Interface",
-    "SIG",
-    "Route",
+EndpointProtocol = Literal[
+    "tcp",
+    "udp",
 ]
 
+TrackerType = Literal["endpoint"]
 
-Criteria = Literal[
+EndpointTrackerType = Literal["static-route"]
+
+CombineBoolean = Literal[
     "and",
     "or",
 ]
 
 
-class SigTracker(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class EndpointTcpUdp(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
-    object_tracker_type: Global[ObjectTrackerType] = Field(
-        serialization_alias="objectTrackerType",
-        validation_alias="objectTrackerType",
-        default=Global[ObjectTrackerType](value="SIG"),
-    )
+    protocol: Optional[Union[Variable, Global[EndpointProtocol]]] = None
+    port: Optional[Union[Variable, Global[int]]] = None
 
 
-class InterfaceTracker(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class TrackerData(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
-    object_tracker_type: Global[ObjectTrackerType] = Field(
-        serialization_alias="objectTrackerType",
-        validation_alias="objectTrackerType",
-        default=Global[ObjectTrackerType](value="Interface"),
+    name: Union[Variable, Global[str]] = Field(serialization_alias="trackerName", validation_alias="trackerName")
+    endpoint_api_url: Optional[Union[Variable, Global[str]]] = Field(
+        serialization_alias="endpointApiUrl", validation_alias="endpointApiUrl", default=None
     )
-    interface: Union[Global[str], Variable]
-
-
-class RouteTracker(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
-    object_tracker_type: Global[ObjectTrackerType] = Field(
-        serialization_alias="objectTrackerType",
-        validation_alias="objectTrackerType",
-        default=Global[ObjectTrackerType](value="Route"),
+    endpoint_dns_name: Optional[Union[Variable, Global[str]]] = Field(
+        serialization_alias="endpointDnsName", validation_alias="endpointDnsName", default=None
+    )
+    endpoint_ip: Optional[Union[Variable, Global[str]]] = Field(
+        serialization_alias="endpointIp", validation_alias="endpointIp", default=None
+    )
+    endpoint_tcp_udp: Optional[EndpointTcpUdp] = Field(
+        serialization_alias="endpointTcpUdp", validation_alias="endpointTcpUdp", default=None
     )
-    route_ip: Union[Global[str], Variable] = Field(serialization_alias="routeIp", validation_alias="routeIp")
-    route_mask: Union[Global[str], Variable, Default[str]] = Field(
-        serialization_alias="routeMask", validation_alias="routeMask"
+    interval: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=60)
+    multiplier: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=3)
+    threshold: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=300)
+    endpoint_tracker_type: Optional[Union[Global[EndpointTrackerType], Variable, Default[EndpointTrackerType]]] = Field(
+        serialization_alias="endpointTrackerType",
+        validation_alias="endpointTrackerType",
+        default=Default[EndpointTrackerType](value="static-route"),
+    )
+    tracker_type: Optional[Union[Global[TrackerType], Variable, Default[TrackerType]]] = Field(
+        serialization_alias="trackerType",
+        validation_alias="trackerType",
+        default=Default[TrackerType](value="endpoint"),
     )
-    vpn: Union[Global[int], Variable, Default[None]] = Default[None](value=None)
 
 
-class ObjectTrackerCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class TrackerCreationPayload(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     name: str
     description: Optional[str] = None
-    data: Union[InterfaceTracker, RouteTracker, SigTracker]
+    data: TrackerData
+    metadata: Optional[dict] = None
 
 
-class ObjectTrackerRef(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class TrackerRef(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     tracker_ref: Global[UUID] = Field(serialization_alias="trackerRef", validation_alias="trackerRef")
 
 
-class ObjectTrackerGroupData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    object_id: Union[Global[int], Variable] = Field(serialization_alias="objectId", validation_alias="objectId")
-    tracker_refs: List[ObjectTrackerRef] = Field(serialization_alias="trackerRefs", validation_alias="trackerRefs")
-    criteria: Union[Global[Criteria], Variable, Default[Criteria]] = Default[Criteria](value="or")
+class TrackerGroupParcel(_ParcelBase):
+    type_: Literal["trackergroup"] = Field(default="trackergroup", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    tracker_refs: List[TrackerRef] = Field(validation_alias=AliasPath("data", "trackerRefs"))
+    combine_boolean: Union[Global[CombineBoolean], Variable, Default[CombineBoolean]] = Field(
+        validation_alias=AliasPath("data", "combineBoolean"),
+        default=Default[CombineBoolean](value="or"),
+    )
 
 
-class ObjectTrackerGroupCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class TrackerAssociationPayload(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    name: str
-    description: Optional[str] = None
-    data: ObjectTrackerGroupData
-    metadata: Optional[dict] = None
+    parcel_id: str = Field(serialization_alias="parcelId", validation_alias="parcelId")
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Address
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default
+from catalystwan.models.common import MetricType
 
 NetworkType = Literal[
     "broadcast",
     "point-to-point",
     "non-broadcast",
     "point-to-multipoint",
 ]
@@ -22,45 +24,43 @@
 ]
 
 AdvertiseType = Literal[
     "administrative",
     "on-startup",
 ]
 
-RedistributeProtocol = Literal[
+RedistributeProtocolOspf = Literal[
     "static",
     "connected",
     "bgp",
     "omp",
     "nat",
     "eigrp",
 ]
 
-MetricType = Literal["type1", "type2"]
-
 
 class SummaryPrefix(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     ip_address: Optional[Union[Global[str], Variable]] = None
     subnet_mask: Optional[Union[Global[str], Variable]] = None
 
 
 class SummaryRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     address: Optional[SummaryPrefix] = None
     cost: Optional[Union[Global[int], Variable, Default[None]]] = None
     no_advertise: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="noAdvertise", validation_alias="noAdvertise", default=None
     )
 
 
 class OspfInterfaceParametres(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     name: Optional[Union[Global[str], Variable]]
     hello_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="helloInterval", validation_alias="helloInterval", default=None
     )
     dead_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="deadInterval", validation_alias="deadInterval", default=None
@@ -82,84 +82,88 @@
     message_digest_key: Optional[Union[Global[int], Variable, Default[None]]] = Field(
         serialization_alias="messageDigestKey", validation_alias="messageDigestKey", default=None
     )
     md5: Optional[Union[Global[str], Variable, Default[None]]] = None
 
 
 class OspfArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_number: Union[Global[int], Variable] = Field(serialization_alias="aNum", validation_alias="aNum")
     area_type: Optional[Union[Global[AreaType], Default[None]]] = Field(
         serialization_alias="aType", validation_alias="aType", default=None
     )
     no_summary: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="noSummary", validation_alias="noSummary", default=None
     )
     interface: Optional[List[OspfInterfaceParametres]] = None
-    range: Optional[List[SummaryRoute]]
+    range: Optional[List[SummaryRoute]] = None
 
 
 class RouterLsa(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     ad_type: Global[AdvertiseType] = Field(serialization_alias="adType", validation_alias="adType")
     time: Optional[Union[Global[int], Variable]] = None
 
 
 class RedistributedRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    protocol: Union[Global[RedistributeProtocol], Variable]
+    protocol: Union[Global[RedistributeProtocolOspf], Variable]
     dia: Optional[Union[Global[bool], Variable, Default[bool]]] = None
-    route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
+    route_policy: Optional[Union[Default[None], Global[str], Global[UUID]]] = Field(
         serialization_alias="routePolicy", validation_alias="routePolicy", default=None
     )
 
 
-class OspfData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class OspfParcel(_ParcelBase):
+    type_: Literal["routing/ospf"] = Field(default="routing/ospf", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    router_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
-        serialization_alias="routerId", validation_alias="routerId", default=None
+    router_id: Union[Global[str], Global[IPv4Address], Variable, Default[None]] = Field(
+        validation_alias=AliasPath("data", "routerId"), default=Default[None](value=None)
+    )
+    reference_bandwidth: Union[Global[int], Variable, Default[int]] = Field(
+        validation_alias=AliasPath("data", "referenceBandwidth"), default=as_default(100)
+    )
+    rfc1583: Union[Global[bool], Variable, Default[bool]] = Field(
+        validation_alias=AliasPath("data", "rfc1583"), default=as_default(True)
     )
-    reference_bandwidth: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="referenceBandwidth", validation_alias="referenceBandwidth", default=None
+    originate: Union[Global[bool], Default[bool]] = Field(
+        validation_alias=AliasPath("data", "originate"), default=as_default(False)
+    )
+    always: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        validation_alias=AliasPath("data", "always"), default=None
+    )
+    metric: Optional[Union[Global[int], Variable, Default[None]]] = Field(
+        validation_alias=AliasPath("data", "metric"), default=None
     )
-    rfc1583: Optional[Union[Global[bool], Variable, Default[bool]]] = None
-    originate: Optional[Union[Global[bool], Default[bool]]] = None
-    always: Optional[Union[Global[bool], Variable, Default[bool]]] = None
-    metric: Optional[Union[Global[int], Variable, Default[None]]] = None
     metric_type: Optional[Union[Global[MetricType], Variable, Default[None]]] = Field(
-        serialization_alias="metricType", validation_alias="metricType", default=None
+        validation_alias=AliasPath("data", "metricType"), default=None
+    )
+    external: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        default=as_default(110), validation_alias=AliasPath("data", "external")
     )
-    external: Optional[Union[Global[int], Variable, Default[int]]] = None
     inter_area: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="interArea", validation_alias="interArea", default=None
+        validation_alias=AliasPath("data", "interArea"), default=as_default(110)
     )
     intra_area: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="intraArea", validation_alias="intraArea", default=None
+        validation_alias=AliasPath("data", "intraArea"), default=as_default(110)
+    )
+    delay: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        validation_alias=AliasPath("data", "delay"), default=as_default(200)
     )
-    delay: Optional[Union[Global[int], Variable, Default[int]]] = None
     initial_hold: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="initialHold", validation_alias="initialHold", default=None
+        validation_alias=AliasPath("data", "initialHold"), default=as_default(1000)
     )
     max_hold: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="maxHold", validation_alias="maxHold", default=None
+        validation_alias=AliasPath("data", "maxHold"), default=as_default(10000)
     )
-    redistribute: Optional[List[RedistributedRoute]] = None
-    router_lsa: Optional[List[RouterLsa]] = Field(
-        serialization_alias="routerLsa", validation_alias="routerLsa", default=None
+    redistribute: Optional[List[RedistributedRoute]] = Field(
+        validation_alias=AliasPath("data", "redistribute"), default=None
     )
-    route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
-        serialization_alias="routePolicy", validation_alias="routePolicy", default=None
+    router_lsa: Optional[List[RouterLsa]] = Field(validation_alias=AliasPath("data", "routerLsa"), default=None)
+    route_policy: Optional[Union[Default[None], Global[str], Global[UUID]]] = Field(
+        validation_alias=AliasPath("data", "routePolicy"), default=None
     )
-    area: Optional[List[OspfArea]] = None
-
-
-class OspfCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: OspfData
-    metadata: Optional[dict] = None
+    area: Optional[List[OspfArea]] = Field(validation_alias=AliasPath("data", "area"), default=None)
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Address, IPv6Interface
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
-from catalystwan.models.configuration.feature_profile.common import Prefix
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.common import MetricType
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask
 
 NetworkType = Literal[
     "broadcast",
     "point-to-point",
     "non-broadcast",
     "point-to-multipoint",
 ]
@@ -36,41 +38,40 @@
 RedistributeProtocolIPv6 = Literal[
     "static",
     "connected",
     "bgp",
     "omp",
     "eigrp",
 ]
-MetricType = Literal["type1", "type2"]
 
 
 class NoAuth(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     auth_type: Union[Global[NoAuthType], Default[NoAuthType]] = Field(
         serialization_alias="authType",
         validation_alias="authType",
         default=Default[NoAuthType](value="no-auth"),
     )
 
 
 class IpsecSha1Auth(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     auth_type: Global[IpsecSha1AuthType] = Field(
         serialization_alias="authType",
         validation_alias="authType",
         default=Global[IpsecSha1AuthType](value="ipsec-sha1"),
     )
     spi: Union[Global[int], Variable]
     auth_key: Union[Global[str], Variable] = Field(serialization_alias="authKey", validation_alias="authKey")
 
 
 class Ospfv3InterfaceParametres(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     name: Optional[Union[Global[str], Variable]] = Field(serialization_alias="ifName", validation_alias="ifName")
     hello_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="helloInterval", validation_alias="helloInterval", default=None
     )
     dead_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="deadInterval", validation_alias="deadInterval", default=None
@@ -88,145 +89,147 @@
     )
     authentication_config: Optional[Union[NoAuth, IpsecSha1Auth]] = Field(
         serialization_alias="authenticationConfig", validation_alias="authenticationConfig", default=None
     )
 
 
 class SummaryRouteIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    network: Union[Global[str], Variable]
+    network: Union[Global[str], Global[IPv6Interface], Variable]
     no_advertise: Union[Global[bool], Variable, Default[bool]] = Field(
-        serialization_alias="noAdvertise", validation_alias="noAdvertise"
+        serialization_alias="noAdvertise", validation_alias="noAdvertise", default=Default[bool](value=False)
     )
     cost: Optional[Union[Global[int], Variable, Default[None]]] = None
 
 
 class SummaryRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    network: Optional[Prefix] = None
+    network: Optional[AddressWithMask] = None
     cost: Optional[Union[Global[int], Variable, Default[None]]] = None
     no_advertise: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="noAdvertise", validation_alias="noAdvertise", default=None
     )
 
 
 class StubArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_type: Global[str] = Field(
         serialization_alias="areaType", validation_alias="areaType", default=Global[str](value="stub")
     )
     no_summary: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="noSummary", validation_alias="noSummary", default=None
     )
 
 
 class NssaArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_type: Global[str] = Field(
         serialization_alias="areaType", validation_alias="areaType", default=Global[str](value="nssa")
     )
     no_summary: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="noSummary", validation_alias="noSummary", default=None
     )
     always_translate: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="alwaysTranslate", validation_alias="alwaysTranslate", default=None
     )
 
 
 class NormalArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_type: Global[str] = Field(
         serialization_alias="areaType", validation_alias="areaType", default=Global[str](value="normal")
     )
 
 
 class DefaultArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_type: Default[None] = Field(
         serialization_alias="areaType", validation_alias="areaType", default=Default[None](value=None)
     )
 
 
 class Ospfv3IPv4Area(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_number: Union[Global[int], Variable] = Field(serialization_alias="areaNum", validation_alias="areaNum")
     area_type_config: Optional[Union[StubArea, NssaArea, NormalArea, DefaultArea]] = Field(
         serialization_alias="areaTypeConfig", validation_alias="areaTypeConfig", default=None
     )
-    interfaces: List[Ospfv3InterfaceParametres]
+    interfaces: List[Ospfv3InterfaceParametres] = Field(min_length=1)
     ranges: Optional[List[SummaryRoute]] = None
 
 
 class Ospfv3IPv6Area(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     area_number: Union[Global[int], Variable] = Field(serialization_alias="areaNum", validation_alias="areaNum")
     area_type_config: Optional[Union[StubArea, NssaArea, NormalArea, DefaultArea]] = Field(
         serialization_alias="areaTypeConfig", validation_alias="areaTypeConfig", default=None
     )
-    interfaces: List[Ospfv3InterfaceParametres]
-    ranges: Optional[List[SummaryRoute]] = None
+    interfaces: List[Ospfv3InterfaceParametres] = Field(min_length=1)
+    ranges: Optional[List[SummaryRouteIPv6]] = None
 
 
 class MaxMetricRouterLsa(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     action: Global[MaxMetricRouterLsaAction]
     on_startup_time: Optional[Union[Global[int], Variable]] = Field(
         serialization_alias="onStartUpTime", validation_alias="onStartUpTime", default=None
     )
 
 
 class RedistributedRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     protocol: Union[Global[RedistributeProtocol], Variable]
     nat_dia: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="natDia", validation_alias="natDia", default=None
     )
     route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="routePolicy", validation_alias="routePolicy", default=None
     )
 
 
 class RedistributedRouteIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     protocol: Union[Global[RedistributeProtocolIPv6], Variable]
     route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="routePolicy", validation_alias="routePolicy", default=None
     )
 
 
 class DefaultOriginate(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     originate: Union[Global[bool], Default[bool]]
     always: Optional[Union[Global[bool], Variable, Default[bool]]] = None
     metric: Optional[Union[Global[str], Variable, Default[None]]] = None
-    metricType: Optional[Union[Global[MetricType], Variable, Default[None]]] = None
+    metric_type: Optional[Union[Global[MetricType], Variable, Default[None]]] = Field(
+        default=None, serialization_alias="metricType", validation_alias="metricType"
+    )
 
 
 class SpfTimers(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     delay: Optional[Union[Global[int], Variable, Default[int]]] = None
     initial_hold: Optional[Union[Global[int], Variable, Default[int]]] = None
     max_hold: Optional[Union[Global[int], Variable, Default[int]]] = None
 
 
 class AdvancedOspfv3Attributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     reference_bandwidth: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="referenceBandwidth", validation_alias="referenceBandwidth", default=None
     )
     compatible_rfc1583: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
         serialization_alias="compatibleRfc1583", validation_alias="compatibleRfc1583", default=None
     )
@@ -237,63 +240,52 @@
     policy_name: Optional[Union[Default[None], Global[UUID]]] = Field(
         serialization_alias="policyName", validation_alias="policyName", default=None
     )
     filter: Optional[Union[Global[bool], Variable, Default[bool]]] = None
 
 
 class BasicOspfv3Attributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    router_id: Optional[Union[Global[str], Variable, Default[None]]] = Field(
+    router_id: Optional[Union[Global[str], Global[IPv4Address], Variable, Default[None]]] = Field(
         serialization_alias="routerId", validation_alias="routerId", default=None
     )
     distance: Optional[Union[Global[int], Variable, Default[int]]] = None
     external_distance: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="externalDistance", validation_alias="externalDistance", default=None
     )
     inter_area_distance: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="interAreaDistance", validation_alias="interAreaDistance", default=None
     )
     intra_area_distance: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="intraAreaDistance", validation_alias="intraAreaDistance", default=None
     )
 
 
-class Ospfv3IPv4Data(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    basic: Optional[BasicOspfv3Attributes] = None
-    advanced: Optional[AdvancedOspfv3Attributes] = None
-    redistribute: Optional[RedistributedRoute] = None
+class Ospfv3IPv4Parcel(_ParcelBase):
+    type_: Literal["routing/ospfv3/ipv4"] = Field(default="routing/ospfv3/ipv4", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    basic: Optional[BasicOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "basic"))
+    advanced: Optional[AdvancedOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "advanced"))
+    redistribute: Optional[List[RedistributedRoute]] = Field(
+        default=None, validation_alias=AliasPath("data", "redistribute")
+    )
     max_metric_router_lsa: Optional[MaxMetricRouterLsa] = Field(
-        serialization_alias="maxMetricRouterLsa", validation_alias="maxMetricRouterLsa", default=None
+        validation_alias=AliasPath("data", "maxMetricRouterLsa"), default=None
     )
-    area: List[Ospfv3IPv4Area]
+    area: List[Ospfv3IPv4Area] = Field(validation_alias=AliasPath("data", "area"))
 
 
-class Ospfv3IPv6Data(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class Ospfv3IPv6Parcel(_ParcelBase):
+    type_: Literal["routing/ospfv3/ipv6"] = Field(default="routing/ospfv3/ipv6", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    basic: Optional[BasicOspfv3Attributes] = None
-    advanced: Optional[AdvancedOspfv3Attributes] = None
-    redistribute: Optional[RedistributedRouteIPv6] = None
+    basic: Optional[BasicOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "basic"))
+    advanced: Optional[AdvancedOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "advanced"))
+    redistribute: Optional[List[RedistributedRouteIPv6]] = Field(
+        default=None, validation_alias=AliasPath("data", "redistribute")
+    )
     max_metric_router_lsa: Optional[MaxMetricRouterLsa] = Field(
-        serialization_alias="maxMetricRouterLsa", validation_alias="maxMetricRouterLsa", default=None
+        validation_alias=AliasPath("data", "maxMetricRouterLsa"), default=None
     )
-    area: List[Ospfv3IPv6Area]
-
-
-class Ospfv3IPv4CreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: Ospfv3IPv4Data
-
-
-class Ospfv3IPv6CreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: Ospfv3IPv6Data
-    metadata: Optional[dict] = None
+    area: List[Ospfv3IPv6Area] = Field(validation_alias=AliasPath("data", "area"))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,171 +1,184 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
 
-Action = Literal[
-    "reject",
-    "accept",
+AttachmentType = Literal[
+    "custom",
+    "auto",
 ]
 
-Protocol = Literal[
-    "IPV4",
-    "IPV6",
-    "BOTH",
+TrafficDirection = Literal[
+    "UNIDIR",
+    "BIDIR",
 ]
 
-Criteria = Literal[
-    "or",
-    "and",
-    "exact",
+ReachableInterfaceType = Literal[
+    "ipv4",
+    "ipv6",
+    "tunnel",
 ]
 
-MetricType = Literal[
-    "type1",
-    "type2",
+TrackType = Literal[
+    "service-icmp",
+    "ipv6-service-icmp",
 ]
 
-Origin = Literal[
-    "egp",
-    "igp",
-    "incomplete",
+InterfaceType = Literal[
+    "fromservice",
+    "toservice",
 ]
 
+RedundancyType = Literal[
+    "active",
+    "backup",
+]
 
-class StandardCommunityList(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    criteria: Union[Global[Criteria], Default[Criteria]] = Default[Criteria](value="or")
-    standard_community_list: List[Global[UUID]] = Field(
-        serialization_alias="standardCommunityList", validation_alias="standardCommunityList"
-    )
+ServiceType = Literal[
+    "Firewall",
+    "Intrusion-detection",
+    "Intrusion-detection-prevention",
+    "NETSVC1",
+    "NETSVC2",
+    "NETSVC3",
+    "NETSVC4",
+    "NETSVC5",
+    "NETSVC6",
+    "NETSVC7",
+]
 
 
-class ExpandedCommunityList(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class GatewayInterface(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    expanded_community_list: Global[UUID] = Field(
-        serialization_alias="expandedCommunityList", validation_alias="expandedCommunityList"
+    interface_name: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="gatewayInterfaceName", validation_alias="gatewayInterfaceName", default=None
+    )
+    ip_address: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="gatewayIpAddress", validation_alias="gatewayIpAddress", default=None
+    )
+    ipv6_address: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="gatewayIpv6Address", validation_alias="gatewayIpv6Address", default=None
     )
 
 
-class RoutePolicyMatch(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ServiceInterface(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    as_path_list: Optional[Global[UUID]] = Field(
-        serialization_alias="asPathList", validation_alias="asPathList", default=None
-    )
-    community_list: Optional[Union[StandardCommunityList, ExpandedCommunityList]] = Field(
-        serialization_alias="communityList", validation_alias="communityList", default=None
+    interface_name: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="serviceInterfaceName", validation_alias="serviceInterfaceName", default=None
     )
-    ext_community_list: Optional[Global[UUID]] = Field(
-        serialization_alias="extCommunityList", validation_alias="extCommunityList", default=None
+    ip_address: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="serviceIpAddress", validation_alias="serviceIpAddress", default=None
     )
-    bgp_local_preference: Optional[Global[int]] = Field(
-        serialization_alias="bgpLocalPreference", validation_alias="bgpLocalPreference", default=None
-    )
-    metric: Optional[Global[int]] = None
-    omp_tag: Optional[Global[int]] = Field(serialization_alias="ompTag", validation_alias="ompTag", default=None)
-    ospf_tag: Optional[Global[int]] = Field(serialization_alias="ospfTag", validation_alias="ospfTag", default=None)
-    ipv4_address: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv4Address", validation_alias="ipv4Address", default=None
-    )
-    ipv4_nexthop: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv4NextHop", validation_alias="ipv4NextHop", default=None
-    )
-    ipv6_address: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv6Address", validation_alias="ipv6Address", default=None
-    )
-    ipv6_nexthop: Optional[Global[UUID]] = Field(
-        serialization_alias="ipv6NextHop", validation_alias="ipv6NextHop", default=None
+    ipv6_address: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="serviceIpv6Address", validation_alias="serviceIpv6Address", default=None
     )
 
 
-class AcceptAction(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class TrackingIP(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    ipv4: Optional[Union[Global[str], Variable]] = None
+    ipv6: Optional[Union[Global[str], Variable]] = None
+
 
-    enable_accept_action: Default[bool] = Default[bool](value=True)
-    set_as_path: Optional[Global[int]] = Field(
-        serialization_alias="setAsPath", validation_alias="setAsPath", default=None
+class ReachableInterface(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    type: Global[ReachableInterfaceType] = Field(
+        serialization_alias="reachableInterfaceType", validation_alias="reachableInterfaceType"
     )
-    set_community: Optional[Union[Global[bool], Default[bool]]] = Field(
-        serialization_alias="setCommunity", validation_alias="setCommunity", default=None
+    name: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="reachableInterfaceName", validation_alias="reachableInterfaceName"
     )
-    set_local_preference: Optional[Global[int]] = Field(
-        serialization_alias="setLocalPreference", validation_alias="setLocalPreference", default=None
+    ip_address: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="reachableIpAddress", validation_alias="reachableIpAddress", default=None
     )
-    set_metric: Optional[Global[int]] = Field(
-        serialization_alias="setMetric", validation_alias="setMetric", default=None
+    ipv6_address: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="reachableIpv6Address", validation_alias="reachableIpv6Address", default=None
     )
-    set_metric_type: Optional[Global[MetricType]] = Field(
-        serialization_alias="setMetricType", validation_alias="setMetricType", default=None
+    tracking_ip: Optional[TrackingIP] = Field(
+        serialization_alias="trackingIp", validation_alias="trackingIp", default=None
     )
-    set_omp_tag: Optional[Global[int]] = Field(
-        serialization_alias="setOmpTag", validation_alias="setOmpTag", default=None
+    track_name: Optional[Union[Global[str], Variable]] = Field(
+        serialization_alias="trackName", validation_alias="trackName", default=None
     )
-    set_origin: Optional[Global[Origin]] = Field(
-        serialization_alias="setOrigin", validation_alias="setOrigin", default=None
+    track_type: Optional[Union[Global[TrackType], Variable]] = Field(
+        serialization_alias="trackType", validation_alias="trackType", default=None
     )
-    set_ospf_tag: Optional[Global[int]] = Field(
-        serialization_alias="setOspfTag", validation_alias="setOspfTag", default=None
+
+
+class InterfaceProperties(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    gateway_interface: Optional[GatewayInterface] = Field(
+        serialization_alias="gatewayInterface", validation_alias="gatewayInterface", default=None
     )
-    set_weight: Optional[Global[int]] = Field(
-        serialization_alias="setWeight", validation_alias="setWeight", default=None
+    service_interface: Optional[ServiceInterface] = Field(
+        serialization_alias="serviceInterface", validation_alias="serviceInterface", default=None
     )
-    set_ipv4_nexthop: Optional[Global[str]] = Field(
-        serialization_alias="setIpv4NextHop", validation_alias="setIpv4NextHop", default=None
+    reachable_interface: Optional[ReachableInterface] = Field(
+        serialization_alias="reachableInterface", validation_alias="reachableInterface", default=None
     )
-    set_ipv6_nexthop: Optional[Global[str]] = Field(
-        serialization_alias="setIpv6NextHop", validation_alias="setIpv6NextHop", default=None
+    interface_type: Optional[Union[Global[InterfaceType], Variable]] = Field(
+        serialization_alias="interfaceType", validation_alias="interfaceType", default=None
+    )
+    redundancy_type: Optional[Union[Global[RedundancyType], Variable]] = Field(
+        serialization_alias="redundancyType", validation_alias="redundancyType", default=None
     )
 
 
-class AcceptActions(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class Attachment(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    accept: AcceptAction
+    interface_properties: List[InterfaceProperties] = Field(
+        serialization_alias="interfaceProperties", validation_alias="interfaceProperties"
+    )
+    traffic_direction: Optional[Union[Global[TrafficDirection], Variable]] = Field(
+        serialization_alias="trafficDirection", validation_alias="trafficDirection", default=None
+    )
 
 
-class RejectActions(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class TrackConfig(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    reject: Default[bool] = Default[bool](value=True)
+    interval: Optional[Union[Global[int], Variable]] = None
+    threshold: Optional[Union[Global[int], Variable]] = None
+    multiplier: Optional[Union[Global[int], Variable]] = None
 
 
-class RoutePolicySequence(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class Service(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    sequence_id: Global[int] = Field(serialization_alias="sequenceId", validation_alias="sequenceId")
-    sequence_name: Global[str] = Field(serialization_alias="sequenceName", validation_alias="sequenceName")
-    base_action: Union[Global[Action], Default[Action]] = Field(
-        serialization_alias="baseAction", validation_alias="baseAction", default=Default[Action](value="reject")
+    service_type: Union[Global[ServiceType], Variable] = Field(
+        serialization_alias="serviceType", validation_alias="serviceType"
     )
-    protocol: Union[Global[Protocol], Default[Protocol]] = Default[Protocol](value="IPV4")
-    match_entries: Optional[List[RoutePolicyMatch]] = Field(
-        serialization_alias="matchEntries", validation_alias="matchEntries", default=None
+    default_track: Optional[Union[Global[bool], Default[bool]]] = Field(
+        serialization_alias="defaultTrack", validation_alias="defaultTrack", default=None
     )
-    actions: Optional[List[Union[AcceptActions, RejectActions]]] = None
-
-
-class RoutePolicyData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    defautl_action: Union[Global[Action], Default[Action]] = Field(
-        serialization_alias="defaultAction",
-        validation_alias="defaultAction",
-        default=Default[Action](value="reject"),
+    track: Optional[Global[bool]] = None
+    track_config: Optional[TrackConfig] = Field(
+        serialization_alias="trackConfig", validation_alias="trackConfig", default=None
     )
-    sequences: List[RoutePolicySequence] = []
+    attachments: Optional[List[Attachment]] = None
 
 
-class RoutePolicyCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class ServiceInsertionAttachmentParcel(_ParcelBase):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    name: str
-    description: Optional[str] = None
-    data: RoutePolicyData
-    metadata: Optional[dict] = None
+    attachment_type: Optional[Union[Global[AttachmentType], Variable]] = Field(
+        validation_alias=AliasPath("data", "attachmentType"), default=None
+    )
+    service_chain_instance_id: Optional[Union[Global[str], Variable]] = Field(
+        validation_alias=AliasPath("data", "serviceChainInstanceID"), default=None
+    )
+    service_chain_definition_id: Global[UUID] = Field(
+        validation_alias=AliasPath("data", "serviceChainDefinitionID"),
+    )
+    vpn: Union[Global[int], Variable] = Field(validation_alias=AliasPath("data", "vpn"))
+    services: Optional[List[Service]] = Field(default=None, validation_alias=AliasPath("data", "services"))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/policy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,86 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
-
-from typing import List, Literal, Optional, Union
+from typing import List, Literal, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Global, Variable, _ParcelBase
+from catalystwan.models.configuration.feature_profile.sdwan.transport.bgp import RefIdItem
 
-EndpointProtocol = Literal[
-    "tcp",
-    "udp",
-]
+PredefinedZone = Literal["self", "default", "untrusted"]
+SettingOn = Literal["on"]
+FailureMode = Literal["close", "open"]
 
-TrackerType = Literal["endpoint"]
 
-EndpointTrackerType = Literal["static-route"]
+class AppHosting(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    nat: Union[Global[bool], Variable]
+    database_url: Union[Global[bool], Variable] = Field(validation_alias="databaseUrl")
+    resource_profile: Union[Global[bool], Variable] = Field(validation_alias="resourceProfile")
 
-CombineBoolean = Literal[
-    "and",
-    "or",
-]
 
+class NetworkSettings(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    option_type: str = Field(default="network-settings", validation_alias="optionType")
+    value: bool
 
-class EndpointTcpUdp(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    protocol: Optional[Union[Variable, Global[EndpointProtocol]]] = None
-    port: Optional[Union[Variable, Global[int]]] = None
+class PolicySettings(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    tcp_syn_flood_limit: Global[str] = Field(default=None, validation_alias="tcpSynFloodLimit")
+    max_incomplete_tcp_limit: Global[str] = Field(default=None, validation_alias="maxIncompleteTcpLimit")
+    max_incomplete_udp_limit: Global[str] = Field(default=None, validation_alias="maxIncompleteUdpLimit")
 
+    max_incomplete_icmp_limit: Global[str] = Field(default=None, validation_alias="maxIncompleteIcmpLimit")
+    audit_trail: Global[SettingOn] = Field(default=None, validation_alias="auditTrail")
+    unified_logging: Global[SettingOn] = Field(default=None, validation_alias="unifiedLogging")
+    session_reclassify_allow: Global[SettingOn] = Field(default=None, validation_alias="sessionReclassifyAllow")
+    icmp_unreachable_allow: Global[SettingOn] = Field(default=None, validation_alias="icmpUnreachableAllow")
+    failure_mode: Global[FailureMode] = Field(default=None, validation_alias="failureMode")
+    security_logging: NetworkSettings = Field(default=None, validation_alias="securityLogging")
 
-class TrackerData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    name: Union[Variable, Global[str]] = Field(serialization_alias="trackerName", validation_alias="trackerName")
-    endpoint_api_url: Optional[Union[Variable, Global[str]]] = Field(
-        serialization_alias="endpointApiUrl", validation_alias="endpointApiUrl", default=None
-    )
-    endpoint_dns_name: Optional[Union[Variable, Global[str]]] = Field(
-        serialization_alias="endpointDnsName", validation_alias="endpointDnsName", default=None
-    )
-    endpoint_ip: Optional[Union[Variable, Global[str]]] = Field(
-        serialization_alias="endpointIp", validation_alias="endpointIp", default=None
-    )
-    endpoint_tcp_udp: Optional[EndpointTcpUdp] = Field(
-        serialization_alias="endpointTcpUdp", validation_alias="endpointTcpUdp", default=None
+class NgFirewallEntry(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    src_zone: Union[RefIdItem, Global[PredefinedZone]] = Field(
+        validation_alias="srcZone", serialization_alias="srcZone"
     )
-    interval: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=60)
-    multiplier: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=3)
-    threshold: Optional[Union[Global[int], Variable, Default[int]]] = Default[int](value=300)
-    endpoint_tracker_type: Optional[Union[Global[EndpointTrackerType], Variable, Default[EndpointTrackerType]]] = Field(
-        serialization_alias="endpointTrackerType",
-        validation_alias="endpointTrackerType",
-        default=Default[EndpointTrackerType](value="static-route"),
+    dst_zone: Union[RefIdItem, Global[PredefinedZone]] = Field(
+        validation_alias="dstZone", serialization_alias="dstZone"
     )
-    tracker_type: Optional[Union[Global[TrackerType], Variable, Default[TrackerType]]] = Field(
-        serialization_alias="trackerType",
-        validation_alias="trackerType",
-        default=Default[TrackerType](value="endpoint"),
-    )
-
 
-class TrackerCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    name: str
-    description: Optional[str] = None
-    data: TrackerData
-    metadata: Optional[dict] = None
+class NgFirewall(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    ref_id: Union[Global[UUID], Global[str]] = Field(validation_alias="refId", serialization_alias="refId")
+    entries: List[NgFirewallEntry] = Field(validation_alias="entries", min_length=1)
 
 
-class TrackerRef(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class NgFirewallContainer(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    ngfirewall: NgFirewall = Field(validation_alias="ngfirewall", serialization_alias="ngfirewall")
 
-    tracker_ref: Global[UUID] = Field(serialization_alias="trackerRef", validation_alias="trackerRef")
 
+class SslDecryption(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    ssl_decryption: RefIdItem = Field(validation_alias="sslDecryption", serialization_alias="sslDecryption")
 
-class TrackerGroupData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
-    tracker_refs: List[TrackerRef] = Field(serialization_alias="trackerRefs", validation_alias="trackerRefs")
-    combine_boolean: Union[Global[CombineBoolean], Variable, Default[CombineBoolean]] = Field(
-        serialization_alias="combineBoolean",
-        validation_alias="combineBoolean",
-        default=Default[CombineBoolean](value="or"),
-    )
+class AdvancedInspectionProfile(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, extra="forbid")
+    advanced_inspection_profile: RefIdItem = Field(validation_alias="advancedInspectionProfile")
 
 
-class TrackerGroupCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: TrackerGroupData
-    metadata: Optional[dict] = None
-
-
-class TrackerAssociationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    parcel_id: str = Field(serialization_alias="parcelId", validation_alias="parcelId")
+class PolicyParcel(_ParcelBase):
+    type_: Literal["policy"] = Field(default="policy", exclude=True)
+    parcel_description: str = Field(
+        default="",
+        serialization_alias="description",
+        validation_alias="description",
+        description="Set the parcel description",
+    )
+    assembly: List[Union[NgFirewallContainer, SslDecryption, AdvancedInspectionProfile]] = Field(
+        validation_alias=AliasPath("data", "assembly"), min_length=1
+    )
+    settings: PolicySettings = Field(default=None, validation_alias=AliasPath("data", "settings"))
+    app_hosting: AppHosting = Field(default=None, validation_alias=AliasPath("data", "appHosting"))
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
+from ipaddress import IPv4Address
 from typing import List, Literal, Optional, Union
 
-from pydantic import BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.common import SubnetMask
 
 CountryCode = Literal[
     "AE",
     "AR",
     "AT",
     "AU",
     "BA",
@@ -131,52 +133,56 @@
     "open",
     "personal",
     "enterprise",
 ]
 
 
 class MeStaticIpConfig(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    me_ipv4_address: Union[Global[str], Variable]
-    netmask: Union[Global[str], Variable]
-    default_gateway: Union[Global[str], Variable] = Field(
+    me_ipv4_address: Union[Global[IPv4Address], Variable] = Field(
+        serialization_alias="meIpv4Address", validation_alias="meIpv4Address"
+    )
+    netmask: Union[Global[SubnetMask], Variable]
+    default_gateway: Union[Global[IPv4Address], Variable] = Field(
         serialization_alias="defaultGateway", validation_alias="defaultGateway"
     )
 
 
 class MeIpConfig(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     me_dynamic_ip_enabled: Union[Global[bool], Default[bool]] = Field(
         serialization_alias="meDynamicIpEnabled",
         validation_alias="meDynamicIpEnabled",
         default=Default[bool](value=True),
     )
-    me_static_ip_config: Optional[MeStaticIpConfig] = None
+    me_static_ip_config: Optional[MeStaticIpConfig] = Field(
+        default=None, serialization_alias="meStaticIpCfg", validation_alias="meStaticIpCfg"
+    )
 
 
 class SecurityConfig(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     security_type: Global[SecurityType] = Field(serialization_alias="securityType", validation_alias="securityType")
-    radius_server_ip: Optional[Union[Global[str], Variable]] = Field(
+    radius_server_ip: Optional[Union[Global[IPv4Address], Variable]] = Field(
         serialization_alias="radiusServerIp", validation_alias="radiusServerIp", default=None
     )
     radius_server_port: Optional[Union[Global[int], Variable, Default[int]]] = Field(
         serialization_alias="radiusServerPort", validation_alias="radiusServerPort", default=None
     )
     radius_server_secret: Optional[Union[Global[str], Variable]] = Field(
         serialization_alias="radiusServerSecret", validation_alias="radiusServerSecret", default=None
     )
     passphrase: Optional[Union[Global[str], Variable]] = None
 
 
 class SSID(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     name: Global[str]
     admin_state: Union[Global[bool], Variable, Default[bool]] = Field(
         serialization_alias="adminState", validation_alias="adminState", default=Default[bool](value=True)
     )
     broadcast_ssid: Union[Global[bool], Variable, Default[bool]] = Field(
         serialization_alias="broadcastSsid", validation_alias="broadcastSsid", default=Default[bool](value=True)
@@ -189,32 +195,22 @@
     qos_profile: Union[Global[QosProfile], Variable, Default[QosProfile]] = Field(
         serialization_alias="qosProfile",
         validation_alias="qosProfile",
         default=Default[QosProfile](value="silver"),
     )
 
 
-class WirelessLanData(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+class WirelessLanParcel(_ParcelBase):
+    type_: Literal["wirelesslan"] = Field(default="wirelesslan", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     enable_2_4G: Union[Global[bool], Variable, Default[bool]] = Field(
-        serialization_alias="enable24G", validation_alias="enable24G", default=Default[bool](value=True)
+        validation_alias=AliasPath("data", "enable24G"), default=Default[bool](value=True)
     )
     enable_5G: Union[Global[bool], Variable, Default[bool]] = Field(
-        serialization_alias="enable5G", validation_alias="enable5G", default=Default[bool](value=True)
-    )
-    ssid: List[SSID]
-    country: Union[Global[CountryCode], Variable]
-    username: Union[Global[str], Variable]
-    password: Union[Global[str], Variable]
-    me_ip_config: MeIpConfig = Field(
-        serialization_alias="meIpConfig", validation_alias="meIpConfig", default=MeIpConfig()
+        validation_alias=AliasPath("data", "enable5G"), default=Default[bool](value=True)
     )
-
-
-class WirelessLanCreationPayload(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    name: str
-    description: Optional[str] = None
-    data: WirelessLanData
-    metadata: Optional[dict] = None
+    ssid: List[SSID] = Field(validation_alias=AliasPath("data", "ssid"))
+    country: Union[Global[CountryCode], Variable] = Field(validation_alias=AliasPath("data", "country"))
+    username: Union[Global[str], Variable] = Field(validation_alias=AliasPath("data", "username"))
+    password: Union[Global[str], Variable] = Field(validation_alias=AliasPath("data", "password"))
+    me_ip_config: MeIpConfig = Field(validation_alias=AliasPath("data", "meIpConfig"), default=MeIpConfig())
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from ipaddress import IPv4Address, IPv6Address
-from typing import List, Optional, Union
+from typing import List, Literal, Optional, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default, as_global
 
+DEFAULT_USER_PRIVILEGE = "15"
+
 
 class PubkeyChainItem(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-    )
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
     key_string: Global[str] = Field(
         validation_alias="keyString",
         serialization_alias="keyString",
         pattern="^AAAA[0-9A-Za-z+/]+[=]{0,3}$",
         description="Set the RSA key string",
     )
 
@@ -25,25 +25,25 @@
         serialization_alias="keyType",
         validation_alias="keyType",
         description="Only RSA is supported",
     )
 
 
 class UserItem(BaseModel):
-    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    model_config = ConfigDict(extra="ignore", populate_by_name=True)
 
     name: Union[Global[str], Variable] = Field(description="Set the username")
     password: Union[Global[str], Variable] = Field(
         description=(
             "Set the user password [Note: Catalyst SD-WAN Manager will encrypt this field before saving."
             "Cleartext strings will not be returned back to the user in GET responses for sensitive fields.]"
         )
     )
     privilege: Union[Global[str], Variable, Default[str], None] = Field(
-        None, description="Set Privilege Level for this user"
+        default=as_default(DEFAULT_USER_PRIVILEGE), description="Set Privilege Level for this user"
     )
     pubkey_chain: Optional[List[PubkeyChainItem]] = Field(
         default=None,
         validation_alias="pubkeyChain",
         serialization_alias="pubkeyChain",
         description="List of RSA public-keys per user",
         max_length=2,
@@ -256,33 +256,38 @@
         default=None,
         validation_alias="ifAuthenticated",
         serialization_alias="ifAuthenticated",
         description="Succeed if user has authenticated",
     )
 
 
-class AAA(_ParcelBase):
+class AAAParcel(_ParcelBase):
+    type_: Literal["aaa"] = Field(default="aaa", exclude=True)
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+
     authentication_group: Union[Variable, Global[bool], Default[bool]] = Field(
         default=as_default(False),
         validation_alias=AliasPath("data", "authenticationGroup"),
         description="Authentication configurations parameters",
     )
     accounting_group: Union[Variable, Global[bool], Default[bool]] = Field(
         default=as_default(False),
         validation_alias=AliasPath("data", "accountingGroup"),
         description="Accounting configurations parameters",
     )
-    # local, radius, tacacs
     server_auth_order: Global[List[str]] = Field(
+        # local, radius, tacacs
         validation_alias=AliasPath("data", "serverAuthOrder"),
         min_length=1,
         max_length=4,
         description="ServerGroups priority order",
     )
-    user: Optional[List[UserItem]] = Field(default=None, description="Create local login account", min_length=1)
+    user: Optional[List[UserItem]] = Field(
+        default=None, validation_alias=AliasPath("data", "user"), description="Create local login account", min_length=1
+    )
     radius: Optional[List[Radius]] = Field(
         default=None, validation_alias=AliasPath("data", "radius"), description="Configure the Radius serverGroup"
     )
     tacacs: Optional[List[Tacacs]] = Field(
         default=None, validation_alias=AliasPath("data", "tacacs"), description="Configure the TACACS serverGroup"
     )
     accounting_rule: Optional[List[AccountingRuleItem]] = Field(
@@ -300,14 +305,56 @@
     )
     authorization_rule: Optional[List[AuthorizationRuleItem]] = Field(
         default=None,
         validation_alias=AliasPath("data", "authorizationRule"),
         description="Configure the Authorization Rules",
     )
 
+    @classmethod
+    def new(
+        cls,
+        parcel_name: str,
+        server_auth_order: List[str],
+        *,
+        parcel_description: Optional[str] = None,
+        accounting_group: bool = False,
+        authorization_console: bool = False,
+        authorization_config_commands: bool = False
+    ) -> "AAAParcel":
+        return cls(
+            parcel_name=parcel_name,
+            parcel_description=parcel_description,
+            server_auth_order=as_global(server_auth_order),
+            accounting_group=as_global(accounting_group),
+            authorization_console=as_global(authorization_console),
+            authorization_config_commands=as_global(authorization_config_commands),
+        )
+
+    def add_user(
+        self,
+        name: str,
+        password: str,
+        *,
+        privilege: str = DEFAULT_USER_PRIVILEGE,
+        pubkey_chain: Optional[List[PubkeyChainItem]] = None
+    ) -> UserItem:
+        user = UserItem(
+            name=as_global(name),
+            password=as_global(password),
+            privilege=as_global(privilege),
+            pubkey_chain=pubkey_chain,
+        )
+        if self.user is None:
+            self.user = []
+        self.user.append(user)
+        return user
+
+    def set_server_auth_order(self, server_auth_order: List[str]) -> None:
+        self.server_auth_order = as_global(server_auth_order)
+
     def add_authorization_rule(
         self, rule_id: str, method: str, level: str, group: List[str], if_authenticated: bool
     ) -> AuthorizationRuleItem:
         item = AuthorizationRuleItem(
             rule_id=as_global(rule_id),
             method=as_global(method),
             level=as_global(level),
```

### Comparing `catalystwan-0.33.6/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py` & `catalystwan-0.33.6.dev0/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_profile.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,70 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from typing import Literal, Union
+from typing import Literal, Optional, Union
 
-from pydantic import AliasPath, BaseModel, ConfigDict, Field
+from pydantic import AliasPath, BaseModel, ConfigDict, Field, model_validator
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
 
-ConfigTypeValue = Literal["non-eSim"]
-
-
-class ControllerConfig(BaseModel):
-    model_config = ConfigDict(extra="forbid", arbitrary_types_allowed=True, populate_by_name=True)
-    id: Union[Variable, Global[str]] = Field(min_length=1, max_length=5, description="Cellular ID")
-    slot: Union[Variable, Global[int], Default[int], None] = Field(
-        default=None, description="Set primary SIM slot", ge=0, le=1
+AuthenticationType = Literal[
+    "chap",
+    "pap",
+    "pap_chap",
+]
+
+
+class NeedAuthentication(BaseModel):
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    password: Union[Variable, Global[str]] = Field()
+    type: Union[Variable, Global[AuthenticationType]] = Field()
+    username: Union[Variable, Global[str]] = Field()
+
+
+class Authentication(BaseModel):
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    need_authentication: Optional[NeedAuthentication] = Field(
+        default=None, validation_alias="needAuthentication", serialization_alias="needAuthentication"
     )
-    max_retry: Union[Variable, Global[int], Default[None], None] = Field(
-        default=None,
-        description="Set SIM failover retries",
-        ge=0,
-        le=65535,
-        serialization_alias="maxRetry",
-        validation_alias="maxRetry",
+    no_authentication: Optional[Default[Literal["none"]]] = Field(
+        default=None, validation_alias="noAuthentication", serialization_alias="noAuthentication"
     )
-    failover_timer: Union[Variable, Global[int], Default[None], None] = Field(
-        default=None,
-        description="Set SIM failover timeout in minutes",
-        ge=3,
-        le=7,
-        serialization_alias="failovertimer",
-        validation_alias="failovertimer",
+
+    @model_validator(mode="after")
+    def validate_authentication_exclusive(self):
+        if self.need_authentication and self.no_authentication:
+            raise ValueError("Only one of need_authentication and no_authentication can be set")
+        return self
+
+
+PdnType = Literal[
+    "ipv4",
+    "ipv4v6",
+    "ipv6",
+]
+
+
+class ProfileInfo(BaseModel):
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    apn: Union[Variable, Global[str]] = Field()
+    authentication: Optional[Authentication] = Field(default=None)
+    no_overwrite: Optional[Union[Variable, Global[bool], Default[None]]] = Field(
+        default=None, validation_alias="noOverwrite", serialization_alias="noOverwrite"
     )
-    auto_sim: Union[Variable, Global[bool], Default[None], None] = Field(
-        default=None,
-        description="Enable/Disable Firmware Auto Sim",
-        serialization_alias="autoSim",
-        validation_alias="autoSim",
+    pdn_type: Optional[Union[Variable, Default[PdnType], Global[PdnType]]] = Field(
+        default=None, validation_alias="pdnType", serialization_alias="pdnType"
     )
 
 
-class CellularController(_ParcelBase):
-    config_type: Default[ConfigTypeValue] = Field(
-        default=Default(value="non-eSim"), validation_alias=AliasPath("data", "configType")
-    )
-    controller_config: ControllerConfig = Field(validation_alias=AliasPath("data", "controllerConfig"))
+class ProfileConfig(BaseModel):
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    id: Union[Variable, Global[int]] = Field()
+    profile_info: ProfileInfo = Field(validation_alias="profileInfo", serialization_alias="profileInfo")
+
 
-    @staticmethod
-    def add_controller_config(
-        id: Union[Variable, Global[str]],
-        max_retry: Union[Variable, Global[int], Default[None], None] = None,
-        failover_timer: Union[Variable, Global[int], Default[None], None] = None,
-        auto_sim: Union[Variable, Global[bool], Default[None], None] = None,
-    ):
-        return ControllerConfig(id=id, max_retry=max_retry, failover_timer=failover_timer, auto_sim=auto_sim)
+class CellularProfileParcel(_ParcelBase):
+    model_config = ConfigDict(extra="forbid", populate_by_name=True)
+    type_: Literal["cellular-profile"] = Field(default="cellular-profile", exclude=True, frozen=True)
+    profile_config: ProfileConfig = Field(validation_alias=AliasPath("data", "profileConfig"))
+    config_type: Optional[Default[Literal["non-eSim"]]] = Field(
+        default=None, validation_alias=AliasPath("data", "configType")
+    )
```

### Comparing `catalystwan-0.33.6/catalystwan/models/device_inventory.py` & `catalystwan-0.33.6.dev0/catalystwan/models/device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/models/misc/application_protocols.py` & `catalystwan-0.33.6.dev0/catalystwan/models/misc/application_protocols.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/centralized.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/centralized.py`

 * *Files 10% similar despite different names*

```diff
@@ -229,40 +229,26 @@
     def add_hub_and_spoke_policy(self, hub_and_spoke_policy_id: UUID) -> None:
         policy_definition = assert_feature_defintion(self.policy_definition)
         policy_definition.assembly.append(HubAndSpokePolicyItem(definition_id=hub_and_spoke_policy_id))
 
     @model_validator(mode="before")
     @classmethod
     def try_parse_policy_definition_string(cls, values):
-        # GET /template/policy/vsmart contains string in policyDefinition field
+        # this is needed because GET /template/policy/vsmart contains string in policyDefinition field
         # while POST /template/policy/vsmart requires a regular object
         # it makes sense to reuse that model for both requests and present parsed data to the user
-        # This is only applicable for "feature" policy type
-        # when we are trying to deserialize "policyDefinition" field obtained from remote as string
-        json_policy_type = values.get("policyType")
-        json_policy_definition = values.get("policyDefinition")
-        if json_policy_type == "feature":
-            if isinstance(json_policy_definition, str):
-                values["policyDefinition"] = CentralizedPolicyDefinition.model_validate_json(json_policy_definition)
-            else:
-                values["policyDefinition"] = CentralizedPolicyDefinition()
+        if not isinstance(values, dict):
+            return values
+        if (policy_definition := values.get("policyDefinition")) and values.get("policyType") != "cli":
+            if isinstance(policy_definition, str):
+                values["policyDefinition"] = CentralizedPolicyDefinition.model_validate_json(policy_definition)
+        else:
+            values["policyDefinition"] = CentralizedPolicyDefinition()
         return values
 
-    @model_validator(mode="after")
-    def check_definition_content_by_type(self):
-        if self.policy_type == "cli":
-            assert isinstance(
-                self.policy_definition, str
-            ), "policy definition must be provided as string for cli policy"
-        elif self.policy_type == "feature":
-            assert isinstance(
-                self.policy_definition, CentralizedPolicyDefinition
-            ), "policy definition must be provided as CentralizedPolicyDefinition object for feature policy"
-        return self
-
 
 class CentralizedPolicyEditPayload(PolicyEditPayload, CentralizedPolicy):
     rid: Optional[int] = Field(default=None, serialization_alias="@rid", validation_alias="@rid")
 
 
 class CentralizedPolicyInfo(PolicyInfo, CentralizedPolicyEditPayload):
     pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/access_control_list.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/access_control_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 from typing import Any, List, Literal, Set, Tuple, Union
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
 from catalystwan.models.policy.policy_definition import (
+    BasicPolicyAction,
+    BasicPolicyActionType,
     ClassMapAction,
     ClassMapListEntry,
     CountAction,
-    DefaultAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataPrefixListEntry,
     DestinationIPEntry,
     DestinationPortEntry,
     DSCPEntry,
     LogAction,
     Match,
     MirrorAction,
     NextHopEntry,
     PacketLengthEntry,
     PLPEntry,
     PolicerAction,
-    PolicyActionType,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     ProtocolEntry,
     Reference,
     SourceDataPrefixListEntry,
     SourceIPEntry,
     SourcePortEntry,
     TCPEntry,
@@ -65,15 +67,15 @@
     entries: List[AclPolicySequenceMatchEntry] = []
 
 
 class AclPolicySequence(PolicyDefinitionSequenceBase):
     sequence_type: Literal["acl"] = Field(
         default="acl", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
-    base_action: PolicyActionType = Field(
+    base_action: BasicPolicyActionType = Field(
         default="accept", serialization_alias="baseAction", validation_alias="baseAction"
     )
     match: AclPolicySequenceMatch = AclPolicySequenceMatch()
     actions: List[AclPolicySequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_dscp(self, dscp: int) -> None:
@@ -87,25 +89,25 @@
 
     def match_high_plp(self) -> None:
         self._insert_match(PLPEntry(value="high"))
 
     def match_protocols(self, protocols: Set[int]) -> None:
         self._insert_match(ProtocolEntry.from_protocol_set(protocols))
 
-    def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_list_id))
+    def match_source_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
+        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_lists))
 
     def match_source_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(SourceIPEntry.from_ipv4_networks(networks))
 
     def match_source_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(SourcePortEntry.from_port_set_and_ranges(ports, port_ranges))
 
     def match_destination_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(DestinationDataPrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(DestinationDataPrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_destination_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(DestinationIPEntry.from_ipv4_networks(networks))
 
     def match_destination_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(DestinationPortEntry.from_port_set_and_ranges(ports, port_ranges))
 
@@ -140,24 +142,32 @@
     @accept_action
     def associate_policer_list_action(self, policer_list_id: UUID) -> None:
         self._insert_action(PolicerAction(parameter=Reference(ref=policer_list_id)))
 
 
 class AclPolicy(AclPolicyHeader, DefinitionWithSequencesCommonBase):
     sequences: List[AclPolicySequence] = []
-    default_action: DefaultAction = Field(
-        default=DefaultAction(type="drop"),
+    default_action: BasicPolicyAction = Field(
+        default=BasicPolicyAction(type="drop"),
         serialization_alias="defaultAction",
         validation_alias="defaultAction",
     )
     model_config = ConfigDict(populate_by_name=True)
 
     def add_acl_sequence(
-        self, name: str = "Access Control List", base_action: PolicyActionType = "accept"
+        self, name: str = "Access Control List", base_action: BasicPolicyActionType = "accept"
     ) -> AclPolicySequence:
         seq = AclPolicySequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         self.add(seq)
         return seq
+
+
+class AclPolicyEditPayload(AclPolicy, PolicyDefinitionId):
+    pass
+
+
+class AclPolicyGetResponse(AclPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/access_control_list_ipv6.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/access_control_list_ipv6.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 from typing import Any, List, Literal, Set, Tuple, Union
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
 from catalystwan.models.policy.policy_definition import (
+    BasicPolicyAction,
+    BasicPolicyActionType,
     ClassMapAction,
     ClassMapListEntry,
     CountAction,
-    DefaultAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataIPv6PrefixListEntry,
     DestinationIPv6Entry,
     DestinationPortEntry,
     LogAction,
     Match,
     MirrorAction,
     NextHeaderEntry,
     NextHopEntry,
     PacketLengthEntry,
     PLPEntry,
     PolicerAction,
-    PolicyActionType,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     Reference,
     SourceDataIPv6PrefixListEntry,
     SourceIPv6Entry,
     SourcePortEntry,
     TCPEntry,
     TrafficClassEntry,
@@ -65,15 +67,15 @@
     entries: List[AclIPv6PolicySequenceMatchEntry] = []
 
 
 class AclIPv6PolicySequence(PolicyDefinitionSequenceBase):
     sequence_type: Literal["aclv6"] = Field(
         default="aclv6", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
-    base_action: PolicyActionType = Field(
+    base_action: BasicPolicyActionType = Field(
         default="accept", serialization_alias="baseAction", validation_alias="baseAction"
     )
     match: AclIPv6PolicySequenceMatch = AclIPv6PolicySequenceMatch()
     actions: List[AclIPv6PolicySequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_next_header(self, next_header: int) -> None:
@@ -85,24 +87,24 @@
     def match_low_plp(self) -> None:
         self._insert_match(PLPEntry(value="low"))
 
     def match_high_plp(self) -> None:
         self._insert_match(PLPEntry(value="high"))
 
     def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(SourceDataIPv6PrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(SourceDataIPv6PrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_source_ip(self, networks: List[IPv6Network]) -> None:
         self._insert_match(SourceIPv6Entry.from_ipv6_networks(networks))
 
     def match_source_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(SourcePortEntry.from_port_set_and_ranges(ports, port_ranges))
 
     def match_destination_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(DestinationDataIPv6PrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(DestinationDataIPv6PrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_destination_ip(self, networks: List[IPv6Network]) -> None:
         self._insert_match(DestinationIPv6Entry.from_ipv6_networks(networks))
 
     def match_destination_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(DestinationPortEntry.from_port_set_and_ranges(ports, port_ranges))
 
@@ -140,24 +142,32 @@
     @accept_action
     def associate_policer_list_action(self, policer_list_id: UUID) -> None:
         self._insert_action(PolicerAction(parameter=Reference(ref=policer_list_id)))
 
 
 class AclIPv6Policy(AclIPv6PolicyHeader, DefinitionWithSequencesCommonBase):
     sequences: List[AclIPv6PolicySequence] = []
-    default_action: DefaultAction = Field(
-        default=DefaultAction(type="drop"),
+    default_action: BasicPolicyAction = Field(
+        default=BasicPolicyAction(type="drop"),
         serialization_alias="defaultAction",
         validation_alias="defaultAction",
     )
     model_config = ConfigDict(populate_by_name=True)
 
     def add_acl_sequence(
-        self, name: str = "Access Control List", base_action: PolicyActionType = "accept"
+        self, name: str = "Access Control List", base_action: BasicPolicyActionType = "accept"
     ) -> AclIPv6PolicySequence:
         seq = AclIPv6PolicySequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv6",
         )
         self.add(seq)
         return seq
+
+
+class AclIPv6PolicyEditPayload(AclIPv6Policy, PolicyDefinitionId):
+    pass
+
+
+class AclIPv6PolicyGetResponse(AclIPv6Policy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/control.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/control.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 from ipaddress import IPv4Address
 from typing import Any, List, Literal, Optional, Union, overload
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
-from catalystwan.models.common import TLOCColor
-from catalystwan.models.policy.lists_entries import EncapType
+from catalystwan.models.common import EncapType, TLOCColor
 from catalystwan.models.policy.policy_definition import (
     AffinityEntry,
-    Carrier,
     CarrierEntry,
+    CarrierType,
     ColorListEntry,
     CommunityAdditiveEntry,
     CommunityEntry,
     CommunityListEntry,
-    DefaultAction,
+    ControlPathType,
     DefinitionWithSequencesCommonBase,
     DomainIDEntry,
     ExpandedCommunityListEntry,
     ExportToAction,
     GroupIDEntry,
     Match,
     MultiRegionRole,
     OMPTagEntry,
     OriginatorEntry,
     OriginEntry,
     OriginProtocol,
-    PathType,
     PathTypeEntry,
-    PolicyActionType,
+    PolicyActionBase,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     PreferenceEntry,
     PrefixListEntry,
     RegionEntry,
     RegionListEntry,
     RoleEntry,
     ServiceEntry,
@@ -97,14 +97,19 @@
         TLOCEntry,
     ],
     Field(discriminator="field"),
 ]
 
 ControlPolicyRouteSequenceActions = Any  # TODO
 ControlPolicyTLOCSequenceActions = Any  # TODO
+ControlPolicyBaseActionType = Literal["accept", "reject"]
+
+
+class ControlPolicyBaseAction(PolicyActionBase):
+    type: ControlPolicyBaseActionType
 
 
 class ControlPolicyHeader(PolicyDefinitionBase):
     type: Literal["control"] = "control"
 
 
 class ControlPolicyRouteSequenceMatch(Match):
@@ -115,15 +120,15 @@
     entries: List[AnyControlPolicyTLOCSequenceMatchEntry] = []
 
 
 class ControlPolicyRouteSequence(PolicyDefinitionSequenceBase):
     sequence_type: Literal["route"] = Field(
         default="route", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
-    base_action: PolicyActionType = Field(
+    base_action: ControlPolicyBaseActionType = Field(
         default="reject", serialization_alias="baseAction", validation_alias="baseAction"
     )
     match: ControlPolicyRouteSequenceMatch = ControlPolicyRouteSequenceMatch()
     actions: List[ControlPolicyRouteSequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_color_list(self, color_list_id: UUID) -> None:
@@ -140,15 +145,15 @@
 
     def match_origin(self, origin: OriginProtocol) -> None:
         self._insert_match(OriginEntry(value=origin))
 
     def match_originator(self, originator: IPv4Address) -> None:
         self._insert_match(OriginatorEntry(value=originator))
 
-    def match_path_type(self, path_type: PathType) -> None:
+    def match_path_type(self, path_type: ControlPathType) -> None:
         self._insert_match(PathTypeEntry(value=path_type))
 
     def match_preference(self, preference: int) -> None:
         self._insert_match(PreferenceEntry(value=str(preference)))
 
     def match_region(self, region_id: int, role: Optional[MultiRegionRole] = None) -> None:
         self._insert_match(RegionEntry(value=str(region_id)))
@@ -234,22 +239,22 @@
         self._insert_action(ExportToAction(parameter=VPNListEntry(ref=vpn_list_id)))
 
 
 class ControlPolicyTLOCSequence(PolicyDefinitionSequenceBase):
     sequence_type: Literal["tloc"] = Field(
         default="tloc", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
-    base_action: PolicyActionType = Field(
+    base_action: ControlPolicyBaseActionType = Field(
         default="reject", serialization_alias="baseAction", validation_alias="baseAction"
     )
     match: ControlPolicyTLOCSequenceMatch = ControlPolicyTLOCSequenceMatch()
     actions: List[ControlPolicyTLOCSequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
-    def match_carrier(self, carrier: Carrier) -> None:
+    def match_carrier(self, carrier: CarrierType) -> None:
         self._insert_match(CarrierEntry(value=carrier))
 
     def match_color_list(self, color_list_id: UUID) -> None:
         self._insert_match(ColorListEntry(ref=color_list_id))
 
     def match_domain_id(self, domain_id: int) -> None:
         self._insert_match(DomainIDEntry(value=str(domain_id)))
@@ -309,35 +314,43 @@
     Union[ControlPolicyRouteSequence, ControlPolicyTLOCSequence],
     Field(discriminator="sequence_type"),
 ]
 
 
 class ControlPolicy(ControlPolicyHeader, DefinitionWithSequencesCommonBase):
     sequences: List[AnyControlPolicySequence] = []
-    default_action: DefaultAction = Field(
-        default=DefaultAction(type="reject"),
+    default_action: ControlPolicyBaseAction = Field(
+        default=ControlPolicyBaseAction(type="reject"),
         serialization_alias="defaultAction",
         validation_alias="defaultAction",
     )
     model_config = ConfigDict(populate_by_name=True)
 
     def add_route_sequence(
-        self, name: str = "Route", base_action: PolicyActionType = "reject"
+        self, name: str = "Route", base_action: ControlPolicyBaseActionType = "reject"
     ) -> ControlPolicyRouteSequence:
         seq = ControlPolicyRouteSequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         self.add(seq)
         return seq
 
     def add_tloc_sequence(
-        self, name: str = "TLOC", base_action: PolicyActionType = "reject"
+        self, name: str = "TLOC", base_action: ControlPolicyBaseActionType = "reject"
     ) -> ControlPolicyTLOCSequence:
         seq = ControlPolicyTLOCSequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         self.add(seq)
         return seq
+
+
+class ControlPolicyEditPayload(ControlPolicy, PolicyDefinitionId):
+    pass
+
+
+class ControlPolicyGetResponse(ControlPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/device_access.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/device_access.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 from typing import Any, List, Literal, Optional, Set, Tuple, Union
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
 from catalystwan.models.policy.policy_definition import (
+    BasicPolicyAction,
+    BasicPolicyActionType,
     CountAction,
-    DefaultAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataPrefixListEntry,
     DestinationIPEntry,
     DestinationPortEntry,
     DeviceAccessProtocol,
     Match,
-    PolicyActionType,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     SourceDataPrefixListEntry,
     SourceIPEntry,
     SourcePortEntry,
 )
 
 DeviceAccessPolicySequenceMatchEntry = Annotated[
@@ -47,60 +49,68 @@
     entries: List[DeviceAccessPolicySequenceMatchEntry] = []
 
 
 class DeviceAccessPolicySequence(PolicyDefinitionSequenceBase):
     sequence_type: Literal["deviceaccesspolicy"] = Field(
         default="deviceaccesspolicy", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
-    base_action: PolicyActionType = Field(
+    base_action: BasicPolicyActionType = Field(
         default="accept", serialization_alias="baseAction", validation_alias="baseAction"
     )
     match: DeviceAccessPolicySequenceMatch = DeviceAccessPolicySequenceMatch()
     actions: List[DeviceAccessPolicySequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_device_access_protocol(self, port: DeviceAccessProtocol) -> None:
         self._insert_match(DestinationPortEntry.from_port_set_and_ranges(ports={port}))
 
-    def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_list_id))
+    def match_source_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
+        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_lists))
 
     def match_source_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(SourceIPEntry.from_ipv4_networks(networks))
 
     def match_source_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(SourcePortEntry.from_port_set_and_ranges(ports, port_ranges))
 
     def match_destination_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(DestinationDataPrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(DestinationDataPrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_destination_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(DestinationIPEntry.from_ipv4_networks(networks))
 
     def associate_count_action(self, counter_name: str) -> None:
         self._insert_action(CountAction(parameter=counter_name))
 
 
 class DeviceAccessPolicy(DeviceAccessPolicyHeader, DefinitionWithSequencesCommonBase):
     sequences: List[DeviceAccessPolicySequence] = []
-    default_action: DefaultAction = Field(
-        default=DefaultAction(type="drop"),
+    default_action: BasicPolicyAction = Field(
+        default=BasicPolicyAction(type="drop"),
         serialization_alias="defaultAction",
         validation_alias="defaultAction",
     )
     model_config = ConfigDict(populate_by_name=True)
 
     def add_acl_sequence(
         self,
         name: str = "Device Access Control List",
-        base_action: PolicyActionType = "accept",
+        base_action: BasicPolicyActionType = "accept",
         device_access_protocol: Optional[DeviceAccessProtocol] = None,
     ) -> DeviceAccessPolicySequence:
         seq = DeviceAccessPolicySequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         if device_access_protocol is not None:
             seq.match_device_access_protocol(port=device_access_protocol)
         self.add(seq)
         return seq
+
+
+class DeviceAccessPolicyEditPayload(DeviceAccessPolicy, PolicyDefinitionId):
+    pass
+
+
+class DeviceAccessPolicyGetResponse(DeviceAccessPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/device_access_ipv6.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/device_access_ipv6.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 from typing import Any, List, Literal, Optional, Set, Tuple, Union
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
 from catalystwan.models.policy.policy_definition import (
+    BasicPolicyAction,
+    BasicPolicyActionType,
     CountAction,
-    DefaultAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataIPv6PrefixListEntry,
     DestinationIPv6Entry,
     DestinationPortEntry,
     DeviceAccessProtocol,
     Match,
-    PolicyActionType,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     SourceDataIPv6PrefixListEntry,
     SourceIPv6Entry,
     SourcePortEntry,
 )
 
 DeviceAccessIPv6PolicySequenceMatchEntry = Annotated[
@@ -47,60 +49,68 @@
     entries: List[DeviceAccessIPv6PolicySequenceMatchEntry] = []
 
 
 class DeviceAccessIPv6PolicySequence(PolicyDefinitionSequenceBase):
     sequence_type: Literal["deviceaccesspolicyv6"] = Field(
         default="deviceaccesspolicyv6", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
-    base_action: PolicyActionType = Field(
+    base_action: BasicPolicyActionType = Field(
         default="accept", serialization_alias="baseAction", validation_alias="baseAction"
     )
     match: DeviceAccessIPv6PolicySequenceMatch = DeviceAccessIPv6PolicySequenceMatch()
     actions: List[DeviceAccessIPv6PolicySequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_device_access_protocol(self, port: DeviceAccessProtocol) -> None:
         self._insert_match(DestinationPortEntry.from_port_set_and_ranges(ports={port}))
 
     def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(SourceDataIPv6PrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(SourceDataIPv6PrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_source_ip(self, networks: List[IPv6Network]) -> None:
         self._insert_match(SourceIPv6Entry.from_ipv6_networks(networks))
 
     def match_source_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(SourcePortEntry.from_port_set_and_ranges(ports, port_ranges))
 
     def match_destination_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(DestinationDataIPv6PrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(DestinationDataIPv6PrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_destination_ip(self, networks: List[IPv6Network]) -> None:
         self._insert_match(DestinationIPv6Entry.from_ipv6_networks(networks))
 
     def associate_count_action(self, counter_name: str) -> None:
         self._insert_action(CountAction(parameter=counter_name))
 
 
 class DeviceAccessIPv6Policy(DeviceAccessIPv6PolicyHeader, DefinitionWithSequencesCommonBase):
     sequences: List[DeviceAccessIPv6PolicySequence] = []
-    default_action: DefaultAction = Field(
-        default=DefaultAction(type="drop"),
+    default_action: BasicPolicyAction = Field(
+        default=BasicPolicyAction(type="drop"),
         serialization_alias="defaultAction",
         validation_alias="defaultAction",
     )
     model_config = ConfigDict(populate_by_name=True)
 
     def add_acl_sequence(
         self,
         name: str = "Device Access Control List",
-        base_action: PolicyActionType = "accept",
+        base_action: BasicPolicyActionType = "accept",
         device_access_protocol: Optional[DeviceAccessProtocol] = None,
     ) -> DeviceAccessIPv6PolicySequence:
         seq = DeviceAccessIPv6PolicySequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         if device_access_protocol is not None:
             seq.match_device_access_protocol(port=device_access_protocol)
         self.add(seq)
         return seq
+
+
+class DeviceAccessIPv6PolicyEditPayload(DeviceAccessIPv6Policy, PolicyDefinitionId):
+    pass
+
+
+class DeviceAccessIPv6PolicyGetResponse(DeviceAccessIPv6Policy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/hub_and_spoke.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/hub_and_spoke.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
-from catalystwan.models.policy.policy_definition import PolicyDefinitionBase
+from catalystwan.models.policy.policy_definition import (
+    PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
+)
 
 
 class Hub(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     site_list: UUID = Field(validation_alias="siteList", serialization_alias="siteList")
     preference: Optional[str] = None
     prefix_lists: List[UUID] = Field(default=[], validation_alias="prefixLists", serialization_alias="prefixLists")
@@ -67,7 +71,15 @@
             equal_preference=True,
             advertise_tloc=(advertise_tloc_list is not None),
             tloc_list=advertise_tloc_list,
             spokes=spokes,
         )
         self.definition.sub_definitions.append(sub_definition)
         return sub_definition
+
+
+class HubAndSpokePolicyEditPayload(HubAndSpokePolicy, PolicyDefinitionId):
+    pass
+
+
+class HubAndSpokePolicyGetResponse(HubAndSpokePolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/mesh.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/mesh.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
-from catalystwan.models.policy.policy_definition import PolicyDefinitionBase
+from catalystwan.models.policy.policy_definition import (
+    PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
+)
 
 
 class Region(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     name: str
     site_lists: List[UUID] = Field(validation_alias="siteLists", serialization_alias="siteLists")
 
@@ -29,7 +33,15 @@
     def from_vpn_list(name: str, vpn_list: UUID) -> "MeshPolicy":
         return MeshPolicy(name=name, definition=MeshPolicyDefinition(vpn_list=vpn_list))
 
     def add_region(self, name: str, site_lists: List[UUID]) -> Region:
         region = Region(name=name, site_lists=site_lists)
         self.definition.regions.append(region)
         return region
+
+
+class MeshPolicyEditPayload(MeshPolicy, PolicyDefinitionId):
+    pass
+
+
+class MeshPolicyGetResponse(MeshPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/qos_map.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/qos_map.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,70 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field, field_validator, model_validator
 
-from catalystwan.models.policy.policy_definition import PolicyDefinitionBase
+from catalystwan.models.common import IntStr
+from catalystwan.models.policy.policy_definition import (
+    PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
+)
 
 QoSScheduling = Literal[
     "llq",
     "wrr",
 ]
 
 QoSDropType = Literal[
     "tail-drop",
     "red-drop",
 ]
 
 
 class QoSScheduler(BaseModel):
-    queue: str
-    class_map_ref: Union[UUID, Literal[""]] = Field(serialization_alias="classMapRef", validation_alias="classMapRef")
-    bandwidth_percent: str = Field("1", serialization_alias="bandwidthPercent", validation_alias="bandwidthPercent")
-    buffer_percent: str = Field("1", serialization_alias="bufferPercent", validation_alias="bufferPercent")
-    burst: Optional[str] = None
+    queue: IntStr = Field(ge=0, le=8)
+    class_map_ref: Optional[UUID] = Field(
+        default=None, serialization_alias="classMapRef", validation_alias="classMapRef"
+    )
+    bandwidth_percent: IntStr = Field(
+        default=1, ge=1, le=100, serialization_alias="bandwidthPercent", validation_alias="bandwidthPercent"
+    )
+    buffer_percent: IntStr = Field(
+        default=1, ge=1, le=100, serialization_alias="bufferPercent", validation_alias="bufferPercent"
+    )
+    burst: Optional[IntStr] = Field(default=None, ge=5000, le=10_000_000)
     scheduling: QoSScheduling = "wrr"
     drops: QoSDropType = "tail-drop"
     temp_key_values: Optional[str] = Field(
         default=None, serialization_alias="tempKeyValues", validation_alias="tempKeyValues"
     )
 
     @staticmethod
     def get_default_control_scheduler() -> "QoSScheduler":
         return QoSScheduler(
-            queue="0",
-            class_map_ref="",
-            bandwidth_percent="100",
-            buffer_percent="100",
-            burst="15000",
+            queue=0,
+            bandwidth_percent=100,
+            buffer_percent=100,
+            burst=15000,
             scheduling="llq",
             drops="tail-drop",
         )
 
     model_config = ConfigDict(populate_by_name=True)
 
-    @field_validator("queue")
+    @field_validator("class_map_ref", mode="before")
     @classmethod
-    def check_queue(cls, queue_str: str):
-        assert 0 <= int(queue_str) <= 7
-        return queue_str
-
-    @field_validator("bandwidth_percent", "buffer_percent")
-    @classmethod
-    def check_bandwidth_and_buffer_percent(cls, percent_str: str):
-        assert 1 <= int(percent_str) <= 100
-        return percent_str
-
-    @field_validator("burst")
-    @classmethod
-    def check_burst(cls, burst_val: Union[str, None]):
-        if burst_val is not None:
-            assert 5000 <= int(burst_val) <= 10_000_000
-        return burst_val
+    def check_optional_class_map_ref(cls, class_map_ref: Union[str, None]):
+        # None and "" indicates missing value, both can be found in server responses
+        if not class_map_ref:
+            return None
+        return class_map_ref
 
 
 class QoSMapDefinition(BaseModel):
     qos_schedulers: List[QoSScheduler] = Field(serialization_alias="qosSchedulers", validation_alias="qosSchedulers")
     model_config = ConfigDict(populate_by_name=True)
 
 
@@ -82,23 +81,31 @@
         buffer: int = 1,
         scheduling: QoSScheduling = "wrr",
         drops: QoSDropType = "tail-drop",
         burst: Optional[int] = None,
     ) -> None:
         self.definition.qos_schedulers.append(
             QoSScheduler(
-                queue=str(queue),
+                queue=queue,
                 class_map_ref=class_map_ref,
-                bandwidth_percent=str(bandwidth),
-                buffer_percent=str(buffer),
-                burst=str(burst) if burst is not None else None,
+                bandwidth_percent=bandwidth,
+                buffer_percent=buffer,
+                burst=burst,
                 scheduling=scheduling,
                 drops=drops,
             )
         )
 
     @model_validator(mode="after")
     def generate_default_control_scheduler(self):
         if not self.definition.qos_schedulers:
             # Only when creating (not when value obtained from remote is present)
             self.definition = QoSMapDefinition(qos_schedulers=[QoSScheduler.get_default_control_scheduler()])
         return self
+
+
+class QoSMapPolicyEditPayload(QoSMapPolicy, PolicyDefinitionId):
+    pass
+
+
+class QoSMapPolicyGetResponse(QoSMapPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/rewrite.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/rewrite.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,33 +5,43 @@
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from catalystwan.models.policy.policy_definition import (
     DefinitionWithSequencesCommonBase,
     PLPEntryType,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
 )
 
 
 class RewritePolicyHeader(PolicyDefinitionBase):
     type: Literal["rewriteRule"] = "rewriteRule"
 
 
 class RewritePolicyRule(BaseModel):
     class_: UUID = Field(serialization_alias="class", validation_alias="class")
     plp: str
     dscp: str
-    l2cos: str = Field(serialization_alias="layer2Cos", validation_alias="layer2Cos")
+    l2cos: int = Field(serialization_alias="layer2Cos", validation_alias="layer2Cos")
     model_config = ConfigDict(populate_by_name=True)
 
 
 class RewritePolicyDefinition(BaseModel):
     rules: List[RewritePolicyRule] = []
 
 
 class RewritePolicy(RewritePolicyHeader, DefinitionWithSequencesCommonBase):
     definition: RewritePolicyDefinition = RewritePolicyDefinition()
 
     def add_rule(self, class_map_ref: UUID, dscp: int, l2cos: int, plp: PLPEntryType) -> None:
-        self.definition.rules.append(RewritePolicyRule(class_=class_map_ref, plp=plp, dscp=str(dscp), l2cos=str(l2cos)))
+        self.definition.rules.append(RewritePolicyRule(class_=class_map_ref, plp=plp, dscp=str(dscp), l2cos=l2cos))
 
     model_config = ConfigDict(populate_by_name=True)
+
+
+class RewritePolicyEditPayload(RewritePolicy, PolicyDefinitionId):
+    pass
+
+
+class RewritePolicyGetResponse(RewritePolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/rule_set.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/rule_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from ipaddress import IPv4Network, IPv6Network
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field, model_validator
-from typing_extensions import Annotated
 
 from catalystwan.models.common import check_fields_exclusive
-from catalystwan.models.policy.policy_definition import PolicyDefinitionBase, Reference, VariableName
+from catalystwan.models.policy.policy_definition import (
+    PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
+    Reference,
+    VariableName,
+)
 
 
 class RuleBase(BaseModel):
     rule: str = ""
     order: str = ""
     action: str = "permit"
     source_security_group: Optional[Reference] = Field(
@@ -33,15 +38,15 @@
     @model_validator(mode="after")
     def check_exclusive_fields(self):
         check_fields_exclusive(self.__dict__, {"protocol", "protocol_name", "protocol_name_list"}, False)
         return self
 
 
 class IPv4Rule(RuleBase):
-    sequence_ip_type: Literal["ipv4"] = Field(
+    sequence_ip_type: Literal[None, "ipv4"] = Field(
         default="ipv4", serialization_alias="sequenceIpType", validation_alias="sequenceIpType"
     )
     source_ip: Union[IPv4Network, VariableName, None] = Field(
         default=None, serialization_alias="sourceIP", validation_alias="sourceIP"
     )
     source_data_prefix_list: Optional[Reference] = Field(
         default=None, serialization_alias="sourceDataPrefixList", validation_alias="sourceDataPrefixList"
@@ -140,15 +145,15 @@
             self.__dict__,
             {"destination_security_group", "destination_ipv6", "destination_ipv6_data_prefix_list"},
             False,
         )
         return self
 
 
-Rule = Annotated[Union[IPv4Rule, IPv6Rule], Field(discriminator="sequence_ip_type")]
+Rule = Union[IPv4Rule, IPv6Rule]
 
 
 class RuleSetDefinition(BaseModel):
     rules: List[Rule] = []
 
 
 class RuleSet(PolicyDefinitionBase):
@@ -250,7 +255,15 @@
             destination_port=destination_port,
             destination_port_list=Reference(ref=destination_port_list_id) if destination_port_list_id else None,
             protocol=" ".join(str(p) for p in protocols) if protocols else None,
             protocol_name=" ".join(p for p in protocol_names) if protocol_names else None,
             protocol_name_list=Reference(ref=protocol_name_list_id) if protocol_name_list_id else None,
         )
         self.add(ipv4_rule)
+
+
+class RuleSetEditPayload(RuleSet, PolicyDefinitionId):
+    pass
+
+
+class RuleSetGetResponse(RuleSet, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/security_group.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/security_group.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 
 from ipaddress import IPv4Network, IPv6Network
 from typing import Literal, Optional, Union
 
 from pydantic import BaseModel, ConfigDict, Field, model_validator
 
 from catalystwan.models.common import check_any_of_exclusive_field_sets, check_fields_exclusive
-from catalystwan.models.policy.policy_definition import PolicyDefinitionBase, Reference, VariableName
+from catalystwan.models.policy.policy_definition import (
+    PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
+    Reference,
+    VariableName,
+)
 
 SequenceIPType = Literal[
     "ipv4",
     "ipv6",
 ]
 
 
@@ -63,7 +69,15 @@
         if (
             self.sequence_ip_type == SequenceIPType.IPV4 and isinstance(self.definition, SecurityGroupIPv6Definition)
         ) or (
             self.sequence_ip_type == SequenceIPType.IPV6 and isinstance(self.definition, SecurityGroupIPv4Definition)
         ):
             raise ValueError(f"Incompatible definition for {self.sequence_ip_type} sequence")
         return self
+
+
+class SecurityGroupEditPayload(SecurityGroup, PolicyDefinitionId):
+    pass
+
+
+class SecurityGroupGetResponse(SecurityGroup, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/traffic_data.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/traffic_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 from ipaddress import IPv4Address, IPv4Network
 from typing import Any, List, Literal, Optional, Set, Tuple, Union, overload
 from uuid import UUID
 
 from pydantic import ConfigDict, Field
 from typing_extensions import Annotated
 
-from catalystwan.models.common import ServiceChainNumber, TLOCColor
-from catalystwan.models.policy.lists_entries import EncapType
+from catalystwan.models.common import EncapType, ICMPMessageType, ServiceChainNumber, TLOCColor
 from catalystwan.models.policy.policy_definition import (
     AppListEntry,
+    BasicPolicyAction,
+    BasicPolicyActionType,
     CFlowDAction,
     CountAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataIPv6PrefixListEntry,
     DestinationDataPrefixListEntry,
     DestinationIPEntry,
     DestinationPortEntry,
@@ -22,30 +23,32 @@
     DNSAppListEntry,
     DNSEntry,
     DNSTypeEntryType,
     DREOptimizationAction,
     DSCPEntry,
     FallBackToRoutingAction,
     ForwardingClassEntry,
+    ICMPMessageEntry,
     LocalTLOCListEntry,
     LocalTLOCListEntryValue,
     LogAction,
     LossProtectionAction,
     LossProtectionFECAction,
     LossProtectionPacketDuplicationAction,
     LossProtectionType,
     Match,
     NATAction,
     NextHopEntry,
     NextHopLooseEntry,
     PacketLengthEntry,
     PLPEntry,
     PolicerListEntry,
-    PolicyActionType,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     PrefferedColorGroupListEntry,
     ProtocolEntry,
     RedirectDNSAction,
     SecureInternetGatewayAction,
     ServiceChainEntry,
     ServiceChainEntryValue,
@@ -62,32 +65,33 @@
     TrafficToEntry,
     VPNEntry,
     accept_action,
 )
 
 TrafficDataPolicySequenceEntry = Annotated[
     Union[
+        AppListEntry,
+        DestinationDataIPv6PrefixListEntry,
+        DestinationDataPrefixListEntry,
+        DestinationIPEntry,
+        DestinationPortEntry,
+        DestinationRegionEntry,
+        DNSAppListEntry,
+        DNSEntry,
+        DSCPEntry,
+        ICMPMessageEntry,
         PacketLengthEntry,
         PLPEntry,
         ProtocolEntry,
-        DSCPEntry,
+        SourceDataIPv6PrefixListEntry,
+        SourceDataPrefixListEntry,
         SourceIPEntry,
         SourcePortEntry,
-        DestinationIPEntry,
-        DestinationPortEntry,
         TCPEntry,
-        DNSEntry,
         TrafficToEntry,
-        SourceDataPrefixListEntry,
-        DestinationDataPrefixListEntry,
-        SourceDataIPv6PrefixListEntry,
-        DestinationDataIPv6PrefixListEntry,
-        DestinationRegionEntry,
-        DNSAppListEntry,
-        AppListEntry,
     ],
     Field(discriminator="field"),
 ]
 
 TrafficDataPolicySequenceActions = Any  # TODO
 
 
@@ -96,15 +100,15 @@
 
 
 class TrafficDataPolicySequenceMatch(Match):
     entries: List[TrafficDataPolicySequenceEntry] = []
 
 
 class TrafficDataPolicySequence(PolicyDefinitionSequenceBase):
-    sequence_type: Literal["data"] = Field(
+    sequence_type: Literal["applicationFirewall", "qos", "serviceChaining", "trafficEngineering", "data"] = Field(
         default="data", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
     match: TrafficDataPolicySequenceMatch = TrafficDataPolicySequenceMatch()
     actions: List[TrafficDataPolicySequenceActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_app_list(self, app_list_id: UUID) -> None:
@@ -118,37 +122,40 @@
 
     def match_dns_response(self) -> None:
         self._insert_match(DNSEntry(value="response"))
 
     def match_dscp(self, dscp: int) -> None:
         self._insert_match(DSCPEntry(value=str(dscp)))
 
+    def match_icmp(self, icmp_message_types: List[ICMPMessageType]) -> None:
+        self._insert_match(ICMPMessageEntry(value=icmp_message_types))
+
     def match_packet_length(self, packet_lengths: Tuple[int, int]) -> None:
         self._insert_match(PacketLengthEntry.from_range(packet_lengths))
 
     def match_low_plp(self) -> None:
         self._insert_match(PLPEntry(value="low"))
 
     def match_high_plp(self) -> None:
         self._insert_match(PLPEntry(value="high"))
 
     def match_protocols(self, protocols: Set[int]) -> None:
         self._insert_match(ProtocolEntry.from_protocol_set(protocols))
 
-    def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_list_id))
+    def match_source_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
+        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_lists))
 
     def match_source_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(SourceIPEntry.from_ipv4_networks(networks))
 
     def match_source_port(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(SourcePortEntry.from_port_set_and_ranges(ports, port_ranges))
 
     def match_destination_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(DestinationDataPrefixListEntry(ref=data_prefix_list_id))
+        self._insert_match(DestinationDataPrefixListEntry(ref=[data_prefix_list_id]))
 
     def match_destination_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(DestinationIPEntry.from_ipv4_networks(networks))
 
     def match_primary_destination_region(self) -> None:
         self._insert_match(DestinationRegionEntry(value="primary-region"))
 
@@ -355,19 +362,32 @@
             self._insert_action(FallBackToRoutingAction())
         else:
             self._remove_action(FallBackToRoutingAction().type)
 
 
 class TrafficDataPolicy(TrafficDataPolicyHeader, DefinitionWithSequencesCommonBase):
     sequences: List[TrafficDataPolicySequence] = []
+    default_action: BasicPolicyAction = Field(
+        default=BasicPolicyAction(type="drop"),
+        serialization_alias="defaultAction",
+        validation_alias="defaultAction",
+    )
     model_config = ConfigDict(populate_by_name=True)
 
     def add_ipv4_sequence(
-        self, name: str = "Custom", base_action: PolicyActionType = "drop", log: bool = False
+        self, name: str = "Custom", base_action: BasicPolicyActionType = "drop", log: bool = False
     ) -> TrafficDataPolicySequence:
         seq = TrafficDataPolicySequence(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
         )
         self.add(seq)
         return seq
+
+
+class TrafficDataPolicyEditPayload(TrafficDataPolicy, PolicyDefinitionId):
+    pass
+
+
+class TrafficDataPolicyGetResponse(TrafficDataPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/vpn_membership.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/vpn_membership.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
-from catalystwan.models.policy.policy_definition import PolicyDefinitionBase
+from catalystwan.models.policy.policy_definition import (
+    PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
+)
 
 
 class Site(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     site_list: UUID = Field(validation_alias="siteList", serialization_alias="siteList")
     vpn_list: List[UUID] = Field(validation_alias="vpnList", serialization_alias="vpnList")
 
@@ -24,7 +28,15 @@
     type: Literal["vpnMembershipGroup"] = "vpnMembershipGroup"
     definition: VPNMembershipPolicyDefinition = VPNMembershipPolicyDefinition()
 
     def add_site(self, site_list: UUID, vpn_lists: List[UUID]) -> Site:
         site = Site(site_list=site_list, vpn_list=vpn_lists)
         self.definition.sites.append(site)
         return site
+
+
+class VPNMembershipPolicyEditPayload(VPNMembershipPolicy, PolicyDefinitionId):
+    pass
+
+
+class VPNMembershipPolicyGetResponse(VPNMembershipPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/definitions/zone_based_firewall.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/definition/zone_based_firewall.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,88 +5,114 @@
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from catalystwan.models.misc.application_protocols import ApplicationProtocol
 from catalystwan.models.policy.policy_definition import (
+    AdvancedInspectionProfileAction,
     AppListEntry,
+    AppListFlatEntry,
+    ConnectionEventsAction,
     DefinitionWithSequencesCommonBase,
     DestinationDataPrefixListEntry,
     DestinationFQDNEntry,
     DestinationGeoLocationEntry,
     DestinationGeoLocationListEntry,
     DestinationIPEntry,
     DestinationPortEntry,
     DestinationPortListEntry,
+    DestinationScalableGroupTagListEntry,
     LogAction,
     Match,
-    PolicyActionType,
+    PolicyActionBase,
     PolicyDefinitionBase,
+    PolicyDefinitionGetResponse,
+    PolicyDefinitionId,
     PolicyDefinitionSequenceBase,
     ProtocolEntry,
     ProtocolNameEntry,
     ProtocolNameListEntry,
     RuleSetListEntry,
     SourceDataPrefixListEntry,
     SourceFQDNEntry,
     SourceFQDNListEntry,
     SourceGeoLocationEntry,
     SourceGeoLocationListEntry,
     SourceIPEntry,
     SourcePortEntry,
     SourcePortListEntry,
+    SourceScalableGroupTagListEntry,
 )
 
 ZoneBasedFWPolicySequenceEntry = Annotated[
     Union[
         AppListEntry,
+        AppListFlatEntry,
         DestinationDataPrefixListEntry,
         DestinationFQDNEntry,
         DestinationGeoLocationEntry,
         DestinationGeoLocationListEntry,
         DestinationIPEntry,
         DestinationPortEntry,
         DestinationPortListEntry,
+        DestinationScalableGroupTagListEntry,
         ProtocolEntry,
         ProtocolNameEntry,
         ProtocolNameListEntry,
         RuleSetListEntry,
         SourceDataPrefixListEntry,
         SourceFQDNEntry,
         SourceFQDNListEntry,
         SourceGeoLocationEntry,
         SourceGeoLocationListEntry,
         SourceIPEntry,
         SourcePortEntry,
         SourcePortListEntry,
+        SourceScalableGroupTagListEntry,
     ],
     Field(discriminator="field"),
 ]
 
 ZoneBasedFWPolicySequenceEntryWithRuleSets = Annotated[
     Union[
         AppListEntry,
         RuleSetListEntry,
     ],
     Field(discriminator="field"),
 ]
 
+ZoneBasedFWPolicyActions = Annotated[
+    Union[
+        AdvancedInspectionProfileAction,
+        ConnectionEventsAction,
+        LogAction,
+    ],
+    Field(discriminator="type"),
+]
+
+ZoneBasedFirewallDefaultActionType = Literal["drop", "pass"]
+ZoneBasedFirewallBaseActionType = Literal["drop", "pass", "inspect"]
+
+
+class ZoneBasedFirewallDefaultAction(PolicyActionBase):
+    type: ZoneBasedFirewallDefaultActionType
+
 
 class ZoneBasedFWPolicyMatches(Match):
     entries: List[ZoneBasedFWPolicySequenceEntry] = []
 
 
 class ZoneBasedFWPolicySequenceWithRuleSets(PolicyDefinitionSequenceBase):
     sequence_type: Literal["zoneBasedFW"] = Field(
         default="zoneBasedFW", serialization_alias="sequenceType", validation_alias="sequenceType"
     )
     match: ZoneBasedFWPolicyMatches
     ruleset: bool = True
-    actions: List[LogAction] = []
+    actions: List[ZoneBasedFWPolicyActions] = []
     model_config = ConfigDict(populate_by_name=True)
 
     def match_rule_set_lists(self, rule_set_ids: Set[UUID]) -> None:
         self._insert_match(RuleSetListEntry.from_rule_set_ids(rule_set_ids))
 
     def match_app_list(self, app_list_id: UUID) -> None:
         if self.base_action != "inspect":
@@ -103,16 +129,16 @@
     model_config = ConfigDict(populate_by_name=True)
 
     def match_app_list(self, app_list_id: UUID) -> None:
         if self.base_action != "inspect":
             raise ValueError("Action must be inspect when Application/Application Family List is selected.")
         self._insert_match(AppListEntry(ref=app_list_id))
 
-    def match_destination_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(DestinationDataPrefixListEntry(ref=data_prefix_list_id))
+    def match_destination_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
+        self._insert_match(DestinationDataPrefixListEntry(ref=data_prefix_lists))
 
     def match_destination_fqdn(self, fqdn: str) -> None:
         self._insert_match(DestinationFQDNEntry(value=fqdn))
 
     def match_destination_geo_location(self, geo_location: str) -> None:
         self._insert_match(DestinationGeoLocationEntry(value=geo_location))
 
@@ -121,36 +147,36 @@
 
     def match_destination_ip(self, networks: List[IPv4Network]) -> None:
         self._insert_match(DestinationIPEntry.from_ipv4_networks(networks))
 
     def match_destination_ports(self, ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> None:
         self._insert_match(DestinationPortEntry.from_port_set_and_ranges(ports, port_ranges))
 
-    def match_destination_port_list(self, port_list_id: UUID) -> None:
-        self._insert_match(DestinationPortListEntry(ref=port_list_id))
+    def match_destination_port_list(self, data_prefix_lists: List[UUID]) -> None:
+        self._insert_match(DestinationPortListEntry(ref=data_prefix_lists))
 
     def match_protocols(self, protocols: Set[int]) -> None:
         self._insert_match(ProtocolEntry.from_protocol_set(protocols))
 
     def match_protocol_names(self, names: Set[str], protocol_map: Dict[str, ApplicationProtocol]) -> None:
         app_protocols = []
         for name in names:
             app_protocol = protocol_map.get(name, None)
             if app_protocol is None:
-                raise ValueError(f"{name} not found in protocol map keys: {protocol_map.keys()}")
+                raise ValueError(f"{name} not found in protocol map keys: {protocol_map.keys()}")  # noqa: E713
             app_protocols.append(app_protocol)
         self._insert_match(ProtocolNameEntry.from_application_protocols(app_protocols))
         self._insert_match(DestinationPortEntry.from_application_protocols(app_protocols), False)
         self._insert_match(ProtocolEntry.from_application_protocols(app_protocols), False)
 
     def match_protocol_name_list(self, protocol_name_list_id: UUID) -> None:
         self._insert_match(ProtocolNameListEntry(ref=protocol_name_list_id))
 
-    def match_source_data_prefix_list(self, data_prefix_list_id: UUID) -> None:
-        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_list_id))
+    def match_source_data_prefix_list(self, data_prefix_lists: List[UUID]) -> None:
+        self._insert_match(SourceDataPrefixListEntry(ref=data_prefix_lists))
 
     def match_source_fqdn(self, fqdn: str) -> None:
         self._insert_match(SourceFQDNEntry(value=fqdn))
 
     def match_source_fqdn_list(self, fqdn_list_id: UUID) -> None:
         self._insert_match(SourceFQDNListEntry(ref=fqdn_list_id))
 
@@ -181,25 +207,30 @@
 class ZoneBasedFWPolicyHeader(PolicyDefinitionBase):
     type: Literal["zoneBasedFW"] = "zoneBasedFW"
     mode: str = Field(default="security")
     model_config = ConfigDict(populate_by_name=True)
 
 
 class ZoneBasedFWPolicyDefinition(DefinitionWithSequencesCommonBase):
+    default_action: ZoneBasedFirewallDefaultAction = Field(
+        default=ZoneBasedFirewallDefaultAction(type="drop"),
+        serialization_alias="defaultAction",
+        validation_alias="defaultAction",
+    )
     sequences: List[Union[ZoneBasedFWPolicySequence, ZoneBasedFWPolicySequenceWithRuleSets]] = []
     entries: List[ZoneBasedFWPolicyEntry] = []
 
 
 class ZoneBasedFWPolicy(ZoneBasedFWPolicyHeader):
     type: Literal["zoneBasedFW"] = "zoneBasedFW"
-    mode: Literal["security"] = "security"
+    mode: Literal["security", "unified"] = "security"
     definition: ZoneBasedFWPolicyDefinition = ZoneBasedFWPolicyDefinition()
 
     def add_ipv4_rule(
-        self, name: str, base_action: PolicyActionType = "drop", log: bool = False
+        self, name: str, base_action: ZoneBasedFirewallBaseActionType = "drop", log: bool = False
     ) -> ZoneBasedFWPolicySequence:
         """Adds new IPv4 Rule to Zone Based Firewall Policy
 
         Args:
             name (str): Rule name
             base_action (BaseAction, optional): Rule base action (drop, pass, inspect) Defaults to BaseAction.DROP.
             log (bool, optional): If true sets log action
@@ -215,15 +246,15 @@
         )
         if log:
             sequence.actions.append(LogAction())
         self.definition.add(sequence)
         return sequence
 
     def add_ipv4_rule_sets(
-        self, name: str, base_action: PolicyActionType = "drop", log: bool = False
+        self, name: str, base_action: ZoneBasedFirewallBaseActionType = "drop", log: bool = False
     ) -> ZoneBasedFWPolicySequenceWithRuleSets:
         sequence = ZoneBasedFWPolicySequenceWithRuleSets(
             sequence_name=name,
             base_action=base_action,
             sequence_ip_type="ipv4",
             match=ZoneBasedFWPolicyMatches(),
         )
@@ -234,7 +265,15 @@
 
     def add_zone_pair(self, source_zone_id: UUID, destination_zone_id: UUID) -> None:
         entry = ZoneBasedFWPolicyEntry(
             source_zone_id=source_zone_id,
             destination_zone_id=destination_zone_id,
         )
         self.definition.entries.append(entry)
+
+
+class ZoneBasedFWPolicyEditPayload(ZoneBasedFWPolicy, PolicyDefinitionId):
+    pass
+
+
+class ZoneBasedFWPolicyGetResponse(ZoneBasedFWPolicy, PolicyDefinitionGetResponse):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/localized.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/localized.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
-from typing import List, Literal, Optional
+from typing import Any, List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field, IPvAnyAddress, field_validator
+from pydantic import BaseModel, ConfigDict, Field, IPvAnyAddress, model_validator
 
 from catalystwan.models.policy.policy import AssemblyItemBase, PolicyCreationPayload, PolicyDefinition, PolicyInfo
 
 LocalizedPolicySupportedItemType = Literal[
     "qosMap",
     "rewriteRule",
     "vpnQoSMap",
@@ -17,14 +17,19 @@
     "deviceAccessPolicy",
     "deviceaccesspolicyv6",
     "deviceAccessPolicyv6",
     "vedgeRoute",
 ]
 
 
+def assert_feature_defintion(definition: Any) -> "LocalizedPolicyDefinition":
+    assert isinstance(definition, LocalizedPolicyDefinition)
+    return definition
+
+
 class LocalizedPolicySettings(BaseModel):
     flow_visibility: Optional[bool] = Field(
         default=None, serialization_alias="flowVisibility", validation_alias="flowVisibility"
     )
     flow_visibility_ipv6: Optional[bool] = Field(
         default=None, serialization_alias="flowVisibilityIPv6", validation_alias="flowVisibilityIPv6"
     )
@@ -64,28 +69,33 @@
 class LocalizedPolicyAssemblyItem(AssemblyItemBase):
     type: LocalizedPolicySupportedItemType
     definition_id: UUID = Field(serialization_alias="definitionId", validation_alias="definitionId")
     model_config = ConfigDict(populate_by_name=True)
 
 
 class LocalizedPolicyDefinition(PolicyDefinition):
-    assembly: List[LocalizedPolicyAssemblyItem]
-    settings: LocalizedPolicySettings
+    assembly: List[LocalizedPolicyAssemblyItem] = []
+    settings: Optional[LocalizedPolicySettings] = None
 
 
 class LocalizedPolicy(PolicyCreationPayload):
-    policy_definition: LocalizedPolicyDefinition = Field(
+    policy_definition: Union[LocalizedPolicyDefinition, str] = Field(
         default=LocalizedPolicyDefinition(assembly=[], settings=LocalizedPolicySettings()),
         serialization_alias="policyDefinition",
         validation_alias="policyDefinition",
     )
-    policy_type: str = Field(default="feature", serialization_alias="policyType", validation_alias="policyType")
+    policy_type: Literal["feature", "cli"] = Field(
+        default="feature", serialization_alias="policyType", validation_alias="policyType"
+    )
 
-    def _add_item(self, type: LocalizedPolicySupportedItemType, id: UUID) -> None:
-        self.policy_definition.assembly.append(LocalizedPolicyAssemblyItem(type=type, definition_id=id))
+    def _add_item(self, type: LocalizedPolicySupportedItemType, id: UUID) -> LocalizedPolicyAssemblyItem:
+        policy_definition = assert_feature_defintion(self.policy_definition)
+        item = LocalizedPolicyAssemblyItem(type=type, definition_id=id)
+        policy_definition.assembly.append(item)
+        return item
 
     def add_qos_map(self, definition_id: UUID) -> None:
         self._add_item("qosMap", definition_id)
 
     def add_rewrite_rule(self, definition_id: UUID) -> None:
         self._add_item("rewriteRule", definition_id)
 
@@ -103,23 +113,28 @@
 
     def add_device_access_policy_ipv6(self, definition_id: UUID) -> None:
         self._add_item("deviceAccessPolicyv6", definition_id)
 
     def add_route_policy(self, definition_id: UUID) -> None:
         self._add_item("vedgeRoute", definition_id)
 
-    @field_validator("policy_definition", mode="before")
+    @model_validator(mode="before")
     @classmethod
-    def try_parse(cls, policy_definition):
+    def try_parse_policy_definition_string(cls, values):
         # this is needed because GET /template/policy/vedge contains string in policyDefinition field
         # while POST /template/policy/vedge requires a regular object
         # it makes sense to reuse that model for both requests and present parsed data to the user
-        if isinstance(policy_definition, str):
-            return LocalizedPolicyDefinition.model_validate_json(policy_definition)
-        return policy_definition
+        if not isinstance(values, dict):
+            return values
+        if (policy_definition := values.get("policyDefinition")) and values.get("policyType") != "cli":
+            if isinstance(policy_definition, str):
+                values["policyDefinition"] = LocalizedPolicyDefinition.model_validate_json(policy_definition)
+        else:
+            values["policyDefinition"] = LocalizedPolicyDefinition()
+        return values
 
 
 class LocalizedPolicyInfo(PolicyInfo, LocalizedPolicy):
     pass
 
 
 class LocalizedPolicyEditResponse(BaseModel):
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/policy.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 import datetime
 from typing import List, Literal, Optional, Sequence, Union
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
 
+ZoneListId = Union[UUID, Literal["self", "default"]]
+
 
 class PolicyId(BaseModel):
     policy_id: UUID = Field(serialization_alias="policyId", validation_alias="policyId")
 
 
 class NGFirewallZoneListEntry(BaseModel):
-    src_zone_list_id: UUID = Field(serialization_alias="srcZoneListId", validation_alias="srcZoneListId")
-    dst_zone_list_id: UUID = Field(serialization_alias="dstZoneListId", validation_alias="dstZoneListId")
+    src_zone_list_id: ZoneListId = Field(serialization_alias="srcZoneListId", validation_alias="srcZoneListId")
+    dst_zone_list_id: ZoneListId = Field(serialization_alias="dstZoneListId", validation_alias="dstZoneListId")
     model_config = ConfigDict(populate_by_name=True)
 
 
 class AssemblyItemBase(BaseModel):
     definition_id: UUID = Field(serialization_alias="definitionId", validation_alias="definitionId")
     type: str
     model_config = ConfigDict(populate_by_name=True)
@@ -43,14 +45,18 @@
     type: Literal["intrusionPrevention"] = "intrusionPrevention"
 
 
 class URLFilteringAssemblyItem(AssemblyItemBase):
     type: Literal["urlFiltering"] = "urlFiltering"
 
 
+class AdvancedInspectionProfileAssemblyItem(AssemblyItemBase):
+    type: Literal["advancedInspectionProfile"] = "advancedInspectionProfile"
+
+
 class AdvancedMalwareProtectionAssemblyItem(AssemblyItemBase):
     type: Literal["advancedMalwareProtection"] = "advancedMalwareProtection"
 
 
 class SSLDecryptionAssemblyItem(AssemblyItemBase):
     type: Literal["sslDecryption"] = "sslDecryption"
 
@@ -59,24 +65,23 @@
     assembly: Sequence[AssemblyItemBase] = []
 
 
 class PolicyCreationPayload(BaseModel):
     policy_name: str = Field(
         serialization_alias="policyName",
         validation_alias="policyName",
-        pattern="^[a-zA-Z0-9_-]{1,127}$",
+        pattern="^[a-zA-Z0-9_-]{0,127}$",
         description="Can include only alpha-numeric characters, hyphen '-' or underscore '_'; maximum 127 characters",
     )
     policy_description: str = Field(
         default="default description", serialization_alias="policyDescription", validation_alias="policyDescription"
     )
     policy_type: str = Field(serialization_alias="policyType", validation_alias="policyType")
     policy_definition: Union[PolicyDefinition, str] = Field(
-        serialization_alias="policyDefinition",
-        validation_alias="policyDefinition",
+        serialization_alias="policyDefinition", validation_alias="policyDefinition"
     )
     is_policy_activated: bool = Field(
         default=False, serialization_alias="isPolicyActivated", validation_alias="isPolicyActivated"
     )
     model_config = ConfigDict(populate_by_name=True)
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/policy_definition.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/policy_definition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 import datetime
 from functools import wraps
 from ipaddress import IPv4Address, IPv4Network, IPv6Network
-from typing import Any, Dict, List, MutableSequence, Optional, Protocol, Sequence, Set, Tuple, Union
+from typing import Any, Dict, List, MutableSequence, Optional, Sequence, Set, Tuple, Union
 from uuid import UUID
 
-from pydantic import BaseModel, ConfigDict, Field, RootModel, model_validator
+from pydantic import BaseModel, ConfigDict, Field, RootModel, field_validator, model_validator
 from typing_extensions import Annotated, Literal
 
-from catalystwan.models.common import ServiceChainNumber, TLOCColor, check_fields_exclusive
+from catalystwan.models.common import (
+    CarrierType,
+    ControlPathType,
+    EncapType,
+    ICMPMessageType,
+    MultiRegionRole,
+    OriginProtocol,
+    SequenceIpType,
+    ServiceChainNumber,
+    ServiceType,
+    SpaceSeparatedUUIDList,
+    TLOCActionType,
+    TLOCColor,
+    check_fields_exclusive,
+    str_as_str_list,
+)
 from catalystwan.models.misc.application_protocols import ApplicationProtocol
-from catalystwan.models.policy.lists_entries import EncapType
-from catalystwan.typed_list import DataSequence
 
 
 def port_set_and_ranges_to_str(ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> str:
     assert ports or port_ranges
     ports_str = " ".join(f"{port_begin}-{port_end}" for port_begin, port_end in port_ranges)
     ports_str += " " if ports_str else ""
     ports_str += " ".join(str(p) for p in ports)
@@ -45,72 +58,37 @@
 
 DestinationRegion = Literal[
     "primary-region",
     "secondary-region",
     "other-region",
 ]
 
-OriginProtocol = Literal[
-    "aggregate",
-    "bgp",
-    "bgp-external",
-    "bgp-internal",
-    "connected",
-    "eigrp",
-    "ospf",
-    "ospf-inter-area",
-    "ospf-intra-area",
-    "ospf-external1",
-    "ospf-external2",
-    "rip",
-    "static",
-    "eigrp-summary",
-    "eigrp-internal",
-    "eigrp-external",
-    "lisp",
-    "nat-dia",
-    "natpool",
-    "isis",
-    "isis-level1",
-    "isis-level2",
-]
-
 PathType = Literal[
     "hierarchical-path",
     "direct-path",
     "transport-gateway-path",
 ]
 
-SequenceIpType = Literal[
-    "ipv4",
-    "ipv6",
-    "all",
-]
 
-PolicyActionType = Literal[
-    "drop",
-    "accept",
-    "pass",
-    "inspect",
-    "reject",
-]
+BasicPolicyActionType = Literal["accept", "drop"]
 
 SequenceType = Literal[
     "applicationFirewall",
     "data",
     "serviceChaining",
     "trafficEngineering",
     "qos",
     "zoneBasedFW",
     "tloc",
     "route",
     "acl",
     "aclv6",
     "deviceaccesspolicy",
     "deviceaccesspolicyv6",
+    "sslDecryption",
 ]
 
 
 Optimized = Literal[
     "true",
     "false",
 ]
@@ -122,48 +100,14 @@
 
 LossProtectionType = Literal[
     "fecAdaptive",
     "fecAlways",
     "packetDuplication",
 ]
 
-MultiRegionRole = Literal[
-    "border-router",
-    "edge-router",
-]
-
-ServiceType = Literal[
-    "FW",
-    "IDP",
-    "IDS",
-    "netsvc1",
-    "netsvc2",
-    "netsvc3",
-    "netsvc4",
-]
-
-TLOCActionType = Literal[
-    "strict",
-    "primary",
-    "backup",
-    "ecmp",
-]
-
-Carrier = Literal[
-    "default",
-    "carrier1",
-    "carrier2",
-    "carrier3",
-    "carrier4",
-    "carrier5",
-    "carrier6",
-    "carrier7",
-    "carrier8",
-]
-
 DeviceAccessProtocol = Literal[22, 161]
 
 
 class Reference(BaseModel):
     ref: UUID
 
 
@@ -227,15 +171,18 @@
 class DSCPEntry(BaseModel):
     field: Literal["dscp"] = "dscp"
     value: str = Field(description="0-63 single numbers separate by space")
 
 
 class SourceIPEntry(BaseModel):
     field: Literal["sourceIp"] = "sourceIp"
-    value: str = Field(description="IP network specifiers separate by space")
+    value: Optional[str] = Field(default=None, description="IP network specifiers separate by space")
+    vipVariableName: Optional[str] = Field(
+        default=None, serialization_alias="vipVariableName", validation_alias="vipVariableName"
+    )
 
     @staticmethod
     def from_ipv4_networks(networks: List[IPv4Network]) -> "SourceIPEntry":
         return SourceIPEntry(value=networks_to_str(networks))
 
 
 class SourceIPv6Entry(BaseModel):
@@ -259,15 +206,18 @@
     @staticmethod
     def from_port_set_and_ranges(ports: Set[int] = set(), port_ranges: List[Tuple[int, int]] = []) -> "SourcePortEntry":
         return SourcePortEntry(value=port_set_and_ranges_to_str(ports, port_ranges))
 
 
 class DestinationIPEntry(BaseModel):
     field: Literal["destinationIp"] = "destinationIp"
-    value: str
+    value: Optional[str] = Field(default=None)
+    vipVariableName: Optional[str] = Field(
+        default=None, serialization_alias="vipVariableName", validation_alias="vipVariableName"
+    )
 
     @staticmethod
     def from_ipv4_networks(networks: List[IPv4Network]) -> "DestinationIPEntry":
         return DestinationIPEntry(value=networks_to_str(networks))
 
 
 class DestinationIPv6Entry(BaseModel):
@@ -395,15 +345,15 @@
 class PreferenceEntry(BaseModel):
     field: Literal["preference"] = "preference"
     value: str = Field(description="Number in range 0-4294967295")
 
 
 class PathTypeEntry(BaseModel):
     field: Literal["pathType"] = "pathType"
-    value: PathType
+    value: ControlPathType
 
 
 class RegionEntry(BaseModel):
     field: Literal["regionId"] = "regionId"
     value: str
 
 
@@ -450,15 +400,15 @@
 class CommunityAdditiveEntry(BaseModel):
     field: Literal["communityAdditive"] = "communityAdditive"
     value: Literal["true"] = "true"
 
 
 class CarrierEntry(BaseModel):
     field: Literal["carrier"] = "carrier"
-    value: Carrier
+    value: CarrierType
 
 
 class DomainIDEntry(BaseModel):
     field: Literal["domainId"] = "domainId"
     value: str = Field(description="Number in range 1-4294967295")
 
 
@@ -483,44 +433,56 @@
     @staticmethod
     def from_nat_vpn(fallback: bool, vpn: int = 0) -> "NATVPNEntry":
         if fallback:
             return NATVPNEntry(root=[UseVPNEntry(value=str(vpn)), FallBackEntry()])
         return NATVPNEntry(root=[UseVPNEntry(value=str(vpn))])
 
 
+class ICMPMessageEntry(BaseModel):
+    field: Literal["icmpMessage"] = "icmpMessage"
+    value: List[ICMPMessageType]
+
+    _value = field_validator("value", mode="before")(str_as_str_list)
+
+
 class SourceDataPrefixListEntry(BaseModel):
     field: Literal["sourceDataPrefixList"] = "sourceDataPrefixList"
-    ref: UUID
+    ref: SpaceSeparatedUUIDList  # usually single id but zone based firewall can use multiple ids separated by space
 
 
 class SourceDataIPv6PrefixListEntry(BaseModel):
     field: Literal["sourceDataIpv6PrefixList"] = "sourceDataIpv6PrefixList"
-    ref: UUID
+    ref: SpaceSeparatedUUIDList  # usually single id but zone based firewall can use multiple ids separated by space
 
 
 class DestinationDataPrefixListEntry(BaseModel):
     field: Literal["destinationDataPrefixList"] = "destinationDataPrefixList"
-    ref: UUID
+    ref: SpaceSeparatedUUIDList  # usually single id but zone based firewall can use multiple ids separated by space
 
 
 class DestinationDataIPv6PrefixListEntry(BaseModel):
     field: Literal["destinationDataIpv6PrefixList"] = "destinationDataIpv6PrefixList"
-    ref: UUID
+    ref: SpaceSeparatedUUIDList  # usually single id but zone based firewall can use multiple ids separated by space
 
 
 class DNSAppListEntry(BaseModel):
     field: Literal["dnsAppList"] = "dnsAppList"
     ref: UUID
 
 
 class AppListEntry(BaseModel):
     field: Literal["appList"] = "appList"
     ref: UUID
 
 
+class AppListFlatEntry(BaseModel):
+    field: Literal["appListFlat"] = "appListFlat"
+    ref: UUID
+
+
 class SourceFQDNListEntry(BaseModel):
     field: Literal["sourceFqdnList"] = "sourceFqdnList"
     ref: UUID
 
 
 class DestinationFQDNListEntry(BaseModel):
     field: Literal["destinationFqdnList"] = "destinationFqdnList"
@@ -543,16 +505,26 @@
 
 
 class SourcePortListEntry(BaseModel):
     field: Literal["sourcePortList"] = "sourcePortList"
     ref: UUID
 
 
+class SourceScalableGroupTagListEntry(BaseModel):
+    field: Literal["sourceScalableGroupTagList"] = "sourceScalableGroupTagList"
+    ref: UUID
+
+
 class DestinationPortListEntry(BaseModel):
     field: Literal["destinationPortList"] = "destinationPortList"
+    ref: SpaceSeparatedUUIDList  # usually single id but zone based firewall can use multiple ids separated by space
+
+
+class DestinationScalableGroupTagListEntry(BaseModel):
+    field: Literal["destinationScalableGroupTagList"] = "destinationScalableGroupTagList"
     ref: UUID
 
 
 class RuleSetListEntry(BaseModel):
     field: Literal["ruleSetList"] = "ruleSetList"
     ref: str
 
@@ -567,14 +539,24 @@
 
 
 class TLOCListEntry(BaseModel):
     field: Literal["tlocList"] = "tlocList"
     ref: UUID
 
 
+class SourceVpnEntry(BaseModel):
+    field: Literal["sourceVpn"] = "sourceVpn"
+    value: str = Field(description="VPN ids numbers separated by space")
+
+
+class DestinationVpnEntry(BaseModel):
+    field: Literal["destinationVpn"] = "destinationVpn"
+    value: str = Field(description="VPN ids numbers separated by space")
+
+
 class PrefferedColorGroupListEntry(BaseModel):
     field: Literal["preferredColorGroup"] = "preferredColorGroup"
     ref: UUID
     color_restrict: bool = Field(False, serialization_alias="colorRestrict", validation_alias="colorRestrict")
     model_config = ConfigDict(populate_by_name=True)
 
 
@@ -748,14 +730,24 @@
 
 
 class PolicerAction(BaseModel):
     type: Literal["policer"] = "policer"
     parameter: Reference
 
 
+class ConnectionEventsAction(BaseModel):
+    type: Literal["connectionEvents"] = "connectionEvents"
+    parameter: str = ""
+
+
+class AdvancedInspectionProfileAction(BaseModel):
+    type: Literal["advancedInspectionProfile"] = "advancedInspectionProfile"
+    parameter: Reference
+
+
 ActionSetEntry = Annotated[
     Union[
         AffinityEntry,
         CommunityAdditiveEntry,
         CommunityEntry,
         DSCPEntry,
         ForwardingClassEntry,
@@ -782,16 +774,18 @@
     type: Literal["set"] = "set"
     parameter: List[ActionSetEntry] = []
 
 
 ActionEntry = Annotated[
     Union[
         ActionSet,
+        AdvancedInspectionProfileAction,
         CFlowDAction,
         ClassMapAction,
+        ConnectionEventsAction,
         CountAction,
         DREOptimizationAction,
         FallBackToRoutingAction,
         LogAction,
         LossProtectionAction,
         LossProtectionFECAction,
         LossProtectionPacketDuplicationAction,
@@ -806,14 +800,15 @@
     ],
     Field(discriminator="type"),
 ]
 
 MatchEntry = Annotated[
     Union[
         AppListEntry,
+        AppListFlatEntry,
         CarrierEntry,
         ClassMapListEntry,
         ColorListEntry,
         CommunityListEntry,
         DestinationDataIPv6PrefixListEntry,
         DestinationDataPrefixListEntry,
         DestinationFQDNEntry,
@@ -821,20 +816,23 @@
         DestinationGeoLocationEntry,
         DestinationGeoLocationListEntry,
         DestinationIPEntry,
         DestinationIPv6Entry,
         DestinationPortEntry,
         DestinationPortListEntry,
         DestinationRegionEntry,
+        DestinationScalableGroupTagListEntry,
+        DestinationVpnEntry,
         DNSAppListEntry,
         DNSEntry,
         DomainIDEntry,
         DSCPEntry,
         ExpandedCommunityListEntry,
         GroupIDEntry,
+        ICMPMessageEntry,
         NextHeaderEntry,
         OMPTagEntry,
         OriginatorEntry,
         OriginEntry,
         PacketLengthEntry,
         PathTypeEntry,
         PLPEntry,
@@ -856,14 +854,16 @@
         SourceFQDNListEntry,
         SourceGeoLocationEntry,
         SourceGeoLocationListEntry,
         SourceIPEntry,
         SourceIPv6Entry,
         SourcePortEntry,
         SourcePortListEntry,
+        SourceScalableGroupTagListEntry,
+        SourceVpnEntry,
         TCPEntry,
         TLOCEntry,
         TLOCListEntry,
         TrafficClassEntry,
         TrafficToEntry,
         VPNListEntry,
     ],
@@ -903,22 +903,22 @@
 class Action(BaseModel):
     pass
 
 
 class PolicyDefinitionSequenceBase(BaseModel):
     sequence_id: int = Field(default=0, serialization_alias="sequenceId", validation_alias="sequenceId")
     sequence_name: str = Field(serialization_alias="sequenceName", validation_alias="sequenceName")
-    base_action: PolicyActionType = Field(
-        default="drop", serialization_alias="baseAction", validation_alias="baseAction"
-    )
+    base_action: str = Field(serialization_alias="baseAction", validation_alias="baseAction")
     sequence_type: SequenceType = Field(serialization_alias="sequenceType", validation_alias="sequenceType")
-    sequence_ip_type: SequenceIpType = Field(serialization_alias="sequenceIpType", validation_alias="sequenceIpType")
+    sequence_ip_type: Optional[SequenceIpType] = Field(
+        default="ipv4", serialization_alias="sequenceIpType", validation_alias="sequenceIpType"
+    )
     ruleset: Optional[bool] = None
     match: Match
-    actions: Sequence[ActionEntry]
+    actions: Optional[Sequence[ActionEntry]] = None
 
     @staticmethod
     def _check_field_collision(field: str, fields: Sequence[str]) -> None:
         existing_fields = set(fields)
         forbidden_fields = set(MUTUALLY_EXCLUSIVE_FIELD_LOOKUP.get(field, []))
         colliding_fields = set(existing_fields) & set(forbidden_fields)
         assert not colliding_fields, f"{field} is mutually exclusive with {colliding_fields}"
@@ -1002,16 +1002,20 @@
     def wrapper(self: PolicyDefinitionSequenceBase, *args, **kwargs):
         assert self.base_action == "accept", f"{method.__name__} only allowed when base_action is accept"
         return method(self, *args, **kwargs)
 
     return wrapper
 
 
-class DefaultAction(BaseModel):
-    type: PolicyActionType
+class PolicyActionBase(BaseModel):
+    type: str
+
+
+class BasicPolicyAction(PolicyActionBase):
+    type: BasicPolicyActionType
 
 
 class InfoTag(BaseModel):
     info_tag: Optional[str] = Field("", serialization_alias="infoTag", validation_alias="infoTag")
 
 
 class PolicyDefinitionId(BaseModel):
@@ -1020,16 +1024,16 @@
 
 class PolicyReference(BaseModel):
     id: UUID
     property: str
 
 
 class DefinitionWithSequencesCommonBase(BaseModel):
-    default_action: Optional[DefaultAction] = Field(
-        default=DefaultAction(type="drop"),
+    default_action: Optional[PolicyActionBase] = Field(
+        default=None,
         serialization_alias="defaultAction",
         validation_alias="defaultAction",
     )
     sequences: Optional[Sequence[PolicyDefinitionSequenceBase]] = None
 
     def _enumerate_sequences(self, from_index: int = 0) -> None:
         """Updates sequence entries with appropriate index.
@@ -1105,24 +1109,7 @@
     master_templates_affected: List[str] = Field(
         default=[], serialization_alias="masterTemplatesAffected", validation_alias="masterTemplatesAffected"
     )
 
 
 class PolicyDefinitionPreview(BaseModel):
     preview: str
-
-
-class PolicyDefinitionEndpoints(Protocol):
-    def create_policy_definition(self, payload: BaseModel) -> PolicyDefinitionId:
-        ...
-
-    def delete_policy_definition(self, id: UUID) -> None:
-        ...
-
-    def edit_policy_definition(self, id: UUID, payload: BaseModel) -> PolicyDefinitionEditResponse:
-        ...
-
-    def get_definitions(self) -> DataSequence[PolicyDefinitionInfo]:
-        ...
-
-    def get_policy_definition(self, id: UUID) -> PolicyDefinitionGetResponse:
-        ...
```

### Comparing `catalystwan-0.33.6/catalystwan/models/policy/policy_list.py` & `catalystwan-0.33.6.dev0/catalystwan/models/policy/list/vpn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,40 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2022 Cisco Systems, Inc. and its affiliates
 
-import datetime
-from typing import List, Optional, Protocol
-from uuid import UUID
+from typing import List, Literal, Set, Tuple
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, field_validator
 
-from catalystwan.models.policy import AnyPolicyList
-from catalystwan.typed_list import DataSequence
+from catalystwan.models.common import IntRangeStr
+from catalystwan.models.policy.policy_list import PolicyListBase, PolicyListId, PolicyListInfo
 
 
-class InfoTag(BaseModel):
-    info_tag: Optional[str] = Field("", alias="infoTag")
+class VPNListEntry(BaseModel):
+    vpn: IntRangeStr = Field(description="0-65530 range or single number")
 
+    @field_validator("vpn")
+    @classmethod
+    def check_vpn_range(cls, vpn: IntRangeStr):
+        for i in vpn:
+            if i is not None:
+                assert 0 <= i <= 65_530
+        return vpn
 
-class PolicyListId(BaseModel):
-    list_id: UUID = Field(alias="listId")
 
+class VPNList(PolicyListBase):
+    type: Literal["vpn"] = "vpn"
+    entries: List[VPNListEntry] = []
 
-class PolicyListInfo(PolicyListId, InfoTag):
-    last_updated: datetime.datetime = Field(alias="lastUpdated")
-    owner: str
-    read_only: bool = Field(alias="readOnly")
-    version: str
-    reference_count: int = Field(alias="referenceCount")
-    references: List
-    is_activated_by_vsmart: Optional[bool] = Field(None, alias="isActivatedByVsmart")
+    def add_vpns(self, vpns: Set[int]):
+        for vpn in vpns:
+            self._add_entry(VPNListEntry(vpn=(vpn, None)))
 
+    def add_vpn_range(self, vpn_range: Tuple[int, int]):
+        self._add_entry(VPNListEntry(vpn=vpn_range))
 
-class PolicyListPreview(BaseModel):
-    preview: str
 
+class VPNListEditPayload(VPNList, PolicyListId):
+    pass
 
-class PolicyListEndpoints(Protocol):
-    def create_policy_list(self, payload: AnyPolicyList) -> PolicyListId:
-        ...
 
-    def delete_policy_list(self, id: UUID) -> None:
-        ...
-
-    def edit_policy_list(self, id: UUID, payload: AnyPolicyList) -> None:
-        ...
-
-    def get_lists_by_id(self, id: UUID) -> PolicyListInfo:
-        ...
-
-    def get_policy_lists(self) -> DataSequence[PolicyListInfo]:
-        ...
+class VPNListInfo(VPNList, PolicyListInfo):
+    pass
```

### Comparing `catalystwan-0.33.6/catalystwan/models/tenant.py` & `catalystwan-0.33.6.dev0/catalystwan/models/tenant.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/response.py` & `catalystwan-0.33.6.dev0/catalystwan/response.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/session.py` & `catalystwan-0.33.6.dev0/catalystwan/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # Copyright 2022 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
 import logging
 from enum import Enum
+from functools import cached_property
 from pathlib import Path
 from time import monotonic, sleep
-from typing import Any, Callable, ClassVar, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Dict, List, Optional, Union
 from urllib.parse import urljoin, urlparse, urlunparse
 
 from packaging.version import Version  # type: ignore
 from requests import PreparedRequest, Request, Response, Session, get, head
 from requests.auth import AuthBase
 from requests.exceptions import ConnectionError, HTTPError, RequestException
 
 from catalystwan import USER_AGENT
-from catalystwan.api.api_container import APIContainer
 from catalystwan.endpoints import APIEndpointClient
 from catalystwan.endpoints.client import AboutInfo, ServerInfo
-from catalystwan.endpoints.endpoints_container import APIEndpointContainter
 from catalystwan.exceptions import (
     DefaultPasswordError,
     ManagerHTTPError,
     ManagerReadyTimeout,
     ManagerRequestException,
     SessionNotCreatedError,
     TenantSubdomainNotFound,
@@ -31,14 +30,18 @@
 from catalystwan.response import ManagerResponse, response_history_debug
 from catalystwan.utils.session_type import SessionType
 from catalystwan.version import NullVersion, parse_api_version
 from catalystwan.vmanage_auth import vManageAuth
 
 JSON = Union[Dict[str, "JSON"], List["JSON"], str, int, float, bool, None]
 
+if TYPE_CHECKING:
+    from catalystwan.api.api_container import APIContainer
+    from catalystwan.endpoints.endpoints_container import APIEndpointContainter
+
 
 class UserMode(str, Enum):
     PROVIDER = "provider"
     TENANT = "tenant"
 
 
 class ViewMode(str, Enum):
@@ -149,15 +152,15 @@
         url: str,
         username: str,
         password: str,
         verify: bool = False,
         port: Optional[int] = None,
         subdomain: Optional[str] = None,
         auth: Optional[AuthBase] = None,
-        validate_responses: bool = True,
+        validate_response: bool = True,
     ):
         self.url = url
         self.port = port
         self.base_url = self.__create_base_url()
         self.username = username
         self.password = password
         self.subdomain = subdomain
@@ -167,22 +170,34 @@
         self.enable_relogin: bool = True
         self.response_trace: Callable[
             [Optional[Response], Union[Request, PreparedRequest, None]], str
         ] = response_history_debug
         super(ManagerSession, self).__init__()
         self.headers.update({"User-Agent": USER_AGENT})
         self.__prepare_session(verify, auth)
-        self.api = APIContainer(self)
-        self.endpoints = APIEndpointContainter(self)
         self._platform_version: str = ""
-        self._api_version: Version
+        self._api_version: Version = NullVersion  # type: ignore
         self._state: ManagerSessionState = ManagerSessionState.OPERATIVE
         self.restart_timeout: int = 1200
         self.polling_requests_timeout: int = 10
-        self._validate_responses = validate_responses
+        self._validate_response = validate_response
+
+    @cached_property
+    def api(self) -> APIContainer:
+        from catalystwan.api.api_container import APIContainer
+
+        self._api = APIContainer(self)
+        return self._api
+
+    @cached_property
+    def endpoints(self) -> APIEndpointContainter:
+        from catalystwan.endpoints.endpoints_container import APIEndpointContainter
+
+        self._endpoints = APIEndpointContainter(self)
+        return self._endpoints
 
     @property
     def state(self) -> ManagerSessionState:
         return self._state
 
     @state.setter
     def state(self, state: ManagerSessionState) -> None:
@@ -425,43 +440,32 @@
             Virtual session token
         """
         url_path = f"/dataservice/tenant/{tenant_id}/vsessionid"
         response = self.post(url_path)
         return response.json()["VSessionId"]
 
     def logout(self) -> Optional[ManagerResponse]:
-        response = None
         if isinstance((version := self.api_version), NullVersion):
             self.logger.warning("Cannot perform logout operation without known api_version.")
-            return response
+            return None
         else:
-            # disable automatic relogin before performing logout request
-            _relogin = self.enable_relogin
-            try:
-                self.enable_relogin = False
-                if version >= Version("20.12"):
-                    response = self.post("/logout")
-                else:
-                    response = self.get("/logout")
-            finally:
-                # restore original setting after performing logout request
-                self.enable_relogin = _relogin
-        return response
+            return self.post("/logout") if version >= Version("20.12") else self.get("/logout")
 
     def close(self) -> None:
         """Closes the ManagerSession.
 
         This method is overrided from requests.Session.
         Firstly it cleans up any resources associated with vManage.
         Then it closes all adapters and as such the session.
 
         Note: It is generally recommended to use the session as a context manager
         using the `with` statement, which ensures that the session is properly
         closed and resources are cleaned up even in case of exceptions.
         """
+        self.enable_relogin = False
         self.logout()
         super().close()
 
     def __prepare_session(self, verify: bool, auth: Optional[AuthBase]) -> None:
         self.auth = auth
         self.verify = verify
 
@@ -479,20 +483,20 @@
         self._api_version = parse_api_version(version)
 
     @property
     def api_version(self) -> Version:
         return self._api_version
 
     @property
-    def validate_responses(self) -> bool:
-        return self._validate_responses
+    def validate_response(self) -> bool:
+        return self._validate_response
 
-    @validate_responses.setter
-    def validate_responses(self, value: bool):
-        self._validate_responses = value
+    @validate_response.setter
+    def validate_response(self, value: bool):
+        self._validate_response = value
 
     def __str__(self) -> str:
         return f"{self.username}@{self.base_url}"
 
     def __repr__(self):
         return (
             f"{self.__class__.__name__}('{self.url}', '{self.username}', '{self.password}', port={self.port}, "
```

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/definitions/banner_1.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/banner_1.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/children.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/children_nested.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/definitions/cisco_bfd.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/definitions/complex_aaa.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/complex_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/definitions/complex_cisco_vpn.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/complex_cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/definitions/default_cisco_system.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/default_cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/definitions/iuo.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/iuo.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/definitions/omp_2.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/omp_2.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/definitions/omp_3.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/definitions/omp_3.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/models/__init__.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/models/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_aaa.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/models/cisco_aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_bfd.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/models/cisco_bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/models/cisco_vpn.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/models/cisco_vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/models/omp_vsmart.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/models/omp_vsmart.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/alias.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/basic/alias.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/basic.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/basic/basic.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/children.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/children_nested.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/schemas/basic/data_path.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/basic/data_path.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/schemas/cedge_aaa.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/cedge_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_banner.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/cisco_banner.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_bfd.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_system.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/schemas/cisco_vpn.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/schemas/omp-vsmart.json` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/schemas/omp-vsmart.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/test_chose_model.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/test_chose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/test_deserialize_model.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/test_deserialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/test_generate_payload.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/test_generate_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/templates/test_serialize_model.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/templates/test_serialize_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         with open(Path(__file__).resolve().parents[0] / Path("schemas") / Path(template.type + ".json")) as f:
             schema = json.load(f)
 
         with open(
             Path(__file__).resolve().parents[0] / Path("definitions") / Path(f"{template.template_name}.json")
         ) as f:
             definition = json.load(f)
-
         # Act
         feature_template_payload = templates_api.generate_feature_template_payload(
             template=template, schema=schema, debug=False
         )
         # Assert
         # self.assertDictEqual
         self.maxDiff = 10000
```

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_admin_tech_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_administration.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_alarms_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_cli_template.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_creation_tools.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_device_action_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_devices_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_endpoints.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Dict, List, Literal, Optional, Union
 from unittest.mock import MagicMock
 from uuid import UUID, uuid4
 
 import pytest  # type: ignore
 from packaging.version import Version  # type: ignore
 from parameterized import parameterized  # type: ignore
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field, model_serializer
 from typing_extensions import Annotated
 
 from catalystwan.endpoints import (
     BASE_PATH,
     JSON,
     APIEndpoints,
     CustomPayloadType,
@@ -25,14 +25,15 @@
     TypeSpecifier,
     delete,
     get,
 )
 from catalystwan.endpoints import logger as endpoints_logger
 from catalystwan.endpoints import post, put, request, versions, view
 from catalystwan.exceptions import APIEndpointError, APIRequestPayloadTypeError, APIVersionError, APIViewError
+from catalystwan.models.common import VersionedField
 from catalystwan.typed_list import DataSequence
 from catalystwan.utils.session_type import ProviderAsTenantView, ProviderView, TenantView
 
 
 class BaseModelExample(BaseModel):
     id: str
     size: int
@@ -870,7 +871,40 @@
 
         AnyBaseModel = Annotated[Union[BaseModel_A, BaseModel_B], Field(discriminator="field")]
 
         class TestAPI(APIEndpoints):
             @request("POST", "/v1/data")
             def create(self, payload: AnyBaseModel) -> None:  # type: ignore [empty-body]
                 ...
+
+    @parameterized.expand(
+        [
+            ("1.3", '{"name":"John"}'),
+            ("1.9", '{"newName":"John"}'),
+        ]
+    )
+    def test_api_version_passed_in_dump_context(self, version, expected_payload_json):
+        # Arrange
+        class Payload(BaseModel):
+            model_config = ConfigDict(populate_by_name=True)
+            name: Annotated[str, VersionedField(versions=">1.6", serialization_alias="newName")]
+
+            @model_serializer(mode="wrap")
+            def serialize(self, handler, info):
+                return VersionedField.dump(self.model_fields, handler(self), info)
+
+        class ExampleAPI(APIEndpoints):
+            @request("POST", "/v1/data")
+            def create(self, payload: Payload) -> None:  # type: ignore [empty-body]
+                ...
+
+        self.session_mock.api_version = Version(version)
+        api = ExampleAPI(self.session_mock)
+        # Act
+        api.create(Payload(name="John"))
+        # Assert
+        self.session_mock.request.assert_called_once_with(
+            "POST",
+            self.base_path + "/v1/data",
+            data=expected_payload_json,
+            headers={"content-type": "application/json"},
+        )
```

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_feature_template_field.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_logs_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_monitoring_server_info.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_monitoring_server_info.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_monitoring_status_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_mtt_aaa_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_omp_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_packet_capture.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_packet_capture.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_partition_manager_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_response.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,23 +151,25 @@
         # Arrange
         self.response_mock.json.return_value = VALIDATE_DATASEQ_TEST_DATA[0]
         vmng_response = ManagerResponse(self.response_mock)
         # Act
         data = vmng_response.dataobj(DataForValidateTest, sourcekey=None, validate=False)
         # Assert
         assert isinstance(data, DataForValidateTest)
+        print(data)
         assert data.important == VALIDATE_DATASEQ_TEST_DATA[0]["important"]
         with self.assertRaises(ValidationError):
             vmng_response.dataobj(DataForValidateTest, sourcekey=None, validate=True)
 
     def test_dataseq_optional_validate(self):
         self.response_mock.json.return_value = VALIDATE_DATASEQ_TEST_DATA
         vmng_response = ManagerResponse(self.response_mock)
         # Act
         dataseq = vmng_response.dataseq(DataForValidateTest, sourcekey=None, validate=False)
         # Assert
         assert isinstance(dataseq, DataSequence)
+        print(dataseq)
         for i, data in enumerate(dataseq):
             assert isinstance(data, DataForValidateTest)
             assert data.important == VALIDATE_DATASEQ_TEST_DATA[i]["important"]
         with self.assertRaises(ValidationError):
             vmng_response.dataseq(DataForValidateTest, sourcekey=None, validate=True)
```

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_session.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_software_action_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_speed_test_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_speed_test_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_task_status_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_templates.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             reachability=Reachability.REACHABLE,
             local_system_ip="192.168.0.1",
             memUsage=1.0,
             connected_vManages=["192.168.0.1"],
             model="vedge-cloud",
             status="normal",
         )
-        sub_tasks_data = SubTaskData.parse_obj(
+        sub_tasks_data = SubTaskData.model_validate(
             {
                 "status": "Success",
                 "statusId": "success",
                 "action": "",
                 "activity": [],
                 "currentActivity": "",
                 "actionConfig": "",
```

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_tenant_backup_restore_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_tenant_management_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_tenant_migration_api.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_typed_list.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_typed_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -361,10 +361,42 @@
         self.assertEqual(output, correct_output)
 
     def test_filter_exception(self):
         # Arrange, Act, Assert
         with self.assertRaises(AttributeError):
             self.data_sequence.filter(does_not="exists")
 
+    def test_find(self):
+        # Arrange
+        expected = self.data_sequence.filter(username="User3").single_or_default()
+        # Act
+        observed = self.data_sequence.find(username="User3")
+
+        # Assert
+        self.assertEqual(observed, expected)
+
+    def test_find_two_attributes(self):
+        # Arrange
+        additional_user = User(username="User1", description="ThisOne")
+        users = copy.deepcopy(self.data_sequence)
+        users.append(additional_user)
+        correct_output = additional_user
+
+        # Act
+        output = users.find(username="User1", description="ThisOne")
+
+        # Assert
+        self.assertEqual(output, correct_output)
+
+    def test_find_wrong_arg(self):
+        # Arrange, Act, Assert
+        with self.assertRaises(AttributeError):
+            self.data_sequence.find(does_not="exists")
+
+    def test_find_no_match(self):
+        # Arrange, Act, Assert
+        with self.assertRaises(InvalidOperationError):
+            self.data_sequence.find(username="NonExistingUser")
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_version.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_version_utils.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/tests/test_vmanage_auth.py` & `catalystwan-0.33.6.dev0/catalystwan/tests/test_vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/typed_list.py` & `catalystwan-0.33.6.dev0/catalystwan/typed_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,7 +255,24 @@
             [T]: The single element of the input sequence.
         """
 
         if len(self.data) < 1:
             raise InvalidOperationError("The input sequence contains no elements.")
 
         return self.data[0]
+
+    def find(self, **kwargs) -> T:
+        """Finds first item in sequence matching values based on attributes.
+        Works similarily as filter but assures single element is returned or raises exception.
+
+        >>> seq = DataSequence(User, [User(username="User1"), User(username="User2")])
+        >>> seq.find(username="User1")
+        User(username='User1', password=None, group=[], locale=None, description=None, resource_group=None)
+
+        Returns:
+            [T]: The single element of the input sequence.
+        """
+        annotations = set(kwargs.keys())
+        result = next(filter(lambda x: all(getattr(x, a) == kwargs[a] for a in annotations), self.data), None)
+        if result is None:
+            raise InvalidOperationError(f"Item matching {kwargs} not found in the input sequence")
+        return result
```

### Comparing `catalystwan-0.33.6/catalystwan/utils/creation_tools.py` & `catalystwan-0.33.6.dev0/catalystwan/utils/creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/utils/dashboard.py` & `catalystwan-0.33.6.dev0/catalystwan/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/utils/device_model.py` & `catalystwan-0.33.6.dev0/catalystwan/utils/device_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/utils/dict.py` & `catalystwan-0.33.6.dev0/catalystwan/utils/dict.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/utils/feature_template/choose_model.py` & `catalystwan-0.33.6.dev0/catalystwan/utils/feature_template/choose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/utils/feature_template/find_template_values.py` & `catalystwan-0.33.6.dev0/catalystwan/utils/feature_template/find_template_values.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         value = template_definition[target_key]
         template_value = template_definition.get(target_key_for_template_value)
 
         field_key = path[-1]
         # TODO: Handle nested DeviceVariable
         if value == "variableName":
             if device_specific_variables is not None:
-                device_specific_variables[field_key] = DeviceVariable(name=template_definition["vipVariableName"])
+                current_nesting = get_nested_dict(device_specific_variables, path[:-1])
+                current_nesting[field_key] = DeviceVariable(name=template_definition["vipVariableName"])
             return template_definition
         if template_value is None:
             return template_definition
 
         if template_definition["vipType"] == "variable":
             if device_specific_variables is not None and template_value:
                 device_specific_variables[field_key] = DeviceVariable(name=template_value)
```

### Comparing `catalystwan-0.33.6/catalystwan/utils/operation_status.py` & `catalystwan-0.33.6.dev0/catalystwan/utils/operation_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/utils/upgrades_helper.py` & `catalystwan-0.33.6.dev0/catalystwan/utils/upgrades_helper.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/version.py` & `catalystwan-0.33.6.dev0/catalystwan/version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/vmanage_auth.py` & `catalystwan-0.33.6.dev0/catalystwan/vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/catalystwan/workflows/tenant_migration.py` & `catalystwan-0.33.6.dev0/catalystwan/workflows/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.6/pyproject.toml` & `catalystwan-0.33.6.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "catalystwan"
-version = "0.33.6"
+version = "0.33.6dev0"
 description = "Cisco Catalyst WAN SDK for Python"
 authors = ["kagorski <kagorski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/cisco-open/cisco-catalyst-wan-sdk"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
@@ -14,15 +14,15 @@
 ciscoconfparse = "1.9.41"
 tenacity = "^8.1.0"
 Jinja2 = "^3.1.2"
 flake8-quotes = "^3.3.1"
 clint = "^0.5.1"
 requests-toolbelt = "^1.0.0"
 packaging = "^23.0"
-pydantic = "^2.5"
+pydantic = "^2.7"
 typing-extensions = "^4.6.1"
 
 [tool.poetry.dev-dependencies]
 parameterized = "^0.8.1"
 pytest = "^7.1.2"
 pytest-mock = "^3.7.0"
 pytest-subtests = "^0.11.0"
```

### Comparing `catalystwan-0.33.6/setup.py` & `catalystwan-0.33.6.dev0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,448 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: catalystwan
+Version: 0.33.6.dev0
+Summary: Cisco Catalyst WAN SDK for Python
+Home-page: https://github.com/cisco-open/cisco-catalyst-wan-sdk
+Author: kagorski
+Author-email: kagorski@cisco.com
+Requires-Python: >=3.8.0,<4.0.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: attrs (>=21.4.0,<22.0.0)
+Requires-Dist: ciscoconfparse (==1.9.41)
+Requires-Dist: clint (>=0.5.1,<0.6.0)
+Requires-Dist: flake8-quotes (>=3.3.1,<4.0.0)
+Requires-Dist: packaging (>=23.0,<24.0)
+Requires-Dist: pydantic (>=2.7,<3.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
+Requires-Dist: tenacity (>=8.1.0,<9.0.0)
+Requires-Dist: typing-extensions (>=4.6.1,<5.0.0)
+Project-URL: Repository, https://github.com/cisco-open/cisco-catalyst-wan-sdk
+Description-Content-Type: text/markdown
 
-packages = \
-['catalystwan',
- 'catalystwan.api',
- 'catalystwan.api.configuration_groups',
- 'catalystwan.api.configuration_groups.parcels',
- 'catalystwan.api.templates',
- 'catalystwan.api.templates.device_template',
- 'catalystwan.api.templates.models',
- 'catalystwan.api.templates.payloads.aaa',
- 'catalystwan.api.templates.payloads.cisco_vpn',
- 'catalystwan.api.templates.payloads.tenant',
- 'catalystwan.endpoints',
- 'catalystwan.endpoints.configuration',
- 'catalystwan.endpoints.configuration.device',
- 'catalystwan.endpoints.configuration.feature_profile.sdwan',
- 'catalystwan.endpoints.configuration.policy',
- 'catalystwan.endpoints.configuration.policy.definition',
- 'catalystwan.endpoints.configuration.policy.list',
- 'catalystwan.endpoints.monitoring',
- 'catalystwan.endpoints.real_time_monitoring',
- 'catalystwan.endpoints.troubleshooting_tools',
- 'catalystwan.integration_tests',
- 'catalystwan.models',
- 'catalystwan.models.configuration',
- 'catalystwan.models.configuration.feature_profile',
- 'catalystwan.models.configuration.feature_profile.sdwan.management',
- 'catalystwan.models.configuration.feature_profile.sdwan.policy_object',
- 'catalystwan.models.configuration.feature_profile.sdwan.policy_object.policy',
- 'catalystwan.models.configuration.feature_profile.sdwan.policy_object.security',
- 'catalystwan.models.configuration.feature_profile.sdwan.service',
- 'catalystwan.models.configuration.feature_profile.sdwan.service.lan',
- 'catalystwan.models.configuration.feature_profile.sdwan.system',
- 'catalystwan.models.configuration.feature_profile.sdwan.transport',
- 'catalystwan.models.misc',
- 'catalystwan.models.monitoring',
- 'catalystwan.models.policy',
- 'catalystwan.models.policy.definitions',
- 'catalystwan.tests',
- 'catalystwan.tests.templates',
- 'catalystwan.tests.templates.models',
- 'catalystwan.utils',
- 'catalystwan.utils.feature_template',
- 'catalystwan.workflows']
-
-package_data = \
-{'': ['*'],
- 'catalystwan.api.templates.payloads.aaa': ['feature/*'],
- 'catalystwan.api.templates.payloads.cisco_vpn': ['feature/*'],
- 'catalystwan.tests.templates': ['definitions/*',
-                                 'definitions/basic/*',
-                                 'schemas/*',
-                                 'schemas/basic/*']}
-
-install_requires = \
-['Jinja2>=3.1.2,<4.0.0',
- 'attrs>=21.4.0,<22.0.0',
- 'ciscoconfparse==1.9.41',
- 'clint>=0.5.1,<0.6.0',
- 'flake8-quotes>=3.3.1,<4.0.0',
- 'packaging>=23.0,<24.0',
- 'pydantic>=2.5,<3.0',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'requests-toolbelt>=1.0.0,<2.0.0',
- 'requests>=2.27.1,<3.0.0',
- 'tenacity>=8.1.0,<9.0.0',
- 'typing-extensions>=4.6.1,<5.0.0']
-
-setup_kwargs = {
-    'name': 'catalystwan',
-    'version': '0.33.6',
-    'description': 'Cisco Catalyst WAN SDK for Python',
-    'long_description': '<p align="center">\n  <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />\n</p>\n\n[![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating simple and parallel automatic requests via official SD-WAN Manager API. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any SD-WAN Manager.\n\n## Important Notice: Early Beta Release\n\nWelcome to the Cisco Catalyst WAN SDK!\n\nWe are thrilled to announce that Cisco Catalyst WAN SDK is now available in early beta. This is an exciting step forward in enabling developers to harness the full potential of Cisco\'s networking solutions.  Please be aware that, as an early beta release, this version of the SDK is still undergoing development and testing. As such, it is provided "as is" and support to address any issues are limited and best effort.\n\n## Not recommend to use in production environments.\nWe encourage developers to explore and test the SDK\'s capabilities, but please exercise caution when using it in production environments.  We are dedicated to improving the Cisco Catalyst WAN SDK and we value your input. Your feedback is crucial to us-it will guide us in refining and enhancing the SDK to better meet your needs.\nTo report any issues, share your insights, or suggest improvements, please visit our Issues page on GitHub or reach out to us through the provided communication channels.\n\nThank you for being a part of our development journey!\n\n## Installation\n```console\npip install catalystwan\n```\n\n## Manager Session\nIn order to execute SDK APIs **ManagerSession** needs to be created. The fastest way to get started is to use `create_manager_session()` method which configures session, performs authentication for given credentials and returns **ManagerSession** instance in operational state. **ManagerSession** provides a collection of supported APIs in `api` instance variable.\nPlease check example below:\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    devices = session.api.devices.get()\n    print(devices)\n```\n**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all functionality from [requests](https://requests.readthedocs.io/en/latest/) library is avaiable to user, it also implements python [contextmanager](https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager) and automatically frees server resources on exit.\n\n<details>\n    <summary> <b>Configure Manager Session before using</b> <i>(click to expand)</i></summary>\n\nIt is possible to configure **ManagerSession** prior sending any request.\n\n```python\nfrom catalystwan.session import ManagerSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\n# configure session using constructor - nothing will be sent to target server yet\nsession = ManagerSession(url=url, username=username, password=password)\n# login and send requests\nsession.login()\nsession.get("/dataservice/device")\nsession.close()\n```\nWhen interacting with the SDWAN Manager API without using a context manager, it\'s important \nto manually execute the `close()` method to release the user session resource.\nEnsure that the `close()` method is called after you have finished using the session to maintain optimal resource management and avoid potential errors.\n\n</details>\n\n<details>\n    <summary> <b>Login as Tenant</b> <i>(click to expand)</i></summary>\n\nTenant domain needs to be provided in url together with Tenant credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "tenant.example.com"\nusername = "tenant_user"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    print(session.session_type)\n```\n\n</details>\n\n<details>\n    <summary> <b>Login as Provider-as-Tenant</b> <i>(click to expand)</i></summary>\n\nTenant `subdomain` needs to be provided as additional argument together with Provider credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "provider"\npassword = "password123"\nsubdomain = "tenant.example.com"\n\nwith create_manager_session(url=url, username=username, password=password, subdomain=subdomain) as session:\n    print(session.session_type)\n```\n\n</details>\n\n\n\n## API usage examples\nAll examples below assumes `session` variable contains logged-in [Manager Session](#Manager-Session) instance.\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\ncontrollers = session.endpoints.configuration_device_inventory.get_device_details(\'controllers\')\nvsmarts = controllers.filter(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices=vsmarts, image=image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\nTo get all alarms:\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn = 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get all critical alarms from past `n` hours:\n\n```python\nfrom catalystwan.utils.alarm_status import Severity\nn = 48\ncritical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)\n```\n\n</details>\n\n<details>\n    <summary> <b>Users</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create user\nfrom catalystwan.endpoints.administration_user_and_group import User\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n# Update user data\nnew_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")\nsession.api.users.update(new_user_update)\n\n# Update user password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n# Reset user\nsession.api.users.reset("new_user")\n\n# Delete user\nsession.api.users.delete("new_user")\n\n# Get current user authentication type and role\nsession.api.users.get_auth_type()\nsession.api.users.get_role()\n```\n\n</details>\n\n<details>\n    <summary> <b>User Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all user groups\nsession.api.user_groups.get()\n\n# Create user group\ngroup = UserGroup("new_user_group", [])\ngroup.enable_read({"Audit Log", "Alarms"})\ngroup.enable_read_and_write({"Device Inventory"})\nsession.api.user_groups.create(group)\n\n# Update user group\ngroup.disable({"Alarms"})\nsession.api.user_groups.update(group)\n\n# Delete user group\nsession.api.user_groups.delete(group.group_name)\n```\n\n</details>\n\n</details>\n\n<details>\n    <summary> <b>Sessions</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all active sessions\nactive_sessions = session.api.sessions.get()\n\n# Invalidate sessions for given user\nnew_user_sessions = active_sessions.filter(raw_username="new_user")\nsession.api.sessions.invalidate(new_user_sessions)\n```\n\n</details>\n\n<details>\n    <summary> <b>Resource Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# get resource groups\nsession.api.resource_groups.get()\n\n# create resource group\nnew_resource_group = ResourceGroup(\n    name="new_resource_group",\n    desc="Custom Resource Group #1",\n    siteIds=[]\n)\nsession.api.resource_groups.create(new_resource_group)\n\n# update resource group\nresource_group = session.api.resource_groups.get().filter(name="new_resource_group").single_or_default()\nupdated_resource_group = ResourceGroupUpdateRequest(\n    id=resource_group.id,\n    name=resource_group.name,\n    desc="Custom Resource Group #1 with updated description and site ids",\n    siteIds=[200]\n)\n\n# switch to resource group view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete resource group\nsession.api.resource_groups.delete(resource_group.id)\n```\n\n</details>\n\n<details>\n    <summary> <b>Tenant management</b> <i>(click to expand)</i></summary>\n\n```python\napi = session.api.tenant_management\n# create tenants\ntenants = [\n    Tenant(\n        name="tenant1",\n        org_name="CiscoDevNet",\n        subdomain="alpha.bravo.net",\n        desc="This is tenant for unit tests",\n        edge_connector_enable=True,\n        edge_connector_system_ip="172.16.255.81",\n        edge_connector_tunnel_interface_name="GigabitEthernet1",\n        wan_edge_forecast=1,\n    )\n]\ncreate_task = api.create(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data = api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id = tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid = api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete([tenant_id])\ndelete_task.wait_for_completed()\n# others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses()\napi.get_vsmart_mapping()\n```\n</details>\n\n<details>\n    <summary> <b>Tenant migration</b> <i>(click to expand)</i></summary>\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import create_manager_session\nfrom catalystwan.models.tenant import TenantExport\nfrom catalystwan.workflows.tenant_migration import migration_workflow\n\ntenant = TenantExport(\n    name="mango",\n    desc="Mango tenant description",\n    org_name="Provider Org-Mango Inc",\n    subdomain="mango.fruits.com",\n    wan_edge_forecast=100,\n    migration_key="MangoTenantMigrationKey",   # only for SDWAN Manager >= 20.13\n    is_destination_overlay_mt=True,            # only for SDWAN Manager >= 20.13\n)\n\nwith create_manager_session(url="10.0.1.15", username="st-admin", password="") as origin_session, \\\n     create_manager_session(url="10.9.0.16", username="mt-provider-admin", password="") as target_session:\n    migration_workflow(\n        origin_session=origin_session,\n        target_session=target_session,\n        workdir=Path("workdir"),\n        tenant=tenant,\n        validator="10.9.12.26"\n    )\n```\n\n`migration_workflow` performs multi-step migration procedure according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)\n\n\nSince 20.13 also MT to ST is supported (just provide suitable origin/target sessions, and `is_destination_overlay_mt` parameter)\n\n\nEach step of the `migration_workflow` procedure can be executed independently using api methods: `export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`\n\n```python\norigin_api = origin_session.api.tenant_migration_api\ntarget_api = target_session.api.tenant_migration_api\ntenant_file = Path("~/tenant.tar.gz")\ntoken_file = Path("~/tenant-token.txt")\n# export\nexport_task = origin_api.export_tenant(tenant=tenant)\nremote_filename = export_task.wait_for_file()\n# download\norigin_api.download(export_path, remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path, tenant.migration_key)\nimport_task.wait_for_completed()\n# get token\nmigration_id = import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token(migration_id, token_path)\n# migrate network\nmigrate_task = origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed()\n```\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n    session.api.users.delete("bogus-user-name")\nexcept ManagerHTTPError as error:\n    # Process an error.\n    print(error.response.status_code)\n    print(error.info.code)\n    print(error.info.message)\n    print(error.info.details)\n\n```\n\n## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on catalystwan@cisco.com.\n',
-    'author': 'kagorski',
-    'author_email': 'kagorski@cisco.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/cisco-open/cisco-catalyst-wan-sdk',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8.0,<4.0.0',
-}
+<p align="center">
+  <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />
+</p>
 
+[![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)
+
+Cisco Catalyst WAN SDK is a package for creating simple and parallel automatic requests via official SD-WAN Manager API. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any SD-WAN Manager.
+
+## Important Notice: Early Beta Release
+
+Welcome to the Cisco Catalyst WAN SDK!
+
+We are thrilled to announce that Cisco Catalyst WAN SDK is now available in early beta. This is an exciting step forward in enabling developers to harness the full potential of Cisco's networking solutions.  Please be aware that, as an early beta release, this version of the SDK is still undergoing development and testing. As such, it is provided "as is" and support to address any issues are limited and best effort.
+
+## Not recommend to use in production environments.
+We encourage developers to explore and test the SDK's capabilities, but please exercise caution when using it in production environments.  We are dedicated to improving the Cisco Catalyst WAN SDK and we value your input. Your feedback is crucial to us-it will guide us in refining and enhancing the SDK to better meet your needs.
+To report any issues, share your insights, or suggest improvements, please visit our Issues page on GitHub or reach out to us through the provided communication channels.
+
+Thank you for being a part of our development journey!
+
+## Installation
+```console
+pip install catalystwan
+```
+
+## Manager Session
+In order to execute SDK APIs **ManagerSession** needs to be created. The fastest way to get started is to use `create_manager_session()` method which configures session, performs authentication for given credentials and returns **ManagerSession** instance in operational state. **ManagerSession** provides a collection of supported APIs in `api` instance variable.
+Please check example below:
+
+```python
+from catalystwan.session import create_manager_session
+
+url = "example.com"
+username = "admin"
+password = "password123"
+
+with create_manager_session(url=url, username=username, password=password) as session:
+    devices = session.api.devices.get()
+    print(devices)
+```
+**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all functionality from [requests](https://requests.readthedocs.io/en/latest/) library is avaiable to user, it also implements python [contextmanager](https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager) and automatically frees server resources on exit.
+
+<details>
+    <summary> <b>Configure Manager Session before using</b> <i>(click to expand)</i></summary>
+
+It is possible to configure **ManagerSession** prior sending any request.
+
+```python
+from catalystwan.session import ManagerSession
+
+url = "example.com"
+username = "admin"
+password = "password123"
+
+# configure session using constructor - nothing will be sent to target server yet
+session = ManagerSession(url=url, username=username, password=password)
+# login and send requests
+session.login()
+session.get("/dataservice/device")
+session.close()
+```
+When interacting with the SDWAN Manager API without using a context manager, it's important 
+to manually execute the `close()` method to release the user session resource.
+Ensure that the `close()` method is called after you have finished using the session to maintain optimal resource management and avoid potential errors.
+
+</details>
+
+<details>
+    <summary> <b>Login as Tenant</b> <i>(click to expand)</i></summary>
+
+Tenant domain needs to be provided in url together with Tenant credentials.
+
+```python
+from catalystwan.session import create_manager_session
+
+url = "tenant.example.com"
+username = "tenant_user"
+password = "password123"
+
+with create_manager_session(url=url, username=username, password=password) as session:
+    print(session.session_type)
+```
+
+</details>
+
+<details>
+    <summary> <b>Login as Provider-as-Tenant</b> <i>(click to expand)</i></summary>
+
+Tenant `subdomain` needs to be provided as additional argument together with Provider credentials.
+
+```python
+from catalystwan.session import create_manager_session
+
+url = "example.com"
+username = "provider"
+password = "password123"
+subdomain = "tenant.example.com"
+
+with create_manager_session(url=url, username=username, password=password, subdomain=subdomain) as session:
+    print(session.session_type)
+```
+
+</details>
+
+
+
+## API usage examples
+All examples below assumes `session` variable contains logged-in [Manager Session](#Manager-Session) instance.
+
+<details>
+    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>
+
+```python
+devices = session.api.devices.get()
+```
+
+</details>
+
+<details>
+    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>
+
+```Python
+admin_tech_file = session.api.admin_tech.generate("172.16.255.11")
+session.api.admin_tech.download(admin_tech_file)
+session.api.admin_tech.delete(admin_tech_file)
+```
+</details>
+
+<details>
+    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>
+
+```python
+devices = session.api.devices.get()
+speedtest = session.api.speedtest.speedtest(devices[0], devices[1])
+```
+
+</details>
+
+<details>
+    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>
+
+```python
+# Prepare devices list
+controllers = session.endpoints.configuration_device_inventory.get_device_details('controllers')
+vsmarts = controllers.filter(personality=Personality.VSMART)
+image = "viptela-20.7.2-x86_64.tar.gz"
+
+# Upload image
+session.api.repository.upload_image(image)
+
+# Install software
+
+install_task = session.api.software.install(devices=vsmarts, image=image)
+
+# Check action status
+install_task.wait_for_completed()
+```
+
+</details>
+
+<details>
+    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>
+To get all alarms:
+
+```python
+alarms = session.api.alarms.get()
+```
+
+To get all not viewed alarms:
+
+```python
+not_viewed_alarms = session.api.alarms.get().filter(viewed=False)
+```
+
+To get all alarms from past `n` hours:
+
+```python
+n = 24
+alarms_from_n_hours = session.api.alarms.get(from_time=n)
+```
+
+To get all critical alarms from past `n` hours:
+
+```python
+n = 48
+critical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)
+```
+
+</details>
+
+<details>
+    <summary> <b>Users</b> <i>(click to expand)</i></summary>
+
+```python
+# Get all users
+session.api.users.get()
+
+# Create user
+new_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")
+session.api.users.create(new_user)
+
+# Update user data
+new_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")
+session.api.users.update(new_user_update)
+
+# Update user password
+session.api.users.update_password("new_user", "n3W-P4s$w0rd")
+
+# Reset user
+session.api.users.reset("new_user")
+
+# Delete user
+session.api.users.delete("new_user")
+
+# Get current user authentication type and role
+session.api.users.get_auth_type()
+session.api.users.get_role()
+```
+
+</details>
+
+<details>
+    <summary> <b>User Groups</b> <i>(click to expand)</i></summary>
+
+```python
+# Get all user groups
+session.api.user_groups.get()
+
+# Create user group
+group = UserGroup("new_user_group", [])
+group.enable_read({"Audit Log", "Alarms"})
+group.enable_read_and_write({"Device Inventory"})
+session.api.user_groups.create(group)
+
+# Update user group
+group.disable({"Alarms"})
+session.api.user_groups.update(group)
+
+# Delete user group
+session.api.user_groups.delete(group.group_name)
+```
+
+</details>
+
+</details>
+
+<details>
+    <summary> <b>Sessions</b> <i>(click to expand)</i></summary>
+
+```python
+# Get all active sessions
+active_sessions = session.api.sessions.get()
+
+# Invalidate sessions for given user
+new_user_sessions = active_sessions.filter(raw_username="new_user")
+session.api.sessions.invalidate(new_user_sessions)
+```
+
+</details>
+
+<details>
+    <summary> <b>Resource Groups</b> <i>(click to expand)</i></summary>
+
+```python
+# get resource groups
+session.api.resource_groups.get()
+
+# create resource group
+new_resource_group = ResourceGroup(
+    name="new_resource_group",
+    desc="Custom Resource Group #1",
+    siteIds=[]
+)
+session.api.resource_groups.create(new_resource_group)
+
+# update resource group
+resource_group = session.api.resource_groups.get().filter(name="new_resource_group").single_or_default()
+updated_resource_group = ResourceGroupUpdateRequest(
+    id=resource_group.id,
+    name=resource_group.name,
+    desc="Custom Resource Group #1 with updated description and site ids",
+    siteIds=[200]
+)
+
+# switch to resource group view
+session.api.resource_groups.switch("new_resource_group")
+
+# delete resource group
+session.api.resource_groups.delete(resource_group.id)
+```
+
+</details>
+
+<details>
+    <summary> <b>Tenant management</b> <i>(click to expand)</i></summary>
+
+```python
+api = session.api.tenant_management
+# create tenants
+tenants = [
+    Tenant(
+        name="tenant1",
+        org_name="CiscoDevNet",
+        subdomain="alpha.bravo.net",
+        desc="This is tenant for unit tests",
+        edge_connector_enable=True,
+        edge_connector_system_ip="172.16.255.81",
+        edge_connector_tunnel_interface_name="GigabitEthernet1",
+        wan_edge_forecast=1,
+    )
+]
+create_task = api.create(tenants)
+create_task.wait_for_completed()
+# list all tenants
+tenants_data = api.get_all()
+# pick tenant from list by name
+tenant = tenants_data.filter(name="tenant1").single_or_default()
+# get selected tenant id
+tenant_id = tenant.tenant_id
+# get vsession id of selected tenant
+vsessionid = api.vsession_id(tenant_id)
+# delete tenant by ids
+delete_task = api.delete([tenant_id])
+delete_task.wait_for_completed()
+# others
+api.get_hosting_capacity_on_vsmarts()
+api.get_statuses()
+api.get_vsmart_mapping()
+```
+</details>
+
+<details>
+    <summary> <b>Tenant migration</b> <i>(click to expand)</i></summary>
+
+```python
+from pathlib import Path
+from catalystwan.session import create_manager_session
+from catalystwan.models.tenant import TenantExport
+from catalystwan.workflows.tenant_migration import migration_workflow
+
+tenant = TenantExport(
+    name="mango",
+    desc="Mango tenant description",
+    org_name="Provider Org-Mango Inc",
+    subdomain="mango.fruits.com",
+    wan_edge_forecast=100,
+    migration_key="MangoTenantMigrationKey",   # only for SDWAN Manager >= 20.13
+    is_destination_overlay_mt=True,            # only for SDWAN Manager >= 20.13
+)
+
+with create_manager_session(url="10.0.1.15", username="st-admin", password="") as origin_session, \
+     create_manager_session(url="10.9.0.16", username="mt-provider-admin", password="") as target_session:
+    migration_workflow(
+        origin_session=origin_session,
+        target_session=target_session,
+        workdir=Path("workdir"),
+        tenant=tenant,
+        validator="10.9.12.26"
+    )
+```
+
+`migration_workflow` performs multi-step migration procedure according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)
+
+
+Since 20.13 also MT to ST is supported (just provide suitable origin/target sessions, and `is_destination_overlay_mt` parameter)
+
+
+Each step of the `migration_workflow` procedure can be executed independently using api methods: `export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`
+
+```python
+origin_api = origin_session.api.tenant_migration_api
+target_api = target_session.api.tenant_migration_api
+tenant_file = Path("~/tenant.tar.gz")
+token_file = Path("~/tenant-token.txt")
+# export
+export_task = origin_api.export_tenant(tenant=tenant)
+remote_filename = export_task.wait_for_file()
+# download
+origin_api.download(export_path, remote_filename)
+# import
+import_task = target_api.import_tenant(export_path, tenant.migration_key)
+import_task.wait_for_completed()
+# get token
+migration_id = import_task.import_info.migration_token_query_params.migration_id
+target_api.store_token(migration_id, token_path)
+# migrate network
+migrate_task = origin_api.migrate_network(token_path)
+migrate_task.wait_for_completed()
+```
+</details>
+
+### Note:
+To remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):
+```Python
+import urllib3
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+```
+
+## Catching Exceptions
+```python
+try:
+    session.api.users.delete("bogus-user-name")
+except ManagerHTTPError as error:
+    # Process an error.
+    print(error.response.status_code)
+    print(error.info.code)
+    print(error.info.message)
+    print(error.info.details)
+
+```
+
+## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)
+
+
+## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)
+
+## Seeking support
+
+You can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on catalystwan@cisco.com.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,233 +1,183 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['catalystwan', 'catalystwan.api', 'catalystwan.api.configuration_groups',
-'catalystwan.api.configuration_groups.parcels', 'catalystwan.api.templates',
-'catalystwan.api.templates.device_template',
-'catalystwan.api.templates.models', 'catalystwan.api.templates.payloads.aaa',
-'catalystwan.api.templates.payloads.cisco_vpn',
-'catalystwan.api.templates.payloads.tenant', 'catalystwan.endpoints',
-'catalystwan.endpoints.configuration',
-'catalystwan.endpoints.configuration.device',
-'catalystwan.endpoints.configuration.feature_profile.sdwan',
-'catalystwan.endpoints.configuration.policy',
-'catalystwan.endpoints.configuration.policy.definition',
-'catalystwan.endpoints.configuration.policy.list',
-'catalystwan.endpoints.monitoring',
-'catalystwan.endpoints.real_time_monitoring',
-'catalystwan.endpoints.troubleshooting_tools', 'catalystwan.integration_tests',
-'catalystwan.models', 'catalystwan.models.configuration',
-'catalystwan.models.configuration.feature_profile',
-'catalystwan.models.configuration.feature_profile.sdwan.management',
-'catalystwan.models.configuration.feature_profile.sdwan.policy_object',
-'catalystwan.models.configuration.feature_profile.sdwan.policy_object.policy',
-'catalystwan.models.configuration.feature_profile.sdwan.policy_object.security',
-'catalystwan.models.configuration.feature_profile.sdwan.service',
-'catalystwan.models.configuration.feature_profile.sdwan.service.lan',
-'catalystwan.models.configuration.feature_profile.sdwan.system',
-'catalystwan.models.configuration.feature_profile.sdwan.transport',
-'catalystwan.models.misc', 'catalystwan.models.monitoring',
-'catalystwan.models.policy', 'catalystwan.models.policy.definitions',
-'catalystwan.tests', 'catalystwan.tests.templates',
-'catalystwan.tests.templates.models', 'catalystwan.utils',
-'catalystwan.utils.feature_template', 'catalystwan.workflows'] package_data = \
-{'': ['*'], 'catalystwan.api.templates.payloads.aaa': ['feature/*'],
-'catalystwan.api.templates.payloads.cisco_vpn': ['feature/*'],
-'catalystwan.tests.templates': ['definitions/*', 'definitions/basic/*',
-'schemas/*', 'schemas/basic/*']} install_requires = \ ['Jinja2>=3.1.2,<4.0.0',
-'attrs>=21.4.0,<22.0.0', 'ciscoconfparse==1.9.41', 'clint>=0.5.1,<0.6.0',
-'flake8-quotes>=3.3.1,<4.0.0', 'packaging>=23.0,<24.0', 'pydantic>=2.5,<3.0',
-'python-dateutil>=2.8.2,<3.0.0', 'requests-toolbelt>=1.0.0,<2.0.0',
-'requests>=2.27.1,<3.0.0', 'tenacity>=8.1.0,<9.0.0', 'typing-
-extensions>=4.6.1,<5.0.0'] setup_kwargs = { 'name': 'catalystwan', 'version':
-'0.33.6', 'description': 'Cisco Catalyst WAN SDK for Python',
-'long_description': '
-                      \n _[_C_i_s_c_o_ _C_a_t_a_l_y_s_t_ _W_A_N_ _S_D_K_ _L_o_g_o_]_\_n
-\n\n[![Python-Supported](https://img.shields.io/static/
+Metadata-Version: 2.1 Name: catalystwan Version: 0.33.6.dev0 Summary: Cisco
+Catalyst WAN SDK for Python Home-page: https://github.com/cisco-open/cisco-
+catalyst-wan-sdk Author: kagorski Author-email: kagorski@cisco.com Requires-
+Python: >=3.8.0,<4.0.0 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Jinja2
+(>=3.1.2,<4.0.0) Requires-Dist: attrs (>=21.4.0,<22.0.0) Requires-Dist:
+ciscoconfparse (==1.9.41) Requires-Dist: clint (>=0.5.1,<0.6.0) Requires-Dist:
+flake8-quotes (>=3.3.1,<4.0.0) Requires-Dist: packaging (>=23.0,<24.0)
+Requires-Dist: pydantic (>=2.7,<3.0) Requires-Dist: python-dateutil
+(>=2.8.2,<3.0.0) Requires-Dist: requests (>=2.27.1,<3.0.0) Requires-Dist:
+requests-toolbelt (>=1.0.0,<2.0.0) Requires-Dist: tenacity (>=8.1.0,<9.0.0)
+Requires-Dist: typing-extensions (>=4.6.1,<5.0.0) Project-URL: Repository,
+https://github.com/cisco-open/cisco-catalyst-wan-sdk Description-Content-Type:
+text/markdown
+                         _[_C_i_s_c_o_ _C_a_t_a_l_y_s_t_ _W_A_N_ _S_D_K_ _L_o_g_o_]
+[![Python-Supported](https://img.shields.io/static/
 v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)]
-(https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating
+(https://www.python.org/) Cisco Catalyst WAN SDK is a package for creating
 simple and parallel automatic requests via official SD-WAN Manager API. It is
 intended to serve as a multiple session handler (provider, provider as a
 tenant, tenant). The library is not dependent on environment which is being run
-in, you just need a connection to any SD-WAN Manager.\n\n## Important Notice:
-Early Beta Release\n\nWelcome to the Cisco Catalyst WAN SDK!\n\nWe are thrilled
-to announce that Cisco Catalyst WAN SDK is now available in early beta. This is
-an exciting step forward in enabling developers to harness the full potential
-of Cisco\'s networking solutions. Please be aware that, as an early beta
-release, this version of the SDK is still undergoing development and testing.
-As such, it is provided "as is" and support to address any issues are limited
-and best effort.\n\n## Not recommend to use in production environments.\nWe
-encourage developers to explore and test the SDK\'s capabilities, but please
-exercise caution when using it in production environments. We are dedicated to
-improving the Cisco Catalyst WAN SDK and we value your input. Your feedback is
-crucial to us-it will guide us in refining and enhancing the SDK to better meet
-your needs.\nTo report any issues, share your insights, or suggest
-improvements, please visit our Issues page on GitHub or reach out to us through
-the provided communication channels.\n\nThank you for being a part of our
-development journey!\n\n## Installation\n```console\npip install
-catalystwan\n```\n\n## Manager Session\nIn order to execute SDK APIs
-**ManagerSession** needs to be created. The fastest way to get started is to
-use `create_manager_session()` method which configures session, performs
-authentication for given credentials and returns **ManagerSession** instance in
-operational state. **ManagerSession** provides a collection of supported APIs
-in `api` instance variable.\nPlease check example below:\n\n```python\nfrom
-catalystwan.session import create_manager_session\n\nurl =
-"example.com"\nusername = "admin"\npassword = "password123"\n\nwith
+in, you just need a connection to any SD-WAN Manager. ## Important Notice:
+Early Beta Release Welcome to the Cisco Catalyst WAN SDK! We are thrilled to
+announce that Cisco Catalyst WAN SDK is now available in early beta. This is an
+exciting step forward in enabling developers to harness the full potential of
+Cisco's networking solutions. Please be aware that, as an early beta release,
+this version of the SDK is still undergoing development and testing. As such,
+it is provided "as is" and support to address any issues are limited and best
+effort. ## Not recommend to use in production environments. We encourage
+developers to explore and test the SDK's capabilities, but please exercise
+caution when using it in production environments. We are dedicated to improving
+the Cisco Catalyst WAN SDK and we value your input. Your feedback is crucial to
+us-it will guide us in refining and enhancing the SDK to better meet your
+needs. To report any issues, share your insights, or suggest improvements,
+please visit our Issues page on GitHub or reach out to us through the provided
+communication channels. Thank you for being a part of our development journey!
+## Installation ```console pip install catalystwan ``` ## Manager Session In
+order to execute SDK APIs **ManagerSession** needs to be created. The fastest
+way to get started is to use `create_manager_session()` method which configures
+session, performs authentication for given credentials and returns
+**ManagerSession** instance in operational state. **ManagerSession** provides a
+collection of supported APIs in `api` instance variable. Please check example
+below: ```python from catalystwan.session import create_manager_session url =
+"example.com" username = "admin" password = "password123" with
 create_manager_session(url=url, username=username, password=password) as
-session:\n devices = session.api.devices.get()\n print
-(devices)\n```\n**ManagerSession** extends [requests.Session](https://
-requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all
-functionality from [requests](https://requests.readthedocs.io/en/latest/
-) library is avaiable to user, it also implements python [contextmanager]
-(https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager)
-and automatically frees server resources on exit.\n\n\n CCoonnffiigguurree MMaannaaggeerr
-SSeessssiioonn bbeeffoorree uussiinngg (click to expand)\n\nIt is possible to configure
-**ManagerSession** prior sending any request.\n\n```python\nfrom
-catalystwan.session import ManagerSession\n\nurl = "example.com"\nusername =
-"admin"\npassword = "password123"\n\n# configure session using constructor -
-nothing will be sent to target server yet\nsession = ManagerSession(url=url,
-username=username, password=password)\n# login and send requests\nsession.login
-()\nsession.get("/dataservice/device")\nsession.close()\n```\nWhen interacting
-with the SDWAN Manager API without using a context manager, it\'s important
-\nto manually execute the `close()` method to release the user session
-resource.\nEnsure that the `close()` method is called after you have finished
-using the session to maintain optimal resource management and avoid potential
-errors.\n\n\n\n\n LLooggiinn aass TTeennaanntt (click to expand)\n\nTenant domain needs to
-be provided in url together with Tenant credentials.\n\n```python\nfrom
-catalystwan.session import create_manager_session\n\nurl =
-"tenant.example.com"\nusername = "tenant_user"\npassword =
-"password123"\n\nwith create_manager_session(url=url, username=username,
-password=password) as session:\n print(session.session_type)\n```\n\n\n\n\n
-LLooggiinn aass PPrroovviiddeerr--aass--TTeennaanntt (click to expand)\n\nTenant `subdomain` needs to be
-provided as additional argument together with Provider
-credentials.\n\n```python\nfrom catalystwan.session import
-create_manager_session\n\nurl = "example.com"\nusername = "provider"\npassword
-= "password123"\nsubdomain = "tenant.example.com"\n\nwith
-create_manager_session(url=url, username=username, password=password,
-subdomain=subdomain) as session:\n print
-(session.session_type)\n```\n\n\n\n\n\n## API usage examples\nAll examples
-below assumes `session` variable contains logged-in [Manager Session](#Manager-
-Session) instance.\n\n\n GGeett ddeevviicceess (click to expand)\n\n```python\ndevices =
-session.api.devices.get()\n```\n\n\n\n\n AAddmmiinn TTeecchh (click to
-expand)\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate
-("172.16.255.11")\nsession.api.admin_tech.download
-(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n\n\n\n
-SSppeeeedd tteesstt (click to expand)\n\n```python\ndevices = session.api.devices.get
-()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices
-[1])\n```\n\n\n\n\n UUppggrraaddee ddeevviiccee (click to expand)\n\n```python\n# Prepare
-devices list\ncontrollers =
+session: devices = session.api.devices.get() print(devices) ```
+**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/
+en/latest/user/advanced/#session-objects) so all functionality from [requests]
+(https://requests.readthedocs.io/en/latest/) library is avaiable to user, it
+also implements python [contextmanager](https://docs.python.org/3.8/library/
+contextlib.html#contextlib.contextmanager) and automatically frees server
+resources on exit. CCoonnffiigguurree MMaannaaggeerr SSeessssiioonn bbeeffoorree uussiinngg (click to expand) It
+is possible to configure **ManagerSession** prior sending any request.
+```python from catalystwan.session import ManagerSession url = "example.com"
+username = "admin" password = "password123" # configure session using
+constructor - nothing will be sent to target server yet session =
+ManagerSession(url=url, username=username, password=password) # login and send
+requests session.login() session.get("/dataservice/device") session.close() ```
+When interacting with the SDWAN Manager API without using a context manager,
+it's important to manually execute the `close()` method to release the user
+session resource. Ensure that the `close()` method is called after you have
+finished using the session to maintain optimal resource management and avoid
+potential errors. LLooggiinn aass TTeennaanntt (click to expand) Tenant domain needs to be
+provided in url together with Tenant credentials. ```python from
+catalystwan.session import create_manager_session url = "tenant.example.com"
+username = "tenant_user" password = "password123" with create_manager_session
+(url=url, username=username, password=password) as session: print
+(session.session_type) ``` LLooggiinn aass PPrroovviiddeerr--aass--TTeennaanntt (click to expand) Tenant
+`subdomain` needs to be provided as additional argument together with Provider
+credentials. ```python from catalystwan.session import create_manager_session
+url = "example.com" username = "provider" password = "password123" subdomain =
+"tenant.example.com" with create_manager_session(url=url, username=username,
+password=password, subdomain=subdomain) as session: print(session.session_type)
+``` ## API usage examples All examples below assumes `session` variable
+contains logged-in [Manager Session](#Manager-Session) instance. GGeett ddeevviicceess
+(click to expand) ```python devices = session.api.devices.get() ``` AAddmmiinn TTeecchh
+(click to expand) ```Python admin_tech_file = session.api.admin_tech.generate
+("172.16.255.11") session.api.admin_tech.download(admin_tech_file)
+session.api.admin_tech.delete(admin_tech_file) ``` SSppeeeedd tteesstt (click to expand)
+```python devices = session.api.devices.get() speedtest =
+session.api.speedtest.speedtest(devices[0], devices[1]) ``` UUppggrraaddee ddeevviiccee
+(click to expand) ```python # Prepare devices list controllers =
 session.endpoints.configuration_device_inventory.get_device_details
-(\'controllers\')\nvsmarts = controllers.filter
-(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n#
-Upload image\nsession.api.repository.upload_image(image)\n\n# Install
-software\n\ninstall_task = session.api.software.install(devices=vsmarts,
-image=image)\n\n# Check action status\ninstall_task.wait_for_completed
-()\n```\n\n\n\n\n GGeett aallaarrmmss (click to expand)\nTo get all alarms:
-\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed
-alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter
-(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn =
-24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get
-all critical alarms from past `n` hours:\n\n```python\nfrom
-catalystwan.utils.alarm_status import Severity\nn = 48\ncritical_alarms =
-session.api.alarms.get(from_time=n).filter
-(severity=Severity.CRITICAL)\n```\n\n\n\n\n UUsseerrss (click to
-expand)\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create
-user\nfrom catalystwan.endpoints.administration_user_and_group import
-User\nnew_user = User(username="new_user", password="new_user", group=
-["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n#
-Update user data\nnew_user_update = UserUpdateRequest(username="new_user",
+('controllers') vsmarts = controllers.filter(personality=Personality.VSMART)
+image = "viptela-20.7.2-x86_64.tar.gz" # Upload image
+session.api.repository.upload_image(image) # Install software install_task =
+session.api.software.install(devices=vsmarts, image=image) # Check action
+status install_task.wait_for_completed() ``` GGeett aallaarrmmss (click to expand) To
+get all alarms: ```python alarms = session.api.alarms.get() ``` To get all not
+viewed alarms: ```python not_viewed_alarms = session.api.alarms.get().filter
+(viewed=False) ``` To get all alarms from past `n` hours: ```python n = 24
+alarms_from_n_hours = session.api.alarms.get(from_time=n) ``` To get all
+critical alarms from past `n` hours: ```python n = 48 critical_alarms =
+session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL) ```
+UUsseerrss (click to expand) ```python # Get all users session.api.users.get() #
+Create user new_user = User(username="new_user", password="new_user", group=
+["netadmin"], description="new user") session.api.users.create(new_user) #
+Update user data new_user_update = UserUpdateRequest(username="new_user",
 group=["netadmin", "netops"], locale="en_US", description="updated-new_user-
-description")\nsession.api.users.update(new_user_update)\n\n# Update user
-password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n#
-Reset user\nsession.api.users.reset("new_user")\n\n# Delete
-user\nsession.api.users.delete("new_user")\n\n# Get current user authentication
-type and role\nsession.api.users.get_auth_type()\nsession.api.users.get_role
-()\n```\n\n\n\n\n UUsseerr GGrroouuppss (click to expand)\n\n```python\n# Get all user
-groups\nsession.api.user_groups.get()\n\n# Create user group\ngroup = UserGroup
-("new_user_group", [])\ngroup.enable_read({"Audit Log",
-"Alarms"})\ngroup.enable_read_and_write({"Device
-Inventory"})\nsession.api.user_groups.create(group)\n\n# Update user
-group\ngroup.disable({"Alarms"})\nsession.api.user_groups.update(group)\n\n#
-Delete user group\nsession.api.user_groups.delete
-(group.group_name)\n```\n\n\n\n\n\n\n SSeessssiioonnss (click to
-expand)\n\n```python\n# Get all active sessions\nactive_sessions =
-session.api.sessions.get()\n\n# Invalidate sessions for given
-user\nnew_user_sessions = active_sessions.filter
-(raw_username="new_user")\nsession.api.sessions.invalidate
-(new_user_sessions)\n```\n\n\n\n\n RReessoouurrccee GGrroouuppss (click to
-expand)\n\n```python\n# get resource groups\nsession.api.resource_groups.get
-()\n\n# create resource group\nnew_resource_group = ResourceGroup(\n
-name="new_resource_group",\n desc="Custom Resource Group #1",\n siteIds=
-[]\n)\nsession.api.resource_groups.create(new_resource_group)\n\n# update
-resource group\nresource_group = session.api.resource_groups.get().filter
-(name="new_resource_group").single_or_default()\nupdated_resource_group =
-ResourceGroupUpdateRequest(\n id=resource_group.id,\n
-name=resource_group.name,\n desc="Custom Resource Group #1 with updated
-description and site ids",\n siteIds=[200]\n)\n\n# switch to resource group
-view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete
-resource group\nsession.api.resource_groups.delete
-(resource_group.id)\n```\n\n\n\n\n TTeennaanntt mmaannaaggeemmeenntt (click to
-expand)\n\n```python\napi = session.api.tenant_management\n# create
-tenants\ntenants = [\n Tenant(\n name="tenant1",\n org_name="CiscoDevNet",\n
-subdomain="alpha.bravo.net",\n desc="This is tenant for unit tests",\n
-edge_connector_enable=True,\n edge_connector_system_ip="172.16.255.81",\n
-edge_connector_tunnel_interface_name="GigabitEthernet1",\n
-wan_edge_forecast=1,\n )\n]\ncreate_task = api.create
-(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data =
-api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter
-(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id =
-tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid =
-api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete(
-[tenant_id])\ndelete_task.wait_for_completed()\n#
-others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses
-()\napi.get_vsmart_mapping()\n```\n\n\n\n TTeennaanntt mmiiggrraattiioonn (click to
-expand)\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import
-create_manager_session\nfrom catalystwan.models.tenant import
-TenantExport\nfrom catalystwan.workflows.tenant_migration import
-migration_workflow\n\ntenant = TenantExport(\n name="mango",\n desc="Mango
-tenant description",\n org_name="Provider Org-Mango Inc",\n
-subdomain="mango.fruits.com",\n wan_edge_forecast=100,\n
-migration_key="MangoTenantMigrationKey", # only for SDWAN Manager >= 20.13\n
-is_destination_overlay_mt=True, # only for SDWAN Manager >= 20.13\n)\n\nwith
+description") session.api.users.update(new_user_update) # Update user password
+session.api.users.update_password("new_user", "n3W-P4s$w0rd") # Reset user
+session.api.users.reset("new_user") # Delete user session.api.users.delete
+("new_user") # Get current user authentication type and role
+session.api.users.get_auth_type() session.api.users.get_role() ``` UUsseerr GGrroouuppss
+(click to expand) ```python # Get all user groups session.api.user_groups.get()
+# Create user group group = UserGroup("new_user_group", []) group.enable_read(
+{"Audit Log", "Alarms"}) group.enable_read_and_write({"Device Inventory"})
+session.api.user_groups.create(group) # Update user group group.disable(
+{"Alarms"}) session.api.user_groups.update(group) # Delete user group
+session.api.user_groups.delete(group.group_name) ``` SSeessssiioonnss (click to expand)
+```python # Get all active sessions active_sessions = session.api.sessions.get
+() # Invalidate sessions for given user new_user_sessions =
+active_sessions.filter(raw_username="new_user") session.api.sessions.invalidate
+(new_user_sessions) ``` RReessoouurrccee GGrroouuppss (click to expand) ```python # get
+resource groups session.api.resource_groups.get() # create resource group
+new_resource_group = ResourceGroup( name="new_resource_group", desc="Custom
+Resource Group #1", siteIds=[] ) session.api.resource_groups.create
+(new_resource_group) # update resource group resource_group =
+session.api.resource_groups.get().filter
+(name="new_resource_group").single_or_default() updated_resource_group =
+ResourceGroupUpdateRequest( id=resource_group.id, name=resource_group.name,
+desc="Custom Resource Group #1 with updated description and site ids", siteIds=
+[200] ) # switch to resource group view session.api.resource_groups.switch
+("new_resource_group") # delete resource group
+session.api.resource_groups.delete(resource_group.id) ``` TTeennaanntt mmaannaaggeemmeenntt
+(click to expand) ```python api = session.api.tenant_management # create
+tenants tenants = [ Tenant( name="tenant1", org_name="CiscoDevNet",
+subdomain="alpha.bravo.net", desc="This is tenant for unit tests",
+edge_connector_enable=True, edge_connector_system_ip="172.16.255.81",
+edge_connector_tunnel_interface_name="GigabitEthernet1", wan_edge_forecast=1, )
+] create_task = api.create(tenants) create_task.wait_for_completed() # list all
+tenants tenants_data = api.get_all() # pick tenant from list by name tenant =
+tenants_data.filter(name="tenant1").single_or_default() # get selected tenant
+id tenant_id = tenant.tenant_id # get vsession id of selected tenant vsessionid
+= api.vsession_id(tenant_id) # delete tenant by ids delete_task = api.delete(
+[tenant_id]) delete_task.wait_for_completed() # others
+api.get_hosting_capacity_on_vsmarts() api.get_statuses() api.get_vsmart_mapping
+() ``` TTeennaanntt mmiiggrraattiioonn (click to expand) ```python from pathlib import Path
+from catalystwan.session import create_manager_session from
+catalystwan.models.tenant import TenantExport from
+catalystwan.workflows.tenant_migration import migration_workflow tenant =
+TenantExport( name="mango", desc="Mango tenant description", org_name="Provider
+Org-Mango Inc", subdomain="mango.fruits.com", wan_edge_forecast=100,
+migration_key="MangoTenantMigrationKey", # only for SDWAN Manager >= 20.13
+is_destination_overlay_mt=True, # only for SDWAN Manager >= 20.13 ) with
 create_manager_session(url="10.0.1.15", username="st-admin", password="") as
-origin_session, \\\n create_manager_session(url="10.9.0.16", username="mt-
-provider-admin", password="") as target_session:\n migration_workflow(\n
-origin_session=origin_session,\n target_session=target_session,\n workdir=Path
-("workdir"),\n tenant=tenant,\n validator="10.9.12.26"\n
-)\n```\n\n`migration_workflow` performs multi-step migration procedure
-according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco
-SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/
-configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-
-multitenancy.html#concept_sjj_jmm_z4b)\n\n\nSince 20.13 also MT to ST is
-supported (just provide suitable origin/target sessions, and
-`is_destination_overlay_mt` parameter)\n\n\nEach step of the
+origin_session, \ create_manager_session(url="10.9.0.16", username="mt-
+provider-admin", password="") as target_session: migration_workflow
+( origin_session=origin_session, target_session=target_session, workdir=Path
+("workdir"), tenant=tenant, validator="10.9.12.26" ) ``` `migration_workflow`
+performs multi-step migration procedure according to [Migrate Single-Tenant
+Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://
+www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/
+vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)
+Since 20.13 also MT to ST is supported (just provide suitable origin/target
+sessions, and `is_destination_overlay_mt` parameter) Each step of the
 `migration_workflow` procedure can be executed independently using api methods:
-`export_tenant`, `download`, `import_tenant`, `store_token`,
-`migrate_network`\n\n```python\norigin_api =
-origin_session.api.tenant_migration_api\ntarget_api =
-target_session.api.tenant_migration_api\ntenant_file = Path("~/
-tenant.tar.gz")\ntoken_file = Path("~/tenant-token.txt")\n# export\nexport_task
-= origin_api.export_tenant(tenant=tenant)\nremote_filename =
-export_task.wait_for_file()\n# download\norigin_api.download(export_path,
-remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path,
-tenant.migration_key)\nimport_task.wait_for_completed()\n# get
-token\nmigration_id =
-import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token
-(migration_id, token_path)\n# migrate network\nmigrate_task =
-origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed
-()\n```\n\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in
-your scripts (warning is suppressed when `catalystwan_devel` environment
-variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings
-(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching
-Exceptions\n```python\ntry:\n session.api.users.delete("bogus-user-
-name")\nexcept ManagerHTTPError as error:\n # Process an error.\n print
-(error.response.status_code)\n print(error.info.code)\n print
-(error.info.message)\n print(error.info.details)\n\n```\n\n## [Supported API
-endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/
-ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https:
-//github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)\n\n##
-Seeking support\n\nYou can contact us by submitting [issues](https://
-github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on
-catalystwan@cisco.com.\n', 'author': 'kagorski', 'author_email':
-'kagorski@cisco.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'https://github.com/cisco-open/cisco-catalyst-wan-sdk', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.8.0,<4.0.0', } setup(**setup_kwargs)
+`export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`
+```python origin_api = origin_session.api.tenant_migration_api target_api =
+target_session.api.tenant_migration_api tenant_file = Path("~/tenant.tar.gz")
+token_file = Path("~/tenant-token.txt") # export export_task =
+origin_api.export_tenant(tenant=tenant) remote_filename =
+export_task.wait_for_file() # download origin_api.download(export_path,
+remote_filename) # import import_task = target_api.import_tenant(export_path,
+tenant.migration_key) import_task.wait_for_completed() # get token migration_id
+= import_task.import_info.migration_token_query_params.migration_id
+target_api.store_token(migration_id, token_path) # migrate network migrate_task
+= origin_api.migrate_network(token_path) migrate_task.wait_for_completed() ```
+### Note: To remove `InsecureRequestWarning`, you can include in your scripts
+(warning is suppressed when `catalystwan_devel` environment variable is set):
+```Python import urllib3 urllib3.disable_warnings
+(urllib3.exceptions.InsecureRequestWarning) ``` ## Catching Exceptions
+```python try: session.api.users.delete("bogus-user-name") except
+ManagerHTTPError as error: # Process an error. print
+(error.response.status_code) print(error.info.code) print(error.info.message)
+print(error.info.details) ``` ## [Supported API endpoints](https://github.com/
+cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md) ## [Contributing, bug
+reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-
+wan-sdk/blob/main/CONTRIBUTING.md) ## Seeking support You can contact us by
+submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/
+issues), or directly via mail on catalystwan@cisco.com.
```

