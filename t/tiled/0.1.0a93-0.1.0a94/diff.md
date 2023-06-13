# Comparing `tmp/tiled-0.1.0a93.tar.gz` & `tmp/tiled-0.1.0a94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiled-0.1.0a93.tar", last modified: Wed Jun  7 14:06:01 2023, max compression
+gzip compressed data, was "tiled-0.1.0a94.tar", last modified: Tue Jun 13 00:47:45 2023, max compression
```

## Comparing `tiled-0.1.0a93.tar` & `tiled-0.1.0a94.tar`

### file list

```diff
@@ -1,434 +1,443 @@
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.257600 tiled-0.1.0a93/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1538 2023-01-06 15:55:44.000000 tiled-0.1.0a93/LICENSE
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      783 2023-03-22 13:14:07.000000 tiled-0.1.0a93/MANIFEST.in
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7221 2023-06-07 14:06:01.257600 tiled-0.1.0a93/PKG-INFO
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6555 2023-03-16 20:17:15.000000 tiled-0.1.0a93/README.md
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.205599 tiled-0.1.0a93/benchmarks/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/benchmarks/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1065 2023-02-10 13:17:36.000000 tiled-0.1.0a93/benchmarks/benchmarks.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.205599 tiled-0.1.0a93/docs/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      673 2023-01-06 15:55:44.000000 tiled-0.1.0a93/docs/Makefile
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      797 2023-01-06 15:55:44.000000 tiled-0.1.0a93/docs/make.bat
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.205599 tiled-0.1.0a93/docs/source/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9186 2023-02-10 13:17:36.000000 tiled-0.1.0a93/docs/source/conf.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.209599 tiled-0.1.0a93/docs/source/reference/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    51041 2023-03-31 20:25:00.000000 tiled-0.1.0a93/docs/source/reference/api.yml
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/docs/source/reference/generated/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      554 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.array.ArrayAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      194 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.dataframe.DataFrameAdapter.read_csv.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      722 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.dataframe.DataFrameAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1269 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.excel.ExcelAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1516 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.files.DirectoryAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      741 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.hdf5.HDF5Adapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1181 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.mapping.MapAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      532 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.sparse.COOAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      510 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.tiff.TiffAdapter.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      191 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.xarray.DatasetAdapter.from_dataset.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      147 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.ArrayClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.ArrayClient.read_block.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1110 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.ArrayClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      165 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.DaskArrayClient.export.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.DaskArrayClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      179 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.DaskArrayClient.read_block.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1242 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.DaskArrayClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      152 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.formats.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      143 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.item.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      144 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.login.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      147 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.logout.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      155 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.metadata.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      170 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.new_variation.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      669 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      146 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.specs.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      140 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.uri.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      180 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseStructureClient.download.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      177 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseStructureClient.refresh.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      183 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseStructureClient.structure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      146 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.cache.Cache.in_memory.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      140 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.cache.Cache.on_disk.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      508 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.cache.Cache.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      266 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.cache.Scorer.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      125 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.cache.download.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      165 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.authenticate.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      187 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.force_auth_refresh.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      169 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.from_any_uri.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      155 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.from_app.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      144 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.login.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      147 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.logout.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      152 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.offline.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1029 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      149 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.tokens.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      189 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.export.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      183 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      215 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.read_partition.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1199 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      171 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      203 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.read_partition.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1060 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      121 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.from_profile.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      109 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.from_uri.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.distinct.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.download.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      120 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.get.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      126 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.items.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.keys.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      137 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.metadata.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      143 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.references.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      132 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.refresh.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      129 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.search.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.sort.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      134 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.sorting.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      128 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.specs.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      122 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.uri.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      129 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.node.Node.values.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.sparse.SparseClient.export.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      153 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.sparse.SparseClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1068 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.sparse.SparseClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      168 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.xarray.DaskDatasetClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1555 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.xarray.DaskDatasetClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      156 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.xarray.DatasetClient.read.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1403 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.client.xarray.DatasetClient.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.config.construct_build_app_kwargs.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      124 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.config.parse_configs.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      138 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.iterviews.ValuesView.first.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.iterviews.ValuesView.head.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.iterviews.ValuesView.last.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.iterviews.ValuesView.tail.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      223 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.aliases.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      237 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.media_types.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      226 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.register.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      732 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      202 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.media_type_registration.serialization_registry.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      425 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Comparison.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      382 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Contains.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      334 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Eq.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      392 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.FullText.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      334 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.In.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      219 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Key.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      367 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.KeyLookup.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      358 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.NotEq.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      358 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.NotIn.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      388 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Regex.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       98 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Spec.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      364 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.Specs.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      411 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.queries.StructureFamily.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      459 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.query_registration.QueryRegistry.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      145 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.query_registration.register.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      124 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.app.build_app.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      164 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.app.build_app_from_config.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      207 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.available_bytes.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      173 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.clear.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      198 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.dask_context.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      179 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.discard.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      196 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.discard_dask.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.get.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.put.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      541 2023-03-31 20:25:01.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      176 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.get_object_cache.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      176 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.set_object_cache.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      538 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.ArrayMacroStructure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      433 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.ArrayStructure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      557 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.BuiltinDtype.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      330 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.Endianness.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      485 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.Kind.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      567 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMacroStructure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      660 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMicroStructure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      473 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.dataframe.DataFrameStructure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      505 2023-03-31 20:25:02.000000 tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.sparse.COOStructure.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1083 2023-01-06 15:55:44.000000 tiled-0.1.0a93/docs/source/reference/min-versions.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-01-06 15:55:44.000000 tiled-0.1.0a93/docs/source/reference/release-history.rst
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/docs/source/tutorials/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2347 2023-01-06 15:55:44.000000 tiled-0.1.0a93/docs/source/tutorials/installation.rst
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      280 2023-01-06 15:55:44.000000 tiled-0.1.0a93/pyproject.toml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       90 2023-01-06 15:55:44.000000 tiled-0.1.0a93/requirements-array.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      175 2023-03-16 20:17:15.000000 tiled-0.1.0a93/requirements-client.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-01-06 15:55:44.000000 tiled-0.1.0a93/requirements-compression.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      107 2023-01-06 15:55:44.000000 tiled-0.1.0a93/requirements-dataframe.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      478 2023-06-07 13:54:46.000000 tiled-0.1.0a93/requirements-dev.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      111 2023-01-06 15:55:44.000000 tiled-0.1.0a93/requirements-formats.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      410 2023-06-07 13:54:46.000000 tiled-0.1.0a93/requirements-server.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       23 2023-01-06 15:55:44.000000 tiled-0.1.0a93/requirements-sparse.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      107 2023-01-06 15:55:44.000000 tiled-0.1.0a93/requirements-xarray.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      174 2023-06-07 14:06:01.257600 tiled-0.1.0a93/setup.cfg
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4316 2023-03-31 19:58:35.000000 tiled-0.1.0a93/setup.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.201599 tiled-0.1.0a93/share/
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/share/tiled/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      128 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/.identifying_file_72628d5f953b4229b58c9f1f8f6a9a09
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/share/tiled/static/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16958 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/static/favicon.ico
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/share/tiled/templates/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      189 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/templates/device_code_failure.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      733 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/templates/device_code_form.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      276 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/templates/device_code_success.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2320 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/templates/index.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      491 2023-01-06 15:55:44.000000 tiled-0.1.0a93/share/tiled/templates/page.html
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/share/tiled/ui/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7954 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/asset-manifest.json
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/share/tiled/ui/config/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1588 2023-02-10 13:17:31.000000 tiled-0.1.0a93/share/tiled/ui/config/default.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      203 2023-02-10 13:17:31.000000 tiled-0.1.0a93/share/tiled/ui/configuration_manifest.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16958 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/favicon.ico
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      674 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/index.html
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      292 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/manifest.json
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       67 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/robots.txt
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.201599 tiled-0.1.0a93/share/tiled/ui/static/
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.221599 tiled-0.1.0a93/share/tiled/ui/static/css/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9577 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/css/main.da25efef.css
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    12761 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/css/main.da25efef.css.map
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.237599 tiled-0.1.0a93/share/tiled/ui/static/js/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8354 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/113.a6dabf86.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    25023 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/113.a6dabf86.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      492 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/128.74bef542.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      869 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/128.74bef542.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    95776 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/197.6f7f332e.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   490879 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/197.6f7f332e.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10212 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/214.2a10743e.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    46572 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/214.2a10743e.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13141 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/276.0058e750.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       88 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/276.0058e750.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    37684 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/276.0058e750.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3633 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/321.c6b9dcec.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14931 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/321.c6b9dcec.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3549 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/356.6a2946e1.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10402 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/356.6a2946e1.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   436519 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/393.73e08fb5.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      808 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/393.73e08fb5.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   943354 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/393.73e08fb5.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5877 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/446.ae1590fd.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    25688 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/446.ae1590fd.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   407639 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/470.a78b4c62.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3921 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/470.a78b4c62.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)  1832576 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/470.a78b4c62.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7736 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/485.0ed51a45.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    18509 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/485.0ed51a45.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13996 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/494.3371b974.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    64957 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/494.3371b974.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    50521 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/689.0cde4405.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      245 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/689.0cde4405.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   221121 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/689.0cde4405.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      534 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/69.c379776e.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1255 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/69.c379776e.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    39133 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/705.eeca3f97.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       68 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/705.eeca3f97.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   168665 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/705.eeca3f97.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1175 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/741.fbe96b6d.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2715 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/741.fbe96b6d.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)  1032300 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/773.590aa2f4.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)  1877220 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/773.590aa2f4.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4591 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/787.54a97274.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10281 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/787.54a97274.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5344 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/837.22b95b21.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14836 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/837.22b95b21.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    27323 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/858.2658cad8.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   124490 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/858.2658cad8.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4386 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/883.31ddd2ac.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14318 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/883.31ddd2ac.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      527 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/921.22e363f6.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1293 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/921.22e363f6.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    22754 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       88 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    84726 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.map
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   257278 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/main.5cc3eaa8.js
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1898 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/main.5cc3eaa8.js.LICENSE.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)   898204 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/js/main.5cc3eaa8.js.map
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.241599 tiled-0.1.0a93/share/tiled/ui/static/media/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    64952 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-300-normal.8fc5f5f22c9951113696.woff
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    65244 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-400-normal.376ea5d93f71583052f6.woff
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    65492 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-500-normal.52cb737b682eb9661ee1.woff
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    65292 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-700-normal.ef6d1d09b20b877fee4e.woff
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9500 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-300-normal.48e4b37ecbc5e155460e.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9688 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-400-normal.5e493812deabd1d01e60.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9776 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-500-normal.d1615fb9cd7f67f5018c.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9544 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-700-normal.0334efc0de1012200889.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14988 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-300-normal.12d37040a0160a948ff1.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15344 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-400-normal.493afe7ae8ecfe268800.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15080 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-500-normal.3e748c93fe6a87bdedaa.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14720 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-700-normal.b816cda3107bb21c87e1.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7120 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-300-normal.7c6b44c55d4d9661e3ed.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7100 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-400-normal.1cbfc636c911faa4d0ca.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7000 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-500-normal.007ca18d2cbae7381b39.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6888 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-700-normal.3292e831b18d0c23d609.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1476 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-300-normal.04e05839d6a35e046c13.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1492 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-400-normal.bb723e8458c9c653e505.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1508 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-500-normal.9c0d384f31e2c914edf3.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1436 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-700-normal.9674bc0ae12c2551d9d1.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15732 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-300-normal.0109a2ace896a506a0aa.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15688 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-400-normal.4673b4537a84c7f7a130.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15920 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-500-normal.869888415d0b1a99ae5c.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15828 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-700-normal.0682ca7f74351d42bf73.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11812 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-300-normal.a29236e0fc30e8482530.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11860 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-400-normal.c3dcdbd5bb4d4af80817.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11768 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-500-normal.feaff916fd609e310efe.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11836 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-700-normal.bcf37d666ce10b3556cd.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5460 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-300-normal.af9afdc10c93e4118e90.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5540 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-400-normal.c0bec65d01f776c00c91.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5580 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-500-normal.b8e494da1ec1f1824769.woff2
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5524 2023-02-01 14:32:01.000000 tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-700-normal.3096f18acebc3f07020d.woff2
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.257600 tiled-0.1.0a93/tiled/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       73 2023-02-28 19:49:29.000000 tiled-0.1.0a93/tiled/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       43 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/__main__.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.249600 tiled-0.1.0a93/tiled/_tests/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1792 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/_tests/conftest.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7046 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/_tests/test_access_control.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1072 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_allow_origins.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5569 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16121 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_authentication.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1453 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/test_authenticators.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2224 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/test_caches.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6224 2023-06-07 13:54:49.000000 tiled-0.1.0a93/tiled/_tests/test_client.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13661 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_client_cache.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3285 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_config.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.249600 tiled-0.1.0a93/tiled/_tests/test_configs/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      166 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/_tests/test_configs/config_missing_api_key.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      332 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/_tests/test_configs/config_missing_secret_keys.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      448 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_configs/config_missing_secret_keys_public.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      195 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/_tests/test_configs/config_public_no_authenticator.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      196 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/_tests/test_configs/config_with_api_key.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      434 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_configs/config_with_secret_keys.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1475 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_custom_format.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2297 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11651 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_directory_walker.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4037 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/_tests/test_distinct.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4628 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_export.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4090 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_hdf5.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      555 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_history.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1189 2023-04-01 11:07:41.000000 tiled-0.1.0a93/tiled/_tests/test_import_object.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2782 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_indexers.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3958 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_inlined_contents.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      780 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/test_json.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1565 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_metrics.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      411 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/test_no_heavy_imports.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5087 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_object_cache.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1385 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_openapi.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1369 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_pickle.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5203 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_queries.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      362 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/test_routes.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1125 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_scaled_config_option.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1999 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_search.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      290 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_sentinel.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2408 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_size_limit.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      621 2023-06-02 00:09:11.000000 tiled-0.1.0a93/tiled/_tests/test_slash.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3364 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_sort.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2320 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2357 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_specs_and_references.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1211 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_structured_array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4237 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_tiff.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      342 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/test_tokenize.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4233 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_validation.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    12165 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_writing.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4967 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/_tests/test_xarray.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      657 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/_tests/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3991 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/_tests/writable_adapters.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      500 2023-06-07 14:06:01.257600 tiled-0.1.0a93/tiled/_version.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2797 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/access_policies.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.249600 tiled-0.1.0a93/tiled/adapters/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/adapters/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3846 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/adapters/array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5288 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/adapters/dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1942 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/adapters/excel.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    30376 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/adapters/files.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4874 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/adapters/hdf5.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    14630 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/adapters/mapping.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3639 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/adapters/sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7634 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/adapters/tiff.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1195 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/adapters/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1890 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/adapters/xarray.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    32406 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/authenticators.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/client/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      244 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/client/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    29314 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/client/_testclient.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8896 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/client/array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6561 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/client/auth.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10204 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/client/base.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    27705 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/client/cache.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10173 2023-06-07 13:54:49.000000 tiled-0.1.0a93/tiled/client/constructors.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    37433 2023-06-07 13:54:49.000000 tiled-0.1.0a93/tiled/client/context.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9129 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/client/dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    33534 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/client/node.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4934 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/client/sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    13106 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/client/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7262 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/client/xarray.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/commandline/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/commandline/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4919 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/commandline/_admin.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3230 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/commandline/_api_key.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1411 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/commandline/_profile.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9116 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/commandline/_serve.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2487 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/commandline/_utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7916 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/commandline/main.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    15934 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/config.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/config_schemas/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5275 2023-02-10 13:17:31.000000 tiled-0.1.0a93/tiled/config_schemas/client_profiles.yml
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    16272 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/config_schemas/service_configuration.yml
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/database/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/database/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2658 2023-01-06 15:55:44.000000 tiled-0.1.0a93/tiled/database/alembic.ini.template
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2690 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/database/alembic_utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      157 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/database/base.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1704 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/database/connection_pool.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11164 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/database/core.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/database/migrations/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2261 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/database/migrations/env.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      494 2023-01-06 15:55:44.000000 tiled-0.1.0a93/tiled/database/migrations/script.py.mako
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/database/migrations/versions/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4023 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/database/migrations/versions/481830dd6c11_initialize.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      889 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/database/migrations/versions/4a9dfaba4a98_add_pendingsession.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1270 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1292 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7283 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/database/orm.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.253600 tiled-0.1.0a93/tiled/examples/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1234 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/generate_files.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4902 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/generated.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      941 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/generated_minimal.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      963 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/nexus.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      454 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/numpy_structured_dtypes.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      582 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/toy_authentication.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4762 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/examples/xdi.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6544 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/iterviews.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    10964 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/media_type_registration.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8917 2023-03-27 20:02:34.000000 tiled-0.1.0a93/tiled/profiles.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    11716 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/queries.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4595 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/query_registration.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      690 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/scopes.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.257600 tiled-0.1.0a93/tiled/serialization/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      960 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5187 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3880 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    12962 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/image_serializer_helpers.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2860 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/node.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3016 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4836 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/serialization/xarray.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.257600 tiled-0.1.0a93/tiled/server/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/server/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    33375 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/app.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    37847 2023-06-07 13:54:49.000000 tiled-0.1.0a93/tiled/server/authentication.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     6204 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/server/compression.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    27685 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/core.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4757 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/dependencies.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1082 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/server/etag.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5637 2023-03-22 13:14:07.000000 tiled-0.1.0a93/tiled/server/metrics.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     5845 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/server/object_cache.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     8486 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/server/pydantic_array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2451 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/pydantic_dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      570 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/server/pydantic_sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    31642 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/router.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     9685 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/schemas.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     3071 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/server/settings.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     4608 2023-06-07 13:54:46.000000 tiled-0.1.0a93/tiled/server/utils.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.257600 tiled-0.1.0a93/tiled/structures/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/structures/__init__.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7821 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/structures/array.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1060 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/structures/core.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2529 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/structures/dataframe.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     1035 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/structures/sparse.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    18076 2023-03-31 19:58:35.000000 tiled-0.1.0a93/tiled/utils.py
--rw-rw-r--   0 dallan    (1000) dallan    (1000)      645 2023-02-10 13:17:36.000000 tiled-0.1.0a93/tiled/validation_registration.py
-drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-07 14:06:01.241599 tiled-0.1.0a93/tiled.egg-info/
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     7221 2023-06-07 14:06:01.000000 tiled-0.1.0a93/tiled.egg-info/PKG-INFO
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    19902 2023-06-07 14:06:01.000000 tiled-0.1.0a93/tiled.egg-info/SOURCES.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)        1 2023-06-07 14:06:01.000000 tiled-0.1.0a93/tiled.egg-info/dependency_links.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       54 2023-06-07 14:06:01.000000 tiled-0.1.0a93/tiled.egg-info/entry_points.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)     2165 2023-06-07 14:06:01.000000 tiled-0.1.0a93/tiled.egg-info/requires.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)       17 2023-06-07 14:06:01.000000 tiled-0.1.0a93/tiled.egg-info/top_level.txt
--rw-rw-r--   0 dallan    (1000) dallan    (1000)    80049 2023-02-10 13:17:37.000000 tiled-0.1.0a93/versioneer.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.646725 tiled-0.1.0a94/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1538 2023-01-06 15:55:44.000000 tiled-0.1.0a94/LICENSE
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      783 2023-03-22 13:14:07.000000 tiled-0.1.0a94/MANIFEST.in
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7221 2023-06-13 00:47:45.646725 tiled-0.1.0a94/PKG-INFO
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6555 2023-03-16 20:17:15.000000 tiled-0.1.0a94/README.md
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.602725 tiled-0.1.0a94/benchmarks/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a94/benchmarks/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1065 2023-02-10 13:17:36.000000 tiled-0.1.0a94/benchmarks/benchmarks.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.602725 tiled-0.1.0a94/docs/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      673 2023-01-06 15:55:44.000000 tiled-0.1.0a94/docs/Makefile
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      797 2023-01-06 15:55:44.000000 tiled-0.1.0a94/docs/make.bat
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.602725 tiled-0.1.0a94/docs/source/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9186 2023-02-10 13:17:36.000000 tiled-0.1.0a94/docs/source/conf.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.602725 tiled-0.1.0a94/docs/source/reference/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    53644 2023-06-12 23:42:24.000000 tiled-0.1.0a94/docs/source/reference/api.yml
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.614725 tiled-0.1.0a94/docs/source/reference/generated/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      554 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.array.ArrayAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      194 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.dataframe.DataFrameAdapter.read_csv.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      722 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.dataframe.DataFrameAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1269 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.excel.ExcelAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1516 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.files.DirectoryAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      741 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.hdf5.HDF5Adapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1181 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.mapping.MapAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      532 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.sparse.COOAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      510 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.tiff.TiffAdapter.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      191 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.xarray.DatasetAdapter.from_dataset.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      147 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.array.ArrayClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.array.ArrayClient.read_block.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1110 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.array.ArrayClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      165 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.array.DaskArrayClient.export.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.array.DaskArrayClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      179 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.array.DaskArrayClient.read_block.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1242 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.array.DaskArrayClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      152 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.base.BaseClient.formats.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      143 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.base.BaseClient.item.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      144 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.base.BaseClient.login.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      147 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.base.BaseClient.logout.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      155 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.base.BaseClient.metadata.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      170 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.base.BaseClient.new_variation.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      669 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.base.BaseClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      146 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.base.BaseClient.specs.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      140 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.base.BaseClient.uri.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      180 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.base.BaseStructureClient.download.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      177 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.base.BaseStructureClient.refresh.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      183 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.base.BaseStructureClient.structure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      146 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.cache.Cache.in_memory.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      140 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.cache.Cache.on_disk.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      508 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.cache.Cache.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      266 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.cache.Scorer.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      125 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.cache.download.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      165 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.context.Context.authenticate.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      187 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.context.Context.force_auth_refresh.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      169 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.context.Context.from_any_uri.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      155 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.context.Context.from_app.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      144 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.context.Context.login.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      147 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.context.Context.logout.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      152 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.context.Context.offline.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1029 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.context.Context.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      149 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.context.Context.tokens.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      189 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.export.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      183 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      215 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.read_partition.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1199 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      171 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      203 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.read_partition.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1060 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      121 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.from_profile.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      109 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.from_uri.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.distinct.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.download.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      120 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.get.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      126 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.items.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.keys.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      137 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.metadata.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      143 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.references.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      132 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.refresh.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      129 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.search.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.sort.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      134 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.sorting.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      128 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.specs.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      122 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.uri.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      129 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.node.Node.values.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.sparse.SparseClient.export.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      153 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.sparse.SparseClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1068 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.sparse.SparseClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      168 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.xarray.DaskDatasetClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1592 2023-06-12 23:33:13.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.xarray.DaskDatasetClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      156 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.xarray.DatasetClient.read.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1436 2023-06-12 23:33:13.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.client.xarray.DatasetClient.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.config.construct_build_app_kwargs.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      124 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.config.parse_configs.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      138 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.iterviews.ValuesView.first.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.iterviews.ValuesView.head.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.iterviews.ValuesView.last.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      135 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.iterviews.ValuesView.tail.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      223 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.aliases.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      237 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.media_types.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      226 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.register.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      732 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      202 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.media_type_registration.serialization_registry.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      425 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.queries.Comparison.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      382 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.queries.Contains.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      334 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.queries.Eq.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      392 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.queries.FullText.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      334 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.queries.In.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      219 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.queries.Key.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      367 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.queries.KeyLookup.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      358 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.queries.NotEq.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      358 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.queries.NotIn.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      388 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.queries.Regex.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       98 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.queries.Spec.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      364 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.queries.Specs.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      411 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.queries.StructureFamily.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      459 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.query_registration.QueryRegistry.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      145 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.query_registration.register.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      124 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.server.app.build_app.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      164 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.server.app.build_app_from_config.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      207 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.available_bytes.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      173 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.clear.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      198 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.dask_context.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      179 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.discard.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      196 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.discard_dask.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:02.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.get.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      167 2023-03-31 20:25:02.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.put.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      541 2023-03-31 20:25:01.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      176 2023-03-31 20:25:02.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.server.object_cache.get_object_cache.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      176 2023-03-31 20:25:02.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.server.object_cache.set_object_cache.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      538 2023-03-31 20:25:02.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.structures.array.ArrayMacroStructure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      433 2023-03-31 20:25:02.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.structures.array.ArrayStructure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      557 2023-03-31 20:25:02.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.structures.array.BuiltinDtype.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      330 2023-03-31 20:25:02.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.structures.array.Endianness.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      485 2023-03-31 20:25:02.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.structures.array.Kind.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      567 2023-03-31 20:25:02.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMacroStructure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      660 2023-03-31 20:25:02.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMicroStructure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      473 2023-03-31 20:25:02.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.structures.dataframe.DataFrameStructure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      505 2023-03-31 20:25:02.000000 tiled-0.1.0a94/docs/source/reference/generated/tiled.structures.sparse.COOStructure.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1083 2023-01-06 15:55:44.000000 tiled-0.1.0a94/docs/source/reference/min-versions.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      123 2023-01-06 15:55:44.000000 tiled-0.1.0a94/docs/source/reference/release-history.rst
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.614725 tiled-0.1.0a94/docs/source/tutorials/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2347 2023-01-06 15:55:44.000000 tiled-0.1.0a94/docs/source/tutorials/installation.rst
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      280 2023-01-06 15:55:44.000000 tiled-0.1.0a94/pyproject.toml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       90 2023-01-06 15:55:44.000000 tiled-0.1.0a94/requirements-array.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      175 2023-03-16 20:17:15.000000 tiled-0.1.0a94/requirements-client.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      159 2023-01-06 15:55:44.000000 tiled-0.1.0a94/requirements-compression.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      107 2023-01-06 15:55:44.000000 tiled-0.1.0a94/requirements-dataframe.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      478 2023-06-08 19:17:08.000000 tiled-0.1.0a94/requirements-dev.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      111 2023-01-06 15:55:44.000000 tiled-0.1.0a94/requirements-formats.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      423 2023-06-13 00:46:49.000000 tiled-0.1.0a94/requirements-server.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       23 2023-01-06 15:55:44.000000 tiled-0.1.0a94/requirements-sparse.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      107 2023-01-06 15:55:44.000000 tiled-0.1.0a94/requirements-xarray.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      174 2023-06-13 00:47:45.646725 tiled-0.1.0a94/setup.cfg
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4316 2023-03-31 19:58:35.000000 tiled-0.1.0a94/setup.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.598725 tiled-0.1.0a94/share/
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.614725 tiled-0.1.0a94/share/tiled/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      128 2023-01-06 15:55:44.000000 tiled-0.1.0a94/share/tiled/.identifying_file_72628d5f953b4229b58c9f1f8f6a9a09
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.614725 tiled-0.1.0a94/share/tiled/static/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16958 2023-01-06 15:55:44.000000 tiled-0.1.0a94/share/tiled/static/favicon.ico
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.614725 tiled-0.1.0a94/share/tiled/templates/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      189 2023-01-06 15:55:44.000000 tiled-0.1.0a94/share/tiled/templates/device_code_failure.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      733 2023-01-06 15:55:44.000000 tiled-0.1.0a94/share/tiled/templates/device_code_form.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      276 2023-01-06 15:55:44.000000 tiled-0.1.0a94/share/tiled/templates/device_code_success.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2320 2023-01-06 15:55:44.000000 tiled-0.1.0a94/share/tiled/templates/index.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      491 2023-01-06 15:55:44.000000 tiled-0.1.0a94/share/tiled/templates/page.html
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.614725 tiled-0.1.0a94/share/tiled/ui/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7954 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/asset-manifest.json
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.618725 tiled-0.1.0a94/share/tiled/ui/config/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1588 2023-02-10 13:17:31.000000 tiled-0.1.0a94/share/tiled/ui/config/default.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      203 2023-02-10 13:17:31.000000 tiled-0.1.0a94/share/tiled/ui/configuration_manifest.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16958 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/favicon.ico
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      674 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/index.html
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      292 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/manifest.json
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       67 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/robots.txt
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.598725 tiled-0.1.0a94/share/tiled/ui/static/
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.618725 tiled-0.1.0a94/share/tiled/ui/static/css/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9577 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/css/main.da25efef.css
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    12761 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/css/main.da25efef.css.map
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.626725 tiled-0.1.0a94/share/tiled/ui/static/js/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8354 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/113.a6dabf86.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    25023 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/113.a6dabf86.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      492 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/128.74bef542.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      869 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/128.74bef542.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    95776 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/197.6f7f332e.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   490879 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/197.6f7f332e.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10212 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/214.2a10743e.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    46572 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/214.2a10743e.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13141 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/276.0058e750.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       88 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/276.0058e750.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    37684 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/276.0058e750.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3633 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/321.c6b9dcec.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14931 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/321.c6b9dcec.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3549 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/356.6a2946e1.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10402 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/356.6a2946e1.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   436519 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/393.73e08fb5.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      808 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/393.73e08fb5.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   943354 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/393.73e08fb5.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5877 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/446.ae1590fd.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    25688 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/446.ae1590fd.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   407639 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/470.a78b4c62.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3921 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/470.a78b4c62.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)  1832576 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/470.a78b4c62.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7736 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/485.0ed51a45.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    18509 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/485.0ed51a45.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13996 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/494.3371b974.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    64957 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/494.3371b974.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    50521 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/689.0cde4405.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      245 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/689.0cde4405.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   221121 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/689.0cde4405.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      534 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/69.c379776e.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1255 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/69.c379776e.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    39133 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/705.eeca3f97.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       68 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/705.eeca3f97.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   168665 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/705.eeca3f97.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1175 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/741.fbe96b6d.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2715 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/741.fbe96b6d.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)  1032300 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/773.590aa2f4.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)  1877220 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/773.590aa2f4.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4591 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/787.54a97274.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10281 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/787.54a97274.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5344 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/837.22b95b21.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14836 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/837.22b95b21.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    27323 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/858.2658cad8.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   124490 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/858.2658cad8.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4386 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/883.31ddd2ac.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14318 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/883.31ddd2ac.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      527 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/921.22e363f6.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1293 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/921.22e363f6.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    22754 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       88 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    84726 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.map
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   257278 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/main.5cc3eaa8.js
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1898 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/main.5cc3eaa8.js.LICENSE.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)   898204 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/js/main.5cc3eaa8.js.map
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.630725 tiled-0.1.0a94/share/tiled/ui/static/media/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    64952 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-all-300-normal.8fc5f5f22c9951113696.woff
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    65244 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-all-400-normal.376ea5d93f71583052f6.woff
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    65492 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-all-500-normal.52cb737b682eb9661ee1.woff
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    65292 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-all-700-normal.ef6d1d09b20b877fee4e.woff
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9500 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-300-normal.48e4b37ecbc5e155460e.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9688 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-400-normal.5e493812deabd1d01e60.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9776 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-500-normal.d1615fb9cd7f67f5018c.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9544 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-700-normal.0334efc0de1012200889.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14988 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-ext-300-normal.12d37040a0160a948ff1.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15344 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-ext-400-normal.493afe7ae8ecfe268800.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15080 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-ext-500-normal.3e748c93fe6a87bdedaa.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14720 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-ext-700-normal.b816cda3107bb21c87e1.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7120 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-300-normal.7c6b44c55d4d9661e3ed.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7100 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-400-normal.1cbfc636c911faa4d0ca.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7000 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-500-normal.007ca18d2cbae7381b39.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6888 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-700-normal.3292e831b18d0c23d609.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1476 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-ext-300-normal.04e05839d6a35e046c13.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1492 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-ext-400-normal.bb723e8458c9c653e505.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1508 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-ext-500-normal.9c0d384f31e2c914edf3.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1436 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-ext-700-normal.9674bc0ae12c2551d9d1.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15732 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-300-normal.0109a2ace896a506a0aa.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15688 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-400-normal.4673b4537a84c7f7a130.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15920 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-500-normal.869888415d0b1a99ae5c.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    15828 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-700-normal.0682ca7f74351d42bf73.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11812 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-ext-300-normal.a29236e0fc30e8482530.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11860 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-ext-400-normal.c3dcdbd5bb4d4af80817.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11768 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-ext-500-normal.feaff916fd609e310efe.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11836 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-ext-700-normal.bcf37d666ce10b3556cd.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5460 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-vietnamese-300-normal.af9afdc10c93e4118e90.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5540 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-vietnamese-400-normal.c0bec65d01f776c00c91.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5580 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-vietnamese-500-normal.b8e494da1ec1f1824769.woff2
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5524 2023-02-01 14:32:01.000000 tiled-0.1.0a94/share/tiled/ui/static/media/roboto-vietnamese-700-normal.3096f18acebc3f07020d.woff2
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.646725 tiled-0.1.0a94/tiled/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       73 2023-02-28 19:49:29.000000 tiled-0.1.0a94/tiled/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       43 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/__main__.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.638725 tiled-0.1.0a94/tiled/_tests/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/_tests/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2826 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/_tests/conftest.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7775 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/_tests/test_access_control.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1072 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_allow_origins.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5569 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16121 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_authentication.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1453 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/_tests/test_authenticators.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2224 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/_tests/test_caches.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10951 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/_tests/test_catalog.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6306 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/_tests/test_client.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13661 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_client_cache.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3285 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_config.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.638725 tiled-0.1.0a94/tiled/_tests/test_configs/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      166 2023-03-22 13:14:07.000000 tiled-0.1.0a94/tiled/_tests/test_configs/config_missing_api_key.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      332 2023-03-22 13:14:07.000000 tiled-0.1.0a94/tiled/_tests/test_configs/config_missing_secret_keys.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      448 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_configs/config_missing_secret_keys_public.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      195 2023-03-22 13:14:07.000000 tiled-0.1.0a94/tiled/_tests/test_configs/config_public_no_authenticator.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      196 2023-03-22 13:14:07.000000 tiled-0.1.0a94/tiled/_tests/test_configs/config_with_api_key.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      434 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_configs/config_with_secret_keys.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1475 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_custom_format.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2297 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11651 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_directory_walker.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4037 2023-06-08 19:17:08.000000 tiled-0.1.0a94/tiled/_tests/test_distinct.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4628 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_export.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4090 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_hdf5.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      555 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_history.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1189 2023-04-01 11:07:41.000000 tiled-0.1.0a94/tiled/_tests/test_import_object.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2782 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_indexers.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3958 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_inlined_contents.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      780 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/_tests/test_json.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1565 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_metrics.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      411 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/_tests/test_no_heavy_imports.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5087 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_object_cache.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1385 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_openapi.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1369 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_pickle.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5203 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_queries.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      362 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/_tests/test_routes.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1125 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_scaled_config_option.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1999 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_search.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      290 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_sentinel.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2408 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_size_limit.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3364 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_sort.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2320 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2357 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_specs_and_references.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1211 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_structured_array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4237 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_tiff.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      342 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/_tests/test_tokenize.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4241 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/_tests/test_validation.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    12796 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/_tests/test_writing.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4967 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/_tests/test_xarray.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2160 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/_tests/utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      500 2023-06-13 00:47:45.646725 tiled-0.1.0a94/tiled/_version.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3198 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/access_policies.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.638725 tiled-0.1.0a94/tiled/adapters/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/adapters/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4176 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/adapters/array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5386 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/adapters/dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1942 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/adapters/excel.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    30376 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/adapters/files.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4635 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/adapters/hdf5.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    14630 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/adapters/mapping.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2115 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/adapters/parquet.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3639 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/adapters/sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3316 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/adapters/sparse_blocks_parquet.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7659 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/adapters/tiff.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1195 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/adapters/utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1890 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/adapters/xarray.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2376 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/adapters/zarr.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    32406 2023-06-08 21:11:20.000000 tiled-0.1.0a94/tiled/authenticators.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.642725 tiled-0.1.0a94/tiled/catalog/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       55 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/catalog/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    26150 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/catalog/adapter.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      157 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/catalog/base.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2230 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/catalog/explain.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6511 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/catalog/orm.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.642725 tiled-0.1.0a94/tiled/client/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      244 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/client/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    29314 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/client/_testclient.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8896 2023-03-22 13:14:07.000000 tiled-0.1.0a94/tiled/client/array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6561 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/client/auth.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10209 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/client/base.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    27705 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/client/cache.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10173 2023-06-13 00:46:46.000000 tiled-0.1.0a94/tiled/client/constructors.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    37473 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/client/context.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     9129 2023-03-22 13:14:07.000000 tiled-0.1.0a94/tiled/client/dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    35731 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/client/node.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4934 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/client/sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13106 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/client/utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8070 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/client/xarray.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.642725 tiled-0.1.0a94/tiled/commandline/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/commandline/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4919 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/commandline/_admin.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3230 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/commandline/_api_key.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1247 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/commandline/_catalog.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1411 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/commandline/_profile.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    13062 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/commandline/_serve.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2487 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/commandline/_utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8073 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/commandline/main.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16568 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/config.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.642725 tiled-0.1.0a94/tiled/config_schemas/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5275 2023-02-10 13:17:31.000000 tiled-0.1.0a94/tiled/config_schemas/client_profiles.yml
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16272 2023-06-08 13:16:20.000000 tiled-0.1.0a94/tiled/config_schemas/service_configuration.yml
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.642725 tiled-0.1.0a94/tiled/database/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/database/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2658 2023-01-06 15:55:44.000000 tiled-0.1.0a94/tiled/database/alembic.ini.template
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2690 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/database/alembic_utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      157 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/database/base.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1704 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/database/connection_pool.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11164 2023-06-08 21:11:20.000000 tiled-0.1.0a94/tiled/database/core.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.642725 tiled-0.1.0a94/tiled/database/migrations/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2261 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/database/migrations/env.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      494 2023-01-06 15:55:44.000000 tiled-0.1.0a94/tiled/database/migrations/script.py.mako
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.642725 tiled-0.1.0a94/tiled/database/migrations/versions/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4023 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/database/migrations/versions/481830dd6c11_initialize.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      889 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/database/migrations/versions/4a9dfaba4a98_add_pendingsession.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1270 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1292 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7253 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/database/orm.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.646725 tiled-0.1.0a94/tiled/examples/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/examples/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1234 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/examples/generate_files.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4902 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/examples/generated.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      941 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/examples/generated_minimal.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      963 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/examples/nexus.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      454 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/examples/numpy_structured_dtypes.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      582 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/examples/toy_authentication.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4762 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/examples/xdi.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6544 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/iterviews.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    10560 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/media_type_registration.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8917 2023-03-27 20:02:34.000000 tiled-0.1.0a94/tiled/profiles.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    11716 2023-03-22 13:14:07.000000 tiled-0.1.0a94/tiled/queries.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4595 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/query_registration.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      690 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/scopes.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.646725 tiled-0.1.0a94/tiled/serialization/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      960 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/serialization/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5187 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/serialization/array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3880 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/serialization/dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    12933 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/serialization/image_serializer_helpers.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3558 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/serialization/node.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3179 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/serialization/sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5155 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/serialization/xarray.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.646725 tiled-0.1.0a94/tiled/server/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/server/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    34219 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/server/app.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    37847 2023-06-13 00:46:46.000000 tiled-0.1.0a94/tiled/server/authentication.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6204 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/server/compression.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    29209 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/server/core.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     6010 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/server/dependencies.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1082 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/server/etag.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5637 2023-03-22 13:14:07.000000 tiled-0.1.0a94/tiled/server/metrics.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     5845 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/server/object_cache.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     8486 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/server/pydantic_array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2739 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/server/pydantic_dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      570 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/server/pydantic_sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    34955 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/server/router.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    16920 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/server/schemas.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     3071 2023-06-08 13:16:20.000000 tiled-0.1.0a94/tiled/server/settings.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     4248 2023-06-13 00:46:49.000000 tiled-0.1.0a94/tiled/server/utils.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.646725 tiled-0.1.0a94/tiled/structures/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        0 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/structures/__init__.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7821 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/structures/array.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1060 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/structures/core.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2529 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/structures/dataframe.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     1035 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/structures/sparse.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    18076 2023-03-31 19:58:35.000000 tiled-0.1.0a94/tiled/utils.py
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)      645 2023-02-10 13:17:36.000000 tiled-0.1.0a94/tiled/validation_registration.py
+drwxrwxr-x   0 dallan    (1000) dallan    (1000)        0 2023-06-13 00:47:45.634725 tiled-0.1.0a94/tiled.egg-info/
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     7221 2023-06-13 00:47:45.000000 tiled-0.1.0a94/tiled.egg-info/PKG-INFO
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    20108 2023-06-13 00:47:45.000000 tiled-0.1.0a94/tiled.egg-info/SOURCES.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)        1 2023-06-13 00:47:45.000000 tiled-0.1.0a94/tiled.egg-info/dependency_links.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       54 2023-06-13 00:47:45.000000 tiled-0.1.0a94/tiled.egg-info/entry_points.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)     2217 2023-06-13 00:47:45.000000 tiled-0.1.0a94/tiled.egg-info/requires.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)       17 2023-06-13 00:47:45.000000 tiled-0.1.0a94/tiled.egg-info/top_level.txt
+-rw-rw-r--   0 dallan    (1000) dallan    (1000)    80049 2023-02-10 13:17:37.000000 tiled-0.1.0a94/versioneer.py
```

### Comparing `tiled-0.1.0a93/LICENSE` & `tiled-0.1.0a94/LICENSE`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/MANIFEST.in` & `tiled-0.1.0a94/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/PKG-INFO` & `tiled-0.1.0a94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiled
-Version: 0.1.0a93
+Version: 0.1.0a94
 Summary: Tile-based access to SciPy/PyData data structures over the web in many formats
 Home-page: https://github.com/bluesky/tiled
 Author: Bluesky Collaboration
 Author-email: dallan@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `tiled-0.1.0a93/README.md` & `tiled-0.1.0a94/README.md`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/benchmarks/benchmarks.py` & `tiled-0.1.0a94/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/Makefile` & `tiled-0.1.0a94/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/make.bat` & `tiled-0.1.0a94/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/conf.py` & `tiled-0.1.0a94/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/api.yml` & `tiled-0.1.0a94/docs/source/reference/api.yml`

 * *Files 5% similar despite different names*

