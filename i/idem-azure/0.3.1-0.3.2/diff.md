# Comparing `tmp/idem-azure-0.3.1.tar.gz` & `tmp/idem-azure-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-azure-0.3.1.tar", last modified: Tue Mar 28 17:32:30 2023, max compression
+gzip compressed data, was "idem-azure-0.3.2.tar", last modified: Tue Apr 11 13:23:00 2023, max compression
```

## Comparing `idem-azure-0.3.1.tar` & `idem-azure-0.3.2.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.498041 idem-azure-0.3.1/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-03-28 17:32:15.000000 idem-azure-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7784 2023-03-28 17:32:30.498041 idem-azure-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6904 2023-03-28 17:32:15.000000 idem-azure-0.3.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.486041 idem-azure-0.3.1/idem_azure/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/acct/azure/
--rw-r--r--   0 root         (0) root         (0)     1994 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/acct/azure/login.py
--rw-r--r--   0 root         (0) root         (0)      801 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/acct/azure/mock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/acct/metadata/
--rw-r--r--   0 root         (0) root         (0)      361 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/acct/metadata/azure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.486041 idem-azure-0.3.1/idem_azure/backup/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/backup/virtual_networks/
--rw-r--r--   0 root         (0) root         (0)    10446 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/backup/virtual_networks/nat_gateways.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/backup/virtual_networks/public_ip_addresses.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/backup/virtual_networks/routes.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.486041 idem-azure-0.3.1/idem_azure/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/exec/azure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/exec/azure/authorization/
--rw-r--r--   0 root         (0) root         (0)     3940 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/authorization/role_assignments.py
--rw-r--r--   0 root         (0) root         (0)     4259 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/authorization/role_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/exec/azure/compute/
--rw-r--r--   0 root         (0) root         (0)     4226 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/compute/log_analytics_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4136 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/compute/virtual_machines.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/exec/azure/management_groups/
--rw-r--r--   0 root         (0) root         (0)     3779 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/management_groups/management_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/exec/azure/network/
--rw-r--r--   0 root         (0) root         (0)     3877 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/network/firewall.py
--rw-r--r--   0 root         (0) root         (0)     4133 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/network/firewall_policies.py
--rw-r--r--   0 root         (0) root         (0)     4030 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/network/network_interfaces.py
--rw-r--r--   0 root         (0) root         (0)     4221 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/network/network_security_groups.py
--rw-r--r--   0 root         (0) root         (0)     4082 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/network/public_ip_addresses.py
--rw-r--r--   0 root         (0) root         (0)     3946 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/network/route_tables.py
--rw-r--r--   0 root         (0) root         (0)     4372 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/network/routes.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/network/security_rules.py
--rw-r--r--   0 root         (0) root         (0)     4368 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/network/subnets.py
--rw-r--r--   0 root         (0) root         (0)     3995 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/network/virtual_networks.py
--rw-r--r--   0 root         (0) root         (0)     1252 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/permission.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/exec/azure/policy/
--rw-r--r--   0 root         (0) root         (0)     3193 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/policy/policy_assignments.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/policy/policy_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/exec/azure/resource_management/
--rw-r--r--   0 root         (0) root         (0)     3948 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/resource_management/resource_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/exec/azure/storage_resource_provider/
--rw-r--r--   0 root         (0) root         (0)     4116 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/storage_resource_provider/storage_accounts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/exec/azure/subscription/
--rw-r--r--   0 root         (0) root         (0)     4191 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/subscription/attach_subscriptions.py
--rw-r--r--   0 root         (0) root         (0)     4405 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/exec/azure/subscription/subscriptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/pop_create/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/pop_create/azure/
--rw-r--r--   0 root         (0) root         (0)     2572 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/pop_create/azure/api_reference.py
--rw-r--r--   0 root         (0) root         (0)     7156 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/pop_create/azure/api_spec.py
--rw-r--r--   0 root         (0) root         (0)     4639 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/pop_create/azure/init.py
--rw-r--r--   0 root         (0) root         (0)     5085 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/pop_create/azure/plugin.py
--rw-r--r--   0 root         (0) root         (0)     1526 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/pop_create/azure/resource.py
--rw-r--r--   0 root         (0) root         (0)     4766 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/pop_create/azure/rest.py
--rw-r--r--   0 root         (0) root         (0)    11179 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/pop_create/azure/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/reconcile/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/reconcile/pending/
--rw-r--r--   0 root         (0) root         (0)     1696 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/reconcile/pending/azure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/states/azure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/states/azure/authorization/
--rw-r--r--   0 root         (0) root         (0)    10160 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/authorization/role_assignments.py
--rw-r--r--   0 root         (0) root         (0)    12558 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/authorization/role_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/states/azure/compute/
--rw-r--r--   0 root         (0) root         (0)    16304 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/compute/log_analytics_workspace.py
--rw-r--r--   0 root         (0) root         (0)    19214 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/compute/virtual_machines.py
--rw-r--r--   0 root         (0) root         (0)      372 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/states/azure/management_groups/
--rw-r--r--   0 root         (0) root         (0)    11659 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/management_groups/management_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/states/azure/network/
--rw-r--r--   0 root         (0) root         (0)    15661 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/network/firewall.py
--rw-r--r--   0 root         (0) root         (0)    14759 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/network/firewall_policies.py
--rw-r--r--   0 root         (0) root         (0)    15558 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/network/network_interfaces.py
--rw-r--r--   0 root         (0) root         (0)    13416 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/network/network_security_groups.py
--rw-r--r--   0 root         (0) root         (0)    15996 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/network/public_ip_addresses.py
--rw-r--r--   0 root         (0) root         (0)    13902 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/network/route_tables.py
--rw-r--r--   0 root         (0) root         (0)    12656 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/network/routes.py
--rw-r--r--   0 root         (0) root         (0)    17082 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/network/security_rules.py
--rw-r--r--   0 root         (0) root         (0)    15622 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/network/subnets.py
--rw-r--r--   0 root         (0) root         (0)    14740 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/network/virtual_networks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/states/azure/policy/
--rw-r--r--   0 root         (0) root         (0)    12273 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/policy/policy_assignments.py
--rw-r--r--   0 root         (0) root         (0)    13235 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/policy/policy_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/states/azure/resource_management/
--rw-r--r--   0 root         (0) root         (0)    11624 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/resource_management/resource_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/states/azure/storage_resource_provider/
--rw-r--r--   0 root         (0) root         (0)    29137 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/storage_resource_provider/storage_accounts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/states/azure/subscription/
--rw-r--r--   0 root         (0) root         (0)     8445 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/subscription/attach_subscriptions.py
--rw-r--r--   0 root         (0) root         (0)    11421 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/states/azure/subscription/subscriptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/tool/azure/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/tool/azure/authorization/
--rw-r--r--   0 root         (0) root         (0)     2377 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/authorization/role_assignments.py
--rw-r--r--   0 root         (0) root         (0)     7362 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/authorization/role_definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/tool/azure/compute/
--rw-r--r--   0 root         (0) root         (0)    16498 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/compute/log_analytics_workspace.py
--rw-r--r--   0 root         (0) root         (0)    31418 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/compute/virtual_machines.py
--rw-r--r--   0 root         (0) root         (0)     1999 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/container.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.494041 idem-azure-0.3.1/idem_azure/tool/azure/management_groups/
--rw-r--r--   0 root         (0) root         (0)     4329 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/management_groups/management_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.498041 idem-azure-0.3.1/idem_azure/tool/azure/network/
--rw-r--r--   0 root         (0) root         (0)     6983 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/network/firewall.py
--rw-r--r--   0 root         (0) root         (0)     7073 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/network/firewall_policies.py
--rw-r--r--   0 root         (0) root         (0)    10032 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/network/network_interfaces.py
--rw-r--r--   0 root         (0) root         (0)    10207 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/network/network_security_groups.py
--rw-r--r--   0 root         (0) root         (0)    14334 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/network/public_ip_addresses.py
--rw-r--r--   0 root         (0) root         (0)     8907 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/network/route_tables.py
--rw-r--r--   0 root         (0) root         (0)     4816 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/network/routes.py
--rw-r--r--   0 root         (0) root         (0)    12345 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/network/security_rules.py
--rw-r--r--   0 root         (0) root         (0)    13498 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/network/subnets.py
--rw-r--r--   0 root         (0) root         (0)    11127 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/network/virtual_networks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.498041 idem-azure-0.3.1/idem_azure/tool/azure/policy/
--rw-r--r--   0 root         (0) root         (0)     3795 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/policy/policy_assignment.py
--rw-r--r--   0 root         (0) root         (0)     6870 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/policy/policy_definition.py
--rw-r--r--   0 root         (0) root         (0)     5513 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.498041 idem-azure-0.3.1/idem_azure/tool/azure/resource_management/
--rw-r--r--   0 root         (0) root         (0)     3308 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/resource_management/resource_groups.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.498041 idem-azure-0.3.1/idem_azure/tool/azure/storage_resource_provider/
--rw-r--r--   0 root         (0) root         (0)    52455 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/storage_resource_provider/storage_accounts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.498041 idem-azure-0.3.1/idem_azure/tool/azure/subscription/
--rw-r--r--   0 root         (0) root         (0)     3956 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/subscription/subscriptions.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/test_state_utils.py
--rw-r--r--   0 root         (0) root         (0)     2048 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/azure/uri.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.498041 idem-azure-0.3.1/idem_azure/tool/validators/
--rw-r--r--   0 root         (0) root         (0)      744 2023-03-28 17:32:15.000000 idem-azure-0.3.1/idem_azure/tool/validators/http.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-28 17:32:29.000000 idem-azure-0.3.1/idem_azure/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 17:32:30.490041 idem-azure-0.3.1/idem_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7784 2023-03-28 17:32:30.000000 idem-azure-0.3.1/idem_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4368 2023-03-28 17:32:30.000000 idem-azure-0.3.1/idem_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 17:32:30.000000 idem-azure-0.3.1/idem_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      197 2023-03-28 17:32:30.000000 idem-azure-0.3.1/idem_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-28 17:32:30.000000 idem-azure-0.3.1/idem_azure.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-28 17:32:30.498041 idem-azure-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2792 2023-03-28 17:32:15.000000 idem-azure-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-04-11 13:22:45.000000 idem-azure-0.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7784 2023-04-11 13:23:00.002657 idem-azure-0.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6904 2023-04-11 13:22:45.000000 idem-azure-0.3.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/acct/azure/
+-rw-r--r--   0 root         (0) root         (0)     1994 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/acct/azure/login.py
+-rw-r--r--   0 root         (0) root         (0)      801 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/acct/azure/mock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/acct/metadata/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/acct/metadata/azure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/backup/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/backup/virtual_networks/
+-rw-r--r--   0 root         (0) root         (0)    10446 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/backup/virtual_networks/nat_gateways.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/backup/virtual_networks/public_ip_addresses.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/backup/virtual_networks/routes.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/authorization/
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/authorization/role_assignments.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/authorization/role_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/compute/
+-rw-r--r--   0 root         (0) root         (0)     4226 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/compute/log_analytics_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4136 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/compute/virtual_machines.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/management_groups/
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/management_groups/management_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/network/
+-rw-r--r--   0 root         (0) root         (0)     3877 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/firewall.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/firewall_policies.py
+-rw-r--r--   0 root         (0) root         (0)     4030 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/network_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)     4221 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/network_security_groups.py
+-rw-r--r--   0 root         (0) root         (0)     4082 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/public_ip_addresses.py
+-rw-r--r--   0 root         (0) root         (0)     3946 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/route_tables.py
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/routes.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/security_rules.py
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/subnets.py
+-rw-r--r--   0 root         (0) root         (0)     3995 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/network/virtual_networks.py
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/permission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/policy/
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/policy/policy_assignments.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/policy/policy_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/resource_management/
+-rw-r--r--   0 root         (0) root         (0)     3948 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/resource_management/resource_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/storage_resource_provider/
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/storage_resource_provider/storage_accounts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/exec/azure/subscription/
+-rw-r--r--   0 root         (0) root         (0)     4191 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/subscription/attach_subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     4405 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/exec/azure/subscription/subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/pop_create/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/pop_create/azure/
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/api_reference.py
+-rw-r--r--   0 root         (0) root         (0)     7156 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/api_spec.py
+-rw-r--r--   0 root         (0) root         (0)     4639 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/init.py
+-rw-r--r--   0 root         (0) root         (0)     5085 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     1526 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/resource.py
+-rw-r--r--   0 root         (0) root         (0)     4766 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/rest.py
+-rw-r--r--   0 root         (0) root         (0)    11179 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/pop_create/azure/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/reconcile/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/reconcile/pending/
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/reconcile/pending/azure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/authorization/
+-rw-r--r--   0 root         (0) root         (0)    10160 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/authorization/role_assignments.py
+-rw-r--r--   0 root         (0) root         (0)    12622 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/authorization/role_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/compute/
+-rw-r--r--   0 root         (0) root         (0)    16304 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/compute/log_analytics_workspace.py
+-rw-r--r--   0 root         (0) root         (0)    19615 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/compute/virtual_machines.py
+-rw-r--r--   0 root         (0) root         (0)      372 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/management_groups/
+-rw-r--r--   0 root         (0) root         (0)    11659 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/management_groups/management_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/network/
+-rw-r--r--   0 root         (0) root         (0)    15838 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/firewall.py
+-rw-r--r--   0 root         (0) root         (0)    14921 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/firewall_policies.py
+-rw-r--r--   0 root         (0) root         (0)    15532 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/network_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)    15488 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/network_security_groups.py
+-rw-r--r--   0 root         (0) root         (0)    16001 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/public_ip_addresses.py
+-rw-r--r--   0 root         (0) root         (0)    13954 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/route_tables.py
+-rw-r--r--   0 root         (0) root         (0)    12656 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/routes.py
+-rw-r--r--   0 root         (0) root         (0)    17142 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/security_rules.py
+-rw-r--r--   0 root         (0) root         (0)    15676 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/subnets.py
+-rw-r--r--   0 root         (0) root         (0)    14926 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/network/virtual_networks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/policy/
+-rw-r--r--   0 root         (0) root         (0)    12283 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/policy/policy_assignments.py
+-rw-r--r--   0 root         (0) root         (0)    13235 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/policy/policy_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/resource_management/
+-rw-r--r--   0 root         (0) root         (0)    11624 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/resource_management/resource_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.998657 idem-azure-0.3.2/idem_azure/states/azure/storage_resource_provider/
+-rw-r--r--   0 root         (0) root         (0)    29668 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/storage_resource_provider/storage_accounts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/states/azure/subscription/
+-rw-r--r--   0 root         (0) root         (0)     8445 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/subscription/attach_subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)    11477 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/states/azure/subscription/subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/authorization/
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/authorization/role_assignments.py
+-rw-r--r--   0 root         (0) root         (0)     7362 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/authorization/role_definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/compute/
+-rw-r--r--   0 root         (0) root         (0)    16498 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/compute/log_analytics_workspace.py
+-rw-r--r--   0 root         (0) root         (0)    31418 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/compute/virtual_machines.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/container.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/management_groups/
+-rw-r--r--   0 root         (0) root         (0)     4329 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/management_groups/management_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/network/
+-rw-r--r--   0 root         (0) root         (0)     6983 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/firewall.py
+-rw-r--r--   0 root         (0) root         (0)     7073 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/firewall_policies.py
+-rw-r--r--   0 root         (0) root         (0)    10032 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/network_interfaces.py
+-rw-r--r--   0 root         (0) root         (0)    10207 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/network_security_groups.py
+-rw-r--r--   0 root         (0) root         (0)    14334 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/public_ip_addresses.py
+-rw-r--r--   0 root         (0) root         (0)     8907 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/route_tables.py
+-rw-r--r--   0 root         (0) root         (0)     4816 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/routes.py
+-rw-r--r--   0 root         (0) root         (0)    12345 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/security_rules.py
+-rw-r--r--   0 root         (0) root         (0)    13498 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/subnets.py
+-rw-r--r--   0 root         (0) root         (0)    11127 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/network/virtual_networks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/policy/
+-rw-r--r--   0 root         (0) root         (0)     3795 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/policy/policy_assignment.py
+-rw-r--r--   0 root         (0) root         (0)     6870 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/policy/policy_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5513 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/resource_management/
+-rw-r--r--   0 root         (0) root         (0)     3308 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/resource_management/resource_groups.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/storage_resource_provider/
+-rw-r--r--   0 root         (0) root         (0)    52455 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/storage_resource_provider/storage_accounts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/azure/subscription/
+-rw-r--r--   0 root         (0) root         (0)     3956 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/subscription/subscriptions.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/test_state_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2048 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/azure/uri.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:23:00.002657 idem-azure-0.3.2/idem_azure/tool/validators/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-04-11 13:22:45.000000 idem-azure-0.3.2/idem_azure/tool/validators/http.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-11 13:22:59.000000 idem-azure-0.3.2/idem_azure/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 13:22:59.994657 idem-azure-0.3.2/idem_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7784 2023-04-11 13:22:59.000000 idem-azure-0.3.2/idem_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4368 2023-04-11 13:22:59.000000 idem-azure-0.3.2/idem_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 13:22:59.000000 idem-azure-0.3.2/idem_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-11 13:22:59.000000 idem-azure-0.3.2/idem_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-11 13:22:59.000000 idem-azure-0.3.2/idem_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 13:23:00.002657 idem-azure-0.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2792 2023-04-11 13:22:45.000000 idem-azure-0.3.2/setup.py
```

### Comparing `idem-azure-0.3.1/LICENSE` & `idem-azure-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/PKG-INFO` & `idem-azure-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-azure
-Version: 0.3.1
+Version: 0.3.2
 Summary: UNKNOWN
 Home-page: https://gitlab.com/vmware/idem/idem-azure
 Author: Yingzhi Hao
 Author-email: hyingzhi@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-azure-0.3.1/README.rst` & `idem-azure-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/acct/azure/login.py` & `idem-azure-0.3.2/idem_azure/acct/azure/login.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/acct/azure/mock.py` & `idem-azure-0.3.2/idem_azure/acct/azure/mock.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/backup/virtual_networks/nat_gateways.py` & `idem-azure-0.3.2/idem_azure/backup/virtual_networks/nat_gateways.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/backup/virtual_networks/public_ip_addresses.py` & `idem-azure-0.3.2/idem_azure/backup/virtual_networks/public_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/backup/virtual_networks/routes.py` & `idem-azure-0.3.2/idem_azure/backup/virtual_networks/routes.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/conf.py` & `idem-azure-0.3.2/idem_azure/conf.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/authorization/role_assignments.py` & `idem-azure-0.3.2/idem_azure/exec/azure/authorization/role_assignments.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/authorization/role_definitions.py` & `idem-azure-0.3.2/idem_azure/exec/azure/authorization/role_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/compute/log_analytics_workspace.py` & `idem-azure-0.3.2/idem_azure/exec/azure/compute/log_analytics_workspace.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/compute/virtual_machines.py` & `idem-azure-0.3.2/idem_azure/exec/azure/compute/virtual_machines.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/management_groups/management_groups.py` & `idem-azure-0.3.2/idem_azure/exec/azure/management_groups/management_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/network/firewall.py` & `idem-azure-0.3.2/idem_azure/exec/azure/network/firewall.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/network/firewall_policies.py` & `idem-azure-0.3.2/idem_azure/exec/azure/network/firewall_policies.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/network/network_interfaces.py` & `idem-azure-0.3.2/idem_azure/exec/azure/network/network_interfaces.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/network/network_security_groups.py` & `idem-azure-0.3.2/idem_azure/exec/azure/network/network_security_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/network/public_ip_addresses.py` & `idem-azure-0.3.2/idem_azure/exec/azure/network/public_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/network/route_tables.py` & `idem-azure-0.3.2/idem_azure/exec/azure/network/route_tables.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/network/routes.py` & `idem-azure-0.3.2/idem_azure/exec/azure/network/routes.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/network/security_rules.py` & `idem-azure-0.3.2/idem_azure/exec/azure/network/security_rules.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/network/subnets.py` & `idem-azure-0.3.2/idem_azure/exec/azure/network/subnets.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/network/virtual_networks.py` & `idem-azure-0.3.2/idem_azure/exec/azure/network/virtual_networks.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/permission.py` & `idem-azure-0.3.2/idem_azure/exec/azure/permission.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/policy/policy_assignments.py` & `idem-azure-0.3.2/idem_azure/exec/azure/policy/policy_assignments.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/policy/policy_definitions.py` & `idem-azure-0.3.2/idem_azure/exec/azure/policy/policy_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/resource_management/resource_groups.py` & `idem-azure-0.3.2/idem_azure/exec/azure/resource_management/resource_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/storage_resource_provider/storage_accounts.py` & `idem-azure-0.3.2/idem_azure/exec/azure/storage_resource_provider/storage_accounts.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/subscription/attach_subscriptions.py` & `idem-azure-0.3.2/idem_azure/exec/azure/subscription/attach_subscriptions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/exec/azure/subscription/subscriptions.py` & `idem-azure-0.3.2/idem_azure/exec/azure/subscription/subscriptions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/pop_create/azure/api_reference.py` & `idem-azure-0.3.2/idem_azure/pop_create/azure/api_reference.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/pop_create/azure/api_spec.py` & `idem-azure-0.3.2/idem_azure/pop_create/azure/api_spec.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/pop_create/azure/init.py` & `idem-azure-0.3.2/idem_azure/pop_create/azure/init.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/pop_create/azure/plugin.py` & `idem-azure-0.3.2/idem_azure/pop_create/azure/plugin.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/pop_create/azure/resource.py` & `idem-azure-0.3.2/idem_azure/pop_create/azure/resource.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/pop_create/azure/rest.py` & `idem-azure-0.3.2/idem_azure/pop_create/azure/rest.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/pop_create/azure/template.py` & `idem-azure-0.3.2/idem_azure/pop_create/azure/template.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/reconcile/pending/azure.py` & `idem-azure-0.3.2/idem_azure/reconcile/pending/azure.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/authorization/role_assignments.py` & `idem-azure-0.3.2/idem_azure/states/azure/authorization/role_assignments.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/authorization/role_definitions.py` & `idem-azure-0.3.2/idem_azure/states/azure/authorization/role_definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,18 +36,22 @@
     Args:
         name(str): The identifier for this state.
         scope(str): The scope of the role definition.
         role_definition_id(str): The ID of the role definition.
         role_definition_name(str): The name of the role definition.
         permissions(list): The permissions of the role definitions.
 
