# Comparing `tmp/c7n_tencentcloud-0.1.6-py3-none-any.whl.zip` & `tmp/c7n_tencentcloud-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 44610 bytes, number of entries: 33
+Zip file size: 45409 bytes, number of entries: 33
 -rw-r--r--  2.0 unx       79 b- defN 80-Jan-01 00:00 c7n_tencentcloud/__init__.py
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 c7n_tencentcloud/actions/__init__.py
 -rw-r--r--  2.0 unx      819 b- defN 80-Jan-01 00:00 c7n_tencentcloud/actions/core.py
 -rw-r--r--  2.0 unx    10845 b- defN 80-Jan-01 00:00 c7n_tencentcloud/actions/tags.py
 -rw-r--r--  2.0 unx     7239 b- defN 80-Jan-01 00:00 c7n_tencentcloud/client.py
 -rw-r--r--  2.0 unx      329 b- defN 80-Jan-01 00:00 c7n_tencentcloud/entry.py
 -rw-r--r--  2.0 unx      116 b- defN 80-Jan-01 00:00 c7n_tencentcloud/filters/__init__.py
@@ -20,16 +20,16 @@
 -rw-r--r--  2.0 unx    12063 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/cos.py
 -rw-r--r--  2.0 unx     5495 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/cvm.py
 -rw-r--r--  2.0 unx     1474 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/elasticsearch.py
 -rw-r--r--  2.0 unx     3041 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/mysql.py
 -rw-r--r--  2.0 unx     2171 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/mysql_backup.py
 -rw-r--r--  2.0 unx     2151 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/nat_gateway.py
 -rw-r--r--  2.0 unx     1253 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/resource_map.py
--rw-r--r--  2.0 unx     7363 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/security_group.py
+-rw-r--r--  2.0 unx     9155 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/security_group.py
 -rw-r--r--  2.0 unx     1399 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/tag.py
 -rw-r--r--  2.0 unx     3179 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/tcr.py
 -rw-r--r--  2.0 unx     3138 b- defN 80-Jan-01 00:00 c7n_tencentcloud/resources/vpc.py
 -rw-r--r--  2.0 unx     1252 b- defN 80-Jan-01 00:00 c7n_tencentcloud/utils.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_tencentcloud-0.1.6.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1629 b- defN 16-Jan-01 00:00 c7n_tencentcloud-0.1.6.dist-info/METADATA
-?rw-------  2.0 unx     2948 b- defN 23-Mar-16 04:36 c7n_tencentcloud-0.1.6.dist-info/RECORD
-33 files, 129277 bytes uncompressed, 39822 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 c7n_tencentcloud-0.1.7.dist-info/WHEEL
+?rw-r--r--  2.0 unx     4207 b- defN 16-Jan-01 00:00 c7n_tencentcloud-0.1.7.dist-info/METADATA
+?rw-------  2.0 unx     2948 b- defN 23-Apr-11 08:33 c7n_tencentcloud-0.1.7.dist-info/RECORD
+33 files, 133647 bytes uncompressed, 40621 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -84,17 +84,17 @@
 
 Filename: c7n_tencentcloud/resources/vpc.py
 Comment: 
 
 Filename: c7n_tencentcloud/utils.py
 Comment: 
 
-Filename: c7n_tencentcloud-0.1.6.dist-info/WHEEL
+Filename: c7n_tencentcloud-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: c7n_tencentcloud-0.1.6.dist-info/METADATA
+Filename: c7n_tencentcloud-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: c7n_tencentcloud-0.1.6.dist-info/RECORD
+Filename: c7n_tencentcloud-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## c7n_tencentcloud/resources/security_group.py

