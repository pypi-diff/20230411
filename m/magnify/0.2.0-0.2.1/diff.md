# Comparing `tmp/magnify-0.2.0.tar.gz` & `tmp/magnify-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnify-0.2.0.tar", max compression
+gzip compressed data, was "magnify-0.2.1.tar", max compression
```

## Comparing `magnify-0.2.0.tar` & `magnify-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.2.0/README.md
--rw-r--r--   0        0        0     1601 2023-04-07 23:32:37.299062 magnify-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      200 2023-04-07 23:32:44.975245 magnify-0.2.0/src/magnify/__init__.py
--rw-r--r--   0        0        0    24452 2023-04-07 23:31:26.665378 magnify-0.2.0/src/magnify/find.py
--rw-r--r--   0        0        0     1406 2023-04-07 22:21:05.340362 magnify-0.2.0/src/magnify/pipeline.py
--rw-r--r--   0        0        0      158 2023-04-07 22:03:32.255470 magnify-0.2.0/src/magnify/postprocess.py
--rw-r--r--   0        0        0     1467 2023-04-07 21:54:53.107240 magnify-0.2.0/src/magnify/preprocess.py
--rw-r--r--   0        0        0    12742 2023-04-07 23:14:57.561770 magnify-0.2.0/src/magnify/reader.py
--rw-r--r--   0        0        0     3084 2023-04-07 23:19:37.400458 magnify-0.2.0/src/magnify/registry.py
--rw-r--r--   0        0        0     1121 2023-04-07 21:54:06.746151 magnify-0.2.0/src/magnify/stitch.py
--rw-r--r--   0        0        0     1583 2023-03-28 01:44:15.928665 magnify-0.2.0/src/magnify/utils.py
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 magnify-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.2.1/README.md
+-rw-r--r--   0        0        0     1601 2023-04-11 21:33:19.187520 magnify-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      200 2023-04-11 21:33:12.099352 magnify-0.2.1/src/magnify/__init__.py
+-rw-r--r--   0        0        0    24766 2023-04-11 21:20:33.945339 magnify-0.2.1/src/magnify/find.py
+-rw-r--r--   0        0        0     1406 2023-04-08 03:43:27.466454 magnify-0.2.1/src/magnify/pipeline.py
+-rw-r--r--   0        0        0      158 2023-04-07 22:03:32.255470 magnify-0.2.1/src/magnify/postprocess.py
+-rw-r--r--   0        0        0     1735 2023-04-11 21:20:43.805573 magnify-0.2.1/src/magnify/preprocess.py
+-rw-r--r--   0        0        0    13646 2023-04-11 21:28:02.015984 magnify-0.2.1/src/magnify/reader.py
+-rw-r--r--   0        0        0     3154 2023-04-08 03:43:33.554598 magnify-0.2.1/src/magnify/registry.py
+-rw-r--r--   0        0        0     1121 2023-04-07 21:54:06.746151 magnify-0.2.1/src/magnify/stitch.py
+-rw-r--r--   0        0        0     1583 2023-04-08 03:43:14.150139 magnify-0.2.1/src/magnify/utils.py
+-rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 magnify-0.2.1/PKG-INFO
```

### Comparing `magnify-0.2.0/pyproject.toml` & `magnify-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnify"
-version = "0.2.0"
+version = "0.2.1"
 description = "A microscopy image processing toolkit."
 authors = ["Karl Krauth <karl.krauth@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 opencv-python = [
```

### Comparing `magnify-0.2.0/src/magnify/find.py` & `magnify-0.2.1/src/magnify/find.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,39 +22,37 @@
         row_dist: float = 375 / 3.22,
         col_dist: float = 655 / 3.22,
         min_button_radius: int = 4,
         max_button_radius: int = 15,
         cluster_penalty: float = 10,
         roi_length: int = 61,
         progress_bar: bool = False,
+        search_timesteps: list[int] | None = None,
     ):
         self.row_dist = row_dist
         self.col_dist = col_dist
         self.min_button_radius = min_button_radius
         self.max_button_radius = max_button_radius
         self.cluster_penalty = cluster_penalty
         self.roi_length = roi_length
         self.progress_bar = progress_bar
