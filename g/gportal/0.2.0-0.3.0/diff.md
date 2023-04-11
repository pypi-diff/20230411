# Comparing `tmp/gportal-0.2.0.tar.gz` & `tmp/gportal-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gportal-0.2.0.tar", max compression
+gzip compressed data, was "gportal-0.3.0.tar", max compression
```

## Comparing `gportal-0.2.0.tar` & `gportal-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-03-31 12:36:39.949408 gportal-0.2.0/LICENSE
--rw-r--r--   0        0        0     1937 2023-03-31 12:36:39.949408 gportal-0.2.0/README.md
--rw-r--r--   0        0        0      286 2023-03-31 12:36:39.949408 gportal-0.2.0/gportal/__init__.py
--rw-r--r--   0        0        0    28946 2023-03-31 12:36:39.949408 gportal-0.2.0/gportal/data/datasets.json
--rw-r--r--   0        0        0     1712 2023-03-31 12:36:39.949408 gportal-0.2.0/gportal/dataset.py
--rw-r--r--   0        0        0      422 2023-03-31 12:36:39.949408 gportal-0.2.0/gportal/http_client.py
--rw-r--r--   0        0        0     4416 2023-03-31 12:36:39.949408 gportal-0.2.0/gportal/product.py
--rw-r--r--   0        0        0     4014 2023-03-31 12:36:39.949408 gportal-0.2.0/gportal/search.py
--rw-r--r--   0        0        0     4343 2023-03-31 12:36:39.949408 gportal-0.2.0/gportal/sftp.py
--rw-r--r--   0        0        0     1380 2023-03-31 12:36:39.953408 gportal-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 gportal-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-11 12:05:29.006972 gportal-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1937 2023-04-11 12:05:29.006972 gportal-0.3.0/README.md
+-rw-r--r--   0        0        0      286 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/__init__.py
+-rw-r--r--   0        0        0    28946 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/data/datasets.json
+-rw-r--r--   0        0        0     1663 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/dataset.py
+-rw-r--r--   0        0        0      422 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/http_client.py
+-rw-r--r--   0        0        0     5257 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/product.py
+-rw-r--r--   0        0        0     4192 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/search.py
+-rw-r--r--   0        0        0     4894 2023-04-11 12:05:29.042973 gportal-0.3.0/gportal/sftp.py
+-rw-r--r--   0        0        0     1357 2023-04-11 12:05:29.042973 gportal-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2721 1970-01-01 00:00:00.000000 gportal-0.3.0/PKG-INFO
```

### Comparing `gportal-0.2.0/LICENSE` & `gportal-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gportal-0.2.0/README.md` & `gportal-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gportal-0.2.0/gportal/data/datasets.json` & `gportal-0.3.0/gportal/data/datasets.json`

 * *Files identical despite different names*

### Comparing `gportal-0.2.0/gportal/dataset.py` & `gportal-0.3.0/gportal/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,34 +18,34 @@
     Note:
         This depends on an undocumented API of G-Portal, which is subject to change.
         If this function is broken, use [`cached_datasets()`][gportal.dataset.cached_datasets] instead.
 
     Returns:
         The dictionary of the dataset tree, where the leaves are dataset IDs.
     """
+    raw_tree = http_client.get("/gpr/search/service/satsensor.json")
+    return _build_datasets(raw_tree)
 
-    def build_datasets(tree: list[dict[str, Any]], root: bool = True) -> dict[str, Any]:
-        datasets = {}
 
-        for node in tree:
-            if root:
-                title = re.sub(r"<img[^>]*>", "", node["title"]).rstrip()
-            else:
-                title = node["title"]
-
-            children = node.get("children")
-            if children:
-                datasets[title] = build_datasets(children, root=False)
-            else:
-                datasets[title] = node["dataset"].split(",")
+def _build_datasets(tree: list[dict[str, Any]], root: bool = True) -> dict[str, Any]:
+    datasets = {}
 
-        return datasets
+    for node in tree:
+        if root:
+            title = re.sub(r"<img[^>]*>", "", node["title"]).rstrip()
+        else:
+            title = node["title"]
 
-    raw_tree = http_client.get("/gpr/search/service/satsensor.json")
-    return build_datasets(raw_tree)
+        children = node.get("children")
+        if children:
+            datasets[title] = _build_datasets(children, root=False)
+        else:
+            datasets[title] = node["dataset"].split(",")
+
+    return datasets
 
 
 @cache
 def cached_datasets() -> Datasets:
     """Loads the dataset tree from the cache included in this package.
 
     Returns:
```

### Comparing `gportal-0.2.0/gportal/product.py` & `gportal-0.3.0/gportal/product.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,139 +1,168 @@
-import re
+import sys
 from datetime import datetime
 from typing import Any, Optional
 
 
 class Product:
     """Wrapper of a product GeoJSON in search results.
 
-    Attributes:
-        geojson: Original dictionary that represents GeoJSON Feature.
+    You can access the `properties` or `properties.gpp` values by `[]` operator like a dictionary.
     """
 
-    def __init__(self, geojson: dict[str, Any]):
-        self.geojson: dict[str, Any] = geojson
+    VALUE_CONVERSION_MAP = {
+        "": None,
+        "true": True,
+        "false": False,
+    }
+
+    def __init__(self, geojson: dict[str, Any], convert_types: bool = False):
+        if convert_types and "properties" in geojson:
+            geojson = {**geojson, "properties": self._convert_type(geojson["properties"])}
+
+        self._geojson = geojson
+
+    @classmethod
+    def _convert_type(cls, val: Any) -> Any:
+        if isinstance(val, str):
+            if val in cls.VALUE_CONVERSION_MAP:
+                return cls.VALUE_CONVERSION_MAP[val]
+            try:
+                return int(val)
+            except ValueError:
+                pass
+            try:
+                return float(val)
+            except ValueError:
+                pass
+        elif isinstance(val, dict):
+            return {key: cls._convert_type(val) for key, val in val.items()}
+
+        return val
 
     def __repr__(self) -> str:
         if self.id is None:
             return super().__repr__()
         else:
             return f"<gportal.Product id={self.id}>"
 
     @property
     def __geo_interface__(self) -> dict[str, Any]:
-        return self.geojson
+        return self._geojson
 
     @property
     def geometry(self) -> dict[str, Any]:
         """GeoJSON geometry."""
-        return self.geojson.get("geometry", {})
+        return self._geojson.get("geometry", {})
 
     @property
     def properties(self) -> dict[str, Any]:
         """GeoJSON properties."""
-        return self.geojson.get("properties", {})
+        return self._geojson.get("properties", {})
+
+    def __getitem__(self, key: str) -> Any:
+        if key in self.properties:
+            return self.properties[key]
+
+        if key in self.properties.get("gpp", {}):
+            return self.properties["gpp"][key]
+
+        raise KeyError(key)
+
+    def get(self, key: str, default: Any = None) -> Any:
+        try:
+            return self[key]
+        except KeyError:
+            return default
 
     @property
     def id(self) -> Optional[str]:
         """Granule ID."""
-        return self.properties.get("identifier")
-
-    @property
-    def dataset_id(self) -> Optional[str]:
-        """Dataset ID belonging to."""
-        return self.properties.get("gpp", {}).get("datasetId")
-
-    @property
-    def start_time(self) -> datetime:
-        """Observation start time."""
-        isoformat = re.sub(r"Z$", "+00:00", self.properties["beginPosition"])  # For Python 3.10 or former
-        return datetime.fromisoformat(isoformat)
-
-    @property
-    def end_time(self) -> datetime:
-        """Observation end time."""
-        isoformat = re.sub(r"Z$", "+00:00", self.properties["endPosition"])  # For Python 3.10 or former
-        return datetime.fromisoformat(isoformat)
+        return self.get("identifier")
 
     @property
     def data_url(self) -> Optional[str]:
         """URL of the product file."""
-        return self.properties.get("product", {}).get("fileName")
+        return self.get("product", {}).get("fileName")
 
     @property
     def data_path(self) -> Optional[str]:
         """Path to the product file on the SFTP server."""
         if self.data_url is None:
             return None
 
         return self.data_url.replace("https://gportal.jaxa.jp/download/", "", 1)
 
-    def get_browse_url(self, type: str = "browse") -> Optional[str]:
-        """URL of the browse image.
+    @property
+    def quicklook_url(self) -> Optional[str]:
+        """Quicklook image URL."""
+        for item in self.get("browse", []):
+            if item.get("type", "").lower() == "quicklook":
+                return item.get("fileName")
 
-        Args:
-            type: Type of the image. Basically, "browse", "sub-browse" or "thumbnail".
-        """
-        items = self.properties.get("browse")
-        if items is None:
+        return None
+
+    def get_as_datetime(self, key: str) -> Optional[datetime]:
+        """Gets a value as a datetime object."""
+        val = self.get(key)
+        if val is None:
             return None
 
