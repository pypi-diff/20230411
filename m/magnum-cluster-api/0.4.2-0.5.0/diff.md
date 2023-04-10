# Comparing `tmp/magnum_cluster_api-0.4.2.tar.gz` & `tmp/magnum_cluster_api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnum_cluster_api-0.4.2.tar", max compression
+gzip compressed data, was "magnum_cluster_api-0.5.0.tar", max compression
```

## Comparing `magnum_cluster_api-0.4.2.tar` & `magnum_cluster_api-0.5.0.tar`

### file list

```diff
@@ -1,53 +1,62 @@
--rw-r--r--   0        0        0    10142 2023-04-04 18:16:18.698675 magnum_cluster_api-0.4.2/LICENSE
--rw-r--r--   0        0        0     2795 2023-04-04 18:16:18.698675 magnum_cluster_api-0.4.2/README.md
--rw-r--r--   0        0        0        0 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/.gitkeep
--rw-r--r--   0        0        0      349 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
--rw-r--r--   0        0        0      437 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
--rw-r--r--   0        0        0    29122 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/README.md
--rw-r--r--   0        0        0    14987 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
--rw-r--r--   0        0        0      827 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
--rw-r--r--   0        0        0     4034 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
--rw-r--r--   0        0        0     2982 2023-04-04 18:16:29.654623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
--rw-r--r--   0        0        0      534 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
--rw-r--r--   0        0        0    13204 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
--rw-r--r--   0        0        0      508 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
--rw-r--r--   0        0        0      972 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
--rw-r--r--   0        0        0      758 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
--rw-r--r--   0        0        0      564 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
--rw-r--r--   0        0        0     1807 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
--rw-r--r--   0        0        0      527 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
--rw-r--r--   0        0        0      989 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
--rw-r--r--   0        0        0     1180 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
--rw-r--r--   0        0        0      528 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      960 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
--rw-r--r--   0        0        0      663 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
--rw-r--r--   0        0        0    18003 2023-04-04 18:16:29.650623 magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
--rw-r--r--   0        0        0      843 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/clients.py
--rw-r--r--   0        0        0        0 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/cmd/__init__.py
--rw-r--r--   0        0        0     4019 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/cmd/image_builder.py
--rw-r--r--   0        0        0     4167 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/cmd/image_loader.py
--rw-r--r--   0        0        0     1778 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/conf.py
--rw-r--r--   0        0        0    10583 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/driver.py
--rw-r--r--   0        0        0     2155 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/helm.py
--rw-r--r--   0        0        0     3161 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/image_utils.py
--rw-r--r--   0        0        0     1116 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/images.py
--rw-r--r--   0        0        0        0 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/__init__.py
--rw-r--r--   0        0        0     4941 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/audit/policy.yaml
--rw-r--r--   0        0        0   235191 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/calico/v3.24.2.yaml
--rw-r--r--   0        0        0      623 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
--rw-r--r--   0        0        0     1430 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
--rw-r--r--   0        0        0     2263 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
--rw-r--r--   0        0        0     4506 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml
--rw-r--r--   0        0        0     4009 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml
--rw-r--r--   0        0        0      609 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml
--rw-r--r--   0        0        0     3297 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml
--rw-r--r--   0        0        0      194 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/csi/csi-cinder-driver.yaml
--rw-r--r--   0        0        0     2542 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/objects.py
--rw-r--r--   0        0        0    67927 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/resources.py
--rw-r--r--   0        0        0     3445 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/tests/test_helm.py
--rw-r--r--   0        0        0     1598 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/tests/test_image_utils.py
--rw-r--r--   0        0        0     2759 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/tests/test_images.py
--rw-r--r--   0        0        0     7384 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/magnum_cluster_api/utils.py
--rw-r--r--   0        0        0      933 2023-04-04 18:16:18.702675 magnum_cluster_api-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3562 1970-01-01 00:00:00.000000 magnum_cluster_api-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2795 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/.gitkeep
+-rw-r--r--   0        0        0      349 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/.helmignore
+-rw-r--r--   0        0        0      437 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/Chart.yaml
+-rw-r--r--   0        0        0    29122 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/README.md
+-rw-r--r--   0        0        0    14987 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl
+-rw-r--r--   0        0        0      827 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt
+-rw-r--r--   0        0        0     4034 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2982 2023-04-10 23:30:35.459469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml
+-rw-r--r--   0        0        0      534 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml
+-rw-r--r--   0        0        0    13204 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml
+-rw-r--r--   0        0        0      508 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/pdb.yaml
+-rw-r--r--   0        0        0      972 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml
+-rw-r--r--   0        0        0      758 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml
+-rw-r--r--   0        0        0      564 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml
+-rw-r--r--   0        0        0     1807 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml
+-rw-r--r--   0        0        0      527 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml
+-rw-r--r--   0        0        0      989 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml
+-rw-r--r--   0        0        0     1180 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml
+-rw-r--r--   0        0        0      528 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      960 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml
+-rw-r--r--   0        0        0      663 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml
+-rw-r--r--   0        0        0    18003 2023-04-10 23:30:35.451469 magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml
+-rw-r--r--   0        0        0      843 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/clients.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/cmd/__init__.py
+-rw-r--r--   0        0        0     4019 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/cmd/image_builder.py
+-rw-r--r--   0        0        0     4167 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/cmd/image_loader.py
+-rw-r--r--   0        0        0      956 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/cmd/proxy.py
+-rw-r--r--   0        0        0     1778 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/conf.py
+-rw-r--r--   0        0        0    10572 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/driver.py
+-rw-r--r--   0        0        0     2155 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/helm.py
+-rw-r--r--   0        0        0     3161 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/image_utils.py
+-rw-r--r--   0        0        0     1116 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/images.py
+-rw-r--r--   0        0        0        0 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/__init__.py
+-rw-r--r--   0        0        0     4941 2023-04-10 23:30:22.150380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/audit/policy.yaml
+-rw-r--r--   0        0        0   235191 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml
+-rw-r--r--   0        0        0      623 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml
+-rw-r--r--   0        0        0     1430 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml
+-rw-r--r--   0        0        0     2263 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml
+-rw-r--r--   0        0        0     4506 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml
+-rw-r--r--   0        0        0     4009 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml
+-rw-r--r--   0        0        0      609 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml
+-rw-r--r--   0        0        0     3297 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml
+-rw-r--r--   0        0        0      194 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/csi-cinder-driver.yaml
+-rw-r--r--   0        0        0     1503 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/monitor.py
+-rw-r--r--   0        0        0     2880 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/objects.py
+-rw-r--r--   0        0        0      828 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/privsep/__init__.py
+-rw-r--r--   0        0        0     1333 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/privsep/haproxy.py
+-rw-r--r--   0        0        0    10475 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/proxy/manager.py
+-rw-r--r--   0        0        0     3294 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/proxy/structs.py
+-rw-r--r--   0        0        0      580 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/proxy/templates/haproxy.cfg.j2
+-rw-r--r--   0        0        0     1511 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/proxy/utils.py
+-rw-r--r--   0        0        0    74957 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/resources.py
+-rw-r--r--   0        0        0     1492 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/service.py
+-rw-r--r--   0        0        0     3445 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/tests/test_helm.py
+-rw-r--r--   0        0        0     1598 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/tests/test_image_utils.py
+-rw-r--r--   0        0        0     2759 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/tests/test_images.py
+-rw-r--r--   0        0        0     7554 2023-04-10 23:30:22.154380 magnum_cluster_api-0.5.0/magnum_cluster_api/utils.py
+-rw-r--r--   0        0        0     1174 2023-04-10 23:30:22.158381 magnum_cluster_api-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 magnum_cluster_api-0.5.0/PKG-INFO
```

### Comparing `magnum_cluster_api-0.4.2/LICENSE` & `magnum_cluster_api-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/README.md` & `magnum_cluster_api-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/README.md` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/README.md`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/README.md.gotmpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/podsecuritypolicy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/priority-expander-configmap.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/prometheusrule.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/rolebinding.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/serviceaccount.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/servicemonitor.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/templates/vpa.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/charts/cluster-autoscaler/values.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/charts/cluster-autoscaler/values.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/clients.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/clients.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/cmd/image_builder.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/cmd/image_builder.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/cmd/image_loader.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/cmd/image_loader.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/conf.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/conf.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/driver.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import keystoneauth1
 from magnum import objects as magnum_objects