-            * actions(list, Optional): Allowed actions
-            * notActions(list, Optional): Denied actions
-            * dataActions(list, Optional): Allowed Data actions
-            * notDataActions(list, Optional): Denied Data actions
+            * actions(list, Optional):
+                Allowed actions
+            * notActions(list, Optional):
+                Denied actions
+            * dataActions(list, Optional):
+                Allowed Data actions
+            * notDataActions(list, Optional):
+                Denied Data actions
         description(str): The description of the role definitions.
         assignable_scopes(list, Optional): The assignable scopes of the role definitions. Defaults to scope.
         resource_id(str, Optional): Role definition resource id on Azure.
 
     Returns:
         dict
```

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/compute/log_analytics_workspace.py` & `idem-azure-0.3.2/idem_azure/states/azure/compute/log_analytics_workspace.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/compute/virtual_machines.py` & `idem-azure-0.3.2/idem_azure/states/azure/compute/virtual_machines.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,47 +71,69 @@
     Args:
         name(str): The identifier for this state.
         resource_group_name(str): The name of the resource group.
         resource_id(str, Optional): Virtual Machine resource id on Azure
         virtual_machine_name(str): The name of the virtual machine.
         location(str): Resource location. Changing this forces a new resource to be created.
         virtual_machine_size(str): Specifies the size of the Virtual Machine.
-        network_interface_ids(List[str]): A list of Network Interface IDs which should be associated with the Virtual Machine.
+        network_interface_ids(list[str]): A list of Network Interface IDs which should be associated with the Virtual Machine.
         subscription_id(str, Optional): Subscription Unique id.
-        tags(Dict, Optional): Resource tags.
-        os_profile(Dict): Specifies the operating system settings used while creating the virtual machine.
+        tags(dict[str, str], Optional): Resource tags.
+        os_profile(dict[str, Any]): Specifies the operating system settings used while creating the virtual machine.
 
-            * computer_name(str): Specifies the name of the Virtual Machine.
-            * admin_username(str): Specifies the name of the local administrator account.
-            * admin_password(str): (Required for Windows, Optional for Linux) The password associated with the local administrator account.
-        storage_image_reference(Dict): Specifies information about the image to use. Eg- platform images, marketplace images.
-
-            * image_sku(str): Specifies the SKU of the image used to create the virtual machine. Changing this forces a new resource to be created.
-            * image_publisher(str): Specifies the publisher of the image used to create the virtual machine. Changing this forces a new resource to be created.
-            * image_version(str): Specifies the version of the image used to create the virtual machine. Changing this forces a new resource to be created.
-            * image_offer(str, Optional):  Specifies the offer of the image used to create the virtual machine. Changing this forces a new resource to be created.
-        storage_os_disk(Dict): Specifies information about the operating system disk used by the virtual machine.
-
-            * disk_name(str): Specifies the name of the OS Disk.
-            * disk_create_option(str): Specifies how the OS Disk should be created. Possible values are Attach (managed disks only) and FromImage.
-            * storage_account_type(str, Optional): Specifies the type of Managed Disk which should be created. Possible values are Standard_LRS, StandardSSD_LRS or Premium_LRS.
-            * disk_caching(str, Optional): Specifies the caching requirements for the OS Disk. Possible values include None, ReadOnly and ReadWrite.
-            * disk_size_in_GB(str, Optional): Specifies the size of the OS Disk in gigabytes.
-            * disk_delete_option(str, Optional): Specifies how the OS Disk should be handled after VM deletion. Possible values are Detach and Delete.
-            * disk_id(str, Optional): Specifies the ID of an existing Managed Disk which should be attached as the OS Disk of this Virtual Machine. If this is set then the create_option must be set to Attach.
-        storage_data_disks(list(Dict), Optional): List of Data disks attached/added to a VM.
-
-            * disk_name(str): The name of the Data Disk.
-            * disk_create_option(str): Specifies how the data disk should be created. Possible values are Attach, FromImage and Empty.
-            * disk_logical_unit_number(str): Specifies the logical unit number of the data disk. This needs to be unique within all the Data Disks on the Virtual Machine.
-            * storage_account_type(str, Optional): Specifies the type of managed disk to create. Possible values are either Standard_LRS, StandardSSD_LRS, Premium_LRS or UltraSSD_LRS.
-            * disk_caching(str, Optional): Specifies the caching requirements for the Data Disk. Possible values include None, ReadOnly and ReadWrite.
-            * disk_size_in_GB(str, Optional): Specifies the size of the data disk in gigabytes.
-            * disk_delete_option(str, Optional): Specifies how the OS Disk should be handled after VM deletion. Possible values are Detach and Delete.
-            * disk_id(str, Optional): Specifies the ID of an Existing Managed Disk which should be attached to this Virtual Machine. When this field is set create_option must be set to Attach.
+            * computer_name(str):
+                Specifies the name of the Virtual Machine.
+            * admin_username(str):
+                Specifies the name of the local administrator account.
+            * admin_password(str):
+                (Required for Windows, Optional for Linux) The password associated with the local administrator account.
+        storage_image_reference(dict[str, Any]): Specifies information about the image to use. Eg- platform images, marketplace images.
+
+            * image_sku(str):
+                Specifies the SKU of the image used to create the virtual machine. Changing this forces a new resource to be created.
+            * image_publisher(str):
+                Specifies the publisher of the image used to create the virtual machine. Changing this forces a new resource to be created.
+            * image_version(str):
+                Specifies the version of the image used to create the virtual machine. Changing this forces a new resource to be created.
+            * image_offer(str, Optional):
+                Specifies the offer of the image used to create the virtual machine. Changing this forces a new resource to be created.
+        storage_os_disk(dict[str, Any]): Specifies information about the operating system disk used by the virtual machine.
+
+            * disk_name(str):
+                Specifies the name of the OS Disk.
+            * disk_create_option(str):
+                Specifies how the OS Disk should be created. Possible values are Attach (managed disks only) and FromImage.
+            * storage_account_type(str, Optional):
+                Specifies the type of Managed Disk which should be created. Possible values are Standard_LRS, StandardSSD_LRS or Premium_LRS.
+            * disk_caching(str, Optional):
+                Specifies the caching requirements for the OS Disk. Possible values include None, ReadOnly and ReadWrite.
+            * disk_size_in_GB(str, Optional):
+                Specifies the size of the OS Disk in gigabytes.
+            * disk_delete_option(str, Optional):
+                Specifies how the OS Disk should be handled after VM deletion. Possible values are Detach and Delete.
+            * disk_id(str, Optional):
+                Specifies the ID of an existing Managed Disk which should be attached as the OS Disk of this Virtual Machine. If this is set then the create_option must be set to Attach.
+        storage_data_disks(list(dict[str, Any]), Optional): List of Data disks attached/added to a VM.
+
+            * disk_name(str):
+                The name of the Data Disk.
+            * disk_create_option(str):
+                Specifies how the data disk should be created. Possible values are Attach, FromImage and Empty.
+            * disk_logical_unit_number(str):
+                Specifies the logical unit number of the data disk. This needs to be unique within all the Data Disks on the Virtual Machine.
+            * storage_account_type(str, Optional):
+                Specifies the type of managed disk to create. Possible values are either Standard_LRS, StandardSSD_LRS, Premium_LRS or UltraSSD_LRS.
+            * disk_caching(str, Optional):
+                Specifies the caching requirements for the Data Disk. Possible values include None, ReadOnly and ReadWrite.
+            * disk_size_in_GB(str, Optional):
+                Specifies the size of the data disk in gigabytes.
+            * disk_delete_option(str, Optional):
+                Specifies how the OS Disk should be handled after VM deletion. Possible values are Detach and Delete.
+            * disk_id(str, Optional):
+                Specifies the ID of an Existing Managed Disk which should be attached to this Virtual Machine. When this field is set create_option must be set to Attach.
 
     Returns:
         Dict
 
     Examples:
         .. code-block:: sls
```

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/management_groups/management_groups.py` & `idem-azure-0.3.2/idem_azure/states/azure/management_groups/management_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/network/firewall.py` & `idem-azure-0.3.2/idem_azure/states/azure/network/firewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,29 +49,40 @@
 
     Args:
         name(str): The identifier for this state.
         location(str): Resource location. Changing this forces a new resource to be created.
         resource_group_name(str): The name of the resource group.
         subscription_id(str, Optional): Subscription Unique id.
         resource_id(str, Optional): firewall resource id on Azure
