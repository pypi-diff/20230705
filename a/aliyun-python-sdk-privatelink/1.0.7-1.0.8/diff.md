# Comparing `tmp/aliyun-python-sdk-privatelink-1.0.7.tar.gz` & `tmp/aliyun-python-sdk-privatelink-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-privatelink-1.0.7.tar", last modified: Fri Jan  7 13:25:16 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-privatelink-1.0.8.tar", last modified: Wed Jul  5 05:41:46 2023, max compression
```

## Comparing `aliyun-python-sdk-privatelink-1.0.7.tar` & `aliyun-python-sdk-privatelink-1.0.8.tar`

### file list

```diff
@@ -1,55 +1,59 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      575 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1577 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      543 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyun_python_sdk_privatelink.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1577 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyun_python_sdk_privatelink.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3168 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyun_python_sdk_privatelink.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyun_python_sdk_privatelink.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyun_python_sdk_privatelink.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyun_python_sdk_privatelink.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/
--rw-r--r--   0 root         (0) root         (0)       21 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/
--rw-r--r--   0 root         (0) root         (0)     2069 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/AddUserToVpcEndpointServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2393 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/AddZoneToVpcEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     2314 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/AttachResourceToVpcEndpointServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2108 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/AttachSecurityGroupToVpcEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     1298 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/CheckProductOpenRequest.py
--rw-r--r--   0 root         (0) root         (0)     4285 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/CreateVpcEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     3510 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/CreateVpcEndpointServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1892 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DeleteVpcEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     1900 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DeleteVpcEndpointServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1331 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1327 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DescribeZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2318 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DetachResourceFromVpcEndpointServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2147 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DetachSecurityGroupFromVpcEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     2099 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DisableVpcEndpointConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2503 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DisableVpcEndpointZoneConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2284 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/EnableVpcEndpointConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2272 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/EnableVpcEndpointZoneConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1538 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/GetVpcEndpointAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1546 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/GetVpcEndpointServiceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3142 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointConnectionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1928 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointSecurityGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1926 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServiceResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2081 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServiceUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     2322 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServicesByEndUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     3300 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServicesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1910 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3108 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1479 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/OpenPrivateLinkServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2079 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/RemoveUserFromVpcEndpointServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2075 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/RemoveZoneFromVpcEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     2358 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2302 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointConnectionAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2868 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointServiceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2378 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointServiceResourceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3196 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointZoneConnectionResourceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2492 2022-01-07 13:25:16.000000 aliyun-python-sdk-privatelink-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      543 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyun_python_sdk_privatelink.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyun_python_sdk_privatelink.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyun_python_sdk_privatelink.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyun_python_sdk_privatelink.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyun_python_sdk_privatelink.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyun_python_sdk_privatelink.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/AddUserToVpcEndpointServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2393 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/AddZoneToVpcEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/AttachResourceToVpcEndpointServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/AttachSecurityGroupToVpcEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ChangeResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/CheckProductOpenRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/CheckResourceSupportOperateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4925 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/CreateVpcEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/CreateVpcEndpointServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DeleteVpcEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1900 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DeleteVpcEndpointServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1327 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DescribeZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DetachResourceFromVpcEndpointServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DetachSecurityGroupFromVpcEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2099 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DisableVpcEndpointConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2503 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DisableVpcEndpointZoneConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/EnableVpcEndpointConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/EnableVpcEndpointZoneConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1538 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/GetVpcEndpointAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1546 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/GetVpcEndpointServiceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3562 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointConnectionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1928 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointSecurityGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServiceResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2284 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServiceUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServicesByEndUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4106 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3723 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/NotifyResourceAddressFamilyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/OpenPrivateLinkServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/RemoveUserFromVpcEndpointServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2075 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/RemoveZoneFromVpcEndpointRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointConnectionAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointServiceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointServiceResourceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3196 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointZoneConnectionResourceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-07-05 05:41:46.000000 aliyun-python-sdk-privatelink-1.0.8/setup.py
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/LICENSE` & `aliyun-python-sdk-privatelink-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/PKG-INFO` & `aliyun-python-sdk-privatelink-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-privatelink
-Version: 1.0.7
+Version: 1.0.8
 Summary: The privatelink module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-privatelink
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/README.rst` & `aliyun-python-sdk-privatelink-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyun_python_sdk_privatelink.egg-info/PKG-INFO` & `aliyun-python-sdk-privatelink-1.0.8/aliyun_python_sdk_privatelink.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-privatelink
-Version: 1.0.7
+Version: 1.0.8
 Summary: The privatelink module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-privatelink
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyun_python_sdk_privatelink.egg-info/SOURCES.txt` & `aliyun-python-sdk-privatelink-1.0.8/aliyun_python_sdk_privatelink.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 aliyunsdkprivatelink/__init__.py
 aliyunsdkprivatelink/endpoint.py
 aliyunsdkprivatelink/request/__init__.py
 aliyunsdkprivatelink/request/v20200415/AddUserToVpcEndpointServiceRequest.py
 aliyunsdkprivatelink/request/v20200415/AddZoneToVpcEndpointRequest.py
 aliyunsdkprivatelink/request/v20200415/AttachResourceToVpcEndpointServiceRequest.py
 aliyunsdkprivatelink/request/v20200415/AttachSecurityGroupToVpcEndpointRequest.py
