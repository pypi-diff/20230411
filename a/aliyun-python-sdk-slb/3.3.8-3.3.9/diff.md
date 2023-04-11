# Comparing `tmp/aliyun-python-sdk-slb-3.3.8.tar.gz` & `tmp/aliyun-python-sdk-slb-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-slb-3.3.8.tar", last modified: Wed Jul 21 03:12:33 2021, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-slb-3.3.9.tar", last modified: Wed Dec 29 10:10:16 2021, max compression
```

## Comparing `aliyun-python-sdk-slb-3.3.8.tar` & `aliyun-python-sdk-slb-3.3.9.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/
--rw-r--r--   0 root         (0) root         (0)      575 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1537 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      527 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyun_python_sdk_slb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1537 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyun_python_sdk_slb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6065 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyun_python_sdk_slb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyun_python_sdk_slb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyun_python_sdk_slb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyun_python_sdk_slb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/
--rw-r--r--   0 root         (0) root         (0)       21 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3020 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/
--rw-r--r--   0 root         (0) root         (0)     2368 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/AddAccessControlListEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2436 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/AddBackendServersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2824 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/AddListenerWhiteListItemRequest.py
--rw-r--r--   0 root         (0) root         (0)     2356 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/AddTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2460 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/AddVServerGroupBackendServersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2620 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateAccessControlListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2806 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateDomainExtensionRequest.py
--rw-r--r--   0 root         (0) root         (0)     8478 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateLoadBalancerHTTPListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     8908 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateLoadBalancerHTTPSListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     5858 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateLoadBalancerRequest.py
--rw-r--r--   0 root         (0) root         (0)     6970 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateLoadBalancerTCPListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     5638 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateLoadBalancerUDPListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2792 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateMasterSlaveServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2780 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2942 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateTLSCipherPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2646 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateVServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2198 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteAccessControlListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2250 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteCACertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2266 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteDomainExtensionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2650 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteLoadBalancerListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2242 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteLoadBalancerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2322 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteMasterSlaveServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2186 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2282 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteServerCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2456 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteTLSCipherPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2242 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteVServerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2422 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeAccessControlListAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2958 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeAccessControlListsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2446 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeAvailableResourceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2458 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeCACertificatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2288 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeDomainExtensionAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2652 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeDomainExtensionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2638 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeHealthStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2674 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeListenerAccessControlAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2264 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeLoadBalancerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2472 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeLoadBalancerHTTPListenerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2474 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeLoadBalancerHTTPSListenerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2936 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeLoadBalancerListenersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2470 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeLoadBalancerTCPListenerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2470 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeLoadBalancerUDPListenerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     5506 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeLoadBalancersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2344 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeMasterSlaveServerGroupAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2470 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeMasterSlaveServerGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2236 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2200 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeRuleAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2624 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2490 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeServerCertificatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2876 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2264 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeVServerGroupAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2628 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeVServerGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2036 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3120 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/ListTLSCipherPoliciesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3082 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2628 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/ModifyLoadBalancerInstanceSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     2806 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/ModifyLoadBalancerInternetSpecRequest.py
--rw-r--r--   0 root         (0) root         (0)     2908 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/ModifyLoadBalancerPayTypeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2698 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/ModifyVServerGroupBackendServersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2374 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/RemoveAccessControlListEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2442 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/RemoveBackendServersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2830 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/RemoveListenerWhiteListItemRequest.py
--rw-r--r--   0 root         (0) root         (0)     2362 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/RemoveTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2466 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/RemoveVServerGroupBackendServersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2364 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetAccessControlListAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2436 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetBackendServersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2466 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetCACertificateNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     2504 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetDomainExtensionAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2884 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetListenerAccessControlStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2476 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetLoadBalancerDeleteProtectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     8080 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetLoadBalancerHTTPListenerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     8890 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetLoadBalancerHTTPSListenerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2840 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetLoadBalancerModificationProtectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2452 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetLoadBalancerNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     2468 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetLoadBalancerStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     7356 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetLoadBalancerTCPListenerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     5864 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetLoadBalancerUDPListenerAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     5552 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2522 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetServerCertificateNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     3168 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetTLSCipherPolicyAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2658 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetVServerGroupAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2648 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/StartLoadBalancerListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2646 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/StopLoadBalancerListenerRequest.py
--rw-r--r--   0 root         (0) root         (0)     2908 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2900 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2654 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/UploadCACertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     3644 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/UploadServerCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2452 2021-07-21 03:12:33.000000 aliyun-python-sdk-slb-3.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/
+-rw-r--r--   0 root         (0) root         (0)      575 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1537 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyun_python_sdk_slb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1537 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyun_python_sdk_slb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6065 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyun_python_sdk_slb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyun_python_sdk_slb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyun_python_sdk_slb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyun_python_sdk_slb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/
+-rw-r--r--   0 root         (0) root         (0)       21 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3020 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/
+-rw-r--r--   0 root         (0) root         (0)     2478 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/AddAccessControlListEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/AddBackendServersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/AddListenerWhiteListItemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/AddTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2570 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/AddVServerGroupBackendServersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2749 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateAccessControlListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateDomainExtensionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     9201 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateLoadBalancerHTTPListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     9667 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateLoadBalancerHTTPSListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6316 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateLoadBalancerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7520 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateLoadBalancerTCPListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6068 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateLoadBalancerUDPListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateMasterSlaveServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateTLSCipherPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2775 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateVServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2289 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteAccessControlListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2341 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteCACertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2357 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteDomainExtensionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2781 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteLoadBalancerListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteLoadBalancerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteMasterSlaveServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2373 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteServerCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteTLSCipherPolicyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteVServerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2532 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeAccessControlListAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3129 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeAccessControlListsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeAvailableResourceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeCACertificatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2379 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeDomainExtensionAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeDomainExtensionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeHealthStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2805 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeListenerAccessControlAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2584 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancerHTTPListenerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancerHTTPSListenerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancerListenersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancerTCPListenerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancerUDPListenerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5943 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeMasterSlaveServerGroupAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeMasterSlaveServerGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2327 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2291 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeRuleAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2755 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeServerCertificatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3049 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeVServerGroupAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2761 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeVServerGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/ListTLSCipherPoliciesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/ModifyLoadBalancerInstanceSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/ModifyLoadBalancerInternetSpecRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3079 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/ModifyLoadBalancerPayTypeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/ModifyVServerGroupBackendServersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/RemoveAccessControlListEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2552 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/RemoveBackendServersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2980 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/RemoveListenerWhiteListItemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/RemoveTagsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2576 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/RemoveVServerGroupBackendServersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2474 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetAccessControlListAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetBackendServersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2576 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetCACertificateNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2614 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetDomainExtensionAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3034 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetListenerAccessControlStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerDeleteProtectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     8761 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerHTTPListenerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     9647 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerHTTPSListenerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerModificationProtectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7942 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerTCPListenerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6311 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerUDPListenerAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5978 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetServerCertificateNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3259 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetTLSCipherPolicyAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetVServerGroupAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/StartLoadBalancerListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2777 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/StopLoadBalancerListenerRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2976 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/UploadCACertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3849 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/UploadServerCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2021-12-29 10:10:16.000000 aliyun-python-sdk-slb-3.3.9/setup.py
```

### Comparing `aliyun-python-sdk-slb-3.3.8/LICENSE` & `aliyun-python-sdk-slb-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-slb-3.3.8/PKG-INFO` & `aliyun-python-sdk-slb-3.3.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-slb
-Version: 3.3.8
+Version: 3.3.9
 Summary: The slb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-slb