-        tags(Dict, Optional): Resource tags.
+        tags(dict[str, str], Optional): Resource tags.
         firewall_name(str): The name of the firewall.
-        zones(List[str]): A list of availability zones denoting where the resource needs to come from.
-        sku(Dict, Optional): The SKU of the Firewall.
-            name(str): SKU name of the Firewall. Possible values are AZFW_Hub and AZFW_VNet. Changing this forces a new resource to be created.
-            tier(str): SKU tier of the Firewall. Possible values are Premium, Standard and Basic.
+        zones(list[str]): A list of availability zones denoting where the resource needs to come from.
+        sku(dict[str, Any], Optional): The SKU of the Firewall.
+
+            * name(str):
+                SKU name of the Firewall. Possible values are AZFW_Hub and AZFW_VNet. Changing this forces a new resource to be created.
+            * tier(str):
+                SKU tier of the Firewall. Possible values are Premium, Standard and Basic.
         firewall_policy_id(str): The ID of the Firewall Policy applied to this Firewall.
-        ip_configuration(List[Dict[str, Any]], Optional): IP configuration of the Firewall.
-            name(str): SKU name of the Firewall. Possible values are AZFW_Hub and AZFW_VNet. Changing this forces a new resource to be created.
-            subnet_id(str): SKU tier of the Firewall. Possible values are Premium, Standard and Basic.
-            public_ip_address_id(str): SKU tier of the Firewall. Possible values are Premium, Standard and Basic.
-        management_ip_configuration(Dict, Optional): Management IP configuration of the Firewall.
-            name(str): Specifies the name of the IP Configuration.
-            subnet_id(str): Reference to the subnet associated with the IP Configuration. Changing this forces a new resource to be created.
-            public_ip_address_id(str): The ID of the Public IP Address associated with the firewall.
+        ip_configuration(list[dict[str, Any]], Optional): IP configuration of the Firewall.
+
+            * name(str):
+                SKU name of the Firewall. Possible values are AZFW_Hub and AZFW_VNet. Changing this forces a new resource to be created.
+            * subnet_id(str):
+                SKU tier of the Firewall. Possible values are Premium, Standard and Basic.
+            * public_ip_address_id(str):
+                SKU tier of the Firewall. Possible values are Premium, Standard and Basic.
+        management_ip_configuration(dict[str, Any], Optional): Management IP configuration of the Firewall.
+
+            * name(str):
+                Specifies the name of the IP Configuration.
+            * subnet_id(str):
+                Reference to the subnet associated with the IP Configuration. Changing this forces a new resource to be created.
+            * public_ip_address_id(str):
+                The ID of the Public IP Address associated with the firewall.
 
     Returns:
         Dict
 
     Examples:
         .. code-block:: sls