+aliyunsdkprivatelink/request/v20200415/ChangeResourceGroupRequest.py
 aliyunsdkprivatelink/request/v20200415/CheckProductOpenRequest.py
+aliyunsdkprivatelink/request/v20200415/CheckResourceSupportOperateRequest.py
 aliyunsdkprivatelink/request/v20200415/CreateVpcEndpointRequest.py
 aliyunsdkprivatelink/request/v20200415/CreateVpcEndpointServiceRequest.py
 aliyunsdkprivatelink/request/v20200415/DeleteVpcEndpointRequest.py
 aliyunsdkprivatelink/request/v20200415/DeleteVpcEndpointServiceRequest.py
 aliyunsdkprivatelink/request/v20200415/DescribeRegionsRequest.py
 aliyunsdkprivatelink/request/v20200415/DescribeZonesRequest.py
 aliyunsdkprivatelink/request/v20200415/DetachResourceFromVpcEndpointServiceRequest.py
@@ -34,16 +36,18 @@
 aliyunsdkprivatelink/request/v20200415/ListVpcEndpointSecurityGroupsRequest.py
 aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServiceResourcesRequest.py
 aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServiceUsersRequest.py
 aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServicesByEndUserRequest.py
 aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServicesRequest.py
 aliyunsdkprivatelink/request/v20200415/ListVpcEndpointZonesRequest.py
 aliyunsdkprivatelink/request/v20200415/ListVpcEndpointsRequest.py
+aliyunsdkprivatelink/request/v20200415/NotifyResourceAddressFamilyRequest.py
 aliyunsdkprivatelink/request/v20200415/OpenPrivateLinkServiceRequest.py
 aliyunsdkprivatelink/request/v20200415/RemoveUserFromVpcEndpointServiceRequest.py
 aliyunsdkprivatelink/request/v20200415/RemoveZoneFromVpcEndpointRequest.py
+aliyunsdkprivatelink/request/v20200415/TagResourcesRequest.py
 aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointAttributeRequest.py
 aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointConnectionAttributeRequest.py
 aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointServiceAttributeRequest.py
 aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointServiceResourceAttributeRequest.py
 aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointZoneConnectionResourceAttributeRequest.py
 aliyunsdkprivatelink/request/v20200415/__init__.py
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/endpoint.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/AddUserToVpcEndpointServiceRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/RemoveUserFromVpcEndpointServiceRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,31 +16,36 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkprivatelink.endpoint import endpoint_data
 
