# Comparing `tmp/magnum_cluster_api-0.7.2.tar.gz` & `tmp/magnum_cluster_api-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnum_cluster_api-0.7.2.tar", max compression
+gzip compressed data, was "magnum_cluster_api-0.8.0.tar", max compression
```

## Comparing `magnum_cluster_api-0.7.2.tar` & `magnum_cluster_api-0.8.0.tar`

### file list

```diff
@@ -1,78 +1,83 @@
--rw-r--r--   0        0        0    10142 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/LICENSE
--rw-r--r--   0        0        0     2795 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/README.md
--rw-r--r--   0        0        0        0 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/.gitkeep
--rw-r--r--   0        0        0      349 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
--rw-r--r--   0        0        0      437 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
--rw-r--r--   0        0        0    29122 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/README.md
--rw-r--r--   0        0        0    14987 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
--rw-r--r--   0        0        0      827 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
--rw-r--r--   0        0        0     4034 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
--rw-r--r--   0        0        0     2982 2023-07-02 04:13:10.249582 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
--rw-r--r--   0        0        0      534 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
--rw-r--r--   0        0        0    13204 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
--rw-r--r--   0        0        0      508 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
--rw-r--r--   0        0        0      972 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
--rw-r--r--   0        0        0      758 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
--rw-r--r--   0        0        0      564 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1807 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
--rw-r--r--   0        0        0      527 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
--rw-r--r--   0        0        0      989 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
--rw-r--r--   0        0        0     1180 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
--rw-r--r--   0        0        0      528 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      960 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
--rw-r--r--   0        0        0      663 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
--rw-r--r--   0        0        0    18003 2023-07-02 04:13:10.225581 magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
--rw-r--r--   0        0        0     1977 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/clients.py
--rw-r--r--   0        0        0        0 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/cmd/__init__.py
--rw-r--r--   0        0        0     4019 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/cmd/image_builder.py
--rw-r--r--   0        0        0     4714 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/cmd/image_loader.py
--rw-r--r--   0        0        0      956 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/cmd/proxy.py
--rw-r--r--   0        0        0     3278 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/conf.py
--rw-r--r--   0        0        0    14251 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/driver.py
--rw-r--r--   0        0        0     1219 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/exceptions.py
--rw-r--r--   0        0        0     3486 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/helm.py
--rw-r--r--   0        0        0     3464 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/image_utils.py
--rw-r--r--   0        0        0     1116 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/images.py
--rw-r--r--   0        0        0        0 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/__init__.py
--rw-r--r--   0        0        0     4941 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/audit/policy.yaml
--rw-r--r--   0        0        0   235191 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/calico/v3.24.2.yaml
--rw-r--r--   0        0        0      623 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
--rw-r--r--   0        0        0     1430 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
--rw-r--r--   0        0        0     2263 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
--rw-r--r--   0        0        0     4506 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     4034 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml
--rw-r--r--   0        0        0      609 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     3307 2023-07-02 04:13:09.009533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml
--rw-r--r--   0        0        0      194 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/cinder-csi/csi-cinder-driver.yaml
--rw-r--r--   0        0        0     3377 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     3944 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml
--rw-r--r--   0        0        0     1513 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     2988 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml
--rw-r--r--   0        0        0      143 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/manila-csi/csidriver.yaml
--rw-r--r--   0        0        0     3127 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml
--rw-r--r--   0        0        0      170 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/nfs-csi/csi-nfs-driverinfo.yaml
--rw-r--r--   0        0        0     3530 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml
--rw-r--r--   0        0        0     1423 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml
--rw-r--r--   0        0        0     1526 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/monitor.py
--rw-r--r--   0        0        0     5673 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/objects.py
--rw-r--r--   0        0        0      828 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/privsep/__init__.py
--rw-r--r--   0        0        0     1333 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/privsep/haproxy.py
--rw-r--r--   0        0        0    11719 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/proxy/manager.py
--rw-r--r--   0        0        0     3616 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/proxy/structs.py
--rw-r--r--   0        0        0      580 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
--rw-r--r--   0        0        0     1511 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/proxy/utils.py
--rw-r--r--   0        0        0    85235 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/resources.py
--rw-r--r--   0        0        0     1492 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/service.py
--rw-r--r--   0        0        0     3119 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/tests/functional/conftest.py
--rw-r--r--   0        0        0      666 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/tests/functional/test_clusters.py
--rw-r--r--   0        0        0      942 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/conftest.py
--rw-r--r--   0        0        0     3813 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/test_helm.py
--rw-r--r--   0        0        0     1731 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/test_image_utils.py
--rw-r--r--   0        0        0     2759 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/test_images.py
--rw-r--r--   0        0        0     5366 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/test_objects.py
--rw-r--r--   0        0        0     1717 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/test_resources.py
--rw-r--r--   0        0        0     1192 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/test_utils.py
--rw-r--r--   0        0        0    10474 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/magnum_cluster_api/utils.py
--rw-r--r--   0        0        0     1220 2023-07-02 04:13:09.013533 magnum_cluster_api-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 magnum_cluster_api-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3353 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/.gitkeep
+-rw-r--r--   0        0        0      349 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
+-rw-r--r--   0        0        0      437 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
+-rw-r--r--   0        0        0    29122 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/README.md
+-rw-r--r--   0        0        0    14987 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
+-rw-r--r--   0        0        0      827 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
+-rw-r--r--   0        0        0     4034 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2982 2023-07-05 04:18:35.571678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
+-rw-r--r--   0        0        0      534 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
+-rw-r--r--   0        0        0    13204 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
+-rw-r--r--   0        0        0      508 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
+-rw-r--r--   0        0        0      972 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
+-rw-r--r--   0        0        0      758 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
+-rw-r--r--   0        0        0      564 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1807 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
+-rw-r--r--   0        0        0      527 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
+-rw-r--r--   0        0        0      989 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
+-rw-r--r--   0        0        0     1180 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
+-rw-r--r--   0        0        0      528 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      960 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0      663 2023-07-05 04:18:35.515678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
+-rw-r--r--   0        0        0    18003 2023-07-05 04:18:35.511678 magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
+-rw-r--r--   0        0        0     1977 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/clients.py
+-rw-r--r--   0        0        0        0 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/cmd/__init__.py
+-rw-r--r--   0        0        0     5005 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/cmd/image_builder.py
+-rw-r--r--   0        0        0     4713 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/cmd/image_loader.py
+-rw-r--r--   0        0        0      956 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/cmd/proxy.py
+-rw-r--r--   0        0        0     3460 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/conf.py
+-rw-r--r--   0        0        0    14117 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/driver.py
+-rw-r--r--   0        0        0     1219 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/exceptions.py
+-rw-r--r--   0        0        0     3486 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/helm.py
+-rw-r--r--   0        0        0     3460 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/image_utils.py
+-rw-r--r--   0        0        0     1116 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/images.py
+-rw-r--r--   0        0        0        0 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/__init__.py
+-rw-r--r--   0        0        0     1759 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/cinder.py
+-rw-r--r--   0        0        0      839 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/cloud_provider.py
+-rw-r--r--   0        0        0     3012 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/common.py
+-rw-r--r--   0        0        0      948 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/integrations/manila.py
+-rw-r--r--   0        0        0        0 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/__init__.py
+-rw-r--r--   0        0        0     4941 2023-07-05 04:18:34.671672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/audit/policy.yaml
+-rw-r--r--   0        0        0   235191 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml
+-rw-r--r--   0        0        0      623 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
+-rw-r--r--   0        0        0     1430 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
+-rw-r--r--   0        0        0     2263 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
+-rw-r--r--   0        0        0     4506 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     4034 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml
+-rw-r--r--   0        0        0      609 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     3307 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      194 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/csi-cinder-driver.yaml
+-rw-r--r--   0        0        0     3377 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     3944 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml
+-rw-r--r--   0        0        0     1513 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     2988 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      143 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csidriver.yaml
+-rw-r--r--   0        0        0     3127 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml
+-rw-r--r--   0        0        0      170 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-driverinfo.yaml
+-rw-r--r--   0        0        0     3530 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml
+-rw-r--r--   0        0        0     1423 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml
+-rw-r--r--   0        0        0     1526 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/monitor.py
+-rw-r--r--   0        0        0     5673 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/objects.py
+-rw-r--r--   0        0        0      828 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/privsep/__init__.py
+-rw-r--r--   0        0        0     1333 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/privsep/haproxy.py
+-rw-r--r--   0        0        0    11719 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/manager.py
+-rw-r--r--   0        0        0     3616 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/structs.py
+-rw-r--r--   0        0        0      580 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
+-rw-r--r--   0        0        0     1511 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/utils.py
+-rw-r--r--   0        0        0    84493 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/resources.py
+-rw-r--r--   0        0        0     1492 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/service.py
+-rw-r--r--   0        0        0     3124 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/functional/conftest.py
+-rw-r--r--   0        0        0      666 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/functional/test_clusters.py
+-rw-r--r--   0        0        0      942 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/conftest.py
+-rw-r--r--   0        0        0     3813 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_helm.py
+-rw-r--r--   0        0        0     1731 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_image_utils.py
+-rw-r--r--   0        0        0     3105 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_images.py
+-rw-r--r--   0        0        0     5366 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_objects.py
+-rw-r--r--   0        0        0     1735 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_resources.py
+-rw-r--r--   0        0        0     1192 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     8746 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/magnum_cluster_api/utils.py
+-rw-r--r--   0        0        0     1288 2023-07-05 04:18:34.675672 magnum_cluster_api-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     4448 1970-01-01 00:00:00.000000 magnum_cluster_api-0.8.0/PKG-INFO
```

### Comparing `magnum_cluster_api-0.7.2/LICENSE` & `magnum_cluster_api-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/README.md` & `magnum_cluster_api-0.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 ![Cluster API driver for Magnum](docs/static/logo.png?raw=true "Cluster API driver for Magnum")
 