```

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/network/firewall_policies.py` & `idem-azure-0.3.2/idem_azure/states/azure/network/firewall_policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,27 +49,37 @@
 
     Args:
         name(str): The identifier for this state.
         location(str): Resource location. Changing this forces a new resource to be created.
         resource_group_name(str): The name of the resource group.
         subscription_id(str, Optional): Subscription Unique id.
         resource_id(str, Optional): Firewall Policy resource id on Azure
-        tags(Dict, Optional): Resource tags.
+        tags(dict[str, str], Optional): Resource tags.
         firewall_policy_name(str): The name of the firewall policy.
         base_policy_id(str, Optional): The ID of the base Firewall Policy.
-        threat_intelligence_allow_list(Dict, Optional): Specifies threat_intelligence_allowlist while creating the Firewall policy.
-            fqdns(List[str]): A list of FQDNs that will be skipped for threat detection.
-            ip_addresses(List[str]): A list of IP addresses or CIDR ranges that will be skipped for threat detection.
-        dns_settings(Dict, Optional): Specifies dns setting while creating the Firewall policy.
-            proxy_enabled(bool): Whether to enable DNS proxy on Firewalls attached to this Firewall Policy.
-            servers(List[str]): A list of custom DNS servers' IP addresses.
-        sku(Dict, Optional): The SKU Tier of the Firewall Policy.
-            tier(str): Possible values are Standard, Premium and Basic. Changing this forces a new Firewall Policy to be created.
-        intrusion_detection(Dict, Optional): A intrusion_detection block for Firewall policy.
-            mode(str): In which mode you want to run intrusion detection: Off, Alert or Deny.
+        threat_intelligence_allow_list(dict[str, Any], Optional): Specifies threat_intelligence_allowlist while creating the Firewall policy.
+
+            * fqdns(list[str]):
+                A list of FQDNs that will be skipped for threat detection.
+            * ip_addresses(list[str]):
+                A list of IP addresses or CIDR ranges that will be skipped for threat detection.
+        dns_settings(dict[str, Any], Optional): Specifies dns setting while creating the Firewall policy.
+
+            * proxy_enabled(bool):
+                Whether to enable DNS proxy on Firewalls attached to this Firewall Policy.
+            * servers(list[str]):
+                A list of custom DNS servers' IP addresses.
+        sku(dict[str, Any], Optional): The SKU Tier of the Firewall Policy.
+
+            * tier(str):
+                Possible values are Standard, Premium and Basic. Changing this forces a new Firewall Policy to be created.
+        intrusion_detection(dict[str, Any], Optional): A intrusion_detection block for Firewall policy.
+
+            * mode(str):
+                In which mode you want to run intrusion detection: Off, Alert or Deny.
         threat_intelligence_mode(str, Optional): The operation mode for Threat Intelligence. Possible values are Alert, Deny and Off. Defaults to Alert.
 
     Returns:
         Dict
 
     Examples:
         .. code-block:: sls
```

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/network/network_interfaces.py` & `idem-azure-0.3.2/idem_azure/states/azure/network/network_interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,37 +37,33 @@
     r"""Create or update Network Interfaces.
 
     Args:
         name(str): The identifier for this state.
         resource_group_name(str): The name of the resource group.
         network_interface_name(str): The name of the network interface.
         location(str): Resource location. This field can not be updated.
-        ip_configurations(List[Dict[str, Any]]): A list of IPConfigurations of the network interface. Each ip configuration supports fields:
+        ip_configurations(list[dict[str, Any]]): A list of IPConfigurations of the network interface. Each ip configuration supports fields:
 
-            * name(str): The name of the resource that is unique within a
-              resource group.
-            * private_ip_address_allocation(str): The allocation method used for
-              the Private IP Address. Possible values are Dynamic and Static.
-              Azure does not assign a Dynamic IP Address until the Network
-              Interface is attached to a running Virtual Machine(or other resource).
-            * subnet_id(str): Resource ID of the Subnet bound to the
-              IP configuration. The name of the resource
-              that is unique within a resource group.
-              This is required when private_ip_address_version is set to IPv4.
-            * private_ip_address_version(str): The specific IP configuration is
-              IPv4 or IPv6. Default is IPv4.
-            * private_ip_address(str): The Static IP Address which should be used.
-              When private_ip_address_allocation is set to Static,
-              private_ip_address can be configured.
-            * primary(bool): To check if this is the primary IP Configuration.
-              Must be true for the first ip_configuration
-              when multiple are specified. Defaults to false.
-              Primary attribute must be true for the first ip_configuration when
-              multiple are specified. Defaults to false.
-        tags(Dict, Optional): Resource tags.
+            * name(str):
+                The name of the resource that is unique within a resource group.
+            * private_ip_address_allocation(str):
+                The allocation method used for the Private IP Address. Possible values are Dynamic and Static.
+                Azure does not assign a Dynamic IP Address until the Network Interface is attached to a running Virtual Machine(or other resource).
+            * subnet_id(str):
+                Resource ID of the Subnet bound to the IP configuration. The name of the resource that is unique within a resource group.
+                This is required when private_ip_address_version is set to IPv4.
+            * private_ip_address_version(str):
+                The specific IP configuration is IPv4 or IPv6. Default is IPv4.
+            * private_ip_address(str):
+                The Static IP Address which should be used. When private_ip_address_allocation is set to Static, private_ip_address can be configured.
+            * primary(bool):
+                To check if this is the primary IP Configuration. Must be true for the first ip_configuration when
+                multiple are specified. Defaults to false. Primary attribute must be true for the first ip_configuration
+                when multiple are specified. Defaults to false.
+        tags(dict[str, str], Optional): Resource tags.
         subscription_id(str, Optional): Subscription Unique id.
         resource_id(str, Optional): Network Interface resource id on Azure.
 
     Returns:
         Dict
 
     Examples:
```

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/network/network_security_groups.py` & `idem-azure-0.3.2/idem_azure/states/azure/network/network_security_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,36 +26,64 @@
                 ("direction", str),
                 ("access", str),
                 ("protocol", str),
                 ("source_port_range", str, field(default=None)),
                 ("destination_port_range", str, field(default=None)),
                 ("source_address_prefix", str, field(default=None)),
                 ("destination_address_prefix", str, field(default=None)),
-                ("source_port_ranges", List, field(default=None)),
-                ("destination_port_ranges", List, field(default=None)),
-                ("source_address_prefixes", List, field(default=None)),
-                ("destination_address_prefixes", List, field(default=None)),
+                ("source_port_ranges", List[str], field(default=None)),
+                ("destination_port_ranges", List[str], field(default=None)),
+                ("source_address_prefixes", List[str], field(default=None)),
+                ("destination_address_prefixes", List[str], field(default=None)),
             ],
         )
     ] = None,
     tags: Dict = None,
     subscription_id: str = None,
     resource_id: str = None,
 ) -> Dict:
     r"""Create or update Network Security Groups.
 
     Args:
         name(str): The identifier for this state.
         resource_group_name(str): The name of the resource group.
         network_security_group_name(str): The name of the network security group.
         location(str): The location to create the resource in.
