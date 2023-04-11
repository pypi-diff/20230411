# Comparing `tmp/arcana_bids-0.2.2.tar.gz` & `tmp/arcana_bids-0.2.3.tar.gz`

## Comparing `arcana_bids-0.2.2.tar` & `arcana_bids-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/arcana/bids/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/arcana/bids/_version.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/arcana/bids/cli.py
--rw-r--r--   0        0        0    24652 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/arcana/bids/data.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/arcana/bids/deploy.py
--rw-r--r--   0        0        0    15208 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/arcana/bids/tasks.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/arcana/bids/tests/test_cli.py
--rw-r--r--   0        0        0     7489 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/arcana/bids/tests/test_data.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/arcana/bids/tests/test_tasks.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/LICENSE
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/README.rst
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    18568 2020-02-02 00:00:00.000000 arcana_bids-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/_version.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/cli.py
+-rw-r--r--   0        0        0    23234 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/data.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/deploy.py
+-rw-r--r--   0        0        0    15156 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/tasks.py
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/tests/test_cli.py
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/tests/test_data.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/tests/test_tasks.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/README.rst
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    18603 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/PKG-INFO
```

### Comparing `arcana_bids-0.2.2/arcana/bids/cli.py` & `arcana_bids-0.2.3/arcana/bids/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 def bids_group():
     pass
 
 
 @bids_group.command(
     name="app-entrypoint",
     help="""Loads a dataset, or creates one it is not already present, then applies and
-launches a pipeline in a single command. To be used within the command configuration
-of an XNAT Container Service ready Docker image.
+launches a pipeline in a single command. To be used inside BidsApp images.
 
 DATASET_LOCATOR string containing the nickname of the data store, the ID of the
 dataset (e.g. XNAT project ID or file-system directory) and the dataset's name
 in the format <store-nickname>//<dataset-id>[@<dataset-name>]
 
 """,
 )
```

### Comparing `arcana_bids-0.2.2/arcana/bids/data.py` & `arcana_bids-0.2.3/arcana/bids/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from __future__ import annotations
 import typing as ty
 import json
 import re
 import logging
 from operator import itemgetter
-from copy import copy
 import attrs
 import jq
 from pathlib import Path
 from arcana.core.data.store import LocalStore
 from fileformats.core import FileSet, Field
 from fileformats.generic import Directory
 from fileformats.medimage.nifti import WithBids
 from arcana.core.exceptions import ArcanaUsageError
 from arcana.core.data.tree import DataTree
 from arcana.core.data.set import Dataset
-from arcana.core.data.space import Clinical
+from arcana.stdlib import Clinical
 from arcana.core.data.entry import DataEntry
 from arcana.core.data.row import DataRow
 
 logger = logging.getLogger("arcana")
 
 
 @attrs.define
@@ -65,19 +64,27 @@
     json_edits: ty.List[JsonEdit] = attrs.field(
         factory=list, converter=JsonEdit.attr_converter
     )
 
     name: str = "bids"
 
     BIDS_VERSION = "1.0.1"
+    DEFAULT_SPACE = Clinical
 
     PROV_SUFFIX = ".provenance"
     FIELDS_FNAME = "__fields__"
     FIELDS_PROV_FNAME = "__fields_provenance__"
 
+    VALID_HIERARCHIES = (
+        ["subject", "timepoint"],
+        ["session"],
+        ["group", "subject", "timepoint"],
+        ["group", "session"],
+    )
+
     #################################
     # Abstract-method implementations
     #################################
 
     def populate_tree(self, tree: DataTree):
         """
         Find all rows within the dataset stored in the store and
@@ -85,40 +92,38 @@
 
         Parameters
         ----------
         dataset : Dataset
             The dataset to construct the tree dimensions for
         """
         root_dir = Path(tree.dataset.id)
-        participants_fspath = root_dir / "participants.tsv"
-        participants = {}
-        if participants_fspath.exists():
-            with open(participants_fspath) as f:
+        if "group" in tree.dataset.hierarchy:
+            with open(root_dir / "participants.tsv") as f:
                 lines = f.read().splitlines()
+            participants = {}
             if lines:
                 participant_keys = lines[0].split("\t")
                 for line in lines[1:]:
                     dct = dict(zip(participant_keys, line.split("\t")))
                     participants[dct.pop("participant_id")[len("sub-") :]] = dct
         for subject_dir in root_dir.iterdir():
             if not subject_dir.name.startswith("sub-"):
                 continue
             subject_id = subject_dir.name[len("sub-") :]