```diff
@@ -1,9 +1,10 @@
 # Copyright The Cloud Custodian Authors.
 # SPDX-License-Identifier: Apache-2.0
+from c7n.utils import type_schema, chunks
 from c7n_tencentcloud.provider import resources
 from c7n_tencentcloud.query import ResourceTypeInfo, QueryResourceManager
 from c7n_tencentcloud.utils import PageMethod
 from c7n.filters.core import Filter, ValueFilter
 
 
 @resources.register('security-group')
@@ -196,7 +197,59 @@
             'type': {'enum': ['egress']},
             'Ports': {'type': 'array', 'items': {'type': 'integer'}},
             'AnyPortsExcept': {'type': 'array', 'items': {'type': 'integer'}},
             'Cidr': {},
             'CidrV6': {}
         },
         'required': ['type']}
+
+
+@SecurityGroup.filter_registry.register('used')
+class StatisticsFilter(ValueFilter):
+    """statistics
+
+    :example:
+
+    .. code-block:: yaml
+
+        policies:
+        - name: used
+          resource: tencentcloud.security-group
+          description: security group used statistical
+          filters:
+            - type: used
+              key: CVM
+              op: greater-than
+              value: 0
+    """
+
+    schema = type_schema('used', rinherit=ValueFilter.schema)
+    annotation_key = "c7n:usage_stats"
+
+    def match(self, i):
+        return super().match(i[self.annotation_key])
+
+    def process(self, resources, event=None):
+        self.augment([r for r in resources if self.annotation_key not in r])
+        return super().process(resources)
+
+    def augment(self, resources):
+        client = self.manager.get_client()
+
+        # DescribeSecurityGroupAssociationStatistics Maximum support 100
+        for batch in chunks(resources, 50):
+            id_resource_map = {r['SecurityGroupId']: r for r in batch}
+            resp = client.execute_query(
+                "DescribeSecurityGroupAssociationStatistics",
+                {"SecurityGroupIds": list(id_resource_map)}
+            )
+            statistics = resp["Response"]["SecurityGroupAssociationStatisticsSet"]
+            for stat in statistics:
+                group = id_resource_map[stat['SecurityGroupId']]
+                group[self.annotation_key] = {
+                    istat['InstanceType']: istat['InstanceCount'] for istat
+                    in stat['InstanceStatistics']
+                }
+                group[self.annotation_key].update(
+                    {'TotalCount': stat['TotalCount'], 'SG': stat['SG']}
+                )
+        return resources
```

## Comparing `c7n_tencentcloud-0.1.6.dist-info/RECORD` & `c7n_tencentcloud-0.1.7.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 c7n_tencentcloud/resources/cos.py,sha256=kY_AjOSqMdrsMvcnwqItluuBHgdmsBVjrUtIyCwc4Lg,12063
 c7n_tencentcloud/resources/cvm.py,sha256=EKMSSe9VsVt5zKmJvfZ8OZCD6mTgQM_VS4pUvkAYrsI,5495
 c7n_tencentcloud/resources/elasticsearch.py,sha256=T1FtH_2RKiOxLsYM5xyQ8jsm18MDX3OFWex2wBlgr6I,1474
 c7n_tencentcloud/resources/mysql.py,sha256=RcAHBVCCXD4sUD54o7wLcVV6D9lJK9qEUBihJZ_v-9Q,3041
 c7n_tencentcloud/resources/mysql_backup.py,sha256=1iUOdIxyxvfXNANCARTe6Ihx_p5ljr4eFOYEgGGQAtY,2171
 c7n_tencentcloud/resources/nat_gateway.py,sha256=b3DhZKC8x92paORrZQ3FbX2sWEit0Iweketn1rK7qqs,2151
 c7n_tencentcloud/resources/resource_map.py,sha256=dm-1PqUUgdyQW5Q2hsfstP4Gw1Z77UFMv_T94pOg2PM,1253
-c7n_tencentcloud/resources/security_group.py,sha256=BiQXc2Dj5QQITBp9pfmz-xrgwdB0e89_WH7hh9SKqF4,7363
+c7n_tencentcloud/resources/security_group.py,sha256=CvMaWS6NJLVg-syICYt63igheQ0DcT-WYQjAMhAiJ3k,9155
 c7n_tencentcloud/resources/tag.py,sha256=3WiuN-y4Dm36Bk7i7CwLrVYPn3xh7a5K4gyCVBhpFC0,1399
 c7n_tencentcloud/resources/tcr.py,sha256=RKf13xKcEt9ZHiJGSKPaUzfda3h2bcVArEaq82IGMmg,3179
 c7n_tencentcloud/resources/vpc.py,sha256=TkPc6bYtK6m7wEj5qqRWoYUFDD8rL6zFRNLFJZcZDRo,3138
 c7n_tencentcloud/utils.py,sha256=6Nr5ZbebrexDRLCANUyN3mp8vO67d-hNkhsX5dN06QU,1252
-c7n_tencentcloud-0.1.6.dist-info/WHEEL,sha256=kLuE8m1WYU0Ig0_YEGrXyTtiJvKPpLpDEiChiNyei5Y,88
-c7n_tencentcloud-0.1.6.dist-info/RECORD,,
-c7n_tencentcloud-0.1.6.dist-info/METADATA,sha256=DqxBBuzrB4Ck8GWkFiCAadsmjNXYEVvkRQ9rK99kHwA,1629
+c7n_tencentcloud-0.1.7.dist-info/WHEEL,sha256=kLuE8m1WYU0Ig0_YEGrXyTtiJvKPpLpDEiChiNyei5Y,88
+c7n_tencentcloud-0.1.7.dist-info/RECORD,,
+c7n_tencentcloud-0.1.7.dist-info/METADATA,sha256=oAJa-0qDnEWu2NbLR5yKhEIQQDrE10ZKHN8IdqoiTUQ,4207
```