-        security_rules(List, Optional): List of security rules.Either source_port_range or source_port_ranges needs to be provided.
-                                        Either destination_port_range or destination_port_ranges needs to be provided.
-                                        Either source_address_prefix or source_address_prefixes needs to be provided.
-                                        Either destination_address_prefix or destination_address_prefixs needs to be provided
+        security_rules(list[dict[str, Any]], Optional): List of security rules. Each security rule contains:
+
+            * name(str):
+                The name of the security rule.
+            * priority(int):
+                The priority of the security rule. The value can be between 100 and 4096.The priority number must
+                be unique for each rule in the collection. The lower the priority number, the higher the priority of the rule.
+            * direction(str):
+                The direction of the rule. The direction specifies if rule will be evaluated on incoming or outgoing traffic.
+            * access(str):
+                The network traffic is allowed or denied.
+            * protocol(str):
+                Network protocol this rule applies to.
+            * source_port_range(str, Optional):
+                The source port or range. Integer or range between 0 and 65535. Asterisk '*' can also be used to match all ports.
+            * destination_port_range(str, Optional):
+                The destination port or range. Integer or range between 0 and 65535. Asterisk '*' can also be used to match all ports.
+            * source_address_prefix(str, Optional):
+                The source address prefix. CIDR or source IP range. Asterisk '*' can also be used to match all
+                source IPs. Default tags such as 'VirtualNetwork', 'AzureLoadBalancer' and 'Internet' can also be used. If
+                this is an ingress rule, specifies where network traffic originates from.
+            * destination_address_prefix(str, Optional):
+                The destination address prefix. CIDR or destination IP range. Asterisk '*' can also be used to match all source IPs. Default tags such as 'VirtualNetwork',
+                'AzureLoadBalancer' and 'Internet' can also be used.
+            * source_port_ranges(list[str], Optional):
+                The source port ranges. Either this or source_port_range need to be provided.
+            * destination_port_ranges(list[str], Optional):
+                The destination port ranges.Either this or destination_port_range need to be provided.
+            * source_address_prefixes(list[str], Optional):
+                The CIDR or source IP ranges. Either source_address_prefix or source_address_prefixes needs to be provided.
+            * destination_address_prefixes(list[str], Optional):
+                The destination address prefixes. CIDR or destination IP ranges. Either destination_address_prefix or destination_address_prefixes needs to be provided.
         tags(Dict, Optional): Resource tags.
         subscription_id(str, Optional): Subscription Unique id.
         resource_id(str, Optional): Resource Group id on Azure.
 
     Returns:
         Dict