```diff
@@ -172,14 +172,27 @@
           - $ref: '#/components/schemas/StructDtype'
           title: Micro
       required:
       - macro
       - micro
       title: ArrayStructure
       type: object
+    Asset:
+      properties:
+        data_uri:
+          title: Data Uri
+          type: string
+        is_directory:
+          title: Is Directory
+          type: boolean
+      required:
+      - data_uri
+      - is_directory
+      title: Asset
+      type: object
     AuthenticationMode:
       description: An enumeration.
       enum:
       - password
       - external
       title: AuthenticationMode
       type: string
@@ -296,14 +309,42 @@
         micro:
           $ref: '#/components/schemas/DataFrameMicroStructure'
       required:
       - micro
       - macro
       title: DataFrameStructure
       type: object
+    DataSource:
+      properties:
+        assets:
+          default: []
+          items:
+            $ref: '#/components/schemas/Asset'
+          title: Assets
+          type: array
+        management:
+          allOf:
+          - $ref: '#/components/schemas/Management'
+          default: writable
+        mimetype:
+          title: Mimetype
+          type: string
+        parameters:
+          default: {}
+          title: Parameters
+          type: object
+        structure:
+          anyOf:
+          - $ref: '#/components/schemas/ArrayStructure'
+          - $ref: '#/components/schemas/DataFrameStructure'
+          - $ref: '#/components/schemas/NodeStructure'
+          - $ref: '#/components/schemas/COOStructure'
+          title: Structure
+      title: DataSource
+      type: object
     DistinctValueInfo:
       properties:
         count:
           title: Count
           type: integer
         value:
           title: Value
@@ -329,14 +370,15 @@
       - structure
       - structure.micro
       - structure.macro
       - count
       - sorting
       - specs
       - references
+      - data_sources
       - ''
       title: EntryFields
       type: string
     Error:
       properties:
         code:
           title: Code
@@ -419,21 +461,35 @@
       - m
       - M
       - S
       - U
       - V
       title: Kind
       type: string
+    Management:
+      description: An enumeration.
+      enum:
+      - external
+      - immutable
+      - locked
+      - writable
+      title: Management
+      type: string
     NodeAttributes:
       properties:
         ancestors:
           items:
             type: string
           title: Ancestors
           type: array
+        data_sources:
+          items:
+            $ref: '#/components/schemas/DataSource'
+          title: Data Sources
+          type: array
         metadata:
           title: Metadata
           type: object
         references:
           items:
             $ref: '#/components/schemas/ReferenceDocument'
           maxItems: 20
@@ -509,14 +565,23 @@
       - prev
       - first
       - last
       title: PaginationLinks
       type: object
     PostMetadataRequest:
       properties:
+        data_sources:
+          default: []
+          items:
+            $ref: '#/components/schemas/DataSource'
+          title: Data Sources
+          type: array
+        id:
+          title: Id
+          type: string
         metadata:
           default: {}
           title: Metadata
           type: object
         references:
           default: []
           items:
@@ -527,29 +592,27 @@
         specs:
           default: []
           items:
             $ref: '#/components/schemas/Spec'
           maxItems: 20
           title: Specs
           type: array
-        structure:
-          anyOf:
-          - $ref: '#/components/schemas/ArrayStructure'
-          - $ref: '#/components/schemas/DataFrameStructure'
-          - $ref: '#/components/schemas/COOStructure'
-          title: Structure
         structure_family:
           $ref: '#/components/schemas/StructureFamily'
       required:
       - structure_family
-      - structure
       title: PostMetadataRequest
       type: object
     PostMetadataResponse:
       properties:
+        data_sources:
+          items:
+            $ref: '#/components/schemas/DataSource'
+          title: Data Sources
+          type: array
         id:
           title: Id
           type: string
         links:
           anyOf:
           - $ref: '#/components/schemas/ArrayLinks'
           - $ref: '#/components/schemas/DataFrameLinks'
@@ -557,14 +620,16 @@
           title: Links
         metadata:
           title: Metadata
           type: object
       required:
       - id
       - links
+      - metadata
+      - data_sources
       title: PostMetadataResponse
       type: object
     PutMetadataRequest:
       properties:
         metadata:
           title: Metadata
           type: object
@@ -578,14 +643,38 @@
           items:
             $ref: '#/components/schemas/Spec'
           maxItems: 20
           title: Specs
           type: array
       title: PutMetadataRequest
       type: object
+    PutMetadataResponse:
+      properties:
+        data_sources:
+          items:
+            $ref: '#/components/schemas/DataSource'
+          title: Data Sources
+          type: array
+        id:
+          title: Id
+          type: string
+        links:
+          anyOf:
+          - $ref: '#/components/schemas/ArrayLinks'
+          - $ref: '#/components/schemas/DataFrameLinks'
+          - $ref: '#/components/schemas/SparseLinks'
+          title: Links
+        metadata:
+          title: Metadata
+          type: object
+      required:
+      - id
+      - links
+      title: PutMetadataResponse
+      type: object
     ReferenceDocument:
       additionalProperties: false
       properties:
         label:
           maxLength: 255
           title: Label
           type: string
@@ -807,15 +896,15 @@
           refreshUrl: token/refresh
           scopes: {}
           tokenUrl: PLACEHOLDER
       type: oauth2
 info:
   description: Structured data access service
   title: Tiled
-  version: 0.1.0a90.post10.dev0+g527579e
+  version: 0.1.0a92.post129.dev0+g681d267
 openapi: 3.0.2
 paths:
   /:
     get:
       operationId: index__get
       responses:
         '200':
@@ -1515,14 +1604,15 @@
           - structure
           - structure.micro
           - structure.macro
           - count
           - sorting
           - specs
           - references
+          - data_sources
           - ''
           items:
             $ref: '#/components/schemas/EntryFields'
           type: array
       - in: query
         name: select_metadata
         required: false
@@ -1541,14 +1631,21 @@
         name: omit_links
         required: false
         schema:
           default: false
           title: Omit Links
           type: boolean
       - in: query
+        name: show_sources
+        required: false
+        schema:
+          default: false
+          title: Show Sources
+          type: boolean
+      - in: query
         name: root_path
         required: false
         schema:
           default: false
           title: Root Path
           type: boolean
       responses:
@@ -1622,15 +1719,16 @@
             schema:
               $ref: '#/components/schemas/PutMetadataRequest'
         required: true
       responses:
         '200':
           content:
             application/json:
-              schema: {}
+              schema:
+                $ref: '#/components/schemas/PutMetadataResponse'
           description: Successful Response
         '422':
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/HTTPValidationError'
           description: Validation Error
@@ -1639,27 +1737,27 @@
         - write:metadata
       - APIKeyQuery: []
       - APIKeyAuthorizationHeader: []
       - APIKeyCookie: []
       summary: Put Metadata
   /api/v1/node/revisions/{path}:
     delete:
-      operationId: revisions_delitem_api_v1_node_revisions__path__delete
+      operationId: delete_revision_api_v1_node_revisions__path__delete
       parameters:
       - in: path
         name: path
         required: true
         schema:
           title: Path
           type: string
       - in: query
-        name: n
+        name: number
         required: true
         schema:
-          title: N
+          title: Number
           type: integer
       responses:
         '200':
           content:
             application/json:
               schema: {}
           description: Successful Response
@@ -1671,17 +1769,17 @@
           description: Validation Error
       security:
       - OAuth2PasswordBearer:
         - write:metadata
       - APIKeyQuery: []
       - APIKeyAuthorizationHeader: []
       - APIKeyCookie: []
-      summary: Revisions Delitem
+      summary: Delete Revision
     get:
-      operationId: node_revisions_api_v1_node_revisions__path__get
+      operationId: get_revisions_api_v1_node_revisions__path__get
       parameters:
       - in: path
         name: path
         required: true
         schema:
           title: Path
           type: string
@@ -1716,15 +1814,15 @@
           description: Validation Error
       security:
       - OAuth2PasswordBearer:
         - read:metadata
       - APIKeyQuery: []
       - APIKeyAuthorizationHeader: []
       - APIKeyCookie: []
-      summary: Node Revisions
+      summary: Get Revisions
   /api/v1/node/search/{path}:
     get:
       operationId: route_with_sig_api_v1_node_search__path__get
       parameters:
       - in: path
         name: path
         required: true
@@ -1741,14 +1839,15 @@
           - structure
           - structure.micro
           - structure.macro
           - count
           - sorting
           - specs
           - references
+          - data_sources
           - ''
           items:
             $ref: '#/components/schemas/EntryFields'
           type: array
       - in: query
         name: select_metadata
         required: false
@@ -1790,14 +1889,21 @@
         name: omit_links
         required: false
         schema:
           default: false
           title: Omit Links
           type: boolean
       - in: query
+        name: show_sources
+        required: false
+        schema:
+          default: false
+          title: Show Sources
+          type: boolean
+      - in: query
         name: filter[fulltext][condition][text]
         required: false
         schema:
           items:
             type: string
           title: Filter[Fulltext][Condition][Text]
           type: array
```

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.array.ArrayAdapter.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.array.ArrayAdapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.dataframe.DataFrameAdapter.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.dataframe.DataFrameAdapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.excel.ExcelAdapter.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.excel.ExcelAdapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.files.DirectoryAdapter.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.files.DirectoryAdapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.hdf5.HDF5Adapter.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.hdf5.HDF5Adapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.mapping.MapAdapter.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.mapping.MapAdapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.adapters.sparse.COOAdapter.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.adapters.sparse.COOAdapter.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.ArrayClient.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.client.array.ArrayClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.array.DaskArrayClient.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.client.array.DaskArrayClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.base.BaseClient.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.client.base.BaseClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.context.Context.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.client.context.Context.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.client.dataframe.DaskDataFrameClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.client.dataframe.DataFrameClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.sparse.SparseClient.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.client.sparse.SparseClient.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.xarray.DaskDatasetClient.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.client.xarray.DaskDatasetClient.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
    
    .. rubric:: Methods
 
    .. autosummary::
    
       ~DaskDatasetClient.__init__
