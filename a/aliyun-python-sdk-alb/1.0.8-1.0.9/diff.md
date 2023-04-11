# Comparing `tmp/aliyun-python-sdk-alb-1.0.8.tar.gz` & `tmp/aliyun-python-sdk-alb-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-alb-1.0.8.tar", last modified: Tue Jan 25 12:31:00 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-alb-1.0.9.tar", last modified: Wed Mar 16 02:15:57 2022, max compression
```

## Comparing `aliyun-python-sdk-alb-1.0.8.tar` & `aliyun-python-sdk-alb-1.0.9.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      575 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyun_python_sdk_alb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyun_python_sdk_alb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5009 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyun_python_sdk_alb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyun_python_sdk_alb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyun_python_sdk_alb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyun_python_sdk_alb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/
--rw-r--r--   0 root         (0) root         (0)       21 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/
--rw-r--r--   0 root         (0) root         (0)     2266 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/AddEntriesToAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     3012 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/AddServersToServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2148 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ApplyHealthCheckTemplateToServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2251 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/AssociateAclsWithListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2239 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/AssociateAdditionalCertificatesWithListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2146 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/AttachCommonBandwidthPackageToLoadBalancerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2020 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     4622 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateHealthCheckTemplateRequest.py
--rw-r--r--   0 root         (0) root         (0)     8837 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     5367 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateLoadBalancerRequest.py
--rw-r--r--   0 root         (0) root         (0)    14338 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)    16021 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2602 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateSecurityPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     6630 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1787 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     1985 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteHealthCheckTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1827 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1859 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteLoadBalancerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1795 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1879 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1875 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteSecurityPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1851 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1487 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1268 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DescribeZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2150 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DetachCommonBandwidthPackageFromLoadBalancerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1849 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DisableDeletionProtectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1879 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DisableLoadBalancerAccessLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2080 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DissociateAclsFromListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2241 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DissociateAdditionalCertificatesFromListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1847 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/EnableDeletionProtectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2247 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/EnableLoadBalancerAccessLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1561 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/GetHealthCheckTemplateAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1473 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/GetListenerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2050 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/GetListenerHealthStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1505 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/GetLoadBalancerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1809 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListAclEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1503 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListAclRelationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2327 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListAclsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2852 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListAsynJobsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2330 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListHealthCheckTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2080 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListListenerCertificatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2415 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListListenersRequest.py
--rw-r--r--   0 root         (0) root         (0)     4145 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListLoadBalancersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2415 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2483 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListSecurityPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1591 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListSecurityPolicyRelationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2514 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListServerGroupServersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2994 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListServerGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1294 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListSystemSecurityPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2197 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListTagKeysRequest.py
--rw-r--r--   0 root         (0) root         (0)     2502 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2207 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListTagValuesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1909 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/MoveResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2044 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/RemoveEntriesFromAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     2587 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/RemoveServersFromServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     3857 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ReplaceServersInServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1825 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/StartListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     1823 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/StopListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2116 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2349 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UnTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1978 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateAclAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     4897 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateHealthCheckTemplateAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     8399 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateListenerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2917 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateListenerLogConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2720 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateLoadBalancerAddressTypeConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2657 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateLoadBalancerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2118 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateLoadBalancerEditionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2501 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateLoadBalancerZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)    14332 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateRuleAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)    15839 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateRulesAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2626 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateSecurityPolicyAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     6075 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateServerGroupAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2874 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateServerGroupServersAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2022-01-25 12:31:00.000000 aliyun-python-sdk-alb-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyun_python_sdk_alb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyun_python_sdk_alb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5009 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyun_python_sdk_alb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyun_python_sdk_alb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyun_python_sdk_alb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyun_python_sdk_alb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/
+-rw-r--r--   0 root         (0) root         (0)     2266 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/AddEntriesToAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3012 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/AddServersToServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ApplyHealthCheckTemplateToServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/AssociateAclsWithListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/AssociateAdditionalCertificatesWithListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/AttachCommonBandwidthPackageToLoadBalancerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2020 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateHealthCheckTemplateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     8837 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5367 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateLoadBalancerRequest.py
+-rw-r--r--   0 root         (0) root         (0)    14338 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)    16021 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateSecurityPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6630 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteHealthCheckTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteLoadBalancerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1875 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteSecurityPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DescribeZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DetachCommonBandwidthPackageFromLoadBalancerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DisableDeletionProtectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1879 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DisableLoadBalancerAccessLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DissociateAclsFromListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DissociateAdditionalCertificatesFromListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/EnableDeletionProtectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/EnableLoadBalancerAccessLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1561 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/GetHealthCheckTemplateAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/GetListenerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/GetListenerHealthStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/GetLoadBalancerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1809 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListAclEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1503 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListAclRelationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListAclsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2852 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListAsynJobsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListHealthCheckTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListListenerCertificatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListListenersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4145 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListLoadBalancersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListSecurityPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListSecurityPolicyRelationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2514 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListServerGroupServersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2994 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListServerGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1294 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListSystemSecurityPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2197 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListTagKeysRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListTagValuesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/MoveResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/RemoveEntriesFromAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2587 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/RemoveServersFromServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3857 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ReplaceServersInServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/StartListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1823 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/StopListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2349 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UnTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateAclAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4897 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateHealthCheckTemplateAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     8399 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateListenerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateListenerLogConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateLoadBalancerAddressTypeConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateLoadBalancerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2118 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateLoadBalancerEditionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateLoadBalancerZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)    14332 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateRuleAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)    15839 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateRulesAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateSecurityPolicyAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6075 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateServerGroupAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateServerGroupServersAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2022-03-16 02:15:57.000000 aliyun-python-sdk-alb-1.0.9/setup.py
```

### Comparing `aliyun-python-sdk-alb-1.0.8/LICENSE` & `aliyun-python-sdk-alb-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/PKG-INFO` & `aliyun-python-sdk-alb-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-alb
-Version: 1.0.8
+Version: 1.0.9
 Summary: The alb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-alb