```

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/network/public_ip_addresses.py` & `idem-azure-0.3.2/idem_azure/states/azure/network/public_ip_addresses.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     Args:
         name(str): The identifier for this state.
         resource_group_name(str): The name of the resource group.
         public_ip_address_name(str): The name of the public IP address.
         location(str): Resource location.
         allocation_method(str): Defines the allocation method for this IP address.
-        zones(List, Optional): A collection containing the availability zone to allocate the Public IP in.
+        zones(list[str], Optional): A collection containing the availability zone to allocate the Public IP in.
         ddos_protection_mode(str, Optional): The DDoS protection mode of the public IP.
         ddos_protection_plan_id(str, Optional): The ID of DDoS protection plan associated with the public IP.
         domain_name_label(str, Optional): Label for the Domain Name.
         edge_zone(str, Optional): Specifies the Edge Zone within the Azure Region where this Public IP should exist.
         idle_timeout_in_minutes(int, Optional): Specifies the timeout for the TCP idle connection.
         ip_tags(dict, Optional): A mapping of IP tags to assign to the public IP.
         ip_version(str, Optional): The IP Version to use.
```

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/network/route_tables.py` & `idem-azure-0.3.2/idem_azure/states/azure/network/route_tables.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,21 +37,26 @@
 
     Args:
         name(str): The identifier for this state.
         resource_group_name(str): The name of the resource group.
         route_table_name(str): The name of the route table.
         location(str): Resource location. This field can not be updated.
         routes(list, Optional): An array of routes on the route table. Collection of routes contained within a route table.
-         Defaults to None
-         * route_name(str) -- The name of the resource that is unique within a resource group.
-         * address_prefix(str) -- The destination CIDR to which the route applies.
-         * next_hop_type(str) -- The type of Azure hop the packet should be sent to.
-         * next_hop_ip_address(str, Optional) -- The IP address packets should be forwarded to. Next hop values are only allowed in routes where the next hop type is VirtualAppliance.
+         Defaults to None.
+
+         * route_name(str):
+            The name of the resource that is unique within a resource group.
+         * address_prefix(str):
+            The destination CIDR to which the route applies.
+         * next_hop_type(str):
+            The type of Azure hop the packet should be sent to.
+         * next_hop_ip_address(str, Optional):
+            The IP address packets should be forwarded to. Next hop values are only allowed in routes where the next hop type is VirtualAppliance.
         disable_bgp_route_propagation(bool, Optional): Whether to disable the routes learned by BGP on that route table. True means disable.
-        tags(Dict, Optional): Resource tags.
+        tags(dict[str, str], Optional): Resource tags.
         subscription_id: Subscription Unique id.
         resource_id: Route table resource id on Azure.
 
     Returns:
         dict
 
     Examples:
```

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/network/routes.py` & `idem-azure-0.3.2/idem_azure/states/azure/network/routes.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/network/security_rules.py` & `idem-azure-0.3.2/idem_azure/states/azure/network/security_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     security_rule_name: str,
     priority: int,
     direction: str,
     access: str,
     protocol: str,
     description: str = None,
     source_port_range: str = None,
-    source_port_ranges: List = None,
+    source_port_ranges: List[str] = None,
     source_address_prefix: str = None,
-    source_address_prefixes: List = None,
-    source_application_security_groups: List = None,
+    source_address_prefixes: List[str] = None,
+    source_application_security_groups: List[str] = None,
     destination_port_range: str = None,
-    destination_port_ranges: List = None,
+    destination_port_ranges: List[str] = None,
     destination_address_prefix: str = None,
-    destination_address_prefixes: List = None,
-    destination_application_security_groups: List = None,
+    destination_address_prefixes: List[str] = None,
+    destination_application_security_groups: List[str] = None,
     subscription_id: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     r"""Create or update Security Rules.
 
     Args:
         name(str): The identifier for this state.
@@ -43,29 +43,29 @@
             be unique for each rule in the collection. The lower the priority number, the higher the priority of the rule.
         direction(str): The direction of the rule. The direction specifies if rule will be evaluated on incoming or outgoing traffic.
         access(str): The network traffic is allowed or denied.
         protocol(str): Network protocol this rule applies to.
         description(str, Optional): A description for this rule.
         source_port_range(str, Optional): The source port or range. Integer or range between 0 and 65535. Asterisk '*'
             can also be used to match all ports.
-        source_port_ranges(List, Optional): The source port ranges. Either this or source_port_range need to be provided.
+        source_port_ranges(list[str], Optional): The source port ranges. Either this or source_port_range need to be provided.
         source_address_prefix(str, Optional): The source address prefix. CIDR or source IP range. Asterisk '*' can also be used to match all
             source IPs. Default tags such as 'VirtualNetwork', 'AzureLoadBalancer' and 'Internet' can also be used. If
             this is an ingress rule, specifies where network traffic originates from.
-        source_address_prefixes(List, Optional): The CIDR or source IP ranges.
-        source_application_security_groups(List, Optional): The list of resource id of the application security group.
+        source_address_prefixes(list[str], Optional): The CIDR or source IP ranges.
+        source_application_security_groups(list[str], Optional): The list of resource id of the application security group.
             Either one of source_address_prefix, source_address_prefixes or source_application_security_groups needs to be provided.
         destination_port_range(str, Optional): The destination port or range. Integer or range between 0 and 65535.
             Asterisk '*' can also be used to match all ports.
-        destination_port_ranges(List, Optional): The destination port ranges. Either this or destination_port_range need to be provided.
+        destination_port_ranges(list[str], Optional): The destination port ranges. Either this or destination_port_range need to be provided.
         destination_address_prefix(str, Optional): The destination address prefix. CIDR or destination IP range.
             Asterisk '*' can also be used to match all source IPs. Default tags such as 'VirtualNetwork',
             'AzureLoadBalancer' and 'Internet' can also be used.
-        destination_address_prefixes(List, Optional): The destination address prefixes. CIDR or destination IP ranges.
-        destination_application_security_groups(List, Optional): The list of resource id of the application security group.
+        destination_address_prefixes(list[str], Optional): The destination address prefixes. CIDR or destination IP ranges.
+        destination_application_security_groups(list[str], Optional): The list of resource id of the application security group.
             Either one of destination_address_prefix, destination_address_prefixes or destination_application_security_groups needs to be provided.
         subscription_id(str, Optional): Subscription Unique id.
         resource_id(str, Optional): Security rule resource id.
 
     Returns:
         Dict[str, Any]
```

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/network/subnets.py` & `idem-azure-0.3.2/idem_azure/states/azure/network/subnets.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,21 +39,23 @@
     Args:
         name(str): The identifier for this state.
         resource_group_name(str): The name of the resource group.
         virtual_network_name(str): The name of the virtual network.
         subnet_name(str): The name of the subnet.
         address_prefix(str): The address prefix for the subnet.
         enforce_private_link_endpoint_network_policies(bool, Optional): Enable or Disable apply network policies on private end point in the subnet.
-        delegations(List, Optional): An array of references to the delegations on the subnet. Defaults to None
+        delegations(list, Optional): An array of references to the delegations on the subnet. Defaults to None
 