-class AddUserToVpcEndpointServiceRequest(RpcRequest):
+class RemoveUserFromVpcEndpointServiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'AddUserToVpcEndpointService','privatelink')
+		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'RemoveUserFromVpcEndpointService','privatelink')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
+	def get_UserARN(self): # String
+		return self.get_query_params().get('UserARN')
+
+	def set_UserARN(self, UserARN):  # String
+		self.add_query_param('UserARN', UserARN)
 	def get_UserId(self): # Long
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # Long
 		self.add_query_param('UserId', UserId)
 	def get_DryRun(self): # Boolean
 		return self.get_query_params().get('DryRun')
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/AddZoneToVpcEndpointRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/AddZoneToVpcEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/AttachResourceToVpcEndpointServiceRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/AttachResourceToVpcEndpointServiceRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,12 +48,17 @@
 	def set_DryRun(self, DryRun):  # Boolean
 		self.add_query_param('DryRun', DryRun)
 	def get_ResourceType(self): # String
 		return self.get_query_params().get('ResourceType')
 
 	def set_ResourceType(self, ResourceType):  # String
 		self.add_query_param('ResourceType', ResourceType)
+	def get_ZoneId(self): # String
+		return self.get_query_params().get('ZoneId')
+
+	def set_ZoneId(self, ZoneId):  # String
+		self.add_query_param('ZoneId', ZoneId)
 	def get_ServiceId(self): # String
 		return self.get_query_params().get('ServiceId')
 
 	def set_ServiceId(self, ServiceId):  # String
 		self.add_query_param('ServiceId', ServiceId)
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/AttachSecurityGroupToVpcEndpointRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/AttachSecurityGroupToVpcEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/CheckProductOpenRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/CheckProductOpenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/CreateVpcEndpointRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/CreateVpcEndpointRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,19 @@
 		self.add_query_param('ClientToken', ClientToken)
 	def get_SecurityGroupIds(self): # RepeatList
 		return self.get_query_params().get('SecurityGroupId')
 
 	def set_SecurityGroupIds(self, SecurityGroupId):  # RepeatList
 		for depth1 in range(len(SecurityGroupId)):
 			self.add_query_param('SecurityGroupId.' + str(depth1 + 1), SecurityGroupId[depth1])
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_EndpointType(self): # String
 		return self.get_query_params().get('EndpointType')
 
 	def set_EndpointType(self, EndpointType):  # String
 		self.add_query_param('EndpointType', EndpointType)
 	def get_Zones(self): # RepeatList
 		return self.get_query_params().get('Zone')
@@ -60,14 +65,23 @@
 			if Zone[depth1].get('ip') is not None:
 				self.add_query_param('Zone.' + str(depth1 + 1) + '.ip', Zone[depth1].get('ip'))
 	def get_ServiceName(self): # String
 		return self.get_query_params().get('ServiceName')
 
 	def set_ServiceName(self, ServiceName):  # String
 		self.add_query_param('ServiceName', ServiceName)
+	def get_Tags(self): # RepeatList
+		return self.get_query_params().get('Tag')
+
+	def set_Tags(self, Tag):  # RepeatList
+		for depth1 in range(len(Tag)):
+			if Tag[depth1].get('Key') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
+			if Tag[depth1].get('Value') is not None:
+				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
 	def get_DryRun(self): # Boolean
 		return self.get_query_params().get('DryRun')
 
 	def set_DryRun(self, DryRun):  # Boolean
 		self.add_query_param('DryRun', DryRun)
 	def get_EndpointDescription(self): # String
 		return self.get_query_params().get('EndpointDescription')
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/CreateVpcEndpointServiceRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointServiceResourceAttributeRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,65 +16,49 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkprivatelink.endpoint import endpoint_data
 
-class CreateVpcEndpointServiceRequest(RpcRequest):
+class UpdateVpcEndpointServiceResourceAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'CreateVpcEndpointService','privatelink')
+		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'UpdateVpcEndpointServiceResourceAttribute','privatelink')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_AutoAcceptEnabled(self): # Boolean
-		return self.get_query_params().get('AutoAcceptEnabled')
-
-	def set_AutoAcceptEnabled(self, AutoAcceptEnabled):  # Boolean
-		self.add_query_param('AutoAcceptEnabled', AutoAcceptEnabled)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
-	def get_Payer(self): # String
-		return self.get_query_params().get('Payer')
+	def get_AutoAllocatedEnabled(self): # Boolean
+		return self.get_query_params().get('AutoAllocatedEnabled')
 