-from magnum.drivers.common import driver, k8s_monitor
+from magnum.drivers.common import driver
 
-from magnum_cluster_api import clients, objects, resources, utils
+from magnum_cluster_api import clients, monitor, objects, resources, utils
 
 
 class BaseDriver(driver.Driver):
     def __init__(self):
         self.k8s_api = clients.get_pykube_api()
 
     def create_cluster(self, context, cluster, cluster_create_timeout):
@@ -257,15 +257,15 @@
         resources.apply_cluster_from_magnum_cluster(
             context,
             self.k8s_api,
             cluster,
         )
 
     def get_monitor(self, context, cluster):
-        return k8s_monitor.K8sMonitor(context, cluster)
+        return monitor.Monitor(context, cluster)
 
     # def rotate_ca_certificate(self, context, cluster):
     #     raise exception.NotSupported(
     #         "'rotate_ca_certificate' is not supported by this driver.")
 
     def create_federation(self, context, federation):
         raise NotImplementedError()
```

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/helm.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/image_utils.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/images.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/audit/policy.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/audit/policy.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/calico/v3.24.2.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/calico/v3.24.2.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-role-bindings.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/ccm/cloud-controller-manager-roles.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/ccm/openstack-cloud-controller-manager-ds.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-controllerplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin-rbac.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml` & `magnum_cluster_api-0.5.0/magnum_cluster_api/manifests/csi/cinder-csi-nodeplugin.yaml`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/objects.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 import pykube
 
 
+class EndpointSlice(pykube.objects.NamespacedAPIObject):
+    version = "discovery.k8s.io/v1"
+    endpoint = "endpointslices"
+    kind = "EndpointSlice"
+
+
 class ClusterResourceSet(pykube.objects.NamespacedAPIObject):
     version = "addons.cluster.x-k8s.io/v1beta1"
     endpoint = "clusterresourcesets"
     kind = "ClusterResourceSet"
 
 
 class OpenStackMachineTemplate(pykube.objects.NamespacedAPIObject):