-         * name(str) -- The name of the resource that is unique within a subnet.
-         * service(str) -- The name of the service to whom the subnet should be delegated.
+            * name(str, Optional):
+                The name of the resource that is unique within a subnet.
+            * service(str, Optional):
+                The name of the service to whom the subnet should be delegated.
         enforce_private_link_service_network_policies(bool, Optional): Enable or Disable apply network policies on private link service in the subnet.
-        service_endpoints(List, Optional): An array of service endpoints
-        service_endpoint_policy_ids(List, Optional): An array of service endpoint policy Ids.\
+        service_endpoints(list, Optional): An array of service endpoints
+        service_endpoint_policy_ids(list, Optional): An array of service endpoint policy Ids.\
         subscription_id(str, Optional): Subscription Unique id.
         resource_id(str, Optional): Subnet resource id on Azure
 
     Returns:
         Dict
 
     Examples:
```

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/network/virtual_networks.py` & `idem-azure-0.3.2/idem_azure/states/azure/network/virtual_networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,24 @@
         resource_group_name(str): The name of the resource group.
         virtual_network_name(str): The name of the virtual network.
         address_space(list): An array of IP address ranges that can be used by subnets of the virtual network.
         location(str): Resource location. This field can not be updated.
         resource_id(str, Optional): Virtual Network resource id on Azure
         bgp_communities(dict, Optional): Bgp Communities sent over ExpressRoute with each route corresponding to a prefix in this VNET.
         flow_timeout_in_minutes(int, Optional): The FlowTimeout value (in minutes) for the Virtual Network
-        subnets(List, Optional): List of Subnet in a virtual network resource.Each Subnet will have fields
-          name(str, required), address_space(str, required) , security_group_id(str, Optional) and service_endpoints(list, Optional)
+        subnets(list, Optional): List of Subnet in a virtual network resource.Each Subnet will have fields
+
+            * name(str):
+                The name of subnet.
+            * address_space(str):
+                Address space of the subnet.
+            * security_group_id(str, Optional):
+                The security group id.
+            * service_endpoints(list, Optional):
+                List of service endpoint.
         subscription_id(str, Optional): Subscription Unique id.
         tags(dict, Optional): Resource tags.
 
     Returns:
         dict
 
     Examples:
```

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/policy/policy_assignments.py` & `idem-azure-0.3.2/idem_azure/states/azure/policy/policy_assignments.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     r"""Create or update Policy Assignments.
 
     Args:
         name(str): The identifier for this state.
         scope(str): The scope of the policy assignment. Valid scopes are: management group (format: '/providers/Microsoft.Management/managementGroups/{managementGroup}'), subscription (format: '/subscriptions/{subscriptionId}'), resource group (format: '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}', or resource (format: '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/{resourceProviderNamespace}/[{parentResourcePath}/]{resourceType}/{resourceName}'.
         policy_assignment_name(str): The name which should be used for this Policy Assignment. Changing this forces a new Resource Policy Assignment to be created.
         policy_definition_id(str): The ID of the Policy Definition or Policy Definition Set. Changing this forces a new Policy Assignment to be created
-        parameters(Dict, Optional): Policy assignment parameters with respect to policy definition rule. Defaults to {}.
+        parameters(dict[str, Any], Optional): Policy assignment parameters with respect to policy definition rule. Defaults to {}.
         resource_id(str, Optional): Policy Assignment resource id on Azure
 
     Returns:
         dict
 
     Examples:
         .. code-block:: sls
```

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/policy/policy_definitions.py` & `idem-azure-0.3.2/idem_azure/states/azure/policy/policy_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/resource_management/resource_groups.py` & `idem-azure-0.3.2/idem_azure/states/azure/resource_management/resource_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/storage_resource_provider/storage_accounts.py` & `idem-azure-0.3.2/idem_azure/states/azure/storage_resource_provider/storage_accounts.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,67 +149,90 @@
         min_tls_version(str, Optional): The minimum supported TLS version for the storage account.
         allow_blob_public_access(bool, Optional): Allow or disallow nested items within this Account to opt into being public.
         allow_shared_key_access(bool, Optional): Indicates whether the storage account permits requests to be authorized with the account access key via Shared Key.
         public_network_access(str, Optional): Allow or disallow public network access to Storage Account. Value is optional but if passed in, must be 'Enabled' or 'Disabled'.
         default_to_oauth_authentication(bool, Optional): A boolean flag which indicates whether the default authentication is OAuth or not. The default interpretation is false for this property.
         is_hns_enabled(bool, Optional): Account HierarchicalNamespace enabled if sets to true.
         nfsv3_enabled(bool, Optional): NFS 3.0 protocol support enabled if set to true.
-        custom_domain(Dict, Optional): User domain assigned to the storage account.
+        custom_domain(dict[str, Any], Optional): User domain assigned to the storage account.
 
-            * name(str): The Custom Domain Name to use for the Storage Account
-            * use_subdomain(bool, Optional): Indicates whether indirect CName validation is enabled. Default value is false
-        customer_managed_key(Dict, Optional): Combination of Key vault key id and user assigned id
-
-            * user_assigned_identity_id(str): User Assigned Identity id
-            * key_vault_key_id(str): The object identifier of the current versioned Key Vault Key in use.
-        identity: The identity of the resource.
-
-            * type(str): The identity type. Possible values are SystemAssigned, UserAssigned, SystemAssigned, UserAssigned
-            * user_assigned_identities(Dict, Optional): Key value pairs that describe the set of User Assigned identities that will be used with this storage account
-        network_rules: Network rule set
-
-            * default_action(str): Specifies the default action of allow or deny when no other rules match. Valid options are Deny or Allow
-            * bypass(str, Optional): Specifies whether traffic is bypassed for Logging/Metrics/AzureServices. Possible values are any combination of Logging|Metrics|AzureServices
-            * ip_rule_values(List, Optional): List of IP or IP range in CIDR format. Only IPV4 address is allowed.
-            * virtual_network_subnet_ids(List, Optional): A list of resource ids of virtual network subnets.
-            * resource_access_rules(Dict, Optional): The resource access rules
+            * name(str):
+                The Custom Domain Name to use for the Storage Account
+            * use_subdomain(bool, Optional):
+                Indicates whether indirect CName validation is enabled. Default value is false
+        customer_managed_key(dict[str, Any], Optional): Combination of Key vault key id and user assigned id
+
+            * user_assigned_identity_id(str):
+                User Assigned Identity id
+            * key_vault_key_id(str):
+                The object identifier of the current versioned Key Vault Key in use.
+        identity(dict[str, Any], Optional): The identity of the resource.
+
+            * type(str):
+                The identity type. Possible values are SystemAssigned, UserAssigned, SystemAssigned, UserAssigned
+            * user_assigned_identities(dict[str, Any], Optional):
+                Key value pairs that describe the set of User Assigned identities that will be used with this storage account
+        network_rules(dict[str, Any], Optional): Network rule set
+
+            * default_action(str):
+                Specifies the default action of allow or deny when no other rules match. Valid options are Deny or Allow
+            * bypass(str, Optional):
+                Specifies whether traffic is bypassed for Logging/Metrics/AzureServices. Possible values are any combination of Logging|Metrics|AzureServices
+            * ip_rule_values(list, Optional):
+                List of IP or IP range in CIDR format. Only IPV4 address is allowed.
+            * virtual_network_subnet_ids(list, Optional):
+                A list of resource ids of virtual network subnets.
+            * resource_access_rules(dict[str, Any], Optional):
+                The resource access rules
         large_file_shares_state(str, Optional): Allow large file shares if sets to enable.
-        azure_files_authentication(Dict, Optional): Provides the identity based authentication settings for Azure Files.
+        azure_files_authentication(dict[str, Any], Optional): Provides the identity based authentication settings for Azure Files.
 
-            * directory_service_options(str): The directory service to be used. Possible values are AADDS, AD and AADKERB.
-            * active_directory_properties(Dict, Optional): Required if directoryServiceOptions are AD, optional if they are AADKERB.
-        routing(Dict, Optional): Maintains information about the network routing choice opted by the user for data transfer.
-
-            * publish_internet_endpoints(bool, Optional): A boolean flag which indicates whether internet routing storage endpoints are to be published.
-            * publish_microsoft_endpoints(bool, Optional): A boolean flag which indicates whether microsoft routing storage endpoints are to be published.
-            * routing_choice(str, Optional): Routing Choice defines the kind of network routing opted by the user.
-        encryption_service(Dict, Optional): Encryption details
-
-            * queue_encryption_key_type(str, Optional): The encryption type of the queue service.
-            * table_encryption_key_type(str, Optional): The encryption type of the table service.
-            * encryption_key_source(str, Optional): The encryption keySource (provider)
+            * directory_service_options(str):
+                The directory service to be used. Possible values are AADDS, AD and AADKERB.
+            * active_directory_properties(dict[str, Any], Optional):
+                Required if directoryServiceOptions are AD, optional if they are AADKERB.
+        routing(dict[str, Any], Optional): Maintains information about the network routing choice opted by the user for data transfer.
+
+            * publish_internet_endpoints(bool, Optional):
+                A boolean flag which indicates whether internet routing storage endpoints are to be published.
+            * publish_microsoft_endpoints(bool, Optional):
+                A boolean flag which indicates whether microsoft routing storage endpoints are to be published.
+            * routing_choice(str, Optional):
+                Routing Choice defines the kind of network routing opted by the user.
+        encryption_service(dict[str, Any], Optional): Encryption details
+
+            * queue_encryption_key_type(str, Optional):
+                The encryption type of the queue service.
+            * table_encryption_key_type(str, Optional):
+                The encryption type of the table service.
+            * encryption_key_source(str, Optional):
+                The encryption keySource (provider)
         require_infrastructure_encryption(bool, Optional): A boolean indicating whether or not the service applies a secondary layer of encryption with platform managed keys for data at rest.
-        immutability_policy(Dict, Optional): This argument specifies the default account-level immutability policy which is inherited and applied to objects.
+        immutability_policy(dict[str, Any], Optional): This argument specifies the default account-level immutability policy which is inherited and applied to objects.
 
-            * allow_protected_append_writes(bool): This property can only be changed for disabled and unlocked time-based retention policies. When enabled, new blocks can be written to an append blob while
+            * allow_protected_append_writes(bool):
+                This property can only be changed for disabled and unlocked time-based retention policies. When enabled, new blocks can be written to an append blob while
                 maintaining immutability protection and compliance. Only new blocks can be added and any existing blocks cannot be modified or deleted.
-            * state(str):Defines the mode of the policy. Disabled state disables the policy, Unlocked state
+            * state(str):
+                Defines the mode of the policy. Disabled state disables the policy, Unlocked state
                 allows increase and decrease of immutability retention time and also allows toggling allowProtectedAppendWrites property,
                 Locked state only allows the increase of the immutability retention time. A policy can only be created
                 in a Disabled or Unlocked state and can be toggled between the two states. Only a policy in an Unlocked
                 state can transition to a Locked state which cannot be reverted.
             * period_since_creation_in_days(int): The immutability period for the blobs in the container since the policy creation, in days.
-        sas_policy(Dict, Optional): SasPolicy assigned to the storage account.
+        sas_policy(dict[str, Any], Optional): SasPolicy assigned to the storage account.
 
-            * expiration_period(str, Optional): The SAS expiration period, DD.HH:MM:SS.
-            * expiration_action(str, Optional): The SAS expiration action. Valid value is Log.
+            * expiration_period(str, Optional):
+                The SAS expiration period, DD.HH:MM:SS.
+            * expiration_action(str, Optional):
+                The SAS expiration action. Valid value is Log.
 
         allowed_copy_scope(str, Optional): Restrict copy to and from Storage Accounts within an AAD tenant or with Private Links to the same VNet.
         sftp_enabled(bool, Optional): Enables Secure File Transfer Protocol, if set to true
-        tags(Dict, Optional): The resource tags.
+        tags(dict[str, str], Optional): The resource tags.
         subscription_id(str, Optional): Subscription Unique id.
         resource_id(str, Optional): Storage account resource id on Azure.
 
     Returns:
         dict
 
     Examples:
```

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/subscription/attach_subscriptions.py` & `idem-azure-0.3.2/idem_azure/states/azure/subscription/attach_subscriptions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/states/azure/subscription/subscriptions.py` & `idem-azure-0.3.2/idem_azure/states/azure/subscription/subscriptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,20 +31,21 @@
 
     Returns:
         Dict
 
     Examples:
         .. code-block:: sls
 
-        azure.subscription.subscriptions.present:
-            - name: create_subscription_3
-            - alias: dupSubTest
-            - billing_scope: /providers/Microsoft.Billing/billingAccounts/{billingAccountID}/enrollmentAccounts/{enrollmentAccountId}}
-            - display_name: Subscription Display Name
-            - workload: Production
+            resource_present:
+              azure.subscription.subscriptions.present:
+                - name: create_subscription_3
+                - alias: dupSubTest
+                - billing_scope: /providers/Microsoft.Billing/billingAccounts/{billingAccountID}/enrollmentAccounts/{enrollmentAccountId}}
+                - display_name: Subscription Display Name
+                - workload: Production
     """
     result = {
         "name": name,
         "result": True,
         "old_state": None,
         "new_state": None,
         "comment": [],
```

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/authorization/role_assignments.py` & `idem-azure-0.3.2/idem_azure/tool/azure/authorization/role_assignments.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/authorization/role_definitions.py` & `idem-azure-0.3.2/idem_azure/tool/azure/authorization/role_definitions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/compute/log_analytics_workspace.py` & `idem-azure-0.3.2/idem_azure/tool/azure/compute/log_analytics_workspace.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/compute/virtual_machines.py` & `idem-azure-0.3.2/idem_azure/tool/azure/compute/virtual_machines.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/container.py` & `idem-azure-0.3.2/idem_azure/tool/azure/container.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/management_groups/management_groups.py` & `idem-azure-0.3.2/idem_azure/tool/azure/management_groups/management_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/network/firewall.py` & `idem-azure-0.3.2/idem_azure/tool/azure/network/firewall.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/network/firewall_policies.py` & `idem-azure-0.3.2/idem_azure/tool/azure/network/firewall_policies.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/network/network_interfaces.py` & `idem-azure-0.3.2/idem_azure/tool/azure/network/network_interfaces.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/network/network_security_groups.py` & `idem-azure-0.3.2/idem_azure/tool/azure/network/network_security_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/network/public_ip_addresses.py` & `idem-azure-0.3.2/idem_azure/tool/azure/network/public_ip_addresses.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/network/route_tables.py` & `idem-azure-0.3.2/idem_azure/tool/azure/network/route_tables.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/network/routes.py` & `idem-azure-0.3.2/idem_azure/tool/azure/network/routes.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/network/security_rules.py` & `idem-azure-0.3.2/idem_azure/tool/azure/network/security_rules.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/network/subnets.py` & `idem-azure-0.3.2/idem_azure/tool/azure/network/subnets.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/network/virtual_networks.py` & `idem-azure-0.3.2/idem_azure/tool/azure/network/virtual_networks.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/policy/policy_assignment.py` & `idem-azure-0.3.2/idem_azure/tool/azure/policy/policy_assignment.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/policy/policy_definition.py` & `idem-azure-0.3.2/idem_azure/tool/azure/policy/policy_definition.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/request.py` & `idem-azure-0.3.2/idem_azure/tool/azure/request.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/resource_management/resource_groups.py` & `idem-azure-0.3.2/idem_azure/tool/azure/resource_management/resource_groups.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/storage_resource_provider/storage_accounts.py` & `idem-azure-0.3.2/idem_azure/tool/azure/storage_resource_provider/storage_accounts.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/subscription/subscriptions.py` & `idem-azure-0.3.2/idem_azure/tool/azure/subscription/subscriptions.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/test_state_utils.py` & `idem-azure-0.3.2/idem_azure/tool/azure/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/azure/uri.py` & `idem-azure-0.3.2/idem_azure/tool/azure/uri.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure/tool/validators/http.py` & `idem-azure-0.3.2/idem_azure/tool/validators/http.py`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/idem_azure.egg-info/PKG-INFO` & `idem-azure-0.3.2/idem_azure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-azure
-Version: 0.3.1
+Version: 0.3.2
 Summary: UNKNOWN
 Home-page: https://gitlab.com/vmware/idem/idem-azure
 Author: Yingzhi Hao
 Author-email: hyingzhi@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-azure-0.3.1/idem_azure.egg-info/SOURCES.txt` & `idem-azure-0.3.2/idem_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-azure-0.3.1/setup.py` & `idem-azure-0.3.2/setup.py`

 * *Files identical despite different names*