+        self.search_timesteps = search_timesteps
 
     def __call__(self, assay: xr.Dataset) -> xr.Dataset:
         num_rows, num_cols = assay.id.shape
         if isinstance(assay.search_channel, str):
             if assay.search_channel in assay.channel:
                 search_channels = [assay.search_channel]
             elif assay.search_channel == "all":
                 search_channels = assay.channel
             else:
                 raise ValueError(f"{assay.search_channel} is not a channel name.")
         else:
             # We're searching across multiple channels.
             search_channels = assay.search_channel
-        min_button_dist = round(min(self.row_dist, self.col_dist) / 2)
-        if min_button_dist % 2 == 0:
-            # Certain opencv functions require an odd blocksize.
-            min_button_dist -= 1
 
         # Create the array of subimage regions.
         roi = da.empty(
             (
                 num_rows,
                 num_cols,
                 assay.dims["channel"],
@@ -102,242 +100,263 @@
                 ("marker_row", "marker_col", "time"),
                 np.empty((num_rows, num_cols, assay.dims["time"])),
             ),
         )
 
         # Run the button finding algorithm for each timestep.
         for t, time in enumerate(tqdm.tqdm(assay.time, disable=not self.progress_bar)):
-            # Preload all images for this timnepoint so we only read from disk once.
-            images = assay.image.sel(time=time).to_numpy()
-            points = np.empty((0, 2))
-            for channel in search_channels:
-                c = np.where(assay.channel == channel)[0][0]
-                image = utils.to_uint8(images[c])
-                # Step 1: Find an imperfect button mask by thresholding.
-                mask = cv.adaptiveThreshold(
-                    image,
-                    maxValue=255,
-                    adaptiveMethod=cv.ADAPTIVE_THRESH_GAUSSIAN_C,
-                    thresholdType=cv.THRESH_BINARY,
-                    blockSize=min_button_dist,
-                    C=-1,
-                )
-                # Step 2: Find connected components and filter out points.
-                _, _, stats, new_points = cv.connectedComponentsWithStats(mask, connectivity=4)
-
-                # Ignore the background point.
-                new_points = new_points[1:]
-                stats = stats[1:]
-
-                # Exclude large and small blobs.
-                new_points = new_points[
-                    (stats[:, cv.CC_STAT_HEIGHT] <= 2 * self.max_button_radius)
-                    & (stats[:, cv.CC_STAT_WIDTH] <= 2 * self.max_button_radius)
-                    & (stats[:, cv.CC_STAT_HEIGHT] >= 2 * self.min_button_radius)
-                    & (stats[:, cv.CC_STAT_WIDTH] >= 2 * self.min_button_radius)
-                ]
-                # Remove points too close to other points in this channel.
-                dist_matrix = np.linalg.norm(
-                    new_points[np.newaxis] - new_points[:, np.newaxis], axis=2
+            # Preload all images for this timestep so we only read from disk once.
+            images = assay.image.sel(time=time).compute()
+            # Re-use the previous button locations if the user has specified that we should only
+            # search on specific timesteps.
+            do_search = t == 0 or self.search_timesteps is None or t in self.search_timesteps
+
+            # Find button centers.
+            if do_search:
+                assay.x[..., t], assay.y[..., t] = self.find_centers(
+                    images.sel(channel=search_channels), assay
                 )
-                dist_matrix[np.diag_indices(len(dist_matrix))] = np.inf
-                new_points = new_points[np.min(dist_matrix, axis=1) > min_button_dist]
-
-                if len(points) > 0:
-                    # Remove points too close to other points in previous channels.
-                    dist_matrix = np.linalg.norm(
-                        points[np.newaxis] - new_points[:, np.newaxis], axis=2
-                    )
-                    new_points = new_points[np.min(dist_matrix, axis=1) > min_button_dist]
-
-                # Add the new points to the list of seen points.
-                points = np.concatenate([points, new_points])
-
-            # Split the points into x and y components.
-            x = points[:, 0]
-            y = points[:, 1]
-
-            # Step 3: Cluster the points into distinct rows and columns.
-            # The number of buttons we expect to see per row/col can vary if we have blank buttons.
-            points_per_row = (assay.id != "").sum(dim="marker_col")
-            row_labels = cluster_1d(
-                y,
-                total_length=image.shape[0],
-                num_clusters=num_rows,
-                cluster_length=self.row_dist,
-                ideal_num_points=points_per_row,
-                penalty=self.cluster_penalty,
-            )
-            points_per_col = (assay.id != "").sum(dim="marker_row")
-            col_labels = cluster_1d(
-                x,
-                total_length=image.shape[1],
-                num_clusters=num_cols,
-                cluster_length=self.col_dist,
-                ideal_num_points=points_per_col,
-                penalty=self.cluster_penalty,
-            )
-
-            # Exclude boundary points that didn't fall into clusters.
-            in_cluster = (row_labels >= 0) & (col_labels >= 0)
-            x, y = x[in_cluster], y[in_cluster]
-            col_labels, row_labels = col_labels[in_cluster], row_labels[in_cluster]
-
-            # Step 4: Draw lines through each cluster.
-            row_slope, row_intercepts = regress_clusters(
-                x, y, labels=row_labels, num_clusters=num_rows, ideal_num_points=points_per_row
-            )
-            # We treat column indices as y and row indices as x to avoid near-infinite slopes.
-            col_slope, col_intercepts = regress_clusters(
-                y,
-                x,
-                labels=col_labels,
-                num_clusters=num_cols,
-                ideal_num_points=points_per_col,
-            )
-
-            # Step 5: Set button locations as the intersection of each line pair.
-            assay.y[..., t] = (
-                row_slope * col_intercepts[np.newaxis] + row_intercepts[:, np.newaxis]
-            ) / (1 - row_slope * col_slope)
-            assay.x[..., t] = assay.y[..., t] * col_slope + col_intercepts[np.newaxis]
+            else:
+                assay.x[..., t] = assay.x[..., t - 1]
+                assay.y[..., t] = assay.y[..., t - 1]
 
-            # Step 6: Extract a region around each button.
+            # Extract a region around each button.
             offsets = np.empty((num_rows, num_cols, 2), dtype=int)
-            roi = np.empty(
-                (num_rows, num_cols, assay.dims["channel"], self.roi_length, self.roi_length),
-                dtype=assay.roi.dtype,
+            roi = xr.DataArray(
+                data=np.empty_like(assay.roi[:, :, :, t]), coords=assay.roi[:, :, :, t].coords
             )
             for i in range(num_rows):
                 for j in range(num_cols):
                     top, bottom, left, right = utils.bounding_box(
                         round(float(assay.x[i, j, t])),
                         round(float(assay.y[i, j, t])),
                         self.roi_length,
                         assay.sizes["im_y"],
                         assay.sizes["im_x"],
                     )
                     roi[i, j] = images[:, top:bottom, left:right]
                     offsets[i, j] = [left, top]
             assay.roi[:, :, :, t] = roi
 
-            # Step 7: Compute the foreground and background masks for all buttons.
-            fg = np.empty(
-                (num_rows, num_cols, assay.dims["channel"], self.roi_length, self.roi_length),
-                dtype=bool,
+            # Compute the foreground and background masks for all buttons.
+            if do_search:
+                assay.fg[:, :, :, t], assay.bg[:, :, :, t] = self.find_masks(
+                    roi.sel(channel=search_channels), offsets, t, assay
+                )
+            else:
+                assay.fg[:, :, :, t] = assay.fg[:, :, :, t - 1]
+                assay.bg[:, :, :, t] = assay.bg[:, :, :, t - 1]
+
+        # assay = assay.stack(marker=("marker_row", "marker_col"), create_index=True).transpose(
+        #     "marker", ...
+        # )
+        # assay = assay.set_xindex("id")
+
+        return assay
+
+    def find_centers(self, images: xr.DataArray, assay: xr.Dataset):
+        points = np.empty((0, 2))
+        min_button_dist = round(min(self.row_dist, self.col_dist) / 2)
+        if min_button_dist % 2 == 0:
+            # Certain opencv functions require an odd blocksize.
+            min_button_dist -= 1
+        for image in images:
+            image = utils.to_uint8(image.to_numpy())
+            # Step 1: Find an imperfect button mask by thresholding.
+            mask = cv.adaptiveThreshold(
+                image,
+                maxValue=255,
+                adaptiveMethod=cv.ADAPTIVE_THRESH_GAUSSIAN_C,
+                thresholdType=cv.THRESH_BINARY,
+                blockSize=min_button_dist,
+                C=-1,
             )
-            bg = np.empty_like(fg)
-            for i in range(num_rows):
-                for j in range(num_cols):
-                    # TODO: This step should occur over multiple channels.
-                    c = np.where(assay.channel == search_channels[0])[0][0]
-                    subimage = utils.to_uint8(roi[i, j, c])
-
-                    # Find circles to refine our button estimate unless we have a blank chamber.
-                    circles = None
-                    if assay.id[i, j] != "":
-                        # Filter the subimage to smooth edges and remove noise.
-                        filtered = cv.bilateralFilter(
-                            subimage,
-                            d=9,
-                            sigmaColor=75,
-                            sigmaSpace=75,
-                            borderType=cv.BORDER_DEFAULT,
-                        )
-
-                        # Find any circles in the subimage.
-                        circles = cv.HoughCircles(
-                            filtered,
-                            method=cv.HOUGH_GRADIENT,
-                            dp=1,
-                            minDist=50,
-                            param1=20,
-                            param2=5,
-                            minRadius=self.min_button_radius,
-                            maxRadius=self.max_button_radius,
-                        )
-
-                    # Update our estimate of the button position if we found some circles.
-                    if circles is not None:
-                        circles = circles[0, :, :2]
-                        point = np.array([assay.x[i, j, t], assay.y[i, j, t]]) - offsets[i, j]
-                        # Use the circle center closest to our previous estimate of the button.
-                        closest_idx = np.argmin(np.linalg.norm(circles - point, axis=1))
-                        assay.x[i, j, t], assay.y[i, j, t] = circles[closest_idx] + offsets[i, j]
+            # Step 2: Find connected components and filter out points.
+            _, _, stats, new_points = cv.connectedComponentsWithStats(mask, connectivity=4)
 
-                    x_rel = round(float(assay.x[i, j, t])) - offsets[i, j, 0]
-                    y_rel = round(float(assay.y[i, j, t])) - offsets[i, j, 1]
+            # Ignore the background point.
+            new_points = new_points[1:]
+            stats = stats[1:]
+
+            # Exclude large and small blobs.
+            new_points = new_points[
+                (stats[:, cv.CC_STAT_HEIGHT] <= 2 * self.max_button_radius)
+                & (stats[:, cv.CC_STAT_WIDTH] <= 2 * self.max_button_radius)
+                & (stats[:, cv.CC_STAT_HEIGHT] >= 2 * self.min_button_radius)
+                & (stats[:, cv.CC_STAT_WIDTH] >= 2 * self.min_button_radius)
+            ]
+            # Remove points too close to other points in this channel.
+            dist_matrix = np.linalg.norm(new_points[np.newaxis] - new_points[:, np.newaxis], axis=2)
+            dist_matrix[np.diag_indices(len(dist_matrix))] = np.inf
+            new_points = new_points[np.min(dist_matrix, axis=1) > min_button_dist]
+
+            if len(points) > 0:
+                # Remove points too close to other points in previous channels.
+                dist_matrix = np.linalg.norm(points[np.newaxis] - new_points[:, np.newaxis], axis=2)
+                new_points = new_points[np.min(dist_matrix, axis=1) > min_button_dist]
 
-                    # Set the foreground (the button) to be a circle of fixed radius.
-                    fg_mask = utils.circle(
-                        self.roi_length,
-                        row=y_rel,
-                        col=x_rel,
-                        radius=self.max_button_radius,
-                        value=True,
-                    )
+            # Add the new points to the list of seen points.
+            points = np.concatenate([points, new_points])
 
-                    # Set the background to be the annulus around our foreground.
-                    bg_mask = utils.circle(
-                        self.roi_length,
-                        row=y_rel,
-                        col=x_rel,
-                        radius=2 * self.max_button_radius,
-                        value=True,
-                    )
-                    bg_mask &= ~fg_mask
+        # Split the points into x and y components.
+        x = points[:, 0]
+        y = points[:, 1]
+
+        # Step 3: Cluster the points into distinct rows and columns.
+        points_per_row = (assay.id != "").sum(dim="marker_col")
+        points_per_col = (assay.id != "").sum(dim="marker_row")
+        num_rows, num_cols = assay.sizes["marker_row"], assay.sizes["marker_col"]
+        row_labels = cluster_1d(
+            y,
+            total_length=image.shape[0],
+            num_clusters=num_rows,
+            cluster_length=self.row_dist,
+            ideal_num_points=points_per_row,
+            penalty=self.cluster_penalty,
+        )
+        col_labels = cluster_1d(
+            x,
+            total_length=image.shape[1],
+            num_clusters=num_cols,
+            cluster_length=self.col_dist,
+            ideal_num_points=points_per_col,
+            penalty=self.cluster_penalty,
+        )
 
-                    # Refine the foreground & background by finding areas that are bright and dim.
-                    _, bright_mask = cv.threshold(
-                        subimage, thresh=0, maxval=1, type=cv.THRESH_BINARY + cv.THRESH_OTSU
+        # Exclude boundary points that didn't fall into clusters.
+        in_cluster = (row_labels >= 0) & (col_labels >= 0)
+        x, y = x[in_cluster], y[in_cluster]
+        col_labels, row_labels = col_labels[in_cluster], row_labels[in_cluster]
+
+        # Step 4: Draw lines through each cluster.
+        row_slope, row_intercepts = regress_clusters(
+            x, y, labels=row_labels, num_clusters=num_rows, ideal_num_points=points_per_row
+        )
+        # We treat column indices as y and row indices as x to avoid near-infinite slopes.
+        col_slope, col_intercepts = regress_clusters(
+            y,
+            x,
+            labels=col_labels,
+            num_clusters=num_cols,
+            ideal_num_points=points_per_col,
+        )
+
+        # Step 5: Set button locations as the intersection of each line pair.
+        marker_y = (row_slope * col_intercepts[np.newaxis] + row_intercepts[:, np.newaxis]) / (
+            1 - row_slope * col_slope
+        )
+        marker_x = marker_y * col_slope + col_intercepts[np.newaxis]
+
+        return marker_x, marker_y
+
+    def find_masks(self, roi: np.ndarray, offsets: np.ndarray, t: int, assay: xr.Dataset):
+        num_rows, num_cols = roi.shape[:2]
+        fg = np.empty_like(roi, dtype=bool)
+        bg = np.empty_like(fg)
+        for i in range(num_rows):
+            for j in range(num_cols):
+                # TODO: This step should occur over multiple channels.
+                subimage = utils.to_uint8(roi[i, j, 0].to_numpy())
+
+                # Find circles to refine our button estimate unless we have a blank chamber.
+                circles = None
+                if assay.id[i, j] != "":
+                    # Filter the subimage to smooth edges and remove noise.
+                    filtered = cv.bilateralFilter(
+                        subimage,
+                        d=9,
+                        sigmaColor=75,
+                        sigmaSpace=75,
+                        borderType=cv.BORDER_DEFAULT,
                     )
-                    dim_mask = ~cv.dilate(
-                        bright_mask, np.ones((self.max_button_radius, self.max_button_radius))
+
+                    # Find any circles in the subimage.
+                    circles = cv.HoughCircles(
+                        filtered,
+                        method=cv.HOUGH_GRADIENT,
+                        dp=1,
+                        minDist=self.roi_length / 2,
+                        param1=20,
+                        param2=5,
+                        minRadius=self.min_button_radius,
+                        maxRadius=self.max_button_radius,
                     )
-                    bright_mask = bright_mask.astype(bool)
-                    dim_mask = dim_mask.astype(bool)
 
-                    # If part of the button is bright then set the foreground to that bright area.
-                    if np.any(fg_mask & bright_mask):
-                        fg_mask &= bright_mask
+                # Update our estimate of the button position if we found some circles.
+                if circles is not None:
+                    circles = circles[0, :, :2]
+                    point = np.array([assay.x[i, j, t], assay.y[i, j, t]]) - offsets[i, j]
+                    # Use the circle center closest to our previous estimate of the button.
+                    closest_idx = np.argmin(np.linalg.norm(circles - point, axis=1))
+                    assay.x[i, j, t], assay.y[i, j, t] = circles[closest_idx] + offsets[i, j]
 
-                    # The background on the other hand should not be bright.
-                    if np.any(bg_mask & dim_mask):
-                        bg_mask &= dim_mask
+                x_rel = round(float(assay.x[i, j, t])) - offsets[i, j, 0]
+                y_rel = round(float(assay.y[i, j, t])) - offsets[i, j, 1]
 
-                    fg[i, j] = fg_mask
-                    bg[i, j] = bg_mask
+                # Set the foreground (the button) to be a circle of fixed radius.
+                fg_mask = utils.circle(
+                    self.roi_length,
+                    row=y_rel,
+                    col=x_rel,
+                    radius=self.max_button_radius,
+                    value=True,
+                )
 
-            assay.fg[:, :, :, t] = fg
-            assay.bg[:, :, :, t] = bg
+                # Set the background to be the annulus around our foreground.
+                bg_mask = utils.circle(
+                    self.roi_length,
+                    row=y_rel,
+                    col=x_rel,
+                    radius=2 * self.max_button_radius,
+                    value=True,
+                )
+                bg_mask &= ~fg_mask
 
-        assay = assay.stack(marker=("marker_row", "marker_col"), create_index=True).transpose(
-            "marker", ...
-        )
-        assay = assay.set_xindex("id")
+                # Refine the foreground & background by finding areas that are bright and dim.
+                _, bright_mask = cv.threshold(
+                    subimage, thresh=0, maxval=1, type=cv.THRESH_BINARY + cv.THRESH_OTSU
+                )
+                dim_mask = ~cv.dilate(
+                    bright_mask, np.ones((self.max_button_radius, self.max_button_radius))
+                )
+                bright_mask = bright_mask.astype(bool)
+                dim_mask = dim_mask.astype(bool)
 
-        return assay
+                # If part of the button is bright then set the foreground to that bright area.
+                if np.any(fg_mask & bright_mask):
+                    fg_mask &= bright_mask
+
+                # The background on the other hand should not be bright.
+                if np.any(bg_mask & dim_mask):
+                    bg_mask &= dim_mask
+
+                fg[i, j] = fg_mask
+                bg[i, j] = bg_mask
+
+        return fg, bg
 
     @registry.components.register("find_buttons")
     def make(
         row_dist: float = 375 / 3.22,
         col_dist: float = 655 / 3.22,
         min_button_radius: int = 4,
         max_button_radius: int = 15,
         cluster_penalty: float = 10,
         roi_length: int = 61,
         progress_bar: bool = False,
+        search_timesteps: list[int] | None = None,
     ):
         return ButtonFinder(
             row_dist=row_dist,
             col_dist=col_dist,
             min_button_radius=min_button_radius,
             cluster_penalty=cluster_penalty,
             roi_length=roi_length,
             progress_bar=progress_bar,
+            search_timesteps=search_timesteps,
         )
 
 
 class BeadFinder:
     def __init__(
         self,
         min_bead_radius: int = 10,
@@ -598,11 +617,11 @@
     # Re-estimate intercepts using a weighted mean of global and local estimates.
     # This reduces outlier effects while still allowing uneven intercepts from image stitching.
     for i, (x, y) in enumerate(cluster_points):
         if ideal_num_points[i] != 0 and not_nan[i]:
             weight = min(len(x), ideal_num_points[i]) / ideal_num_points[i]
             intercepts[i] = weight * intercepts[i] + (1 - weight) * (intercept_m * i + intercept_b)
         else:
-            # Just use our global estimate when we have an cluster.
+            # Just use our global estimate when we have an empty cluster.
             intercepts[i] = intercept_m * i + intercept_b
 
     return slope, intercepts
```

### Comparing `magnify-0.2.0/src/magnify/pipeline.py` & `magnify-0.2.1/src/magnify/pipeline.py`

 * *Files identical despite different names*

### Comparing `magnify-0.2.0/src/magnify/preprocess.py` & `magnify-0.2.1/src/magnify/preprocess.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,7 +40,15 @@
 @registry.component("horizontal_flip")
 def horizontal_flip(assay: xr.Dataset):
     if "image" in assay:
         assay["image"] = assay.image.isel(im_x=slice(None, None, -1))
     else:
         assay["tile"] = assay.tile.isel(tile_x=slice(None, None, -1))
     return assay
+
+@registry.component("vertical_flip")
+def vertical_flip(assay: xr.Dataset):
+    if "image" in assay:
+        assay["image"] = assay.image.isel(im_y=slice(None, None, -1))
+    else:
+        assay["tile"] = assay.tile.isel(tile_y=slice(None, None, -1))
+    return assay
```

### Comparing `magnify-0.2.0/src/magnify/reader.py` & `magnify-0.2.1/src/magnify/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         times: Sequence[int] | None = None,
         channels: Sequence[str] | None = None,
     ) -> Iterator[xr.Dataset]:
         if isinstance(data, str):
             data = [data]
 
         for d in data:
-            path_dict = extract_paths(d)
+            path_dict, info_dict = extract_paths(d)
             if len(path_dict) == 0:
                 raise FileNotFoundError(f"The pattern {d} did not lead to any files.")
 
             for assay_name, assay_dict in sorted(
                 path_dict.items(), key=lambda x: utils.natural_sort_key(x[0])
             ):
                 # Use these variables within the loop so we don't affect other assays.
@@ -139,16 +139,16 @@
 
                 # Check the dimensions specified in the path and inside the tiff file do not overlap.
                 if set(dims_in_file).intersection(dims_in_path):
                     raise ValueError(
                         "Dimensions specified in the path names and inside the tiff file overlap."
                     )
 
-                # Setup a dask array to lazyload image tiles.
-                filenames = [path for _, path in sorted(assay_dict.items())]
+                # Setup a dask array to lazyload image tiles and extract attributes.
+                filenames = [x for _, x in sorted(assay_dict.items())]
 
                 def read_tile(block_id, filenames):
                     outer_id = block_id[: len(outer_shape)]
                     inner_id = block_id[len(outer_shape) :]
                     if len(outer_id) > 0:
                         file_idx = np.ravel_multi_index(outer_id, outer_shape)
                     else:
@@ -184,14 +184,21 @@
 
                 coords = {}
                 # Set named coordinates for channels and times if they're available.
                 if channel_coords is not None:
                     coords["channel"] = channel_coords
                 if time_coords is not None:
                     coords["time"] = time_coords
+                # Get the indices specified in the info dict each in sorted order.
+                assay_info = info_dict[assay_name]
+                if assay_info:
+                    info_idxs, time_idxs = (sorted(set(idx)) for idx in zip(*assay_info.keys()))
+                    for info_idx in info_idxs:
+                        info_vals = [assay_info[(info_idx, time_idx)] for time_idx in time_idxs]
+                        coords[info_idx] = ("time", info_vals)
 
                 # Put all our data into an xarray dataset.
                 assay = xr.Dataset(
                     {"tile": (dims_in_path + dims_in_file, tiles)},
                     coords=coords,
                     attrs={
                         "name": assay_name,
@@ -245,27 +252,30 @@
 
     # Filter out special signifiers used for pattern matching.
     glob_path = pattern.replace("(assay)", "*")
     glob_path = glob_path.replace("(channel)", "*")
     glob_path = re.sub(r"\(time\s*\|?.*?\)", "*", glob_path)
     glob_path = glob_path.replace("(row)", "*")
     glob_path = glob_path.replace("(col)", "*")
+    glob_path = re.sub(r"\(info\s*=\s*.*?\)", "*", glob_path)
 
     # Search for files matching the pattern.
     paths = glob.glob(glob_path, recursive=True)
 
     regex_path = fnmatch.translate(pattern)
-    regex_path = regex_path.replace("\\(assay\\)", "(?P<assay>.*)")
-    regex_path = regex_path.replace("\\(channel\\)", "(?P<channel>.*)")
-    regex_path = re.sub(r"\\\(time\s*\|?.*?\\\)", r"(?P<time>.*)", regex_path)
-    regex_path = regex_path.replace("\\(row\\)", "(?P<row>.*)")
-    regex_path = regex_path.replace("\\(col\\)", "(?P<col>.*)")
+    regex_path = regex_path.replace("\\(assay\\)", "(?P<assay>.*?)")
+    regex_path = regex_path.replace("\\(channel\\)", "(?P<channel>.*?)")
+    regex_path = re.sub(r"\\\(time\s*\|?.*?\\\)", r"(?P<time>.*?)", regex_path)
+    regex_path = regex_path.replace("\\(row\\)", "(?P<row>.*?)")
+    regex_path = regex_path.replace("\\(col\\)", "(?P<col>.*?)")
+    regex_path = re.sub(r"\\\(info\s*=\s*(.*?)\\\)", r"(?P<\1>.*?)", regex_path)
     regex_path = re.compile(regex_path, re.IGNORECASE)
 
     path_dict = collections.defaultdict(dict)
+    info_dict = collections.defaultdict(dict)
     for path in paths:
         match = regex_path.fullmatch(path)
         if "(assay)" in pattern:
             assay = match.group("assay")
         else:
             assay = ""
 
@@ -296,8 +306,13 @@
 
         idx = (channel, time, row, col)
         if idx not in path_dict[assay]:
             path_dict[assay][idx] = os.path.abspath(path)
         else:
             raise ValueError(f"{path} and {path_dict[assay][idx]} map to the same index.")
 
-    return path_dict
+        info_search = re.search(r"\(info\s*=\s*(.*?)\)", pattern)
+        if info_search:
+            for info in info_search.groups():
+                info_dict[assay][info, time] = match.group(info)
+
+    return path_dict, info_dict
```

### Comparing `magnify-0.2.0/src/magnify/registry.py` & `magnify-0.2.1/src/magnify/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,32 +51,34 @@
     config = defaults.merge(confection.Config(kwargs))
     pipe = Pipeline("read", config=config)
     pipe.add_pipe("read_pinlist")
     # pipe.add_pipe("preprocessor")
     pipe.add_pipe("horizontal_flip")
     pipe.add_pipe("stitch")
     pipe.add_pipe("horizontal_flip")
+    pipe.add_pipe("vertical_flip")
     pipe.add_pipe("find_buttons")
     # pipe.add_pipe("background_filter")
     pipe.add_pipe("squeeze")
 
     return pipe
 
 
 def pc_chip_pipeline(**kwargs):
     # Button centers are apart 412um vertically and 760um horizontally.
     # Assuming a 4x objective and 2x2 binning each pixel is 3.22um.
     defaults = confection.Config(dict(row_dist=412 / 3.22, col_dist=760 / 3.22))
     config = defaults.merge(confection.Config(kwargs))
-    pipe = Pipeline("read", config=kwargs)
+    pipe = Pipeline("read", config=config)
     pipe.add_pipe("read_pinlist")
     # pipe.add_pipe("preprocessor")
     pipe.add_pipe("horizontal_flip")
     pipe.add_pipe("stitch")
     pipe.add_pipe("horizontal_flip")
+    pipe.add_pipe("vertical_flip")
     pipe.add_pipe("find_buttons")
     # pipe.add_pipe("background_filter")
     pipe.add_pipe("squeeze")
 
     return pipe
```

### Comparing `magnify-0.2.0/src/magnify/stitch.py` & `magnify-0.2.1/src/magnify/stitch.py`

 * *Files identical despite different names*

### Comparing `magnify-0.2.0/src/magnify/utils.py` & `magnify-0.2.1/src/magnify/utils.py`

 * *Files identical despite different names*

### Comparing `magnify-0.2.0/PKG-INFO` & `magnify-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnify
-Version: 0.2.0
+Version: 0.2.1
 Summary: A microscopy image processing toolkit.
 Author: Karl Krauth
 Author-email: karl.krauth@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