@@ -59,14 +65,20 @@
 
 class OpenStackClusterTemplate(pykube.objects.NamespacedAPIObject):
     version = "infrastructure.cluster.x-k8s.io/v1alpha6"
     endpoint = "openstackclustertemplates"
     kind = "OpenStackClusterTemplate"
 
 
+class OpenStackCluster(pykube.objects.NamespacedAPIObject):
+    version = "infrastructure.cluster.x-k8s.io/v1alpha6"
+    endpoint = "openstackclusters"
+    kind = "OpenStackCluster"
+
+
 class ClusterClass(pykube.objects.NamespacedAPIObject):
     version = "cluster.x-k8s.io/v1beta1"
     endpoint = "clusterclasses"
     kind = "ClusterClass"
 
 
 class Cluster(pykube.objects.NamespacedAPIObject):
```

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/resources.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/resources.py`

 * *Files 6% similar despite different names*

```diff
@@ -733,14 +733,23 @@
                             "schema": {
                                 "openAPIV3Schema": {
                                     "type": "string",
                                 },
                             },
                         },
                         {
+                            "name": "disableAPIServerFloatingIP",
+                            "required": True,
+                            "schema": {
+                                "openAPIV3Schema": {
+                                    "type": "boolean",
+                                },
+                            },
+                        },
+                        {
                             "name": "dnsNameservers",
                             "required": True,
                             "schema": {
                                 "openAPIV3Schema": {
                                     "type": "array",
                                     "items": {
                                         "type": "string",
@@ -754,14 +763,32 @@
                             "schema": {
                                 "openAPIV3Schema": {
                                     "type": "string",
                                 },
                             },
                         },
                         {
+                            "name": "fixedNetworkName",
+                            "required": True,
+                            "schema": {
+                                "openAPIV3Schema": {
+                                    "type": "string",
+                                },
+                            },
+                        },
+                        {
+                            "name": "fixedSubnetId",
+                            "required": True,
+                            "schema": {
+                                "openAPIV3Schema": {
+                                    "type": "string",
+                                },
+                            },
+                        },
+                        {
                             "name": "flavor",
                             "required": True,
                             "schema": {
                                 "openAPIV3Schema": {
                                     "type": "string",
                                 },
                             },
@@ -992,34 +1019,104 @@
                                             "path": "/spec/template/spec/identityRef",
                                             "valueFrom": {
                                                 "variable": "clusterIdentityRef"
                                             },
                                         },
                                         {
                                             "op": "add",
+                                            "path": "/spec/template/spec/disableAPIServerFloatingIP",
+                                            "valueFrom": {
+                                                "variable": "disableAPIServerFloatingIP"
+                                            },
+                                        },
+                                        {
+                                            "op": "add",
                                             "path": "/spec/template/spec/dnsNameservers",
                                             "valueFrom": {"variable": "dnsNameservers"},
                                         },
                                         {
                                             "op": "add",
                                             "path": "/spec/template/spec/externalNetworkId",
                                             "valueFrom": {
                                                 "variable": "externalNetworkId"
                                             },
                                         },
+                                    ],
+                                },
+                            ],
+                        },
+                        {
+                            "name": "newNetworkConfig",
+                            "enabledIf": '{{ if eq .fixedNetworkName "" }}true{{end}}',
+                            "definitions": [
+                                {
+                                    "selector": {
+                                        "apiVersion": objects.OpenStackClusterTemplate.version,
+                                        "kind": objects.OpenStackClusterTemplate.kind,
+                                        "matchResources": {
+                                            "infrastructureCluster": True,
+                                        },
+                                    },
+                                    "jsonPatches": [
                                         {
                                             "op": "add",
                                             "path": "/spec/template/spec/nodeCidr",
                                             "valueFrom": {"variable": "nodeCidr"},
                                         },
                                     ],
                                 },
                             ],
                         },
                         {
+                            "name": "existingFixedNetworkNameConfig",
+                            "enabledIf": '{{ if ne .fixedNetworkName "" }}true{{end}}',
+                            "definitions": [
+                                {
+                                    "selector": {
+                                        "apiVersion": objects.OpenStackClusterTemplate.version,
+                                        "kind": objects.OpenStackClusterTemplate.kind,
+                                        "matchResources": {
+                                            "infrastructureCluster": True,
+                                        },
+                                    },
+                                    "jsonPatches": [
+                                        {
+                                            "op": "add",
+                                            "path": "/spec/template/spec/network/name",
+                                            "valueFrom": {
+                                                "variable": "fixedNetworkName"
+                                            },
+                                        },
+                                    ],
+                                },
+                            ],
+                        },
+                        {
+                            "name": "existingFixedSubnetIdConfig",
+                            "enabledIf": '{{ if ne .fixedSubnetId "" }}true{{end}}',
+                            "definitions": [
+                                {
+                                    "selector": {
+                                        "apiVersion": objects.OpenStackClusterTemplate.version,
+                                        "kind": objects.OpenStackClusterTemplate.kind,
+                                        "matchResources": {
+                                            "infrastructureCluster": True,
+                                        },
+                                    },
+                                    "jsonPatches": [
+                                        {
+                                            "op": "add",
+                                            "path": "/spec/template/spec/subnet/id",
+                                            "valueFrom": {"variable": "fixedSubnetId"},
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
@@ -1047,14 +1144,28 @@
                                             "path": "/spec/template/spec/kubeadmConfigSpec/clusterConfiguration/imageRepository",  # noqa: E501
                                             "valueFrom": {
                                                 "variable": "imageRepository",
                                             },
                                         },
                                         {
                                             "op": "add",
+                                            "path": "/spec/template/spec/kubeadmConfigSpec/clusterConfiguration/apiServer/certSANs",  # noqa: E501
+                                            "valueFrom": {
+                                                "template": textwrap.dedent(
+                                                    """\
+                                                    - {{ .builtin.cluster.name }}
+                                                    - {{ .builtin.cluster.name }}.{{ .builtin.cluster.namespace }}
+                                                    - {{ .builtin.cluster.name }}.{{ .builtin.cluster.namespace }}.svc
+                                                    - {{ .builtin.cluster.name }}.{{ .builtin.cluster.namespace }}.svc.cluster.local # noqa: E501
+                                                    """
+                                                ),
+                                            },
+                                        },
+                                        {
+                                            "op": "add",
                                             "path": "/spec/template/spec/kubeadmConfigSpec/files/-",
                                             "valueFrom": {
                                                 "template": textwrap.dedent(
                                                     """\
                                                     path: "/etc/kubernetes/cloud.conf"
                                                     owner: "root:root"
                                                     permissions: "0600"
@@ -1354,27 +1465,47 @@
                                 ),
                             },
                             {
                                 "name": "controlPlaneFlavor",
                                 "value": self.cluster.master_flavor_id,
                             },
                             {
+                                "name": "disableAPIServerFloatingIP",
+                                "value": utils.get_cluster_floating_ip_disabled(
+                                    self.cluster
+                                ),
+                            },
+                            {
                                 "name": "dnsNameservers",
                                 "value": self.cluster.cluster_template.dns_nameserver.split(
                                     ","
                                 ),
                             },
                             {
                                 "name": "externalNetworkId",
                                 "value": neutron.get_external_network_id(
                                     self.context,
                                     self.cluster.cluster_template.external_network_id,
                                 ),
                             },
                             {
+                                "name": "fixedNetworkName",
+                                "value": neutron.get_fixed_network_name(
+                                    self.context, self.cluster.fixed_network
+                                )
+                                or "",
+                            },
+                            {
+                                "name": "fixedSubnetId",
+                                "value": neutron.get_fixed_subnet_id(
+                                    self.context, self.cluster.fixed_subnet
+                                )
+                                or "",
+                            },
+                            {
                                 "name": "flavor",
                                 "value": self.cluster.flavor_id,
                             },
                             {
                                 "name": "imageRepository",
                                 "value": utils.get_cluster_container_infra_prefix(
                                     self.cluster,
```

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/tests/test_helm.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/tests/test_image_utils.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/tests/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/tests/test_images.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `magnum_cluster_api-0.4.2/magnum_cluster_api/utils.py` & `magnum_cluster_api-0.5.0/magnum_cluster_api/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,14 +98,18 @@
     return get_cluster_label(
         cluster,
         "container_infra_prefix",
         "quay.io/vexxhost",
     )
 
 
+def get_cluster_floating_ip_disabled(cluster: magnum_objects.Cluster) -> bool:
+    return not get_cluster_label_as_bool(cluster, "master_lb_floating_ip_enabled", True)
+
+
 def generate_containerd_config(
     cluster: magnum_objects.Cluster,
 ):
     image_repository = get_cluster_container_infra_prefix(cluster)
     sandbox_image = image_utils.get_image(images.PAUSE, image_repository)
 
     return textwrap.dedent(
```