-	def set_Payer(self, Payer):  # String
-		self.add_query_param('Payer', Payer)
-	def get_ZoneAffinityEnabled(self): # Boolean
-		return self.get_query_params().get('ZoneAffinityEnabled')
+	def set_AutoAllocatedEnabled(self, AutoAllocatedEnabled):  # Boolean
+		self.add_query_param('AutoAllocatedEnabled', AutoAllocatedEnabled)
+	def get_ResourceId(self): # String
+		return self.get_query_params().get('ResourceId')
 
-	def set_ZoneAffinityEnabled(self, ZoneAffinityEnabled):  # Boolean
-		self.add_query_param('ZoneAffinityEnabled', ZoneAffinityEnabled)
+	def set_ResourceId(self, ResourceId):  # String
+		self.add_query_param('ResourceId', ResourceId)
 	def get_DryRun(self): # Boolean
 		return self.get_query_params().get('DryRun')
 
 	def set_DryRun(self, DryRun):  # Boolean
 		self.add_query_param('DryRun', DryRun)
-	def get_Resources(self): # RepeatList
-		return self.get_query_params().get('Resource')
+	def get_ZoneId(self): # String
+		return self.get_query_params().get('ZoneId')
 
-	def set_Resources(self, Resource):  # RepeatList
-		for depth1 in range(len(Resource)):
-			if Resource[depth1].get('ResourceType') is not None:
-				self.add_query_param('Resource.' + str(depth1 + 1) + '.ResourceType', Resource[depth1].get('ResourceType'))
-			if Resource[depth1].get('ResourceId') is not None:
-				self.add_query_param('Resource.' + str(depth1 + 1) + '.ResourceId', Resource[depth1].get('ResourceId'))
-			if Resource[depth1].get('ZoneId') is not None:
-				self.add_query_param('Resource.' + str(depth1 + 1) + '.ZoneId', Resource[depth1].get('ZoneId'))
-	def get_ServiceResourceType(self): # String
-		return self.get_query_params().get('ServiceResourceType')
-
-	def set_ServiceResourceType(self, ServiceResourceType):  # String
-		self.add_query_param('ServiceResourceType', ServiceResourceType)
-	def get_ServiceDescription(self): # String
-		return self.get_query_params().get('ServiceDescription')
+	def set_ZoneId(self, ZoneId):  # String
+		self.add_query_param('ZoneId', ZoneId)
+	def get_ServiceId(self): # String
+		return self.get_query_params().get('ServiceId')
 
-	def set_ServiceDescription(self, ServiceDescription):  # String
-		self.add_query_param('ServiceDescription', ServiceDescription)
+	def set_ServiceId(self, ServiceId):  # String
+		self.add_query_param('ServiceId', ServiceId)
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DeleteVpcEndpointRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DeleteVpcEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DeleteVpcEndpointServiceRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DeleteVpcEndpointServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DescribeRegionsRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DescribeRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DescribeZonesRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DescribeZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DetachResourceFromVpcEndpointServiceRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/CheckResourceSupportOperateRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,44 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkprivatelink.endpoint import endpoint_data
 
-class DetachResourceFromVpcEndpointServiceRequest(RpcRequest):
+class CheckResourceSupportOperateRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'DetachResourceFromVpcEndpointService','privatelink')
-		self.set_protocol_type('https')
+		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'CheckResourceSupportOperate','privatelink')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ClientToken(self): # String
-		return self.get_query_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_query_param('ClientToken', ClientToken)
 	def get_ResourceId(self): # String
 		return self.get_query_params().get('ResourceId')
 
 	def set_ResourceId(self, ResourceId):  # String
 		self.add_query_param('ResourceId', ResourceId)
-	def get_DryRun(self): # Boolean
-		return self.get_query_params().get('DryRun')
+	def get_ZoneId(self): # String
+		return self.get_query_params().get('ZoneId')
 