-            try:
-                additional_ids = {"group": participants[subject_id]["group"]}
-            except KeyError:
-                additional_ids = {}
+            if "group" in tree.dataset.hierarchy:
+                tree_path = [participants[subject_id]["group"]]
+            else:
+                tree_path = []
+            tree_path.append(subject_id)
             if any(d.name.startswith("ses-") for d in subject_dir.iterdir()):
                 for sess_dir in subject_dir.iterdir():
                     timepoint_id = sess_dir.name[len("ses-") :]
-                    sess_add_ids = copy(additional_ids)
-                    sess_add_ids["session"] = f"sub-{subject_id}_ses-{timepoint_id}"
-                    tree.add_leaf([subject_id, timepoint_id], additional_ids=sess_add_ids)
+                    tree.add_leaf(tree_path + [timepoint_id])
             else:
-                tree.add_leaf([subject_id], additional_ids=additional_ids)
+                tree.add_leaf([subject_id])
 
     def populate_row(self, row: DataRow):
         root_dir = row.dataset.root_dir
         relpath = self._rel_row_path(row)
         session_path = root_dir / relpath
         session_path.mkdir(exist_ok=True)
         for modality_dir in session_path.iterdir():
@@ -163,15 +168,15 @@
                             )
 
     def fileset_uri(self, path: str, datatype: type, row: DataRow) -> str:
         path, dataset_name = DataEntry.split_dataset_name_from_path(path)
         if dataset_name is None:
             base_uri = ""
         elif not dataset_name:
-            base_uri = f"derivatives/{Dataset.EMPTY_NAME}"
+            base_uri = f"derivatives/{self.EMPTY_DATASET_NAME}"
         else:
             base_uri = f"derivatives/{dataset_name}"
         return base_uri + str(
             self._entry2fs_path(
                 path,
                 subject_id=row.frequency_id("subject"),
                 timepoint_id=(
@@ -184,15 +189,15 @@
         )
 
     def field_uri(self, path: str, datatype: type, row: DataRow) -> str:
         path, dataset_name = DataEntry.split_dataset_name_from_path(path)
         if dataset_name is None:
             base_uri = ""
         elif not dataset_name:
-            base_uri = f"derivatives/{Dataset.EMPTY_NAME}"
+            base_uri = f"derivatives/{self.EMPTY_DATASET_NAME}"
         else:
             base_uri = f"derivatives/{dataset_name}"
         try:
             namespace, field_name = path.split("/")
         except ValueError:
             raise ArcanaUsageError(
                 f"Field path '{path}', should contain two sections delimted by '/', "
@@ -264,59 +269,57 @@
         self.update_json(fspath, key, provenance)
 
     def create_data_tree(
         self,
         id: str,
         leaves: list[tuple[str, ...]],
         hierarchy: list[str],
-        id_composition: dict[str, str] = None,
         **kwargs
     ):
+        if hierarchy not in self.VALID_HIERARCHIES:
+            raise ArcanaUsageError(
+                f"Invalid hiearchy {hierarchy} provided to create a new data tree "
+                f"needs to be one of the following:\n"
+                + "\n".join(str(h) for h in self.VALID_HIERARCHIES)
+            )
         root_dir = Path(id)
         root_dir.mkdir(parents=True)
         # Create sub-directories corresponding to rows of the dataset
         group_ids = set()
-        subject_group_ids = {}
+        subjects_group_id = {}
         for ids_tuple in leaves:
             ids = dict(zip(hierarchy, ids_tuple))
             # Add in composed IDs
-            ids.update(Dataset.decompose_ids(ids, id_composition))
-            if "session" in hierarchy:
-                subject_id = ids["session"]
-                timepoint_id = None
-                assert "subject" not in ids
-                assert "timepoint" not in ids
-            else:
+            try:
                 subject_id = ids["subject"]
-                timepoint_id = ids["timepoint"]
-                assert "session" not in ids
+            except KeyError:
+                subject_id = ids["session"]
+            timepoint_id = ids.get("timepoint")
             group_id = ids.get("group")
             if group_id:
                 group_ids.add(group_id)
-                subject_group_ids[subject_id] = group_id
+                subjects_group_id[subject_id] = group_id
             sess_dir_fspath = root_dir / self._entry2fs_path(
                 entry_path=None, subject_id=subject_id, timepoint_id=timepoint_id
             )
-            sess_dir_fspath.mkdir(parents=True)
+            sess_dir_fspath.mkdir(parents=True, exist_ok=True)
         # Add participants.tsv to define the groups if present
         if group_ids:
             with open(root_dir / "participants.tsv", "w") as f:
                 f.write("participant_id\tgroup\n")
-                for subject_id, group_id in subject_group_ids.items():
+                for subject_id, group_id in subjects_group_id.items():
                     f.write(f"sub-{subject_id}\t{group_id}\n")
 
     ####################
     # Overrides of API #
     ####################
 
-    def save_dataset(
-        self, dataset: Dataset, name: str = None, overwrite_bids_metadata: bool = False
-    ):
+    def save_dataset(self, dataset: Dataset, name: str = None):
         super().save_dataset(dataset, name=name)
-        self._save_metadata(dataset, overwrite_bids_metadata=overwrite_bids_metadata)
+        self._save_metadata(dataset)
 
     def create_dataset(
         self,
         id: str,
         leaves: list[tuple[str, ...]],
         hierarchy: list[str] = ["session"],
         space: type = Clinical,
@@ -343,89 +346,65 @@
         -------
         Dataset
             the newly created dataset
         """
         dataset = super().create_dataset(
             id=id, leaves=leaves, hierarchy=hierarchy, space=space, name=name, **kwargs
         )
-        self._save_metadata(dataset, overwrite_bids_metadata=True)
+        self._save_metadata(dataset)
         return dataset
 
     ################
     # Helper methods
     ################
 
-    def _save_metadata(self, dataset: Dataset, overwrite_bids_metadata: bool = False):
+    def _save_metadata(self, dataset: Dataset):
         root_dir = Path(dataset.id)
         dataset_description_fspath = root_dir / "dataset_description.json"
-        if dataset_description_fspath.exists() and not overwrite_bids_metadata:
-            logger.warning(
-                "Not attempting to overwrite existing BIDS dataset description at "
-                "'%s, use 'overwrite_bids_metadata' to "
-                "force.",
-                str(dataset_description_fspath),
-            )
-        else:
-            dataset_description = map_to_bids_names(
-                attrs.asdict(dataset.metadata, recurse=True)
-            )
-            dataset_description["BIDSVersion"] = self.BIDS_VERSION
-            with open(dataset_description_fspath, "w") as f:
-                json.dump(dataset_description, f, indent="    ")
+        dataset_description = map_to_bids_names(
+            attrs.asdict(dataset.metadata, recurse=True)
+        )
+        dataset_description["BIDSVersion"] = self.BIDS_VERSION
+        with open(dataset_description_fspath, "w") as f:
+            json.dump(dataset_description, f, indent="    ")
 
         if dataset.metadata.description is not None:
             readme_path = root_dir / "README"
-            if readme_path.exists() and not overwrite_bids_metadata:
-                logger.warning(
-                    "Not attempting to overwrite existing BIDS dataset description at "
-                    "%s, use 'overwrite_bids_metadata' to "
-                    "force.",
-                    str(readme_path),
-                )
-            else:
-                with open(readme_path, "w") as f:
-                    f.write(dataset.metadata.description)
-        participants_tsv_fspath = dataset.root_dir / "participants.tsv"
+            with open(readme_path, "w") as f:
+                f.write(dataset.metadata.description)
         columns = list(dataset.metadata.row_metadata)
         group_ids = [i for i in dataset.row_ids("group") if i is not None]
         if group_ids or columns:
-            if participants_tsv_fspath.exists() and not overwrite_bids_metadata:
-                logger.warning(
-                    "Not attempting to overwrite existing BIDS participants TSV at "
-                    "%s, use 'overwrite_bids_metadata' to "
-                    "force.",
-                    str(participants_tsv_fspath),
-                )
-            else:
-                with open(dataset.root_dir / "participants.tsv", "w") as f:
-                    f.write("participant_id")
+            subject_rows = dataset.rows("subject")
+            with open(dataset.root_dir / "participants.tsv", "w") as f:
+                f.write("participant_id")
+                if group_ids:
+                    f.write("\tgroup")
+                if columns:
+                    f.write("\t" + "\t".join(columns))
+                f.write("\n")
+                for row in subject_rows:
+                    f.write(
+                        f"sub-{row.id}"
+                    )
                     if group_ids:
-                        f.write("\tgroup")
+                        f.write("\t" + row.frequency_id('group'))
                     if columns:
-                        f.write("\t" + "\t".join(columns))
+                        f.write("\t" + "\t".join(row.metadata[k] for k in columns))
                     f.write("\n")
-                    for row in dataset.rows("subject"):
-                        f.write(
-                            f"sub-{row.id}"
-                        )
-                        if group_ids:
-                            f.write("\t" + row.frequency_id('group'))
-                        if columns:
-                            f.write("\t" + "\t".join(row.metadata[k] for k in columns))
-                        f.write("\n")
-                participants_desc = {}
-                if group_ids:
-                    participants_desc["group"] = {
-                        "Description": "the group the participant belonged to",
-                        "Levels": {g: f"{g} group" for g in dataset.row_ids("group")},
-                    }
-                for name, desc in dataset.metadata.row_metadata.items():
-                    participants_desc[name] = {"Description": desc}
-                with open(dataset.root_dir / "participants.json", "w") as f:
-                    json.dump(participants_desc, f)
+            participants_desc = {}
+            if group_ids:
+                participants_desc["group"] = {
+                    "Description": "the group the participant belonged to",
+                    "Levels": {g: f"{g} group" for g in dataset.row_ids("group")},
+                }
+            for name, desc in dataset.metadata.row_metadata.items():
+                participants_desc[name] = {"Description": desc}
+            with open(dataset.root_dir / "participants.json", "w") as f:
+                json.dump(participants_desc, f)
 
     def _fileset_fspath(self, entry: DataEntry) -> Path:
         return Path(entry.row.dataset.id) / entry.uri
 
     def _fields_fspath_and_key(self, entry: DataEntry) -> tuple[Path, str]:
         relpath, key = entry.uri.split("::")
         fspath = Path(entry.row.dataset.id) / relpath
```

### Comparing `arcana_bids-0.2.2/arcana/bids/tasks.py` & `arcana_bids-0.2.3/arcana/bids/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     DockerSpec,
     SingularitySpec,
     ShellOutSpec,
 )
 from arcana.core import __version__
 from arcana.core.data.set import Dataset
 from fileformats.core import FileSet
-from arcana.core.data.space import Clinical
+from arcana.stdlib import Clinical
 from arcana.bids.data import JsonEdit
 from arcana.core.exceptions import ArcanaUsageError
 from arcana.core.utils.serialize import (
     ClassResolver,
     ObjectListConverter,
 )
 from arcana.core.utils.misc import func_task
@@ -78,16 +78,15 @@
         The inputs to be inserted into the BIDS dataset. Should be a list of tuples
         consisting of the the path the file/directory should be stored within a BIDS subject/session,
         e.g. anat/T1w, func/bold, and the DataFormat class it should be stored in, e.g.
         arcana.bids.data.NiftiGzX.
     outputs : list[ty.Union[AppField, dict[str, str]]]
         The outputs to be extracted from the derivatives directory. Should be a list of tuples
         consisting of the the path the file/directory is saved by the app within a BIDS subject/session,
-        e.g. freesurfer/recon-all, and the DataFormat class it is stored in, e.g.
-        arcana.dirtree.data.Directory.
+        e.g. freesurfer/recon-all, and the DataFormat class it is stored in, 
     executable : str, optional
         Name of the executable within the image to run (i.e. the entrypoint of the image).
         Required when extending the base image and launching Arcana within it. Defaults to
         empty string, i.e. the entrypoint of the BIDS app container image
     container_image : str, optional
         Name of the BIDS app image to wrap
     parameters : dict[str, type], optional
```

### Comparing `arcana_bids-0.2.2/arcana/bids/tests/test_cli.py` & `arcana_bids-0.2.3/arcana/bids/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import reduce
 from operator import mul
 import pytest
 from fileformats.text import Plain as Text
 from arcana.testing.data.blueprint import (
     TestDatasetBlueprint, FileSetEntryBlueprint as FileBP
 )
-from arcana.core.data.space import Clinical
+from arcana.stdlib import Clinical
 from fileformats.medimage import NiftiGzX
 from arcana.bids.cli import app_entrypoint
 from arcana.core.utils.serialize import ClassResolver
 from arcana.core.utils.misc import path2varname
 from arcana.core.utils.misc import show_cli_trace
 from arcana.core.deploy import App
 from arcana.bids.data import Bids
```

### Comparing `arcana_bids-0.2.2/arcana/bids/tests/test_data.py` & `arcana_bids-0.2.3/arcana/bids/tests/test_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,53 +8,56 @@
 import numpy.random
 import shutil
 from dataclasses import dataclass
 import pytest
 import docker
 from fileformats.medimage import NiftiX
 from arcana.core import __version__
-from arcana.core.data.space import Clinical
+from arcana.stdlib import Clinical
 from arcana.bids.data import Bids
 
 
 MOCK_BIDS_APP_NAME = "mockapp"
 MOCK_README = "A dummy readme\n" * 100
 MOCK_AUTHORS = ["Dumm Y. Author", "Another D. Author"]
 
 
 def test_bids_roundtrip(bids_validator_docker, bids_success_str, work_dir):
 
     path = work_dir / "bids-dataset"
     dataset_name = "adataset"
 
     shutil.rmtree(path, ignore_errors=True)
-    group_ids = ["test", "control"]
-    member_ids = [str(i) for i in range(1, 4)]
-    subject_ids = ["{}{}".format(*t) for t in itertools.product(group_ids, member_ids)]
-    timepoint_ids = [str(i) for i in range(1, 3)]
     dataset = Bids().create_dataset(
         id=path,
         name=dataset_name,
         space=Clinical,
-        hierarchy=["subject", "timepoint"],
-        leaves=itertools.product(subject_ids, timepoint_ids),
-        id_composition={
-            "subject": r"(?P<group>\w+)(?P<member>\d+)"
+        hierarchy=["group", "subject", "timepoint"],
+        leaves=[
+            (group, f"{group}{member}", timepoint)
+            for group, member, timepoint in itertools.product(
+                ["test", "control"],
+                [str(i) for i in range(1, 4)],
+                [str(i) for i in range(1, 3)],
+            )
+        ],
+        id_patterns={
+            "member": r"subject::\w+(\d+)",
         },
         metadata={
             "description": MOCK_README,
             "authors": MOCK_AUTHORS,
             "generated_by": [
                 {
                     "name": "arcana",
                     "version": __version__,
                     "description": "Dataset was created programmatically from scratch",
                     "code_url": "http://arcana.readthedocs.io",
                 }
-            ]
+            ],
         },
     )
 
     dataset.add_sink("t1w", datatype=NiftiX, path="anat/T1w")
 
     dummy_nifti = work_dir / "t1w.nii"
     # dummy_nifti_gz = dummy_nifti + '.gz'
@@ -93,15 +96,17 @@
         volumes=[f"{path}:/data:ro"],
         remove=True,
         stderr=True,
     ).decode("utf-8")
     assert bids_success_str in result
 
     reloaded = Bids().load_dataset(id=path, name=dataset_name)
-    reloaded.add_sink("t1w", datatype=NiftiX, path="anat/T1w")  # add sink to reloaded so it matches
+    reloaded.add_sink(
+        "t1w", datatype=NiftiX, path="anat/T1w"
+    )  # add sink to reloaded so it matches
     reloaded.name = ""  # remove saved name so it matches
 
     assert dataset == reloaded
 
 
 @dataclass
 class SourceNiftiXBlueprint:
@@ -181,33 +186,30 @@
 
     bp = json_edit_blueprint  # shorten name
 
     path = work_dir / "bids-dataset"
     name = "bids-dataset"
 
     shutil.rmtree(path, ignore_errors=True)
-    dataset = Bids(
-        json_edits=[(bp.path_re, bp.jq_script)],
-    ).create_dataset(
+    dataset = Bids(json_edits=[(bp.path_re, bp.jq_script)],).create_dataset(
         id=path,
         name=name,
         leaves=[("1",)],
         metadata={
             "description": MOCK_README,
             "authors": MOCK_AUTHORS,
             "generated_by": [
                 {
                     "name": "arcana",
                     "version": __version__,
                     "description": "Dataset was created programmatically from scratch",
                     "code_url": "http://arcana.readthedocs.io",
                 }
-            ]
+            ],
         },
-        
     )
 
     for sf_name, sf_bp in bp.source_niftis.items():
         dataset.add_sink(sf_name, datatype=NiftiX, path=sf_bp.path)
 
         nifti_fspath = work_dir / (sf_name + ".nii")
         # dummy_nifti_gz = dummy_nifti + '.gz'
```

### Comparing `arcana_bids-0.2.2/arcana/bids/tests/test_tasks.py` & `arcana_bids-0.2.3/arcana/bids/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.2/LICENSE` & `arcana_bids-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.2/README.rst` & `arcana_bids-0.2.3/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 .. image:: https://codecov.io/gh/arcanaframework/arcana-bids/branch/main/graph/badge.svg?token=UIS0OGPST7
    :target: https://codecov.io/gh/arcanaframework/arcana-bids
 .. image:: https://img.shields.io/pypi/pyversions/arcana-bids.svg
    :target: https://pypi.python.org/pypi/arcana-bids/
    :alt: Python versions
 .. image:: https://img.shields.io/pypi/v/arcana-bids.svg
    :target: https://pypi.python.org/pypi/arcana-bids/
-   :alt: Latest Version  
-.. image:: https://github.com/ArcanaFramework/arcana/actions/workflows/docs.yml/badge.svg
-   :target: http://arcana.readthedocs.io/en/latest/?badge=latest
-   :alt: Docs
+   :alt: Latest Version
+.. image:: https://readthedocs.org/projects/arcana/badge/?version=latest
+  :target: https://arcanaframework.github.io/arcana
+  :alt: Documentation Status
 
 
 An extension of the Arcana framework to work with Brain Imaging Data Structure (BIDS)
 datasets and apps
 
 
 Quick Installation
```

### Comparing `arcana_bids-0.2.2/pyproject.toml` & `arcana_bids-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     "packaging",
     "sphinx >=2.1.2",
     "sphinx-argparse>=0.2.0",
     "sphinx-click>=3.1",
 ]
 test = [
     "codecov",
+    "fileformats-testing",
     "medimages4tests >=0.3",
     "pytest>=5.4.3",
     "pytest-cov>=2.12.1",
     "pytest-env>=0.6.2",
 ]
 
 [project.urls]
```

### Comparing `arcana_bids-0.2.2/PKG-INFO` & `arcana_bids-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcana-bids
-Version: 0.2.2
+Version: 0.2.3
 Summary: An Arcana extension for interacting with Brain Imaging Structure (BIDS) datasets and associated "Apps"
 Project-URL: documentation, https://arcana.readthedocs.io
 Project-URL: repository, https://github.com/ArcanaFramework/arcana-bids.git
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
@@ -128,14 +128,15 @@
 Requires-Dist: numpydoc>=0.6.0; extra == 'doc'
 Requires-Dist: packaging; extra == 'doc'
 Requires-Dist: sphinx-argparse>=0.2.0; extra == 'doc'
 Requires-Dist: sphinx-click>=3.1; extra == 'doc'
 Requires-Dist: sphinx>=2.1.2; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: codecov; extra == 'test'
+Requires-Dist: fileformats-testing; extra == 'test'
 Requires-Dist: medimages4tests>=0.3; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=5.4.3; extra == 'test'
 Description-Content-Type: text/x-rst
 
 Arcana Extension - bids
@@ -145,18 +146,18 @@
 .. image:: https://codecov.io/gh/arcanaframework/arcana-bids/branch/main/graph/badge.svg?token=UIS0OGPST7
    :target: https://codecov.io/gh/arcanaframework/arcana-bids
 .. image:: https://img.shields.io/pypi/pyversions/arcana-bids.svg
    :target: https://pypi.python.org/pypi/arcana-bids/
    :alt: Python versions
 .. image:: https://img.shields.io/pypi/v/arcana-bids.svg
    :target: https://pypi.python.org/pypi/arcana-bids/
-   :alt: Latest Version  
-.. image:: https://github.com/ArcanaFramework/arcana/actions/workflows/docs.yml/badge.svg
-   :target: http://arcana.readthedocs.io/en/latest/?badge=latest
-   :alt: Docs
+   :alt: Latest Version
+.. image:: https://readthedocs.org/projects/arcana/badge/?version=latest
+  :target: https://arcanaframework.github.io/arcana
+  :alt: Documentation Status
 
 
 An extension of the Arcana framework to work with Brain Imaging Data Structure (BIDS)
 datasets and apps
 
 
 Quick Installation
```