+      ~DaskDatasetClient.create_node
       ~DaskDatasetClient.discover_clients_from_entrypoints
       ~DaskDatasetClient.distinct
       ~DaskDatasetClient.download
       ~DaskDatasetClient.export
       ~DaskDatasetClient.get
       ~DaskDatasetClient.items
       ~DaskDatasetClient.keys
```

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.client.xarray.DatasetClient.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.client.xarray.DatasetClient.rst`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
    
    .. rubric:: Methods
 
    .. autosummary::
    
       ~DatasetClient.__init__
+      ~DatasetClient.create_node
       ~DatasetClient.discover_clients_from_entrypoints
       ~DatasetClient.distinct
       ~DatasetClient.download
       ~DatasetClient.export
       ~DatasetClient.get
       ~DatasetClient.items
       ~DatasetClient.keys
```

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.media_type_registration.SerializationRegistry.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.server.object_cache.ObjectCache.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.ArrayMacroStructure.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.structures.array.ArrayMacroStructure.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.array.BuiltinDtype.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.structures.array.BuiltinDtype.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMacroStructure.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMacroStructure.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMicroStructure.rst` & `tiled-0.1.0a94/docs/source/reference/generated/tiled.structures.dataframe.DataFrameMicroStructure.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/reference/min-versions.rst` & `tiled-0.1.0a94/docs/source/reference/min-versions.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/docs/source/tutorials/installation.rst` & `tiled-0.1.0a94/docs/source/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/setup.py` & `tiled-0.1.0a94/setup.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/static/favicon.ico` & `tiled-0.1.0a94/share/tiled/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/templates/device_code_form.html` & `tiled-0.1.0a94/share/tiled/templates/device_code_form.html`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/templates/index.html` & `tiled-0.1.0a94/share/tiled/templates/index.html`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/asset-manifest.json` & `tiled-0.1.0a94/share/tiled/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/config/default.yml` & `tiled-0.1.0a94/share/tiled/ui/config/default.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/favicon.ico` & `tiled-0.1.0a94/share/tiled/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/index.html` & `tiled-0.1.0a94/share/tiled/ui/index.html`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/css/main.da25efef.css` & `tiled-0.1.0a94/share/tiled/ui/static/css/main.da25efef.css`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/css/main.da25efef.css.map` & `tiled-0.1.0a94/share/tiled/ui/static/css/main.da25efef.css.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/113.a6dabf86.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/113.a6dabf86.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/113.a6dabf86.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/113.a6dabf86.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/128.74bef542.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/128.74bef542.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/197.6f7f332e.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/197.6f7f332e.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/197.6f7f332e.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/197.6f7f332e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/214.2a10743e.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/214.2a10743e.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/214.2a10743e.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/214.2a10743e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/276.0058e750.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/276.0058e750.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/276.0058e750.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/276.0058e750.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/321.c6b9dcec.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/321.c6b9dcec.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/321.c6b9dcec.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/321.c6b9dcec.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/356.6a2946e1.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/356.6a2946e1.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/356.6a2946e1.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/356.6a2946e1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/393.73e08fb5.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/393.73e08fb5.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/393.73e08fb5.chunk.js.LICENSE.txt` & `tiled-0.1.0a94/share/tiled/ui/static/js/393.73e08fb5.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/393.73e08fb5.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/393.73e08fb5.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/446.ae1590fd.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/446.ae1590fd.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/446.ae1590fd.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/446.ae1590fd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/470.a78b4c62.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/470.a78b4c62.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/470.a78b4c62.chunk.js.LICENSE.txt` & `tiled-0.1.0a94/share/tiled/ui/static/js/470.a78b4c62.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/470.a78b4c62.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/470.a78b4c62.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/485.0ed51a45.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/485.0ed51a45.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/485.0ed51a45.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/485.0ed51a45.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/494.3371b974.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/494.3371b974.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/494.3371b974.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/494.3371b974.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/689.0cde4405.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/689.0cde4405.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/689.0cde4405.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/689.0cde4405.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/69.c379776e.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/69.c379776e.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/69.c379776e.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/69.c379776e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/705.eeca3f97.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/705.eeca3f97.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/705.eeca3f97.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/705.eeca3f97.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/741.fbe96b6d.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/741.fbe96b6d.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/741.fbe96b6d.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/741.fbe96b6d.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/773.590aa2f4.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/773.590aa2f4.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/773.590aa2f4.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/773.590aa2f4.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/787.54a97274.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/787.54a97274.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/787.54a97274.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/787.54a97274.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/837.22b95b21.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/837.22b95b21.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/837.22b95b21.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/837.22b95b21.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/858.2658cad8.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/858.2658cad8.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/858.2658cad8.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/858.2658cad8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/883.31ddd2ac.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/883.31ddd2ac.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/883.31ddd2ac.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/883.31ddd2ac.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/921.22e363f6.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/921.22e363f6.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/921.22e363f6.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/921.22e363f6.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/986.f5c9d7cf.chunk.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/main.5cc3eaa8.js` & `tiled-0.1.0a94/share/tiled/ui/static/js/main.5cc3eaa8.js`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/main.5cc3eaa8.js.LICENSE.txt` & `tiled-0.1.0a94/share/tiled/ui/static/js/main.5cc3eaa8.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/js/main.5cc3eaa8.js.map` & `tiled-0.1.0a94/share/tiled/ui/static/js/main.5cc3eaa8.js.map`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-300-normal.8fc5f5f22c9951113696.woff` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-all-300-normal.8fc5f5f22c9951113696.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-400-normal.376ea5d93f71583052f6.woff` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-all-400-normal.376ea5d93f71583052f6.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-500-normal.52cb737b682eb9661ee1.woff` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-all-500-normal.52cb737b682eb9661ee1.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-all-700-normal.ef6d1d09b20b877fee4e.woff` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-all-700-normal.ef6d1d09b20b877fee4e.woff`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-300-normal.48e4b37ecbc5e155460e.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-300-normal.48e4b37ecbc5e155460e.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-400-normal.5e493812deabd1d01e60.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-400-normal.5e493812deabd1d01e60.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-500-normal.d1615fb9cd7f67f5018c.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-500-normal.d1615fb9cd7f67f5018c.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-700-normal.0334efc0de1012200889.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-700-normal.0334efc0de1012200889.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-300-normal.12d37040a0160a948ff1.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-ext-300-normal.12d37040a0160a948ff1.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-400-normal.493afe7ae8ecfe268800.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-ext-400-normal.493afe7ae8ecfe268800.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-500-normal.3e748c93fe6a87bdedaa.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-ext-500-normal.3e748c93fe6a87bdedaa.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-cyrillic-ext-700-normal.b816cda3107bb21c87e1.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-cyrillic-ext-700-normal.b816cda3107bb21c87e1.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-300-normal.7c6b44c55d4d9661e3ed.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-300-normal.7c6b44c55d4d9661e3ed.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-400-normal.1cbfc636c911faa4d0ca.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-400-normal.1cbfc636c911faa4d0ca.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-500-normal.007ca18d2cbae7381b39.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-500-normal.007ca18d2cbae7381b39.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-700-normal.3292e831b18d0c23d609.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-700-normal.3292e831b18d0c23d609.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-300-normal.04e05839d6a35e046c13.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-ext-300-normal.04e05839d6a35e046c13.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-400-normal.bb723e8458c9c653e505.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-ext-400-normal.bb723e8458c9c653e505.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-500-normal.9c0d384f31e2c914edf3.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-ext-500-normal.9c0d384f31e2c914edf3.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-greek-ext-700-normal.9674bc0ae12c2551d9d1.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-greek-ext-700-normal.9674bc0ae12c2551d9d1.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-300-normal.0109a2ace896a506a0aa.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-300-normal.0109a2ace896a506a0aa.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-400-normal.4673b4537a84c7f7a130.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-400-normal.4673b4537a84c7f7a130.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-500-normal.869888415d0b1a99ae5c.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-500-normal.869888415d0b1a99ae5c.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-700-normal.0682ca7f74351d42bf73.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-700-normal.0682ca7f74351d42bf73.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-300-normal.a29236e0fc30e8482530.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-ext-300-normal.a29236e0fc30e8482530.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-400-normal.c3dcdbd5bb4d4af80817.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-ext-400-normal.c3dcdbd5bb4d4af80817.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-500-normal.feaff916fd609e310efe.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-ext-500-normal.feaff916fd609e310efe.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-latin-ext-700-normal.bcf37d666ce10b3556cd.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-latin-ext-700-normal.bcf37d666ce10b3556cd.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-300-normal.af9afdc10c93e4118e90.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-vietnamese-300-normal.af9afdc10c93e4118e90.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-400-normal.c0bec65d01f776c00c91.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-vietnamese-400-normal.c0bec65d01f776c00c91.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-500-normal.b8e494da1ec1f1824769.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-vietnamese-500-normal.b8e494da1ec1f1824769.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/share/tiled/ui/static/media/roboto-vietnamese-700-normal.3096f18acebc3f07020d.woff2` & `tiled-0.1.0a94/share/tiled/ui/static/media/roboto-vietnamese-700-normal.3096f18acebc3f07020d.woff2`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_access_control.py` & `tiled-0.1.0a94/tiled/_tests/test_access_control.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,55 +4,56 @@
 import numpy
 import pytest
 
 from ..adapters.array import ArrayAdapter
 from ..adapters.mapping import MapAdapter
 from ..client import Context, from_context
 from ..server.app import build_app_from_config
-from .utils import fail_with_status_code
-from .writable_adapters import WritableMapAdapter
+from .utils import enter_password, fail_with_status_code
 
-arr = ArrayAdapter.from_array(numpy.ones((5, 5)))
+arr = numpy.ones((5, 5))
+arr_ad = ArrayAdapter.from_array(arr)
 
 
 def tree_a(access_policy=None):
-    return MapAdapter({"A1": arr, "A2": arr}, access_policy=access_policy)
+    return MapAdapter({"A1": arr_ad, "A2": arr_ad}, access_policy=access_policy)
 
 
 def tree_b(access_policy=None):
-    return MapAdapter({"B1": arr, "B2": arr}, access_policy=access_policy)
-
-
-def writable_tree(access_policy=None):
-    return WritableMapAdapter({"A1": arr, "A2": arr}, access_policy=access_policy)
+    return MapAdapter({"B1": arr_ad, "B2": arr_ad}, access_policy=access_policy)
 
 
 @pytest.fixture(scope="module")
-def context():
+def context(tmpdir_module):
     config = {
         "authentication": {
             "secret_keys": ["SECRET"],
             "providers": [
                 {
                     "provider": "toy",
                     "authenticator": "tiled.authenticators:DictionaryAuthenticator",
                     "args": {
-                        "users_to_passwords": {"alice": "secret1", "bob": "secret2"}
+                        "users_to_passwords": {
+                            "alice": "secret1",
+                            "bob": "secret2",
+                            "admin": "admin",
+                        }
                     },
                 }
             ],
         },
         "database": {
             "uri": "sqlite+aiosqlite://",  # in-memory
         },
         "access_control": {
             "access_policy": "tiled.access_policies:SimpleAccessPolicy",
             "args": {
                 "access_lists": {"alice": ["a", "c", "d", "e"]},
                 "provider": "toy",
+                "admins": ["admin"],
             },
         },
         "trees": [
             {
                 "tree": f"{__name__}:tree_a",
                 "path": "/a",
                 "access_control": {
@@ -61,70 +62,83 @@
                         "provider": "toy",
                         "access_lists": {
                             "alice": ["A2"],
                             # This should have no effect because bob
                             # cannot access the parent node.
                             "bob": ["A1", "A2"],
                         },
+                        "admins": ["admin"],
                     },
                 },
             },
             {"tree": f"{__name__}:tree_b", "path": "/b", "access_policy": None},
             {
-                "tree": f"{__name__}:writable_tree",
+                "tree": "tiled.catalog:in_memory",
+                "args": {"writable_storage": tmpdir_module / "c"},
                 "path": "/c",
                 "access_control": {
                     "access_policy": "tiled.access_policies:SimpleAccessPolicy",
                     "args": {
                         "provider": "toy",
                         "access_lists": {
-                            "alice": "tiled.access_policies:SimpleAccessPolicy.ALL",
+                            "alice": "tiled.access_policies:ALL_ACCESS",
                         },
+                        "admins": ["admin"],
                     },
                 },
             },
             {
-                "tree": f"{__name__}:writable_tree",
+                "tree": "tiled.catalog:in_memory",
+                "args": {"writable_storage": tmpdir_module / "d"},
                 "path": "/d",
                 "access_control": {
                     "access_policy": "tiled.access_policies:SimpleAccessPolicy",
                     "args": {
                         "provider": "toy",
                         "access_lists": {
-                            "alice": "tiled.access_policies:SimpleAccessPolicy.ALL",
+                            "alice": "tiled.access_policies:ALL_ACCESS",
                         },
+                        "admins": ["admin"],
                         # Block writing.
                         "scopes": ["read:metadata", "read:data"],
                     },
                 },
             },
             {
-                "tree": f"{__name__}:writable_tree",
+                "tree": "tiled.catalog:in_memory",
+                "args": {"writable_storage": tmpdir_module / "e"},
                 "path": "/e",
                 "access_control": {
                     "access_policy": "tiled.access_policies:SimpleAccessPolicy",
                     "args": {
                         "provider": "toy",
                         "access_lists": {
-                            "alice": "tiled.access_policies:SimpleAccessPolicy.ALL",
+                            "alice": "tiled.access_policies:ALL_ACCESS",
                         },
+                        "admins": ["admin"],
                         # Block creation.
                         "scopes": [
                             "read:metadata",
                             "read:data",
                             "write:metadata",
                             "write:data",
                         ],
                     },
                 },
             },
         ],
     }
     app = build_app_from_config(config)
     with Context.from_app(app) as context:
+        with enter_password("admin"):
+            admin_client = from_context(context, username="admin")
+            for k in ["c", "d", "e"]:
+                admin_client[k].write_array(arr, key="A1")
+                admin_client[k].write_array(arr, key="A2")
+                admin_client[k].write_array(arr, key="x")
         yield context
 
 
 def test_top_level_access_control(context, enter_password):
     with enter_password("secret1"):
         alice_client = from_context(context, username="alice")
     assert "a" in alice_client
@@ -177,28 +191,28 @@
 
 
 def test_create_and_update_allowed(enter_password, context):
     with enter_password("secret1"):
         alice_client = from_context(context, username="alice")
 
     # Update
-    alice_client["c"].metadata
-    alice_client["c"].update_metadata(metadata={"added_key": 3})
-    assert alice_client["c"].metadata["added_key"] == 3
+    alice_client["c"]["x"].metadata
+    alice_client["c"]["x"].update_metadata(metadata={"added_key": 3})
+    assert alice_client["c"]["x"].metadata["added_key"] == 3
 
     # Create
     alice_client["c"].write_array([1, 2, 3])
 
 
 def test_writing_blocked_by_access_policy(enter_password, context):
     with enter_password("secret1"):
         alice_client = from_context(context, username="alice")
-    alice_client["d"].metadata
+    alice_client["d"]["x"].metadata
     with fail_with_status_code(403):
-        alice_client["d"].update_metadata(metadata={"added_key": 3})
+        alice_client["d"]["x"].update_metadata(metadata={"added_key": 3})
 
 
 def test_create_blocked_by_access_policy(enter_password, context):
     with enter_password("secret1"):
         alice_client = from_context(context, username="alice")
     with fail_with_status_code(403):
         alice_client["e"].write_array([1, 2, 3])
```

### Comparing `tiled-0.1.0a93/tiled/_tests/test_allow_origins.py` & `tiled-0.1.0a94/tiled/_tests/test_allow_origins.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_array.py` & `tiled-0.1.0a94/tiled/_tests/test_array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_authentication.py` & `tiled-0.1.0a94/tiled/_tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_authenticators.py` & `tiled-0.1.0a94/tiled/_tests/test_authenticators.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_caches.py` & `tiled-0.1.0a94/tiled/_tests/test_caches.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_client.py` & `tiled-0.1.0a94/tiled/_tests/test_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         load_profiles.cache_clear()
         with pytest.raises(ConfigError):
             from_profile("test")
     finally:
         paths.remove(profile_dir)
 
 