+The Cluster API driver for Magnum allows you to deploy fully conformant
+Kubernetes cluster using the [Cluster API](https://cluster-api.sigs.k8s.io/)
+project which are fully integrated with the OpenStack cluster they are running
+on.
+
 ## Images
 
 The images are built and published to an object storage bucket hosted at the
 [VEXXHOST](https://vexxhost.com) public cloud.  These images are built and
 published for the latest stable release of Kubernetes.
 
 ### Pre-built images
 
 You can find the pre-built images for the latest stable release of Kubernetes
 at the following URL:
 
-* [v1.23.13](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2004-v1.23.13.qcow2)
-* [v1.24.7](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2004-v1.24.7.qcow2)
-* [v1.25.3](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2004-v1.25.3.qcow2)
+* [v1.23.17](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-v1.23.17.qcow2)
+* [v1.24.15](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-v1.24.15.qcow2)
+* [v1.25.11](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-v1.25.11.qcow2)
+* [v1.26.6](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-v1.26.6.qcow2)
+* [v1.27.3](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-v1.27.3.qcow2)
 
 ### Building images
 
 The Cluster API driver for Magnum provides a tool in order to build images, you
 can use it by installing the `magnum-cluster-api` package and running the
 the following command:
 
@@ -39,18 +46,18 @@
 
 1. Upload an image to use with Magnum and create cluster templates
 
    ```bash
    pushd /tmp
    source /opt/stack/openrc
    for version in v1.23.13 v1.24.7 v1.25.3; do \
-      curl -LO https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2004-${version}.qcow2; \
-      openstack image create ubuntu-2004-${version} --disk-format=qcow2 --container-format=bare --property os_distro=ubuntu-focal --file=ubuntu-2004-${version}.qcow2; \
+      curl -LO https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-${version}.qcow2; \
+      openstack image create ubuntu-2204-kube-${version} --disk-format=qcow2 --container-format=bare --property os_distro=ubuntu --file=ubuntu-2204-kube-${version}.qcow2; \
       openstack coe cluster template create \
-         --image $(openstack image show ubuntu-2004-${version} -c id -f value) \
+         --image $(openstack image show ubuntu-2204-kube-${version} -c id -f value) \
          --external-network public \
          --dns-nameserver 8.8.8.8 \
          --master-lb-enabled \
          --master-flavor m1.medium \
          --flavor m1.medium \
          --network-driver calico \
          --docker-storage-driver overlay2 \
```

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/README.md` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/charts/cluster-autoscaler/values.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/clients.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/clients.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/cmd/image_builder.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/cmd/image_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,32 +32,39 @@
     "virtinst",
     "cpu-checker",
     "libguestfs-tools",
     "libosinfo-bin",
 ]
 
 
+def validate_version(_, __, value):
+    if not value.startswith("v"):
+        raise click.BadParameter("Version should start with 'v'")
+    return value
+
+
 @click.command()
 @click.option(
     "--operating-system",
     show_default=True,
-    default="ubuntu-2004",
+    default="ubuntu-2204",
     type=click.Choice(["ubuntu-2004", "ubuntu-2204"]),
     help="Operating system to build image for",
 )
 @click.option(
     "--version",
     show_default=True,
-    default="v1.26.2",
+    default="v1.27.3",
+    callback=validate_version,
     help="Kubernetes version",
 )
 @click.option(
     "--image-builder-version",
     show_default=True,
-    default="v0.1.14",
+    default="d37da2a",
     help="Image builder tag (or commit) to use for building image",
 )
 def main(operating_system, version, image_builder_version):
     ib_path = f"/tmp/image-builder-{image_builder_version}"
     output = f"{operating_system}-kube-{version}"
 
     target = f"{ib_path}/images/capi/output/{output}/{output}"
@@ -107,14 +114,37 @@
     click.echo("- Create customization file")
     kubernetes_series = ".".join(version.split(".")[0:2])
     customization = {
         "kubernetes_deb_version": f"{version.replace('v', '')}-00",
         "kubernetes_semver": f"{version}",
         "kubernetes_series": f"{kubernetes_series}",
     }
+
+    # NOTE(mnaser): We use the latest tested daily ISO for Ubuntu 22.04 in order
+    #               to avoid a lengthy upgrade process.
+    if operating_system == "ubuntu-2204":
+        iso = "jammy-live-server-amd64.iso"
+
+        customization[
+            "iso_url"
+        ] = f"http://cdimage.ubuntu.com/ubuntu-server/jammy/daily-live/current/{iso}"
+
+        # Get the SHA256 sum for the ISO
+        r = requests.get(
+            "http://cdimage.ubuntu.com/ubuntu-server/jammy/daily-live/current/SHA256SUMS"
+        )
+        r.raise_for_status()
+        for line in r.text.splitlines():
+            if iso in line:
+                customization["iso_checksum"] = line.split()[0]
+                break
+
+        # Assert that we have the checksum
+        assert "iso_checksum" in customization
+
     with tempfile.NamedTemporaryFile(suffix=".json") as fp:
         fp.write(json.dumps(customization).encode("utf-8"))
         fp.flush()
 
         click.echo("- Build image")
         subprocess.run(
             [
```

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/cmd/image_loader.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/cmd/image_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     "registry.k8s.io/coredns/coredns:v1.8.6",
     "registry.k8s.io/coredns/coredns:v1.9.3",
     CONF.auto_scaling.v1_22_image,
     CONF.auto_scaling.v1_23_image,
     CONF.auto_scaling.v1_24_image,
     CONF.auto_scaling.v1_25_image,
     CONF.auto_scaling.v1_26_image,
+    CONF.auto_scaling.v1_27_image,
     "registry.k8s.io/etcd:3.5.1-0",
     "registry.k8s.io/etcd:3.5.3-0",
     "registry.k8s.io/etcd:3.5.3-0",
     "registry.k8s.io/etcd:3.5.4-0",
     "registry.k8s.io/etcd:3.5.6-0",
     "registry.k8s.io/kube-apiserver:v1.23.13",
     "registry.k8s.io/kube-apiserver:v1.24.7",
@@ -78,16 +79,15 @@
     "registry.k8s.io/sig-storage/livenessprobe:v2.8.0",
 ]
 
 
 @click.command()
 @click.option(
     "--repository",
-    show_default=True,
-    default="quay.io/vexxhost",
+    required=True,
     help="Target image repository",
 )
 @click.option(
     "--insecure",
     is_flag=True,
     help="Allow insecure connections to the registry.",
 )
```

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/cmd/proxy.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/cmd/proxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/conf.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,37 +26,42 @@
     cfg.StrOpt(
         "image_repository",
         default="registry.k8s.io/autoscaling",
         help="Image repository for the cluster auto-scaler.",
     ),
     cfg.StrOpt(
         "v1_22_image",
-        default="$image_repository/cluster-autoscaler:v1.22.1",
+        default="$image_repository/cluster-autoscaler:v1.22.3",
         help="Image for the cluster auto-scaler for Kubernetes v1.22.",
     ),
     cfg.StrOpt(
         "v1_23_image",
-        default="$image_repository/cluster-autoscaler:v1.23.0",
+        default="$image_repository/cluster-autoscaler:v1.23.1",
         help="Image for the cluster auto-scaler for Kubernetes v1.23.",
     ),
     cfg.StrOpt(
         "v1_24_image",
-        default="$image_repository/cluster-autoscaler:v1.24.1",
+        default="$image_repository/cluster-autoscaler:v1.24.2",
         help="Image for the cluster auto-scaler for Kubernetes v1.24.",
     ),
     cfg.StrOpt(
         "v1_25_image",
-        default="$image_repository/cluster-autoscaler:v1.25.1",
+        default="$image_repository/cluster-autoscaler:v1.25.2",
         help="Image for the cluster auto-scaler for Kubernetes v1.25.",
     ),
     cfg.StrOpt(
         "v1_26_image",
-        default="$image_repository/cluster-autoscaler:v1.26.1",
+        default="$image_repository/cluster-autoscaler:v1.26.3",
         help="Image for the cluster auto-scaler for Kubernetes v1.26.",
     ),
+    cfg.StrOpt(
+        "v1_27_image",
+        default="$image_repository/cluster-autoscaler:v1.27.2",
+        help="Image for the cluster auto-scaler for Kubernetes v1.27.",
+    ),
 ]
 
 
 manila_client_opts = [
     cfg.StrOpt(
         "region_name",
         help=_(
```

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/driver.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,20 +309,14 @@
             if phase in ("ScalingUp", "ScalingDown"):
                 nodegroup.status = f"{action}_IN_PROGRESS"
             elif phase == "Running":
                 nodegroup.status = f"{action}_COMPLETE"
             elif phase in ("Failed", "Unknown"):
                 nodegroup.status = f"{action}_FAILED"
 
-            # TODO(mnaser): We can remove this once we support Cluster API 1.4.0
-            #               https://github.com/kubernetes-sigs/cluster-api/pull/7917
-            resources.set_autoscaler_metadata_in_machinedeployment(
-                context, self.k8s_api, cluster, nodegroup
-            )
-
         nodegroup.save()
 
         return nodegroup
 
     def update_nodegroup(self, context, cluster, nodegroup):
         # TODO
 
@@ -359,13 +353,21 @@
     def update_federation(self, context, federation):
         raise NotImplementedError()
 
     def delete_federation(self, context, federation):
         raise NotImplementedError()
 
 
-class UbuntuFocalDriver(BaseDriver):
+class UbuntuDriver(BaseDriver):
+    @property
+    def provides(self):
+        return [
+            {"server_type": "vm", "os": "ubuntu", "coe": "kubernetes"},
+        ]
+
+
+class UbuntuFocalDriver(UbuntuDriver):
     @property
     def provides(self):
         return [
             {"server_type": "vm", "os": "ubuntu-focal", "coe": "kubernetes"},
         ]
```

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/exceptions.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/helm.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/image_utils.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/image_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 def get_image(name: str, repository: str = None):
     """
     Get the image name from the target registry given a full image name.
     """
 
-    if repository is None:
+    if not repository:
         return name
 
     new_image_name = name
     if name.startswith("docker.io/calico"):
         new_image_name = name.replace("docker.io/calico/", f"{repository}/calico-")
     if name.startswith("docker.io/k8scloudprovider"):
         new_image_name = name.replace("docker.io/k8scloudprovider", repository)
```

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/images.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/audit/policy.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/audit/policy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/calico/v3.24.2.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/cinder-csi/cinder-csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/manila-csi/csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-controller.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/csi-nfs-node.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml` & `magnum_cluster_api-0.8.0/magnum_cluster_api/manifests/nfs-csi/rbac-csi-nfs.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/monitor.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/monitor.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/objects.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/objects.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/privsep/__init__.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/privsep/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/privsep/haproxy.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/privsep/haproxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/proxy/manager.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/manager.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/proxy/structs.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/structs.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/proxy/templates/haproxy.cfg.j2` & `magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/proxy/utils.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/proxy/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/resources.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,75 +19,79 @@
 import types
 
 import certifi
 import pkg_resources
 import pykube
 import yaml
 from magnum import objects as magnum_objects
-from magnum.common import cert_manager, cinder, context, neutron
+from magnum.common import cert_manager, context, neutron
 from magnum.common import utils as magnum_utils
 from magnum.common.x509 import operations as x509
 from oslo_config import cfg
 from oslo_serialization import base64
 from oslo_utils import encodeutils
 
 from magnum_cluster_api import clients, helm, image_utils, images, objects, utils
+from magnum_cluster_api.integrations import cinder, cloud_provider, manila
 
 CONF = cfg.CONF
-CLOUD_PROVIDER_TAG = "v1.25.3"
 CALICO_TAG = "v3.24.2"
-CINDER_CSI_TAG = "v1.25.3"
-MANILA_CSI_TAG = "v1.25.3"
 
 CLUSTER_CLASS_VERSION = pkg_resources.require("magnum_cluster_api")[0].version
 CLUSTER_CLASS_NAME = f"magnum-v{CLUSTER_CLASS_VERSION}"
 
 CLUSTER_UPGRADE_LABELS = {"kube_tag"}
 
 PLACEHOLDER = "PLACEHOLDER"
 
 AUTOSCALE_ANNOTATION_MIN = "cluster.x-k8s.io/cluster-api-autoscaler-node-group-min-size"
 AUTOSCALE_ANNOTATION_MAX = "cluster.x-k8s.io/cluster-api-autoscaler-node-group-max-size"
 
 
 class ClusterAutoscalerHelmRelease:
     def __init__(self, api, cluster) -> None:
+        self.cluster = cluster
+
+    @property
+    def apply(self):
         image = images.get_cluster_autoscaler_image(
-            utils.get_kube_tag(cluster),
+            utils.get_kube_tag(self.cluster),
         )
         image_repo, image_tag = image.split(":", 1)
 
-        self.apply = helm.UpgradeReleaseCommand(
+        return helm.UpgradeReleaseCommand(
             namespace="magnum-system",
-            release_name=cluster.stack_id,
+            release_name=self.cluster.stack_id,
             chart_ref=os.path.join(
                 pkg_resources.resource_filename("magnum_cluster_api", "charts"),
                 "cluster-autoscaler/",
             ),
             values={
-                "fullnameOverride": f"{cluster.stack_id}-autoscaler",
+                "fullnameOverride": f"{self.cluster.stack_id}-autoscaler",
                 "cloudProvider": "clusterapi",
                 "clusterAPIMode": "kubeconfig-incluster",
-                "clusterAPIKubeconfigSecret": f"{cluster.stack_id}-kubeconfig",
+                "clusterAPIKubeconfigSecret": f"{self.cluster.stack_id}-kubeconfig",
                 "autoDiscovery": {
-                    "clusterName": cluster.stack_id,
+                    "clusterName": self.cluster.stack_id,
                 },
                 "image": {
                     "repository": image_repo,
                     "tag": image_tag,
                 },
                 "nodeSelector": {
                     "openstack-control-plane": "enabled",
                 },
             },
         )
 
-        self.delete = helm.DeleteReleaseCommand(
+    @property
+    def delete(self):
+        return helm.DeleteReleaseCommand(
             namespace="magnum-system",
-            release_name=cluster.stack_id,
+            release_name=self.cluster.stack_id,
             skip_missing=True,
         )
 
 
 class Base:
     def __init__(self, api: pykube.HTTPClient):
         self.api = api
@@ -156,63 +160,57 @@
         # NOTE(mnaser): We have to assert that the only CNI we support is Calico.
         assert CONF.cluster_template.kubernetes_allowed_network_drivers == ["calico"]
 
         manifests_path = pkg_resources.resource_filename(
             "magnum_cluster_api", "manifests"
         )
         calico_version = utils.get_cluster_label(self.cluster, "calico_tag", CALICO_TAG)
-        ccm_version = utils.get_cluster_label(
-            self.cluster, "cloud_provider_tag", CLOUD_PROVIDER_TAG
-        )
 
         repository = utils.get_cluster_container_infra_prefix(self.cluster)
 
         osc = clients.get_openstack_api(self.context)
 
         data = {
             **{
                 os.path.basename(manifest): image_utils.update_manifest_images(
                     self.cluster.uuid,
                     manifest,
                     repository=repository,
                     replacements=[
                         (
                             "docker.io/k8scloudprovider/openstack-cloud-controller-manager:latest",
-                            f"docker.io/k8scloudprovider/openstack-cloud-controller-manager:{ccm_version}",
+                            cloud_provider.get_image(self.cluster),
                         ),
                     ],
                 )
                 for manifest in glob.glob(os.path.join(manifests_path, "ccm/*.yaml"))
             },
             **{
                 "calico.yml": image_utils.update_manifest_images(
                     self.cluster.uuid,
                     os.path.join(manifests_path, f"calico/{calico_version}.yaml"),
                     repository=repository,
                 )
             },
         }
 
-        if utils.is_cinder_csi_enabled(self.cluster):
+        if cinder.is_enabled(self.cluster):
             volume_types = osc.cinder().volume_types.list()
             default_volume_type = osc.cinder().volume_types.default()
-            csi_version = utils.get_cluster_label(
-                self.cluster, "cinder_csi_plugin_tag", CINDER_CSI_TAG
-            )
             data = {
                 **data,
                 **{
                     os.path.basename(manifest): image_utils.update_manifest_images(
                         self.cluster.uuid,
                         manifest,
                         repository=repository,
                         replacements=[
                             (
                                 "docker.io/k8scloudprovider/cinder-csi-plugin:latest",
-                                f"docker.io/k8scloudprovider/cinder-csi-plugin:{csi_version}",
+                                cinder.get_image(self.cluster),
                             ),
                         ],
                     )
                     for manifest in glob.glob(
                         os.path.join(manifests_path, "cinder-csi/*.yaml")
                     )
                 },
@@ -239,19 +237,16 @@
                         }
                     )
                     for vt in volume_types
                     if vt.name != "__DEFAULT__"
                 },
             }
 