### Comparing `magnum_cluster_api-0.4.2/pyproject.toml` & `magnum_cluster_api-0.5.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 [tool.poetry]
 name = "magnum-cluster-api"
-version = "0.4.2"
+version = "0.5.0"
 description = "Cluster API driver for Magnum"
 authors = ["Mohammed Naser <mnaser@vexxhost.com>"]
 readme = "README.md"
 packages = [{include = "magnum_cluster_api"}]
 include = ["magnum_cluster_api/charts/**/*"]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-pykube-ng = "*"
-click = "*"
-requests = "*"
-shortuuid = "*"
 certifi = "*"
-"oslo.concurrency" = "*"
+click = ">=8.0.4"
+magnum = ">=14.0.0"
+oslo-concurrency = ">=4.5.0"
+oslo-config = ">=8.8.0"
+oslo-context = ">=4.1.0"
+oslo-log = ">=4.7.0"
+oslo-privsep = ">=2.7.0"
+oslo-service = ">=2.8.0"
+pykube-ng = "*"
+pyroute2 = ">=0.3.4"
+python = "^3.6"
+requests = ">=2.27.1"
 semver = "^2.0.0"
+shortuuid = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "<7"
 pytest-mock = "^3.6.1"
 
 [build-system]
 requires = ["setuptools", "poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 magnum-cluster-api-image-builder = "magnum_cluster_api.cmd.image_builder:main"
 magnum-cluster-api-image-loader = "magnum_cluster_api.cmd.image_loader:main"
+magnum-cluster-api-proxy = "magnum_cluster_api.cmd.proxy:main"
 
 [tool.poetry.plugins."magnum.drivers"]
 "k8s_cluster_api_ubuntu_focal" = "magnum_cluster_api.driver:UbuntuFocalDriver"
 
 [tool.isort]
 profile = "black"
```

### Comparing `magnum_cluster_api-0.4.2/PKG-INFO` & `magnum_cluster_api-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: magnum-cluster-api
-Version: 0.4.2
+Version: 0.5.0
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
-Requires-Dist: click
-Requires-Dist: oslo.concurrency
+Requires-Dist: click (>=8.0.4)
+Requires-Dist: magnum (>=14.0.0)
+Requires-Dist: oslo-concurrency (>=4.5.0)
+Requires-Dist: oslo-config (>=8.8.0)
+Requires-Dist: oslo-context (>=4.1.0)
+Requires-Dist: oslo-log (>=4.7.0)
+Requires-Dist: oslo-privsep (>=2.7.0)
+Requires-Dist: oslo-service (>=2.8.0)
 Requires-Dist: pykube-ng
-Requires-Dist: requests
+Requires-Dist: pyroute2 (>=0.3.4)
+Requires-Dist: requests (>=2.27.1)
 Requires-Dist: semver (>=2.0.0,<3.0.0)
 Requires-Dist: shortuuid
 Description-Content-Type: text/markdown
 
 ![Cluster API driver for Magnum](docs/static/logo.png?raw=true "Cluster API driver for Magnum")
 
 ## Images
```