+@pytest.mark.xfail(reason="Change in pytest behavior regarding output capturing")
 def test_stdin_closed(monkeypatch):
     "When stdin is closed do not prompt for authentication."
     # https://github.com/bluesky/tiled/pull/427
     __stdin__ = types.SimpleNamespace(closed=True)
     monkeypatch.setattr(sys, "__stdin__", __stdin__)
     config = {
         "authentication": {
```

### Comparing `tiled-0.1.0a93/tiled/_tests/test_client_cache.py` & `tiled-0.1.0a94/tiled/_tests/test_client_cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_config.py` & `tiled-0.1.0a94/tiled/_tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_custom_format.py` & `tiled-0.1.0a94/tiled/_tests/test_custom_format.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_dataframe.py` & `tiled-0.1.0a94/tiled/_tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_directory_walker.py` & `tiled-0.1.0a94/tiled/_tests/test_directory_walker.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_distinct.py` & `tiled-0.1.0a94/tiled/_tests/test_distinct.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_export.py` & `tiled-0.1.0a94/tiled/_tests/test_export.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_hdf5.py` & `tiled-0.1.0a94/tiled/_tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_history.py` & `tiled-0.1.0a94/tiled/_tests/test_history.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_import_object.py` & `tiled-0.1.0a94/tiled/_tests/test_import_object.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_indexers.py` & `tiled-0.1.0a94/tiled/_tests/test_indexers.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_inlined_contents.py` & `tiled-0.1.0a94/tiled/_tests/test_inlined_contents.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_json.py` & `tiled-0.1.0a94/tiled/_tests/test_json.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_metrics.py` & `tiled-0.1.0a94/tiled/_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_object_cache.py` & `tiled-0.1.0a94/tiled/_tests/test_object_cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_openapi.py` & `tiled-0.1.0a94/tiled/_tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_pickle.py` & `tiled-0.1.0a94/tiled/_tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_queries.py` & `tiled-0.1.0a94/tiled/_tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_scaled_config_option.py` & `tiled-0.1.0a94/tiled/_tests/test_scaled_config_option.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_search.py` & `tiled-0.1.0a94/tiled/_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_size_limit.py` & `tiled-0.1.0a94/tiled/_tests/test_size_limit.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_sort.py` & `tiled-0.1.0a94/tiled/_tests/test_sort.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_sparse.py` & `tiled-0.1.0a94/tiled/_tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_specs_and_references.py` & `tiled-0.1.0a94/tiled/_tests/test_specs_and_references.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_structured_array.py` & `tiled-0.1.0a94/tiled/_tests/test_structured_array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_tiff.py` & `tiled-0.1.0a94/tiled/_tests/test_tiff.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/_tests/test_validation.py` & `tiled-0.1.0a94/tiled/_tests/test_validation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 This tests tiled's validation registry
 """
 
 import numpy as np
 import pandas as pd
+import pytest
 
 from ..client import Context, from_context
 from ..config import merge
 from ..server.app import build_app_from_config
 from ..validation_registration import ValidationError
 from .utils import fail_with_status_code
-from .writable_adapters import WritableMapAdapter
 
 
 def lower_case_dict(d):
     out = {}
     modified = False
 
     for k, v in d.items():
@@ -39,84 +39,95 @@
     if "foo" not in metadata:
         raise ValidationError("metadata for spec {spec} must contain foo")
 
     if metadata_modified:
         return metadata
 
 
-tree = WritableMapAdapter({})
-
-
-def test_validators():
+@pytest.fixture(scope="module")
+def client(tmpdir_module):
     config = {
-        "trees": [{"tree": f"{__name__}:tree", "path": "/"}],
-        "specs": [{"spec": "foo", "validator": f"{__name__}:validate_foo"}],
+        "trees": [
+            {
+                "tree": "tiled.catalog:in_memory",
+                "path": "/",
+                "args": {"writable_storage": tmpdir_module},
+            },
+        ],
+        "specs": [
+            {"spec": "foo", "validator": f"{__name__}:validate_foo"},
+            {"spec": "a"},
+        ],
     }
     # Check that specs propagate correctly through merging configs.
     merged_config = merge({"filepath_placeholder": config})
     assert merged_config["specs"]
     with Context.from_app(build_app_from_config(merged_config)) as context:
-        client = from_context(context)
+        yield from_context(context)
 
-        # valid example
-        df = pd.DataFrame({"a": np.zeros(10), "b": np.zeros(10)})
-        client.write_dataframe(df, metadata={"foo": 1}, specs=["foo"])
 
-        with fail_with_status_code(400):
-            # not expected structure family
-            a = np.ones((5, 7))
-            client.write_array(a, metadata={}, specs=["foo"])
+def test_validators(client):
+    # valid example
+    df = pd.DataFrame({"a": np.zeros(10), "b": np.zeros(10)})
+    client.write_dataframe(df, metadata={"foo": 1}, specs=["foo"])
 
-        with fail_with_status_code(400):
-            # column names are not expected
-            df = pd.DataFrame({"x": np.zeros(10), "y": np.zeros(10)})
-            client.write_dataframe(df, metadata={}, specs=["foo"])
+    with fail_with_status_code(400):
+        # not expected structure family
+        a = np.ones((5, 7))
+        client.write_array(a, metadata={}, specs=["foo"])
 
-        with fail_with_status_code(400):
-            # missing expected metadata
-            df = pd.DataFrame({"a": np.zeros(10), "b": np.zeros(10)})
-            client.write_dataframe(df, metadata={}, specs=["foo"])
+    with fail_with_status_code(400):
+        # column names are not expected
+        df = pd.DataFrame({"x": np.zeros(10), "y": np.zeros(10)})
+        client.write_dataframe(df, metadata={}, specs=["foo"])
 
-        metadata = {"id": 1, "foo": "bar"}
+    with fail_with_status_code(400):
+        # missing expected metadata
         df = pd.DataFrame({"a": np.zeros(10), "b": np.zeros(10)})
-        result = client.write_dataframe(df, metadata=metadata, specs=["foo"])
-        assert result.metadata == metadata
-        result_df = result.read()
-        pd.testing.assert_frame_equal(result_df, df)
-
-        metadata_upper = {"ID": 2, "FOO": "bar"}
-        metadata_lower, _ = lower_case_dict(metadata_upper)
-        result = client.write_dataframe(df, metadata=metadata_upper, specs=["foo"])
-        assert result.metadata == metadata_lower
-        result_df = result.read()
-        pd.testing.assert_frame_equal(result_df, df)
+        client.write_dataframe(df, metadata={}, specs=["foo"])
 
+    metadata = {"id": 1, "foo": "bar"}
+    df = pd.DataFrame({"a": np.zeros(10), "b": np.zeros(10)})
+    result = client.write_dataframe(df, metadata=metadata, specs=["foo"])
+    assert result.metadata == metadata
+    result_df = result.read()
+    pd.testing.assert_frame_equal(result_df, df)
+
+    metadata_upper = {"ID": 2, "FOO": "bar"}
+    metadata_lower, _ = lower_case_dict(metadata_upper)
+    result = client.write_dataframe(df, metadata=metadata_upper, specs=["foo"])
+    assert result.metadata == metadata_lower
+    result_df = result.read()
+    pd.testing.assert_frame_equal(result_df, df)
 
-def test_unknown_spec_strict():
+
+def test_unknown_spec_strict(tmpdir):
     "Test unknown spec rejected for upload."
     config = {
-        "trees": [{"tree": f"{__name__}:tree", "path": "/"}],
-        "specs": [{"spec": "a"}],
+        "trees": [
+            {
+                "tree": "tiled.catalog:in_memory",
+                "path": "/",
+                "args": {"writable_storage": tmpdir},
+            },
+        ],
+        "specs": [
+            {"spec": "a"},
+        ],
         "reject_undeclared_specs": True,
     }
+    # Check that specs propagate correctly through merging configs.
     with Context.from_app(build_app_from_config(config)) as context:
         client = from_context(context)
         a = np.ones((5, 7))
         client.write_array(a, metadata={}, specs=["a"])
         with fail_with_status_code(400):
             # unknown spec 'b' should be rejected
             client.write_array(a, metadata={}, specs=["b"])
 
 
-def test_unknown_spec_permissive():
+def test_unknown_spec_permissive(client):
     "Test unknown spec rejected for upload."
-    config = {
-        "trees": [{"tree": f"{__name__}:tree", "path": "/"}],
-        "specs": [{"spec": "a"}],
-        #  "reject_undeclared_specs": false,  # the default
-    }
-    with Context.from_app(build_app_from_config(config)) as context:
-        client = from_context(context)
-        a = np.ones((5, 7))
-        client.write_array(a, metadata={}, specs=["a"])
-        # unknown spec 'b' should be accepted
-        client.write_array(a, metadata={}, specs=["b"])
+    a = np.ones((5, 7))
+    client.write_array(a, metadata={}, specs=["a"])
+    # unknown spec 'b' should be accepted
+    client.write_array(a, metadata={}, specs=["b"])
```

### Comparing `tiled-0.1.0a93/tiled/_tests/test_writing.py` & `tiled-0.1.0a94/tiled/_tests/test_writing.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,31 +3,36 @@
 
 Persistent stores are being developed externally to the tiled package.
 """
 
 import dask.dataframe
 import numpy
 import pandas.testing
+import pytest
 import sparse
 
+from ..catalog import in_memory
 from ..client import Context, from_context, record_history
 from ..queries import Key
 from ..server.app import build_app
 from ..structures.core import Spec
 from ..structures.sparse import COOStructure
 from ..validation_registration import ValidationRegistry
 from .utils import fail_with_status_code
-from .writable_adapters import WritableMapAdapter
 
 validation_registry = ValidationRegistry()
 validation_registry.register("SomeSpec", lambda *args, **kwargs: None)
 
 
-def test_write_array_full():
-    tree = WritableMapAdapter({})
+@pytest.fixture
+def tree(tmpdir):
+    return in_memory(writable_storage=tmpdir)
+
+
+def test_write_array_full(tree):
     with Context.from_app(
         build_app(tree, validation_registry=validation_registry)
     ) as context:
         client = from_context(context)
 
         a = numpy.ones((5, 7))
 
@@ -45,18 +50,16 @@
 
         numpy.testing.assert_equal(result_array, a)
         assert result.metadata == metadata
         assert result.specs == specs
         assert result.references == references
 
 
-def test_write_large_array_full():
+def test_write_large_array_full(tree):
     "Test that a large array is chunked"
-
-    tree = WritableMapAdapter({})
     with Context.from_app(
         build_app(tree, validation_registry=validation_registry)
     ) as context:
         client = from_context(context)
 
         a = numpy.ones(100, dtype=numpy.uint8)
         # Low the limit so we can test on small data, for speed.
@@ -81,16 +84,15 @@
             assert result.metadata == metadata
             assert result.specs == specs
             assert result.references == references
         finally:
             client._SUGGESTED_MAX_UPLOAD_SIZE = original
 
 
-def test_write_array_chunked():
-    tree = WritableMapAdapter({})
+def test_write_array_chunked(tree):
     with Context.from_app(
         build_app(tree, validation_registry=validation_registry)
     ) as context:
         client = from_context(context)
 
         a = dask.array.arange(1500).reshape((50, 30)).rechunk((20, 15))
 
@@ -108,16 +110,15 @@
 
         numpy.testing.assert_equal(result_array, a.compute())
         assert result.metadata == metadata
         assert result.specs == specs
         assert result.references == references
 
 
-def test_write_dataframe_full():
-    tree = WritableMapAdapter({})
+def test_write_dataframe_full(tree):
     with Context.from_app(
         build_app(tree, validation_registry=validation_registry)
     ) as context:
         client = from_context(context)
 
         data = {f"Column{i}": (1 + i) * numpy.ones(5) for i in range(5)}
         df = pandas.DataFrame(data)
@@ -138,16 +139,15 @@
 
         pandas.testing.assert_frame_equal(result_dataframe, df)
         assert result.metadata == metadata
         assert result.specs == specs
         assert result.references == references
 
 
-def test_write_dataframe_partitioned():
-    tree = WritableMapAdapter({})
+def test_write_dataframe_partitioned(tree):
     with Context.from_app(
         build_app(tree, validation_registry=validation_registry)
     ) as context:
         client = from_context(context)
 
         data = {f"Column{i}": (1 + i) * numpy.ones(10) for i in range(5)}
         df = pandas.DataFrame(data)
@@ -169,16 +169,15 @@
 
         pandas.testing.assert_frame_equal(result_dataframe, df)
         assert result.metadata == metadata
         assert result.specs == specs
         assert result.references == references
 
 
-def test_write_sparse_full():
-    tree = WritableMapAdapter({})
+def test_write_sparse_full(tree):
     with Context.from_app(
         build_app(tree, validation_registry=validation_registry)
     ) as context:
         client = from_context(context)
 
         coo = sparse.COO(coords=[[0, 1], [2, 3]], data=[3.8, 4.0], shape=(4, 4))
 
@@ -203,16 +202,15 @@
 
         numpy.testing.assert_equal(result_array.todense(), coo.todense())
         assert result.metadata == metadata
         assert result.specs == specs
         assert result.references == references
 
 
-def test_write_sparse_chunked():
-    tree = WritableMapAdapter({})
+def test_write_sparse_chunked(tree):
     with Context.from_app(
         build_app(tree, validation_registry=validation_registry)
     ) as context:
         client = from_context(context)
 
         metadata = {"scan_id": 1, "method": "A"}
         specs = [Spec("SomeSpec")]
@@ -244,23 +242,22 @@
 
         # numpy.testing.assert_equal(result_array, sparse.COO(coords=[0, 1, ]))
         assert result.metadata == metadata
         assert result.specs == specs
         assert result.references == references
 
 
-def test_limits():
+def test_limits(tree):
     "Test various limits on uploaded metadata."
 
     MAX_ALLOWED_SPECS = 20
     MAX_SPEC_CHARS = 255
     MAX_ALLOWED_REFERENCES = 20
     MAX_LABEL_CHARS = 255
 
-    tree = WritableMapAdapter({})
     validation_registry = ValidationRegistry()
     for i in range(101):
         validation_registry.register(f"spec{i}", lambda *args, **kwargs: None)
     validation_registry.register("one_too_many", lambda *args, **kwargs: None)
     validation_registry.register("a" * MAX_SPEC_CHARS, lambda *args, **kwargs: None)
     validation_registry.register(
         "a" * (1 + MAX_SPEC_CHARS), lambda *args, **kwargs: None
@@ -321,7 +318,26 @@
         with fail_with_status_code(422):
             client.write_array(
                 [1, 2, 3],
                 references=[{"label": too_many_chars, "url": "https://example.com"}],
             )
         with fail_with_status_code(422):
             y.update_metadata(references=too_many_chars)
+
+
+def test_metadata_revisions(tree):
+    with Context.from_app(build_app(tree)) as context:
+        client = from_context(context)
+        ac = client.write_array([1, 2, 3], key="revise_me")
+        assert len(ac.metadata_revisions[:]) == 0
+        ac.update_metadata(metadata={"a": 1})
+        assert ac.metadata["a"] == 1
+        client["revise_me"].metadata["a"] == 1
+        assert len(ac.metadata_revisions[:]) == 1
+        ac.update_metadata(metadata={"a": 2})
+        assert ac.metadata["a"] == 2
+        client["revise_me"].metadata["a"] == 2
+        assert len(ac.metadata_revisions[:]) == 2
+        ac.metadata_revisions.delete_revision(1)
+        assert len(ac.metadata_revisions[:]) == 1
+        with fail_with_status_code(404):
+            ac.metadata_revisions.delete_revision(1)
```

### Comparing `tiled-0.1.0a93/tiled/_tests/test_xarray.py` & `tiled-0.1.0a94/tiled/_tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/access_policies.py` & `tiled-0.1.0a94/tiled/access_policies.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,36 @@
 
     def filters(self, node, principal, scopes):
         return []
 
 
 class SimpleAccessPolicy:
     """
-    A mapping of user names to lists of entries they have full access.
+    A mapping of user names to lists of entries they have access to.
 
     This simple policy does not provide fine-grained control of scopes.
+    Any restriction on scopes is applied the same to all users, except
+    for an optional list of 'admins'.
+
+    This is used in the test suite; it may be suitable for very simple
+    deployments.
 
     >>> SimpleAccessPolicy({"alice": ["A", "B"], "bob": ["B"]}, provider="toy")
     """
 
     ALL = ALL_ACCESS
 
-    def __init__(self, access_lists, *, provider, scopes=None, public=None):
+    def __init__(
+        self, access_lists, *, provider, scopes=None, public=None, admins=None
+    ):
         self.access_lists = {}
         self.provider = provider
         self.scopes = scopes if (scopes is not None) else ALL_SCOPES
         self.public = set(public or [])
+        self.admins = set(admins or [])
         for key, value in access_lists.items():
             if isinstance(value, str):
                 value = import_object(value)
             self.access_lists[key] = value
 
     def _get_id(self, principal):
         # Get the id (i.e. username) of this Principal for the
@@ -49,25 +57,29 @@
             raise ValueError(
                 f"Principcal {principal} has no identity from provider {self.provider}. "
                 f"Its identities are: {principal.identities}"
             )
         return id
 
     def allowed_scopes(self, node, principal):
+        if self._get_id(principal) in self.admins:
+            return ALL_SCOPES
         # The simple policy does not provide for different Principals to
         # have different scopes on different Nodes. If the Principal has access,
         # they have the same hard-coded access everywhere.
         return self.scopes
 
     def filters(self, node, principal, scopes):
+        id = self._get_id(principal)
+        queries = []
+        if id in self.admins:
+            return queries
         if not scopes.issubset(self.scopes):
             return NO_ACCESS
-        id = self._get_id(principal)
         access_list = self.access_lists.get(id, [])
-        queries = []
         if not ((principal is SpecialUsers.admin) or (access_list == self.ALL)):
             try:
                 allowed = set(access_list or [])
             except TypeError:
                 # Provide rich debugging info because we have encountered a confusing
                 # bug here in a previous implementation.
                 raise TypeError(
```

### Comparing `tiled-0.1.0a93/tiled/adapters/array.py` & `tiled-0.1.0a94/tiled/adapters/array.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,30 +24,38 @@
 
     structure_family = "array"
 
     def __init__(
         self,
         array,
         *,
+        shape=None,
         chunks=None,
         metadata=None,
         dims=None,
         specs=None,
         references=None,
     ):
+        # Why would shape ever be different from array.shape, you ask?
+        # Some formats (notably Zarr) force shape to be a multiple of
+        # a chunk size, such that array.shape may include a margin beyond the
+        # actual data.
+        if shape is None:
+            shape = array.shape
+        self._shape = shape
         if chunks is None:
             if hasattr(array, "chunks"):
                 chunks = array.chunks  # might be None
             else:
                 chunks = None
             if chunks is None:
-                chunks = ("auto",) * len(array.shape)
+                chunks = ("auto",) * len(shape)
         self._chunks = normalize_chunks(
             chunks,
-            shape=array.shape,
+            shape=shape,
             dtype=array.dtype,
         )
         self._array = array
         self._metadata = metadata or {}
         self._dims = dims
         self.specs = specs or []
         self.references = references or []
@@ -78,15 +86,15 @@
     @property
     def metadata(self):
         return DictView(self._metadata)
 
     def macrostructure(self):
         "Structures of the layout of blocks of this array"
         return ArrayMacroStructure(
-            shape=self._array.shape, chunks=self._chunks, dims=self._dims
+            shape=self._shape, chunks=self._chunks, dims=self._dims
         )
 
     def microstructure(self):
         "Internal structure of a block of this array --- i.e. its data type"
         if self._array.dtype.fields is not None:
             micro = StructDtype.from_numpy_dtype(self._array.dtype)
         else:
```

### Comparing `tiled-0.1.0a93/tiled/adapters/dataframe.py` & `tiled-0.1.0a94/tiled/adapters/dataframe.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,24 @@
             ddf.divisions,
             metadata=metadata,
             specs=specs,
             references=references,
         )
 
     @classmethod
-    def read_csv(cls, *args, metadata=None, specs=None, references=None, **kwargs):
+    def read_csv(
+        cls,
+        *args,
+        metadata=None,
+        meta=None,
+        divisions=None,
+        specs=None,
+        references=None,
+        **kwargs,
+    ):
         """
         Read a CSV.
 
         Internally, this uses dask.dataframe.read_csv.
         It forward all parameters to that function. See
         https://docs.dask.org/en/latest/dataframe-api.html#dask.dataframe.read_csv
```

### Comparing `tiled-0.1.0a93/tiled/adapters/excel.py` & `tiled-0.1.0a94/tiled/adapters/excel.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/adapters/files.py` & `tiled-0.1.0a94/tiled/adapters/files.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/adapters/hdf5.py` & `tiled-0.1.0a94/tiled/adapters/hdf5.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,20 +46,14 @@
     >>> HDF5Adapter(file["some_group']["some_sub_group"])
 
     """
 
     structure_family = "node"
 
     def __init__(self, node, *, specs=None, references=None, access_policy=None):
-        if (access_policy is not None) and (
-            not access_policy.check_compatibility(self)
-        ):
-            raise ValueError(
-                f"Access policy {access_policy} is not compatible with this Tree."
-            )
         self._node = node
         self._access_policy = access_policy
         self.specs = specs or []
         self.references = references or []
         super().__init__()
 
     @classmethod
```

### Comparing `tiled-0.1.0a93/tiled/adapters/mapping.py` & `tiled-0.1.0a94/tiled/adapters/mapping.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/adapters/sparse.py` & `tiled-0.1.0a94/tiled/adapters/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/adapters/tiff.py` & `tiled-0.1.0a94/tiled/adapters/tiff.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     --------
 
     >>> TiffAdapter("path/to/file.tiff")
     """
 
     structure_family = "array"
 
-    def __init__(self, path, *, specs=None, references=None):
+    def __init__(self, path, *, shape=None, chunks=None, specs=None, references=None):
         self._file = tifffile.TiffFile(path)
         self._cache_key = (type(self).__module__, type(self).__qualname__, path)
         self.specs = specs or []
         self.references = references or []
 
     @property
     def metadata(self):
```

### Comparing `tiled-0.1.0a93/tiled/adapters/utils.py` & `tiled-0.1.0a94/tiled/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/adapters/xarray.py` & `tiled-0.1.0a94/tiled/adapters/xarray.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/authenticators.py` & `tiled-0.1.0a94/tiled/authenticators.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/client/_testclient.py` & `tiled-0.1.0a94/tiled/client/_testclient.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/client/array.py` & `tiled-0.1.0a94/tiled/client/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/client/auth.py` & `tiled-0.1.0a94/tiled/client/auth.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/client/base.py` & `tiled-0.1.0a94/tiled/client/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                 else:
                     result["data"].append(content["data"])
                 next_page = content["links"]["next"]
 
             return result["data"]
 
     def delete_revision(self, n):
-        self.context.delete_content(self._link, None, params={"n": n})
+        self.context.delete_content(self._link, None, params={"number": n})
 
 
 class BaseClient:
     def __init__(self, context, *, item, structure_clients):
         self._context = context
         self._item = item
         self._cached_len = None  # a cache just for __len__
```

### Comparing `tiled-0.1.0a93/tiled/client/cache.py` & `tiled-0.1.0a94/tiled/client/cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/client/constructors.py` & `tiled-0.1.0a94/tiled/client/constructors.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/client/context.py` & `tiled-0.1.0a94/tiled/client/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -594,25 +594,26 @@
         return msgpack.unpackb(
             self.get_content(
                 path, accept="application/x-msgpack", stream=stream, **kwargs
             ),
             timestamp=3,  # Decode msgpack Timestamp as datetime.datetime object.
         )
 
-    def post_json(self, path, content):
+    def post_json(self, path, content, params=None):
         request = self.http_client.build_request(
             "POST",
             path,
             json=content,
             # Submit CSRF token in both header and cookie.
             # https://cheatsheetseries.owasp.org/cheatsheets/Cross-Site_Request_Forgery_Prevention_Cheat_Sheet.html#double-submit-cookie
             headers={
                 "x-csrf": self.http_client.cookies["tiled_csrf"],
                 "accept": "application/x-msgpack",
             },
+            params=params,
         )
         response = self.http_client.send(request)
         handle_error(response)
         return msgpack.unpackb(
             response.content,
             timestamp=3,  # Decode msgpack Timestamp as datetime.datetime object.
         )
```

### Comparing `tiled-0.1.0a93/tiled/client/dataframe.py` & `tiled-0.1.0a94/tiled/client/dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/client/node.py` & `tiled-0.1.0a94/tiled/client/node.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,18 +70,14 @@
         structure_clients,
         queries=None,
         sorting=None,
         structure=None,
     ):
         "This is not user-facing. Use Node.from_uri."
 
-        if structure is not None:
-            # Node accepts 'structure' param for API compatibility with other clients,
-            # but it should always be None.
-            raise ValueError(f"Node received unexpected structure: {structure}")
         self.structure_clients = structure_clients
         self._queries = list(queries or [])
         self._queries_as_params = _queries_to_params(*self._queries)
         # If the user has not specified a sorting, give the server the opportunity
         # to tell us the default sorting.
         if sorting:
             self._sorting = sorting
@@ -551,59 +547,82 @@
             else:
                 return list(self)
         except Exception:
             # Do not print messy traceback from thread. Just fail silently.
             return []
 
     def new(
-        self, structure_family, structure, *, metadata=None, specs=None, references=None
+        self,
+        structure_family,
+        structure,
+        *,
+        key=None,
+        metadata=None,
+        specs=None,
+        references=None,
     ):
         """
         Create a new item within this Node.
 
         This is a low-level method. See high-level convenience methods listed below.
 
         See Also
         --------
         write_array
         write_dataframe
         write_coo_array
         """
+        self._cached_len = None
         metadata = metadata or {}
         specs = specs or []
         normalized_specs = []
         for spec in specs:
             if isinstance(spec, str):
                 spec = Spec(spec)
             normalized_specs.append(asdict(spec))
         references = references or []
+        data_sources = []
+        if structure_family != StructureFamily.node:
+            # TODO Handle multiple data sources.
+            data_sources.append({"structure": asdict(structure)})
         item = {
             "attributes": {
                 "metadata": metadata,
-                "structure": asdict(structure),
                 "structure_family": StructureFamily(structure_family),
                 "specs": normalized_specs,
                 "references": references,
+                "data_sources": data_sources,
             }
         }
 
         if structure_family == StructureFamily.dataframe:
             # send bytes base64 encoded
-            item["attributes"]["structure"]["micro"]["meta"] = base64.b64encode(
-                item["attributes"]["structure"]["micro"]["meta"]
+            item["attributes"]["data_sources"][0]["structure"]["micro"][
+                "meta"
+            ] = base64.b64encode(
+                item["attributes"]["data_sources"][0]["structure"]["micro"]["meta"]
             ).decode()
-            item["attributes"]["structure"]["micro"]["divisions"] = base64.b64encode(
-                item["attributes"]["structure"]["micro"]["divisions"]
+            item["attributes"]["data_sources"][0]["structure"]["micro"][
+                "divisions"
+            ] = base64.b64encode(
+                item["attributes"]["data_sources"][0]["structure"]["micro"]["divisions"]
             ).decode()
 
-        document = self.context.post_json(self.uri, item["attributes"])
+        body = dict(item["attributes"])
+        if key is not None:
+            body["id"] = key
+        document = self.context.post_json(self.uri, body)
+        item["attributes"]["structure"] = structure
 
         # if server returned modified metadata update the local copy
         if "metadata" in document:
             item["attributes"]["metadata"] = document.pop("metadata")
+        # Ditto for structure
+        if "structure" in document:
+            item["attributes"]["structure"] = document.pop("structure")
 
         # Merge in "id" and "links" returned by the server.
         item.update(document)
 
         return client_for_item(
             self.context,
             self.structure_clients,
@@ -611,21 +630,58 @@
             structure=structure,
         )
 
     # When (re)chunking arrays for upload, we use this limit
     # to attempt to avoid bumping into size limits.
     _SUGGESTED_MAX_UPLOAD_SIZE = 100_000_000  # 100 MB
 
-    def write_array(self, array, metadata=None, dims=None, specs=None, references=None):
+    def create_node(
+        self, key=None, *, metadata=None, dims=None, specs=None, references=None
+    ):
+        """
+        EXPERIMENTAL: Write an array.
+
+        Parameters
+        ----------
+        key : str, optional
+            Key (name) for this new node. If None, the server will provide a unique key.
+        metadata : dict, optional
+            User metadata. May be nested. Must contain only basic types
+            (e.g. numbers, strings, lists, dicts) that are JSON-serializable.
+        dims : List[str], optional
+            A label for each dimension of the array.
+        specs : List[Spec], optional
+            List of names that are used to label that the data and/or metadata
+            conform to some named standard specification.
+        references : List[Dict[str, URL]], optional
+            References (e.g. links) to related information. This may include
+            links into other Tiled data sets, search results, or external
+            resources unrelated to Tiled.
+
+        """
+        return self.new(
+            StructureFamily.node,
+            {"contents": None, "count": None},
+            key=key,
+            metadata=metadata,
+            specs=specs,
+            references=references,
+        )
+
+    def write_array(
+        self, array, *, key=None, metadata=None, dims=None, specs=None, references=None
+    ):
         """
         EXPERIMENTAL: Write an array.
 
         Parameters
         ----------
         array : array-like
+        key : str, optional
+            Key (name) for this new node. If None, the server will provide a unique key.
         metadata : dict, optional
             User metadata. May be nested. Must contain only basic types
             (e.g. numbers, strings, lists, dicts) that are JSON-serializable.
         dims : List[str], optional
             A label for each dimension of the array.
         specs : List[Spec], optional
             List of names that are used to label that the data and/or metadata
@@ -638,15 +694,14 @@
         """
         import dask.array
         import numpy
         from dask.array.core import normalize_chunks
 
         from ..structures.array import ArrayMacroStructure, ArrayStructure, BuiltinDtype
 
-        self._cached_len = None
         if not (hasattr(array, "shape") and hasattr(array, "dtype")):
             # This does not implement enough of the array-like interface.
             # Coerce to numpy.
             array = numpy.asarray(array)
 
         # Determine chunks such that each chunk is not too large to upload.
         # Any existing chunking will be taken into account.
@@ -673,14 +728,15 @@
                 dims=dims,
             ),
             micro=BuiltinDtype.from_numpy_dtype(array.dtype),
         )
         client = self.new(
             StructureFamily.array,
             structure,
+            key=key,
             metadata=metadata,
             specs=specs,
             references=references,
         )
         chunked = any(len(dim) > 1 for dim in chunks)
         if not chunked:
             client.write(array)
@@ -701,19 +757,48 @@
 
             # TODO Is there a fire-and-forget analogue such that we don't need
             # to bother with the return type?
             da.map_blocks(write_block, dtype=da.dtype, client=client).compute()
         return client
 
     def write_sparse(
-        self, coords, data, shape, metadata=None, dims=None, specs=None, references=None
+        self,
+        coords,
+        data,
+        shape,
+        *,
+        key=None,
+        metadata=None,
+        dims=None,
+        specs=None,
+        references=None,
     ):
         """
         EXPERIMENTAL: Write a sparse array.
 
+        Parameters
+        ----------
+        coords : array-like
+        data : array-like
+        shape : tuple
+        key : str, optional
+            Key (name) for this new node. If None, the server will provide a unique key.
+        metadata : dict, optional
+            User metadata. May be nested. Must contain only basic types
+            (e.g. numbers, strings, lists, dicts) that are JSON-serializable.
+        dims : List[str], optional
+            A label for each dimension of the array.
+        specs : List[Spec], optional
+            List of names that are used to label that the data and/or metadata
+            conform to some named standard specification.
+        references : List[Dict[str, URL]], optional
+            References (e.g. links) to related information. This may include
+            links into other Tiled data sets, search results, or external
+            resources unrelated to Tiled.
+
         Examples
         --------
 
         Write a sparse.COO array.
 
         >>> import sparse
         >>> coo = sparse.COO(coords=[[2, 5]], data=[1.3, 7.5], shape=(10,))
@@ -724,61 +809,47 @@
         # Define the overall shape and the dimensions of each chunk.
         >>> from tiled.structures.sparse import COOStructure
         >>> x = c.new("sparse", COOStructure(shape=(10,), chunks=((5, 5),)))
         # Upload the data in each chunk.
         # Coords are given with in the reference frame of each chunk.
         >>> x.write_block(coords=[[2, 4]], data=[3.1, 2.8], block=(0,))
         >>> x.write_block(coords=[[0, 1]], data=[6.7, 1.2], block=(1,))
-
-        Parameters
-        ----------
-        coords : array-like
-        data : array-like
-        shape: Tuple
-        metadata : dict, optional
-            User metadata. May be nested. Must contain only basic types
-            (e.g. numbers, strings, lists, dicts) that are JSON-serializable.
-        dims : List[str], optional
-            A label for each dimension of the array.
-        specs : List[Spec], optional
-            List of names that are used to label that the data and/or metadata
-            conform to some named standard specification.
-        references : Dict[str, URL], optional
-            References (e.g. links) to related information. This may include
-            links into other Tiled data sets, search results, or external
-            resources unrelated to Tiled.
-
         """
         from ..structures.sparse import COOStructure
 
         structure = COOStructure(
             shape=shape,
             # This method only supports single-chunk COO arrays.
             chunks=tuple((dim,) for dim in shape),
             dims=dims,
         )
         client = self.new(
             StructureFamily.sparse,
             structure,
+            key=key,
             metadata=metadata,
             specs=specs,
             references=references,
         )
         client.write(coords, data)
         return client
 
-    def write_dataframe(self, dataframe, metadata=None, specs=None, references=None):
+    def write_dataframe(
+        self, dataframe, *, key=None, metadata=None, specs=None, references=None
+    ):
         """
         EXPERIMENTAL: Write a DataFrame.
 
         This is subject to change or removal without notice
 
         Parameters
         ----------
         dataframe : pandas.DataFrame
+        key : str, optional
+            Key (name) for this new node. If None, the server will provide a unique key.
         metadata : dict, optional
             User metadata. May be nested. Must contain only basic types
             (e.g. numbers, strings, lists, dicts) that are JSON-serializable.
         specs : List[Spec], optional
             List of names that are used to label that the data and/or metadata
             conform to some named standard specification.
         references : List[Dict[str, URL]], optional
@@ -792,16 +863,14 @@
         from ..serialization.dataframe import serialize_arrow
         from ..structures.dataframe import (
             DataFrameMacroStructure,
             DataFrameMicroStructure,
             DataFrameStructure,
         )
 
-        self._cached_len = None
-
         metadata = metadata or {}
         specs = specs or []
 
         if isinstance(dataframe, dask.dataframe.DataFrame):
             meta = bytes(serialize_arrow(dataframe._meta, {}))
             divisions = bytes(
                 serialize_arrow(
@@ -820,14 +889,15 @@
                 npartitions=npartitions, columns=list(dataframe.columns)
             ),
         )
 
         client = self.new(
             StructureFamily.dataframe,
             structure,
+            key=key,
             metadata=metadata,
             specs=specs,
             references=references,
         )
 
         if hasattr(dataframe, "partitions"):
             if isinstance(dataframe, dask.dataframe.DataFrame):
```

### Comparing `tiled-0.1.0a93/tiled/client/sparse.py` & `tiled-0.1.0a94/tiled/client/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/client/utils.py` & `tiled-0.1.0a94/tiled/client/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/client/xarray.py` & `tiled-0.1.0a94/tiled/client/xarray.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import dask
 import dask.array
 import pandas
 import xarray
 
 from ..client.base import BaseStructureClient
 from ..serialization.dataframe import deserialize_arrow
+from ..structures.core import Spec
 from ..utils import APACHE_ARROW_FILE_MIME_TYPE
 from .node import Node
 
 LENGTH_LIMIT_FOR_WIDE_TABLE_OPTIMIZATION = 1_000_000
 
 
 class DaskDatasetClient(Node):
@@ -181,7 +182,31 @@
 
     def _fetch_variables(self, variables):
         content = self.get(
             self.link,
             params={"format": APACHE_ARROW_FILE_MIME_TYPE, "field": variables},
         )
         return deserialize_arrow(content)
+
+
+def write_xarray_dataset(client_node, dataset, key=None):
+    dataset_client = client_node.create_node(
+        key=key, specs=[Spec("xarray_dataset")], metadata={"attrs": dataset.attrs}
+    )
+    for name in dataset.data_vars:
+        data_array = dataset[name]
+        dataset_client.write_array(
+            data_array.data,
+            key=name,
+            metadata={"attrs": data_array.attrs},
+            specs=[Spec("xarray_data_var")],
+        )
+    for name in dataset.coords:
+        data_array = dataset[name]
+        dataset_client.write_array(
+            data_array.data,
+            key=name,
+            metadata={"attrs": data_array.attrs},
+            dims=data_array.dims,
+            specs=[Spec("xarray_coord")],
+        )
+    return dataset_client
```

### Comparing `tiled-0.1.0a93/tiled/commandline/_admin.py` & `tiled-0.1.0a94/tiled/commandline/_admin.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/commandline/_api_key.py` & `tiled-0.1.0a94/tiled/commandline/_api_key.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/commandline/_profile.py` & `tiled-0.1.0a94/tiled/commandline/_profile.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/commandline/_serve.py` & `tiled-0.1.0a94/tiled/commandline/_serve.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from pathlib import Path
-from typing import Optional
+from typing import List, Optional
 
 import typer
 
 serve_app = typer.Typer()
 
 
+SQLITE_CATALOG_FILENAME = "tiled_catalog.sqlite"
+
+
 @serve_app.command("directory")
 def serve_directory(
     directory: str,
     public: bool = typer.Option(
         False,
         "--public",
         help=(
@@ -88,14 +91,135 @@
     print_admin_api_key_if_generated(web_app, host=host, port=port)
 
     import uvicorn
 
     uvicorn.run(web_app, host=host, port=port)
 
 
+def serve_catalog(
+    database: str = typer.Argument(
+        None, help="A filepath or database URI, e.g. 'catalog.db'"
+    ),
+    read: List[str] = typer.Option(
+        None,
+        "--read",
+        "-r",
+        help="Locations that the server may read from",
+    ),
+    write: str = typer.Option(
+        None,
+        "--write",
+        "-w",
+        help="Location that the server may write to",
+    ),
+    temp: bool = typer.Option(
+        False,
+        "--temp",
+        help="Make a new catalog in a temporary directory.",
+    ),
+    public: bool = typer.Option(
+        False,
+        "--public",
+        help=(
+            "Turns off requirement for API key authentication for reading. "
+            "However, the API key is still required for writing, so data cannot be modified even with "
+            "this option selected."
+        ),
+    ),
+    host: str = typer.Option(
+        "127.0.0.1",
+        help=(
+            "Bind socket to this host. Use `--host 0.0.0.0` to make the application "
+            "available on your local network. IPv6 addresses are supported, for "
+            "example: --host `'::'`."
+        ),
+    ),
+    port: int = typer.Option(8000, help="Bind to a socket with this port."),
+    object_cache_available_bytes: Optional[float] = typer.Option(
+        None,
+        "--data-cache",
+        help=(
+            "Maximum size for the object cache, given as a number of bytes as in "
+            "1_000_000 or as a fraction of system RAM (total physical memory) as in "
+            "0.3. Set to 0 to disable this cache. By default, it will use up to "
+            "0.15 (15%) of RAM."
+        ),
+    ),
+    scalable: bool = typer.Option(
+        False,
+        "--scalable",
+        help=(
+            "This verifies that the configuration is compatible with scaled (multi-process) deployments."
+        ),
+    ),
+):
+    "Serve a catalog."
+    import urllib.parse
+
+    from ..catalog import from_uri
+    from ..server.app import build_app, print_admin_api_key_if_generated
+
+    parsed_database = urllib.parse.urlparse(database)
+    if parsed_database.scheme in ("", "file"):
+        database = f"sqlite+aiosqlite:///{parsed_database.path}"
+
+    if temp:
+        if database is not None:
+            typer.echo(
+                "The option --temp was set but a database was also provided. "
+                "Do one or the other.",
+                err=True,
+            )
+            raise typer.Abort()
+        import tempfile
+
+        directory = Path(tempfile.TemporaryDirectory().name)
+        directory.mkdir()
+        SQLITE_CATALOG_FILENAME = "catalog.db"
+        DATA_SUBDIRECTORY = "data"
+        typer.echo(
+            f"Creating catalog database at {directory / SQLITE_CATALOG_FILENAME}",
+            err=True,
+        )
+        typer.echo(
+            f"Creating writable catalog data directory at {directory / DATA_SUBDIRECTORY}",
+            err=True,
+        )
+        database = f"sqlite+aiosqlite:///{Path(directory, SQLITE_CATALOG_FILENAME)}"
+        if write is None:
+            write = directory / DATA_SUBDIRECTORY
+        # TODO Hook into server lifecycle hooks to delete this at shutdown.
+
+    tree_kwargs = {}
+    server_settings = {}
+    if object_cache_available_bytes is not None:
+        server_settings["object_cache"] = {}
+        server_settings["object_cache"][
+            "available_bytes"
+        ] = object_cache_available_bytes
+    tree = from_uri(
+        database,
+        writable_storage=write,
+        readable_storage=read,
+        initialize_database_at_startup=temp,
+        **tree_kwargs,
+    )
+    web_app = build_app(
+        tree, {"allow_anonymous_access": public}, server_settings, scalable=scalable
+    )
+    print_admin_api_key_if_generated(web_app, host=host, port=port)
+
+    import uvicorn
+
+    uvicorn.run(web_app, host=host, port=port)
+
+
+serve_app.command("catalog")(serve_catalog)
+
+
 @serve_app.command("pyobject")
 def serve_pyobject(
     object_path: str = typer.Argument(
         ..., help="Object path, as in 'package.subpackage.module:object_name'"
     ),
     public: bool = typer.Option(
         False,
```

### Comparing `tiled-0.1.0a93/tiled/commandline/_utils.py` & `tiled-0.1.0a94/tiled/commandline/_utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/commandline/main.py` & `tiled-0.1.0a94/tiled/commandline/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,27 @@
 """
     ) from err
 
 cli_app = typer.Typer()
 
 from ._admin import admin_app  # noqa: E402
 from ._api_key import api_key_app  # noqa: E402
+from ._catalog import catalog_app  # noqa: E402
 from ._profile import profile_app  # noqa: E402
 from ._serve import serve_app  # noqa: E402
 from ._utils import (  # noqa E402
     CLI_CACHE_DIR,
     get_context,
     get_default_profile_name,
     get_profile,
 )
 
+cli_app.add_typer(
+    catalog_app, name="catalog", help="Manage a catalog of data to be served by Tiled."
+)
 cli_app.add_typer(serve_app, name="serve", help="Launch a Tiled server.")
 cli_app.add_typer(
     profile_app, name="profile", help="Examine Tiled 'profiles' (client-side config)."
 )
 cli_app.add_typer(
     api_key_app, name="api_key", help="Create, list, and revoke API keys."
 )
```

### Comparing `tiled-0.1.0a93/tiled/config.py` & `tiled-0.1.0a94/tiled/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from collections import defaultdict
 from datetime import timedelta
 from functools import lru_cache
 from pathlib import Path
 
 import jsonschema
 
+from .adapters.mapping import MapAdapter
 from .media_type_registration import (
     compression_registry as default_compression_registry,
 )
 from .media_type_registration import (
     serialization_registry as default_serialization_registry,
 )
 from .query_registration import query_registry as default_query_registry
@@ -48,14 +49,17 @@
 
     The parameters query_registry, compression_registry, and
     serialization_registry are used by the tests to inject separate registry
     instances. By default, the singleton global instances of these registries
     and used (and modified).
     """
     config = copy.deepcopy(config)  # Avoid mutating input.
+    startup_tasks = []
+    shutdown_tasks = []
+    background_tasks = []
     if query_registry is None:
         query_registry = default_query_registry
     if serialization_registry is None:
         serialization_registry = default_serialization_registry
     if compression_registry is None:
         compression_registry = default_compression_registry
     if validation_registry is None:
@@ -126,30 +130,35 @@
                 args = {}
                 args.update(item.get("args", {}))
                 if access_policy is not None:
                     args["access_policy"] = access_policy
                 tree = obj(**args)
             else:
                 # Interpret obj as a tree *instance*.
+                if access_policy is not None:
+                    raise ValueError(
+                        f"Cannot apply access_policy to object {obj} which is already instantiated."
+                    )
                 tree = obj
             if segments in trees:
                 raise ValueError(f"The path {'/'.join(segments)} was specified twice.")
             trees[segments] = tree
+            startup_tasks.extend(getattr(tree, "startup_tasks", []))
+            shutdown_tasks.extend(getattr(tree, "shutdown_tasks", []))
+            background_tasks.extend(getattr(tree, "background_tasks", []))
         if not len(trees):
             raise ValueError("Configuration contains no trees")
         if list(trees) == [()]:
             # Simple case: there is one tree, served at the root path /.
             root_tree = tree
             if root_access_policy is not None:
                 tree.access_policy = root_access_policy
         else:
             # There are one or more tree(s) to be served at
             # sub-paths. Merged them into one root MapAdapter.
-            from .adapters.mapping import MapAdapter
-
             # Map path segments to dicts containing Adapters at that path.
             root_mapping = {}
             index = {(): root_mapping}
             include_routers = []
             for segments, tree in trees.items():
                 for i in range(len(segments)):
                     if segments[:i] not in index:
@@ -198,14 +207,19 @@
         "tree": root_tree,
         "authentication": auth_spec,
         "server_settings": server_settings,
         "query_registry": query_registry,
         "serialization_registry": serialization_registry,
         "compression_registry": compression_registry,
         "validation_registry": validation_registry,
+        "tasks": {
+            "startup": startup_tasks,
+            "shutdown": shutdown_tasks,
+            "background": background_tasks,
+        },
     }
 
 
 def merge(configs):
     merged = {"trees": []}
 
     # These variables are used to produce error messages that point
```

### Comparing `tiled-0.1.0a93/tiled/config_schemas/client_profiles.yml` & `tiled-0.1.0a94/tiled/config_schemas/client_profiles.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/config_schemas/service_configuration.yml` & `tiled-0.1.0a94/tiled/config_schemas/service_configuration.yml`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/database/alembic.ini.template` & `tiled-0.1.0a94/tiled/database/alembic.ini.template`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/database/alembic_utils.py` & `tiled-0.1.0a94/tiled/database/alembic_utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/database/connection_pool.py` & `tiled-0.1.0a94/tiled/database/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/database/core.py` & `tiled-0.1.0a94/tiled/database/core.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/database/migrations/env.py` & `tiled-0.1.0a94/tiled/database/migrations/env.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/database/migrations/versions/481830dd6c11_initialize.py` & `tiled-0.1.0a94/tiled/database/migrations/versions/481830dd6c11_initialize.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/database/migrations/versions/4a9dfaba4a98_add_pendingsession.py` & `tiled-0.1.0a94/tiled/database/migrations/versions/4a9dfaba4a98_add_pendingsession.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py` & `tiled-0.1.0a94/tiled/database/migrations/versions/56809bcbfcb0_add_create_scope_to_default_roles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py` & `tiled-0.1.0a94/tiled/database/migrations/versions/722ff4e4fcc7_add_write_scopes_to_default_roles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/database/orm.py` & `tiled-0.1.0a94/tiled/database/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     Column("role_id", Integer, ForeignKey("roles.id"), primary_key=True),
 )
 
 
 class Principal(Timestamped, Base):
     __tablename__ = "principals"
 
-    # This id is internal, never exposed to the user.
+    # This id is internal, never exposed to the client.
     id = Column(Integer, primary_key=True, index=True, autoincrement=True)
     # This uuid is public.
     uuid = Column(
         UUID,
         index=True,
         nullable=False,
         default=lambda: uuid_module.uuid4(),
@@ -188,23 +188,18 @@
     When the client attempts to use a refresh token, we first check
     here to ensure that the "session", which is associated with a chain
     of refresh tokens that came from a single authentication, are still valid.
     """
 
     __tablename__ = "sessions"
 
-    # This id is internal, never exposed to the user.
+    # This id is internal, never exposed to the client.
     id = Column(Integer, primary_key=True, index=True, autoincrement=True)
-    # This uuid is public.
-    uuid = Column(
-        UUID,
-        index=True,
-        nullable=False,
-        default=lambda: uuid_module.uuid4(),
-    )
+    # This uuid is exposed to the client.
+    uuid = Column(UUID, index=True, nullable=False, default=uuid_module.uuid4)
     time_last_refreshed = Column(DateTime(timezone=False), nullable=True)
     refresh_count = Column(Integer, nullable=False, default=0)
     expiration_time = Column(DateTime(timezone=False), nullable=False)
     principal_id = Column(Integer, ForeignKey("principals.id"), nullable=False)
     revoked = Column(Boolean, default=False, nullable=False)
 
     principal = relationship("Principal", back_populates="sessions", lazy="joined")
```

### Comparing `tiled-0.1.0a93/tiled/examples/generate_files.py` & `tiled-0.1.0a94/tiled/examples/generate_files.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/examples/generated.py` & `tiled-0.1.0a94/tiled/examples/generated.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/examples/generated_minimal.py` & `tiled-0.1.0a94/tiled/examples/generated_minimal.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/examples/nexus.py` & `tiled-0.1.0a94/tiled/examples/nexus.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/examples/toy_authentication.py` & `tiled-0.1.0a94/tiled/examples/toy_authentication.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/examples/xdi.py` & `tiled-0.1.0a94/tiled/examples/xdi.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/iterviews.py` & `tiled-0.1.0a94/tiled/iterviews.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/media_type_registration.py` & `tiled-0.1.0a94/tiled/media_type_registration.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,20 +116,14 @@
             return self._lookup[structure_family][media_type]
         except KeyError:
             pass
         raise ValueError(
             f"No dispatch for structure_family {structure_family} with media type {media_type}"
         )
 
-    def __call__(self, structure_family, media_type, *args, **kwargs):
-        """
-        Invoke a writer for a given structure and media type.
-        """
-        return self.dispatch(structure_family, media_type)(*args, **kwargs)
-
 
 class CompressionRegistry:
     def __init__(self):
         self._lookup = defaultdict(collections.OrderedDict)
 
     def encodings(self, media_type):
         # The last encoding registered is the first preferred by server
@@ -169,23 +163,20 @@
         """
         return self.dispatch(media_type, encoder)(*args, **kwargs)
 
 
 serialization_registry = SerializationRegistry()
 "Global serialization registry. See Registry for usage examples."
 
+deserialization_registry = SerializationRegistry()
+"Global deserialization registry. See Registry for usage examples."
+
 compression_registry = CompressionRegistry()
 "Global compression registry. See Registry for usage examples."
 
-# TODO Do we *need* a deserialization registry?
-# The Python client always deals with a certain preferred format
-# for each structure family. Deserializing other formats is other
-# clients' problem, and we can't help with that from here.
-deserialization_registry = SerializationRegistry()
-
 
 compression_registry.register(
     "application/json",
     "gzip",
     lambda buffer: gzip.GzipFile(mode="wb", fileobj=buffer, compresslevel=9),
 )
 compression_registry.register(
```

### Comparing `tiled-0.1.0a93/tiled/profiles.py` & `tiled-0.1.0a94/tiled/profiles.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/queries.py` & `tiled-0.1.0a94/tiled/queries.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/query_registration.py` & `tiled-0.1.0a94/tiled/query_registration.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/scopes.py` & `tiled-0.1.0a94/tiled/scopes.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/serialization/__init__.py` & `tiled-0.1.0a94/tiled/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/serialization/array.py` & `tiled-0.1.0a94/tiled/serialization/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/serialization/dataframe.py` & `tiled-0.1.0a94/tiled/serialization/dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/serialization/image_serializer_helpers.py` & `tiled-0.1.0a94/tiled/serialization/image_serializer_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     np.longlong,
     np.ulonglong,
 )  # 64 bits
 _integer_ranges = {t: (np.iinfo(t).min, np.iinfo(t).max) for t in _integer_types}
 dtype_range = {
     bool: (False, True),
     np.bool_: (False, True),
-    np.bool8: (False, True),
     float: (-1, 1),
     np.float_: (-1, 1),
     np.float16: (-1, 1),
     np.float32: (-1, 1),
     np.float64: (-1, 1),
 }
 dtype_range.update(_integer_ranges)
```

### Comparing `tiled-0.1.0a93/tiled/serialization/node.py` & `tiled-0.1.0a94/tiled/serialization/node.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import io
 
 from ..media_type_registration import serialization_registry
 from ..utils import SerializationError, modules_available, safe_json_dump
 
 
-def walk(node, pre=None):
+async def walk(node, filter_for_access, pre=None):
     """
     Yield (key_path, value) where each value is an ArrayAdapter.
 
     As a succinct illustration (does not literally run):
 
     >>> list(walk{"a": {"b": 1, "c": {"d": 2}}})
     [
         (("a", "b"), 1),
         (("a", "c", "d"), 2),
     ]
     """
     pre = pre[:] if pre else []
     if node.structure_family != "array":
-        for key, value in node.items():
-            for d in walk(value, pre + [key]):
-                yield d
+        if hasattr(node, "items_range"):
+            for key, value in await filter_for_access(node).items_range(0, None):
+                async for d in walk(value, filter_for_access, pre + [key]):
+                    yield d
+        else:
+            for key, value in filter_for_access(node).items():
+                async for d in walk(value, filter_for_access, pre + [key]):
+                    yield d
     else:
         yield (pre, node)
 
 
 if modules_available("h5py"):
 
-    def serialize_hdf5(node, metadata):
+    async def serialize_hdf5(node, metadata, filter_for_access):
         """
         Encode everything below this node as HDF5.
 
         Walk node. Encode all nodes an dataframes as Groups, all arrays and columns as Datasets.
         """
         import h5py
 
@@ -39,19 +44,22 @@
         root_node = node
         MSG = "Metadata contains types or structure that does not fit into HDF5."
         with h5py.File(buffer, mode="w") as file:
             try:
                 file.attrs.update(metadata)
             except TypeError:
                 raise SerializationError(MSG)
-            for key_path, array_adapter in walk(node):
+            async for key_path, array_adapter in walk(node, filter_for_access):
                 group = file
                 node = root_node
                 for key in key_path[:-1]:
-                    node = node[key]
+                    if hasattr(node, "lookup_node"):
+                        node = await node.lookup_node([key])
+                    else:
+                        node = node[key]
                     if key in group:
                         group = group[key]
                     else:
                         group = group.create_group(key)
                         try:
                             group.attrs.update(node.metadata)
                         except TypeError:
@@ -62,22 +70,25 @@
                     dataset.attrs.create(k, v)
         return buffer.getbuffer()
 
     serialization_registry.register("node", "application/x-hdf5", serialize_hdf5)
 
 if modules_available("orjson"):
 
-    def serialize_json(node, metadata):
+    async def serialize_json(node, metadata, filter_for_access):
         "Export node to JSON, with each node having a 'contents' and 'metadata' sub-key."
         root_node = node
         to_serialize = {"contents": {}, "metadata": dict(root_node.metadata)}
-        for key_path, array_adapter in walk(node):
+        async for key_path, array_adapter in walk(node, filter_for_access):
             d = to_serialize["contents"]
             node = root_node
             for key in key_path:
-                node = node[key]
+                if hasattr(node, "lookup_node"):
+                    node = await node.lookup_node([key])
+                else:
+                    node = node[key]
                 if key not in d:
                     d[key] = {"contents": {}, "metadata": dict(node.metadata)}
                 d = d[key]["contents"]
         return safe_json_dump(to_serialize)
 
     serialization_registry.register("node", "application/json", serialize_json)
```

### Comparing `tiled-0.1.0a93/tiled/serialization/sparse.py` & `tiled-0.1.0a94/tiled/serialization/sparse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import io
 
-from ..media_type_registration import serialization_registry
+from ..media_type_registration import deserialization_registry, serialization_registry
 from ..utils import modules_available
 
 if modules_available("h5py"):
 
     def serialize_hdf5(sparse_arr, metadata):
         """
         Place coords and data in HDF5 datasets with those names.
@@ -23,28 +23,32 @@
 
 if modules_available("pandas", "pyarrow"):
     import pandas
 
     from .dataframe import (
         APACHE_ARROW_FILE_MIME_TYPE,
         XLSX_MIME_TYPE,
+        deserialize_arrow,
         serialize_arrow,
         serialize_csv,
         serialize_excel,
         serialize_html,
         serialize_parquet,
     )
 
     # Support DataFrame formats by first converting to DataFrame.
     # naming columns like dim0, dim1, ..., dimN, data.
     def to_dataframe(sparse_arr):
         d = {f"dim{i}": coords for i, coords in enumerate(sparse_arr.coords)}
         d["data"] = sparse_arr.data
         return pandas.DataFrame(d)
 
+    deserialization_registry.register(
+        "sparse", APACHE_ARROW_FILE_MIME_TYPE, deserialize_arrow
+    )
     serialization_registry.register(
         "sparse",
         APACHE_ARROW_FILE_MIME_TYPE,
         lambda sparse_arr, metadata: serialize_arrow(
             to_dataframe(sparse_arr), metadata, preserve_index=False
         ),
     )
```

### Comparing `tiled-0.1.0a93/tiled/serialization/xarray.py` & `tiled-0.1.0a94/tiled/serialization/xarray.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def close(self):
         # When the netcdf writer tells us to close(), ignore it.
         pass
 
 
 if modules_available("scipy"):
 
-    def serialize_netcdf(node, metadata):
+    def serialize_netcdf(node, metadata, filter_for_access):
         file = _BytesIOThatIgnoresClose()
         # Per the xarray.Dataset.to_netcdf documentation,
         # file-like objects are only supported by the scipy engine.
         as_dataset(node).to_netcdf(file, engine="scipy")
         return file.getbuffer()
 
     # Both application/netcdf and application/x-netcdf are used.
@@ -67,74 +67,88 @@
 
 # Support DataFrame formats by first converting to DataFrame.
 # This doesn't make much sense for N-dimensional variables, but for
 # 1-dimensional variables it is useful.
 serialization_registry.register(
     "xarray_dataset",
     APACHE_ARROW_FILE_MIME_TYPE,
-    lambda node, metadata: serialize_arrow(as_dataset(node).to_dataframe(), metadata),
+    lambda node, metadata, filter_for_access: serialize_arrow(
+        as_dataset(node).to_dataframe(), metadata
+    ),
 )
 serialization_registry.register(
     "xarray_dataset",
     "application/x-parquet",
-    lambda node, metadata: serialize_parquet(as_dataset(node).to_dataframe(), metadata),
+    lambda node, metadata, filter_for_access: serialize_parquet(
+        as_dataset(node).to_dataframe(), metadata
+    ),
 )
 serialization_registry.register(
     "xarray_dataset",
     "text/csv",
-    lambda node, metadata: serialize_csv(as_dataset(node).to_dataframe(), metadata),
+    lambda node, metadata, filter_for_access: serialize_csv(
+        as_dataset(node).to_dataframe(), metadata
+    ),
 )
 serialization_registry.register(
     "xarray_dataset",
     "text/x-comma-separated-values",
-    lambda node, metadata: serialize_csv(as_dataset(node).to_dataframe(), metadata),
+    lambda node, metadata, filter_for_access: serialize_csv(
+        as_dataset(node).to_dataframe(), metadata
+    ),
 )
 serialization_registry.register(
     "xarray_dataset",
     "text/plain",
-    lambda node, metadata: serialize_csv(as_dataset(node).to_dataframe(), metadata),
+    lambda node, metadata, filter_for_access: serialize_csv(
+        as_dataset(node).to_dataframe(), metadata
+    ),
 )
 serialization_registry.register(
     "xarray_dataset",
     "text/html",
-    lambda node, metadata: serialize_html(as_dataset(node).to_dataframe(), metadata),
+    lambda node, metadata, filter_for_access: serialize_html(
+        as_dataset(node).to_dataframe(), metadata
+    ),
 )
 serialization_registry.register(
     "xarray_dataset",
     XLSX_MIME_TYPE,
-    lambda node, metadata: serialize_excel(as_dataset(node).to_dataframe(), metadata),
+    lambda node, metadata, filter_for_access: serialize_excel(
+        as_dataset(node).to_dataframe(), metadata
+    ),
 )
 if modules_available("orjson"):
     import orjson
 
-    def serialize_json(node, metadata):
+    def serialize_json(node, metadata, filter_for_access):
         df = as_dataset(node).to_dataframe()
         return orjson.dumps(
             {column: df[column].tolist() for column in df},
         )
 
     serialization_registry.register(
         "xarray_dataset",
         "application/json",
         serialize_json,
     )
 if modules_available("h5py"):
 
-    def serialize_hdf5(node, metadata):
+    async def serialize_hdf5(node, metadata, filter_for_access):
         """
         Like for node, but encode everything under 'attrs' in attrs.
         """
         import h5py
 
         buffer = io.BytesIO()
         root_node = node
         with h5py.File(buffer, mode="w") as file:
             for k, v in metadata["attrs"].items():
                 file.attrs.create(k, v)
-            for key_path, array_adapter in walk(node):
+            async for key_path, array_adapter in walk(node, filter_for_access):
                 group = file
                 node = root_node
                 for key in key_path[:-1]:
                     node = node[key]
                     if key in group:
                         group = group[key]
                     else:
```

### Comparing `tiled-0.1.0a93/tiled/server/app.py` & `tiled-0.1.0a94/tiled/server/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     tree,
     authentication=None,
     server_settings=None,
     query_registry=None,
     serialization_registry=None,
     compression_registry=None,
     validation_registry=None,
+    tasks=None,
     scalable=False,
 ):
     """
     Serve a Tree
 
     Parameters
     ----------
@@ -121,14 +122,24 @@
         spec["provider"]: spec["authenticator"]
         for spec in authentication.get("providers", [])
     }
     server_settings = server_settings or {}
     query_registry = query_registry or get_query_registry()
     compression_registry = compression_registry or default_compression_registry
     validation_registry = validation_registry or default_validation_registry
+    tasks = tasks or {}
+    tasks.setdefault("startup", [])
+    tasks.setdefault("background", [])
+    tasks.setdefault("shutdown", [])
+    # The tasks are collected at config-parsing time off of the sub-trees.
+    # Collect the tasks off the root tree here, so that it works when
+    # a single tree is passed to build_app(...) directly, as happens in the tests.
+    tasks["startup"].extend(getattr(tree, "startup_tasks", []))
+    tasks["background"].extend(getattr(tree, "background_tasks", []))
+    tasks["shutdown"].extend(getattr(tree, "shutdown_tasks", []))
 
     if scalable:
         if authentication.get("providers"):
             # Even if the deployment allows public, anonymous access, secret
             # keys are needed to generate JWTs for any users that do log in.
             if not (
                 ("secret_keys" in authentication)
@@ -412,19 +423,23 @@
     openssl rand -hex 32
 
     # With Python:
     python -c "import secrets; print(secrets.token_hex(32))"
     """
                 )
 
+        # Run startup tasks collected from trees (adapters).
+        for task in tasks.get("startup", []):
+            await task()
+
         # Stash these to cancel this on shutdown.
         app.state.tasks = []
         # Trees and Authenticators can run tasks in the background.
         background_tasks = []
-        background_tasks.extend(getattr(tree, "background_tasks", []))
+        background_tasks.extend(tasks.get("background_tasks", []))
         for authenticator in authenticators:
             background_tasks.extend(getattr(authenticator, "background_tasks", []))
         for task in background_tasks or []:
             asyncio_task = asyncio.create_task(task())
             app.state.tasks.append(asyncio_task)
 
         app.state.allow_origins.extend(settings.allow_origins)
@@ -555,14 +570,18 @@
 
             app.state.tasks.append(
                 asyncio.create_task(purge_expired_sessions_and_api_keys())
             )
 
     @app.on_event("shutdown")
     async def shutdown_event():
+        # Run shutdown tasks collected from trees (adapters).
+        for task in tasks.get("shutdown", []):
+            await task()
+
         settings = app.dependency_overrides[get_settings]()
         if settings.database_uri is not None:
             from ..database.connection_pool import close_database_connection_pool
 
             for task in app.state.tasks:
                 task.cancel()
             await close_database_connection_pool(settings.database_settings)
```

### Comparing `tiled-0.1.0a93/tiled/server/authentication.py` & `tiled-0.1.0a94/tiled/server/authentication.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/server/compression.py` & `tiled-0.1.0a94/tiled/server/compression.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/server/core.py` & `tiled-0.1.0a94/tiled/server/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import types
 import uuid
 from collections import defaultdict
 from datetime import datetime, timedelta
 from hashlib import md5
 from typing import Any
 
+import anyio
 import dateutil.tz
 import jmespath
 import msgpack
 from fastapi import HTTPException, Response
 from starlette.responses import JSONResponse, Send, StreamingResponse
 
 # Some are not directly used, but they register things on import.
@@ -29,15 +30,15 @@
     APACHE_ARROW_FILE_MIME_TYPE,
     SerializationError,
     UnsupportedShape,
     safe_json_dump,
 )
 from . import schemas
 from .etag import tokenize
-from .utils import record_timing
+from .utils import ensure_awaitable, record_timing
 
 del queries
 register_builtin_serializers()
 
 
 _FILTER_PARAM_PATTERN = re.compile(r"filter___(?P<name>.*)___(?P<field>[^\d\W][\w\d]+)")
 _LOCAL_TZINFO = dateutil.tz.gettz()
@@ -57,22 +58,24 @@
 # opt in to this behavior and decide on a reasonable depth.
 DEPTH_LIMIT = 5
 
 DEFAULT_PAGE_SIZE = 100
 MAX_PAGE_SIZE = 300
 
 
-def len_or_approx(tree):
+async def len_or_approx(tree):
     """
     Prefer approximate length if implemented. (It's cheaper.)
     """
+    if hasattr(tree, "async_len"):
+        return await tree.async_len()
     try:
-        return operator.length_hint(tree)
+        return await anyio.to_thread.run_sync(operator.length_hint, tree)
     except TypeError:
-        return len(tree)
+        return await anyio.to_thread.run_sync(len, tree)
 
 
 def pagination_links(base_url, route, path_parts, offset, limit, length_hint):
     path_str = "/".join(path_parts)
     links = {
         "self": f"{base_url}{route}/{path_str}?page[offset]={offset}&page[limit]={limit}",
         # These are conditionally overwritten below.
@@ -166,56 +169,63 @@
                 status_code=400, detail="This Tree does not support sorting."
             )
         tree = tree.sort(sorting)
 
     return tree
 
 
-def construct_entries_response(
+async def construct_entries_response(
     query_registry,
     tree,
     route,
     path,
     offset,
     limit,
     fields,
     select_metadata,
     omit_links,
+    show_sources,
     filters,
     sort,
     base_url,
     media_type,
     max_depth,
 ):
     path_parts = [segment for segment in path.split("/") if segment]
     tree = apply_search(tree, filters, query_registry)
     tree = apply_sort(tree, sort)
 
-    count = len_or_approx(tree)
+    count = await len_or_approx(tree)
     links = pagination_links(base_url, route, path_parts, offset, limit, count)
     data = []
     if fields != [schemas.EntryFields.none]:
         # Pull a page of items into memory.
-        items = tree.items()[offset : offset + limit]  # noqa: E203
+        if hasattr(tree, "items_range"):
+            items = await tree.items_range(offset, limit)
+        else:
+            items = tree.items()[offset : offset + limit]  # noqa: E203
     else:
         # Pull a page of just the keys, which is cheaper.
-        items = (
-            (key, None) for key in tree.keys()[offset : offset + limit]  # noqa: E203
-        )
+        if hasattr(tree, "keys_range"):
+            keys = await tree.keys_range(offset, limit)
+        else:
+            keys = tree.keys()[offset : offset + limit]  # noqa: E203
+        items = [(key, None) for key in keys]
     # This value will not leak out. It just used to seed comparisons.
     metadata_stale_at = datetime.utcnow() + timedelta(days=1_000_000)
     must_revalidate = getattr(tree, "must_revalidate", True)
     for key, entry in items:
-        resource = construct_resource(
+        resource = await construct_resource(
             base_url,
             path_parts + [key],
             entry,
             fields,
             select_metadata,
             omit_links,
+            show_sources,
             media_type,
             max_depth=max_depth,
         )
         data.append(resource)
         # If any entry has emtry.metadata_stale_at = None, then there will
         # be no 'Expires' header. We will pessimistically assume the values
         # are immediately stale.
@@ -235,54 +245,55 @@
     "array": {"*/*": "application/octet-stream", "image/*": "image/png"},
     "dataframe": {"*/*": APACHE_ARROW_FILE_MIME_TYPE},
     "node": {"*/*": "application/x-hdf5"},
     "sparse": {"*/*": APACHE_ARROW_FILE_MIME_TYPE},
 }
 
 
-def construct_revisions_response(
+async def construct_revisions_response(
     entry,
     base_url,
     route,
     path,
     offset,
     limit,
     media_type,
 ):
     path_parts = [segment for segment in path.split("/") if segment]
-    revisions = entry.revisions[offset : offset + limit]  # noqa: E203
+    revisions = await entry.revisions(offset, limit)
     data = []
     for revision in revisions:
         item = {
-            "revision": revision["revision"],
+            "revision_number": revision.revision_number,
             "attributes": {
-                "metadata": revision["metadata"],
-                "specs": revision["specs"],
-                "references": revision["references"],
-                "updated_at": revision["updated_at"],
+                "metadata": revision.metadata,
+                "specs": revision.specs,
+                "references": revision.references,
+                "time_updated": revision.time_updated,
             },
         }
         data.append(item)
     count = len(data)
     links = pagination_links(
         base_url, route, path_parts, offset, limit, count
     )  # maybe reuse or maybe make a new pagination_revision_links
     return schemas.Response(data=data, links=links, meta={"count": count})
 
 
-def construct_data_response(
+async def construct_data_response(
     structure_family,
     serialization_registry,
     payload,
     metadata,
     request,
     format=None,
     specs=None,
     expires=None,
     filename=None,
+    filter_for_access=None,
 ):
     request.state.endpoint = "data"
     if specs is None:
         specs = []
     default_media_type = DEFAULT_MEDIA_TYPES[structure_family]["*/*"]
     # Give priority to the `format` query parameter. Otherwise, consult Accept
     # header.
@@ -338,17 +349,23 @@
     if expires is not None:
         headers["Expires"] = expires.strftime(HTTP_EXPIRES_HEADER_FORMAT)
     if request.headers.get("If-None-Match", "") == etag:
         # If the client already has this content, confirm that.
         return Response(status_code=304, headers=headers)
     if filename:
         headers["Content-Disposition"] = f"attachment;filename={filename}"
+    serializer = serialization_registry.dispatch(spec, media_type)
     # This is the expensive step: actually serialize.
     try:
-        content = serialization_registry(spec, media_type, payload, metadata)
+        if filter_for_access is not None:
+            content = await ensure_awaitable(
+                serializer, payload, metadata, filter_for_access
+            )
+        else:
+            content = await ensure_awaitable(serializer, payload, metadata)
     except UnsupportedShape as err:
         raise UnsupportedMediaTypes(
             f"The shape of this data {err.args[0]} is incompatible with the requested format ({media_type}). "
             f"Slice it or choose a different format.",
         )
     except SerializationError as err:
         raise UnsupportedMediaTypes(
@@ -361,27 +378,30 @@
     return response_class(
         content,
         media_type=media_type,
         headers=headers,
     )
 
 
-def construct_resource(
+async def construct_resource(
     base_url,
     path_parts,
     entry,
     fields,
     select_metadata,
     omit_links,
+    show_sources,
     media_type,
     max_depth,
     depth=0,
 ):
     path_str = "/".join(path_parts)
     attributes = {"ancestors": path_parts[:-1]}
+    if show_sources and hasattr(entry, "data_sources"):
+        attributes["data_sources"] = entry.data_sources
     if schemas.EntryFields.metadata in fields:
         if select_metadata is not None:
             attributes["metadata"] = jmespath.compile(select_metadata).search(
                 entry.metadata
             )
         else:
             attributes["metadata"] = entry.metadata
@@ -405,70 +425,76 @@
                 ((max_depth is None) or (depth < max_depth))
                 and hasattr(entry, "inlined_contents_enabled")
                 and entry.inlined_contents_enabled(depth)
                 and depth <= DEPTH_LIMIT
             ):
                 # This node wants us to inline its contents.
                 # First check that it is not too large.
-                est_count = len_or_approx(entry)
+                est_count = await len_or_approx(entry)
                 if est_count > INLINED_CONTENTS_LIMIT:
                     # Too large: do not inline its contents.
                     count = est_count
                     contents = None
                 else:
                     contents = {}
                     # The size may change as we are walking the entry.
                     # Keep a *true* count separately from est_count.
                     count = 0
                     for key, adapter in entry.items():
                         count += 1
                         if count > INLINED_CONTENTS_LIMIT:
                             # The est_count was inaccurate or else the entry has grown
                             # new children while we are walking it. Too large!
-                            count = len_or_approx(entry)
+                            count = await len_or_approx(entry)
                             contents = None
                             break
-                        contents[key] = construct_resource(
+                        contents[key] = await construct_resource(
                             base_url,
                             path_parts + [key],
                             adapter,
                             fields,
                             select_metadata,
                             omit_links,
+                            show_sources,
                             media_type,
                             max_depth,
                             depth=1 + depth,
                         )
             else:
-                count = len_or_approx(entry)
+                count = await len_or_approx(entry)
                 contents = None
             structure = schemas.NodeStructure(
                 count=count,
                 contents=contents,
             )
             attributes["structure"] = structure
         if schemas.EntryFields.sorting in fields:
             if hasattr(entry, "sorting"):
+                # HUGE HACK
                 # In the Python API we encode sorting as (key, direction).
                 # This order-based "record" notion does not play well with OpenAPI.
                 # In the HTTP API, therefore, we use {"key": key, "direction": direction}.
-                attributes["sorting"] = [
-                    {"key": key, "direction": direction}
-                    for key, direction in entry.sorting
-                ]
+                if entry.sorting and isinstance(entry.sorting[0], schemas.SortingItem):
+                    attributes["sorting"] = entry.sorting
+                else:
+                    attributes["sorting"] = [
+                        {"key": key, "direction": direction}
+                        for key, direction in entry.sorting
+                    ]
         d = {
             "id": path_parts[-1] if path_parts else "",
             "attributes": schemas.NodeAttributes(**attributes),
         }
         if not omit_links:
             d["links"] = {
                 "self": f"{base_url}/node/metadata/{path_str}",
                 "search": f"{base_url}/node/search/{path_str}",
                 "full": f"{base_url}/node/full/{path_str}",
             }
+
         resource = schemas.Resource[
             schemas.NodeAttributes, schemas.NodeLinks, schemas.NodeMeta
         ](**d)
     else:
         links = {"self": f"{base_url}/node/metadata/{path_str}"}
         structure = {}
         if entry is not None:
@@ -482,33 +508,37 @@
                     link: template.format(base_url=base_url, path=path_str)
                     for link, template in FULL_LINKS[entry.structure_family].items()
                 }
             )
             if schemas.EntryFields.structure_family in fields:
                 attributes["structure_family"] = entry.structure_family
             if entry.structure_family == "sparse":
-                if schemas.EntryFields.structure in fields:
-                    structure = dataclasses.asdict(entry.structure())
-                    shape = structure.get("shape")
+                # This arises from back-compat...needs revisiting.
+                structure_maybe_method = entry.structure
+                if callable(structure_maybe_method):
+                    structure = asdict(structure_maybe_method())
                 else:
-                    # The client did not request structure so we have not yet
-                    # accessed it, and we have access it specifically to construct this link.
-                    shape = entry.structure().shape
+                    structure = asdict(structure_maybe_method)
+                shape = structure.get("shape")
+                if schemas.EntryFields.structure not in fields:
+                    # We needed to access the structure to get the shape for
+                    # use in constructing links below, but we are not supposed
+                    # to include in the response.
                     structure = None
                 block_template = ",".join(f"{{{index}}}" for index in range(len(shape)))
                 links[
                     "block"
                 ] = f"{base_url}/array/block/{path_str}?block={block_template}"
             else:
                 if (schemas.EntryFields.macrostructure in fields) or (
                     schemas.EntryFields.structure in fields
                 ):
                     macrostructure = entry.macrostructure()
                     if macrostructure is not None:
-                        structure["macro"] = dataclasses.asdict(macrostructure)
+                        structure["macro"] = asdict(macrostructure)
                 if (schemas.EntryFields.microstructure in fields) or (
                     schemas.EntryFields.structure in fields
                 ):
                     if entry.structure_family == "node":
                         assert False  # not sure if this ever happens
                         pass
                     elif entry.structure_family == "dataframe":
@@ -527,15 +557,15 @@
                         structure["micro"] = {
                             "meta": meta,
                             "divisions": divisions,
                         }
                     else:
                         microstructure = entry.microstructure()
                         if microstructure is not None:
-                            structure["micro"] = dataclasses.asdict(microstructure)
+                            structure["micro"] = asdict(microstructure)
                 if entry.structure_family == "array":
                     shape = structure.get("macro", {}).get("shape")
                     if shape is None:
                         # The client did not request structure so we have not yet
                         # accessed it, and we have access it specifically to construct this link.
                         shape = entry.macrostructure().shape
                     block_template = ",".join(
@@ -725,7 +755,15 @@
 
 FULL_LINKS = {
     "node": {"full": "{base_url}/node/full/{path}"},
     "array": {"full": "{base_url}/array/full/{path}"},
     "dataframe": {"full": "{base_url}/node/full/{path}"},
     "sparse": {"full": "{base_url}/array/full/{path}"},
 }
+
+
+def asdict(dc):
+    "Compat for converting dataclass or pydantic.BaseModel to dict."
+    try:
+        return dataclasses.asdict(dc)
+    except TypeError:
+        return dict(dc)
```

### Comparing `tiled-0.1.0a93/tiled/server/dependencies.py` & `tiled-0.1.0a94/tiled/server/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,135 +1,126 @@
-from functools import lru_cache
-from typing import Optional
+import contextlib
+import inspect
+import time
+from typing import Any, Callable
 
-import pydantic
-from fastapi import Depends, HTTPException, Query, Request, Security
+import anyio
 
-from ..media_type_registration import (
-    serialization_registry as default_serialization_registry,
-)
-from ..query_registration import query_registry as default_query_registry
-from ..validation_registration import validation_registry as default_validation_registry
-from .authentication import get_current_principal
-from .core import NoEntry
-from .utils import filter_for_access, record_timing
+from ..access_policies import NO_ACCESS
+from ..adapters.mapping import MapAdapter
+from ..structures.array import ArrayStructure
+from ..structures.dataframe import DataFrameStructure
 
+EMPTY_NODE = MapAdapter({})
+API_KEY_COOKIE_NAME = "tiled_api_key"
+API_KEY_QUERY_PARAMETER = "api_key"
+CSRF_COOKIE_NAME = "tiled_csrf"
 
-@lru_cache(1)
-def get_query_registry():
-    "This may be overridden via dependency_overrides."
-    return default_query_registry
 
-
-@lru_cache(1)
-def get_serialization_registry():
-    "This may be overridden via dependency_overrides."
-    return default_serialization_registry
-
-
-@lru_cache(1)
-def get_validation_registry():
-    "This may be overridden via dependency_overrides."
-    return default_validation_registry
-
-
-def get_root_tree():
+def get_authenticators():
     raise NotImplementedError(
         "This should be overridden via dependency_overrides. "
         "See tiled.server.app.build_app()."
     )
 
 
-def SecureEntry(scopes):
-    def inner(
-        path: str,
-        request: Request,
-        principal: str = Depends(get_current_principal),
-        root_tree: pydantic.BaseSettings = Depends(get_root_tree),
-    ):
-        """
-        Obtain a node in the tree from its path.
-
-        Walk down the path from the root tree, filtering each intermediate node by
-        'read:metadata' and finally filtering by the specified scope.
-        """
-        path_parts = [segment for segment in path.split("/") if segment]
-        entry = root_tree
-        try:
-            # Traverse into sub-tree(s). This requires only 'read:metadata' scope.
-            for segment in path_parts:
-                entry = filter_for_access(
-                    entry, principal, ["read:metadata"], request.state.metrics
-                )
-                try:
-                    entry = entry[segment]
-                except (KeyError, TypeError):
-                    raise NoEntry(path_parts)
-            # Now check that we have the requested scope on the final node.
-            access_policy = getattr(entry, "access_policy", None)
-            if access_policy is not None:
-                with record_timing(request.state.metrics, "acl"):
-                    allowed_scopes = entry.access_policy.allowed_scopes(
-                        entry, principal
-                    )
-                    if not set(scopes).issubset(allowed_scopes):
-                        if "read:metadata" not in allowed_scopes:
-                            # If you can't read metadata, it does not exit for you.
-                            raise NoEntry(path_parts)
-                        else:
-                            # You can see this, but you cannot perform the requested
-                            # operation on it.
-                            raise HTTPException(
-                                status_code=403,
-                                detail=(
-                                    "Not enough permissions to perform this action on this node. "
-                                    f"Requires scopes {scopes}. "
-                                    f"Principal had scopes {list(allowed_scopes)} on this node."
-                                ),
-                            )
-        except NoEntry:
-            raise HTTPException(status_code=404, detail=f"No such entry: {path_parts}")
-        return entry
-
-    return Security(inner, scopes=scopes)
-
-
-def block(
-    # Ellipsis as the "default" tells FastAPI to make this parameter required.
-    block: str = Query(..., regex="^[0-9]*(,[0-9]+)*$"),
-):
-    "Specify and parse a block index parameter."
-    if not block:
-        return ()
-    return tuple(map(int, block.split(",")))
-
-
-def expected_shape(
-    expected_shape: Optional[str] = Query(
-        None, min_length=1, regex="^[0-9]+(,[0-9]+)*$|^scalar$"
-    ),
-):
-    "Specify and parse an expected_shape parameter."
-    if expected_shape is None:
-        return
-    if expected_shape == "scalar":
-        return ()
-    return tuple(map(int, expected_shape.split(",")))
-
-
-def slice_(
-    slice: str = Query(None, regex="^[-0-9,:]*$"),
-):
-    "Specify and parse a block index parameter."
-    import numpy
-
-    # IMPORTANT We are eval-ing a user-provider string here so we need to be
-    # very careful about locking down what can be in it. The regex above
-    # excludes any letters or operators, so it is not possible to execute
-    # functions or expensive arithmetic.
-    return tuple(
-        [
-            eval(f"numpy.s_[{dim!s}]", {"numpy": numpy})
-            for dim in (slice or "").split(",")
-            if dim
-        ]
-    )
+@contextlib.contextmanager
+def record_timing(metrics, key):
+    """
+    Set timings[key] equal to the run time (in milliseconds) of the context body.
+    """
+    t0 = time.perf_counter()
+    yield
+    metrics[key]["dur"] += time.perf_counter() - t0  # Units: seconds
+
+
+def get_root_url(request):
+    """
+    URL at which the app is being server, including API and UI
+    """
+    return f"{get_root_url_low_level(request.headers, request.scope)}"
+
+
+def get_base_url(request):
+    """
+    Base URL for the API
+    """
+    return f"{get_root_url(request)}/api/v1"
+
+
+def get_root_url_low_level(request_headers, scope):
+    # We want to get the scheme, host, and root_path (if any)
+    # *as it appears to the client* for use in assembling links to
+    # include in our responses.
+    #
+    # We need to consider:
+    #
+    # * FastAPI may be behind a load balancer, such that for a client request
+    #   like "https://example.com/..." the Host header is set to something
+    #   like "localhost:8000" and the request.url.scheme is "http".
+    #   We consult X-Forwarded-* headers to get the original Host and scheme.
+    #   Note that, although these are a de facto standard, they may not be
+    #   set by default. With nginx, for example, they need to be configured.
+    #
+    # * The client may be connecting through SSH port-forwarding. (This
+    #   is a niche use case but one that we nonetheless care about.)
+    #   The Host or X-Forwarded-Host header may include a non-default port.
+    #   The HTTP spec specifies that the Host header may include a port
+    #   to specify a non-default port.
+    #   https://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.23
+    host = request_headers.get("x-forwarded-host", request_headers["host"])
+    scheme = request_headers.get("x-forwarded-proto", scope["scheme"])
+    root_path = scope.get("root_path", "")
+    if root_path.endswith("/"):
+        root_path = root_path[:-1]
+    return f"{scheme}://{host}{root_path}"
+
+
+def filter_for_access(entry, principal, scopes, metrics):
+    access_policy = getattr(entry, "access_policy", None)
+    if access_policy is not None:
+        with record_timing(metrics, "acl"):
+            queries = entry.access_policy.filters(entry, principal, set(scopes))
+            if queries is NO_ACCESS:
+                entry = EMPTY_NODE
+            else:
+                for query in queries:
+                    entry = entry.search(query)
+    return entry
+
+
+def get_structure(entry):
+    "Abtract over the fact that some have micro/macrostructure."
+    structure_family = entry.structure_family
+    if structure_family == "node":
+        structure = None
+    elif structure_family == "array":
+        structure = ArrayStructure(
+            macro=entry.macrostructure(),
+            micro=entry.microstructure(),
+        )
+    elif structure_family == "dataframe":
+        structure = DataFrameStructure(
+            macro=entry.macrostructure(),
+            micro=entry.microstructure(),
+        )
+    elif structure_family == "sparse":
+        structure = entry.structure()
+    else:
+        raise ValueError(f"Unrecognized structure family {structure_family}")
+    return structure
+
+
+def is_coroutine_callable(call: Callable[..., Any]) -> bool:
+    if inspect.isroutine(call):
+        return inspect.iscoroutinefunction(call)
+    if inspect.isclass(call):
+        return False
+    dunder_call = getattr(call, "__call__", None)  # noqa: B004
+    return inspect.iscoroutinefunction(dunder_call)
+
+
+async def ensure_awaitable(func, *args):
+    if is_coroutine_callable(func):
+        return await func(*args)
+    else:
+        return await anyio.to_thread.run_sync(func, *args)
```

### Comparing `tiled-0.1.0a93/tiled/server/etag.py` & `tiled-0.1.0a94/tiled/server/etag.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/server/metrics.py` & `tiled-0.1.0a94/tiled/server/metrics.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/server/object_cache.py` & `tiled-0.1.0a94/tiled/server/object_cache.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/server/pydantic_array.py` & `tiled-0.1.0a94/tiled/server/pydantic_array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/server/pydantic_dataframe.py` & `tiled-0.1.0a94/tiled/server/pydantic_dataframe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Tuple, Union
 
 import pandas
 from pydantic import BaseModel
 
 from ..media_type_registration import deserialization_registry
-from ..serialization.dataframe import serialize_arrow
+from ..serialization.dataframe import deserialize_arrow, serialize_arrow
 from ..utils import APACHE_ARROW_FILE_MIME_TYPE
 
 
 class DataFrameMicroStructure(BaseModel):
     meta: bytes
     divisions: bytes
 
@@ -36,14 +36,23 @@
         ddf = dask.dataframe.from_pandas(df, npartitions=1)
         meta = bytes(serialize_arrow(dask.dataframe.utils.make_meta(ddf), {}))
         divisions = bytes(
             serialize_arrow(pandas.DataFrame({"divisions": list(ddf.divisions)}), {})
         )
         return cls(meta=meta, divisions=divisions)
 
+    @property
+    def meta_decoded(self):
+        return deserialize_arrow(self.meta)
+
+    @property
+    def divisions_decoded(self):
+        divisions_wrapped_in_df = deserialize_arrow(self.divisions)
+        return tuple(divisions_wrapped_in_df["divisions"].values)
+
 
 class DataFrameMacroStructure(BaseModel):
     npartitions: int
     columns: List[str]
     resizable: Union[bool, Tuple[bool, ...]] = False
 
     @classmethod
```

### Comparing `tiled-0.1.0a93/tiled/server/pydantic_sparse.py` & `tiled-0.1.0a94/tiled/server/pydantic_sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/server/router.py` & `tiled-0.1.0a94/tiled/server/router.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
 import dataclasses
 import inspect
 from datetime import datetime, timedelta
+from functools import partial
 from typing import Any, List, Optional
 
 from fastapi import APIRouter, Depends, HTTPException, Query, Request, Security
 from jmespath.exceptions import JMESPathError
 from pydantic import BaseSettings
 
 from .. import __version__
@@ -25,25 +26,27 @@
     construct_entries_response,
     construct_resource,
     construct_revisions_response,
     json_or_msgpack,
     resolve_media_type,
 )
 from .dependencies import (
+    EntryKind,
     SecureEntry,
     block,
     expected_shape,
+    get_deserialization_registry,
     get_query_registry,
     get_serialization_registry,
     get_validation_registry,
     slice_,
 )
 from .settings import get_settings
 from .utils import (
-    FilteredNode,
+    ensure_awaitable,
     filter_for_access,
     get_base_url,
     get_structure,
     record_timing,
 )
 
 router = APIRouter()
@@ -145,36 +148,38 @@
     offset: Optional[int] = Query(0, alias="page[offset]", ge=0),
     limit: Optional[int] = Query(
         DEFAULT_PAGE_SIZE, alias="page[limit]", ge=0, le=MAX_PAGE_SIZE
     ),
     sort: Optional[str] = Query(None),
     max_depth: Optional[int] = Query(None, ge=0, le=DEPTH_LIMIT),
     omit_links: bool = Query(False),
-    entry: Any = SecureEntry(scopes=["read:metadata"]),
+    show_sources: bool = Query(False),
+    entry: Any = SecureEntry(scopes=["read:metadata"], kind=EntryKind.adapter),
     query_registry=Depends(get_query_registry),
     principal: str = Depends(get_current_principal),
     **filters,
 ):
     request.state.endpoint = "search"
     if entry.structure_family != "node":
         raise WrongTypeForRoute("This is not a Node; it cannot be searched or listed.")
     entry = filter_for_access(
         entry, principal, ["read:metadata"], request.state.metrics
     )
     try:
-        resource, metadata_stale_at, must_revalidate = construct_entries_response(
+        resource, metadata_stale_at, must_revalidate = await construct_entries_response(
             query_registry,
             entry,
             "/node/search",
             path,
             offset,
             limit,
             fields,
             select_metadata,
             omit_links,
+            show_sources,
             filters,
             sort,
             get_base_url(request),
             resolve_media_type(request),
             max_depth=max_depth,
         )
         # We only get one Expires header, so if different parts
@@ -207,15 +212,15 @@
 
 async def node_distinct(
     request: Request,
     structure_families: bool = False,
     specs: bool = False,
     metadata: Optional[List[str]] = Query(default=[]),
     counts: bool = False,
-    entry: Any = SecureEntry(scopes=["read:metadata"]),
+    entry: Any = SecureEntry(scopes=["read:metadata"], kind=EntryKind.node),
     query_registry=Depends(get_query_registry),
     **filters,
 ):
     if hasattr(entry, "get_distinct"):
         distinct = apply_search(entry, filters, query_registry).get_distinct(
             metadata=metadata,
             structure_families=structure_families,
@@ -301,30 +306,32 @@
 async def node_metadata(
     request: Request,
     path: str,
     fields: Optional[List[schemas.EntryFields]] = Query(list(schemas.EntryFields)),
     select_metadata: Optional[str] = Query(None),
     max_depth: Optional[int] = Query(None, ge=0, le=DEPTH_LIMIT),
     omit_links: bool = Query(False),
-    entry: Any = SecureEntry(scopes=["read:metadata"]),
+    show_sources: bool = Query(False),
+    entry: Any = SecureEntry(scopes=["read:metadata"], kind=EntryKind.node),
     root_path: bool = Query(False),
 ):
     "Fetch the metadata and structure information for one entry."
 
     request.state.endpoint = "metadata"
     base_url = get_base_url(request)
     path_parts = [segment for segment in path.split("/") if segment]
     try:
-        resource = construct_resource(
+        resource = await construct_resource(
             base_url,
             path_parts,
             entry,
             fields,
             select_metadata,
             omit_links,
+            show_sources,
             resolve_media_type(request),
             max_depth=max_depth,
         )
     except JMESPathError as err:
         raise HTTPException(
             status_code=400,
             detail=f"Malformed 'select_metadata' parameter raised JMESPathError: {err}",
@@ -336,15 +343,15 @@
         expires=getattr(entry, "metadata_stale_at", None),
     )
 
 
 @router.get(
     "/array/block/{path:path}", response_model=schemas.Response, name="array block"
 )
-def array_block(
+async def array_block(
     request: Request,
     entry=SecureEntry(scopes=["read:data"]),
     block=Depends(block),
     slice=Depends(slice_),
     expected_shape=Depends(expected_shape),
     format: Optional[str] = None,
     filename: Optional[str] = None,
@@ -377,19 +384,19 @@
         # Handle special case of numpy scalar.
         if shape != ():
             raise HTTPException(
                 status_code=400,
                 detail=f"Requested scalar but shape is {entry.macrostructure().shape}",
             )
         with record_timing(request.state.metrics, "read"):
-            array = entry.read()
+            array = await ensure_awaitable(entry.read)
     else:
         try:
             with record_timing(request.state.metrics, "read"):
-                array = entry.read_block(block, slice=slice)
+                array = await ensure_awaitable(entry.read_block, block, slice)
         except IndexError:
             raise HTTPException(status_code=400, detail="Block index out of range")
         if (expected_shape is not None) and (expected_shape != array.shape):
             raise HTTPException(
                 status_code=400,
                 detail=f"The expected_shape {expected_shape} does not match the actual shape {array.shape}",
             )
@@ -399,15 +406,15 @@
             detail=(
                 f"Response would exceed {settings.response_bytesize_limit}. "
                 "Use slicing ('?slice=...') to request smaller chunks."
             ),
         )
     try:
         with record_timing(request.state.metrics, "pack"):
-            return construct_data_response(
+            return await construct_data_response(
                 entry.structure_family,
                 serialization_registry,
                 array,
                 entry.metadata,
                 request,
                 format,
                 specs=getattr(entry, "specs", []),
@@ -418,15 +425,15 @@
         # raise HTTPException(status_code=406, detail=", ".join(err.supported))
         raise HTTPException(status_code=406, detail=err.args[0])
 
 
 @router.get(
     "/array/full/{path:path}", response_model=schemas.Response, name="full array"
 )
-def array_full(
+async def array_full(
     request: Request,
     entry=SecureEntry(scopes=["read:data"]),
     slice=Depends(slice_),
     expected_shape=Depends(expected_shape),
     format: Optional[str] = None,
     filename: Optional[str] = None,
     serialization_registry=Depends(get_serialization_registry),
@@ -443,15 +450,15 @@
         )
     # Deferred import because this is not a required dependency of the server
     # for some use cases.
     import numpy
 
     try:
         with record_timing(request.state.metrics, "read"):
-            array = entry.read(slice)
+            array = await ensure_awaitable(entry.read, slice)
         if structure_family == "array":
             array = numpy.asarray(array)  # Force dask or PIMS or ... to do I/O.
     except IndexError:
         raise HTTPException(status_code=400, detail="Block index out of range")
     if (expected_shape is not None) and (expected_shape != array.shape):
         raise HTTPException(
             status_code=400,
@@ -463,15 +470,15 @@
             detail=(
                 f"Response would exceed {settings.response_bytesize_limit}. "
                 "Use slicing ('?slice=...') to request smaller chunks."
             ),
         )
     try:
         with record_timing(request.state.metrics, "pack"):
-            return construct_data_response(
+            return await construct_data_response(
                 structure_family,
                 serialization_registry,
                 array,
                 entry.metadata,
                 request,
                 format,
                 specs=getattr(entry, "specs", []),
@@ -483,15 +490,15 @@
 
 
 @router.get(
     "/dataframe/partition/{path:path}",
     response_model=schemas.Response,
     name="dataframe partition",
 )
-def dataframe_partition(
+async def dataframe_partition(
     request: Request,
     partition: int,
     entry=SecureEntry(scopes=["read:data"]),
     field: Optional[List[str]] = Query(None, min_length=1),
     format: Optional[str] = None,
     filename: Optional[str] = None,
     serialization_registry=Depends(get_serialization_registry),
@@ -505,15 +512,15 @@
             status_code=404,
             detail=f"Cannot read {entry.structure_family} structure with /dataframe/partition route.",
         )
     try:
         # The singular/plural mismatch here of "fields" and "field" is
         # due to the ?field=A&field=B&field=C... encodes in a URL.
         with record_timing(request.state.metrics, "read"):
-            df = entry.read_partition(partition, fields=field)
+            df = await ensure_awaitable(entry.read_partition, partition, field)
     except IndexError:
         raise HTTPException(status_code=400, detail="Partition out of range")
     except KeyError as err:
         (key,) = err.args
         raise HTTPException(status_code=400, detail=f"No such field {key}.")
     if df.memory_usage().sum() > settings.response_bytesize_limit:
         raise HTTPException(
@@ -522,15 +529,15 @@
                 f"Response would exceed {settings.response_bytesize_limit}. "
                 "Select a subset of the columns ('?field=...') to "
                 "request a smaller chunks."
             ),
         )
     try:
         with record_timing(request.state.metrics, "pack"):
-            return construct_data_response(
+            return await construct_data_response(
                 "dataframe",
                 serialization_registry,
                 df,
                 entry.metadata,
                 request,
                 format,
                 specs=getattr(entry, "specs", []),
@@ -542,32 +549,30 @@
 
 
 @router.get(
     "/node/full/{path:path}",
     response_model=schemas.Response,
     name="full generic 'node' or 'dataframe'",
 )
-def node_full(
+async def node_full(
     request: Request,
     entry=SecureEntry(scopes=["read:data"]),
     principal: str = Depends(get_current_principal),
     field: Optional[List[str]] = Query(None, min_length=1),
     format: Optional[str] = None,
     filename: Optional[str] = None,
     serialization_registry=Depends(get_serialization_registry),
     settings: BaseSettings = Depends(get_settings),
 ):
     """
     Fetch the data below the given node.
     """
     try:
-        # The singular/plural mismatch here of "fields" and "field" is
-        # due to the ?field=A&field=B&field=C... encodes in a URL.
         with record_timing(request.state.metrics, "read"):
-            data = entry.read(fields=field)
+            data = await ensure_awaitable(entry.read, field)
     except KeyError as err:
         (key,) = err.args
         raise HTTPException(status_code=400, detail=f"No such field {key}.")
     if (entry.structure_family == "dataframe") and (
         data.memory_usage().sum() > settings.response_bytesize_limit
     ):
         raise HTTPException(
@@ -575,59 +580,77 @@
             detail=(
                 f"Response would exceed {settings.response_bytesize_limit}. "
                 "Select a subset of the columns ('?field=...') to "
                 "request a smaller chunks."
             ),
         )
     if entry.structure_family == "node":
-        data = FilteredNode(data, principal, ["read:data"], request.state.metrics)
+        curried_filter = partial(
+            filter_for_access,
+            principal=principal,
+            scopes=["read:data"],
+            metrics=request.state.metrics,
+        )
+    else:
+        curried_filter = None
         # TODO Walk node to determine size before handing off to serializer.
     try:
         with record_timing(request.state.metrics, "pack"):
-            return construct_data_response(
+            return await construct_data_response(
                 entry.structure_family,
                 serialization_registry,
                 data,
                 entry.metadata,
                 request,
                 format,
                 specs=getattr(entry, "specs", []),
                 expires=getattr(entry, "content_stale_at", None),
                 filename=filename,
+                filter_for_access=curried_filter,
             )
     except UnsupportedMediaTypes as err:
         raise HTTPException(status_code=406, detail=err.args[0])
 
 
 @router.post("/node/metadata/{path:path}", response_model=schemas.PostMetadataResponse)
-def post_metadata(
+async def post_metadata(
     request: Request,
     path: str,
     body: schemas.PostMetadataRequest,
     validation_registry=Depends(get_validation_registry),
     settings: BaseSettings = Depends(get_settings),
-    entry=SecureEntry(scopes=["write:metadata", "create"]),
+    entry=SecureEntry(scopes=["write:metadata", "create"], kind=EntryKind.adapter),
 ):
-    if not hasattr(entry, "post_metadata"):
-        raise HTTPException(status_code=405, detail="This path cannot accept metadata.")
+    if not getattr(entry, "writable", False):
+        raise HTTPException(
+            status_code=405, detail=f"Data cannot be written at the path {path}"
+        )
 
     if body.structure_family == StructureFamily.dataframe:
         # Decode meta for pydantic validation
-        body.structure.micro.meta = base64.b64decode(body.structure.micro.meta)
-        body.structure.micro.divisions = base64.b64decode(
-            body.structure.micro.divisions
+        # TODO This is fragile.
+        body.data_sources[0].structure.micro.meta = base64.b64decode(
+            body.data_sources[0].structure.micro.meta
+        )
+        body.data_sources[0].structure.micro.divisions = base64.b64decode(
+            body.data_sources[0].structure.micro.divisions
         )
 
-    metadata, structure_family, structure, specs, references = (
+    metadata, structure_family, specs, references = (
         body.metadata,
         body.structure_family,
-        body.structure,
         body.specs,
         body.references,
     )
+    if structure_family == StructureFamily.node:
+        structure = None
+    else:
+        if len(body.data_sources) != 1:
+            raise NotImplementedError
+        structure = body.data_sources[0].structure
 
     metadata_modified = False
 
     # Specs should be ordered from most specific/constrained to least.
     # Validate them in reverse order, with the least constrained spec first,
     # because it may do normalization that helps pass the more constrained one.
     # Known Issue:
@@ -652,141 +675,178 @@
                     status_code=400,
                     detail=f"failed validation for spec {spec.name}:\n{e}",
                 )
             if result is not None:
                 metadata_modified = True
                 metadata = result
 
-    key = entry.post_metadata(
+    key, node = await entry.create_node(
         metadata=body.metadata,
         structure_family=body.structure_family,
-        structure=body.structure,
+        key=body.id,
         specs=body.specs,
         references=body.references,
+        data_sources=body.data_sources,
     )
     links = {}
     base_url = get_base_url(request)
     path_parts = [segment for segment in path.split("/") if segment] + [key]
     path_str = "/".join(path_parts)
     links["self"] = f"{base_url}/node/metadata/{path_str}"
     if body.structure_family == StructureFamily.array:
         block_template = ",".join(
-            f"{{{index}}}" for index in range(len(body.structure.macro.shape))
+            f"{{{index}}}" for index in range(len(node.structure.macro.shape))
         )
         links["block"] = f"{base_url}/array/block/{path_str}?block={block_template}"
         links["full"] = f"{base_url}/array/full/{path_str}"
     elif body.structure_family == StructureFamily.sparse:
         # Different from array because of structure.macro.shape vs structure.shape
         # Can be unified if we drop macro/micro namespace.
         block_template = ",".join(
-            f"{{{index}}}" for index in range(len(body.structure.shape))
+            f"{{{index}}}" for index in range(len(node.structure.shape))
         )
         links["block"] = f"{base_url}/array/block/{path_str}?block={block_template}"
         links["full"] = f"{base_url}/array/full/{path_str}"
     elif body.structure_family == StructureFamily.dataframe:
         links[
             "partition"
         ] = f"{base_url}/dataframe/partition/{path_str}?partition={{index}}"
         links["full"] = f"{base_url}/node/full/{path_str}"
+    elif body.structure_family == StructureFamily.node:
+        links["full"] = f"{base_url}/node/full/{path_str}"
+        links["search"] = f"{base_url}/node/search/{path_str}"
     else:
         raise NotImplementedError(body.structure_family)
-    response_data = {"id": key, "links": links}
+    response_data = {
+        "id": key,
+        "links": links,
+        "data_sources": [ds.dict() for ds in node.data_sources],
+    }
     if metadata_modified:
         response_data["metadata"] = metadata
     return json_or_msgpack(request, response_data)
 
 
 @router.delete("/node/metadata/{path:path}")
 async def delete(
     request: Request,
-    entry=SecureEntry(scopes=["write:data", "write:metadata"]),
+    entry=SecureEntry(scopes=["write:data", "write:metadata"], kind=EntryKind.node),
 ):
     if hasattr(entry, "delete"):
         entry.delete()
     else:
         raise HTTPException(
             status_code=405, detail="This path does not support deletion."
         )
     return json_or_msgpack(request, None)
 
 
 @router.put("/array/full/{path:path}")
 async def put_array_full(
     request: Request,
     entry=SecureEntry(scopes=["write:data"]),
+    deserialization_registry=Depends(get_deserialization_registry),
 ):
-    data = await request.body()
-    if hasattr(entry, "put_data"):
-        entry.put_data(data)
-    else:
+    body = await request.body()
+    if not hasattr(entry, "write"):
         raise HTTPException(
             status_code=405, detail="This path cannot accept array data."
         )
+    media_type = request.headers["content-type"]
+    if entry.structure_family == "array":
+        dtype = entry.microstructure().to_numpy_dtype()
+        shape = entry.macrostructure().shape
+        deserializer = deserialization_registry.dispatch("array", media_type)
+        data = await ensure_awaitable(deserializer, body, dtype, shape)
+    elif entry.structure_family == "sparse":
+        deserializer = deserialization_registry.dispatch("sparse", media_type)
+        data = await ensure_awaitable(deserializer, body)
+    else:
+        raise NotImplementedError(entry.structure_family)
+    await ensure_awaitable(entry.write, data)
     return json_or_msgpack(request, None)
 
 
 @router.put("/array/block/{path:path}")
 async def put_array_block(
     request: Request,
     entry=SecureEntry(scopes=["write:data"]),
+    deserialization_registry=Depends(get_deserialization_registry),
     block=Depends(block),
 ):
-    data = await request.body()
-
-    if hasattr(entry, "put_data"):
-        entry.put_data(data, block=block)
-    else:
+    if not hasattr(entry, "write_block"):
         raise HTTPException(
             status_code=405, detail="This path cannot accept array data."
         )
+    from tiled.adapters.array import slice_and_shape_from_block_and_chunks
+
+    body = await request.body()
+    media_type = request.headers["content-type"]
+    if entry.structure_family == "array":
+        dtype = entry.microstructure().to_numpy_dtype()
+        _, shape = slice_and_shape_from_block_and_chunks(
+            block, entry.macrostructure().chunks
+        )
+        deserializer = deserialization_registry.dispatch("array", media_type)
+        data = await ensure_awaitable(deserializer, body, dtype, shape)
+    elif entry.structure_family == "sparse":
+        deserializer = deserialization_registry.dispatch("sparse", media_type)
+        data = await ensure_awaitable(deserializer, body)
+    else:
+        raise NotImplementedError(entry.structure_family)
+    await ensure_awaitable(entry.write_block, data, block)
     return json_or_msgpack(request, None)
 
 
 @router.put("/node/full/{path:path}")
 async def put_dataframe_full(
     request: Request,
     entry=SecureEntry(scopes=["write:data"]),
+    deserialization_registry=Depends(get_deserialization_registry),
 ):
-    data = await request.body()
-
-    if hasattr(entry, "put_data"):
-        entry.put_data(data)
-    else:
+    if not hasattr(entry, "write"):
         raise HTTPException(
             status_code=405, detail="This path cannot accept dataframe data."
         )
+    body = await request.body()
+    media_type = request.headers["content-type"]
+    deserializer = deserialization_registry.dispatch("dataframe", media_type)
+    data = await ensure_awaitable(deserializer, body)
+    await ensure_awaitable(entry.write, data)
     return json_or_msgpack(request, None)
 
 
 @router.put("/dataframe/partition/{path:path}")
 async def put_dataframe_partition(
     partition: int,
     request: Request,
     entry=SecureEntry(scopes=["write:data"]),
+    deserialization_registry=Depends(get_deserialization_registry),
 ):
-    data = await request.body()
-
-    if hasattr(entry, "put_data"):
-        entry.put_data(data, partition=partition)
-    else:
+    if not hasattr(entry, "write_partition"):
         raise HTTPException(
             status_code=405, detail="This path cannot accept dataframe data."
         )
+    body = await request.body()
+    media_type = request.headers["content-type"]
+    deserializer = deserialization_registry.dispatch("dataframe", media_type)
+    data = await ensure_awaitable(deserializer, body)
+    await ensure_awaitable(entry.write_partition, data, partition)
     return json_or_msgpack(request, None)
 
 
-@router.put("/node/metadata/{path:path}")
+@router.put("/node/metadata/{path:path}", response_model=schemas.PutMetadataResponse)
 async def put_metadata(
     request: Request,
     body: schemas.PutMetadataRequest,
     validation_registry=Depends(get_validation_registry),
     settings: BaseSettings = Depends(get_settings),
-    entry=SecureEntry(scopes=["write:metadata"]),
+    entry=SecureEntry(scopes=["write:metadata"], kind=EntryKind.node),
 ):
-    if not hasattr(entry, "put_metadata"):
+    if not hasattr(entry, "update_metadata"):
         raise HTTPException(
             status_code=405, detail="This path does not support update of metadata."
         )
 
     metadata, structure_family, structure, specs, references = (
         body.metadata if body.metadata is not None else entry.metadata,
         entry.structure_family,
@@ -822,55 +882,57 @@
                     status_code=400,
                     detail=f"failed validation for spec {spec.name}:\n{e}",
                 )
             if result is not None:
                 metadata_modified = True
                 metadata = result
 
-    entry.put_metadata(metadata=metadata, specs=specs, references=references)
+    await entry.update_metadata(metadata=metadata, specs=specs, references=references)
 
     response_data = {"id": entry.key}
     if metadata_modified:
         response_data["metadata"] = metadata
     return json_or_msgpack(request, response_data)
 
 
 @router.get("/node/revisions/{path:path}")
-async def node_revisions(
+async def get_revisions(
     request: Request,
     path: str,
     offset: Optional[int] = Query(0, alias="page[offset]", ge=0),
     limit: Optional[int] = Query(
         DEFAULT_PAGE_SIZE, alias="page[limit]", ge=0, le=MAX_PAGE_SIZE
     ),
-    entry=SecureEntry(scopes=["read:metadata"]),
+    entry=SecureEntry(scopes=["read:metadata"], kind=EntryKind.node),
 ):
     if not hasattr(entry, "revisions"):
         raise HTTPException(
-            status_code=405, detail="This path does not support update of metadata."
+            status_code=405, detail="This path does not support revisions."
         )
 
     base_url = get_base_url(request)
-    resource = construct_revisions_response(
+    resource = await construct_revisions_response(
         entry,
         base_url,
         "/node/revisions",
         path,
         offset,
         limit,
         resolve_media_type(request),
     )
     return json_or_msgpack(request, resource.dict())
 
 
 @router.delete("/node/revisions/{path:path}")
-async def revisions_delitem(
-    request: Request, n: int, entry=SecureEntry(scopes=["write:metadata"])
+async def delete_revision(
+    request: Request,
+    number: int,
+    entry=SecureEntry(scopes=["write:metadata"], kind=EntryKind.node),
 ):
     if not hasattr(entry, "revisions"):
         raise HTTPException(
             status_code=405,
             detail="This path does not support a del request for revisions.",
         )
 
-    entry.revisions.delete_revision(n)
+    await entry.delete_revision(number)
     return json_or_msgpack(request, None)
```

### Comparing `tiled-0.1.0a93/tiled/server/settings.py` & `tiled-0.1.0a94/tiled/server/settings.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/structures/array.py` & `tiled-0.1.0a94/tiled/structures/array.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/structures/core.py` & `tiled-0.1.0a94/tiled/structures/core.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/structures/dataframe.py` & `tiled-0.1.0a94/tiled/structures/dataframe.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/structures/sparse.py` & `tiled-0.1.0a94/tiled/structures/sparse.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/utils.py` & `tiled-0.1.0a94/tiled/utils.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled/validation_registration.py` & `tiled-0.1.0a94/tiled/validation_registration.py`

 * *Files identical despite different names*

### Comparing `tiled-0.1.0a93/tiled.egg-info/PKG-INFO` & `tiled-0.1.0a94/tiled.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiled
-Version: 0.1.0a93
+Version: 0.1.0a94
 Summary: Tile-based access to SciPy/PyData data structures over the web in many formats
 Home-page: https://github.com/bluesky/tiled
 Author: Bluesky Collaboration
 Author-email: dallan@bnl.gov
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `tiled-0.1.0a93/tiled.egg-info/SOURCES.txt` & `tiled-0.1.0a94/tiled.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -270,14 +270,15 @@
 tiled/_tests/conftest.py
 tiled/_tests/test_access_control.py
 tiled/_tests/test_allow_origins.py
 tiled/_tests/test_array.py
 tiled/_tests/test_authentication.py
 tiled/_tests/test_authenticators.py
 tiled/_tests/test_caches.py
+tiled/_tests/test_catalog.py
 tiled/_tests/test_client.py
 tiled/_tests/test_client_cache.py
 tiled/_tests/test_config.py
 tiled/_tests/test_custom_format.py
 tiled/_tests/test_dataframe.py
 tiled/_tests/test_directory_walker.py
 tiled/_tests/test_distinct.py
@@ -295,43 +296,49 @@
 tiled/_tests/test_pickle.py
 tiled/_tests/test_queries.py
 tiled/_tests/test_routes.py
 tiled/_tests/test_scaled_config_option.py
 tiled/_tests/test_search.py
 tiled/_tests/test_sentinel.py
 tiled/_tests/test_size_limit.py
-tiled/_tests/test_slash.py
 tiled/_tests/test_sort.py
 tiled/_tests/test_sparse.py
 tiled/_tests/test_specs_and_references.py
 tiled/_tests/test_structured_array.py
 tiled/_tests/test_tiff.py
 tiled/_tests/test_tokenize.py
 tiled/_tests/test_validation.py
 tiled/_tests/test_writing.py
 tiled/_tests/test_xarray.py
 tiled/_tests/utils.py
-tiled/_tests/writable_adapters.py
 tiled/_tests/test_configs/config_missing_api_key.yml
 tiled/_tests/test_configs/config_missing_secret_keys.yml
 tiled/_tests/test_configs/config_missing_secret_keys_public.yml
 tiled/_tests/test_configs/config_public_no_authenticator.yml
 tiled/_tests/test_configs/config_with_api_key.yml
 tiled/_tests/test_configs/config_with_secret_keys.yml
 tiled/adapters/__init__.py
 tiled/adapters/array.py
 tiled/adapters/dataframe.py
 tiled/adapters/excel.py
 tiled/adapters/files.py
 tiled/adapters/hdf5.py
 tiled/adapters/mapping.py
+tiled/adapters/parquet.py
 tiled/adapters/sparse.py
+tiled/adapters/sparse_blocks_parquet.py
 tiled/adapters/tiff.py
 tiled/adapters/utils.py
 tiled/adapters/xarray.py
+tiled/adapters/zarr.py
+tiled/catalog/__init__.py
+tiled/catalog/adapter.py
+tiled/catalog/base.py
+tiled/catalog/explain.py
+tiled/catalog/orm.py
 tiled/client/__init__.py
 tiled/client/_testclient.py
 tiled/client/array.py
 tiled/client/auth.py
 tiled/client/base.py
 tiled/client/cache.py
 tiled/client/constructors.py
@@ -340,14 +347,15 @@
 tiled/client/node.py
 tiled/client/sparse.py
 tiled/client/utils.py
 tiled/client/xarray.py
 tiled/commandline/__init__.py
 tiled/commandline/_admin.py
 tiled/commandline/_api_key.py
+tiled/commandline/_catalog.py
 tiled/commandline/_profile.py
 tiled/commandline/_serve.py
 tiled/commandline/_utils.py
 tiled/commandline/main.py
 tiled/config_schemas/client_profiles.yml
 tiled/config_schemas/service_configuration.yml
 tiled/database/__init__.py
```

### Comparing `tiled-0.1.0a93/tiled.egg-info/requires.txt` & `tiled-0.1.0a94/tiled.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 msgpack>=1.0.0
 ndindex
 numpy
 openpyxl
 orjson
 packaging
 pandas
+parquet
 pillow
 prometheus_client
 psutil
 pyarrow
 pydantic>=1.8.2
 python-dateutil
 python-jose[cryptography]
@@ -43,14 +44,15 @@
 starlette
 tifffile
 toolz
 typer
 uvicorn[standard]
 watchgod
 xarray
+zarr
 zstandard
 
 [client]
 appdirs
 blosc
 click!=8.1.0
 dask[array]
@@ -97,14 +99,15 @@
 msgpack>=1.0.0
 ndindex
 numpy
 openpyxl
 orjson
 packaging
 pandas
+parquet
 pillow
 prometheus_client
 psutil
 pyarrow
 pydantic>=1.8.2
 python-dateutil
 python-jose[cryptography]
@@ -115,14 +118,15 @@
 starlette
 tifffile
 toolz
 typer
 uvicorn[standard]
 watchgod
 xarray
+zarr
 zstandard
 
 [formats]
 h5py
 h5netcdf
 openpyxl
 pillow
@@ -153,27 +157,29 @@
 httpx!=0.23.1,>=0.20.0
 jinja2
 jmespath
 jsonschema
 msgpack>=1.0.0
 orjson
 packaging
+parquet
 psutil
 prometheus_client
 pydantic>=1.8.2
 python-dateutil
 python-jose[cryptography]
 python-multipart
 pyyaml
 sqlalchemy>=2
 starlette
 toolz
 typer
 uvicorn[standard]
 watchgod
+zarr
 
 [server]
 aiofiles
 aiosqlite
 alembic
 anyio
 appdirs
@@ -192,14 +198,15 @@
 lz4
 msgpack>=1.0.0
 ndindex
 numpy
 orjson
 packaging
 pandas
+parquet
 prometheus_client
 psutil
 pyarrow
 pydantic>=1.8.2
 python-dateutil
 python-jose[cryptography]
 python-multipart
@@ -208,8 +215,9 @@
 sqlalchemy>=2
 starlette
 toolz
 typer
 uvicorn[standard]
 watchgod
 xarray
+zarr
 zstandard
```

### Comparing `tiled-0.1.0a93/versioneer.py` & `tiled-0.1.0a94/versioneer.py`

 * *Files identical despite different names*