-        type = {
-            "thumbnail": "thm",
-            "browse": "br",
-            "sub-browse": "sb",
-        }.get(type, type)
-
-        for item in items:
-            if f"/img/{type}" in item["fileName"]:
-                return item["fileName"]
+        if sys.version_info < (3, 11):
+            val = val.replace("Z", "+00:00")
 
-        return None
+        return datetime.fromisoformat(val)
 
     def flatten_properties(self) -> dict[str, Any]:
         """Flattens the nested properties.
 
         This method processes nested properties from the following keys:
 
         - `product`: Each key is prefixed with `product` (e.g. `product.fileName` => `productFileName`).
-        - `browse`: Keys are the image type (e.g. browse-br, browse-thm), and their values are `fileName`.
+        - `browse`: Keys are the `type` fields (e.g. quicklook, thumbnail), and their values are `fileName` fields.
         - `gpp`: Keys and values are directly merged.
 
         Returns:
             The flattened properties.
         """
         properties = self.properties.copy()
 
         if "product" in properties and isinstance(properties["product"], dict):
             for key, value in properties["product"].items():
                 properties[f"product{key[0].upper()}{key[1:]}"] = value
 
             del properties["product"]
 
         if "browse" in properties and isinstance(properties["browse"], list):
-            for browse in properties["browse"]:
-                match = re.search(r"\/img\/([\w]+)\/", browse.get("fileName", ""))
-                if match:
-                    properties[f"browse-{match.group(1)}"] = browse["fileName"]
+            for i, browse in enumerate(properties["browse"]):
+                if "type" in browse and "fileName" in browse:
+                    type = browse["type"].lower()
+                    if type in properties:
+                        properties[f"{type}{i}"] = browse["fileName"]
+                    else:
+                        properties[type] = browse["fileName"]
 
             del properties["browse"]
 
         if "gpp" in properties and isinstance(properties["gpp"], dict):
             properties.update(properties["gpp"])
             del properties["gpp"]
 
         return properties
 
-    def to_dict(self) -> dict[str, Any]:
-        return self.geojson
+    def to_dict(self, flatten_properties: bool = False) -> dict[str, Any]:
+        """Converts to a dictionary of GeoJSON Feature.
 
-    def to_flat_properties_dict(self) -> dict[str, Any]:
-        """Converts to a dictionary of GeoJSON Feature with flattened properties.
+        Args:
+            flatten_properties: If True, the properties are flattened using
+                [`flatten_properties`][gportal.product.Product.flatten_properties].
 
         Returns:
-            A dictionary of GeoJSON Feature with flattened properties.
+            This product as a dictionary.
         """
-        return {
-            **self.geojson,
-            "properties": self.flatten_properties(),
-        }
+        if flatten_properties:
+            return {
+                **self._geojson,
+                "properties": self.flatten_properties(),
+            }
+        else:
+            return self._geojson
```

### Comparing `gportal-0.2.0/gportal/search.py` & `gportal-0.3.0/gportal/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,23 +82,26 @@
 
         Returns:
             The number of products matched the query.
         """
         response = self._request({"count": 0})
         return response.get("properties", {}).get("numberOfRecordsMatched")
 
-    def products(self) -> Iterator[Product]:
+    def products(self, convert_types: bool = True) -> Iterator[Product]:
         """Yields products matched the query.
 
+        Args:
+            convert_types: Whether to convert string values in properties into int, float, bool, or None.
+
         Yields:
             A [Product][gportal.product.Product] instance.
         """
         for page in self.pages():
             for product_dict in page.get("features", []):
-                yield Product(product_dict)
+                yield Product(product_dict, convert_types=convert_types)
 
     def pages(self) -> Iterator[dict[str, Any]]:
         """Iterates a search request with pagination.
 
         Yields:
             A dictionary of GeoJSON FeatureCollection.
         """
```

### Comparing `gportal-0.2.0/gportal/sftp.py` & `gportal-0.3.0/gportal/sftp.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,25 +12,28 @@
 
 
 def download(
     target: Union[str, Product, Iterable[Union[str, Product]]],
     local_dir: str = ".",
     username: Optional[str] = None,
     password: Optional[str] = None,
-) -> None:
+) -> list[str]:
     """Downloads files to a local directory via SFTP.
 
     Args:
         target: Remote path, Product object, or a list of them.
         local_dir: Local directory to download to.
         username: G-Portal username. If not provided, the value of `gportal.username` is used.
         password: G-Portal password. If not provided, the value of `gportal.password` is used.
+
+    Returns:
+        A list of local paths of the downloaded files.
     """
     with SFTP.connect(username, password) as sftp:
-        sftp.download(target, local_dir)
+        return sftp.download(target, local_dir)
 
 
 class SFTP:
     """Wrapper of the G-Portal SFTP interface.
 
     Attributes:
         client: An instance of [`paramiko.SFTPClient`][paramiko.sftp_client.SFTPClient].
@@ -98,35 +101,43 @@
             entries = [entry for entry in entries if re.search(filter_pattern, entry)]
 
         if fullpath:
             return [os.path.join(path, entry) for entry in entries]
         else:
             return entries
 
-    def download(self, target: Union[str, Product, Iterable[Union[str, Product]]], local_dir: str) -> None:
+    def download(
+        self, target: Union[str, Product, Iterable[Union[str, Product]]], local_dir: str
+    ) -> Union[str, list[str]]:
         """Downloads files to a local directory.
 
         Args:
             target: Remote path, Product object, or a list of them.
             local_dir: Local directory to download to.
 
+        Returns:
+            If `target` is a single path or Product object, returns the local path of the downloaded file.
+            If `target` is a list of paths or Product objects, returns a list of local paths of the downloaded files.
+
         Raises:
             ValueError: If the given product has no URL to download.
         """
         self._reset_cwd()
 
-        if isinstance(target, Iterable):
-            targets = target
+        if isinstance(target, Iterable) and not isinstance(target, str):
+            return [self._download_single(t, local_dir) for t in target]
         else:
-            targets = [target]
-
-        for target in targets:
-            if isinstance(target, Product):
-                if target.data_path is None:
-                    raise ValueError(f"Product {target.id} has no URL to download")
-
-                target = target.data_path
+            return self._download_single(target, local_dir)
 
-            self.client.get(target, os.path.join(local_dir, os.path.basename(target)))
+    def _download_single(self, target: Union[str, Product], local_dir: str) -> str:
+        if isinstance(target, Product):
+            if target.data_path is None:
+                raise ValueError(f"Product {target.id} has no URL to download")
+
+            target = target.data_path
+
+        local_path = os.path.join(local_dir, os.path.basename(target))
+        self.client.get(target, local_path)
+        return local_path
 
     def _reset_cwd(self) -> None:
         self.client.chdir()
```

### Comparing `gportal-0.2.0/pyproject.toml` & `gportal-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+[project]
+requires-python = ">=3.9"
+
 [tool.poetry]
 name = "gportal"
-version = "0.2.0"
+version = "0.3.0"
 description = "Client for JAXA G-Portal Catalogue Service and SFTP"
 authors = ["Takahiro Miyoshi <takahiro-miyoshi@sankichi.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sankichi92/gportal-python"
 documentation = "https://gportal.readthedocs.io/"
 packages = [{include = "gportal"}]
@@ -12,22 +15,21 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.2"
 paramiko = "^3.1.0"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "^23.1.0"}
-isort = "^5.12.0"
-flake8 = "^6.0.0"
-pytest = "^7.2.2"
-responses = "^0.23.1"
+ruff = "^0.0.260"
 mypy = "^1.1.1"
 types-requests = "^2.28.11.16"
 types-paramiko = "^3.0.0.4"
+pytest = "^7.2.2"
 pytest-mock = "^3.10.0"
+responses = "^0.23.1"
 
 [tool.poetry.group.notebook.dependencies]
 notebook = "^6.5.3"
 geopandas = "^0.12.2"
 matplotlib = "^3.7.1"
 folium = "^0.14.0"
 mapclassify = "^2.5.0"
@@ -41,20 +43,18 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 
-[tool.isort]
-profile = "black"
-line_length = 120
+[tool.ruff]
+line-length = 120
 
 [tool.mypy]
-python_version = "3.9"
 strict = true
 warn_return_any = false
 
 [[tool.mypy.overrides]]
 module = "tests.*"
 allow_untyped_defs = true
 disable_error_code = ["call-overload"]
```

### Comparing `gportal-0.2.0/PKG-INFO` & `gportal-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gportal
-Version: 0.2.0
+Version: 0.3.0
 Summary: Client for JAXA G-Portal Catalogue Service and SFTP
 Home-page: https://github.com/sankichi92/gportal-python
 License: MIT
 Author: Takahiro Miyoshi
 Author-email: takahiro-miyoshi@sankichi.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