```

### Comparing `aliyun-python-sdk-alb-1.0.8/README.rst` & `aliyun-python-sdk-alb-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyun_python_sdk_alb.egg-info/PKG-INFO` & `aliyun-python-sdk-alb-1.0.9/aliyun_python_sdk_alb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-alb
-Version: 1.0.8
+Version: 1.0.9
 Summary: The alb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-alb
```

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyun_python_sdk_alb.egg-info/SOURCES.txt` & `aliyun-python-sdk-alb-1.0.9/aliyun_python_sdk_alb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/endpoint.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/AddEntriesToAclRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/AddEntriesToAclRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/AddServersToServerGroupRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/AddServersToServerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ApplyHealthCheckTemplateToServerGroupRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ApplyHealthCheckTemplateToServerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/AssociateAclsWithListenerRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/AssociateAclsWithListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/AssociateAdditionalCertificatesWithListenerRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/AssociateAdditionalCertificatesWithListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/AttachCommonBandwidthPackageToLoadBalancerRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/AttachCommonBandwidthPackageToLoadBalancerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateAclRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateAclRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateHealthCheckTemplateRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateHealthCheckTemplateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateListenerRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateLoadBalancerRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateLoadBalancerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateRuleRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateRulesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateSecurityPolicyRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateSecurityPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/CreateServerGroupRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/CreateServerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteAclRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteAclRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteHealthCheckTemplatesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteHealthCheckTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteListenerRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteLoadBalancerRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteLoadBalancerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteRuleRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteRulesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteSecurityPolicyRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteSecurityPolicyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DeleteServerGroupRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DeleteServerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DescribeRegionsRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DescribeZonesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DescribeZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DetachCommonBandwidthPackageFromLoadBalancerRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DetachCommonBandwidthPackageFromLoadBalancerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DisableDeletionProtectionRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DisableDeletionProtectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DisableLoadBalancerAccessLogRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DisableLoadBalancerAccessLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DissociateAclsFromListenerRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DissociateAclsFromListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/DissociateAdditionalCertificatesFromListenerRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/DissociateAdditionalCertificatesFromListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/EnableDeletionProtectionRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/EnableDeletionProtectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/EnableLoadBalancerAccessLogRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/EnableLoadBalancerAccessLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/GetHealthCheckTemplateAttributeRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/GetHealthCheckTemplateAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/GetListenerAttributeRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/GetListenerAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/GetListenerHealthStatusRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/GetListenerHealthStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/GetLoadBalancerAttributeRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/GetLoadBalancerAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListAclEntriesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListAclEntriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListAclRelationsRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListAclRelationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListAclsRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListAclsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListAsynJobsRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListAsynJobsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListHealthCheckTemplatesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListHealthCheckTemplatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListListenerCertificatesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListListenerCertificatesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListListenersRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListListenersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListLoadBalancersRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListLoadBalancersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListRulesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListSecurityPoliciesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListSecurityPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListSecurityPolicyRelationsRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListSecurityPolicyRelationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListServerGroupServersRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListServerGroupServersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListServerGroupsRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListServerGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListSystemSecurityPoliciesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListSystemSecurityPoliciesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListTagKeysRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListTagKeysRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListTagResourcesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ListTagValuesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ListTagValuesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/MoveResourceGroupRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/MoveResourceGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/RemoveEntriesFromAclRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/RemoveEntriesFromAclRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/RemoveServersFromServerGroupRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/RemoveServersFromServerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/ReplaceServersInServerGroupRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/ReplaceServersInServerGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/StartListenerRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/StartListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/StopListenerRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/StopListenerRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/TagResourcesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UnTagResourcesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UnTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateAclAttributeRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateAclAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateHealthCheckTemplateAttributeRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateHealthCheckTemplateAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateListenerAttributeRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateListenerAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateListenerLogConfigRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateListenerLogConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateLoadBalancerAddressTypeConfigRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateLoadBalancerAddressTypeConfigRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateLoadBalancerAttributeRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateLoadBalancerAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateLoadBalancerEditionRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateLoadBalancerEditionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateLoadBalancerZonesRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateLoadBalancerZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateRuleAttributeRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateRuleAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateRulesAttributeRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateRulesAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateSecurityPolicyAttributeRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateSecurityPolicyAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateServerGroupAttributeRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateServerGroupAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/aliyunsdkalb/request/v20200616/UpdateServerGroupServersAttributeRequest.py` & `aliyun-python-sdk-alb-1.0.9/aliyunsdkalb/request/v20200616/UpdateServerGroupServersAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alb-1.0.8/setup.py` & `aliyun-python-sdk-alb-1.0.9/setup.py`

 * *Files identical despite different names*

