# Comparing `tmp/magnum_cluster_api-0.5.0.tar.gz` & `tmp/magnum_cluster_api-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnum_cluster_api-0.5.0.tar", max compression
+gzip compressed data, was "magnum_cluster_api-0.5.1.tar", max compression
```

## Comparing `magnum_cluster_api-0.5.0.tar` & `magnum_cluster_api-0.5.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0    10142 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/LICENSE
--rw-r--r--   0        0        0     2795 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/.gitkeep
--rw-r--r--   0        0        0      349 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
--rw-r--r--   0        0        0      437 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
--rw-r--r--   0        0        0    29122 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/README.md
--rw-r--r--   0        0        0    14987 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
--rw-r--r--   0        0        0      827 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
--rw-r--r--   0        0        0     4034 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
--rw-r--r--   0        0        0     2982 2023-04-10 23:30:35.459469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
--rw-r--r--   0        0        0      534 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
--rw-r--r--   0        0        0    13204 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
--rw-r--r--   0        0        0      508 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
--rw-r--r--   0        0        0      972 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
--rw-r--r--   0        0        0      758 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
--rw-r--r--   0        0        0      564 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1807 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
--rw-r--r--   0        0        0      527 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
--rw-r--r--   0        0        0      989 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
--rw-r--r--   0        0        0     1180 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
--rw-r--r--   0        0        0      528 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      960 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
--rw-r--r--   0        0        0      663 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
--rw-r--r--   0        0        0    18003 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
--rw-r--r--   0        0        0      843 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/clients.py
--rw-r--r--   0        0        0        0 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/cmd/__init__.py
--rw-r--r--   0        0        0     4019 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/cmd/image_builder.py
--rw-r--r--   0        0        0     4167 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/cmd/image_loader.py
--rw-r--r--   0        0        0      956 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/cmd/proxy.py
--rw-r--r--   0        0        0     1778 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/conf.py
--rw-r--r--   0        0        0    10572 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/driver.py
--rw-r--r--   0        0        0     2155 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/helm.py
--rw-r--r--   0        0        0     3161 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/image_utils.py
--rw-r--r--   0        0        0     1116 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/images.py
--rw-r--r--   0        0        0        0 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/__init__.py
--rw-r--r--   0        0        0     4941 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/audit/policy.yaml
--rw-r--r--   0        0        0   235191 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml
--rw-r--r--   0        0        0      623 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
--rw-r--r--   0        0        0     1430 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
--rw-r--r--   0        0        0     2263 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
--rw-r--r--   0        0        0     4506 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     4009 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml
--rw-r--r--   0        0        0      609 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     3297 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml
--rw-r--r--   0        0        0      194 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/csi-cinder-driver.yaml
--rw-r--r--   0        0        0     1503 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/monitor.py
--rw-r--r--   0        0        0     2880 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/objects.py
--rw-r--r--   0        0        0      828 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/privsep/__init__.py
--rw-r--r--   0        0        0     1333 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/privsep/haproxy.py
--rw-r--r--   0        0        0    10475 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/proxy/manager.py
--rw-r--r--   0        0        0     3294 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/proxy/structs.py
--rw-r--r--   0        0        0      580 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
--rw-r--r--   0        0        0     1511 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/proxy/utils.py
--rw-r--r--   0        0        0    74957 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/resources.py
--rw-r--r--   0        0        0     1492 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/service.py
--rw-r--r--   0        0        0     3445 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/tests/test_helm.py
--rw-r--r--   0        0        0     1598 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/tests/test_image_utils.py
--rw-r--r--   0        0        0     2759 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/tests/test_images.py
--rw-r--r--   0        0        0     7554 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/utils.py
--rw-r--r--   0        0        0     1174 2023-04-10 23:30:22.158381 magnum_cluster_api-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 magnum_cluster_api-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2795 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/.gitkeep
+-rw-r--r--   0        0        0      349 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
+-rw-r--r--   0        0        0      437 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
+-rw-r--r--   0        0        0    29122 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/README.md
+-rw-r--r--   0        0        0    14987 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
+-rw-r--r--   0        0        0      827 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
+-rw-r--r--   0        0        0     4034 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2982 2023-04-11 18:44:25.504991 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
+-rw-r--r--   0        0        0      534 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
+-rw-r--r--   0        0        0    13204 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
+-rw-r--r--   0        0        0      508 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
+-rw-r--r--   0        0        0      972 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
+-rw-r--r--   0        0        0      758 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
+-rw-r--r--   0        0        0      564 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1807 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
+-rw-r--r--   0        0        0      527 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
+-rw-r--r--   0        0        0      989 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
+-rw-r--r--   0        0        0     1180 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
+-rw-r--r--   0        0        0      528 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      960 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0      663 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
+-rw-r--r--   0        0        0    18003 2023-04-11 18:44:25.500990 magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
+-rw-r--r--   0        0        0      843 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/clients.py
+-rw-r--r--   0        0        0        0 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/cmd/__init__.py
+-rw-r--r--   0        0        0     4019 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/cmd/image_builder.py
+-rw-r--r--   0        0        0     4167 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/cmd/image_loader.py
+-rw-r--r--   0        0        0      956 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/cmd/proxy.py
+-rw-r--r--   0        0        0     1778 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/conf.py
+-rw-r--r--   0        0        0    10862 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/driver.py
+-rw-r--r--   0        0        0     2155 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/helm.py
+-rw-r--r--   0        0        0     3161 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/image_utils.py
+-rw-r--r--   0        0        0     1116 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/images.py
+-rw-r--r--   0        0        0        0 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/__init__.py
+-rw-r--r--   0        0        0     4941 2023-04-11 18:44:22.692986 magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/audit/policy.yaml
+-rw-r--r--   0        0        0   235191 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/calico/v3.24.2.yaml
+-rw-r--r--   0        0        0      623 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
+-rw-r--r--   0        0        0     1430 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
+-rw-r--r--   0        0        0     2263 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
+-rw-r--r--   0        0        0     4506 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     4009 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml
+-rw-r--r--   0        0        0      609 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     3297 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      194 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/csi/csi-cinder-driver.yaml
+-rw-r--r--   0        0        0     1526 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/monitor.py
+-rw-r--r--   0        0        0     2880 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/objects.py
+-rw-r--r--   0        0        0      828 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/privsep/__init__.py
+-rw-r--r--   0        0        0     1333 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/privsep/haproxy.py
+-rw-r--r--   0        0        0    11719 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/proxy/manager.py
+-rw-r--r--   0        0        0     3616 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/proxy/structs.py
+-rw-r--r--   0        0        0      580 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
+-rw-r--r--   0        0        0     1511 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/proxy/utils.py
+-rw-r--r--   0        0        0    74957 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/resources.py
+-rw-r--r--   0        0        0     1492 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/service.py
+-rw-r--r--   0        0        0     3445 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/tests/test_helm.py
+-rw-r--r--   0        0        0     1598 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/tests/test_image_utils.py
+-rw-r--r--   0        0        0     2759 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/tests/test_images.py
+-rw-r--r--   0        0        0     7554 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/magnum_cluster_api/utils.py
+-rw-r--r--   0        0        0     1186 2023-04-11 18:44:22.696986 magnum_cluster_api-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 magnum_cluster_api-0.5.1/PKG-INFO
```

### Comparing `magnum_cluster_api-0.5.0/LICENSE` & `magnum_cluster_api-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/README.md` & `magnum_cluster_api-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/README.md` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/charts/cluster-autoscaler/values.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/clients.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/clients.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/cmd/image_builder.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/cmd/image_builder.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/cmd/image_loader.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/cmd/image_loader.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/cmd/proxy.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/cmd/proxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/conf.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/conf.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/driver.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,20 @@
 
         capi_cluster = resources.Cluster(context, self.k8s_api, cluster).get_or_none()
 
         if cluster.status in (
             "CREATE_IN_PROGRESS",
             "UPDATE_IN_PROGRESS",
         ):
+            # NOTE(mnaser): It's possible we run a cluster status update before
+            #               the cluster is created. In that case, we don't want
+            #               to update the cluster status.
+            if capi_cluster is None:
+                return
+
             capi_cluster.reload()
             status_map = {
                 c["type"]: c["status"] for c in capi_cluster.obj["status"]["conditions"]
             }
 
             for condition in ("ControlPlaneReady", "InfrastructureReady", "Ready"):
                 if status_map.get(condition) != "True":
@@ -199,15 +205,15 @@
         action = nodegroup.status.split("_")[0]
 
         if nodegroup.role == "master":
             kcp = resources.get_kubeadm_control_plane(self.k8s_api, cluster)
             if kcp is None:
                 return nodegroup
 
-            generation = kcp.obj["status"].get("observedGeneration")
+            generation = kcp.obj.get("status", {}).get("observedGeneration", 1)
             if generation > 1:
                 action = "UPDATE"
 
             ready = kcp.obj["status"].get("ready", False)
             failure_message = kcp.obj["status"].get("failureMessage")
 
             updated_replicas = kcp.obj["status"].get("updatedReplicas")
```

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/helm.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/image_utils.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/images.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/audit/policy.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/audit/policy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/calico/v3.24.2.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml` & `magnum_cluster_api-0.5.1/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/monitor.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/monitor.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 LOG = logging.getLogger(__name__)
 
 
 class Monitor(k8s_monitor.K8sMonitor):
     def poll_health_status(self):
         # NOTE(mnaser): We override the `api_address` for the cluster if it's
         #               an isolated cluster so we can go through the proxy.