-	def set_DryRun(self, DryRun):  # Boolean
-		self.add_query_param('DryRun', DryRun)
+	def set_ZoneId(self, ZoneId):  # String
+		self.add_query_param('ZoneId', ZoneId)
 	def get_ResourceType(self): # String
 		return self.get_query_params().get('ResourceType')
 
 	def set_ResourceType(self, ResourceType):  # String
 		self.add_query_param('ResourceType', ResourceType)
-	def get_ServiceId(self): # String
-		return self.get_query_params().get('ServiceId')
-
-	def set_ServiceId(self, ServiceId):  # String
-		self.add_query_param('ServiceId', ServiceId)
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DetachSecurityGroupFromVpcEndpointRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DetachSecurityGroupFromVpcEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DisableVpcEndpointConnectionRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DisableVpcEndpointConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/DisableVpcEndpointZoneConnectionRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DisableVpcEndpointZoneConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/EnableVpcEndpointConnectionRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/EnableVpcEndpointConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/EnableVpcEndpointZoneConnectionRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/EnableVpcEndpointZoneConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/GetVpcEndpointAttributeRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/GetVpcEndpointAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/GetVpcEndpointServiceAttributeRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/GetVpcEndpointServiceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointConnectionsRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointConnectionsRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,19 +43,29 @@
 	def set_EndpointOwnerId(self, EndpointOwnerId):  # Long
 		self.add_query_param('EndpointOwnerId', EndpointOwnerId)
 	def get_ReplacedResourceId(self): # String
 		return self.get_query_params().get('ReplacedResourceId')
 
 	def set_ReplacedResourceId(self, ReplacedResourceId):  # String
 		self.add_query_param('ReplacedResourceId', ReplacedResourceId)
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
+	def get_ConnectionId(self): # Long
+		return self.get_query_params().get('ConnectionId')
+
+	def set_ConnectionId(self, ConnectionId):  # Long
+		self.add_query_param('ConnectionId', ConnectionId)
 	def get_ResourceId(self): # String
 		return self.get_query_params().get('ResourceId')
 
 	def set_ResourceId(self, ResourceId):  # String
 		self.add_query_param('ResourceId', ResourceId)
 	def get_ConnectionStatus(self): # String
 		return self.get_query_params().get('ConnectionStatus')
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointSecurityGroupsRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointSecurityGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServiceResourcesRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServiceResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServiceUsersRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServiceUsersRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,19 @@
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_UserListType(self): # String
+		return self.get_query_params().get('UserListType')
+
+	def set_UserListType(self, UserListType):  # String
+		self.add_query_param('UserListType', UserListType)
 	def get_UserId(self): # Long
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # Long
 		self.add_query_param('UserId', UserId)
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServicesByEndUserRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServicesByEndUserRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,24 +28,38 @@
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
 	def get_ServiceName(self): # String
 		return self.get_query_params().get('ServiceName')
 
 	def set_ServiceName(self, ServiceName):  # String
 		self.add_query_param('ServiceName', ServiceName)
+	def get_Tag(self): # Array
+		return self.get_query_params().get('Tag')
+
+	def set_Tag(self, Tag):  # Array
+		for index1, value1 in enumerate(Tag):
+			if value1.get('Key') is not None:
+				self.add_query_param('Tag.' + str(index1 + 1) + '.Key', value1.get('Key'))
+			if value1.get('Value') is not None:
+				self.add_query_param('Tag.' + str(index1 + 1) + '.Value', value1.get('Value'))
 	def get_ServiceType(self): # String
 		return self.get_query_params().get('ServiceType')
 
 	def set_ServiceType(self, ServiceType):  # String
 		self.add_query_param('ServiceType', ServiceType)
 	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointServicesRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointServiceAttributeRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,64 +16,59 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkprivatelink.endpoint import endpoint_data
 