```

### Comparing `aliyun-python-sdk-slb-3.3.8/README.rst` & `aliyun-python-sdk-slb-3.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyun_python_sdk_slb.egg-info/PKG-INFO` & `aliyun-python-sdk-slb-3.3.9/aliyun_python_sdk_slb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-slb
-Version: 3.3.8
+Version: 3.3.9
 Summary: The slb module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-slb
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyun_python_sdk_slb.egg-info/SOURCES.txt` & `aliyun-python-sdk-slb-3.3.9/aliyun_python_sdk_slb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/endpoint.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/AddAccessControlListEntryRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeVServerGroupAttributeRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,53 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class AddAccessControlListEntryRequest(RpcRequest):
+class DescribeVServerGroupAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'AddAccessControlListEntry','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeVServerGroupAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_AclEntrys(self):
-		return self.get_query_params().get('AclEntrys')
-
-	def set_AclEntrys(self,AclEntrys):
-		self.add_query_param('AclEntrys',AclEntrys)
-
-	def get_AclId(self):
-		return self.get_query_params().get('AclId')
-
-	def set_AclId(self,AclId):
-		self.add_query_param('AclId',AclId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_VServerGroupId(self): # String
+		return self.get_query_params().get('VServerGroupId')
+
+	def set_VServerGroupId(self, VServerGroupId):  # String
+		self.add_query_param('VServerGroupId', VServerGroupId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/AddBackendServersRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/RemoveBackendServersRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class AddBackendServersRequest(RpcRequest):
+class RemoveBackendServersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'AddBackendServers','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'RemoveBackendServers','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_BackendServers(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_BackendServers(self): # String
 		return self.get_query_params().get('BackendServers')
 
-	def set_BackendServers(self,BackendServers):
-		self.add_query_param('BackendServers',BackendServers)
-
-	def get_ResourceOwnerAccount(self):
+	def set_BackendServers(self, BackendServers):  # String
+		self.add_query_param('BackendServers', BackendServers)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/AddListenerWhiteListItemRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeMasterSlaveServerGroupsRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,65 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class AddListenerWhiteListItemRequest(RpcRequest):
+class DescribeMasterSlaveServerGroupsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'AddListenerWhiteListItem','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeMasterSlaveServerGroups','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_SourceItems(self):
-		return self.get_query_params().get('SourceItems')
-
-	def set_SourceItems(self,SourceItems):
-		self.add_query_param('SourceItems',SourceItems)
-
-	def get_ListenerPort(self):
-		return self.get_query_params().get('ListenerPort')
-
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_IncludeListener(self): # Boolean
+		return self.get_query_params().get('IncludeListener')
+
+	def set_IncludeListener(self, IncludeListener):  # Boolean
+		self.add_query_param('IncludeListener', IncludeListener)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ListenerProtocol(self):
-		return self.get_query_params().get('ListenerProtocol')
-
-	def set_ListenerProtocol(self,ListenerProtocol):
-		self.add_query_param('ListenerProtocol',ListenerProtocol)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/AddTagsRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/ModifyLoadBalancerInternetSpecRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,53 +16,58 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class AddTagsRequest(RpcRequest):
+class ModifyLoadBalancerInternetSpecRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'AddTags','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'ModifyLoadBalancerInternetSpec','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_AutoPay(self): # Boolean
+		return self.get_query_params().get('AutoPay')
+
+	def set_AutoPay(self, AutoPay):  # Boolean
+		self.add_query_param('AutoPay', AutoPay)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_Bandwidth(self): # Integer
+		return self.get_query_params().get('Bandwidth')
+
+	def set_Bandwidth(self, Bandwidth):  # Integer
+		self.add_query_param('Bandwidth', Bandwidth)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_Tags(self):
-		return self.get_query_params().get('Tags')
-
-	def set_Tags(self,Tags):
-		self.add_query_param('Tags',Tags)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
+	def get_InternetChargeType(self): # String
+		return self.get_query_params().get('InternetChargeType')
+
+	def set_InternetChargeType(self, InternetChargeType):  # String
+		self.add_query_param('InternetChargeType', InternetChargeType)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/AddVServerGroupBackendServersRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateRulesRequest.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,53 +16,58 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class AddVServerGroupBackendServersRequest(RpcRequest):
+class CreateRulesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'AddVServerGroupBackendServers','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateRules','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_BackendServers(self):
-		return self.get_query_params().get('BackendServers')
-
-	def set_BackendServers(self,BackendServers):
-		self.add_query_param('BackendServers',BackendServers)
-
-	def get_VServerGroupId(self):
-		return self.get_query_params().get('VServerGroupId')
-
-	def set_VServerGroupId(self,VServerGroupId):
-		self.add_query_param('VServerGroupId',VServerGroupId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_RuleList(self): # String
+		return self.get_query_params().get('RuleList')
+
+	def set_RuleList(self, RuleList):  # String
+		self.add_query_param('RuleList', RuleList)
+	def get_ListenerPort(self): # Integer
+		return self.get_query_params().get('ListenerPort')
+
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ListenerProtocol(self): # String
+		return self.get_query_params().get('ListenerProtocol')
+
+	def set_ListenerProtocol(self, ListenerProtocol):  # String
+		self.add_query_param('ListenerProtocol', ListenerProtocol)
+	def get_LoadBalancerId(self): # String
+		return self.get_query_params().get('LoadBalancerId')
+
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateAccessControlListRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancerTCPListenerAttributeRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,59 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class CreateAccessControlListRequest(RpcRequest):
+class DescribeLoadBalancerTCPListenerAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateAccessControlList','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeLoadBalancerTCPListenerAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_AclName(self):
-		return self.get_query_params().get('AclName')
-
-	def set_AclName(self,AclName):
-		self.add_query_param('AclName',AclName)
-
-	def get_AddressIPVersion(self):
-		return self.get_query_params().get('AddressIPVersion')
-
-	def set_AddressIPVersion(self,AddressIPVersion):
-		self.add_query_param('AddressIPVersion',AddressIPVersion)
-
-	def get_ResourceGroupId(self):
-		return self.get_query_params().get('ResourceGroupId')
-
-	def set_ResourceGroupId(self,ResourceGroupId):
-		self.add_query_param('ResourceGroupId',ResourceGroupId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ListenerPort(self): # Integer
+		return self.get_query_params().get('ListenerPort')
+
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
+		return self.get_query_params().get('LoadBalancerId')
+
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateDomainExtensionRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateDomainExtensionRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,62 +19,55 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class CreateDomainExtensionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateDomainExtension','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateDomainExtension','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ListenerPort(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ListenerPort(self): # Integer
 		return self.get_query_params().get('ListenerPort')
 
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ServerCertificateId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ServerCertificateId(self): # String
 		return self.get_query_params().get('ServerCertificateId')
 
-	def set_ServerCertificateId(self,ServerCertificateId):
-		self.add_query_param('ServerCertificateId',ServerCertificateId)
-
-	def get_LoadBalancerId(self):
+	def set_ServerCertificateId(self, ServerCertificateId):  # String
+		self.add_query_param('ServerCertificateId', ServerCertificateId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
-
-	def get_Domain(self):
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
+	def get_Domain(self): # String
 		return self.get_query_params().get('Domain')
 
-	def set_Domain(self,Domain):
-		self.add_query_param('Domain',Domain)
+	def set_Domain(self, Domain):  # String
+		self.add_query_param('Domain', Domain)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateLoadBalancerHTTPListenerRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerTCPListenerAttributeRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,239 +16,168 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class CreateLoadBalancerHTTPListenerRequest(RpcRequest):
+class SetLoadBalancerTCPListenerAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateLoadBalancerHTTPListener','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetLoadBalancerTCPListenerAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_HealthCheckTimeout(self):
-		return self.get_query_params().get('HealthCheckTimeout')
-
-	def set_HealthCheckTimeout(self,HealthCheckTimeout):
-		self.add_query_param('HealthCheckTimeout',HealthCheckTimeout)
-
-	def get_ListenerForward(self):
-		return self.get_query_params().get('ListenerForward')
-
-	def set_ListenerForward(self,ListenerForward):
-		self.add_query_param('ListenerForward',ListenerForward)
-
-	def get_XForwardedFor(self):
-		return self.get_query_params().get('XForwardedFor')
-
-	def set_XForwardedFor(self,XForwardedFor):
-		self.add_query_param('XForwardedFor',XForwardedFor)
-
-	def get_HealthCheckURI(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_HealthCheckURI(self): # String
 		return self.get_query_params().get('HealthCheckURI')
 
-	def set_HealthCheckURI(self,HealthCheckURI):
-		self.add_query_param('HealthCheckURI',HealthCheckURI)
-
-	def get_AclStatus(self):
+	def set_HealthCheckURI(self, HealthCheckURI):  # String
+		self.add_query_param('HealthCheckURI', HealthCheckURI)
+	def get_AclStatus(self): # String
 		return self.get_query_params().get('AclStatus')
 
-	def set_AclStatus(self,AclStatus):
-		self.add_query_param('AclStatus',AclStatus)
-
-	def get_AclType(self):
+	def set_AclStatus(self, AclStatus):  # String
+		self.add_query_param('AclStatus', AclStatus)
+	def get_AclType(self): # String
 		return self.get_query_params().get('AclType')
 
-	def set_AclType(self,AclType):
-		self.add_query_param('AclType',AclType)
-
-	def get_HealthCheck(self):
-		return self.get_query_params().get('HealthCheck')
-
-	def set_HealthCheck(self,HealthCheck):
-		self.add_query_param('HealthCheck',HealthCheck)
-
-	def get_VServerGroupId(self):
+	def set_AclType(self, AclType):  # String
+		self.add_query_param('AclType', AclType)
+	def get_MasterSlaveServerGroup(self): # String
+		return self.get_query_params().get('MasterSlaveServerGroup')
+
+	def set_MasterSlaveServerGroup(self, MasterSlaveServerGroup):  # String
+		self.add_query_param('MasterSlaveServerGroup', MasterSlaveServerGroup)
+	def get_EstablishedTimeout(self): # Integer
+		return self.get_query_params().get('EstablishedTimeout')
+
+	def set_EstablishedTimeout(self, EstablishedTimeout):  # Integer
+		self.add_query_param('EstablishedTimeout', EstablishedTimeout)
+	def get_PersistenceTimeout(self): # Integer
+		return self.get_query_params().get('PersistenceTimeout')
+
+	def set_PersistenceTimeout(self, PersistenceTimeout):  # Integer
+		self.add_query_param('PersistenceTimeout', PersistenceTimeout)
+	def get_VServerGroupId(self): # String
 		return self.get_query_params().get('VServerGroupId')
 
-	def set_VServerGroupId(self,VServerGroupId):
-		self.add_query_param('VServerGroupId',VServerGroupId)
-
-	def get_AclId(self):
+	def set_VServerGroupId(self, VServerGroupId):  # String
+		self.add_query_param('VServerGroupId', VServerGroupId)
+	def get_AclId(self): # String
 		return self.get_query_params().get('AclId')
 
-	def set_AclId(self,AclId):
-		self.add_query_param('AclId',AclId)
-
-	def get_Cookie(self):
-		return self.get_query_params().get('Cookie')
-
-	def set_Cookie(self,Cookie):
-		self.add_query_param('Cookie',Cookie)
-
-	def get_HealthCheckMethod(self):
-		return self.get_query_params().get('HealthCheckMethod')
-
-	def set_HealthCheckMethod(self,HealthCheckMethod):
-		self.add_query_param('HealthCheckMethod',HealthCheckMethod)
-
-	def get_HealthCheckDomain(self):
+	def set_AclId(self, AclId):  # String
+		self.add_query_param('AclId', AclId)
+	def get_HealthCheckDomain(self): # String
 		return self.get_query_params().get('HealthCheckDomain')
 
-	def set_HealthCheckDomain(self,HealthCheckDomain):
-		self.add_query_param('HealthCheckDomain',HealthCheckDomain)
-
-	def get_RequestTimeout(self):
-		return self.get_query_params().get('RequestTimeout')
-
-	def set_RequestTimeout(self,RequestTimeout):
-		self.add_query_param('RequestTimeout',RequestTimeout)
-
-	def get_OwnerId(self):
+	def set_HealthCheckDomain(self, HealthCheckDomain):  # String
+		self.add_query_param('HealthCheckDomain', HealthCheckDomain)
+	def get_SynProxy(self): # String
+		return self.get_query_params().get('SynProxy')
+
+	def set_SynProxy(self, SynProxy):  # String
+		self.add_query_param('SynProxy', SynProxy)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
-
-	def get_XForwardedFor_SLBIP(self):
-		return self.get_query_params().get('XForwardedFor_SLBIP')
-
-	def set_XForwardedFor_SLBIP(self,XForwardedFor_SLBIP):
-		self.add_query_param('XForwardedFor_SLBIP',XForwardedFor_SLBIP)
-
-	def get_BackendServerPort(self):
-		return self.get_query_params().get('BackendServerPort')
-
-	def set_BackendServerPort(self,BackendServerPort):
-		self.add_query_param('BackendServerPort',BackendServerPort)
-
-	def get_HealthCheckInterval(self):
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
+	def get_MasterSlaveServerGroupId(self): # String
+		return self.get_query_params().get('MasterSlaveServerGroupId')
+
+	def set_MasterSlaveServerGroupId(self, MasterSlaveServerGroupId):  # String
+		self.add_query_param('MasterSlaveServerGroupId', MasterSlaveServerGroupId)
+	def get_HealthCheckInterval(self): # Integer
 		return self.get_query_params().get('HealthCheckInterval')
 
-	def set_HealthCheckInterval(self,HealthCheckInterval):
-		self.add_query_param('HealthCheckInterval',HealthCheckInterval)
-
-	def get_XForwardedFor_SLBID(self):
-		return self.get_query_params().get('XForwardedFor_SLBID')
-
-	def set_XForwardedFor_SLBID(self,XForwardedFor_SLBID):
-		self.add_query_param('XForwardedFor_SLBID',XForwardedFor_SLBID)
-
-	def get_Description(self):
+	def set_HealthCheckInterval(self, HealthCheckInterval):  # Integer
+		self.add_query_param('HealthCheckInterval', HealthCheckInterval)
+	def get_ConnectionDrain(self): # String
+		return self.get_query_params().get('ConnectionDrain')
+
+	def set_ConnectionDrain(self, ConnectionDrain):  # String
+		self.add_query_param('ConnectionDrain', ConnectionDrain)
+	def get_HealthCheckConnectTimeout(self): # Integer
+		return self.get_query_params().get('HealthCheckConnectTimeout')
+
+	def set_HealthCheckConnectTimeout(self, HealthCheckConnectTimeout):  # Integer
+		self.add_query_param('HealthCheckConnectTimeout', HealthCheckConnectTimeout)
+	def get_Description(self): # String
 		return self.get_query_params().get('Description')
 
-	def set_Description(self,Description):
-		self.add_query_param('Description',Description)
-
-	def get_UnhealthyThreshold(self):
+	def set_Description(self, Description):  # String
+		self.add_query_param('Description', Description)
+	def get_UnhealthyThreshold(self): # Integer
 		return self.get_query_params().get('UnhealthyThreshold')
 
-	def set_UnhealthyThreshold(self,UnhealthyThreshold):
-		self.add_query_param('UnhealthyThreshold',UnhealthyThreshold)
-
-	def get_HealthyThreshold(self):
+	def set_UnhealthyThreshold(self, UnhealthyThreshold):  # Integer
+		self.add_query_param('UnhealthyThreshold', UnhealthyThreshold)
+	def get_HealthyThreshold(self): # Integer
 		return self.get_query_params().get('HealthyThreshold')
 
-	def set_HealthyThreshold(self,HealthyThreshold):
-		self.add_query_param('HealthyThreshold',HealthyThreshold)
-
-	def get_Scheduler(self):
+	def set_HealthyThreshold(self, HealthyThreshold):  # Integer
+		self.add_query_param('HealthyThreshold', HealthyThreshold)
+	def get_Scheduler(self): # String
 		return self.get_query_params().get('Scheduler')
 
-	def set_Scheduler(self,Scheduler):
-		self.add_query_param('Scheduler',Scheduler)
-
-	def get_ForwardPort(self):
-		return self.get_query_params().get('ForwardPort')
-
-	def set_ForwardPort(self,ForwardPort):
-		self.add_query_param('ForwardPort',ForwardPort)
-
-	def get_CookieTimeout(self):
-		return self.get_query_params().get('CookieTimeout')
-
-	def set_CookieTimeout(self,CookieTimeout):
-		self.add_query_param('CookieTimeout',CookieTimeout)
-
-	def get_StickySessionType(self):
-		return self.get_query_params().get('StickySessionType')
-
-	def set_StickySessionType(self,StickySessionType):
-		self.add_query_param('StickySessionType',StickySessionType)
-
-	def get_ListenerPort(self):
+	def set_Scheduler(self, Scheduler):  # String
+		self.add_query_param('Scheduler', Scheduler)
+	def get_ListenerPort(self): # Integer
 		return self.get_query_params().get('ListenerPort')
 
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_HealthCheckType(self): # String
+		return self.get_query_params().get('HealthCheckType')
+
+	def set_HealthCheckType(self, HealthCheckType):  # String
+		self.add_query_param('HealthCheckType', HealthCheckType)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_Bandwidth(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_Bandwidth(self): # Integer
 		return self.get_query_params().get('Bandwidth')
 
-	def set_Bandwidth(self,Bandwidth):
-		self.add_query_param('Bandwidth',Bandwidth)
-
-	def get_StickySession(self):
-		return self.get_query_params().get('StickySession')
-
-	def set_StickySession(self,StickySession):
-		self.add_query_param('StickySession',StickySession)
-
-	def get_OwnerAccount(self):
+	def set_Bandwidth(self, Bandwidth):  # Integer
+		self.add_query_param('Bandwidth', Bandwidth)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_Gzip(self):
-		return self.get_query_params().get('Gzip')
-
-	def set_Gzip(self,Gzip):
-		self.add_query_param('Gzip',Gzip)
-
-	def get_IdleTimeout(self):
-		return self.get_query_params().get('IdleTimeout')
-
-	def set_IdleTimeout(self,IdleTimeout):
-		self.add_query_param('IdleTimeout',IdleTimeout)
-
-	def get_XForwardedFor_proto(self):
-		return self.get_query_params().get('XForwardedFor_proto')
-
-	def set_XForwardedFor_proto(self,XForwardedFor_proto):
-		self.add_query_param('XForwardedFor_proto',XForwardedFor_proto)
-
-	def get_HealthCheckConnectPort(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_ConnectionDrainTimeout(self): # Integer
+		return self.get_query_params().get('ConnectionDrainTimeout')
+
+	def set_ConnectionDrainTimeout(self, ConnectionDrainTimeout):  # Integer
+		self.add_query_param('ConnectionDrainTimeout', ConnectionDrainTimeout)
+	def get_HealthCheckConnectPort(self): # Integer
 		return self.get_query_params().get('HealthCheckConnectPort')
 
-	def set_HealthCheckConnectPort(self,HealthCheckConnectPort):
-		self.add_query_param('HealthCheckConnectPort',HealthCheckConnectPort)
-
-	def get_HealthCheckHttpCode(self):
+	def set_HealthCheckConnectPort(self, HealthCheckConnectPort):  # Integer
+		self.add_query_param('HealthCheckConnectPort', HealthCheckConnectPort)
+	def get_HealthCheckHttpCode(self): # String
 		return self.get_query_params().get('HealthCheckHttpCode')
 
-	def set_HealthCheckHttpCode(self,HealthCheckHttpCode):
-		self.add_query_param('HealthCheckHttpCode',HealthCheckHttpCode)
+	def set_HealthCheckHttpCode(self, HealthCheckHttpCode):  # String
+		self.add_query_param('HealthCheckHttpCode', HealthCheckHttpCode)
+	def get_VServerGroup(self): # String
+		return self.get_query_params().get('VServerGroup')
+
+	def set_VServerGroup(self, VServerGroup):  # String
+		self.add_query_param('VServerGroup', VServerGroup)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateLoadBalancerRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancersRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,161 +16,133 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class CreateLoadBalancerRequest(RpcRequest):
+class DescribeLoadBalancersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateLoadBalancer','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeLoadBalancers','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_AddressIPVersion(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_NetworkType(self): # String
+		return self.get_query_params().get('NetworkType')
+
+	def set_NetworkType(self, NetworkType):  # String
+		self.add_query_param('NetworkType', NetworkType)
+	def get_AddressIPVersion(self): # String
 		return self.get_query_params().get('AddressIPVersion')
 
-	def set_AddressIPVersion(self,AddressIPVersion):
-		self.add_query_param('AddressIPVersion',AddressIPVersion)
-
-	def get_MasterZoneId(self):
+	def set_AddressIPVersion(self, AddressIPVersion):  # String
+		self.add_query_param('AddressIPVersion', AddressIPVersion)
+	def get_MasterZoneId(self): # String
 		return self.get_query_params().get('MasterZoneId')
 
-	def set_MasterZoneId(self,MasterZoneId):
-		self.add_query_param('MasterZoneId',MasterZoneId)
-
-	def get_ResourceGroupId(self):
+	def set_MasterZoneId(self, MasterZoneId):  # String
+		self.add_query_param('MasterZoneId', MasterZoneId)
+	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
-	def set_ResourceGroupId(self,ResourceGroupId):
-		self.add_query_param('ResourceGroupId',ResourceGroupId)
-
-	def get_LoadBalancerName(self):
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_LoadBalancerName(self): # String
 		return self.get_query_params().get('LoadBalancerName')
 
-	def set_LoadBalancerName(self,LoadBalancerName):
-		self.add_query_param('LoadBalancerName',LoadBalancerName)
-
-	def get_SlaveZoneId(self):
+	def set_LoadBalancerName(self, LoadBalancerName):  # String
+		self.add_query_param('LoadBalancerName', LoadBalancerName)
+	def get_SlaveZoneId(self): # String
 		return self.get_query_params().get('SlaveZoneId')
 
-	def set_SlaveZoneId(self,SlaveZoneId):
-		self.add_query_param('SlaveZoneId',SlaveZoneId)
-
-	def get_LoadBalancerSpec(self):
-		return self.get_query_params().get('LoadBalancerSpec')
-
-	def set_LoadBalancerSpec(self,LoadBalancerSpec):
-		self.add_query_param('LoadBalancerSpec',LoadBalancerSpec)
-
-	def get_OwnerId(self):
+	def set_SlaveZoneId(self, SlaveZoneId):  # String
+		self.add_query_param('SlaveZoneId', SlaveZoneId)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_VSwitchId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ServerId(self): # String
+		return self.get_query_params().get('ServerId')
+
+	def set_ServerId(self, ServerId):  # String
+		self.add_query_param('ServerId', ServerId)
+	def get_Tags(self): # String
+		return self.get_query_params().get('Tags')
+
+	def set_Tags(self, Tags):  # String
+		self.add_query_param('Tags', Tags)
+	def get_ServerIntranetAddress(self): # String
+		return self.get_query_params().get('ServerIntranetAddress')
+
+	def set_ServerIntranetAddress(self, ServerIntranetAddress):  # String
+		self.add_query_param('ServerIntranetAddress', ServerIntranetAddress)
+	def get_VSwitchId(self): # String
 		return self.get_query_params().get('VSwitchId')
 
-	def set_VSwitchId(self,VSwitchId):
-		self.add_query_param('VSwitchId',VSwitchId)
-
-	def get_InternetChargeType(self):
+	def set_VSwitchId(self, VSwitchId):  # String
+		self.add_query_param('VSwitchId', VSwitchId)
+	def get_LoadBalancerId(self): # String
+		return self.get_query_params().get('LoadBalancerId')
+
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
+	def get_InternetChargeType(self): # String
 		return self.get_query_params().get('InternetChargeType')
 
-	def set_InternetChargeType(self,InternetChargeType):
-		self.add_query_param('InternetChargeType',InternetChargeType)
-
-	def get_PricingCycle(self):
-		return self.get_query_params().get('PricingCycle')
-
-	def set_PricingCycle(self,PricingCycle):
-		self.add_query_param('PricingCycle',PricingCycle)
-
-	def get_ModificationProtectionReason(self):
-		return self.get_query_params().get('ModificationProtectionReason')
-
-	def set_ModificationProtectionReason(self,ModificationProtectionReason):
-		self.add_query_param('ModificationProtectionReason',ModificationProtectionReason)
-
-	def get_ClientToken(self):
-		return self.get_query_params().get('ClientToken')
-
-	def set_ClientToken(self,ClientToken):
-		self.add_query_param('ClientToken',ClientToken)
-
-	def get_Duration(self):
-		return self.get_query_params().get('Duration')
-
-	def set_Duration(self,Duration):
-		self.add_query_param('Duration',Duration)
-
-	def get_AddressType(self):
+	def set_InternetChargeType(self, InternetChargeType):  # String
+		self.add_query_param('InternetChargeType', InternetChargeType)
+	def get_PageNumber(self): # Integer
+		return self.get_query_params().get('PageNumber')
+
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_PageSize(self): # Integer
+		return self.get_query_params().get('PageSize')
+
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
+	def get_AddressType(self): # String
 		return self.get_query_params().get('AddressType')
 
-	def set_AddressType(self,AddressType):
-		self.add_query_param('AddressType',AddressType)
-
-	def get_DeleteProtection(self):
-		return self.get_query_params().get('DeleteProtection')
-
-	def set_DeleteProtection(self,DeleteProtection):
-		self.add_query_param('DeleteProtection',DeleteProtection)
-
-	def get_AutoPay(self):
-		return self.get_query_params().get('AutoPay')
-
-	def set_AutoPay(self,AutoPay):
-		self.add_query_param('AutoPay',AutoPay)
-
-	def get_Address(self):
+	def set_AddressType(self, AddressType):  # String
+		self.add_query_param('AddressType', AddressType)
+	def get_Address(self): # String
 		return self.get_query_params().get('Address')
 
-	def set_Address(self,Address):
-		self.add_query_param('Address',Address)
-
-	def get_ResourceOwnerAccount(self):
+	def set_Address(self, Address):  # String
+		self.add_query_param('Address', Address)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_Bandwidth(self):
-		return self.get_query_params().get('Bandwidth')
-
-	def set_Bandwidth(self,Bandwidth):
-		self.add_query_param('Bandwidth',Bandwidth)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_ModificationProtectionStatus(self):
-		return self.get_query_params().get('ModificationProtectionStatus')
-
-	def set_ModificationProtectionStatus(self,ModificationProtectionStatus):
-		self.add_query_param('ModificationProtectionStatus',ModificationProtectionStatus)
-
-	def get_VpcId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_LoadBalancerStatus(self): # String
+		return self.get_query_params().get('LoadBalancerStatus')
+
+	def set_LoadBalancerStatus(self, LoadBalancerStatus):  # String
+		self.add_query_param('LoadBalancerStatus', LoadBalancerStatus)
+	def get_VpcId(self): # String
 		return self.get_query_params().get('VpcId')
 
-	def set_VpcId(self,VpcId):
-		self.add_query_param('VpcId',VpcId)
-
-	def get_PayType(self):
+	def set_VpcId(self, VpcId):  # String
+		self.add_query_param('VpcId', VpcId)
+	def get_PayType(self): # String
 		return self.get_query_params().get('PayType')
 
-	def set_PayType(self,PayType):
-		self.add_query_param('PayType',PayType)
+	def set_PayType(self, PayType):  # String
+		self.add_query_param('PayType', PayType)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateLoadBalancerUDPListenerRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateLoadBalancerRequest.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,149 +16,138 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class CreateLoadBalancerUDPListenerRequest(RpcRequest):
+class CreateLoadBalancerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateLoadBalancerUDPListener','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateLoadBalancer','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_AclStatus(self):
-		return self.get_query_params().get('AclStatus')
-
-	def set_AclStatus(self,AclStatus):
-		self.add_query_param('AclStatus',AclStatus)
-
-	def get_AclType(self):
-		return self.get_query_params().get('AclType')
-
-	def set_AclType(self,AclType):
-		self.add_query_param('AclType',AclType)
-
-	def get_VServerGroupId(self):
-		return self.get_query_params().get('VServerGroupId')
-
-	def set_VServerGroupId(self,VServerGroupId):
-		self.add_query_param('VServerGroupId',VServerGroupId)
-
-	def get_AclId(self):
-		return self.get_query_params().get('AclId')
-
-	def set_AclId(self,AclId):
-		self.add_query_param('AclId',AclId)
-
-	def get_OwnerId(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_AddressIPVersion(self): # String
+		return self.get_query_params().get('AddressIPVersion')
+
+	def set_AddressIPVersion(self, AddressIPVersion):  # String
+		self.add_query_param('AddressIPVersion', AddressIPVersion)
+	def get_MasterZoneId(self): # String
+		return self.get_query_params().get('MasterZoneId')
+
+	def set_MasterZoneId(self, MasterZoneId):  # String
+		self.add_query_param('MasterZoneId', MasterZoneId)
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_LoadBalancerName(self): # String
+		return self.get_query_params().get('LoadBalancerName')
+
+	def set_LoadBalancerName(self, LoadBalancerName):  # String
+		self.add_query_param('LoadBalancerName', LoadBalancerName)
+	def get_SlaveZoneId(self): # String
+		return self.get_query_params().get('SlaveZoneId')
+
+	def set_SlaveZoneId(self, SlaveZoneId):  # String
+		self.add_query_param('SlaveZoneId', SlaveZoneId)
+	def get_LoadBalancerSpec(self): # String
+		return self.get_query_params().get('LoadBalancerSpec')
+
+	def set_LoadBalancerSpec(self, LoadBalancerSpec):  # String
+		self.add_query_param('LoadBalancerSpec', LoadBalancerSpec)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
-		return self.get_query_params().get('LoadBalancerId')
-
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
-
-	def get_MasterSlaveServerGroupId(self):
-		return self.get_query_params().get('MasterSlaveServerGroupId')
-
-	def set_MasterSlaveServerGroupId(self,MasterSlaveServerGroupId):
-		self.add_query_param('MasterSlaveServerGroupId',MasterSlaveServerGroupId)
-
-	def get_healthCheckReq(self):
-		return self.get_query_params().get('healthCheckReq')
-
-	def set_healthCheckReq(self,healthCheckReq):
-		self.add_query_param('healthCheckReq',healthCheckReq)
-
-	def get_BackendServerPort(self):
-		return self.get_query_params().get('BackendServerPort')
-
-	def set_BackendServerPort(self,BackendServerPort):
-		self.add_query_param('BackendServerPort',BackendServerPort)
-
-	def get_healthCheckInterval(self):
-		return self.get_query_params().get('healthCheckInterval')
-
-	def set_healthCheckInterval(self,healthCheckInterval):
-		self.add_query_param('healthCheckInterval',healthCheckInterval)
-
-	def get_healthCheckExp(self):
-		return self.get_query_params().get('healthCheckExp')
-
-	def set_healthCheckExp(self,healthCheckExp):
-		self.add_query_param('healthCheckExp',healthCheckExp)
-
-	def get_HealthCheckConnectTimeout(self):
-		return self.get_query_params().get('HealthCheckConnectTimeout')
-
-	def set_HealthCheckConnectTimeout(self,HealthCheckConnectTimeout):
-		self.add_query_param('HealthCheckConnectTimeout',HealthCheckConnectTimeout)
-
-	def get_Description(self):
-		return self.get_query_params().get('Description')
-
-	def set_Description(self,Description):
-		self.add_query_param('Description',Description)
-
-	def get_UnhealthyThreshold(self):
-		return self.get_query_params().get('UnhealthyThreshold')
-
-	def set_UnhealthyThreshold(self,UnhealthyThreshold):
-		self.add_query_param('UnhealthyThreshold',UnhealthyThreshold)
-
-	def get_HealthyThreshold(self):
-		return self.get_query_params().get('HealthyThreshold')
-
-	def set_HealthyThreshold(self,HealthyThreshold):
-		self.add_query_param('HealthyThreshold',HealthyThreshold)
-
-	def get_Scheduler(self):
-		return self.get_query_params().get('Scheduler')
-
-	def set_Scheduler(self,Scheduler):
-		self.add_query_param('Scheduler',Scheduler)
-
-	def get_ListenerPort(self):
-		return self.get_query_params().get('ListenerPort')
-
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_VSwitchId(self): # String
+		return self.get_query_params().get('VSwitchId')
+
+	def set_VSwitchId(self, VSwitchId):  # String
+		self.add_query_param('VSwitchId', VSwitchId)
+	def get_InternetChargeType(self): # String
+		return self.get_query_params().get('InternetChargeType')
+
+	def set_InternetChargeType(self, InternetChargeType):  # String
+		self.add_query_param('InternetChargeType', InternetChargeType)
+	def get_PricingCycle(self): # String
+		return self.get_query_params().get('PricingCycle')
+
+	def set_PricingCycle(self, PricingCycle):  # String
+		self.add_query_param('PricingCycle', PricingCycle)
+	def get_ModificationProtectionReason(self): # String
+		return self.get_query_params().get('ModificationProtectionReason')
+
+	def set_ModificationProtectionReason(self, ModificationProtectionReason):  # String
+		self.add_query_param('ModificationProtectionReason', ModificationProtectionReason)
+	def get_ClientToken(self): # String
+		return self.get_query_params().get('ClientToken')
+
+	def set_ClientToken(self, ClientToken):  # String
+		self.add_query_param('ClientToken', ClientToken)
+	def get_Duration(self): # Integer
+		return self.get_query_params().get('Duration')
+
+	def set_Duration(self, Duration):  # Integer
+		self.add_query_param('Duration', Duration)
+	def get_AddressType(self): # String
+		return self.get_query_params().get('AddressType')
+
+	def set_AddressType(self, AddressType):  # String
+		self.add_query_param('AddressType', AddressType)
+	def get_DeleteProtection(self): # String
+		return self.get_query_params().get('DeleteProtection')
+
+	def set_DeleteProtection(self, DeleteProtection):  # String
+		self.add_query_param('DeleteProtection', DeleteProtection)
+	def get_AutoPay(self): # Boolean
+		return self.get_query_params().get('AutoPay')
+
+	def set_AutoPay(self, AutoPay):  # Boolean
+		self.add_query_param('AutoPay', AutoPay)
+	def get_Address(self): # String
+		return self.get_query_params().get('Address')
+
+	def set_Address(self, Address):  # String
+		self.add_query_param('Address', Address)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_Bandwidth(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_Bandwidth(self): # Integer
 		return self.get_query_params().get('Bandwidth')
 
-	def set_Bandwidth(self,Bandwidth):
-		self.add_query_param('Bandwidth',Bandwidth)
-
-	def get_OwnerAccount(self):
+	def set_Bandwidth(self, Bandwidth):  # Integer
+		self.add_query_param('Bandwidth', Bandwidth)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_HealthCheckConnectPort(self):
-		return self.get_query_params().get('HealthCheckConnectPort')
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_ModificationProtectionStatus(self): # String
+		return self.get_query_params().get('ModificationProtectionStatus')
+
+	def set_ModificationProtectionStatus(self, ModificationProtectionStatus):  # String
+		self.add_query_param('ModificationProtectionStatus', ModificationProtectionStatus)
+	def get_VpcId(self): # String
+		return self.get_query_params().get('VpcId')
+
+	def set_VpcId(self, VpcId):  # String
+		self.add_query_param('VpcId', VpcId)
+	def get_PayType(self): # String
+		return self.get_query_params().get('PayType')
 
-	def set_HealthCheckConnectPort(self,HealthCheckConnectPort):
-		self.add_query_param('HealthCheckConnectPort',HealthCheckConnectPort)
+	def set_PayType(self, PayType):  # String
+		self.add_query_param('PayType', PayType)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateMasterSlaveServerGroupRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateMasterSlaveServerGroupRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,56 +19,50 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class CreateMasterSlaveServerGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateMasterSlaveServerGroup','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateMasterSlaveServerGroup','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_MasterSlaveBackendServers(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_MasterSlaveBackendServers(self): # String
 		return self.get_query_params().get('MasterSlaveBackendServers')
 
-	def set_MasterSlaveBackendServers(self,MasterSlaveBackendServers):
-		self.add_query_param('MasterSlaveBackendServers',MasterSlaveBackendServers)
-
-	def get_ResourceOwnerAccount(self):
+	def set_MasterSlaveBackendServers(self, MasterSlaveBackendServers):  # String
+		self.add_query_param('MasterSlaveBackendServers', MasterSlaveBackendServers)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_MasterSlaveServerGroupName(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_MasterSlaveServerGroupName(self): # String
 		return self.get_query_params().get('MasterSlaveServerGroupName')
 
-	def set_MasterSlaveServerGroupName(self,MasterSlaveServerGroupName):
-		self.add_query_param('MasterSlaveServerGroupName',MasterSlaveServerGroupName)
-
-	def get_OwnerId(self):
+	def set_MasterSlaveServerGroupName(self, MasterSlaveServerGroupName):  # String
+		self.add_query_param('MasterSlaveServerGroupName', MasterSlaveServerGroupName)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateRulesRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/StopLoadBalancerListenerRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,65 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class CreateRulesRequest(RpcRequest):
+class StopLoadBalancerListenerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateRules','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'StopLoadBalancerListener','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_RuleList(self):
-		return self.get_query_params().get('RuleList')
-
-	def set_RuleList(self,RuleList):
-		self.add_query_param('RuleList',RuleList)
-
-	def get_ListenerPort(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ListenerPort(self): # Integer
 		return self.get_query_params().get('ListenerPort')
 
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ListenerProtocol(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ListenerProtocol(self): # String
 		return self.get_query_params().get('ListenerProtocol')
 
-	def set_ListenerProtocol(self,ListenerProtocol):
-		self.add_query_param('ListenerProtocol',ListenerProtocol)
-
-	def get_LoadBalancerId(self):
+	def set_ListenerProtocol(self, ListenerProtocol):  # String
+		self.add_query_param('ListenerProtocol', ListenerProtocol)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateTLSCipherPolicyRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateVServerGroupRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,69 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class CreateTLSCipherPolicyRequest(RpcRequest):
+class CreateVServerGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateTLSCipherPolicy','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateVServerGroup','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_access_key_id(self):
-		return self.get_query_params().get('access_key_id')
-
-	def set_access_key_id(self,access_key_id):
-		self.add_query_param('access_key_id',access_key_id)
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_Cipherss(self):
-		return self.get_query_params().get('Ciphers')
-
-	def set_Cipherss(self, Cipherss):
-		for depth1 in range(len(Cipherss)):
-			if Cipherss[depth1] is not None:
-				self.add_query_param('Ciphers.' + str(depth1 + 1) , Cipherss[depth1])
-
-	def get_TLSVersionss(self):
-		return self.get_query_params().get('TLSVersions')
-
-	def set_TLSVersionss(self, TLSVersionss):
-		for depth1 in range(len(TLSVersionss)):
-			if TLSVersionss[depth1] is not None:
-				self.add_query_param('TLSVersions.' + str(depth1 + 1) , TLSVersionss[depth1])
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_BackendServers(self): # String
+		return self.get_query_params().get('BackendServers')
+
+	def set_BackendServers(self, BackendServers):  # String
+		self.add_query_param('BackendServers', BackendServers)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_Name(self):
-		return self.get_query_params().get('Name')
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_VServerGroupName(self): # String
+		return self.get_query_params().get('VServerGroupName')
+
+	def set_VServerGroupName(self, VServerGroupName):  # String
+		self.add_query_param('VServerGroupName', VServerGroupName)
+	def get_LoadBalancerId(self): # String
+		return self.get_query_params().get('LoadBalancerId')
 
-	def set_Name(self,Name):
-		self.add_query_param('Name',Name)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/CreateVServerGroupRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/RemoveVServerGroupBackendServersRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,59 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class CreateVServerGroupRequest(RpcRequest):
+class RemoveVServerGroupBackendServersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateVServerGroup','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'RemoveVServerGroupBackendServers','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_BackendServers(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_BackendServers(self): # String
 		return self.get_query_params().get('BackendServers')
 
-	def set_BackendServers(self,BackendServers):
-		self.add_query_param('BackendServers',BackendServers)
-
-	def get_ResourceOwnerAccount(self):
+	def set_BackendServers(self, BackendServers):  # String
+		self.add_query_param('BackendServers', BackendServers)
+	def get_VServerGroupId(self): # String
+		return self.get_query_params().get('VServerGroupId')
+
+	def set_VServerGroupId(self, VServerGroupId):  # String
+		self.add_query_param('VServerGroupId', VServerGroupId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_VServerGroupName(self):
-		return self.get_query_params().get('VServerGroupName')
-
-	def set_VServerGroupName(self,VServerGroupName):
-		self.add_query_param('VServerGroupName',VServerGroupName)
-
-	def get_LoadBalancerId(self):
-		return self.get_query_params().get('LoadBalancerId')
-
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteAccessControlListRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeZonesRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,47 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DeleteAccessControlListRequest(RpcRequest):
+class DescribeZonesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteAccessControlList','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeZones','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_AclId(self):
-		return self.get_query_params().get('AclId')
-
-	def set_AclId(self,AclId):
-		self.add_query_param('AclId',AclId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteCACertificateRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteCACertificateRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,44 +19,40 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class DeleteCACertificateRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteCACertificate','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteCACertificate','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_CACertificateId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_CACertificateId(self): # String
 		return self.get_query_params().get('CACertificateId')
 
-	def set_CACertificateId(self,CACertificateId):
-		self.add_query_param('CACertificateId',CACertificateId)
+	def set_CACertificateId(self, CACertificateId):  # String
+		self.add_query_param('CACertificateId', CACertificateId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteDomainExtensionRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeDomainExtensionAttributeRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,47 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DeleteDomainExtensionRequest(RpcRequest):
+class DescribeDomainExtensionAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteDomainExtension','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeDomainExtensionAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_DomainExtensionId(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_DomainExtensionId(self): # String
 		return self.get_query_params().get('DomainExtensionId')
 
-	def set_DomainExtensionId(self,DomainExtensionId):
-		self.add_query_param('DomainExtensionId',DomainExtensionId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_DomainExtensionId(self, DomainExtensionId):  # String
+		self.add_query_param('DomainExtensionId', DomainExtensionId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteLoadBalancerListenerRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetListenerAccessControlStatusRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,59 +16,58 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DeleteLoadBalancerListenerRequest(RpcRequest):
+class SetListenerAccessControlStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteLoadBalancerListener','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetListenerAccessControlStatus','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ListenerPort(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_AccessControlStatus(self): # String
+		return self.get_query_params().get('AccessControlStatus')
+
+	def set_AccessControlStatus(self, AccessControlStatus):  # String
+		self.add_query_param('AccessControlStatus', AccessControlStatus)
+	def get_ListenerPort(self): # Integer
 		return self.get_query_params().get('ListenerPort')
 
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ListenerProtocol(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ListenerProtocol(self): # String
 		return self.get_query_params().get('ListenerProtocol')
 
-	def set_ListenerProtocol(self,ListenerProtocol):
-		self.add_query_param('ListenerProtocol',ListenerProtocol)
-
-	def get_LoadBalancerId(self):
+	def set_ListenerProtocol(self, ListenerProtocol):  # String
+		self.add_query_param('ListenerProtocol', ListenerProtocol)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteLoadBalancerRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancerAttributeRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,47 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DeleteLoadBalancerRequest(RpcRequest):
+class DescribeLoadBalancerAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteLoadBalancer','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeLoadBalancerAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteMasterSlaveServerGroupRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteMasterSlaveServerGroupRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,44 +19,40 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class DeleteMasterSlaveServerGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteMasterSlaveServerGroup','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteMasterSlaveServerGroup','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_MasterSlaveServerGroupId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_MasterSlaveServerGroupId(self): # String
 		return self.get_query_params().get('MasterSlaveServerGroupId')
 
-	def set_MasterSlaveServerGroupId(self,MasterSlaveServerGroupId):
-		self.add_query_param('MasterSlaveServerGroupId',MasterSlaveServerGroupId)
+	def set_MasterSlaveServerGroupId(self, MasterSlaveServerGroupId):  # String
+		self.add_query_param('MasterSlaveServerGroupId', MasterSlaveServerGroupId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteRulesRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetBackendServersRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,47 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DeleteRulesRequest(RpcRequest):
+class SetBackendServersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteRules','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetBackendServers','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_BackendServers(self): # String
+		return self.get_query_params().get('BackendServers')
+
+	def set_BackendServers(self, BackendServers):  # String
+		self.add_query_param('BackendServers', BackendServers)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_RuleIds(self):
-		return self.get_query_params().get('RuleIds')
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
+		return self.get_query_params().get('LoadBalancerId')
 
-	def set_RuleIds(self,RuleIds):
-		self.add_query_param('RuleIds',RuleIds)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteServerCertificateRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteServerCertificateRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,44 +19,40 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class DeleteServerCertificateRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteServerCertificate','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteServerCertificate','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ServerCertificateId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ServerCertificateId(self): # String
 		return self.get_query_params().get('ServerCertificateId')
 
-	def set_ServerCertificateId(self,ServerCertificateId):
-		self.add_query_param('ServerCertificateId',ServerCertificateId)
+	def set_ServerCertificateId(self, ServerCertificateId):  # String
+		self.add_query_param('ServerCertificateId', ServerCertificateId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteTLSCipherPolicyRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteTLSCipherPolicyRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,50 +19,45 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class DeleteTLSCipherPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteTLSCipherPolicy','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteTLSCipherPolicy','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_access_key_id(self):
+	def get_access_key_id(self): # String
 		return self.get_query_params().get('access_key_id')
 
-	def set_access_key_id(self,access_key_id):
-		self.add_query_param('access_key_id',access_key_id)
-
-	def get_ResourceOwnerId(self):
+	def set_access_key_id(self, access_key_id):  # String
+		self.add_query_param('access_key_id', access_key_id)
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_TLSCipherPolicyId(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_TLSCipherPolicyId(self): # String
 		return self.get_query_params().get('TLSCipherPolicyId')
 
-	def set_TLSCipherPolicyId(self,TLSCipherPolicyId):
-		self.add_query_param('TLSCipherPolicyId',TLSCipherPolicyId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_TLSCipherPolicyId(self, TLSCipherPolicyId):  # String
+		self.add_query_param('TLSCipherPolicyId', TLSCipherPolicyId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DeleteVServerGroupRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetVServerGroupAttributeRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,47 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DeleteVServerGroupRequest(RpcRequest):
+class SetVServerGroupAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteVServerGroup','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetVServerGroupAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_VServerGroupId(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_BackendServers(self): # String
+		return self.get_query_params().get('BackendServers')
+
+	def set_BackendServers(self, BackendServers):  # String
+		self.add_query_param('BackendServers', BackendServers)
+	def get_VServerGroupId(self): # String
 		return self.get_query_params().get('VServerGroupId')
 
-	def set_VServerGroupId(self,VServerGroupId):
-		self.add_query_param('VServerGroupId',VServerGroupId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_VServerGroupId(self, VServerGroupId):  # String
+		self.add_query_param('VServerGroupId', VServerGroupId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_VServerGroupName(self): # String
+		return self.get_query_params().get('VServerGroupName')
+
+	def set_VServerGroupName(self, VServerGroupName):  # String
+		self.add_query_param('VServerGroupName', VServerGroupName)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeAccessControlListsRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeAccessControlListsRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,68 +19,60 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class DescribeAccessControlListsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeAccessControlLists','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeAccessControlLists','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_AclName(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_AclName(self): # String
 		return self.get_query_params().get('AclName')
 
-	def set_AclName(self,AclName):
-		self.add_query_param('AclName',AclName)
-
-	def get_AddressIPVersion(self):
+	def set_AclName(self, AclName):  # String
+		self.add_query_param('AclName', AclName)
+	def get_AddressIPVersion(self): # String
 		return self.get_query_params().get('AddressIPVersion')
 
-	def set_AddressIPVersion(self,AddressIPVersion):
-		self.add_query_param('AddressIPVersion',AddressIPVersion)
-
-	def get_PageNumber(self):
+	def set_AddressIPVersion(self, AddressIPVersion):  # String
+		self.add_query_param('AddressIPVersion', AddressIPVersion)
+	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_ResourceGroupId(self):
+	def set_PageNumber(self, PageNumber):  # Integer
+		self.add_query_param('PageNumber', PageNumber)
+	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
-	def set_ResourceGroupId(self,ResourceGroupId):
-		self.add_query_param('ResourceGroupId',ResourceGroupId)
-
-	def get_PageSize(self):
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
-
-	def get_ResourceOwnerAccount(self):
+	def set_PageSize(self, PageSize):  # Integer
+		self.add_query_param('PageSize', PageSize)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeAvailableResourceRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeHealthStatusRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,53 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeAvailableResourceRequest(RpcRequest):
+class DescribeHealthStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeAvailableResource','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeHealthStatus','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_AddressIPVersion(self):
-		return self.get_query_params().get('AddressIPVersion')
-
-	def set_AddressIPVersion(self,AddressIPVersion):
-		self.add_query_param('AddressIPVersion',AddressIPVersion)
-
-	def get_AddressType(self):
-		return self.get_query_params().get('AddressType')
-
-	def set_AddressType(self,AddressType):
-		self.add_query_param('AddressType',AddressType)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ListenerPort(self): # Integer
+		return self.get_query_params().get('ListenerPort')
+
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ListenerProtocol(self): # String
+		return self.get_query_params().get('ListenerProtocol')
+
+	def set_ListenerProtocol(self, ListenerProtocol):  # String
+		self.add_query_param('ListenerProtocol', ListenerProtocol)
+	def get_LoadBalancerId(self): # String
+		return self.get_query_params().get('LoadBalancerId')
+
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeCACertificatesRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeCACertificatesRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,50 +19,45 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class DescribeCACertificatesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeCACertificates','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeCACertificates','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceGroupId(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
-	def set_ResourceGroupId(self,ResourceGroupId):
-		self.add_query_param('ResourceGroupId',ResourceGroupId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_CACertificateId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_CACertificateId(self): # String
 		return self.get_query_params().get('CACertificateId')
 
-	def set_CACertificateId(self,CACertificateId):
-		self.add_query_param('CACertificateId',CACertificateId)
+	def set_CACertificateId(self, CACertificateId):  # String
+		self.add_query_param('CACertificateId', CACertificateId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeDomainExtensionAttributeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeRuleAttributeRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,47 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeDomainExtensionAttributeRequest(RpcRequest):
+class DescribeRuleAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeDomainExtensionAttribute','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeRuleAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_DomainExtensionId(self):
-		return self.get_query_params().get('DomainExtensionId')
-
-	def set_DomainExtensionId(self,DomainExtensionId):
-		self.add_query_param('DomainExtensionId',DomainExtensionId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_RuleId(self): # String
+		return self.get_query_params().get('RuleId')
+
+	def set_RuleId(self, RuleId):  # String
+		self.add_query_param('RuleId', RuleId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeDomainExtensionsRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetDomainExtensionAttributeRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,59 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeDomainExtensionsRequest(RpcRequest):
+class SetDomainExtensionAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeDomainExtensions','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetDomainExtensionAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_DomainExtensionId(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_DomainExtensionId(self): # String
 		return self.get_query_params().get('DomainExtensionId')
 
-	def set_DomainExtensionId(self,DomainExtensionId):
-		self.add_query_param('DomainExtensionId',DomainExtensionId)
-
-	def get_ListenerPort(self):
-		return self.get_query_params().get('ListenerPort')
-
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_DomainExtensionId(self, DomainExtensionId):  # String
+		self.add_query_param('DomainExtensionId', DomainExtensionId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
-		return self.get_query_params().get('LoadBalancerId')
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ServerCertificateId(self): # String
+		return self.get_query_params().get('ServerCertificateId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_ServerCertificateId(self, ServerCertificateId):  # String
+		self.add_query_param('ServerCertificateId', ServerCertificateId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeHealthStatusRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancerListenersRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,59 +16,59 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeHealthStatusRequest(RpcRequest):
+class DescribeLoadBalancerListenersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeHealthStatus','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeLoadBalancerListeners','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ListenerPort(self):
-		return self.get_query_params().get('ListenerPort')
-
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_NextToken(self): # String
+		return self.get_query_params().get('NextToken')
+
+	def set_NextToken(self, NextToken):  # String
+		self.add_query_param('NextToken', NextToken)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ListenerProtocol(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ListenerProtocol(self): # String
 		return self.get_query_params().get('ListenerProtocol')
 
-	def set_ListenerProtocol(self,ListenerProtocol):
-		self.add_query_param('ListenerProtocol',ListenerProtocol)
-
-	def get_LoadBalancerId(self):
+	def set_ListenerProtocol(self, ListenerProtocol):  # String
+		self.add_query_param('ListenerProtocol', ListenerProtocol)
+	def get_LoadBalancerIds(self): # RepeatList
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerIds(self, LoadBalancerId):  # RepeatList
+		for depth1 in range(len(LoadBalancerId)):
+			self.add_query_param('LoadBalancerId.' + str(depth1 + 1), LoadBalancerId[depth1])
+	def get_MaxResults(self): # Integer
+		return self.get_query_params().get('MaxResults')
+
+	def set_MaxResults(self, MaxResults):  # Integer
+		self.add_query_param('MaxResults', MaxResults)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeListenerAccessControlAttributeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteLoadBalancerListenerRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,59 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeListenerAccessControlAttributeRequest(RpcRequest):
+class DeleteLoadBalancerListenerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeListenerAccessControlAttribute','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteLoadBalancerListener','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ListenerPort(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ListenerPort(self): # Integer
 		return self.get_query_params().get('ListenerPort')
 
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ListenerProtocol(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ListenerProtocol(self): # String
 		return self.get_query_params().get('ListenerProtocol')
 
-	def set_ListenerProtocol(self,ListenerProtocol):
-		self.add_query_param('ListenerProtocol',ListenerProtocol)
-
-	def get_LoadBalancerId(self):
+	def set_ListenerProtocol(self, ListenerProtocol):  # String
+		self.add_query_param('ListenerProtocol', ListenerProtocol)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeLoadBalancerAttributeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteAccessControlListRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,47 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeLoadBalancerAttributeRequest(RpcRequest):
+class DeleteAccessControlListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeLoadBalancerAttribute','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteAccessControlList','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_AclId(self): # String
+		return self.get_query_params().get('AclId')
+
+	def set_AclId(self, AclId):  # String
+		self.add_query_param('AclId', AclId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
-		return self.get_query_params().get('LoadBalancerId')
-
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeLoadBalancerHTTPListenerAttributeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancerHTTPSListenerAttributeRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeLoadBalancerHTTPListenerAttributeRequest(RpcRequest):
+class DescribeLoadBalancerHTTPSListenerAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeLoadBalancerHTTPListenerAttribute','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeLoadBalancerHTTPSListenerAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ListenerPort(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ListenerPort(self): # Integer
 		return self.get_query_params().get('ListenerPort')
 
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeLoadBalancerHTTPSListenerAttributeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancerUDPListenerAttributeRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeLoadBalancerHTTPSListenerAttributeRequest(RpcRequest):
+class DescribeLoadBalancerUDPListenerAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeLoadBalancerHTTPSListenerAttribute','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeLoadBalancerUDPListenerAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ListenerPort(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ListenerPort(self): # Integer
 		return self.get_query_params().get('ListenerPort')
 
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeLoadBalancerListenersRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/AddTagsRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,67 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeLoadBalancerListenersRequest(RpcRequest):
+class AddTagsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeLoadBalancerListeners','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'AddTags','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_NextToken(self):
-		return self.get_query_params().get('NextToken')
-
-	def set_NextToken(self,NextToken):
-		self.add_query_param('NextToken',NextToken)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ListenerProtocol(self):
-		return self.get_query_params().get('ListenerProtocol')
-
-	def set_ListenerProtocol(self,ListenerProtocol):
-		self.add_query_param('ListenerProtocol',ListenerProtocol)
-
-	def get_LoadBalancerIds(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_Tags(self): # String
+		return self.get_query_params().get('Tags')
+
+	def set_Tags(self, Tags):  # String
+		self.add_query_param('Tags', Tags)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerIds(self, LoadBalancerIds):
-		for depth1 in range(len(LoadBalancerIds)):
-			if LoadBalancerIds[depth1] is not None:
-				self.add_query_param('LoadBalancerId.' + str(depth1 + 1) , LoadBalancerIds[depth1])
-
-	def get_MaxResults(self):
-		return self.get_query_params().get('MaxResults')
-
-	def set_MaxResults(self,MaxResults):
-		self.add_query_param('MaxResults',MaxResults)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeLoadBalancerTCPListenerAttributeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeLoadBalancerHTTPListenerAttributeRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeLoadBalancerTCPListenerAttributeRequest(RpcRequest):
+class DescribeLoadBalancerHTTPListenerAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeLoadBalancerTCPListenerAttribute','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeLoadBalancerHTTPListenerAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ListenerPort(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ListenerPort(self): # Integer
 		return self.get_query_params().get('ListenerPort')
 
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeLoadBalancerUDPListenerAttributeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/StartLoadBalancerListenerRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,53 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeLoadBalancerUDPListenerAttributeRequest(RpcRequest):
+class StartLoadBalancerListenerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeLoadBalancerUDPListenerAttribute','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'StartLoadBalancerListener','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ListenerPort(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ListenerPort(self): # Integer
 		return self.get_query_params().get('ListenerPort')
 
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ListenerProtocol(self): # String
+		return self.get_query_params().get('ListenerProtocol')
+
+	def set_ListenerProtocol(self, ListenerProtocol):  # String
+		self.add_query_param('ListenerProtocol', ListenerProtocol)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeMasterSlaveServerGroupAttributeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/AddVServerGroupBackendServersRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,47 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeMasterSlaveServerGroupAttributeRequest(RpcRequest):
+class AddVServerGroupBackendServersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeMasterSlaveServerGroupAttribute','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'AddVServerGroupBackendServers','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_BackendServers(self): # String
+		return self.get_query_params().get('BackendServers')
+
+	def set_BackendServers(self, BackendServers):  # String
+		self.add_query_param('BackendServers', BackendServers)
+	def get_VServerGroupId(self): # String
+		return self.get_query_params().get('VServerGroupId')
+
+	def set_VServerGroupId(self, VServerGroupId):  # String
+		self.add_query_param('VServerGroupId', VServerGroupId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_MasterSlaveServerGroupId(self):
-		return self.get_query_params().get('MasterSlaveServerGroupId')
-
-	def set_MasterSlaveServerGroupId(self,MasterSlaveServerGroupId):
-		self.add_query_param('MasterSlaveServerGroupId',MasterSlaveServerGroupId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeMasterSlaveServerGroupsRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/ListTagResourcesRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,53 +16,63 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeMasterSlaveServerGroupsRequest(RpcRequest):
+class ListTagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeMasterSlaveServerGroups','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'ListTagResources','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_IncludeListener(self):
-		return self.get_query_params().get('IncludeListener')
-
-	def set_IncludeListener(self,IncludeListener):
-		self.add_query_param('IncludeListener',IncludeListener)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_NextToken(self): # String
+		return self.get_query_params().get('NextToken')
+
+	def set_NextToken(self, NextToken):  # String
+		self.add_query_param('NextToken', NextToken)
+	def get_Tags(self): # RepeatList
+		return self.get_query_params().get('Tag')
+
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Value') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
+			if Tag[depth1].get('Key') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+	def get_ResourceIds(self): # RepeatList
+		return self.get_query_params().get('ResourceId')
+
+	def set_ResourceIds(self, ResourceId):  # RepeatList
+		for depth1 in range(len(ResourceId)):
+			self.add_query_param('ResourceId.' + str(depth1 + 1), ResourceId[depth1])
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
-		return self.get_query_params().get('LoadBalancerId')
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ResourceType(self): # String
+		return self.get_query_params().get('ResourceType')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_ResourceType(self, ResourceType):  # String
+		self.add_query_param('ResourceType', ResourceType)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeRegionsRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeRegionsRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,44 +19,40 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class DescribeRegionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeRegions','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeRegions','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_AcceptLanguage(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_AcceptLanguage(self): # String
 		return self.get_query_params().get('AcceptLanguage')
 
-	def set_AcceptLanguage(self,AcceptLanguage):
-		self.add_query_param('AcceptLanguage',AcceptLanguage)
+	def set_AcceptLanguage(self, AcceptLanguage):  # String
+		self.add_query_param('AcceptLanguage', AcceptLanguage)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeRuleAttributeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteLoadBalancerRequest.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,47 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeRuleAttributeRequest(RpcRequest):
+class DeleteLoadBalancerRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeRuleAttribute','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteLoadBalancer','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_RuleId(self):
-		return self.get_query_params().get('RuleId')
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
+		return self.get_query_params().get('LoadBalancerId')
 
-	def set_RuleId(self,RuleId):
-		self.add_query_param('RuleId',RuleId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeRulesRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeListenerAccessControlAttributeRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,59 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeRulesRequest(RpcRequest):
+class DescribeListenerAccessControlAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeRules','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeListenerAccessControlAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ListenerPort(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ListenerPort(self): # Integer
 		return self.get_query_params().get('ListenerPort')
 
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ListenerProtocol(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ListenerProtocol(self): # String
 		return self.get_query_params().get('ListenerProtocol')
 
-	def set_ListenerProtocol(self,ListenerProtocol):
-		self.add_query_param('ListenerProtocol',ListenerProtocol)
-
-	def get_LoadBalancerId(self):
+	def set_ListenerProtocol(self, ListenerProtocol):  # String
+		self.add_query_param('ListenerProtocol', ListenerProtocol)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeServerCertificatesRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeServerCertificatesRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,50 +19,45 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class DescribeServerCertificatesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeServerCertificates','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeServerCertificates','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceGroupId(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
-	def set_ResourceGroupId(self,ResourceGroupId):
-		self.add_query_param('ResourceGroupId',ResourceGroupId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ServerCertificateId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ServerCertificateId(self): # String
 		return self.get_query_params().get('ServerCertificateId')
 
-	def set_ServerCertificateId(self,ServerCertificateId):
-		self.add_query_param('ServerCertificateId',ServerCertificateId)
+	def set_ServerCertificateId(self, ServerCertificateId):  # String
+		self.add_query_param('ServerCertificateId', ServerCertificateId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeTagsRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateAccessControlListRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,71 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class DescribeTagsRequest(RpcRequest):
+class CreateAccessControlListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeTags','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateAccessControlList','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_PageNumber(self):
-		return self.get_query_params().get('PageNumber')
-
-	def set_PageNumber(self,PageNumber):
-		self.add_query_param('PageNumber',PageNumber)
-
-	def get_PageSize(self):
-		return self.get_query_params().get('PageSize')
-
-	def set_PageSize(self,PageSize):
-		self.add_query_param('PageSize',PageSize)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_AclName(self): # String
+		return self.get_query_params().get('AclName')
+
+	def set_AclName(self, AclName):  # String
+		self.add_query_param('AclName', AclName)
+	def get_AddressIPVersion(self): # String
+		return self.get_query_params().get('AddressIPVersion')
+
+	def set_AddressIPVersion(self, AddressIPVersion):  # String
+		self.add_query_param('AddressIPVersion', AddressIPVersion)
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_DistinctKey(self):
-		return self.get_query_params().get('DistinctKey')
-
-	def set_DistinctKey(self,DistinctKey):
-		self.add_query_param('DistinctKey',DistinctKey)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_Tags(self):
-		return self.get_query_params().get('Tags')
-
-	def set_Tags(self,Tags):
-		self.add_query_param('Tags',Tags)
-
-	def get_LoadBalancerId(self):
-		return self.get_query_params().get('LoadBalancerId')
-
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/DescribeVServerGroupsRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeVServerGroupsRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,56 +19,50 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class DescribeVServerGroupsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeVServerGroups','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeVServerGroups','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_IncludeListener(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_IncludeListener(self): # Boolean
 		return self.get_query_params().get('IncludeListener')
 
-	def set_IncludeListener(self,IncludeListener):
-		self.add_query_param('IncludeListener',IncludeListener)
-
-	def get_IncludeRule(self):
+	def set_IncludeListener(self, IncludeListener):  # Boolean
+		self.add_query_param('IncludeListener', IncludeListener)
+	def get_IncludeRule(self): # Boolean
 		return self.get_query_params().get('IncludeRule')
 
-	def set_IncludeRule(self,IncludeRule):
-		self.add_query_param('IncludeRule',IncludeRule)
-
-	def get_ResourceOwnerAccount(self):
+	def set_IncludeRule(self, IncludeRule):  # Boolean
+		self.add_query_param('IncludeRule', IncludeRule)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/ListTLSCipherPoliciesRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteDomainExtensionRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,77 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class ListTLSCipherPoliciesRequest(RpcRequest):
+class DeleteDomainExtensionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'ListTLSCipherPolicies','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteDomainExtension','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_access_key_id(self):
-		return self.get_query_params().get('access_key_id')
-
-	def set_access_key_id(self,access_key_id):
-		self.add_query_param('access_key_id',access_key_id)
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_IncludeListener(self):
-		return self.get_query_params().get('IncludeListener')
-
-	def set_IncludeListener(self,IncludeListener):
-		self.add_query_param('IncludeListener',IncludeListener)
-
-	def get_TLSCipherPolicyId(self):
-		return self.get_query_params().get('TLSCipherPolicyId')
-
-	def set_TLSCipherPolicyId(self,TLSCipherPolicyId):
-		self.add_query_param('TLSCipherPolicyId',TLSCipherPolicyId)
-
-	def get_NextToken(self):
-		return self.get_query_params().get('NextToken')
-
-	def set_NextToken(self,NextToken):
-		self.add_query_param('NextToken',NextToken)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_DomainExtensionId(self): # String
+		return self.get_query_params().get('DomainExtensionId')
+
+	def set_DomainExtensionId(self, DomainExtensionId):  # String
+		self.add_query_param('DomainExtensionId', DomainExtensionId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_Name(self):
-		return self.get_query_params().get('Name')
-
-	def set_Name(self,Name):
-		self.add_query_param('Name',Name)
-
-	def get_MaxItems(self):
-		return self.get_query_params().get('MaxItems')
-
-	def set_MaxItems(self,MaxItems):
-		self.add_query_param('MaxItems',MaxItems)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/ListTagResourcesRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/TagResourcesRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,71 +16,58 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class ListTagResourcesRequest(RpcRequest):
+class TagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'ListTagResources','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'TagResources','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_NextToken(self):
-		return self.get_query_params().get('NextToken')
-
-	def set_NextToken(self,NextToken):
-		self.add_query_param('NextToken',NextToken)
-
-	def get_Tags(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_Tags(self): # RepeatList
 		return self.get_query_params().get('Tag')
 
-	def set_Tags(self, Tags):
-		for depth1 in range(len(Tags)):
-			if Tags[depth1].get('Value') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
-			if Tags[depth1].get('Key') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
-
-	def get_ResourceIds(self):
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Value') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
+			if Tag[depth1].get('Key') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+	def get_ResourceIds(self): # RepeatList
 		return self.get_query_params().get('ResourceId')
 
-	def set_ResourceIds(self, ResourceIds):
-		for depth1 in range(len(ResourceIds)):
-			if ResourceIds[depth1] is not None:
-				self.add_query_param('ResourceId.' + str(depth1 + 1) , ResourceIds[depth1])
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceIds(self, ResourceId):  # RepeatList
+		for depth1 in range(len(ResourceId)):
+			self.add_query_param('ResourceId.' + str(depth1 + 1), ResourceId[depth1])
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ResourceType(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ResourceType(self): # String
 		return self.get_query_params().get('ResourceType')
 
-	def set_ResourceType(self,ResourceType):
-		self.add_query_param('ResourceType',ResourceType)
+	def set_ResourceType(self, ResourceType):  # String
+		self.add_query_param('ResourceType', ResourceType)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/ModifyLoadBalancerInstanceSpecRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/ModifyLoadBalancerInstanceSpecRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,56 +19,50 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class ModifyLoadBalancerInstanceSpecRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'ModifyLoadBalancerInstanceSpec','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'ModifyLoadBalancerInstanceSpec','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_LoadBalancerSpec(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_LoadBalancerSpec(self): # String
 		return self.get_query_params().get('LoadBalancerSpec')
 
-	def set_LoadBalancerSpec(self,LoadBalancerSpec):
-		self.add_query_param('LoadBalancerSpec',LoadBalancerSpec)
-
-	def get_AutoPay(self):
+	def set_LoadBalancerSpec(self, LoadBalancerSpec):  # String
+		self.add_query_param('LoadBalancerSpec', LoadBalancerSpec)
+	def get_AutoPay(self): # Boolean
 		return self.get_query_params().get('AutoPay')
 
-	def set_AutoPay(self,AutoPay):
-		self.add_query_param('AutoPay',AutoPay)
-
-	def get_ResourceOwnerAccount(self):
+	def set_AutoPay(self, AutoPay):  # Boolean
+		self.add_query_param('AutoPay', AutoPay)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/ModifyLoadBalancerInternetSpecRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/ModifyLoadBalancerPayTypeRequest.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,65 +16,63 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class ModifyLoadBalancerInternetSpecRequest(RpcRequest):
+class ModifyLoadBalancerPayTypeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'ModifyLoadBalancerInternetSpec','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'ModifyLoadBalancerPayType','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_AutoPay(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_Duration(self): # Integer
+		return self.get_query_params().get('Duration')
+
+	def set_Duration(self, Duration):  # Integer
+		self.add_query_param('Duration', Duration)
+	def get_AutoPay(self): # Boolean
 		return self.get_query_params().get('AutoPay')
 
-	def set_AutoPay(self,AutoPay):
-		self.add_query_param('AutoPay',AutoPay)
-
-	def get_ResourceOwnerAccount(self):
+	def set_AutoPay(self, AutoPay):  # Boolean
+		self.add_query_param('AutoPay', AutoPay)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_Bandwidth(self):
-		return self.get_query_params().get('Bandwidth')
-
-	def set_Bandwidth(self,Bandwidth):
-		self.add_query_param('Bandwidth',Bandwidth)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
-
-	def get_InternetChargeType(self):
-		return self.get_query_params().get('InternetChargeType')
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
+	def get_PayType(self): # String
+		return self.get_query_params().get('PayType')
+
+	def set_PayType(self, PayType):  # String
+		self.add_query_param('PayType', PayType)
+	def get_PricingCycle(self): # String
+		return self.get_query_params().get('PricingCycle')
 
-	def set_InternetChargeType(self,InternetChargeType):
-		self.add_query_param('InternetChargeType',InternetChargeType)
+	def set_PricingCycle(self, PricingCycle):  # String
+		self.add_query_param('PricingCycle', PricingCycle)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/ModifyLoadBalancerPayTypeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/CreateTLSCipherPolicyRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,71 +16,60 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class ModifyLoadBalancerPayTypeRequest(RpcRequest):
+class CreateTLSCipherPolicyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'ModifyLoadBalancerPayType','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'CreateTLSCipherPolicy','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_access_key_id(self): # String
+		return self.get_query_params().get('access_key_id')
 
-	def get_ResourceOwnerId(self):
+	def set_access_key_id(self, access_key_id):  # String
+		self.add_query_param('access_key_id', access_key_id)
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_Duration(self):
-		return self.get_query_params().get('Duration')
-
-	def set_Duration(self,Duration):
-		self.add_query_param('Duration',Duration)
-
-	def get_AutoPay(self):
-		return self.get_query_params().get('AutoPay')
-
-	def set_AutoPay(self,AutoPay):
-		self.add_query_param('AutoPay',AutoPay)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_Cipherss(self): # RepeatList
+		return self.get_query_params().get('Ciphers')
+
+	def set_Cipherss(self, Ciphers):  # RepeatList
+		for depth1 in range(len(Ciphers)):
+			self.add_query_param('Ciphers.' + str(depth1 + 1), Ciphers[depth1])
+	def get_TLSVersionss(self): # RepeatList
+		return self.get_query_params().get('TLSVersions')
+
+	def set_TLSVersionss(self, TLSVersions):  # RepeatList
+		for depth1 in range(len(TLSVersions)):
+			self.add_query_param('TLSVersions.' + str(depth1 + 1), TLSVersions[depth1])
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
-		return self.get_query_params().get('LoadBalancerId')
-
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
-
-	def get_PayType(self):
-		return self.get_query_params().get('PayType')
-
-	def set_PayType(self,PayType):
-		self.add_query_param('PayType',PayType)
-
-	def get_PricingCycle(self):
-		return self.get_query_params().get('PricingCycle')
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_Name(self): # String
+		return self.get_query_params().get('Name')
 
-	def set_PricingCycle(self,PricingCycle):
-		self.add_query_param('PricingCycle',PricingCycle)
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/ModifyVServerGroupBackendServersRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteVServerGroupRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,59 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class ModifyVServerGroupBackendServersRequest(RpcRequest):
+class DeleteVServerGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'ModifyVServerGroupBackendServers','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteVServerGroup','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_VServerGroupId(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_VServerGroupId(self): # String
 		return self.get_query_params().get('VServerGroupId')
 
-	def set_VServerGroupId(self,VServerGroupId):
-		self.add_query_param('VServerGroupId',VServerGroupId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_VServerGroupId(self, VServerGroupId):  # String
+		self.add_query_param('VServerGroupId', VServerGroupId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_NewBackendServers(self):
-		return self.get_query_params().get('NewBackendServers')
-
-	def set_NewBackendServers(self,NewBackendServers):
-		self.add_query_param('NewBackendServers',NewBackendServers)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_OldBackendServers(self):
-		return self.get_query_params().get('OldBackendServers')
-
-	def set_OldBackendServers(self,OldBackendServers):
-		self.add_query_param('OldBackendServers',OldBackendServers)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/RemoveBackendServersRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/AddBackendServersRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class RemoveBackendServersRequest(RpcRequest):
+class AddBackendServersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'RemoveBackendServers','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'AddBackendServers','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_BackendServers(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_BackendServers(self): # String
 		return self.get_query_params().get('BackendServers')
 
-	def set_BackendServers(self,BackendServers):
-		self.add_query_param('BackendServers',BackendServers)
-
-	def get_ResourceOwnerAccount(self):
+	def set_BackendServers(self, BackendServers):  # String
+		self.add_query_param('BackendServers', BackendServers)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/RemoveListenerWhiteListItemRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeRulesRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,65 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class RemoveListenerWhiteListItemRequest(RpcRequest):
+class DescribeRulesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'RemoveListenerWhiteListItem','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeRules','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_SourceItems(self):
-		return self.get_query_params().get('SourceItems')
-
-	def set_SourceItems(self,SourceItems):
-		self.add_query_param('SourceItems',SourceItems)
-
-	def get_ListenerPort(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ListenerPort(self): # Integer
 		return self.get_query_params().get('ListenerPort')
 
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ListenerProtocol(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ListenerProtocol(self): # String
 		return self.get_query_params().get('ListenerProtocol')
 
-	def set_ListenerProtocol(self,ListenerProtocol):
-		self.add_query_param('ListenerProtocol',ListenerProtocol)
-
-	def get_LoadBalancerId(self):
+	def set_ListenerProtocol(self, ListenerProtocol):  # String
+		self.add_query_param('ListenerProtocol', ListenerProtocol)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/RemoveTagsRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DeleteRulesRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,53 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class RemoveTagsRequest(RpcRequest):
+class DeleteRulesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'RemoveTags','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DeleteRules','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_Tags(self):
-		return self.get_query_params().get('Tags')
-
-	def set_Tags(self,Tags):
-		self.add_query_param('Tags',Tags)
-
-	def get_LoadBalancerId(self):
-		return self.get_query_params().get('LoadBalancerId')
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_RuleIds(self): # String
+		return self.get_query_params().get('RuleIds')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_RuleIds(self, RuleIds):  # String
+		self.add_query_param('RuleIds', RuleIds)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetBackendServersRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/UntagResourcesRequest.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,53 +16,60 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class SetBackendServersRequest(RpcRequest):
+class UntagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetBackendServers','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'UntagResources','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_BackendServers(self):
-		return self.get_query_params().get('BackendServers')
-
-	def set_BackendServers(self,BackendServers):
-		self.add_query_param('BackendServers',BackendServers)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_All(self): # Boolean
+		return self.get_query_params().get('All')
+
+	def set_All(self, All):  # Boolean
+		self.add_query_param('All', All)
+	def get_ResourceIds(self): # RepeatList
+		return self.get_query_params().get('ResourceId')
+
+	def set_ResourceIds(self, ResourceId):  # RepeatList
+		for depth1 in range(len(ResourceId)):
+			self.add_query_param('ResourceId.' + str(depth1 + 1), ResourceId[depth1])
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
-		return self.get_query_params().get('LoadBalancerId')
-
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ResourceType(self): # String
+		return self.get_query_params().get('ResourceType')
+
+	def set_ResourceType(self, ResourceType):  # String
+		self.add_query_param('ResourceType', ResourceType)
+	def get_TagKeys(self): # RepeatList
+		return self.get_query_params().get('TagKey')
+
+	def set_TagKeys(self, TagKey):  # RepeatList
+		for depth1 in range(len(TagKey)):
+			self.add_query_param('TagKey.' + str(depth1 + 1), TagKey[depth1])
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetCACertificateNameRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeAccessControlListAttributeRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class SetCACertificateNameRequest(RpcRequest):
+class DescribeAccessControlListAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetCACertificateName','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeAccessControlListAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_CACertificateName(self):
-		return self.get_query_params().get('CACertificateName')
-
-	def set_CACertificateName(self,CACertificateName):
-		self.add_query_param('CACertificateName',CACertificateName)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_AclId(self): # String
+		return self.get_query_params().get('AclId')
+
+	def set_AclId(self, AclId):  # String
+		self.add_query_param('AclId', AclId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_AclEntryComment(self): # String
+		return self.get_query_params().get('AclEntryComment')
+
+	def set_AclEntryComment(self, AclEntryComment):  # String
+		self.add_query_param('AclEntryComment', AclEntryComment)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_CACertificateId(self):
-		return self.get_query_params().get('CACertificateId')
-
-	def set_CACertificateId(self,CACertificateId):
-		self.add_query_param('CACertificateId',CACertificateId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetDomainExtensionAttributeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetServerCertificateNameRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class SetDomainExtensionAttributeRequest(RpcRequest):
+class SetServerCertificateNameRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetDomainExtensionAttribute','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetServerCertificateName','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_DomainExtensionId(self):
-		return self.get_query_params().get('DomainExtensionId')
-
-	def set_DomainExtensionId(self,DomainExtensionId):
-		self.add_query_param('DomainExtensionId',DomainExtensionId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ServerCertificateId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_ServerCertificateId(self): # String
 		return self.get_query_params().get('ServerCertificateId')
 
-	def set_ServerCertificateId(self,ServerCertificateId):
-		self.add_query_param('ServerCertificateId',ServerCertificateId)
+	def set_ServerCertificateId(self, ServerCertificateId):  # String
+		self.add_query_param('ServerCertificateId', ServerCertificateId)
+	def get_ServerCertificateName(self): # String
+		return self.get_query_params().get('ServerCertificateName')
+
+	def set_ServerCertificateName(self, ServerCertificateName):  # String
+		self.add_query_param('ServerCertificateName', ServerCertificateName)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetListenerAccessControlStatusRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeDomainExtensionsRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,65 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class SetListenerAccessControlStatusRequest(RpcRequest):
+class DescribeDomainExtensionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetListenerAccessControlStatus','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeDomainExtensions','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_AccessControlStatus(self):
-		return self.get_query_params().get('AccessControlStatus')
-
-	def set_AccessControlStatus(self,AccessControlStatus):
-		self.add_query_param('AccessControlStatus',AccessControlStatus)
-
-	def get_ListenerPort(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_DomainExtensionId(self): # String
+		return self.get_query_params().get('DomainExtensionId')
+
+	def set_DomainExtensionId(self, DomainExtensionId):  # String
+		self.add_query_param('DomainExtensionId', DomainExtensionId)
+	def get_ListenerPort(self): # Integer
 		return self.get_query_params().get('ListenerPort')
 
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ListenerProtocol(self):
-		return self.get_query_params().get('ListenerProtocol')
-
-	def set_ListenerProtocol(self,ListenerProtocol):
-		self.add_query_param('ListenerProtocol',ListenerProtocol)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetLoadBalancerDeleteProtectionRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerDeleteProtectionRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,50 +19,45 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class SetLoadBalancerDeleteProtectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetLoadBalancerDeleteProtection','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetLoadBalancerDeleteProtection','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_DeleteProtection(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_DeleteProtection(self): # String
 		return self.get_query_params().get('DeleteProtection')
 
-	def set_DeleteProtection(self,DeleteProtection):
-		self.add_query_param('DeleteProtection',DeleteProtection)
-
-	def get_ResourceOwnerAccount(self):
+	def set_DeleteProtection(self, DeleteProtection):  # String
+		self.add_query_param('DeleteProtection', DeleteProtection)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetLoadBalancerModificationProtectionRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerModificationProtectionRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,56 +19,50 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class SetLoadBalancerModificationProtectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetLoadBalancerModificationProtection','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetLoadBalancerModificationProtection','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ModificationProtectionReason(self):
+	def get_ModificationProtectionReason(self): # String
 		return self.get_query_params().get('ModificationProtectionReason')
 
-	def set_ModificationProtectionReason(self,ModificationProtectionReason):
-		self.add_query_param('ModificationProtectionReason',ModificationProtectionReason)
-
-	def get_ResourceOwnerId(self):
+	def set_ModificationProtectionReason(self, ModificationProtectionReason):  # String
+		self.add_query_param('ModificationProtectionReason', ModificationProtectionReason)
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_ModificationProtectionStatus(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_ModificationProtectionStatus(self): # String
 		return self.get_query_params().get('ModificationProtectionStatus')
 
-	def set_ModificationProtectionStatus(self,ModificationProtectionStatus):
-		self.add_query_param('ModificationProtectionStatus',ModificationProtectionStatus)
-
-	def get_OwnerAccount(self):
+	def set_ModificationProtectionStatus(self, ModificationProtectionStatus):  # String
+		self.add_query_param('ModificationProtectionStatus', ModificationProtectionStatus)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetLoadBalancerNameRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerNameRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,50 +19,45 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class SetLoadBalancerNameRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetLoadBalancerName','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetLoadBalancerName','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_LoadBalancerName(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_LoadBalancerName(self): # String
 		return self.get_query_params().get('LoadBalancerName')
 
-	def set_LoadBalancerName(self,LoadBalancerName):
-		self.add_query_param('LoadBalancerName',LoadBalancerName)
-
-	def get_ResourceOwnerAccount(self):
+	def set_LoadBalancerName(self, LoadBalancerName):  # String
+		self.add_query_param('LoadBalancerName', LoadBalancerName)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetLoadBalancerStatusRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeAvailableResourceRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class SetLoadBalancerStatusRequest(RpcRequest):
+class DescribeAvailableResourceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetLoadBalancerStatus','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeAvailableResource','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_AddressIPVersion(self): # String
+		return self.get_query_params().get('AddressIPVersion')
+
+	def set_AddressIPVersion(self, AddressIPVersion):  # String
+		self.add_query_param('AddressIPVersion', AddressIPVersion)
+	def get_AddressType(self): # String
+		return self.get_query_params().get('AddressType')
+
+	def set_AddressType(self, AddressType):  # String
+		self.add_query_param('AddressType', AddressType)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerStatus(self):
-		return self.get_query_params().get('LoadBalancerStatus')
-
-	def set_LoadBalancerStatus(self,LoadBalancerStatus):
-		self.add_query_param('LoadBalancerStatus',LoadBalancerStatus)
-
-	def get_LoadBalancerId(self):
-		return self.get_query_params().get('LoadBalancerId')
-
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetLoadBalancerUDPListenerAttributeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerUDPListenerAttributeRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,152 +19,130 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class SetLoadBalancerUDPListenerAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetLoadBalancerUDPListenerAttribute','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetLoadBalancerUDPListenerAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_AclStatus(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_AclStatus(self): # String
 		return self.get_query_params().get('AclStatus')
 
-	def set_AclStatus(self,AclStatus):
-		self.add_query_param('AclStatus',AclStatus)
-
-	def get_AclType(self):
+	def set_AclStatus(self, AclStatus):  # String
+		self.add_query_param('AclStatus', AclStatus)
+	def get_AclType(self): # String
 		return self.get_query_params().get('AclType')
 
-	def set_AclType(self,AclType):
-		self.add_query_param('AclType',AclType)
-
-	def get_MasterSlaveServerGroup(self):
+	def set_AclType(self, AclType):  # String
+		self.add_query_param('AclType', AclType)
+	def get_MasterSlaveServerGroup(self): # String
 		return self.get_query_params().get('MasterSlaveServerGroup')
 
-	def set_MasterSlaveServerGroup(self,MasterSlaveServerGroup):
-		self.add_query_param('MasterSlaveServerGroup',MasterSlaveServerGroup)
-
-	def get_VServerGroupId(self):
+	def set_MasterSlaveServerGroup(self, MasterSlaveServerGroup):  # String
+		self.add_query_param('MasterSlaveServerGroup', MasterSlaveServerGroup)
+	def get_VServerGroupId(self): # String
 		return self.get_query_params().get('VServerGroupId')
 
-	def set_VServerGroupId(self,VServerGroupId):
-		self.add_query_param('VServerGroupId',VServerGroupId)
-
-	def get_AclId(self):
+	def set_VServerGroupId(self, VServerGroupId):  # String
+		self.add_query_param('VServerGroupId', VServerGroupId)
+	def get_AclId(self): # String
 		return self.get_query_params().get('AclId')
 
-	def set_AclId(self,AclId):
-		self.add_query_param('AclId',AclId)
-
-	def get_OwnerId(self):
+	def set_AclId(self, AclId):  # String
+		self.add_query_param('AclId', AclId)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
-
-	def get_MasterSlaveServerGroupId(self):
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
+	def get_MasterSlaveServerGroupId(self): # String
 		return self.get_query_params().get('MasterSlaveServerGroupId')
 
-	def set_MasterSlaveServerGroupId(self,MasterSlaveServerGroupId):
-		self.add_query_param('MasterSlaveServerGroupId',MasterSlaveServerGroupId)
-
-	def get_healthCheckReq(self):
+	def set_MasterSlaveServerGroupId(self, MasterSlaveServerGroupId):  # String
+		self.add_query_param('MasterSlaveServerGroupId', MasterSlaveServerGroupId)
+	def get_healthCheckReq(self): # String
 		return self.get_query_params().get('healthCheckReq')
 
-	def set_healthCheckReq(self,healthCheckReq):
-		self.add_query_param('healthCheckReq',healthCheckReq)
-
-	def get_HealthCheckInterval(self):
+	def set_healthCheckReq(self, healthCheckReq):  # String
+		self.add_query_param('healthCheckReq', healthCheckReq)
+	def get_HealthCheckInterval(self): # Integer
 		return self.get_query_params().get('HealthCheckInterval')
 
-	def set_HealthCheckInterval(self,HealthCheckInterval):
-		self.add_query_param('HealthCheckInterval',HealthCheckInterval)
-
-	def get_healthCheckExp(self):
+	def set_HealthCheckInterval(self, HealthCheckInterval):  # Integer
+		self.add_query_param('HealthCheckInterval', HealthCheckInterval)
+	def get_healthCheckExp(self): # String
 		return self.get_query_params().get('healthCheckExp')
 
-	def set_healthCheckExp(self,healthCheckExp):
-		self.add_query_param('healthCheckExp',healthCheckExp)
-
-	def get_HealthCheckConnectTimeout(self):
+	def set_healthCheckExp(self, healthCheckExp):  # String
+		self.add_query_param('healthCheckExp', healthCheckExp)
+	def get_HealthCheckConnectTimeout(self): # Integer
 		return self.get_query_params().get('HealthCheckConnectTimeout')
 
-	def set_HealthCheckConnectTimeout(self,HealthCheckConnectTimeout):
-		self.add_query_param('HealthCheckConnectTimeout',HealthCheckConnectTimeout)
-
-	def get_Description(self):
+	def set_HealthCheckConnectTimeout(self, HealthCheckConnectTimeout):  # Integer
+		self.add_query_param('HealthCheckConnectTimeout', HealthCheckConnectTimeout)
+	def get_Description(self): # String
 		return self.get_query_params().get('Description')
 
-	def set_Description(self,Description):
-		self.add_query_param('Description',Description)
-
-	def get_UnhealthyThreshold(self):
+	def set_Description(self, Description):  # String
+		self.add_query_param('Description', Description)
+	def get_UnhealthyThreshold(self): # Integer
 		return self.get_query_params().get('UnhealthyThreshold')
 
-	def set_UnhealthyThreshold(self,UnhealthyThreshold):
-		self.add_query_param('UnhealthyThreshold',UnhealthyThreshold)
-
-	def get_HealthyThreshold(self):
+	def set_UnhealthyThreshold(self, UnhealthyThreshold):  # Integer
+		self.add_query_param('UnhealthyThreshold', UnhealthyThreshold)
+	def get_HealthyThreshold(self): # Integer
 		return self.get_query_params().get('HealthyThreshold')
 
-	def set_HealthyThreshold(self,HealthyThreshold):
-		self.add_query_param('HealthyThreshold',HealthyThreshold)
-
-	def get_Scheduler(self):
+	def set_HealthyThreshold(self, HealthyThreshold):  # Integer
+		self.add_query_param('HealthyThreshold', HealthyThreshold)
+	def get_Scheduler(self): # String
 		return self.get_query_params().get('Scheduler')
 
-	def set_Scheduler(self,Scheduler):
-		self.add_query_param('Scheduler',Scheduler)
-
-	def get_ListenerPort(self):
+	def set_Scheduler(self, Scheduler):  # String
+		self.add_query_param('Scheduler', Scheduler)
+	def get_ListenerPort(self): # Integer
 		return self.get_query_params().get('ListenerPort')
 
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ListenerPort(self, ListenerPort):  # Integer
+		self.add_query_param('ListenerPort', ListenerPort)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_Bandwidth(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_Bandwidth(self): # Integer
 		return self.get_query_params().get('Bandwidth')
 
-	def set_Bandwidth(self,Bandwidth):
-		self.add_query_param('Bandwidth',Bandwidth)
-
-	def get_OwnerAccount(self):
+	def set_Bandwidth(self, Bandwidth):  # Integer
+		self.add_query_param('Bandwidth', Bandwidth)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_HealthCheckConnectPort(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_HealthCheckConnectPort(self): # Integer
 		return self.get_query_params().get('HealthCheckConnectPort')
 
-	def set_HealthCheckConnectPort(self,HealthCheckConnectPort):
-		self.add_query_param('HealthCheckConnectPort',HealthCheckConnectPort)
-
-	def get_VServerGroup(self):
+	def set_HealthCheckConnectPort(self, HealthCheckConnectPort):  # Integer
+		self.add_query_param('HealthCheckConnectPort', HealthCheckConnectPort)
+	def get_VServerGroup(self): # String
 		return self.get_query_params().get('VServerGroup')
 
-	def set_VServerGroup(self,VServerGroup):
-		self.add_query_param('VServerGroup',VServerGroup)
+	def set_VServerGroup(self, VServerGroup):  # String
+		self.add_query_param('VServerGroup', VServerGroup)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetServerCertificateNameRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetCACertificateNameRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,53 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class SetServerCertificateNameRequest(RpcRequest):
+class SetCACertificateNameRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetServerCertificateName','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetCACertificateName','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_CACertificateName(self): # String
+		return self.get_query_params().get('CACertificateName')
+
+	def set_CACertificateName(self, CACertificateName):  # String
+		self.add_query_param('CACertificateName', CACertificateName)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ServerCertificateId(self):
-		return self.get_query_params().get('ServerCertificateId')
-
-	def set_ServerCertificateId(self,ServerCertificateId):
-		self.add_query_param('ServerCertificateId',ServerCertificateId)
-
-	def get_ServerCertificateName(self):
-		return self.get_query_params().get('ServerCertificateName')
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_CACertificateId(self): # String
+		return self.get_query_params().get('CACertificateId')
 
-	def set_ServerCertificateName(self,ServerCertificateName):
-		self.add_query_param('ServerCertificateName',ServerCertificateName)
+	def set_CACertificateId(self, CACertificateId):  # String
+		self.add_query_param('CACertificateId', CACertificateId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetTLSCipherPolicyAttributeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetTLSCipherPolicyAttributeRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,72 +19,62 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class SetTLSCipherPolicyAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetTLSCipherPolicyAttribute','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetTLSCipherPolicyAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_access_key_id(self):
+	def get_access_key_id(self): # String
 		return self.get_query_params().get('access_key_id')
 
-	def set_access_key_id(self,access_key_id):
-		self.add_query_param('access_key_id',access_key_id)
-
-	def get_ResourceOwnerId(self):
+	def set_access_key_id(self, access_key_id):  # String
+		self.add_query_param('access_key_id', access_key_id)
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_TLSCipherPolicyId(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_TLSCipherPolicyId(self): # String
 		return self.get_query_params().get('TLSCipherPolicyId')
 
-	def set_TLSCipherPolicyId(self,TLSCipherPolicyId):
-		self.add_query_param('TLSCipherPolicyId',TLSCipherPolicyId)
-
-	def get_Cipherss(self):
+	def set_TLSCipherPolicyId(self, TLSCipherPolicyId):  # String
+		self.add_query_param('TLSCipherPolicyId', TLSCipherPolicyId)
+	def get_Cipherss(self): # RepeatList
 		return self.get_query_params().get('Ciphers')
 
-	def set_Cipherss(self, Cipherss):
-		for depth1 in range(len(Cipherss)):
-			if Cipherss[depth1] is not None:
-				self.add_query_param('Ciphers.' + str(depth1 + 1) , Cipherss[depth1])
-
-	def get_TLSVersionss(self):
+	def set_Cipherss(self, Ciphers):  # RepeatList
+		for depth1 in range(len(Ciphers)):
+			self.add_query_param('Ciphers.' + str(depth1 + 1), Ciphers[depth1])
+	def get_TLSVersionss(self): # RepeatList
 		return self.get_query_params().get('TLSVersions')
 
-	def set_TLSVersionss(self, TLSVersionss):
-		for depth1 in range(len(TLSVersionss)):
-			if TLSVersionss[depth1] is not None:
-				self.add_query_param('TLSVersions.' + str(depth1 + 1) , TLSVersionss[depth1])
-
-	def get_ResourceOwnerAccount(self):
+	def set_TLSVersionss(self, TLSVersions):  # RepeatList
+		for depth1 in range(len(TLSVersions)):
+			self.add_query_param('TLSVersions.' + str(depth1 + 1), TLSVersions[depth1])
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_Name(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_Name(self): # String
 		return self.get_query_params().get('Name')
 
-	def set_Name(self,Name):
-		self.add_query_param('Name',Name)
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/SetVServerGroupAttributeRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/DescribeMasterSlaveServerGroupAttributeRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,59 +16,43 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class SetVServerGroupAttributeRequest(RpcRequest):
+class DescribeMasterSlaveServerGroupAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetVServerGroupAttribute','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'DescribeMasterSlaveServerGroupAttribute','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_BackendServers(self):
-		return self.get_query_params().get('BackendServers')
-
-	def set_BackendServers(self,BackendServers):
-		self.add_query_param('BackendServers',BackendServers)
-
-	def get_VServerGroupId(self):
-		return self.get_query_params().get('VServerGroupId')
-
-	def set_VServerGroupId(self,VServerGroupId):
-		self.add_query_param('VServerGroupId',VServerGroupId)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_VServerGroupName(self):
-		return self.get_query_params().get('VServerGroupName')
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_MasterSlaveServerGroupId(self): # String
+		return self.get_query_params().get('MasterSlaveServerGroupId')
 
-	def set_VServerGroupName(self,VServerGroupName):
-		self.add_query_param('VServerGroupName',VServerGroupName)
+	def set_MasterSlaveServerGroupId(self, MasterSlaveServerGroupId):  # String
+		self.add_query_param('MasterSlaveServerGroupId', MasterSlaveServerGroupId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/StartLoadBalancerListenerRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/SetLoadBalancerStatusRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,59 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class StartLoadBalancerListenerRequest(RpcRequest):
+class SetLoadBalancerStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'StartLoadBalancerListener','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'SetLoadBalancerStatus','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ListenerPort(self):
-		return self.get_query_params().get('ListenerPort')
-
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ListenerProtocol(self):
-		return self.get_query_params().get('ListenerProtocol')
-
-	def set_ListenerProtocol(self,ListenerProtocol):
-		self.add_query_param('ListenerProtocol',ListenerProtocol)
-
-	def get_LoadBalancerId(self):
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_LoadBalancerStatus(self): # String
+		return self.get_query_params().get('LoadBalancerStatus')
+
+	def set_LoadBalancerStatus(self, LoadBalancerStatus):  # String
+		self.add_query_param('LoadBalancerStatus', LoadBalancerStatus)
+	def get_LoadBalancerId(self): # String
 		return self.get_query_params().get('LoadBalancerId')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/StopLoadBalancerListenerRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/ListTLSCipherPoliciesRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,59 +16,68 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class StopLoadBalancerListenerRequest(RpcRequest):
+class ListTLSCipherPoliciesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'StopLoadBalancerListener','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'ListTLSCipherPolicies','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_access_key_id(self): # String
+		return self.get_query_params().get('access_key_id')
 
-	def get_ResourceOwnerId(self):
+	def set_access_key_id(self, access_key_id):  # String
+		self.add_query_param('access_key_id', access_key_id)
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ListenerPort(self):
-		return self.get_query_params().get('ListenerPort')
-
-	def set_ListenerPort(self,ListenerPort):
-		self.add_query_param('ListenerPort',ListenerPort)
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_IncludeListener(self): # Boolean
+		return self.get_query_params().get('IncludeListener')
+
+	def set_IncludeListener(self, IncludeListener):  # Boolean
+		self.add_query_param('IncludeListener', IncludeListener)
+	def get_TLSCipherPolicyId(self): # String
+		return self.get_query_params().get('TLSCipherPolicyId')
+
+	def set_TLSCipherPolicyId(self, TLSCipherPolicyId):  # String
+		self.add_query_param('TLSCipherPolicyId', TLSCipherPolicyId)
+	def get_NextToken(self): # String
+		return self.get_query_params().get('NextToken')
+
+	def set_NextToken(self, NextToken):  # String
+		self.add_query_param('NextToken', NextToken)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ListenerProtocol(self):
-		return self.get_query_params().get('ListenerProtocol')
-
-	def set_ListenerProtocol(self,ListenerProtocol):
-		self.add_query_param('ListenerProtocol',ListenerProtocol)
-
-	def get_LoadBalancerId(self):
-		return self.get_query_params().get('LoadBalancerId')
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_Name(self): # String
+		return self.get_query_params().get('Name')
+
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
+	def get_MaxItems(self): # Integer
+		return self.get_query_params().get('MaxItems')
 
-	def set_LoadBalancerId(self,LoadBalancerId):
-		self.add_query_param('LoadBalancerId',LoadBalancerId)
+	def set_MaxItems(self, MaxItems):  # Integer
+		self.add_query_param('MaxItems', MaxItems)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/TagResourcesRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/RemoveTagsRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,65 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class TagResourcesRequest(RpcRequest):
+class RemoveTagsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'TagResources','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'RemoveTags','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_Tags(self):
-		return self.get_query_params().get('Tag')
-
-	def set_Tags(self, Tags):
-		for depth1 in range(len(Tags)):
-			if Tags[depth1].get('Value') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tags[depth1].get('Value'))
-			if Tags[depth1].get('Key') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tags[depth1].get('Key'))
-
-	def get_ResourceIds(self):
-		return self.get_query_params().get('ResourceId')
-
-	def set_ResourceIds(self, ResourceIds):
-		for depth1 in range(len(ResourceIds)):
-			if ResourceIds[depth1] is not None:
-				self.add_query_param('ResourceId.' + str(depth1 + 1) , ResourceIds[depth1])
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ResourceType(self):
-		return self.get_query_params().get('ResourceType')
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_Tags(self): # String
+		return self.get_query_params().get('Tags')
+
+	def set_Tags(self, Tags):  # String
+		self.add_query_param('Tags', Tags)
+	def get_LoadBalancerId(self): # String
+		return self.get_query_params().get('LoadBalancerId')
 
-	def set_ResourceType(self,ResourceType):
-		self.add_query_param('ResourceType',ResourceType)
+	def set_LoadBalancerId(self, LoadBalancerId):  # String
+		self.add_query_param('LoadBalancerId', LoadBalancerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/UntagResourcesRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/ModifyVServerGroupBackendServersRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,69 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
-class UntagResourcesRequest(RpcRequest):
+class ModifyVServerGroupBackendServersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'UntagResources','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'ModifyVServerGroupBackendServers','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_All(self):
-		return self.get_query_params().get('All')
-
-	def set_All(self,All):
-		self.add_query_param('All',All)
-
-	def get_ResourceIds(self):
-		return self.get_query_params().get('ResourceId')
-
-	def set_ResourceIds(self, ResourceIds):
-		for depth1 in range(len(ResourceIds)):
-			if ResourceIds[depth1] is not None:
-				self.add_query_param('ResourceId.' + str(depth1 + 1) , ResourceIds[depth1])
-
-	def get_ResourceOwnerAccount(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_VServerGroupId(self): # String
+		return self.get_query_params().get('VServerGroupId')
+
+	def set_VServerGroupId(self, VServerGroupId):  # String
+		self.add_query_param('VServerGroupId', VServerGroupId)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_NewBackendServers(self): # String
+		return self.get_query_params().get('NewBackendServers')
+
+	def set_NewBackendServers(self, NewBackendServers):  # String
+		self.add_query_param('NewBackendServers', NewBackendServers)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
-
-	def get_ResourceType(self):
-		return self.get_query_params().get('ResourceType')
-
-	def set_ResourceType(self,ResourceType):
-		self.add_query_param('ResourceType',ResourceType)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
+	def get_OldBackendServers(self): # String
+		return self.get_query_params().get('OldBackendServers')
 
-	def get_TagKeys(self):
-		return self.get_query_params().get('TagKey')
-
-	def set_TagKeys(self, TagKeys):
-		for depth1 in range(len(TagKeys)):
-			if TagKeys[depth1] is not None:
-				self.add_query_param('TagKey.' + str(depth1 + 1) , TagKeys[depth1])
+	def set_OldBackendServers(self, OldBackendServers):  # String
+		self.add_query_param('OldBackendServers', OldBackendServers)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/aliyunsdkslb/request/v20140515/UploadCACertificateRequest.py` & `aliyun-python-sdk-slb-3.3.9/aliyunsdkslb/request/v20140515/UploadCACertificateRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,56 +19,50 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkslb.endpoint import endpoint_data
 
 class UploadCACertificateRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'UploadCACertificate','slb')
-		self.set_method('POST')
+		RpcRequest.__init__(self, 'Slb', '2014-05-15', 'UploadCACertificate','Slb')
+		self.set_method('POST')
+
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-
-	def get_ResourceOwnerId(self):
+	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self,ResourceOwnerId):
-		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
-
-	def get_ResourceGroupId(self):
+	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
+		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
-	def set_ResourceGroupId(self,ResourceGroupId):
-		self.add_query_param('ResourceGroupId',ResourceGroupId)
-
-	def get_CACertificateName(self):
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_CACertificateName(self): # String
 		return self.get_query_params().get('CACertificateName')
 
-	def set_CACertificateName(self,CACertificateName):
-		self.add_query_param('CACertificateName',CACertificateName)
-
-	def get_CACertificate(self):
+	def set_CACertificateName(self, CACertificateName):  # String
+		self.add_query_param('CACertificateName', CACertificateName)
+	def get_CACertificate(self): # String
 		return self.get_query_params().get('CACertificate')
 
-	def set_CACertificate(self,CACertificate):
-		self.add_query_param('CACertificate',CACertificate)
-
-	def get_ResourceOwnerAccount(self):
+	def set_CACertificate(self, CACertificate):  # String
+		self.add_query_param('CACertificate', CACertificate)
+	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
-		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
-
-	def get_OwnerAccount(self):
+	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
+		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
+	def get_OwnerAccount(self): # String
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self,OwnerAccount):
-		self.add_query_param('OwnerAccount',OwnerAccount)
-
-	def get_OwnerId(self):
+	def set_OwnerAccount(self, OwnerAccount):  # String
+		self.add_query_param('OwnerAccount', OwnerAccount)
+	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self,OwnerId):
-		self.add_query_param('OwnerId',OwnerId)
+	def set_OwnerId(self, OwnerId):  # Long
+		self.add_query_param('OwnerId', OwnerId)
```

### Comparing `aliyun-python-sdk-slb-3.3.8/setup.py` & `aliyun-python-sdk-slb-3.3.9/setup.py`

 * *Files identical despite different names*