-        if utils.get_cluster_floating_ip_disabled(self.cluster):
-            api_address = f"https://{self.cluster.stack_id}.magnum-system:6443"
-            self.cluster.api_address = api_address
+        cluster = self.cluster.obj_clone()
+        if utils.get_cluster_floating_ip_disabled(cluster):
+            api_address = f"https://{cluster.stack_id}.magnum-system:6443"
+            cluster.api_address = api_address
             LOG.debug("Overriding cluster api_address to %s", api_address)
 
-        k8s_api = k8s.KubernetesAPI(self.context, self.cluster)
+        k8s_api = k8s.KubernetesAPI(self.context, cluster)
         status, reason = self._poll_health_status(k8s_api)
 
         self.data["health_status"] = status
         self.data["health_status_reason"] = reason
```

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/objects.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/objects.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/privsep/__init__.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/privsep/__init__.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/privsep/haproxy.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/privsep/haproxy.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/proxy/manager.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/proxy/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import base64
 import socket
+from datetime import datetime, timezone
 from pathlib import Path
 
 import jinja2
 import pykube
 import yaml
 from oslo_config import cfg
 from oslo_log import log as logging
@@ -183,35 +184,41 @@
                     {
                         "apiVersion": objects.EndpointSlice.version,
                         "kind": objects.EndpointSlice.kind,
                         "metadata": {
                             "name": proxied_cluster.endpoint_slice_name,
                             "namespace": "magnum-system",
                             "labels": proxied_cluster.endpoint_slice_labels,
+                            "annotations": proxied_cluster.endpoint_slice_annotations,
                         },
                         "addressType": "IPv4",
                         "endpoints": proxied_cluster.endpoint_slice_endpoints,
                         "ports": endpoint_slice_ports,
                     },
                 ).create()
                 endpoint_slice = objects.EndpointSlice.objects(
                     self.api, namespace="magnum-system"
                 ).get(name=proxied_cluster.endpoint_slice_name)
 
             if (
                 endpoint_slice.metadata["labels"]
                 != proxied_cluster.endpoint_slice_labels
+                or endpoint_slice.metadata["annotations"]
+                != proxied_cluster.endpoint_slice_annotations
                 or endpoint_slice.obj["endpoints"]
                 != proxied_cluster.endpoint_slice_endpoints
                 or endpoint_slice.obj["ports"] != endpoint_slice_ports
             ):
                 LOG.info("Updating EndpointSlice %s", endpoint_slice.name)
                 endpoint_slice.metadata[
                     "labels"
                 ] = proxied_cluster.endpoint_slice_labels
+                endpoint_slice.metadata[
+                    "annotations"
+                ] = proxied_cluster.endpoint_slice_annotations
                 endpoint_slice.obj[
                     "endpoints"
                 ] = proxied_cluster.endpoint_slice_endpoints
                 endpoint_slice.obj["ports"] = endpoint_slice_ports
                 endpoint_slice.update()
 
     def _sync_kubeconfigs(self, proxied_clusters: list):
@@ -246,14 +253,32 @@
 
             # Update the secret with the new kubeconfig
             secret.obj["data"]["value"] = base64.b64encode(
                 yaml.safe_dump(kubeconfig).encode("utf-8")
             ).decode("utf-8")
             secret.update()
 
+    def _cleanup_endpoint_slices(self):
+        # Get list of all endpoint slices managed by the proxy service
+        endpoint_slices = objects.EndpointSlice.objects(
+            self.api, namespace="magnum-system"
+        ).filter(selector={structs.ProxiedCluster.SERVICE_LABEL: "true"})
+
+        # Look if any of the endpoint slices should be expired (aka >30s age)
+        for endpoint_slice in endpoint_slices:
+            timestamp = datetime.fromisoformat(
+                endpoint_slice.metadata["annotations"][
+                    structs.ProxiedCluster.TIMESTAMP_ANNOTATION
+                ]
+            )
+
+            if (datetime.now(timezone.utc) - timestamp).total_seconds() > 30:
+                LOG.info("Deleting expired EndpointSlice %s", endpoint_slice.name)
+                endpoint_slice.delete()
+
     @periodic_task.periodic_task(spacing=10, run_immediately=True)
     def sync(self, context):
         # Generate list of all clusters
         clusters = objects.OpenStackCluster.objects(
             self.api, namespace="magnum-system"
         ).all()
 
@@ -264,7 +289,8 @@
             if proxied_cluster:
                 proxied_clusters.append(proxied_cluster)
 
         self._sync_haproxy(proxied_clusters)
         self._sync_services(proxied_clusters, clusters)
         self._sync_endpoint_slices(proxied_clusters)
         self._sync_kubeconfigs(proxied_clusters)
+        self._cleanup_endpoint_slices()
```

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/proxy/structs.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/proxy/structs.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import dataclasses
 import os
 import socket