-class ListVpcEndpointServicesRequest(RpcRequest):
+class UpdateVpcEndpointServiceAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'ListVpcEndpointServices','privatelink')
+		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'UpdateVpcEndpointServiceAttribute','privatelink')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ServiceBusinessStatus(self): # String
-		return self.get_query_params().get('ServiceBusinessStatus')
-
-	def set_ServiceBusinessStatus(self, ServiceBusinessStatus):  # String
-		self.add_query_param('ServiceBusinessStatus', ServiceBusinessStatus)
 	def get_AutoAcceptEnabled(self): # Boolean
 		return self.get_query_params().get('AutoAcceptEnabled')
 
 	def set_AutoAcceptEnabled(self, AutoAcceptEnabled):  # Boolean
 		self.add_query_param('AutoAcceptEnabled', AutoAcceptEnabled)
-	def get_ServiceStatus(self): # String
-		return self.get_query_params().get('ServiceStatus')
+	def get_ClientToken(self): # String
+		return self.get_query_params().get('ClientToken')
 
-	def set_ServiceStatus(self, ServiceStatus):  # String
-		self.add_query_param('ServiceStatus', ServiceStatus)
-	def get_NextToken(self): # String
-		return self.get_query_params().get('NextToken')
+	def set_ClientToken(self, ClientToken):  # String
+		self.add_query_param('ClientToken', ClientToken)
+	def get_ConnectBandwidth(self): # Integer
+		return self.get_query_params().get('ConnectBandwidth')
 
-	def set_NextToken(self, NextToken):  # String
-		self.add_query_param('NextToken', NextToken)
+	def set_ConnectBandwidth(self, ConnectBandwidth):  # Integer
+		self.add_query_param('ConnectBandwidth', ConnectBandwidth)
 	def get_ZoneAffinityEnabled(self): # Boolean
 		return self.get_query_params().get('ZoneAffinityEnabled')
 
 	def set_ZoneAffinityEnabled(self, ZoneAffinityEnabled):  # Boolean
 		self.add_query_param('ZoneAffinityEnabled', ZoneAffinityEnabled)
-	def get_ServiceName(self): # String
-		return self.get_query_params().get('ServiceName')
+	def get_DryRun(self): # Boolean
+		return self.get_query_params().get('DryRun')
 
-	def set_ServiceName(self, ServiceName):  # String
-		self.add_query_param('ServiceName', ServiceName)
-	def get_ServiceResourceType(self): # String
-		return self.get_query_params().get('ServiceResourceType')
-
-	def set_ServiceResourceType(self, ServiceResourceType):  # String
-		self.add_query_param('ServiceResourceType', ServiceResourceType)
-	def get_MaxResults(self): # Integer
-		return self.get_query_params().get('MaxResults')
+	def set_DryRun(self, DryRun):  # Boolean
+		self.add_query_param('DryRun', DryRun)
+	def get_ServiceSupportIPv6(self): # Boolean
+		return self.get_query_params().get('ServiceSupportIPv6')
+
+	def set_ServiceSupportIPv6(self, ServiceSupportIPv6):  # Boolean
+		self.add_query_param('ServiceSupportIPv6', ServiceSupportIPv6)
+	def get_ServiceDescription(self): # String
+		return self.get_query_params().get('ServiceDescription')
 
-	def set_MaxResults(self, MaxResults):  # Integer
-		self.add_query_param('MaxResults', MaxResults)
+	def set_ServiceDescription(self, ServiceDescription):  # String
+		self.add_query_param('ServiceDescription', ServiceDescription)
 	def get_ServiceId(self): # String
 		return self.get_query_params().get('ServiceId')
 
 	def set_ServiceId(self, ServiceId):  # String
 		self.add_query_param('ServiceId', ServiceId)
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointZonesRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointsRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/ListVpcEndpointsRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,14 +38,19 @@
 	def set_EndpointId(self, EndpointId):  # String
 		self.add_query_param('EndpointId', EndpointId)
 	def get_EndpointStatus(self): # String
 		return self.get_query_params().get('EndpointStatus')
 
 	def set_EndpointStatus(self, EndpointStatus):  # String
 		self.add_query_param('EndpointStatus', EndpointStatus)