-        if utils.is_manila_csi_enabled(self.cluster):
+        if manila.is_enabled(self.cluster):
             share_types = osc.manila().share_types.list()
-            csi_version = utils.get_cluster_label(
-                self.cluster, "manila_csi_plugin_tag", MANILA_CSI_TAG
-            )
             share_network_id = utils.get_cluster_label(
                 self.cluster, "manila_csi_share_network_id", None
             )
             data = {
                 **data,
                 **{
                     "manila-csi-secret.yaml": yaml.dump(
@@ -283,15 +278,15 @@
                     os.path.basename(manifest): image_utils.update_manifest_images(
                         self.cluster.uuid,
                         manifest,
                         repository=repository,
                         replacements=[
                             (
                                 "registry.k8s.io/provider-os/manila-csi-plugin:latest",
-                                f"registry.k8s.io/provider-os/manila-csi-plugin:{csi_version}",
+                                manila.get_image(self.cluster),
                             ),
                         ],
                     )
                     for manifest in glob.glob(
                         os.path.join(manifests_path, "manila-csi/*.yaml")
                     )
                 },
@@ -465,16 +460,16 @@
 
         return pykube.Secret(
             self.api,
             {
                 "apiVersion": pykube.Secret.version,
                 "kind": pykube.Secret.kind,
                 "metadata": {
-                    "name": utils.get_or_generate_cluster_api_cloud_config_secret_name(
-                        self.api, self.cluster
+                    "name": utils.get_cluster_api_cloud_config_secret_name(
+                        self.cluster
                     ),
                     "namespace": "magnum-system",
                     "labels": self.labels,
                 },
                 "stringData": {
                     "cacert": ca_certificate
                     if ca_certificate
@@ -1310,14 +1305,62 @@
                                             "valueFrom": {"variable": "fixedSubnetId"},
                                         },
                                     ],
                                 },
                             ],
                         },
                         {
+                            "name": "customImageRepository",
+                            "enabledIf": '{{ if ne .imageRepository "" }}true{{end}}',
+                            "definitions": [
+                                {
+                                    "selector": {
+                                        "apiVersion": objects.KubeadmControlPlaneTemplate.version,
+                                        "kind": objects.KubeadmControlPlaneTemplate.kind,
+                                        "matchResources": {
+                                            "controlPlane": True,
+                                        },
+                                    },
+                                    "jsonPatches": [
+                                        {
+                                            "op": "add",
+                                            "path": "/spec/template/spec/kubeadmConfigSpec/clusterConfiguration/imageRepository",  # noqa: E501
+                                            "valueFrom": {
+                                                "variable": "imageRepository",
+                                            },
+                                        },
+                                    ],
+                                },
+                                {
+                                    "selector": {
+                                        "apiVersion": objects.KubeadmConfigTemplate.version,
+                                        "kind": objects.KubeadmConfigTemplate.kind,
+                                        "matchResources": {
+                                            "machineDeploymentClass": {
+                                                "names": ["default-worker"],
+                                            }
+                                        },
+                                    },
+                                    "jsonPatches": [
+                                        {
+                                            "op": "add",
+                                            "path": "/spec/template/spec/clusterConfiguration",
+                                            "valueFrom": {
+                                                "template": textwrap.dedent(
+                                                    """\
+                                                    imageRepository: "{{ .imageRepository }}"
+                                                    """
+                                                ),
+                                            },
+                                        },
+                                    ],
+                                },
+                            ],
+                        },
+                        {
                             "name": "controlPlaneConfig",
                             "definitions": [
                                 {
                                     "selector": {
                                         "apiVersion": objects.KubeadmControlPlaneTemplate.version,
                                         "kind": objects.KubeadmControlPlaneTemplate.kind,
                                         "matchResources": {
@@ -1338,21 +1381,14 @@
                                                     encoding: "base64"
                                                     """
                                                 )
                                             },
                                         },
                                         {
                                             "op": "add",
-                                            "path": "/spec/template/spec/kubeadmConfigSpec/clusterConfiguration/imageRepository",  # noqa: E501
-                                            "valueFrom": {
-                                                "variable": "imageRepository",
-                                            },
-                                        },
-                                        {
-                                            "op": "add",
                                             "path": "/spec/template/spec/kubeadmConfigSpec/clusterConfiguration/apiServer/certSANs",  # noqa: E501
                                             "valueFrom": {
                                                 "template": textwrap.dedent(
                                                     """\
                                                     - {{ .builtin.cluster.name }}
                                                     - {{ .builtin.cluster.name }}.{{ .builtin.cluster.namespace }}
                                                     - {{ .builtin.cluster.name }}.{{ .builtin.cluster.namespace }}.svc
@@ -1387,25 +1423,14 @@
                                                 "names": ["default-worker"],
                                             }
                                         },
                                     },
                                     "jsonPatches": [
                                         {
                                             "op": "add",
-                                            "path": "/spec/template/spec/clusterConfiguration",
-                                            "valueFrom": {
-                                                "template": textwrap.dedent(
-                                                    """\
-                                                    imageRepository: "{{ .imageRepository }}"
-                                                    """
-                                                ),
-                                            },
-                                        },
-                                        {
-                                            "op": "add",
                                             "path": "/spec/template/spec/files",
                                             "valueFrom": {
                                                 "template": textwrap.dedent(
                                                     """\
                                                     - path: "/etc/kubernetes/cloud.conf"
                                                       owner: "root:root"
                                                       permissions: "0600"
@@ -1493,15 +1518,15 @@
                     },
                     {
                         "name": "imageRepository",
                         "value": utils.get_node_group_label(
                             context,
                             ng,
                             "container_infra_prefix",
-                            "quay.io/vexxhost",
+                            "",
                         ),
                     },
                     {
                         "name": "imageUUID",
                         "value": ng.image_id,
                     },
                 ],
@@ -1521,36 +1546,19 @@
     ):
         self.context = context
         self.api = api
         self.cluster = cluster
 
     @property
     def labels(self) -> dict:
-        ccm_version = utils.get_cluster_label(
-            self.cluster, "cloud_provider_tag", CLOUD_PROVIDER_TAG
-        )
         cni_version = utils.get_cluster_label(self.cluster, "calico_tag", CALICO_TAG)
         labels = {
             "cni": f"calico-{cni_version}",
-            "ccm": f"openstack-cloud-controller-manager-{ccm_version}",
         }
 
-        if utils.is_cinder_csi_enabled(self.cluster):
-            csi_version = utils.get_cluster_label(
-                self.cluster, "cinder_csi_plugin_tag", CINDER_CSI_TAG
-            )
-            labels["csi"] = "cinder"
-            labels["cinder-csi-version"] = csi_version
-
-        if utils.is_manila_csi_enabled(self.cluster):
-            manila_version = utils.get_cluster_label(
-                self.cluster, "manila_csi_plugin_tag", MANILA_CSI_TAG
-            )
-            labels["manila-csi-version"] = manila_version
-
         return {**super().labels, **labels}
 
     def get_or_none(self) -> objects.Cluster:
         return objects.Cluster.objects(self.api, namespace="magnum-system").get_or_none(
             name=self.cluster.stack_id
         )
 
@@ -1677,16 +1685,16 @@
                                     ),
                                 },
                             },
                             {
                                 "name": "clusterIdentityRef",
                                 "value": {
                                     "kind": pykube.Secret.kind,
-                                    "name": utils.get_or_generate_cluster_api_cloud_config_secret_name(
-                                        self.api, self.cluster
+                                    "name": utils.get_cluster_api_cloud_config_secret_name(
+                                        self.cluster
                                     ),
                                 },
                             },
                             {
                                 "name": "cloudControllerManagerConfig",
                                 "value": base64.encode_as_text(
                                     utils.generate_cloud_controller_manager_config(
@@ -1771,43 +1779,14 @@
 
     def delete(self):
         capi_cluster = self.get_or_none()
         if capi_cluster:
             capi_cluster.delete()
 
 
-def set_autoscaler_metadata_in_machinedeployment(
-    context: context.RequestContext,
-    api: pykube.HTTPClient,
-    cluster: magnum_objects.Cluster,
-    nodegroup: magnum_objects.NodeGroup,
-):
-    if not utils.get_auto_scaling_enabled(cluster):
-        return
-    mds = objects.MachineDeployment.objects(api).filter(
-        namespace="magnum-system",
-        selector={
-            "cluster.x-k8s.io/cluster-name": cluster.stack_id,
-            "topology.cluster.x-k8s.io/deployment-name": nodegroup.name,
-        },
-    )
-    for md in mds:
-        # NOTE(mnaser): The autoscaler will not scale under the minimum number
-        #               of nodes, so we do that ourselves here.
-        if AUTOSCALE_ANNOTATION_MIN not in md.obj["metadata"]["annotations"]:
-            md.obj["spec"]["replicas"] = nodegroup.node_count
-        md.obj["metadata"]["annotations"][AUTOSCALE_ANNOTATION_MIN] = str(
-            utils.get_node_group_min_node_count(nodegroup)
-        )
-        md.obj["metadata"]["annotations"][AUTOSCALE_ANNOTATION_MAX] = str(
-            utils.get_node_group_max_node_count(context, nodegroup)
-        )
-        md.update()
-
-
 def apply_cluster_from_magnum_cluster(
     context: context.RequestContext,
     api: pykube.HTTPClient,
     cluster: magnum_objects.Cluster,
     cluster_template: magnum_objects.ClusterTemplate = None,
 ) -> objects.Cluster:
     """
```

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/service.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/service.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/tests/functional/conftest.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/functional/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 @pytest.fixture(scope="session")
 def conn():
     return openstack.connect(cloud="envvars")
 
 
 @pytest.fixture(scope="session")
 def image(conn, kube_tag):
-    image_name = os.getenv("CAPI_IMAGE_NAME", f"ubuntu-2004-{kube_tag}")
+    image_name = os.getenv("CAPI_IMAGE_NAME", f"ubuntu-2204-kube-{kube_tag}")
     return conn.image.find_image(image_name)
 
 
 @pytest.fixture(scope="session")
 def cluster_template(conn, image, kube_tag):
     cluster_template = conn.container_infra.create_cluster_template(
         name="k8s-%s" % shortuuid.uuid(),
```

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/tests/functional/test_clusters.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/functional/test_clusters.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/conftest.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/test_helm.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/test_image_utils.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/test_images.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_images.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,34 +17,38 @@
 
 from magnum_cluster_api import images
 
 
 @pytest.mark.parametrize(
     "version,image,image_repository",
     [
-        ("v1.22.0", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.22.1", None),
-        ("v1.22.17", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.22.1", None),
-        ("v1.23.0", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.23.0", None),
-        ("v1.23.17", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.23.0", None),
-        ("v1.24.0", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.24.1", None),
-        ("v1.24.17", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.24.1", None),
-        ("v1.25.0", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.25.1", None),
-        ("v1.25.17", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.25.1", None),
-        ("v1.26.0", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.26.1", None),
-        ("v1.26.3", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.26.1", None),
-        ("v1.22.0", "quay.io/vexxhost/cluster-autoscaler:v1.22.1", "quay.io/vexxhost"),
-        ("v1.22.17", "quay.io/vexxhost/cluster-autoscaler:v1.22.1", "quay.io/vexxhost"),
-        ("v1.23.0", "quay.io/vexxhost/cluster-autoscaler:v1.23.0", "quay.io/vexxhost"),
-        ("v1.23.17", "quay.io/vexxhost/cluster-autoscaler:v1.23.0", "quay.io/vexxhost"),
-        ("v1.24.0", "quay.io/vexxhost/cluster-autoscaler:v1.24.1", "quay.io/vexxhost"),
-        ("v1.24.17", "quay.io/vexxhost/cluster-autoscaler:v1.24.1", "quay.io/vexxhost"),
-        ("v1.25.0", "quay.io/vexxhost/cluster-autoscaler:v1.25.1", "quay.io/vexxhost"),
-        ("v1.25.17", "quay.io/vexxhost/cluster-autoscaler:v1.25.1", "quay.io/vexxhost"),
-        ("v1.26.3", "quay.io/vexxhost/cluster-autoscaler:v1.26.1", "quay.io/vexxhost"),
-        ("v1.26.3", "quay.io/vexxhost/cluster-autoscaler:v1.26.1", "quay.io/vexxhost"),
+        ("v1.22.0", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.22.3", None),
+        ("v1.22.17", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.22.3", None),
+        ("v1.23.0", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.23.1", None),
+        ("v1.23.17", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.23.1", None),
+        ("v1.24.0", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.24.2", None),
+        ("v1.24.17", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.24.2", None),
+        ("v1.25.0", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.25.2", None),
+        ("v1.25.17", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.25.2", None),
+        ("v1.26.0", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.26.3", None),
+        ("v1.26.3", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.26.3", None),
+        ("v1.27.0", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.27.2", None),
+        ("v1.27.3", "registry.k8s.io/autoscaling/cluster-autoscaler:v1.27.2", None),
+        ("v1.22.0", "quay.io/vexxhost/cluster-autoscaler:v1.22.3", "quay.io/vexxhost"),
+        ("v1.22.17", "quay.io/vexxhost/cluster-autoscaler:v1.22.3", "quay.io/vexxhost"),
+        ("v1.23.0", "quay.io/vexxhost/cluster-autoscaler:v1.23.1", "quay.io/vexxhost"),
+        ("v1.23.17", "quay.io/vexxhost/cluster-autoscaler:v1.23.1", "quay.io/vexxhost"),
+        ("v1.24.0", "quay.io/vexxhost/cluster-autoscaler:v1.24.2", "quay.io/vexxhost"),
+        ("v1.24.17", "quay.io/vexxhost/cluster-autoscaler:v1.24.2", "quay.io/vexxhost"),
+        ("v1.25.0", "quay.io/vexxhost/cluster-autoscaler:v1.25.2", "quay.io/vexxhost"),
+        ("v1.25.17", "quay.io/vexxhost/cluster-autoscaler:v1.25.2", "quay.io/vexxhost"),
+        ("v1.26.0", "quay.io/vexxhost/cluster-autoscaler:v1.26.3", "quay.io/vexxhost"),
+        ("v1.26.3", "quay.io/vexxhost/cluster-autoscaler:v1.26.3", "quay.io/vexxhost"),
+        ("v1.27.0", "quay.io/vexxhost/cluster-autoscaler:v1.27.2", "quay.io/vexxhost"),
+        ("v1.27.3", "quay.io/vexxhost/cluster-autoscaler:v1.27.2", "quay.io/vexxhost"),
     ],
 )
 def test_get_cluster_autoscaler_image(image_repository, version, image):
     if image_repository:
         cfg.CONF.set_override(
             "image_repository", image_repository, group="auto_scaling"
         )
```

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/test_objects.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_objects.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/test_resources.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         mocker.Mock(name="deleted-worker", status="DELETE_COMPLETE", labels={}),
     ]
 
     cluster_get_by_uuid = mocker.patch("magnum.objects.Cluster.get_by_uuid")
     cluster_get_by_uuid.return_value = cluster
 
     mock_get_default_boot_volume_type = mocker.patch(
-        "magnum.common.cinder.get_default_boot_volume_type"
+        "magnum_cluster_api.integrations.cinder.get_default_boot_volume_type"
     )
     mock_get_default_boot_volume_type.return_value = "foo"
 
     mds = resources.generate_machine_deployments_for_cluster(
         context,
         cluster,
     )
```

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/tests/unit/test_utils.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.7.2/magnum_cluster_api/utils.py` & `magnum_cluster_api-0.8.0/magnum_cluster_api/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,30 +17,24 @@
 import textwrap
 
 import pykube
 import shortuuid
 import yaml
 from magnum import objects as magnum_objects
 from magnum.common import context, exception, octavia
-from magnum.common.keystone import KeystoneClientV3
-from oslo_log import log as logging
 from oslo_serialization import base64
 from oslo_utils import strutils
 from tenacity import retry, retry_if_exception_type
 
 from magnum_cluster_api import clients
 from magnum_cluster_api import exceptions as mcapi_exceptions
 from magnum_cluster_api import image_utils, images, objects
 
-LOG = logging.getLogger(__name__)
 
-
-def get_or_generate_cluster_api_cloud_config_secret_name(
-    api: pykube.HTTPClient, cluster: magnum_objects.Cluster
-) -> str:
+def get_cluster_api_cloud_config_secret_name(cluster: magnum_objects.Cluster) -> str:
     return f"{cluster.stack_id}-cloud-config"
 
 
 @retry(retry=retry_if_exception_type(exception.Conflict))
 def generate_cluster_api_name(
     api: pykube.HTTPClient,
 ) -> str:
@@ -66,15 +60,15 @@
     cluster: magnum_objects.Cluster,
 ) -> str:
     """
     Generate coniguration for openstack-cloud-controller-manager if it does
     already exist.
     """
     data = pykube.Secret.objects(api, namespace="magnum-system").get_by_name(
-        get_or_generate_cluster_api_cloud_config_secret_name(api, cluster)
+        get_cluster_api_cloud_config_secret_name(cluster)
     )
     clouds_yaml = base64.decode_as_text(data.obj["data"]["clouds.yaml"])
     cloud_config = yaml.safe_load(clouds_yaml)
 
     return textwrap.dedent(
         f"""\
         [Global]
@@ -91,15 +85,15 @@
     api: pykube.HTTPClient,
     cluster: magnum_objects.Cluster,
 ) -> str:
     """
     Generate coniguration of Openstack authentication  for manila csi
     """
     data = pykube.Secret.objects(api, namespace="magnum-system").get_by_name(
-        get_or_generate_cluster_api_cloud_config_secret_name(api, cluster)
+        get_cluster_api_cloud_config_secret_name(cluster)
     )
     clouds_yaml = base64.decode_as_text(data.obj["data"]["clouds.yaml"])
     cloud_config = yaml.safe_load(clouds_yaml)
 
     return {
         "os-authURL": cloud_config["clouds"]["default"]["auth"]["auth_url"],
         "os-region": cloud_config["clouds"]["default"]["region_name"],
@@ -123,15 +117,15 @@
     return get_cluster_label_as_bool(cluster, "auto_scaling_enabled", False)
 
 
 def get_cluster_container_infra_prefix(cluster: magnum_objects.Cluster) -> str:
     return get_cluster_label(
         cluster,
         "container_infra_prefix",
-        "quay.io/vexxhost",
+        "",
     )
 
 
 def get_cluster_floating_ip_disabled(cluster: magnum_objects.Cluster) -> bool:
     return not get_cluster_label_as_bool(cluster, "master_lb_floating_ip_enabled", True)
 
 
@@ -256,67 +250,14 @@
             return
 
         octavia.wait_for_lb_deleted(octavia_client, candidates)
     except Exception as e:
         raise exception.PreDeletionFailed(cluster_uuid=cluster.uuid, msg=str(e))
 
 
-def is_cinder_enabled():
-    """Check if Cinder service is deployed in the cloud."""
-
-    admin_context = context.make_admin_context()
-    keystone = KeystoneClientV3(admin_context)
-
-    try:
-        cinder_svc = keystone.client.services.list(type="volumev3")
-    except Exception:
-        LOG.exception("Failed to list services")
-        raise exception.ServicesListFailed()
-
-    # Always assume there is only one load balancing service configured.
-    if cinder_svc and cinder_svc[0].enabled:
-        return True
-
-    LOG.info("There is no volumev3 service enabled in the cloud.")
-    return False
-
-
-def is_manila_enabled():
-    """Check if Manila service is deployed in the cloud."""
-
-    admin_context = context.make_admin_context()
-    keystone = KeystoneClientV3(admin_context)
-
-    try:
-        manila_svc = keystone.client.services.list(type="sharev2")
-    except Exception:
-        LOG.exception("Failed to list services")
-        raise exception.ServicesListFailed()
-
-    if manila_svc and manila_svc[0].enabled:
-        return True
-
-    LOG.info("There is no sharev2 service enabled in the cloud.")
-    return False
-
-
-def is_cinder_csi_enabled(cluster: magnum_objects.Cluster) -> bool:
-    return (
-        get_cluster_label_as_bool(cluster, "cinder_csi_enabled", True)
-        and is_cinder_enabled()
-    )
-
-
-def is_manila_csi_enabled(cluster: magnum_objects.Cluster) -> bool:
-    return (
-        get_cluster_label_as_bool(cluster, "manila_csi_enabled", True)
-        and is_manila_enabled()
-    )
-
-
 def format_event_message(event: pykube.Event):
     return "%s: %s" % (
         event.obj["reason"],
         event.obj["message"],
     )
```

### Comparing `magnum_cluster_api-0.7.2/pyproject.toml` & `magnum_cluster_api-0.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnum-cluster-api"
-version = "0.7.2"
+version = "0.8.0"
 description = "Cluster API driver for Magnum"
 authors = ["Mohammed Naser <mnaser@vexxhost.com>"]
 readme = "README.md"
 packages = [{include = "magnum_cluster_api"}]
 include = ["magnum_cluster_api/charts/**/*"]
 
 [tool.poetry.dependencies]
@@ -35,11 +35,12 @@
 
 [tool.poetry.scripts]
 magnum-cluster-api-image-builder = "magnum_cluster_api.cmd.image_builder:main"
 magnum-cluster-api-image-loader = "magnum_cluster_api.cmd.image_loader:main"
 magnum-cluster-api-proxy = "magnum_cluster_api.cmd.proxy:main"
 
 [tool.poetry.plugins."magnum.drivers"]
+"k8s_cluster_api_ubuntu" = "magnum_cluster_api.driver:UbuntuDriver"
 "k8s_cluster_api_ubuntu_focal" = "magnum_cluster_api.driver:UbuntuFocalDriver"
 
 [tool.isort]
 profile = "black"
```

### Comparing `magnum_cluster_api-0.7.2/PKG-INFO` & `magnum_cluster_api-0.8.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnum-cluster-api
-Version: 0.7.2
+Version: 0.8.0
 Summary: Cluster API driver for Magnum
 Author: Mohammed Naser
 Author-email: mnaser@vexxhost.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -27,28 +27,35 @@
 Requires-Dist: requests (>=2.27.1)
 Requires-Dist: semver (>=2.0.0,<3.0.0)
 Requires-Dist: shortuuid
 Description-Content-Type: text/markdown
 
 ![Cluster API driver for Magnum](docs/static/logo.png?raw=true "Cluster API driver for Magnum")
 
+The Cluster API driver for Magnum allows you to deploy fully conformant
+Kubernetes cluster using the [Cluster API](https://cluster-api.sigs.k8s.io/)
+project which are fully integrated with the OpenStack cluster they are running
+on.
+
 ## Images
 
 The images are built and published to an object storage bucket hosted at the
 [VEXXHOST](https://vexxhost.com) public cloud.  These images are built and
 published for the latest stable release of Kubernetes.
 
 ### Pre-built images
 
 You can find the pre-built images for the latest stable release of Kubernetes
 at the following URL:
 
-* [v1.23.13](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2004-v1.23.13.qcow2)
-* [v1.24.7](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2004-v1.24.7.qcow2)
-* [v1.25.3](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2004-v1.25.3.qcow2)
+* [v1.23.17](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-v1.23.17.qcow2)
+* [v1.24.15](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-v1.24.15.qcow2)
+* [v1.25.11](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-v1.25.11.qcow2)
+* [v1.26.6](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-v1.26.6.qcow2)
+* [v1.27.3](https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-v1.27.3.qcow2)
 
 ### Building images
 
 The Cluster API driver for Magnum provides a tool in order to build images, you
 can use it by installing the `magnum-cluster-api` package and running the
 the following command:
 
@@ -70,18 +77,18 @@
 
 1. Upload an image to use with Magnum and create cluster templates
 
    ```bash
    pushd /tmp
    source /opt/stack/openrc
    for version in v1.23.13 v1.24.7 v1.25.3; do \
-      curl -LO https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2004-${version}.qcow2; \
-      openstack image create ubuntu-2004-${version} --disk-format=qcow2 --container-format=bare --property os_distro=ubuntu-focal --file=ubuntu-2004-${version}.qcow2; \
+      curl -LO https://object-storage.public.mtl1.vexxhost.net/swift/v1/a91f106f55e64246babde7402c21b87a/magnum-capi/ubuntu-2204-kube-${version}.qcow2; \
+      openstack image create ubuntu-2204-kube-${version} --disk-format=qcow2 --container-format=bare --property os_distro=ubuntu --file=ubuntu-2204-kube-${version}.qcow2; \
       openstack coe cluster template create \
-         --image $(openstack image show ubuntu-2004-${version} -c id -f value) \
+         --image $(openstack image show ubuntu-2204-kube-${version} -c id -f value) \
          --external-network public \
          --dns-nameserver 8.8.8.8 \
          --master-lb-enabled \
          --master-flavor m1.medium \
          --flavor m1.medium \
          --network-driver calico \
          --docker-storage-driver overlay2 \
```