+from datetime import datetime, timezone
 
 from oslo_log import log as logging
 from pyroute2 import netns
 
 from magnum_cluster_api import objects
 from magnum_cluster_api.proxy import utils
 
@@ -28,14 +29,15 @@
 @dataclasses.dataclass
 class ProxiedCluster:
     """A cluster that is proxied by this service."""
 
     NODE_LABEL = "magnum-cluster-api.vexxhost.com/node"
     CLUSTER_LABEL = "magnum-cluster-api.vexxhost.com/proxied-cluster"
     SERVICE_LABEL = "magnum-cluster-api.vexxhost.com/proxied-service"
+    TIMESTAMP_ANNOTATION = "magnum-cluster-api.vexxhost.com/timestamp"
 
     name: str
     internal_ip: str
     namespace: str
 
     @classmethod
     def from_openstack_cluster(
@@ -75,14 +77,21 @@
 
     @property
     def endpoint_slice_labels(self) -> dict:
         return {
             "kubernetes.io/service-name": self.name,
             self.NODE_LABEL: socket.gethostname(),
             self.CLUSTER_LABEL: self.name,
+            self.SERVICE_LABEL: "true",
+        }
+
+    @property
+    def endpoint_slice_annotations(self) -> dict:
+        return {
+            self.TIMESTAMP_ANNOTATION: datetime.now(timezone.utc).isoformat(),
         }
 
     @property
     def endpoint_slice_endpoints(self) -> list:
         ip = os.getenv("POD_IP", utils.get_default_ip_address())
 
         return [
```

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2` & `magnum_cluster_api-0.5.1/magnum_cluster_api/proxy/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/proxy/utils.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/proxy/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/resources.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/resources.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/service.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/service.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/tests/test_helm.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/tests/test_image_utils.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/tests/test_images.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/magnum_cluster_api/utils.py` & `magnum_cluster_api-0.5.1/magnum_cluster_api/utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.5.0/pyproject.toml` & `magnum_cluster_api-0.5.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "magnum-cluster-api"
-version = "0.5.0"
+version = "0.5.1"
 description = "Cluster API driver for Magnum"
 authors = ["Mohammed Naser <mnaser@vexxhost.com>"]
 readme = "README.md"
 packages = [{include = "magnum_cluster_api"}]
 include = ["magnum_cluster_api/charts/**/*"]
 
 [tool.poetry.dependencies]
 certifi = "*"
 click = ">=8.0.4"
 magnum = ">=14.0.0"
-oslo-concurrency = ">=4.5.0"
-oslo-config = ">=8.8.0"
-oslo-context = ">=4.1.0"
-oslo-log = ">=4.7.0"
-oslo-privsep = ">=2.7.0"
-oslo-service = ">=2.8.0"
+"oslo.concurrency" = ">=4.5.0"
+"oslo.config" = ">=8.8.0"
+"oslo.context" = ">=4.1.0"
+"oslo.log" = ">=4.7.0"
+"oslo.privsep" = ">=2.7.0"
+"oslo.service" = ">=2.8.0"
 pykube-ng = "*"
 pyroute2 = ">=0.3.4"
 python = "^3.6"
 requests = ">=2.27.1"
 semver = "^2.0.0"
 shortuuid = "*"
```

### Comparing `magnum_cluster_api-0.5.0/PKG-INFO` & `magnum_cluster_api-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: magnum-cluster-api
-Version: 0.5.0
+Version: 0.5.1
 Summary: Cluster API driver for Magnum
 Author: Mohammed Naser
 Author-email: mnaser@vexxhost.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi
 Requires-Dist: click (>=8.0.4)
 Requires-Dist: magnum (>=14.0.0)
-Requires-Dist: oslo-concurrency (>=4.5.0)
-Requires-Dist: oslo-config (>=8.8.0)
-Requires-Dist: oslo-context (>=4.1.0)
-Requires-Dist: oslo-log (>=4.7.0)
-Requires-Dist: oslo-privsep (>=2.7.0)
-Requires-Dist: oslo-service (>=2.8.0)
+Requires-Dist: oslo.concurrency (>=4.5.0)
+Requires-Dist: oslo.config (>=8.8.0)
+Requires-Dist: oslo.context (>=4.1.0)
+Requires-Dist: oslo.log (>=4.7.0)
+Requires-Dist: oslo.privsep (>=2.7.0)
+Requires-Dist: oslo.service (>=2.8.0)
 Requires-Dist: pykube-ng
 Requires-Dist: pyroute2 (>=0.3.4)
 Requires-Dist: requests (>=2.27.1)
 Requires-Dist: semver (>=2.0.0,<3.0.0)
 Requires-Dist: shortuuid
 Description-Content-Type: text/markdown
```