+	def get_ResourceGroupId(self): # String
+		return self.get_query_params().get('ResourceGroupId')
+
+	def set_ResourceGroupId(self, ResourceGroupId):  # String
+		self.add_query_param('ResourceGroupId', ResourceGroupId)
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
 	def get_EndpointType(self): # String
 		return self.get_query_params().get('EndpointType')
@@ -53,14 +58,23 @@
 	def set_EndpointType(self, EndpointType):  # String
 		self.add_query_param('EndpointType', EndpointType)
 	def get_ServiceName(self): # String
 		return self.get_query_params().get('ServiceName')
 
 	def set_ServiceName(self, ServiceName):  # String
 		self.add_query_param('ServiceName', ServiceName)
+	def get_Tag(self): # Array
+		return self.get_query_params().get('Tag')
+
+	def set_Tag(self, Tag):  # Array
+		for index1, value1 in enumerate(Tag):
+			if value1.get('Key') is not None:
+				self.add_query_param('Tag.' + str(index1 + 1) + '.Key', value1.get('Key'))
+			if value1.get('Value') is not None:
+				self.add_query_param('Tag.' + str(index1 + 1) + '.Value', value1.get('Value'))
 	def get_ConnectionStatus(self): # String
 		return self.get_query_params().get('ConnectionStatus')
 
 	def set_ConnectionStatus(self, ConnectionStatus):  # String
 		self.add_query_param('ConnectionStatus', ConnectionStatus)
 	def get_VpcId(self): # String
 		return self.get_query_params().get('VpcId')
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/OpenPrivateLinkServiceRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/OpenPrivateLinkServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/RemoveUserFromVpcEndpointServiceRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/AddUserToVpcEndpointServiceRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,31 +16,36 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkprivatelink.endpoint import endpoint_data
 
-class RemoveUserFromVpcEndpointServiceRequest(RpcRequest):
+class AddUserToVpcEndpointServiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'RemoveUserFromVpcEndpointService','privatelink')
+		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'AddUserToVpcEndpointService','privatelink')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
+	def get_UserARN(self): # String
+		return self.get_query_params().get('UserARN')
+
+	def set_UserARN(self, UserARN):  # String
+		self.add_query_param('UserARN', UserARN)
 	def get_UserId(self): # Long
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self, UserId):  # Long
 		self.add_query_param('UserId', UserId)
 	def get_DryRun(self): # Boolean
 		return self.get_query_params().get('DryRun')
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/RemoveZoneFromVpcEndpointRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/RemoveZoneFromVpcEndpointRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointAttributeRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointConnectionAttributeRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointConnectionAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointServiceAttributeRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/DetachResourceFromVpcEndpointServiceRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,54 +16,49 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkprivatelink.endpoint import endpoint_data
 
-class UpdateVpcEndpointServiceAttributeRequest(RpcRequest):
+class DetachResourceFromVpcEndpointServiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'UpdateVpcEndpointServiceAttribute','privatelink')
+		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'DetachResourceFromVpcEndpointService','privatelink')
 		self.set_protocol_type('https')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_AutoAcceptEnabled(self): # Boolean
-		return self.get_query_params().get('AutoAcceptEnabled')
-
-	def set_AutoAcceptEnabled(self, AutoAcceptEnabled):  # Boolean
-		self.add_query_param('AutoAcceptEnabled', AutoAcceptEnabled)
 	def get_ClientToken(self): # String
 		return self.get_query_params().get('ClientToken')
 
 	def set_ClientToken(self, ClientToken):  # String
 		self.add_query_param('ClientToken', ClientToken)
-	def get_ConnectBandwidth(self): # Integer
-		return self.get_query_params().get('ConnectBandwidth')
-
-	def set_ConnectBandwidth(self, ConnectBandwidth):  # Integer
-		self.add_query_param('ConnectBandwidth', ConnectBandwidth)
-	def get_ZoneAffinityEnabled(self): # Boolean
-		return self.get_query_params().get('ZoneAffinityEnabled')
+	def get_ResourceId(self): # String
+		return self.get_query_params().get('ResourceId')
 
