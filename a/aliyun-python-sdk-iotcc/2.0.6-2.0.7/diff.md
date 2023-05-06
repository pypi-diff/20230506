# Comparing `tmp/aliyun-python-sdk-iotcc-2.0.6.tar.gz` & `tmp/aliyun-python-sdk-iotcc-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-iotcc-2.0.6.tar", last modified: Sat May  6 09:12:10 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-iotcc-2.0.7.tar", last modified: Sat May  6 09:14:12 2023, max compression
```

## Comparing `aliyun-python-sdk-iotcc-2.0.6.tar` & `aliyun-python-sdk-iotcc-2.0.7.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1547 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyun_python_sdk_iotcc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1547 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyun_python_sdk_iotcc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5668 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyun_python_sdk_iotcc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyun_python_sdk_iotcc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyun_python_sdk_iotcc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyun_python_sdk_iotcc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/
--rw-r--r--   0 root         (0) root         (0)     2099 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/AddCidrToConnectionPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/AddIoTCloudConnectorToGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2294 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/AssociateIpWithConnectionPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/AssociateVSwitchWithIoTCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ConfirmIoTCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     3455 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     3423 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2543 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateConnectionPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateDNSServiceRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     3650 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateGroupAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2752 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateGroupDNSServiceRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2571 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateGroupIpMappingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorBackhaulRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2853 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2531 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateIpMappingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2666 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateServiceEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1882 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1858 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteConnectionPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     1858 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteDNSServiceRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteGroupAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1898 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteGroupDNSServiceRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1920 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteGroupIpMappingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1677 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1637 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnetorBackhaulRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1850 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteIpMappingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteServiceEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DisableIoTCloudConnectorAccessLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2296 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DissociateIpFromConnectionPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DissociateVSwitchFromIoTCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2151 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/EnableIoTCloudConnectorAccessLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1735 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/GetConnectionPoolIpOperationResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1255 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/GetDiagnoseResultForSingleCardRequest.py
--rw-r--r--   0 root         (0) root         (0)     1649 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/GetIoTCloudConnectorAccessLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/GetStsInfoAndOssPathRequest.py
--rw-r--r--   0 root         (0) root         (0)     1285 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/GrantVirtualBorderRouterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1827 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListAPNsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4851 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListAuthorizationRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2176 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListConnectionPoolAllIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListConnectionPoolIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListConnectionPoolsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3342 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListDNSServiceRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2019 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListDiagnoseInfoForSingleCardRequest.py
--rw-r--r--   0 root         (0) root         (0)     4275 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListGroupAuthorizationRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3382 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListGroupDNSServiceRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3232 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListGroupIpMappingRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1295 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorAvailableZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1653 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorEIPsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3589 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListIoTCoudConnectorBackhaulRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     3192 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListIpMappingRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1217 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3279 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListServiceEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2491 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1902 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/MoveAuthorizationRuleToDNSServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1942 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/MoveGroupAuthorizationRuleToDNSServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/OpenIoTCloudConnectorServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/RemoveIoTCloudConnectorFromGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1637 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/RevertIoTCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2606 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/SubmitDiagnoseTaskForSingleCardRequest.py
--rw-r--r--   0 root         (0) root         (0)     3718 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateAuthorizationRuleAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateConnectionPoolAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2957 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateDNSServiceRuleAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3758 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateGroupAuthorizationRuleAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateGroupDNSServiceRuleAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2822 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateGroupIpMappingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2625 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2047 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorGroupAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2752 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateIpMappingRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateServiceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2541 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateServiceEntryAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2462 2023-05-06 09:12:10.000000 aliyun-python-sdk-iotcc-2.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      531 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyun_python_sdk_iotcc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyun_python_sdk_iotcc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5668 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyun_python_sdk_iotcc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyun_python_sdk_iotcc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyun_python_sdk_iotcc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyun_python_sdk_iotcc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/
+-rw-r--r--   0 root         (0) root         (0)     2099 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/AddCidrToConnectionPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/AddIoTCloudConnectorToGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/AssociateIpWithConnectionPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/AssociateVSwitchWithIoTCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ConfirmIoTCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3455 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3423 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateConnectionPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateDNSServiceRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3650 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateGroupAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateGroupDNSServiceRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateGroupIpMappingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorBackhaulRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateIpMappingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2666 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateServiceEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteConnectionPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteDNSServiceRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteGroupAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteGroupDNSServiceRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteGroupIpMappingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnetorBackhaulRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteIpMappingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteServiceEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DisableIoTCloudConnectorAccessLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DissociateIpFromConnectionPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DissociateVSwitchFromIoTCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/EnableIoTCloudConnectorAccessLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/GetConnectionPoolIpOperationResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/GetDiagnoseResultForSingleCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/GetIoTCloudConnectorAccessLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/GetStsInfoAndOssPathRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/GrantVirtualBorderRouterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListAPNsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListAuthorizationRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListConnectionPoolAllIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListConnectionPoolIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListConnectionPoolsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3342 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListDNSServiceRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListDiagnoseInfoForSingleCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4275 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListGroupAuthorizationRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3382 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListGroupDNSServiceRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3232 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListGroupIpMappingRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorAvailableZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorEIPsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3589 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListIoTCoudConnectorBackhaulRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListIpMappingRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1217 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3279 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListServiceEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/MoveAuthorizationRuleToDNSServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/MoveGroupAuthorizationRuleToDNSServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/OpenIoTCloudConnectorServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/RemoveIoTCloudConnectorFromGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/RevertIoTCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/SubmitDiagnoseTaskForSingleCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3718 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateAuthorizationRuleAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateConnectionPoolAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2957 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateDNSServiceRuleAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3758 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateGroupAuthorizationRuleAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateGroupDNSServiceRuleAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateGroupIpMappingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorGroupAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateIpMappingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateServiceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateServiceEntryAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-05-06 09:14:12.000000 aliyun-python-sdk-iotcc-2.0.7/setup.py
```

### Comparing `aliyun-python-sdk-iotcc-2.0.6/LICENSE` & `aliyun-python-sdk-iotcc-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/PKG-INFO` & `aliyun-python-sdk-iotcc-2.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-iotcc
-Version: 2.0.6
+Version: 2.0.7
 Summary: The iotcc module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-iotcc