-	def set_ZoneAffinityEnabled(self, ZoneAffinityEnabled):  # Boolean
-		self.add_query_param('ZoneAffinityEnabled', ZoneAffinityEnabled)
+	def set_ResourceId(self, ResourceId):  # String
+		self.add_query_param('ResourceId', ResourceId)
 	def get_DryRun(self): # Boolean
 		return self.get_query_params().get('DryRun')
 
 	def set_DryRun(self, DryRun):  # Boolean
 		self.add_query_param('DryRun', DryRun)
-	def get_ServiceDescription(self): # String
-		return self.get_query_params().get('ServiceDescription')
+	def get_ResourceType(self): # String
+		return self.get_query_params().get('ResourceType')
+
+	def set_ResourceType(self, ResourceType):  # String
+		self.add_query_param('ResourceType', ResourceType)
+	def get_ZoneId(self): # String
+		return self.get_query_params().get('ZoneId')
 
-	def set_ServiceDescription(self, ServiceDescription):  # String
-		self.add_query_param('ServiceDescription', ServiceDescription)
+	def set_ZoneId(self, ZoneId):  # String
+		self.add_query_param('ZoneId', ZoneId)
 	def get_ServiceId(self): # String
 		return self.get_query_params().get('ServiceId')
 
 	def set_ServiceId(self, ServiceId):  # String
 		self.add_query_param('ServiceId', ServiceId)
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointServiceResourceAttributeRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/NotifyResourceAddressFamilyRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,44 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkprivatelink.endpoint import endpoint_data
 
-class UpdateVpcEndpointServiceResourceAttributeRequest(RpcRequest):
+class NotifyResourceAddressFamilyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'UpdateVpcEndpointServiceResourceAttribute','privatelink')
-		self.set_protocol_type('https')
+		RpcRequest.__init__(self, 'Privatelink', '2020-04-15', 'NotifyResourceAddressFamily','privatelink')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ClientToken(self): # String
-		return self.get_query_params().get('ClientToken')
-
-	def set_ClientToken(self, ClientToken):  # String
-		self.add_query_param('ClientToken', ClientToken)
-	def get_AutoAllocatedEnabled(self): # Boolean
-		return self.get_query_params().get('AutoAllocatedEnabled')
-
-	def set_AutoAllocatedEnabled(self, AutoAllocatedEnabled):  # Boolean
-		self.add_query_param('AutoAllocatedEnabled', AutoAllocatedEnabled)
 	def get_ResourceId(self): # String
 		return self.get_query_params().get('ResourceId')
 
 	def set_ResourceId(self, ResourceId):  # String
 		self.add_query_param('ResourceId', ResourceId)
-	def get_DryRun(self): # Boolean
-		return self.get_query_params().get('DryRun')
+	def get_ResourceType(self): # String
+		return self.get_query_params().get('ResourceType')
 
-	def set_DryRun(self, DryRun):  # Boolean
-		self.add_query_param('DryRun', DryRun)
-	def get_ServiceId(self): # String
-		return self.get_query_params().get('ServiceId')
+	def set_ResourceType(self, ResourceType):  # String
+		self.add_query_param('ResourceType', ResourceType)
+	def get_AddressFamily(self): # String
+		return self.get_query_params().get('AddressFamily')
+
+	def set_AddressFamily(self, AddressFamily):  # String
+		self.add_query_param('AddressFamily', AddressFamily)
+	def get_Ipv6Address(self): # String
+		return self.get_query_params().get('Ipv6Address')
 
-	def set_ServiceId(self, ServiceId):  # String
-		self.add_query_param('ServiceId', ServiceId)
+	def set_Ipv6Address(self, Ipv6Address):  # String
+		self.add_query_param('Ipv6Address', Ipv6Address)
```

### Comparing `aliyun-python-sdk-privatelink-1.0.7/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointZoneConnectionResourceAttributeRequest.py` & `aliyun-python-sdk-privatelink-1.0.8/aliyunsdkprivatelink/request/v20200415/UpdateVpcEndpointZoneConnectionResourceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-privatelink-1.0.7/setup.py` & `aliyun-python-sdk-privatelink-1.0.8/setup.py`

 * *Files identical despite different names*