```

### Comparing `aliyun-python-sdk-iotcc-2.0.6/README.rst` & `aliyun-python-sdk-iotcc-2.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyun_python_sdk_iotcc.egg-info/PKG-INFO` & `aliyun-python-sdk-iotcc-2.0.7/aliyun_python_sdk_iotcc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-iotcc
-Version: 2.0.6
+Version: 2.0.7
 Summary: The iotcc module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-iotcc
```

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyun_python_sdk_iotcc.egg-info/SOURCES.txt` & `aliyun-python-sdk-iotcc-2.0.7/aliyun_python_sdk_iotcc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/AddCidrToConnectionPoolRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/AddCidrToConnectionPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/AddIoTCloudConnectorToGroupRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/AddIoTCloudConnectorToGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/AssociateIpWithConnectionPoolRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/AssociateIpWithConnectionPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/AssociateVSwitchWithIoTCloudConnectorRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/AssociateVSwitchWithIoTCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ConfirmIoTCloudConnectorRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ConfirmIoTCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRulesRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateConnectionPoolRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateConnectionPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateDNSServiceRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateDNSServiceRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateGroupAuthorizationRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateGroupAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateGroupDNSServiceRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateGroupDNSServiceRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateGroupIpMappingRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateGroupIpMappingRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorBackhaulRouteRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorBackhaulRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorGroupRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateIpMappingRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateIpMappingRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateServiceEntryRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateServiceEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/CreateServiceRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/CreateServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRulesRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteConnectionPoolRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteConnectionPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteDNSServiceRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteDNSServiceRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteGroupAuthorizationRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteGroupAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteGroupDNSServiceRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteGroupDNSServiceRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteGroupIpMappingRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteGroupIpMappingRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorGroupRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnetorBackhaulRouteRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnetorBackhaulRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteIpMappingRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteIpMappingRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteServiceEntryRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteServiceEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DeleteServiceRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DeleteServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DisableIoTCloudConnectorAccessLogRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DisableIoTCloudConnectorAccessLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DissociateIpFromConnectionPoolRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DissociateIpFromConnectionPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/DissociateVSwitchFromIoTCloudConnectorRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/DissociateVSwitchFromIoTCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/EnableIoTCloudConnectorAccessLogRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/EnableIoTCloudConnectorAccessLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/GetConnectionPoolIpOperationResultRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/GetConnectionPoolIpOperationResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/GetDiagnoseResultForSingleCardRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/GetDiagnoseResultForSingleCardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/GetIoTCloudConnectorAccessLogRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/GetIoTCloudConnectorAccessLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/GetStsInfoAndOssPathRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/GetStsInfoAndOssPathRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/GrantVirtualBorderRouterRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/GrantVirtualBorderRouterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListAPNsRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListAPNsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListAuthorizationRulesRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListAuthorizationRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListConnectionPoolAllIpsRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListConnectionPoolAllIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListConnectionPoolIpsRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListConnectionPoolIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListConnectionPoolsRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListConnectionPoolsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListDNSServiceRulesRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListDNSServiceRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListDiagnoseInfoForSingleCardRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListDiagnoseInfoForSingleCardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListGroupAuthorizationRulesRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListGroupAuthorizationRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListGroupDNSServiceRulesRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListGroupDNSServiceRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListGroupIpMappingRulesRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListGroupIpMappingRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorAvailableZonesRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorAvailableZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorEIPsRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorEIPsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorGroupsRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorsRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListIoTCoudConnectorBackhaulRouteRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListIoTCoudConnectorBackhaulRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListIpMappingRulesRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListIpMappingRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListRegionsRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListServiceEntriesRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListServiceEntriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/ListServiceRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/ListServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/MoveAuthorizationRuleToDNSServiceRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/MoveAuthorizationRuleToDNSServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/MoveGroupAuthorizationRuleToDNSServiceRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/MoveGroupAuthorizationRuleToDNSServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/OpenIoTCloudConnectorServiceRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/OpenIoTCloudConnectorServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/RemoveIoTCloudConnectorFromGroupRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/RemoveIoTCloudConnectorFromGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/RevertIoTCloudConnectorRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/RevertIoTCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/SubmitDiagnoseTaskForSingleCardRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/SubmitDiagnoseTaskForSingleCardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateAuthorizationRuleAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateAuthorizationRuleAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateConnectionPoolAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateConnectionPoolAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateDNSServiceRuleAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateDNSServiceRuleAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateGroupAuthorizationRuleAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateGroupAuthorizationRuleAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateGroupDNSServiceRuleAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateGroupDNSServiceRuleAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateGroupIpMappingRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateGroupIpMappingRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorGroupAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorGroupAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateIpMappingRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateIpMappingRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateServiceAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateServiceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/aliyunsdkiotcc/request/v20210513/UpdateServiceEntryAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.7/aliyunsdkiotcc/request/v20210513/UpdateServiceEntryAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.6/setup.py` & `aliyun-python-sdk-iotcc-2.0.7/setup.py`

 * *Files identical despite different names*

