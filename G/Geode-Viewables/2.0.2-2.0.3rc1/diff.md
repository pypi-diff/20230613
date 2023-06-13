# Comparing `tmp/Geode_Viewables-2.0.2-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Viewables-2.0.3rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 155982 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      202 b- defN 23-May-03 09:56 geode_viewables/__init__.py
--rw-rw-rw-  2.0 fat     1284 b- defN 23-May-03 09:56 geode_viewables/conversion.py
--rw-rw-rw-  2.0 fat     1251 b- defN 23-May-03 09:56 geode_viewables/qem_proxy.py
--rw-rw-rw-  2.0 fat    27648 b- defN 23-May-03 09:56 geode_viewables/bin/Geode-Viewables_conversion.dll
--rw-rw-rw-  2.0 fat    56320 b- defN 23-May-03 09:56 geode_viewables/bin/Geode-Viewables_qem_proxy.dll
--rw-rw-rw-  2.0 fat   153600 b- defN 23-May-03 09:56 geode_viewables/bin/geode_viewables_py_conversion.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   126464 b- defN 23-May-03 09:56 geode_viewables/bin/geode_viewables_py_qem_proxy.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1965 b- defN 23-May-03 09:56 Geode_Viewables-2.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-03 09:56 Geode_Viewables-2.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-May-03 09:56 Geode_Viewables-2.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1053 b- defN 23-May-03 09:56 Geode_Viewables-2.0.2.dist-info/RECORD
-11 files, 369903 bytes uncompressed, 154168 bytes compressed:  58.3%
+Zip file size: 156533 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      202 b- defN 23-Jun-13 10:27 geode_viewables/__init__.py
+-rw-rw-rw-  2.0 fat     1284 b- defN 23-Jun-13 10:27 geode_viewables/conversion.py
+-rw-rw-rw-  2.0 fat     1251 b- defN 23-Jun-13 10:27 geode_viewables/qem_proxy.py
+-rw-rw-rw-  2.0 fat    27648 b- defN 23-Jun-13 10:27 geode_viewables/bin/Geode-Viewables_conversion.dll
+-rw-rw-rw-  2.0 fat    57344 b- defN 23-Jun-13 10:27 geode_viewables/bin/Geode-Viewables_qem_proxy.dll
+-rw-rw-rw-  2.0 fat   153600 b- defN 23-Jun-13 10:27 geode_viewables/bin/geode_viewables_py_conversion.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   126464 b- defN 23-Jun-13 10:27 geode_viewables/bin/geode_viewables_py_qem_proxy.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1969 b- defN 23-Jun-13 10:27 Geode_Viewables-2.0.3rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-13 10:27 Geode_Viewables-2.0.3rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-Jun-13 10:27 Geode_Viewables-2.0.3rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1065 b- defN 23-Jun-13 10:27 Geode_Viewables-2.0.3rc1.dist-info/RECORD
+11 files, 370943 bytes uncompressed, 154695 bytes compressed:  58.3%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: geode_viewables/bin/geode_viewables_py_conversion.cp39-win_amd64.pyd
 Comment: 
 
 Filename: geode_viewables/bin/geode_viewables_py_qem_proxy.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Viewables-2.0.2.dist-info/METADATA
+Filename: Geode_Viewables-2.0.3rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Viewables-2.0.2.dist-info/WHEEL
+Filename: Geode_Viewables-2.0.3rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Viewables-2.0.2.dist-info/top_level.txt
+Filename: Geode_Viewables-2.0.3rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Viewables-2.0.2.dist-info/RECORD
+Filename: Geode_Viewables-2.0.3rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_viewables/bin/Geode-Viewables_conversion.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180002ddc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May  3 09:56:27 2023
+Time/Date		Tue Jun 13 10:27:44 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000002c00
 SizeOfInitializedData	0000000000003c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000002ddc
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		0000c000
 SizeOfHeaders		00000400
-CheckSum		0000d39d
+CheckSum		0000fe5e
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -71,63 +71,63 @@
 	vma:  Hint/Ord Member-Name Bound-To
 	63d0	    4  ?initialize@IOModelLibrary@geode@@SAXXZ
 
  00006058	000061e0 00000000 00000000 000064ac 00004080
 
 	DLL Name: OpenGeode-Geosciences_explicit.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	645c	  517  ?save_structural_model@geode@@YAXAEBVStructuralModel@1@Vstring_view@absl@@@Z
-	6412	  507  ?save_cross_section@geode@@YAXAEBVCrossSection@1@Vstring_view@absl@@@Z
+	645c	  533  ?save_structural_model@geode@@YAXAEBVStructuralModel@1@Vstring_view@absl@@@Z
+	6412	  523  ?save_cross_section@geode@@YAXAEBVCrossSection@1@Vstring_view@absl@@@Z
 
  0000606c	000061f8 00000000 00000000 000064fa 00004098
 
 	DLL Name: OpenGeode-IO_mesh.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	64d0	    4  ?initialize@IOMeshLibrary@geode@@SAXXZ
 
  00006080	000062d0 00000000 00000000 00006586 00004170
 
 	DLL Name: OpenGeode_model.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	6548	 1048  ?save_section@geode@@YAXAEBVSection@1@Vstring_view@absl@@@Z
-	6510	 1039  ?save_brep@geode@@YAXAEBVBRep@1@Vstring_view@absl@@@Z
+	6548	 1066  ?save_section@geode@@YAXAEBVSection@1@Vstring_view@absl@@@Z
+	6510	 1057  ?save_brep@geode@@YAXAEBVBRep@1@Vstring_view@absl@@@Z
 
  00006094	00006260 00000000 00000000 00006a14 00004100
 
 	DLL Name: OpenGeode_mesh.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	694c	   73  ??$save_triangulated_surface@$01@geode@@YAXAEBV?$TriangulatedSurface@$01@0@Vstring_view@absl@@@Z
-	68ee	   72  ??$save_tetrahedral_solid@$02@geode@@YAXAEBV?$TetrahedralSolid@$02@0@Vstring_view@absl@@@Z
-	689a	   71  ??$save_regular_grid@$02@geode@@YAXAEBV?$RegularGrid@$02@0@Vstring_view@absl@@@Z
-	6846	   70  ??$save_regular_grid@$01@geode@@YAXAEBV?$RegularGrid@$01@0@Vstring_view@absl@@@Z
-	67ea	   69  ??$save_polyhedral_solid@$02@geode@@YAXAEBV?$PolyhedralSolid@$02@0@Vstring_view@absl@@@Z
-	678c	   68  ??$save_polygonal_surface@$02@geode@@YAXAEBV?$PolygonalSurface@$02@0@Vstring_view@absl@@@Z
-	672e	   67  ??$save_polygonal_surface@$01@geode@@YAXAEBV?$PolygonalSurface@$01@0@Vstring_view@absl@@@Z
-	66e0	   66  ??$save_point_set@$02@geode@@YAXAEBV?$PointSet@$02@0@Vstring_view@absl@@@Z
-	69b0	   74  ??$save_triangulated_surface@$02@geode@@YAXAEBV?$TriangulatedSurface@$02@0@Vstring_view@absl@@@Z
-	6692	   65  ??$save_point_set@$01@geode@@YAXAEBV?$PointSet@$01@0@Vstring_view@absl@@@Z
-	663e	   64  ??$save_hybrid_solid@$02@geode@@YAXAEBV?$HybridSolid@$02@0@Vstring_view@absl@@@Z
-	65ec	   63  ??$save_edged_curve@$02@geode@@YAXAEBV?$EdgedCurve@$02@0@Vstring_view@absl@@@Z
-	659a	   62  ??$save_edged_curve@$01@geode@@YAXAEBV?$EdgedCurve@$01@0@Vstring_view@absl@@@Z
+	694c	   80  ??$save_triangulated_surface@$01@geode@@YAXAEBV?$TriangulatedSurface@$01@0@Vstring_view@absl@@@Z
+	68ee	   79  ??$save_tetrahedral_solid@$02@geode@@YAXAEBV?$TetrahedralSolid@$02@0@Vstring_view@absl@@@Z
+	689a	   78  ??$save_regular_grid@$02@geode@@YAXAEBV?$RegularGrid@$02@0@Vstring_view@absl@@@Z
+	6846	   77  ??$save_regular_grid@$01@geode@@YAXAEBV?$RegularGrid@$01@0@Vstring_view@absl@@@Z
+	67ea	   76  ??$save_polyhedral_solid@$02@geode@@YAXAEBV?$PolyhedralSolid@$02@0@Vstring_view@absl@@@Z
+	678c	   75  ??$save_polygonal_surface@$02@geode@@YAXAEBV?$PolygonalSurface@$02@0@Vstring_view@absl@@@Z
+	672e	   74  ??$save_polygonal_surface@$01@geode@@YAXAEBV?$PolygonalSurface@$01@0@Vstring_view@absl@@@Z
+	66e0	   73  ??$save_point_set@$02@geode@@YAXAEBV?$PointSet@$02@0@Vstring_view@absl@@@Z
+	69b0	   81  ??$save_triangulated_surface@$02@geode@@YAXAEBV?$TriangulatedSurface@$02@0@Vstring_view@absl@@@Z
+	6692	   72  ??$save_point_set@$01@geode@@YAXAEBV?$PointSet@$01@0@Vstring_view@absl@@@Z
+	663e	   71  ??$save_hybrid_solid@$02@geode@@YAXAEBV?$HybridSolid@$02@0@Vstring_view@absl@@@Z
+	65ec	   70  ??$save_edged_curve@$02@geode@@YAXAEBV?$EdgedCurve@$02@0@Vstring_view@absl@@@Z
+	659a	   69  ??$save_edged_curve@$01@geode@@YAXAEBV?$EdgedCurve@$01@0@Vstring_view@absl@@@Z
 
  000060a8	00006248 00000000 00000000 00006ad0 000040e8
 
 	DLL Name: OpenGeode_image.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	6a7c	    6  ??$save_raster_image@$02@geode@@YAXAEBV?$RasterImage@$02@0@Vstring_view@absl@@@Z
 	6a28	    5  ??$save_raster_image@$01@geode@@YAXAEBV?$RasterImage@$01@0@Vstring_view@absl@@@Z
 
  000060bc	00006218 00000000 00000000 00006bc0 000040b8
 
 	DLL Name: OpenGeode_basic.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	6b92	   89  ?call_initialize@Library@geode@@IEAAXPEBD@Z
+	6b92	   91  ?call_initialize@Library@geode@@IEAAXPEBD@Z
 	6b76	   26  ??0Library@geode@@IEAA@XZ
-	6ae4	  192  ?set_instance@Singleton@geode@@CAXAEBVtype_info@@PEAV12@@Z
-	6b22	  140  ?instance@Singleton@geode@@CAPEAV12@AEBVtype_info@@@Z
+	6ae4	  199  ?set_instance@Singleton@geode@@CAXAEBVtype_info@@PEAV12@@Z
+	6b22	  143  ?instance@Singleton@geode@@CAPEAV12@AEBVtype_info@@@Z
 	6b5a	   49  ??1Library@geode@@UEAA@XZ
 
  000060d0	00006348 00000000 00000000 00006c3a 000041e8
 
 	DLL Name: absl_strings.dll
 	vma:  Hint/Ord Member-Name Bound-To
 	6bd4	  347  ?StrCat@absl@@YA?AV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@AEBVAlphaNum@1@00@Z
@@ -990,105 +990,105 @@
 	  15b0: 00 00 00 00 7e 6d 00 00 00 00 00 00 58 6d 00 00
 	  15c0: 00 00 00 00 ee 6d 00 00 00 00 00 00 44 6e 00 00
 	  15d0: 00 00 00 00 c2 6d 00 00 00 00 00 00 00 00 00 00
 	  15e0: 00 00 00 00 04 00 3f 69 6e 69 74 69 61 6c 69 7a
 	  15f0: 65 40 49 4f 4d 6f 64 65 6c 4c 69 62 72 61 72 79
 	  1600: 40 67 65 6f 64 65 40 40 53 41 58 58 5a 00 4f 70
 	  1610: 65 6e 47 65 6f 64 65 2d 49 4f 5f 6d 6f 64 65 6c
-	  1620: 2e 64 6c 6c 00 00 fb 01 3f 73 61 76 65 5f 63 72
+	  1620: 2e 64 6c 6c 00 00 0b 02 3f 73 61 76 65 5f 63 72
 	  1630: 6f 73 73 5f 73 65 63 74 69 6f 6e 40 67 65 6f 64
 	  1640: 65 40 40 59 41 58 41 45 42 56 43 72 6f 73 73 53
 	  1650: 65 63 74 69 6f 6e 40 31 40 56 73 74 72 69 6e 67
 	  1660: 5f 76 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00
-	  1670: 05 02 3f 73 61 76 65 5f 73 74 72 75 63 74 75 72
+	  1670: 15 02 3f 73 61 76 65 5f 73 74 72 75 63 74 75 72
 	  1680: 61 6c 5f 6d 6f 64 65 6c 40 67 65 6f 64 65 40 40
 	  1690: 59 41 58 41 45 42 56 53 74 72 75 63 74 75 72 61
 	  16a0: 6c 4d 6f 64 65 6c 40 31 40 56 73 74 72 69 6e 67
 	  16b0: 5f 76 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00
 	  16c0: 4f 70 65 6e 47 65 6f 64 65 2d 47 65 6f 73 63 69
 	  16d0: 65 6e 63 65 73 5f 65 78 70 6c 69 63 69 74 2e 64
 	  16e0: 6c 6c 00 00 04 00 3f 69 6e 69 74 69 61 6c 69 7a
 	  16f0: 65 40 49 4f 4d 65 73 68 4c 69 62 72 61 72 79 40
 	  1700: 67 65 6f 64 65 40 40 53 41 58 58 5a 00 00 4f 70
 	  1710: 65 6e 47 65 6f 64 65 2d 49 4f 5f 6d 65 73 68 2e
-	  1720: 64 6c 6c 00 0f 04 3f 73 61 76 65 5f 62 72 65 70
+	  1720: 64 6c 6c 00 21 04 3f 73 61 76 65 5f 62 72 65 70
 	  1730: 40 67 65 6f 64 65 40 40 59 41 58 41 45 42 56 42
 	  1740: 52 65 70 40 31 40 56 73 74 72 69 6e 67 5f 76 69
-	  1750: 65 77 40 61 62 73 6c 40 40 40 5a 00 18 04 3f 73
+	  1750: 65 77 40 61 62 73 6c 40 40 40 5a 00 2a 04 3f 73
 	  1760: 61 76 65 5f 73 65 63 74 69 6f 6e 40 67 65 6f 64
 	  1770: 65 40 40 59 41 58 41 45 42 56 53 65 63 74 69 6f
 	  1780: 6e 40 31 40 56 73 74 72 69 6e 67 5f 76 69 65 77
 	  1790: 40 61 62 73 6c 40 40 40 5a 00 4f 70 65 6e 47 65
-	  17a0: 6f 64 65 5f 6d 6f 64 65 6c 2e 64 6c 6c 00 3e 00
+	  17a0: 6f 64 65 5f 6d 6f 64 65 6c 2e 64 6c 6c 00 45 00
 	  17b0: 3f 3f 24 73 61 76 65 5f 65 64 67 65 64 5f 63 75
 	  17c0: 72 76 65 40 24 30 31 40 67 65 6f 64 65 40 40 59
 	  17d0: 41 58 41 45 42 56 3f 24 45 64 67 65 64 43 75 72
 	  17e0: 76 65 40 24 30 31 40 30 40 56 73 74 72 69 6e 67
 	  17f0: 5f 76 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00
-	  1800: 3f 00 3f 3f 24 73 61 76 65 5f 65 64 67 65 64 5f
+	  1800: 46 00 3f 3f 24 73 61 76 65 5f 65 64 67 65 64 5f
 	  1810: 63 75 72 76 65 40 24 30 32 40 67 65 6f 64 65 40
 	  1820: 40 59 41 58 41 45 42 56 3f 24 45 64 67 65 64 43
 	  1830: 75 72 76 65 40 24 30 32 40 30 40 56 73 74 72 69
 	  1840: 6e 67 5f 76 69 65 77 40 61 62 73 6c 40 40 40 5a
-	  1850: 00 00 40 00 3f 3f 24 73 61 76 65 5f 68 79 62 72
+	  1850: 00 00 47 00 3f 3f 24 73 61 76 65 5f 68 79 62 72
 	  1860: 69 64 5f 73 6f 6c 69 64 40 24 30 32 40 67 65 6f
 	  1870: 64 65 40 40 59 41 58 41 45 42 56 3f 24 48 79 62
 	  1880: 72 69 64 53 6f 6c 69 64 40 24 30 32 40 30 40 56
 	  1890: 73 74 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c
-	  18a0: 40 40 40 5a 00 00 41 00 3f 3f 24 73 61 76 65 5f
+	  18a0: 40 40 40 5a 00 00 48 00 3f 3f 24 73 61 76 65 5f
 	  18b0: 70 6f 69 6e 74 5f 73 65 74 40 24 30 31 40 67 65
 	  18c0: 6f 64 65 40 40 59 41 58 41 45 42 56 3f 24 50 6f
 	  18d0: 69 6e 74 53 65 74 40 24 30 31 40 30 40 56 73 74
 	  18e0: 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c 40 40
-	  18f0: 40 5a 00 00 42 00 3f 3f 24 73 61 76 65 5f 70 6f
+	  18f0: 40 5a 00 00 49 00 3f 3f 24 73 61 76 65 5f 70 6f
 	  1900: 69 6e 74 5f 73 65 74 40 24 30 32 40 67 65 6f 64
 	  1910: 65 40 40 59 41 58 41 45 42 56 3f 24 50 6f 69 6e
 	  1920: 74 53 65 74 40 24 30 32 40 30 40 56 73 74 72 69
 	  1930: 6e 67 5f 76 69 65 77 40 61 62 73 6c 40 40 40 5a
-	  1940: 00 00 43 00 3f 3f 24 73 61 76 65 5f 70 6f 6c 79
+	  1940: 00 00 4a 00 3f 3f 24 73 61 76 65 5f 70 6f 6c 79
 	  1950: 67 6f 6e 61 6c 5f 73 75 72 66 61 63 65 40 24 30
 	  1960: 31 40 67 65 6f 64 65 40 40 59 41 58 41 45 42 56
 	  1970: 3f 24 50 6f 6c 79 67 6f 6e 61 6c 53 75 72 66 61
 	  1980: 63 65 40 24 30 31 40 30 40 56 73 74 72 69 6e 67
 	  1990: 5f 76 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00
-	  19a0: 44 00 3f 3f 24 73 61 76 65 5f 70 6f 6c 79 67 6f
+	  19a0: 4b 00 3f 3f 24 73 61 76 65 5f 70 6f 6c 79 67 6f
 	  19b0: 6e 61 6c 5f 73 75 72 66 61 63 65 40 24 30 32 40
 	  19c0: 67 65 6f 64 65 40 40 59 41 58 41 45 42 56 3f 24
 	  19d0: 50 6f 6c 79 67 6f 6e 61 6c 53 75 72 66 61 63 65
 	  19e0: 40 24 30 32 40 30 40 56 73 74 72 69 6e 67 5f 76
-	  19f0: 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00 45 00
+	  19f0: 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00 4c 00
 	  1a00: 3f 3f 24 73 61 76 65 5f 70 6f 6c 79 68 65 64 72
 	  1a10: 61 6c 5f 73 6f 6c 69 64 40 24 30 32 40 67 65 6f
 	  1a20: 64 65 40 40 59 41 58 41 45 42 56 3f 24 50 6f 6c
 	  1a30: 79 68 65 64 72 61 6c 53 6f 6c 69 64 40 24 30 32
 	  1a40: 40 30 40 56 73 74 72 69 6e 67 5f 76 69 65 77 40
-	  1a50: 61 62 73 6c 40 40 40 5a 00 00 46 00 3f 3f 24 73
+	  1a50: 61 62 73 6c 40 40 40 5a 00 00 4d 00 3f 3f 24 73
 	  1a60: 61 76 65 5f 72 65 67 75 6c 61 72 5f 67 72 69 64
 	  1a70: 40 24 30 31 40 67 65 6f 64 65 40 40 59 41 58 41
 	  1a80: 45 42 56 3f 24 52 65 67 75 6c 61 72 47 72 69 64
 	  1a90: 40 24 30 31 40 30 40 56 73 74 72 69 6e 67 5f 76
-	  1aa0: 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00 47 00
+	  1aa0: 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00 4e 00
 	  1ab0: 3f 3f 24 73 61 76 65 5f 72 65 67 75 6c 61 72 5f
 	  1ac0: 67 72 69 64 40 24 30 32 40 67 65 6f 64 65 40 40
 	  1ad0: 59 41 58 41 45 42 56 3f 24 52 65 67 75 6c 61 72
 	  1ae0: 47 72 69 64 40 24 30 32 40 30 40 56 73 74 72 69
 	  1af0: 6e 67 5f 76 69 65 77 40 61 62 73 6c 40 40 40 5a
-	  1b00: 00 00 48 00 3f 3f 24 73 61 76 65 5f 74 65 74 72
+	  1b00: 00 00 4f 00 3f 3f 24 73 61 76 65 5f 74 65 74 72
 	  1b10: 61 68 65 64 72 61 6c 5f 73 6f 6c 69 64 40 24 30
 	  1b20: 32 40 67 65 6f 64 65 40 40 59 41 58 41 45 42 56
 	  1b30: 3f 24 54 65 74 72 61 68 65 64 72 61 6c 53 6f 6c
 	  1b40: 69 64 40 24 30 32 40 30 40 56 73 74 72 69 6e 67
 	  1b50: 5f 76 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00
-	  1b60: 49 00 3f 3f 24 73 61 76 65 5f 74 72 69 61 6e 67
+	  1b60: 50 00 3f 3f 24 73 61 76 65 5f 74 72 69 61 6e 67
 	  1b70: 75 6c 61 74 65 64 5f 73 75 72 66 61 63 65 40 24
 	  1b80: 30 31 40 67 65 6f 64 65 40 40 59 41 58 41 45 42
 	  1b90: 56 3f 24 54 72 69 61 6e 67 75 6c 61 74 65 64 53
 	  1ba0: 75 72 66 61 63 65 40 24 30 31 40 30 40 56 73 74
 	  1bb0: 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c 40 40
-	  1bc0: 40 5a 00 00 4a 00 3f 3f 24 73 61 76 65 5f 74 72
+	  1bc0: 40 5a 00 00 51 00 3f 3f 24 73 61 76 65 5f 74 72
 	  1bd0: 69 61 6e 67 75 6c 61 74 65 64 5f 73 75 72 66 61
 	  1be0: 63 65 40 24 30 32 40 67 65 6f 64 65 40 40 59 41
 	  1bf0: 58 41 45 42 56 3f 24 54 72 69 61 6e 67 75 6c 61
 	  1c00: 74 65 64 53 75 72 66 61 63 65 40 24 30 32 40 30
 	  1c10: 40 56 73 74 72 69 6e 67 5f 76 69 65 77 40 61 62
 	  1c20: 73 6c 40 40 40 5a 00 00 4f 70 65 6e 47 65 6f 64
 	  1c30: 65 5f 6d 65 73 68 2e 64 6c 6c 00 00 05 00 3f 3f
@@ -1099,26 +1099,26 @@
 	  1c80: 5f 76 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00
 	  1c90: 06 00 3f 3f 24 73 61 76 65 5f 72 61 73 74 65 72
 	  1ca0: 5f 69 6d 61 67 65 40 24 30 32 40 67 65 6f 64 65
 	  1cb0: 40 40 59 41 58 41 45 42 56 3f 24 52 61 73 74 65
 	  1cc0: 72 49 6d 61 67 65 40 24 30 32 40 30 40 56 73 74
 	  1cd0: 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c 40 40
 	  1ce0: 40 5a 00 00 4f 70 65 6e 47 65 6f 64 65 5f 69 6d
-	  1cf0: 61 67 65 2e 64 6c 6c 00 c0 00 3f 73 65 74 5f 69
+	  1cf0: 61 67 65 2e 64 6c 6c 00 c7 00 3f 73 65 74 5f 69
 	  1d00: 6e 73 74 61 6e 63 65 40 53 69 6e 67 6c 65 74 6f
 	  1d10: 6e 40 67 65 6f 64 65 40 40 43 41 58 41 45 42 56
 	  1d20: 74 79 70 65 5f 69 6e 66 6f 40 40 50 45 41 56 31
-	  1d30: 32 40 40 5a 00 00 8c 00 3f 69 6e 73 74 61 6e 63
+	  1d30: 32 40 40 5a 00 00 8f 00 3f 69 6e 73 74 61 6e 63
 	  1d40: 65 40 53 69 6e 67 6c 65 74 6f 6e 40 67 65 6f 64
 	  1d50: 65 40 40 43 41 50 45 41 56 31 32 40 41 45 42 56
 	  1d60: 74 79 70 65 5f 69 6e 66 6f 40 40 40 5a 00 31 00
 	  1d70: 3f 3f 31 4c 69 62 72 61 72 79 40 67 65 6f 64 65
 	  1d80: 40 40 55 45 41 41 40 58 5a 00 1a 00 3f 3f 30 4c
 	  1d90: 69 62 72 61 72 79 40 67 65 6f 64 65 40 40 49 45
-	  1da0: 41 41 40 58 5a 00 59 00 3f 63 61 6c 6c 5f 69 6e
+	  1da0: 41 41 40 58 5a 00 5b 00 3f 63 61 6c 6c 5f 69 6e
 	  1db0: 69 74 69 61 6c 69 7a 65 40 4c 69 62 72 61 72 79
 	  1dc0: 40 67 65 6f 64 65 40 40 49 45 41 41 58 50 45 42
 	  1dd0: 44 40 5a 00 4f 70 65 6e 47 65 6f 64 65 5f 62 61
 	  1de0: 73 69 63 2e 64 6c 6c 00 5b 01 3f 53 74 72 43 61
 	  1df0: 74 40 61 62 73 6c 40 40 59 41 3f 41 56 3f 24 62
 	  1e00: 61 73 69 63 5f 73 74 72 69 6e 67 40 44 55 3f 24
 	  1e10: 63 68 61 72 5f 74 72 61 69 74 73 40 44 40 73 74
@@ -4635,20 +4635,17 @@
    1800043fa:	(bad)
    1800043fb:	(bad)
    1800043fc:	(bad)
    1800043fd:	(bad)
    1800043fe:	(bad)
    1800043ff:	incl   (%rax)
    180004401:	add    %al,(%rax)
-   180004403:	add    %cl,%bl
-   180004405:	(bad)
-   180004406:	push   %rdx
-   180004407:	add    %al,%fs:(%rax)
-   18000440a:	add    %al,(%rax)
-   18000440c:	or     $0x7c000000,%eax
+   180004403:	add    %ah,0x648844(%rax)
+   180004409:	add    %al,(%rax)
+   18000440b:	add    %cl,0x7c000000(%rip)        # 0x1fc004411
    180004411:	add    (%rax),%al
    180004413:	add    %cl,%ah
    180004415:	rex.W add %al,(%rax)
    180004418:	int3
    180004419:	cmp    %al,(%rax)
    18000441b:	add    %al,(%rax)
    18000441d:	add    %al,(%rax)
@@ -7919,16 +7916,16 @@
    1800063ff:	outsl  %gs:(%rsi),(%dx)
    180006401:	fs gs sub $0x6d5f4f49,%eax
    180006408:	outsl  %ds:(%rsi),(%dx)
    180006409:	fs gs insb (%dx),%es:(%rdi)
    18000640c:	cs fs insb (%dx),%es:(%rdi)
    18000640f:	insb   (%dx),%es:(%rdi)
    180006410:	add    %al,(%rax)
-   180006412:	sti
-   180006413:	add    %edi,(%rdi)
+   180006412:	or     (%rdx),%eax
+   180006414:	(bad)
    180006415:	jae    0x180006478
    180006417:	jbe    0x18000647e
    180006419:	pop    %rdi
    18000641a:	movsxd 0x6f(%rdx),%esi
    18000641d:	jae    0x180006492
    18000641f:	pop    %rdi
    180006420:	jae    0x180006487
@@ -7954,15 +7951,15 @@
    18000644b:	addr32 pop %rdi
    18000644d:	jbe    0x1800064b8
    18000644f:	gs ja  0x180006492
    180006452:	(bad)
    180006453:	(bad)
    180006458:	rex pop %rdx
    18000645a:	add    %al,(%rax)
-   18000645c:	add    $0x61733f02,%eax
+   18000645c:	adc    $0x61733f02,%eax
    180006461:	jbe    0x1800064c8
    180006463:	pop    %rdi
    180006464:	jae    0x1800064da
    180006466:	jb     0x1800064dd
    180006468:	movsxd 0x72(%rbp,%rsi,2),%esi
    18000646c:	(bad)
    18000646d:	insb   (%dx),%es:(%rdi)
@@ -8028,15 +8025,15 @@
    1800064fd:	outsb  %ds:(%rsi),(%dx)
    1800064fe:	rex.RXB
    1800064ff:	outsl  %gs:(%rsi),(%dx)
    180006501:	fs gs sub $0x6d5f4f49,%eax
    180006508:	gs jae 0x180006573
    18000650b:	cs fs insb (%dx),%es:(%rdi)
    18000650e:	insb   (%dx),%es:(%rdi)
-   18000650f:	add    %cl,(%rdi)
+   18000650f:	add    %ah,(%rcx)
    180006511:	add    $0x3f,%al
    180006513:	jae    0x180006576
    180006515:	jbe    0x18000657c
    180006517:	pop    %rdi
    180006518:	(bad)
    18000651d:	outsl  %gs:(%esi),(%dx)
    180006520:	fs gs rex
@@ -8053,15 +8050,15 @@
    180006537:	outsb  %ds:(%rsi),(%dx)
    180006538:	addr32 pop %rdi
    18000653a:	jbe    0x1800065a5
    18000653c:	gs ja  0x18000657f
    18000653f:	(bad)
    180006540:	(bad)
    180006545:	rex pop %rdx
-   180006547:	add    %bl,(%rax)
+   180006547:	add    %ch,(%rdx)
    180006549:	add    $0x3f,%al
    18000654b:	jae    0x1800065ae
    18000654d:	jbe    0x1800065b4
    18000654f:	pop    %rdi
    180006550:	jae    0x1800065b7
    180006552:	movsxd 0x6f(%rcx,%rbp,2),%esi
    180006556:	outsb  %ds:(%rsi),(%dx)
@@ -8092,16 +8089,16 @@
    18000658b:	outsl  %gs:(%rsi),(%dx)
    18000658d:	fs gs pop %rdi
    180006590:	insl   (%dx),%es:(%rdi)
    180006591:	outsl  %ds:(%rsi),(%dx)
    180006592:	fs gs insb (%dx),%es:(%rdi)
    180006595:	cs fs insb (%dx),%es:(%rdi)
    180006598:	insb   (%dx),%es:(%rdi)
-   180006599:	add    %bh,(%rsi)
-   18000659b:	add    %bh,(%rdi)
+   180006599:	add    %al,0x0(%rbp)
+   18000659c:	(bad)
    18000659d:	(bad)
    18000659e:	and    $0x73,%al
    1800065a0:	(bad)
    1800065a1:	jbe    0x180006608
    1800065a3:	pop    %rdi
    1800065a4:	gs fs addr32 gs fs pop %rdi
    1800065aa:	movsxd 0x72(%rbp),%esi
@@ -8128,16 +8125,15 @@
    1800065db:	addr32 pop %rdi
    1800065dd:	jbe    0x180006648
    1800065df:	gs ja  0x180006622
    1800065e2:	(bad)
    1800065e3:	(bad)
    1800065e8:	rex pop %rdx
    1800065ea:	add    %al,(%rax)
-   1800065ec:	(bad)
-   1800065ed:	add    %bh,(%rdi)
+   1800065ec:	rex.RX add %r15b,(%rdi)
    1800065ef:	(bad)
    1800065f0:	and    $0x73,%al
    1800065f2:	(bad)
    1800065f3:	jbe    0x18000665a
    1800065f5:	pop    %rdi
    1800065f6:	gs fs addr32 gs fs pop %rdi
    1800065fc:	movsxd 0x72(%rbp),%esi
@@ -8164,15 +8160,15 @@
    18000662d:	addr32 pop %rdi
    18000662f:	jbe    0x18000669a
    180006631:	gs ja  0x180006674
    180006634:	(bad)
    180006635:	(bad)
    18000663a:	rex pop %rdx
    18000663c:	add    %al,(%rax)
-   18000663e:	add    %dil,(%rdi)
+   18000663e:	rex.RXB add %r15b,(%r15)
    180006641:	(bad)
    180006642:	and    $0x73,%al
    180006644:	(bad)
    180006645:	jbe    0x1800066ac
    180006647:	pop    %rdi
    180006648:	push   $0x69726279
    18000664d:	fs pop %rdi
@@ -8201,15 +8197,15 @@
    180006681:	addr32 pop %rdi
    180006683:	jbe    0x1800066ee
    180006685:	gs ja  0x1800066c8
    180006688:	(bad)
    180006689:	(bad)
    18000668e:	rex pop %rdx
    180006690:	add    %al,(%rax)
-   180006692:	add    %dil,(%r15)
+   180006692:	rex.W add %dil,(%rdi)
    180006695:	(bad)
    180006696:	and    $0x73,%al
    180006698:	(bad)
    180006699:	jbe    0x180006700
    18000669b:	pop    %rdi
    18000669c:	jo     0x18000670d
    18000669e:	imul   $0x7465735f,0x74(%rsi),%ebp
@@ -8235,15 +8231,15 @@
    1800066cf:	addr32 pop %rdi
    1800066d1:	jbe    0x18000673c
    1800066d3:	gs ja  0x180006716
    1800066d6:	(bad)
    1800066d7:	(bad)
    1800066dc:	rex pop %rdx
    1800066de:	add    %al,(%rax)
-   1800066e0:	rex.X add %dil,(%rdi)
+   1800066e0:	rex.WB add %dil,(%r15)
    1800066e3:	(bad)
    1800066e4:	and    $0x73,%al
    1800066e6:	(bad)
    1800066e7:	jbe    0x18000674e
    1800066e9:	pop    %rdi
    1800066ea:	jo     0x18000675b
    1800066ec:	imul   $0x7465735f,0x74(%rsi),%ebp
@@ -8269,15 +8265,15 @@
    18000671d:	addr32 pop %rdi
    18000671f:	jbe    0x18000678a
    180006721:	gs ja  0x180006764
    180006724:	(bad)
    180006725:	(bad)
    18000672a:	rex pop %rdx
    18000672c:	add    %al,(%rax)
-   18000672e:	rex.XB add %dil,(%r15)
+   18000672e:	rex.WX add %dil,(%rdi)
    180006731:	(bad)
    180006732:	and    $0x73,%al
    180006734:	(bad)
    180006735:	jbe    0x18000679c
    180006737:	pop    %rdi
    180006738:	jo     0x1800067a9
    18000673a:	insb   (%dx),%es:(%rdi)
@@ -8322,15 +8318,15 @@
    18000677b:	addr32 pop %rdi
    18000677d:	jbe    0x1800067e8
    18000677f:	gs ja  0x1800067c2
    180006782:	(bad)
    180006783:	(bad)
    180006788:	rex pop %rdx
    18000678a:	add    %al,(%rax)
-   18000678c:	add    %r15b,(%rdi)
+   18000678c:	rex.WXB add %dil,(%r15)
    18000678f:	(bad)
    180006790:	and    $0x73,%al
    180006792:	(bad)
    180006793:	jbe    0x1800067fa
    180006795:	pop    %rdi
    180006796:	jo     0x180006807
    180006798:	insb   (%dx),%es:(%rdi)
@@ -8375,15 +8371,15 @@
    1800067d9:	addr32 pop %rdi
    1800067db:	jbe    0x180006846
    1800067dd:	gs ja  0x180006820
    1800067e0:	(bad)
    1800067e1:	(bad)
    1800067e6:	rex pop %rdx
    1800067e8:	add    %al,(%rax)
-   1800067ea:	add    %r15b,(%r15)
+   1800067ea:	rex.WR add %r15b,(%rdi)
    1800067ed:	(bad)
    1800067ee:	and    $0x73,%al
    1800067f0:	(bad)
    1800067f1:	jbe    0x180006858
    1800067f3:	pop    %rdi
    1800067f4:	jo     0x180006865
    1800067f6:	insb   (%dx),%es:(%rdi)
@@ -8419,15 +8415,15 @@
    180006835:	addr32 pop %rdi
    180006837:	jbe    0x1800068a2
    180006839:	gs ja  0x18000687c
    18000683c:	(bad)
    18000683d:	(bad)
    180006842:	rex pop %rdx
    180006844:	add    %al,(%rax)
-   180006846:	rex.RX add %r15b,(%rdi)
+   180006846:	rex.WRB add %r15b,(%r15)
    180006849:	(bad)
    18000684a:	and    $0x73,%al
    18000684c:	(bad)
    18000684d:	jbe    0x1800068b4
    18000684f:	pop    %rdi
    180006850:	jb     0x1800068b7
    180006852:	addr32 jne 0x1800068c1
@@ -8458,15 +8454,15 @@
    180006889:	addr32 pop %rdi
    18000688b:	jbe    0x1800068f6
    18000688d:	gs ja  0x1800068d0
    180006890:	(bad)
    180006891:	(bad)
    180006896:	rex pop %rdx
    180006898:	add    %al,(%rax)
-   18000689a:	rex.RXB add %r15b,(%r15)
+   18000689a:	rex.WRX add %r15b,(%rdi)
    18000689d:	(bad)
    18000689e:	and    $0x73,%al
    1800068a0:	(bad)
    1800068a1:	jbe    0x180006908
    1800068a3:	pop    %rdi
    1800068a4:	jb     0x18000690b
    1800068a6:	addr32 jne 0x180006915
@@ -8497,15 +8493,15 @@
    1800068dd:	addr32 pop %rdi
    1800068df:	jbe    0x18000694a
    1800068e1:	gs ja  0x180006924
    1800068e4:	(bad)
    1800068e5:	(bad)
    1800068ea:	rex pop %rdx
    1800068ec:	add    %al,(%rax)
-   1800068ee:	rex.W add %dil,(%rdi)
+   1800068ee:	rex.WRXB add %r15b,(%r15)
    1800068f1:	(bad)
    1800068f2:	and    $0x73,%al
    1800068f4:	(bad)
    1800068f5:	jbe    0x18000695c
    1800068f7:	pop    %rdi
    1800068f8:	je     0x18000695f
    1800068fa:	je     0x18000696e
@@ -8540,15 +8536,16 @@
    18000693b:	addr32 pop %rdi
    18000693d:	jbe    0x1800069a8
    18000693f:	gs ja  0x180006982
    180006942:	(bad)
    180006943:	(bad)
    180006948:	rex pop %rdx
    18000694a:	add    %al,(%rax)
-   18000694c:	rex.WB add %dil,(%r15)
+   18000694c:	push   %rax
+   18000694d:	add    %bh,(%rdi)
    18000694f:	(bad)
    180006950:	and    $0x73,%al
    180006952:	(bad)
    180006953:	jbe    0x1800069ba
    180006955:	pop    %rdi
    180006956:	je     0x1800069ca
    180006958:	imul   $0x616c7567,0x6e(%rcx),%esp
@@ -8588,15 +8585,16 @@
    18000699f:	addr32 pop %rdi
    1800069a1:	jbe    0x180006a0c
    1800069a3:	gs ja  0x1800069e6
    1800069a6:	(bad)
    1800069a7:	(bad)
    1800069ac:	rex pop %rdx
    1800069ae:	add    %al,(%rax)
-   1800069b0:	rex.WX add %dil,(%rdi)
+   1800069b0:	push   %rcx
+   1800069b1:	add    %bh,(%rdi)
    1800069b3:	(bad)
    1800069b4:	and    $0x73,%al
    1800069b6:	(bad)
    1800069b7:	jbe    0x180006a1e
    1800069b9:	pop    %rdi
    1800069ba:	je     0x180006a2e
    1800069bc:	imul   $0x616c7567,0x6e(%rcx),%esp
@@ -8731,15 +8729,15 @@
    180006ad3:	outsb  %ds:(%rsi),(%dx)
    180006ad4:	rex.RXB
    180006ad5:	outsl  %gs:(%rsi),(%dx)
    180006ad7:	fs gs pop %rdi
    180006ada:	imul   $0x642e6567,0x61(%rbp),%ebp
    180006ae1:	insb   (%dx),%es:(%rdi)
    180006ae2:	insb   (%dx),%es:(%rdi)
-   180006ae3:	add    %al,%al
+   180006ae3:	add    %al,%bh
    180006ae5:	add    %bh,(%rdi)
    180006ae7:	jae    0x180006b4e
    180006ae9:	je     0x180006b4a
    180006aeb:	imul   $0x636e6174,0x73(%rsi),%ebp
    180006af2:	gs rex push %rbx
    180006af5:	imul   $0x6f74656c,0x67(%rsi),%ebp
    180006afc:	outsb  %ds:(%rsi),(%dx)
@@ -8758,15 +8756,15 @@
    180006b11:	imul   $0x5040406f,0x66(%rsi),%ebp
    180006b18:	rex.RB
    180006b19:	push   %r14
    180006b1b:	xor    %esi,(%rdx)
    180006b1d:	rex
    180006b1e:	rex pop %rdx
    180006b20:	add    %al,(%rax)
-   180006b22:	mov    %es,(%rax)
+   180006b22:	pop    (%rax)
    180006b24:	(bad)
    180006b25:	imul   $0x636e6174,0x73(%rsi),%ebp
    180006b2c:	gs rex push %rbx
    180006b2f:	imul   $0x6f74656c,0x67(%rsi),%ebp
    180006b36:	outsb  %ds:(%rsi),(%dx)
    180006b37:	rex
    180006b38:	outsl  %gs:(%esi),(%dx)
@@ -8813,15 +8811,15 @@
    180006b89:	rex
    180006b8a:	rex.WB
    180006b8b:	rex.RB
    180006b8c:	rex.B
    180006b8d:	rex.B
    180006b8e:	rex pop %rax
    180006b90:	pop    %rdx
-   180006b91:	add    %bl,0x0(%rcx)
+   180006b91:	add    %bl,0x0(%rbx)
    180006b94:	(bad)
    180006b95:	movsxd 0x6c(%rcx),%esp
    180006b98:	insb   (%dx),%es:(%rdi)
    180006b99:	pop    %rdi
    180006b9a:	imul   $0x6c616974,0x69(%rsi),%ebp
    180006ba1:	imul   $0x62694c40,0x65(%rdx),%edi
    180006ba8:	jb     0x180006c0b
```

## geode_viewables/bin/Geode-Viewables_qem_proxy.dll

### objdump

```diff
@@ -1,298 +1,298 @@
 
 architecture: i386:x86-64, flags 0x0000012f:
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
-start address 0x000000018000759c
+start address 0x000000018000785c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May  3 09:56:31 2023
+Time/Date		Tue Jun 13 10:27:46 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
-SizeOfCode		0000000000007800
+SizeOfCode		0000000000007c00
 SizeOfInitializedData	0000000000006000
 SizeOfUninitializedData	0000000000000000
-AddressOfEntryPoint	000000000000759c
+AddressOfEntryPoint	000000000000785c
 BaseOfCode		0000000000001000
 ImageBase		0000000180000000
 SectionAlignment	00001000
 FileAlignment		00000200
 MajorOSystemVersion	6
 MinorOSystemVersion	0
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00012000
 SizeOfHeaders		00000400
-CheckSum		000157fb
+CheckSum		00018af8
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
 NumberOfRvaAndSizes	00000010
 
 The Data Directory
-Entry 0 000000000000b7d0 000001a4 Export Directory [.edata (or where ever we found it)]
-Entry 1 000000000000b974 0000012c Import Directory [parts of .idata]
+Entry 0 000000000000b840 000001a4 Export Directory [.edata (or where ever we found it)]
+Entry 1 000000000000b9e4 0000012c Import Directory [parts of .idata]
 Entry 2 0000000000010000 000001b4 Resource Directory [.rsrc]
-Entry 3 000000000000f000 000008a0 Exception Directory [.pdata]
+Entry 3 000000000000f000 000008d0 Exception Directory [.pdata]
 Entry 4 0000000000000000 00000000 Security Directory
 Entry 5 0000000000011000 000000e4 Base Relocation Directory [.reloc]
-Entry 6 00000000000099f0 0000001c Debug Directory
+Entry 6 00000000000099f8 0000001c Debug Directory
 Entry 7 0000000000000000 00000000 Description Directory
 Entry 8 0000000000000000 00000000 Special Directory
 Entry 9 0000000000000000 00000000 Thread Storage Directory [.tls]
-Entry a 0000000000009a10 00000138 Load Configuration Directory
+Entry a 0000000000009a20 00000138 Load Configuration Directory
 Entry b 0000000000000000 00000000 Bound Import Directory
 Entry c 0000000000009000 00000470 Import Address Table Directory
 Entry d 0000000000000000 00000000 Delay Import Directory
 Entry e 0000000000000000 00000000 CLR Runtime Header
 Entry f 0000000000000000 00000000 Reserved
 
-There is an import table in .rdata at 0x18000b974
+There is an import table in .rdata at 0x18000b9e4
 
 The Import Tables (interpreted .rdata section contents)
  vma:            Hint    Time      Forward  DLL       First
                  Table   Stamp     Chain    Name      Thunk
- 0000b974	0000baa0 00000000 00000000 0000c180 00009000
+ 0000b9e4	0000bb10 00000000 00000000 0000c1f0 00009000
 
 	DLL Name: Geode-Common_modifier_surface.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	bf48	   39  ??0?$TriangulatedSurfaceModifier@$02@geode@@QEAA@AEBV?$SurfaceMesh@$02@1@AEAV?$TriangulatedSurfaceBuilder@$02@1@@Z
-	bfbe	   44  ??1?$TriangulatedSurfaceModifier@$02@geode@@QEAA@XZ
-	bff4	   68  ?is_edge_active@?$TriangulatedSurfaceModifier@$02@geode@@QEBA_NI@Z
-	c03a	   57  ?collapse_edge@?$TriangulatedSurfaceModifier@$02@geode@@QEAA?AUCollapseEdgeInfo@12@IAEBV?$Point@$02@2@@Z
-	c0a6	   48  ?clean@?$TriangulatedSurfaceModifier@$02@geode@@QEAA?AV?$tuple@V?$vector@IV?$allocator@I@std@@@std@@V12@V12@@std@@XZ
-	c11e	    7  ??$is_collapse_edge_valid@$02@geode@@YA_NAEBV?$TriangulatedSurface@$02@0@IAEBV?$Point@$02@0@@Z
-	bf10	   60  ?initialize@CommonModifierSurfaceLibrary@geode@@SAXXZ
+	bfb8	   39  ??0?$TriangulatedSurfaceModifier@$02@geode@@QEAA@AEBV?$SurfaceMesh@$02@1@AEAV?$TriangulatedSurfaceBuilder@$02@1@@Z
+	c02e	   44  ??1?$TriangulatedSurfaceModifier@$02@geode@@QEAA@XZ
+	c064	   68  ?is_edge_active@?$TriangulatedSurfaceModifier@$02@geode@@QEBA_NI@Z
+	c0aa	   57  ?collapse_edge@?$TriangulatedSurfaceModifier@$02@geode@@QEAA?AUCollapseEdgeInfo@12@IAEBV?$Point@$02@2@@Z
+	c116	   48  ?clean@?$TriangulatedSurfaceModifier@$02@geode@@QEAA?AV?$tuple@V?$vector@IV?$allocator@I@std@@@std@@V12@V12@@std@@XZ
+	c18e	    7  ??$is_collapse_edge_valid@$02@geode@@YA_NAEBV?$TriangulatedSurface@$02@0@IAEBV?$Point@$02@0@@Z
+	bf80	   60  ?initialize@CommonModifierSurfaceLibrary@geode@@SAXXZ
 
- 0000b988	0000bce0 00000000 00000000 0000c684 00009240
+ 0000b9f8	0000bd50 00000000 00000000 0000c6f4 00009240
 
 	DLL Name: OpenGeode_mesh.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	c5a2	   53  ??$polygon_vertex_normal@$02@?$SurfaceMesh@$02@geode@@QEBA?AV?$optional@V?$Vector@$02@geode@@@absl@@I@Z
-	c44e	 1314  ?enable_edges@?$SurfaceMesh@$02@geode@@QEBAXXZ
-	c63a	 1299  ?edge_vertices@?$SurfaceEdges@$02@geode@@QEBAAEBV?$array@I$01@std@@I@Z
-	c53e	   74  ??$save_triangulated_surface@$02@geode@@YAXAEBV?$TriangulatedSurface@$02@0@Vstring_view@absl@@@Z
-	c3b6	 1655  ?polygons_around_vertex@?$SurfaceMesh@$02@geode@@QEBAAEBV?$InlinedVector@UPolygonVertex@geode@@$09V?$allocator@UPolygonVertex@geode@@@std@@@absl@@I@Z
-	c370	 1293  ?edge_length@?$SurfaceMesh@$02@geode@@QEBANAEBV?$array@I$01@std@@@Z
-	c340	 1575  ?nb_polygons@?$SurfaceMesh@$02@geode@@QEBAIXZ
-	c2ee	 1623  ?point@?$CoordinateReferenceSystemManagers@$02@geode@@QEBAAEBV?$Point@$02@2@I@Z
-	c216	  946  ?create@?$TriangulatedSurfaceBuilder@$02@geode@@SA?AV?$unique_ptr@V?$TriangulatedSurfaceBuilder@$02@geode@@U?$default_delete@V?$TriangulatedSurfaceBuilder@$02@geode@@@std@@@std@@AEAV?$TriangulatedSurface@$02@2@@Z
-	c1ca	 1977  ?vertex_attribute_manager@VertexSet@geode@@QEBAAEAVAttributeManager@2@XZ
-	c1a2	 1586  ?nb_vertices@VertexSet@geode@@QEBAIXZ
-	c4b2	 1307  ?edges@?$SurfaceMesh@$02@geode@@QEBAAEBV?$SurfaceEdges@$02@2@XZ
-	c60c	 1562  ?nb_edges@?$SurfaceEdges@$02@geode@@QEBAIXZ
-	c4f4	 1866  ?triangle@?$TriangulatedSurface@$02@geode@@QEBA?AV?$Triangle@$02@2@I@Z
-	c480	 1089  ?disable_edges@?$SurfaceMesh@$02@geode@@QEBAXXZ
+	c612	   60  ??$polygon_vertex_normal@$02@?$SurfaceMesh@$02@geode@@QEBA?AV?$optional@V?$Vector@$02@geode@@@absl@@I@Z
+	c4be	 1358  ?enable_edges@?$SurfaceMesh@$02@geode@@QEBAXXZ
+	c6aa	 1343  ?edge_vertices@?$SurfaceEdges@$02@geode@@QEBAAEBV?$array@I$01@std@@I@Z
+	c5ae	   81  ??$save_triangulated_surface@$02@geode@@YAXAEBV?$TriangulatedSurface@$02@0@Vstring_view@absl@@@Z
+	c426	 1699  ?polygons_around_vertex@?$SurfaceMesh@$02@geode@@QEBAAEBV?$InlinedVector@UPolygonVertex@geode@@$09V?$allocator@UPolygonVertex@geode@@@std@@@absl@@I@Z
+	c3e0	 1337  ?edge_length@?$SurfaceMesh@$02@geode@@QEBANAEBV?$array@I$01@std@@@Z
+	c3b0	 1619  ?nb_polygons@?$SurfaceMesh@$02@geode@@QEBAIXZ
+	c35e	 1667  ?point@?$CoordinateReferenceSystemManagers@$02@geode@@QEBAAEBV?$Point@$02@2@I@Z
+	c286	  990  ?create@?$TriangulatedSurfaceBuilder@$02@geode@@SA?AV?$unique_ptr@V?$TriangulatedSurfaceBuilder@$02@geode@@U?$default_delete@V?$TriangulatedSurfaceBuilder@$02@geode@@@std@@@std@@AEAV?$TriangulatedSurface@$02@2@@Z
+	c23a	 2021  ?vertex_attribute_manager@VertexSet@geode@@QEBAAEAVAttributeManager@2@XZ
+	c212	 1630  ?nb_vertices@VertexSet@geode@@QEBAIXZ
+	c522	 1351  ?edges@?$SurfaceMesh@$02@geode@@QEBAAEBV?$SurfaceEdges@$02@2@XZ
+	c67c	 1606  ?nb_edges@?$SurfaceEdges@$02@geode@@QEBAIXZ
+	c564	 1910  ?triangle@?$TriangulatedSurface@$02@geode@@QEBA?AV?$Triangle@$02@2@I@Z
+	c4f0	 1133  ?disable_edges@?$SurfaceMesh@$02@geode@@QEBAXXZ
 
- 0000b99c	0000bcc8 00000000 00000000 0000c7c4 00009228
+ 0000ba0c	0000bd38 00000000 00000000 0000c834 00009228
 
 	DLL Name: OpenGeode_geometry.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	c732	   11  ??$normal@$02@?$GenericTriangle@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBA?AV?$optional@V?$Vector@$02@geode@@@absl@@XZ
-	c698	  626  ?set_point@?$GenericTriangle@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEAAXIV?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@@Z
+	c7a2	   11  ??$normal@$02@?$GenericTriangle@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEBA?AV?$optional@V?$Vector@$02@geode@@@absl@@XZ
+	c708	  685  ?set_point@?$GenericTriangle@V?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@$02@geode@@QEAAXIV?$reference_wrapper@$$CBV?$Point@$02@geode@@@std@@@Z
 
- 0000b9b0	0000bc78 00000000 00000000 0000ca4c 000091d8
+ 0000ba20	0000bce8 00000000 00000000 0000cabc 000091d8
 
 	DLL Name: OpenGeode_basic.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	c7dc	  192  ?set_instance@Singleton@geode@@CAXAEBVtype_info@@PEAV12@@Z
-	c81a	  140  ?instance@Singleton@geode@@CAPEAV12@AEBVtype_info@@@Z
-	c852	   49  ??1Library@geode@@UEAA@XZ
-	c9d8	  176  ?register_attribute@AttributeManager@geode@@AEAAXV?$shared_ptr@VAttributeBase@geode@@@std@@Vstring_view@absl@@@Z
-	c962	  121  ?find_attribute_base@AttributeManager@geode@@AEBA?AV?$shared_ptr@VAttributeBase@geode@@@std@@Vstring_view@absl@@@Z
-	c91a	  102  ?delete_attribute@AttributeManager@geode@@QEAAXVstring_view@absl@@@Z
-	c8b8	  149  ?log_debug@Logger@geode@@CAXAEBV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@@Z
-	c88a	   89  ?call_initialize@Library@geode@@IEAAXPEBD@Z
-	c86e	   26  ??0Library@geode@@IEAA@XZ
+	c84c	  199  ?set_instance@Singleton@geode@@CAXAEBVtype_info@@PEAV12@@Z
+	c88a	  143  ?instance@Singleton@geode@@CAPEAV12@AEBVtype_info@@@Z
+	c8c2	   49  ??1Library@geode@@UEAA@XZ
+	ca48	  179  ?register_attribute@AttributeManager@geode@@AEAAXV?$shared_ptr@VAttributeBase@geode@@@std@@Vstring_view@absl@@@Z
+	c9d2	  123  ?find_attribute_base@AttributeManager@geode@@AEBA?AV?$shared_ptr@VAttributeBase@geode@@@std@@Vstring_view@absl@@@Z
+	c98a	  104  ?delete_attribute@AttributeManager@geode@@QEAAXVstring_view@absl@@@Z
+	c928	  152  ?log_debug@Logger@geode@@CAXAEBV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@@Z
+	c8fa	   91  ?call_initialize@Library@geode@@IEAAXPEBD@Z
+	c8de	   26  ??0Library@geode@@IEAA@XZ
 
- 0000b9c4	0000bde0 00000000 00000000 0000cafe 00009340
+ 0000ba34	0000be50 00000000 00000000 0000cb6e 00009340
 
 	DLL Name: absl_strings.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	ca98	  347  ?StrCat@absl@@YA?AV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@AEBVAlphaNum@1@00@Z
-	ca60	  298  ?FastIntToBuffer@numbers_internal@absl@@YAPEADIPEAD@Z
+	cb08	  347  ?StrCat@absl@@YA?AV?$basic_string@DU?$char_traits@D@std@@V?$allocator@D@2@@std@@AEBVAlphaNum@1@00@Z
+	cad0	  298  ?FastIntToBuffer@numbers_internal@absl@@YAPEADIPEAD@Z
 
- 0000b9d8	0000bb60 00000000 00000000 0000d334 000090c0
+ 0000ba48	0000bbd0 00000000 00000000 0000d3a4 000090c0
 
 	DLL Name: MSVCP140.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	d294	  427  ?_Fiopen@std@@YAPEAU_iobuf@@PEBDHH@Z
-	d258	  128  ??1?$basic_iostream@DU?$char_traits@D@std@@@std@@UEAA@XZ
-	d1ec	   19  ??0?$basic_iostream@DU?$char_traits@D@std@@@std@@QEAA@PEAV?$basic_streambuf@DU?$char_traits@D@std@@@1@@Z
-	d1a8	  872  ?flush@?$basic_ostream@DU?$char_traits@D@std@@@std@@QEAAAEAV12@XZ
-	d166	  260  ??6?$basic_ostream@DU?$char_traits@D@std@@@std@@QEAAAEAV01@N@Z
-	d124	  256  ??6?$basic_ostream@DU?$char_traits@D@std@@@std@@QEAAAEAV01@I@Z
-	d0e6	  580  ?_Osfx@?$basic_ostream@DU?$char_traits@D@std@@@std@@QEAAXXZ
-	d0b0	   12  ??0?$basic_ios@DU?$char_traits@D@std@@@std@@IEAA@XZ
-	d070	 1221  ?setstate@?$basic_ios@DU?$char_traits@D@std@@@std@@QEAAXH_N@Z
-	d032	  678  ?clear@?$basic_ios@DU?$char_traits@D@std@@@std@@QEAAXH_N@Z
-	cffc	  125  ??1?$basic_ios@DU?$char_traits@D@std@@@std@@UEAA@XZ
-	cfb4	 1350  ?xsputn@?$basic_streambuf@DU?$char_traits@D@std@@@std@@MEAA_JPEBD_J@Z
-	cf6c	 1347  ?xsgetn@?$basic_streambuf@DU?$char_traits@D@std@@@std@@MEAA_JPEAD_J@Z
-	cf1c	  500  ?_Init@?$basic_streambuf@DU?$char_traits@D@std@@@std@@IEAAXPEAPEAD0PEAH001@Z
-	d302	  969  ?id@?$codecvt@DDU_Mbstatet@@@std@@2V0locale@2@A
-	d2bc	 1237  ?showmanyc@?$basic_streambuf@DU?$char_traits@D@std@@@std@@MEAA_JXZ
-	cb10	  109  ??0_Lockit@std@@QEAA@H@Z
-	cb2c	  165  ??1_Lockit@std@@QEAA@XZ
-	cb46	  654  ?_Xlength_error@std@@YAXPEBD@Z
-	cb68	 1310  ?uncaught_exception@std@@YA_NXZ
-	cb8a	  305  ??Bid@locale@std@@QEAA_KXZ
-	cba8	  469  ?_Getgloballocale@locale@std@@CAPEAV_Locimp@12@XZ
-	cbdc	  669  ?always_noconv@codecvt_base@std@@QEBA_NXZ
-	cc08	 1018  ?in@?$codecvt@DDU_Mbstatet@@@std@@QEBAHAEAU_Mbstatet@@PEBD1AEAPEBDPEAD3AEAPEAD@Z
-	cc5c	 1075  ?out@?$codecvt@DDU_Mbstatet@@@std@@QEBAHAEAU_Mbstatet@@PEBD1AEAPEBDPEAD3AEAPEAD@Z
-	ccb0	 1319  ?unshift@?$codecvt@DDU_Mbstatet@@@std@@QEBAHAEAU_Mbstatet@@PEAD1AEAPEAD@Z
-	ccfc	  433  ?_Getcat@?$codecvt@DDU_Mbstatet@@@std@@SA_KPEAPEBVfacet@locale@2@PEBV42@@Z
-	cd4a	   47  ??0?$basic_streambuf@DU?$char_traits@D@std@@@std@@IEAA@XZ
-	cd86	  137  ??1?$basic_streambuf@DU?$char_traits@D@std@@@std@@UEAA@XZ
-	cdc2	  960  ?getloc@?$basic_streambuf@DU?$char_traits@D@std@@@std@@QEBA?AVlocale@2@XZ
-	ce0e	 1246  ?sputc@?$basic_streambuf@DU?$char_traits@D@std@@@std@@QEAAHD@Z
-	ce50	 1249  ?sputn@?$basic_streambuf@DU?$char_traits@D@std@@@std@@QEAA_JPEBD_J@Z
-	ce98	  586  ?_Pninc@?$basic_streambuf@DU?$char_traits@D@std@@@std@@IEAAPEADXZ
-	cedc	  501  ?_Init@?$basic_streambuf@DU?$char_traits@D@std@@@std@@IEAAXXZ
+	d304	  427  ?_Fiopen@std@@YAPEAU_iobuf@@PEBDHH@Z
+	d2c8	  128  ??1?$basic_iostream@DU?$char_traits@D@std@@@std@@UEAA@XZ
+	d25c	   19  ??0?$basic_iostream@DU?$char_traits@D@std@@@std@@QEAA@PEAV?$basic_streambuf@DU?$char_traits@D@std@@@1@@Z
+	d218	  872  ?flush@?$basic_ostream@DU?$char_traits@D@std@@@std@@QEAAAEAV12@XZ
+	d1d6	  260  ??6?$basic_ostream@DU?$char_traits@D@std@@@std@@QEAAAEAV01@N@Z
+	d194	  256  ??6?$basic_ostream@DU?$char_traits@D@std@@@std@@QEAAAEAV01@I@Z
+	d156	  580  ?_Osfx@?$basic_ostream@DU?$char_traits@D@std@@@std@@QEAAXXZ
+	d120	   12  ??0?$basic_ios@DU?$char_traits@D@std@@@std@@IEAA@XZ
+	d0e0	 1221  ?setstate@?$basic_ios@DU?$char_traits@D@std@@@std@@QEAAXH_N@Z
+	d0a2	  678  ?clear@?$basic_ios@DU?$char_traits@D@std@@@std@@QEAAXH_N@Z
+	d06c	  125  ??1?$basic_ios@DU?$char_traits@D@std@@@std@@UEAA@XZ
+	d024	 1350  ?xsputn@?$basic_streambuf@DU?$char_traits@D@std@@@std@@MEAA_JPEBD_J@Z
+	cfdc	 1347  ?xsgetn@?$basic_streambuf@DU?$char_traits@D@std@@@std@@MEAA_JPEAD_J@Z
+	cf8c	  500  ?_Init@?$basic_streambuf@DU?$char_traits@D@std@@@std@@IEAAXPEAPEAD0PEAH001@Z
+	d372	  969  ?id@?$codecvt@DDU_Mbstatet@@@std@@2V0locale@2@A
+	d32c	 1237  ?showmanyc@?$basic_streambuf@DU?$char_traits@D@std@@@std@@MEAA_JXZ
+	cb80	  109  ??0_Lockit@std@@QEAA@H@Z
+	cb9c	  165  ??1_Lockit@std@@QEAA@XZ
+	cbb6	  654  ?_Xlength_error@std@@YAXPEBD@Z
+	cbd8	 1310  ?uncaught_exception@std@@YA_NXZ
+	cbfa	  305  ??Bid@locale@std@@QEAA_KXZ
+	cc18	  469  ?_Getgloballocale@locale@std@@CAPEAV_Locimp@12@XZ
+	cc4c	  669  ?always_noconv@codecvt_base@std@@QEBA_NXZ
+	cc78	 1018  ?in@?$codecvt@DDU_Mbstatet@@@std@@QEBAHAEAU_Mbstatet@@PEBD1AEAPEBDPEAD3AEAPEAD@Z
+	cccc	 1075  ?out@?$codecvt@DDU_Mbstatet@@@std@@QEBAHAEAU_Mbstatet@@PEBD1AEAPEBDPEAD3AEAPEAD@Z
+	cd20	 1319  ?unshift@?$codecvt@DDU_Mbstatet@@@std@@QEBAHAEAU_Mbstatet@@PEAD1AEAPEAD@Z
+	cd6c	  433  ?_Getcat@?$codecvt@DDU_Mbstatet@@@std@@SA_KPEAPEBVfacet@locale@2@PEBV42@@Z
+	cdba	   47  ??0?$basic_streambuf@DU?$char_traits@D@std@@@std@@IEAA@XZ
+	cdf6	  137  ??1?$basic_streambuf@DU?$char_traits@D@std@@@std@@UEAA@XZ
+	ce32	  960  ?getloc@?$basic_streambuf@DU?$char_traits@D@std@@@std@@QEBA?AVlocale@2@XZ
+	ce7e	 1246  ?sputc@?$basic_streambuf@DU?$char_traits@D@std@@@std@@QEAAHD@Z
+	cec0	 1249  ?sputn@?$basic_streambuf@DU?$char_traits@D@std@@@std@@QEAA_JPEBD_J@Z
+	cf08	  586  ?_Pninc@?$basic_streambuf@DU?$char_traits@D@std@@@std@@IEAAPEADXZ
+	cf4c	  501  ?_Init@?$basic_streambuf@DU?$char_traits@D@std@@@std@@IEAAXXZ
 
- 0000b9ec	0000bdd0 00000000 00000000 0000d466 00009330
+ 0000ba5c	0000be40 00000000 00000000 0000d4d6 00009330
 
 	DLL Name: VCRUNTIME140_1.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	d342	    0  __CxxFrameHandler4
+	d3b2	    0  __CxxFrameHandler4
 
- 0000ba00	0000bd60 00000000 00000000 0000d47a 000092c0
+ 0000ba70	0000bdd0 00000000 00000000 0000d4ea 000092c0
 
 	DLL Name: VCRUNTIME140.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	d42e	    8  __C_specific_handler
-	d446	   37  __std_type_info_destroy_list
-	d3f0	   62  memset
-	d3dc	   60  memcpy
-	d3c6	    1  _CxxThrowException
-	d3ae	   39  __std_type_info_name
-	d394	   34  __std_exception_destroy
-	d37c	   33  __std_exception_copy
-	d36a	   35  __std_terminate
-	d358	   24  __RTDynamicCast
-	d410	   28  __current_exception_context
-	d3fa	   27  __current_exception
-	d3e6	   61  memmove
+	d49e	    8  __C_specific_handler
+	d4b6	   37  __std_type_info_destroy_list
+	d460	   62  memset
+	d44c	   60  memcpy
+	d436	    1  _CxxThrowException
+	d41e	   39  __std_type_info_name
+	d404	   34  __std_exception_destroy
+	d3ec	   33  __std_exception_copy
+	d3da	   35  __std_terminate
+	d3c8	   24  __RTDynamicCast
+	d480	   28  __current_exception_context
+	d46a	   27  __current_exception
+	d456	   61  memmove
 
- 0000ba14	0000be40 00000000 00000000 0000d65a 000093a0
+ 0000ba84	0000beb0 00000000 00000000 0000d6ca 000093a0
 
 	DLL Name: api-ms-win-crt-runtime-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	d63a	   30  _crt_atexit
-	d648	   22  _cexit
-	d606	   60  _register_onexit_function
-	d48c	   57  _invalid_parameter_noinfo_noreturn
-	d582	   54  _initterm
-	d5ae	   24  _configure_narrow_argv
-	d622	   34  _execute_onexit_table
-	d5c8	   51  _initialize_narrow_environment
-	d59c	   63  _seh_filter_dll
-	d5ea	   52  _initialize_onexit_table
-	d58e	   55  _initterm_e
-	d560	  103  terminate
+	d6aa	   30  _crt_atexit
+	d6b8	   22  _cexit
+	d676	   60  _register_onexit_function
+	d4fc	   57  _invalid_parameter_noinfo_noreturn
+	d5f2	   54  _initterm
+	d61e	   24  _configure_narrow_argv
+	d692	   34  _execute_onexit_table
+	d638	   51  _initialize_narrow_environment
+	d60c	   63  _seh_filter_dll
+	d65a	   52  _initialize_onexit_table
+	d5fe	   55  _initterm_e
+	d5d0	  103  terminate
 
- 0000ba28	0000bea8 00000000 00000000 0000d67c 00009408
+ 0000ba98	0000bf18 00000000 00000000 0000d6ec 00009408
 
 	DLL Name: api-ms-win-crt-stdio-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	d526	  152  setvbuf
-	d51c	  138  fwrite
-	d510	   47  _fseeki64
-	d506	  136  fsetpos
-	d4fe	  131  fread
-	d530	  157  ungetc
-	d4ec	  121  fgetpos
-	d4e4	  120  fgetc
-	d4da	  119  fflush
-	d4d0	  116  fclose
-	d4b2	   57  _get_stream_buffer_pointers
-	d4f6	  127  fputc
+	d596	  152  setvbuf
+	d58c	  138  fwrite
+	d580	   47  _fseeki64
+	d576	  136  fsetpos
+	d56e	  131  fread
+	d5a0	  157  ungetc
+	d55c	  121  fgetpos
+	d554	  120  fgetc
+	d54a	  119  fflush
+	d540	  116  fclose
+	d522	   57  _get_stream_buffer_pointers
+	d566	  127  fputc
 
- 0000ba3c	0000bdf8 00000000 00000000 0000d69c 00009358
+ 0000baac	0000be68 00000000 00000000 0000d70c 00009358
 
 	DLL Name: api-ms-win-crt-filesystem-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	d53a	   22  _lock_file
-	d548	   36  _unlock_file
+	d5aa	   22  _lock_file
+	d5b8	   36  _unlock_file
 
- 0000ba50	0000be30 00000000 00000000 0000d6c2 00009390
+ 0000bac0	0000bea0 00000000 00000000 0000d732 00009390
 
 	DLL Name: api-ms-win-crt-math-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	d558	  278  sqrt
+	d5c8	  278  sqrt
 
- 0000ba64	0000be10 00000000 00000000 0000d6e2 00009370
+ 0000bad4	0000be80 00000000 00000000 0000d752 00009370
 
 	DLL Name: api-ms-win-crt-heap-l1-1-0.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	d56c	    8  _callnewh
-	d578	   25  malloc
-	d652	   24  free
+	d5dc	    8  _callnewh
+	d5e8	   25  malloc
+	d6c2	   24  free
 
- 0000ba78	0000bae0 00000000 00000000 0000d868 00009040
+ 0000bae8	0000bb50 00000000 00000000 0000d8d8 00009040
 
 	DLL Name: KERNEL32.dll
 	vma:  Hint/Ord Member-Name Bound-To
-	d854	  928  IsDebuggerPresent
-	d838	  308  DisableThreadLibraryCalls
-	d81e	  778  GetSystemTimeAsFileTime
-	d808	  567  GetCurrentThreadId
-	d7f2	  563  GetCurrentProcessId
-	d7d8	 1136  QueryPerformanceCounter
-	d7bc	  936  IsProcessorFeaturePresent
-	d7a8	 1476  TerminateProcess
-	d794	  562  GetCurrentProcess
-	d776	 1444  SetUnhandledExceptionFilter
-	d75a	 1510  UnhandledExceptionFilter
-	d746	 1284  RtlVirtualUnwind
-	d72c	 1277  RtlLookupFunctionEntry
-	d718	 1269  RtlCaptureContext
-	d702	  906  InitializeSListHead
+	d8c4	  928  IsDebuggerPresent
+	d8a8	  308  DisableThreadLibraryCalls
+	d88e	  778  GetSystemTimeAsFileTime
+	d878	  567  GetCurrentThreadId
+	d862	  563  GetCurrentProcessId
+	d848	 1136  QueryPerformanceCounter
+	d82c	  936  IsProcessorFeaturePresent
+	d818	 1476  TerminateProcess
+	d804	  562  GetCurrentProcess
+	d7e6	 1444  SetUnhandledExceptionFilter
+	d7ca	 1510  UnhandledExceptionFilter
+	d7b6	 1284  RtlVirtualUnwind
+	d79c	 1277  RtlLookupFunctionEntry
+	d788	 1269  RtlCaptureContext
+	d772	  906  InitializeSListHead
 
- 0000ba8c	00000000 00000000 00000000 00000000 00000000
+ 0000bafc	00000000 00000000 00000000 00000000 00000000
 
-There is an export table in .rdata at 0x18000b7d0
+There is an export table in .rdata at 0x18000b840
 
 The Export Tables (interpreted .rdata section contents)
 
 Export Flags 			0
 Time/Date stamp 		ffffffff
 Major/Minor 			0/0
-Name 				000000000000b834 Geode-Viewables_qem_proxy.dll
+Name 				000000000000b8a4 Geode-Viewables_qem_proxy.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		00000006
 	[Name Pointer/Ordinal] Table	00000006
 Table Addresses
-	Export Address Table 		000000000000b7f8
-	Name Pointer Table 		000000000000b810
-	Ordinal Table 			000000000000b828
+	Export Address Table 		000000000000b868
+	Name Pointer Table 		000000000000b880
+	Ordinal Table 			000000000000b898
 
 Export Address Table -- Ordinal Base 1
 	[   0] +base[   1] 1010 Export RVA
 	[   1] +base[   2] 1040 Export RVA
 	[   2] +base[   3] 94f0 Export RVA
 	[   3] +base[   4] 10e0 Export RVA
 	[   4] +base[   5] 10f0 Export RVA
-	[   5] +base[   6] 5690 Export RVA
+	[   5] +base[   6] 5940 Export RVA
 
 [Ordinal/Name Pointer] Table
 	[   0] ??0ViewablesQEMProxyLibrary@geode@@QEAA@XZ
 	[   1] ??1ViewablesQEMProxyLibrary@geode@@UEAA@XZ
 	[   2] ??_7ViewablesQEMProxyLibrary@geode@@6B@
 	[   3] ?do_initialize@ViewablesQEMProxyLibrary@geode@@EEAAXXZ
 	[   4] ?initialize@ViewablesQEMProxyLibrary@geode@@SAXXZ
@@ -301,31 +301,31 @@
 The Function Table (interpreted .pdata section contents)
 vma:			BeginAddress	 EndAddress	  UnwindData
  000000018000f000:	0000000180001010 0000000180001032 000000018000aa80
  000000018000f00c:	0000000180001050 00000001800010dc 000000018000aa88
  000000018000f018:	00000001800010f0 0000000180001189 000000018000aa50
  000000018000f024:	0000000180001190 0000000180001290 000000018000ab60
  000000018000f030:	0000000180001290 0000000180001459 000000018000afac
- 000000018000f03c:	0000000180001460 0000000180001483 000000018000b3f4
- 000000018000f048:	0000000180001490 00000001800015c5 000000018000b1d8
- 000000018000f054:	00000001800015d0 0000000180001848 000000018000b30c
- 000000018000f060:	0000000180001850 0000000180001ac8 000000018000b30c
- 000000018000f06c:	0000000180001ad0 0000000180001b02 000000018000b250
- 000000018000f078:	0000000180001b02 0000000180001c2a 000000018000b260
- 000000018000f084:	0000000180001c2a 0000000180001c30 000000018000b27c
- 000000018000f090:	0000000180001c30 0000000180001c36 000000018000b28c
- 000000018000f09c:	0000000180001c40 0000000180001d79 000000018000b3bc
- 000000018000f0a8:	0000000180001d80 0000000180001eb8 000000018000b384
+ 000000018000f03c:	0000000180001460 0000000180001483 000000018000b468
+ 000000018000f048:	0000000180001490 00000001800015c5 000000018000b24c
+ 000000018000f054:	00000001800015d0 0000000180001848 000000018000b380
+ 000000018000f060:	0000000180001850 0000000180001ac8 000000018000b380
+ 000000018000f06c:	0000000180001ad0 0000000180001b02 000000018000b2c4
+ 000000018000f078:	0000000180001b02 0000000180001c2a 000000018000b2d4
+ 000000018000f084:	0000000180001c2a 0000000180001c30 000000018000b2f0
+ 000000018000f090:	0000000180001c30 0000000180001c36 000000018000b300
+ 000000018000f09c:	0000000180001c40 0000000180001d79 000000018000b430
+ 000000018000f0a8:	0000000180001d80 0000000180001eb8 000000018000b3f8
  000000018000f0b4:	0000000180001ec0 000000018000207f 000000018000ae14
- 000000018000f0c0:	0000000180002080 00000001800022fd 000000018000b2a8
- 000000018000f0cc:	0000000180002300 0000000180002557 000000018000b168
- 000000018000f0d8:	0000000180002560 00000001800025a5 000000018000b350
- 000000018000f0e4:	00000001800025a5 000000018000266f 000000018000b358
- 000000018000f0f0:	000000018000266f 0000000180002677 000000018000b374
- 000000018000f0fc:	0000000180002680 000000018000274f 000000018000b1a4
+ 000000018000f0c0:	0000000180002080 00000001800022fd 000000018000b31c
+ 000000018000f0cc:	0000000180002300 0000000180002557 000000018000b1dc
+ 000000018000f0d8:	0000000180002560 00000001800025a5 000000018000b3c4
+ 000000018000f0e4:	00000001800025a5 000000018000266f 000000018000b3cc
+ 000000018000f0f0:	000000018000266f 0000000180002677 000000018000b3e8
+ 000000018000f0fc:	0000000180002680 000000018000274f 000000018000b218
  000000018000f108:	0000000180002750 000000018000287c 000000018000aba4
  000000018000f114:	0000000180002880 00000001800028bc 000000018000aa80
  000000018000f120:	00000001800028c0 0000000180002a79 000000018000abd4
  000000018000f12c:	0000000180002a80 0000000180002abc 000000018000aa80
  000000018000f138:	0000000180002ac0 0000000180002afc 000000018000aa80
  000000018000f144:	0000000180002b30 0000000180002b6c 000000018000aa80
  000000018000f150:	0000000180002ba0 0000000180002bd2 000000018000aa80
@@ -342,31 +342,31 @@
  000000018000f1d4:	0000000180002f30 0000000180002f91 000000018000aa80
  000000018000f1e0:	0000000180002fa0 000000018000314c 000000018000b010
  000000018000f1ec:	0000000180003170 0000000180003174 000000018000aabc
  000000018000f1f8:	0000000180003174 000000018000318a 000000018000adb0
  000000018000f204:	000000018000318a 00000001800031c0 000000018000adc8
  000000018000f210:	00000001800031c0 00000001800031e5 000000018000addc
  000000018000f21c:	00000001800031e5 00000001800031f9 000000018000adec
- 000000018000f228:	0000000180003200 0000000180003224 000000018000b214
+ 000000018000f228:	0000000180003200 0000000180003224 000000018000b288
  000000018000f234:	0000000180003230 000000018000325f 000000018000aabc
- 000000018000f240:	0000000180003260 000000018000329d 000000018000b22c
+ 000000018000f240:	0000000180003260 000000018000329d 000000018000b2a0
  000000018000f24c:	00000001800032a0 0000000180003305 000000018000aa80
  000000018000f258:	0000000180003320 0000000180003360 000000018000aaa8
  000000018000f264:	0000000180003360 0000000180003381 000000018000aa80
  000000018000f270:	0000000180003390 00000001800033c4 000000018000aaa8
  000000018000f27c:	00000001800033d0 000000018000340b 000000018000aaa8
  000000018000f288:	0000000180003410 0000000180003452 000000018000aaa8
  000000018000f294:	0000000180003460 0000000180003509 000000018000ad9c
- 000000018000f2a0:	0000000180003510 00000001800035c1 000000018000b154
+ 000000018000f2a0:	0000000180003510 00000001800035c1 000000018000b1c8
  000000018000f2ac:	00000001800035d0 00000001800036ad 000000018000aaa8
  000000018000f2b8:	00000001800036f0 0000000180003725 000000018000af64
  000000018000f2c4:	0000000180003725 0000000180003784 000000018000af74
  000000018000f2d0:	0000000180003784 00000001800037c3 000000018000af88
  000000018000f2dc:	00000001800037c3 00000001800037d8 000000018000af9c
- 000000018000f2e8:	0000000180003820 00000001800038bd 000000018000b11c
+ 000000018000f2e8:	0000000180003820 00000001800038bd 000000018000b190
  000000018000f2f4:	00000001800038f0 0000000180003910 000000018000aab4
  000000018000f300:	0000000180003910 0000000180003930 000000018000aab4
  000000018000f30c:	0000000180003950 0000000180003961 000000018000aabc
  000000018000f318:	0000000180003970 0000000180003981 000000018000aabc
  000000018000f324:	0000000180003990 00000001800039a1 000000018000aabc
  000000018000f330:	00000001800039b0 00000001800039c1 000000018000aabc
  000000018000f33c:	00000001800039d0 0000000180003a40 000000018000aabc
@@ -377,346 +377,350 @@
  000000018000f378:	0000000180003c64 0000000180003c7a 000000018000aaec
  000000018000f384:	0000000180003c7a 0000000180003c81 000000018000aafc
  000000018000f390:	0000000180003c81 0000000180003c87 000000018000aaec
  000000018000f39c:	0000000180003c87 0000000180003c8d 000000018000aafc
  000000018000f3a8:	0000000180003c90 0000000180003e15 000000018000b030
  000000018000f3b4:	0000000180003e20 0000000180003ed0 000000018000ae14
  000000018000f3c0:	0000000180003f20 0000000180004553 000000018000ad20
- 000000018000f3cc:	0000000180004590 00000001800045d4 000000018000aaa8
- 000000018000f3d8:	00000001800045e0 0000000180004671 000000018000b080
- 000000018000f3e4:	0000000180004671 00000001800046d1 000000018000b090
- 000000018000f3f0:	00000001800046d1 00000001800046e2 000000018000b0a8
- 000000018000f3fc:	00000001800046f0 0000000180004733 000000018000aabc
- 000000018000f408:	0000000180004740 000000018000477f 000000018000aabc
- 000000018000f414:	0000000180004780 00000001800047c3 000000018000aabc
- 000000018000f420:	00000001800047e0 000000018000482d 000000018000acc8
- 000000018000f42c:	000000018000482d 0000000180004bb8 000000018000acd4
- 000000018000f438:	0000000180004bb8 0000000180004bc2 000000018000ad10
- 000000018000f444:	0000000180004bd0 0000000180004d9f 000000018000b0b8
- 000000018000f450:	0000000180004da0 0000000180004e84 000000018000ab70
- 000000018000f45c:	0000000180004e90 0000000180004ea2 000000018000aabc
- 000000018000f468:	0000000180004eb0 0000000180004f00 000000018000aaa8
- 000000018000f474:	0000000180004f20 0000000180004f80 000000018000ae24
- 000000018000f480:	0000000180004f80 00000001800050a2 000000018000ae38
- 000000018000f48c:	00000001800050a2 00000001800050c0 000000018000ae4c
- 000000018000f498:	00000001800050c0 00000001800051a2 000000018000aaa8
- 000000018000f4a4:	00000001800051b0 00000001800051cf 000000018000b028
- 000000018000f4b0:	0000000180005210 000000018000532e 000000018000ad9c
- 000000018000f4bc:	0000000180005330 00000001800053fb 000000018000b110
- 000000018000f4c8:	0000000180005400 00000001800054ca 000000018000af10
- 000000018000f4d4:	00000001800054d0 00000001800055a5 000000018000af24
- 000000018000f4e0:	00000001800055b0 00000001800055ee 000000018000af34
- 000000018000f4ec:	00000001800055ee 0000000180005683 000000018000af40
- 000000018000f4f8:	0000000180005683 000000018000568c 000000018000af54
- 000000018000f504:	0000000180005690 0000000180005721 000000018000ab10
- 000000018000f510:	0000000180005730 00000001800068ef 000000018000ac14
- 000000018000f51c:	00000001800068f0 0000000180006938 000000018000aa80
- 000000018000f528:	0000000180006940 0000000180006999 000000018000aa80
- 000000018000f534:	00000001800069a0 0000000180006c4b 000000018000ae84
- 000000018000f540:	0000000180006c50 0000000180006c83 000000018000aa80
- 000000018000f54c:	0000000180006c83 0000000180006c9d 000000018000ae5c
- 000000018000f558:	0000000180006c9d 0000000180006cb5 000000018000ae70
- 000000018000f564:	0000000180006cf0 0000000180006d43 000000018000aeb8
- 000000018000f570:	0000000180006d43 0000000180006e52 000000018000aec8
- 000000018000f57c:	0000000180006e52 0000000180006e57 000000018000aee0
- 000000018000f588:	0000000180006e60 0000000180006f34 000000018000aef8
- 000000018000f594:	0000000180006f9c 0000000180006fd4 000000018000aa80
- 000000018000f5a0:	0000000180006fec 0000000180007057 000000018000b424
- 000000018000f5ac:	0000000180007058 00000001800070b9 000000018000b44c
- 000000018000f5b8:	00000001800070bc 00000001800070f8 000000018000aa80
- 000000018000f5c4:	0000000180007108 0000000180007133 000000018000aa80
- 000000018000f5d0:	0000000180007134 0000000180007151 000000018000aabc
- 000000018000f5dc:	0000000180007154 00000001800071af 000000018000b484
- 000000018000f5e8:	00000001800071b0 000000018000722f 000000018000b48c
- 000000018000f5f4:	0000000180007240 000000018000725e 000000018000b4a8
- 000000018000f600:	000000018000727c 00000001800072cc 000000018000aabc
- 000000018000f60c:	00000001800072cc 00000001800073e2 000000018000b4ac
- 000000018000f618:	00000001800073e4 0000000180007468 000000018000b4e8
- 000000018000f624:	0000000180007468 0000000180007599 000000018000b53c
- 000000018000f630:	000000018000759c 00000001800075d9 000000018000ae14
- 000000018000f63c:	00000001800075dc 0000000180007615 000000018000aabc
- 000000018000f648:	0000000180007618 000000018000764c 000000018000aabc
- 000000018000f654:	000000018000764c 0000000180007661 000000018000aabc
- 000000018000f660:	0000000180007664 000000018000768c 000000018000aabc
- 000000018000f66c:	000000018000768c 00000001800076a1 000000018000aabc
- 000000018000f678:	00000001800076a4 0000000180007704 000000018000ad9c
- 000000018000f684:	0000000180007704 0000000180007734 000000018000aabc
- 000000018000f690:	0000000180007734 0000000180007748 000000018000aabc
- 000000018000f69c:	0000000180007748 0000000180007791 000000018000aa80
- 000000018000f6a8:	0000000180007794 000000018000781f 000000018000aa80
- 000000018000f6b4:	0000000180007820 00000001800078b8 000000018000b56c
- 000000018000f6c0:	00000001800078b8 00000001800078dc 000000018000aa80
- 000000018000f6cc:	00000001800078dc 0000000180007905 000000018000aa80
- 000000018000f6d8:	0000000180007908 0000000180007942 000000018000aa80
- 000000018000f6e4:	0000000180007944 000000018000795b 000000018000aabc
- 000000018000f6f0:	0000000180007980 00000001800079a0 000000018000aab4
- 000000018000f6fc:	00000001800079a8 00000001800079dc 000000018000aa80
- 000000018000f708:	00000001800079dc 0000000180007aae 000000018000b594
- 000000018000f714:	0000000180007ab0 0000000180007b21 000000018000b59c
- 000000018000f720:	0000000180007b24 0000000180007bd0 000000018000b5a8
- 000000018000f72c:	0000000180007bd0 0000000180007bf3 000000018000aabc
- 000000018000f738:	0000000180007c04 0000000180007c1f 000000018000aabc
- 000000018000f744:	0000000180007c30 0000000180007d7b 000000018000b5b4
- 000000018000f750:	0000000180007d7c 0000000180007db8 000000018000aaa8
- 000000018000f75c:	0000000180007db8 0000000180007df4 000000018000aaa8
- 000000018000f768:	0000000180007df4 0000000180007f95 000000018000b5c4
- 000000018000f774:	0000000180008070 0000000180008072 000000018000b5d8
- 000000018000f780:	0000000180008090 0000000180008096 000000018000b5e0
- 000000018000f78c:	00000001800080a0 00000001800080bd 000000018000aa78
- 000000018000f798:	00000001800080e0 000000018000811b 000000018000ad94
- 000000018000f7a4:	0000000180008120 0000000180008137 000000018000ad94
- 000000018000f7b0:	0000000180008140 0000000180008168 000000018000ad94
- 000000018000f7bc:	0000000180008170 0000000180008198 000000018000ad94
- 000000018000f7c8:	00000001800081a0 00000001800081d0 000000018000ad94
- 000000018000f7d4:	00000001800081d0 0000000180008200 000000018000ad94
- 000000018000f7e0:	0000000180008210 0000000180008239 000000018000aa78
- 000000018000f7ec:	0000000180008240 0000000180008260 000000018000aa78
- 000000018000f7f8:	0000000180008310 0000000180008340 000000018000ad94
- 000000018000f804:	0000000180008340 000000018000835d 000000018000aa78
- 000000018000f810:	00000001800083d0 0000000180008402 000000018000ad94
- 000000018000f81c:	0000000180008410 0000000180008430 000000018000aa78
- 000000018000f828:	0000000180008470 0000000180008496 000000018000aa78
- 000000018000f834:	00000001800084d0 00000001800084fe 000000018000aa78
- 000000018000f840:	000000018000856c 0000000180008598 000000018000aa78
- 000000018000f84c:	0000000180008598 00000001800085f7 000000018000b478
- 000000018000f858:	00000001800085f7 000000018000860e 000000018000aa78
- 000000018000f864:	000000018000860e 0000000180008627 000000018000aa78
- 000000018000f870:	0000000180008627 000000018000863b 000000018000aa78
- 000000018000f87c:	000000018000863b 0000000180008671 000000018000b564
- 000000018000f888:	0000000180008671 0000000180008689 000000018000b58c
- 000000018000f894:	000000018000868c 00000001800086e7 000000018000aa80
+ 000000018000f3cc:	0000000180004590 00000001800045d7 000000018000aaa8
+ 000000018000f3d8:	00000001800045e0 0000000180004648 000000018000b080
+ 000000018000f3e4:	0000000180004648 0000000180004709 000000018000b08c
+ 000000018000f3f0:	0000000180004709 000000018000475f 000000018000b0a0
+ 000000018000f3fc:	000000018000475f 0000000180004764 000000018000b0b4
+ 000000018000f408:	0000000180004764 000000018000476d 000000018000b0c4
+ 000000018000f414:	0000000180004770 00000001800047b3 000000018000aabc
+ 000000018000f420:	00000001800047c0 00000001800047ff 000000018000aabc
+ 000000018000f42c:	0000000180004800 0000000180004843 000000018000aabc
+ 000000018000f438:	0000000180004860 00000001800048ad 000000018000acc8
+ 000000018000f444:	00000001800048ad 0000000180004c3e 000000018000acd4
+ 000000018000f450:	0000000180004c3e 0000000180004c48 000000018000ad10
+ 000000018000f45c:	0000000180004c50 0000000180004ef3 000000018000b12c
+ 000000018000f468:	0000000180004f00 00000001800050d2 000000018000b0d4
+ 000000018000f474:	00000001800050e0 00000001800051c4 000000018000ab70
+ 000000018000f480:	00000001800051d0 00000001800051e5 000000018000aabc
+ 000000018000f48c:	00000001800051f0 0000000180005240 000000018000aaa8
+ 000000018000f498:	0000000180005260 00000001800052c0 000000018000ae24
+ 000000018000f4a4:	00000001800052c0 00000001800053e2 000000018000ae38
+ 000000018000f4b0:	00000001800053e2 0000000180005400 000000018000ae4c
+ 000000018000f4bc:	0000000180005400 00000001800054e2 000000018000aaa8
+ 000000018000f4c8:	00000001800054f0 000000018000550f 000000018000b028
+ 000000018000f4d4:	0000000180005550 00000001800055cc 000000018000ae14
+ 000000018000f4e0:	00000001800055d0 00000001800056a8 000000018000b180
+ 000000018000f4ec:	00000001800056b0 000000018000577a 000000018000af10
+ 000000018000f4f8:	0000000180005780 0000000180005855 000000018000af24
+ 000000018000f504:	0000000180005860 000000018000589e 000000018000af34
+ 000000018000f510:	000000018000589e 0000000180005933 000000018000af40
+ 000000018000f51c:	0000000180005933 000000018000593c 000000018000af54
+ 000000018000f528:	0000000180005940 00000001800059d1 000000018000ab10
+ 000000018000f534:	00000001800059e0 0000000180006baf 000000018000ac14
+ 000000018000f540:	0000000180006bb0 0000000180006bf8 000000018000aa80
+ 000000018000f54c:	0000000180006c00 0000000180006c59 000000018000aa80
+ 000000018000f558:	0000000180006c60 0000000180006f0b 000000018000ae84
+ 000000018000f564:	0000000180006f10 0000000180006f43 000000018000aa80
+ 000000018000f570:	0000000180006f43 0000000180006f5d 000000018000ae5c
+ 000000018000f57c:	0000000180006f5d 0000000180006f75 000000018000ae70
+ 000000018000f588:	0000000180006fb0 0000000180007003 000000018000aeb8
+ 000000018000f594:	0000000180007003 0000000180007112 000000018000aec8
+ 000000018000f5a0:	0000000180007112 0000000180007117 000000018000aee0
+ 000000018000f5ac:	0000000180007120 00000001800071f4 000000018000aef8
+ 000000018000f5b8:	000000018000725c 0000000180007294 000000018000aa80
+ 000000018000f5c4:	00000001800072ac 0000000180007317 000000018000b498
+ 000000018000f5d0:	0000000180007318 0000000180007379 000000018000b4c0
+ 000000018000f5dc:	000000018000737c 00000001800073b8 000000018000aa80
+ 000000018000f5e8:	00000001800073c8 00000001800073f3 000000018000aa80
+ 000000018000f5f4:	00000001800073f4 0000000180007411 000000018000aabc
+ 000000018000f600:	0000000180007414 000000018000746f 000000018000b4f8
+ 000000018000f60c:	0000000180007470 00000001800074ef 000000018000b500
+ 000000018000f618:	0000000180007500 000000018000751e 000000018000b518
+ 000000018000f624:	000000018000753c 000000018000758c 000000018000aabc
+ 000000018000f630:	000000018000758c 00000001800076a2 000000018000b51c
+ 000000018000f63c:	00000001800076a4 0000000180007728 000000018000b558
+ 000000018000f648:	0000000180007728 0000000180007859 000000018000b5ac
+ 000000018000f654:	000000018000785c 0000000180007899 000000018000ae14
+ 000000018000f660:	000000018000789c 00000001800078d5 000000018000aabc
+ 000000018000f66c:	00000001800078d8 000000018000790c 000000018000aabc
+ 000000018000f678:	000000018000790c 0000000180007921 000000018000aabc
+ 000000018000f684:	0000000180007924 000000018000794c 000000018000aabc
+ 000000018000f690:	000000018000794c 0000000180007961 000000018000aabc
+ 000000018000f69c:	0000000180007964 00000001800079c4 000000018000ad9c
+ 000000018000f6a8:	00000001800079c4 00000001800079f4 000000018000aabc
+ 000000018000f6b4:	00000001800079f4 0000000180007a08 000000018000aabc
+ 000000018000f6c0:	0000000180007a08 0000000180007a51 000000018000aa80
+ 000000018000f6cc:	0000000180007a54 0000000180007adf 000000018000aa80
+ 000000018000f6d8:	0000000180007ae0 0000000180007b78 000000018000b5dc
+ 000000018000f6e4:	0000000180007b78 0000000180007b9c 000000018000aa80
+ 000000018000f6f0:	0000000180007b9c 0000000180007bc5 000000018000aa80
+ 000000018000f6fc:	0000000180007bc8 0000000180007c02 000000018000aa80
+ 000000018000f708:	0000000180007c04 0000000180007c1b 000000018000aabc
+ 000000018000f714:	0000000180007c40 0000000180007c60 000000018000aab4
+ 000000018000f720:	0000000180007c68 0000000180007c9c 000000018000aa80
+ 000000018000f72c:	0000000180007c9c 0000000180007d6e 000000018000b604
+ 000000018000f738:	0000000180007d70 0000000180007de1 000000018000b60c
+ 000000018000f744:	0000000180007de4 0000000180007e90 000000018000b618
+ 000000018000f750:	0000000180007e90 0000000180007eb3 000000018000aabc
+ 000000018000f75c:	0000000180007ec4 0000000180007edf 000000018000aabc
+ 000000018000f768:	0000000180007ef0 000000018000803b 000000018000b624
+ 000000018000f774:	000000018000803c 0000000180008078 000000018000aaa8
+ 000000018000f780:	0000000180008078 00000001800080b4 000000018000aaa8
+ 000000018000f78c:	00000001800080b4 0000000180008255 000000018000b634
+ 000000018000f798:	0000000180008330 0000000180008332 000000018000b648
+ 000000018000f7a4:	0000000180008350 0000000180008356 000000018000b650
+ 000000018000f7b0:	0000000180008360 000000018000837d 000000018000aa78
+ 000000018000f7bc:	00000001800083a0 00000001800083db 000000018000ad94
+ 000000018000f7c8:	00000001800083e0 00000001800083f7 000000018000ad94
+ 000000018000f7d4:	0000000180008400 0000000180008428 000000018000ad94
+ 000000018000f7e0:	0000000180008430 0000000180008458 000000018000ad94
+ 000000018000f7ec:	0000000180008460 0000000180008490 000000018000ad94
+ 000000018000f7f8:	0000000180008490 00000001800084c0 000000018000ad94
+ 000000018000f804:	00000001800084d0 00000001800084f9 000000018000aa78
+ 000000018000f810:	0000000180008500 0000000180008520 000000018000aa78
+ 000000018000f81c:	00000001800085d0 0000000180008600 000000018000ad94
+ 000000018000f828:	0000000180008600 000000018000861d 000000018000aa78
+ 000000018000f834:	0000000180008690 00000001800086c2 000000018000ad94
+ 000000018000f840:	00000001800086d0 00000001800086ed 000000018000aa78
+ 000000018000f84c:	0000000180008730 0000000180008750 000000018000aa78
+ 000000018000f858:	0000000180008790 00000001800087b6 000000018000aa78
+ 000000018000f864:	00000001800087f0 000000018000881e 000000018000aa78
+ 000000018000f870:	000000018000888c 00000001800088b8 000000018000aa78
+ 000000018000f87c:	00000001800088b8 0000000180008917 000000018000b4ec
+ 000000018000f888:	0000000180008917 000000018000892e 000000018000aa78
+ 000000018000f894:	000000018000892e 0000000180008947 000000018000aa78
+ 000000018000f8a0:	0000000180008947 000000018000895b 000000018000aa78
+ 000000018000f8ac:	000000018000895b 0000000180008991 000000018000b5d4
+ 000000018000f8b8:	0000000180008991 00000001800089a9 000000018000b5fc
+ 000000018000f8c4:	00000001800089ac 0000000180008a07 000000018000aa80
 
 Dump of .rdata
  000000018000aa80 (rva: 0000aa80): 0000000180001010 - 0000000180001032
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
  000000018000aa88 (rva: 0000aa88): 0000000180001050 - 00000001800010dc
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 6, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0f: save rsi at rsp + 0x38
 	  pc+0x0f: save rbx at rsp + 0x30
 	  pc+0x0f: alloc small area: rsp = rsp - 0x20
 	  pc+0x0b: push rdi
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
 	  000: a0 aa 00 00 60 a5 aa 00 00 02 58 00
  000000018000aa50 (rva: 0000aa50): 00000001800010f0 - 0000000180001189
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x30
 	  pc+0x02: push rbx
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: 60 aa 00 00 28 69 aa 00 00 6f aa 00 00 02 0e a0
-	  010: 80 00 00 06 1a 00 7c 02 50 00 00 00
+	  000: 60 aa 00 00 28 69 aa 00 00 6f aa 00 00 02 0e 60
+	  010: 83 00 00 06 1a 00 7c 02 50 00 00 00
  000000018000ab60 (rva: 0000ab60): 0000000180001190 - 0000000180001290
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 2, Prologue size: 0x15, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x60
 	  pc+0x02: push rbx
-	Handler: 0000000180007134.
+	Handler: 00000001800073f4.
 	User data:
 	  000: 50 00 00 00
  000000018000afac (rva: 0000afac): 0000000180001290 - 0000000180001459
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 8, Prologue size: 0x16, Frame offset: 0x0, Frame reg: none
 	  pc+0x16: save rbx at rsp + 0x68
 	  pc+0x16: alloc small area: rsp = rsp - 0x30
 	  pc+0x12: push r15
 	  pc+0x10: push r14
 	  pc+0x0e: push r12
 	  pc+0x0c: push rdi
 	  pc+0x0b: push rsi
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
 	  000: c8 af 00 00 38 d5 af 00 00 ee af 00 00 ff af 00
 	  010: 00 0c 0a 00 32 00 00 40 3a 60 32 00 00 40 30 38
-	  020: 7e bc 7f 00 00 2e bc 7f 00 00 02 04 04 06 f6 af
-	  030: 00 00 02 11 80 e0 80 00 00 91 05 0e e2 00 54 02
+	  020: 7e 7c 82 00 00 2e 7c 82 00 00 02 04 04 06 f6 af
+	  030: 00 00 02 11 80 a0 83 00 00 91 05 0e e2 00 54 02
 	  040: b6 06 d8 04 4c 0a 26 0c 32 00 00 00
- 000000018000b3f4 (rva: 0000b3f4): 0000000180001460 - 0000000180001483
+ 000000018000b468 (rva: 0000b468): 0000000180001460 - 0000000180001483
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: 04 b4 00 00 38 3d b1 00 00 11 b4 00 00 20 b4 00
-	  010: 00 02 00 00 02 19 b4 00 00 02 01 80 20 81 00 00
+	  000: 78 b4 00 00 38 b1 b1 00 00 85 b4 00 00 94 b4 00
+	  010: 00 02 00 00 02 8d b4 00 00 02 01 80 e0 83 00 00
 	  020: 00 00 00 00
- 000000018000b1d8 (rva: 0000b1d8): 0000000180001490 - 00000001800015c5
+ 000000018000b24c (rva: 0000b24c): 0000000180001490 - 00000001800015c5
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 8, Prologue size: 0x14, Frame offset: 0x0, Frame reg: none
 	  pc+0x14: alloc small area: rsp = rsp - 0x20
 	  pc+0x10: push r15
 	  pc+0x0e: push r14
 	  pc+0x0c: push r13
 	  pc+0x0a: push r12
 	  pc+0x08: push rdi
 	  pc+0x07: push rsi
 	  pc+0x06: push rbx
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: f4 b1 00 00 38 3d b1 00 00 01 b2 00 00 10 b2 00
-	  010: 00 02 00 00 02 09 b2 00 00 02 01 80 40 81 00 00
+	  000: 68 b2 00 00 38 b1 b1 00 00 75 b2 00 00 84 b2 00
+	  010: 00 02 00 00 02 7d b2 00 00 02 01 80 00 84 00 00
 	  020: 02 fc 00 00
- 000000018000b30c (rva: 0000b30c): 00000001800015d0 - 0000000180001848
+ 000000018000b380 (rva: 0000b380): 00000001800015d0 - 0000000180001848
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 12, Prologue size: 0x21, Frame offset: 0x0, Frame reg: none
 	  pc+0x21: save xmm6 at rsp + 0x30
 	  pc+0x1c: save rsi at rsp + 0x88
 	  pc+0x1c: save rbx at rsp + 0x80
 	  pc+0x1c: alloc small area: rsp = rsp - 0x40
 	  pc+0x18: push r15
 	  pc+0x16: push r14
 	  pc+0x14: push r13
 	  pc+0x12: push r12
 	  pc+0x10: push rdi
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: 30 b3 00 00 38 3d b1 00 00 3d b3 00 00 4c b3 00
-	  010: 00 02 00 00 02 45 b3 00 00 02 01 80 70 81 00 00
+	  000: a4 b3 00 00 38 b1 b1 00 00 b1 b3 00 00 c0 b3 00
+	  010: 00 02 00 00 02 b9 b3 00 00 02 01 80 30 84 00 00
 	  020: 02 21 03 00
- 000000018000b30c also used for function at 0000000180001850
- 000000018000b250 (rva: 0000b250): 0000000180001ad0 - 0000000180001b02
+ 000000018000b380 also used for function at 0000000180001850
+ 000000018000b2c4 (rva: 0000b2c4): 0000000180001ad0 - 0000000180001b02
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0e, Frame offset: 0x0, Frame reg: none
 	  pc+0x0e: save rbx at rsp + 0x58
 	  pc+0x0e: alloc small area: rsp = rsp - 0x20
 	  pc+0x0a: push r15
 	  pc+0x08: push r14
 	  pc+0x06: push rsi
- 000000018000b260 (rva: 0000b260): 0000000180001b02 - 0000000180001c2a
+ 000000018000b2d4 (rva: 0000b2d4): 0000000180001b02 - 0000000180001c2a
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 6, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
 	  pc+0x13: save r12 at rsp + 0x50
 	  pc+0x0e: save rdi at rsp + 0x48
 	  pc+0x05: save rbp at rsp + 0x40
 	Chain: start: 0000000000001ad0, end: 0000000000001b02
-	 unwind data: 000000000000b250.
- 000000018000b27c (rva: 0000b27c): 0000000180001c2a - 0000000180001c30
+	 unwind data: 000000000000b2c4.
+ 000000018000b2f0 (rva: 0000b2f0): 0000000180001c2a - 0000000180001c30
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 	Chain: start: 0000000000001ad0, end: 0000000000001b02
-	 unwind data: 000000000000b250.
- 000000018000b28c (rva: 0000b28c): 0000000180001c30 - 0000000180001c36
+	 unwind data: 000000000000b2c4.
+ 000000018000b300 (rva: 0000b300): 0000000180001c30 - 0000000180001c36
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 6, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 	  pc+0x00: save r12 at rsp + 0x50
 	  pc+0x00: save rdi at rsp + 0x48
 	  pc+0x00: save rbp at rsp + 0x40
 	Chain: start: 0000000000001ad0, end: 0000000000001b02
-	 unwind data: 000000000000b250.
- 000000018000b3bc (rva: 0000b3bc): 0000000180001c40 - 0000000180001d79
+	 unwind data: 000000000000b2c4.
+ 000000018000b430 (rva: 0000b430): 0000000180001c40 - 0000000180001d79
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 6, Prologue size: 0x12, Frame offset: 0x0, Frame reg: none
 	  pc+0x12: save rbx at rsp + 0x50
 	  pc+0x12: alloc small area: rsp = rsp - 0x20
 	  pc+0x0e: push r14
 	  pc+0x0c: push rdi
 	  pc+0x0b: push rsi
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: d4 b3 00 00 38 3d b1 00 00 e1 b3 00 00 f0 b3 00
-	  010: 00 02 00 00 02 e9 b3 00 00 02 01 80 a0 81 00 00
+	  000: 48 b4 00 00 38 b1 b1 00 00 55 b4 00 00 64 b4 00
+	  010: 00 02 00 00 02 5d b4 00 00 02 01 80 60 84 00 00
 	  020: 02 55 02 00
- 000000018000b384 (rva: 0000b384): 0000000180001d80 - 0000000180001eb8
+ 000000018000b3f8 (rva: 0000b3f8): 0000000180001d80 - 0000000180001eb8
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 6, Prologue size: 0x10, Frame offset: 0x0, Frame reg: none
 	  pc+0x10: alloc small area: rsp = rsp - 0x20
 	  pc+0x0c: push r15
 	  pc+0x0a: push r14
 	  pc+0x08: push rdi
 	  pc+0x07: push rsi
 	  pc+0x06: push rbx
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: 9c b3 00 00 38 3d b1 00 00 a9 b3 00 00 b8 b3 00
-	  010: 00 02 00 00 02 b1 b3 00 00 02 01 80 d0 81 00 00
+	  000: 10 b4 00 00 38 b1 b1 00 00 1d b4 00 00 2c b4 00
+	  010: 00 02 00 00 02 25 b4 00 00 02 01 80 90 84 00 00
 	  020: 02 59 02 00
  000000018000ae14 (rva: 0000ae14): 0000000180001ec0 - 000000018000207f
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0f: save rsi at rsp + 0x38
 	  pc+0x0f: save rbx at rsp + 0x30
 	  pc+0x0f: alloc small area: rsp = rsp - 0x20
 	  pc+0x0b: push rdi
- 000000018000b2a8 (rva: 0000b2a8): 0000000180002080 - 00000001800022fd
+ 000000018000b31c (rva: 0000b31c): 0000000180002080 - 00000001800022fd
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 11, Prologue size: 0x1c, Frame offset: 0x0, Frame reg: none
 	  pc+0x1c: save rbx at rsp + 0xd0
 	  pc+0x1c: alloc large area: rsp = rsp - 0x90
 	  pc+0x15: push r15
 	  pc+0x13: push r14
 	  pc+0x11: push r13
 	  pc+0x0f: push r12
 	  pc+0x0d: push rdi
 	  pc+0x0c: push rsi
 	  pc+0x0b: push rbp
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: cc b2 00 00 28 d5 b2 00 00 fe b2 00 00 0e 0e 10
-	  010: 82 00 00 2a e0 2d 00 00 80 36 bc 7f 00 00 5e 40
-	  020: 82 00 00 2c 70 2c 00 00 81 03 3e 70 82 00 00 e2
+	  000: 40 b3 00 00 28 49 b3 00 00 72 b3 00 00 0e 0e d0
+	  010: 84 00 00 2a e0 2d 00 00 80 36 7c 82 00 00 5e 00
+	  020: 85 00 00 2c 70 2c 00 00 81 03 3e 30 85 00 00 e2
 	  030: 80 2c 00 00 81 03 0c 86 02 42 06 ca 04 de 0c 36
 	  040: 0e c9 02 04
- 000000018000b168 (rva: 0000b168): 0000000180002300 - 0000000180002557
+ 000000018000b1dc (rva: 0000b1dc): 0000000180002300 - 0000000180002557
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 12, Prologue size: 0x1c, Frame offset: 0x0, Frame reg: none
 	  pc+0x1c: save rsi at rsp + 0xa0
 	  pc+0x1c: save rbp at rsp + 0x98
 	  pc+0x1c: save rbx at rsp + 0x90
 	  pc+0x1c: alloc small area: rsp = rsp - 0x60
 	  pc+0x18: push r15
 	  pc+0x16: push r14
 	  pc+0x14: push r13
 	  pc+0x12: push r12
 	  pc+0x10: push rdi
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: 8c b1 00 00 28 95 b1 00 00 9c b1 00 00 02 0a a0
+	  000: 00 b2 00 00 28 09 b2 00 00 10 b2 00 00 02 0a a0
 	  010: 2c 00 00 80 04 a4 00 fd 07 02 00 00
- 000000018000b350 (rva: 0000b350): 0000000180002560 - 00000001800025a5
+ 000000018000b3c4 (rva: 0000b3c4): 0000000180002560 - 00000001800025a5
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc large area: rsp = rsp - 0x98
- 000000018000b358 (rva: 0000b358): 00000001800025a5 - 000000018000266f
+ 000000018000b3cc (rva: 0000b3cc): 00000001800025a5 - 000000018000266f
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 6, Prologue size: 0x28, Frame offset: 0x0, Frame reg: none
 	  pc+0x28: save xmm8 at rsp + 0x60
 	  pc+0x12: save xmm7 at rsp + 0x70
 	  pc+0x08: save xmm6 at rsp + 0x80
 	Chain: start: 0000000000002560, end: 00000000000025a5
-	 unwind data: 000000000000b350.
- 000000018000b374 (rva: 0000b374): 000000018000266f - 0000000180002677
+	 unwind data: 000000000000b3c4.
+ 000000018000b3e8 (rva: 0000b3e8): 000000018000266f - 0000000180002677
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 	Chain: start: 0000000000002560, end: 00000000000025a5
-	 unwind data: 000000000000b350.
- 000000018000b1a4 (rva: 0000b1a4): 0000000180002680 - 000000018000274f
+	 unwind data: 000000000000b3c4.
+ 000000018000b218 (rva: 0000b218): 0000000180002680 - 000000018000274f
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 4, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x20
 	  pc+0x04: push rdi
 	  pc+0x03: push rsi
 	  pc+0x02: push rbx
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: b8 b1 00 00 28 c1 b1 00 00 ce b1 00 00 04 0a 88
-	  010: 6f 00 00 80 32 80 2c 00 00 a0 08 58 02 d4 04 3a
+	  000: 2c b2 00 00 28 35 b2 00 00 42 b2 00 00 04 0a 48
+	  010: 72 00 00 80 32 80 2c 00 00 a0 08 58 02 d4 04 3a
 	  020: 00 2c 02 00
  000000018000aba4 (rva: 0000aba4): 0000000180002750 - 000000018000287c
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 6, Prologue size: 0x14, Frame offset: 0x0, Frame reg: none
 	  pc+0x14: save rsi at rsp + 0x48
 	  pc+0x14: save rbx at rsp + 0x40
 	  pc+0x14: alloc small area: rsp = rsp - 0x20
 	  pc+0x10: push rdi
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
 	  000: bc ab 00 00 28 c5 ab 00 00 cc ab 00 00 02 0c 20
 	  010: 2c 00 00 60 06 c9 02 02 c2 00 26 02
  000000018000aa80 (rva: 0000aa80): 0000000180002880 - 00000001800028bc
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
@@ -724,18 +728,18 @@
  000000018000abd4 (rva: 0000abd4): 00000001800028c0 - 0000000180002a79
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 5, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0f: alloc large area: rsp = rsp - 0xc0
 	  pc+0x08: push rdi
 	  pc+0x07: push rsi
 	  pc+0x06: push rbx
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: ec ab 00 00 28 f5 ab 00 00 0a ac 00 00 08 0e d0
-	  010: 82 00 00 2e e0 82 00 00 2e f0 82 00 00 2e 00 83
+	  000: ec ab 00 00 28 f5 ab 00 00 0a ac 00 00 08 0e 90
+	  010: 85 00 00 2e a0 85 00 00 2e b0 85 00 00 2e c0 85
 	  020: 00 00 08 3a 00 62 02 44 08 ed 04 00
  000000018000aa80 (rva: 0000aa80): 0000000180002a80 - 0000000180002abc
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
  000000018000aa80 also used for function at 0000000180002ac0
@@ -752,15 +756,15 @@
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
  000000018000adfc (rva: 0000adfc): 0000000180002d00 - 0000000180002d69
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
 	  000: 0c ae 00 00 60 11 ae 00 00 02 aa 00
  000000018000aa80 (rva: 0000aa80): 0000000180002d70 - 0000000180002dcf
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
@@ -815,34 +819,34 @@
 	Chain: start: 0000000000003174, end: 000000000000318a
 	 unwind data: 000000000000adb0.
  000000018000adec (rva: 0000adec): 00000001800031e5 - 00000001800031f9
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 	Chain: start: 0000000000003170, end: 0000000000003174
 	 unwind data: 000000000000aabc.
- 000000018000b214 (rva: 0000b214): 0000000180003200 - 0000000180003224
+ 000000018000b288 (rva: 0000b288): 0000000180003200 - 0000000180003224
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: 24 b2 00 00 60 29 b2 00 00 02 36 00
+	  000: 98 b2 00 00 60 9d b2 00 00 02 36 00
  000000018000aabc (rva: 0000aabc): 0000000180003230 - 000000018000325f
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000018000b22c (rva: 0000b22c): 0000000180003260 - 000000018000329d
+ 000000018000b2a0 (rva: 0000b2a0): 0000000180003260 - 000000018000329d
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: 3c b2 00 00 68 45 b2 00 00 4b b2 00 00 02 0e bc
-	  010: 7f 00 00 04 2a 00 3c 02
+	  000: b0 b2 00 00 68 b9 b2 00 00 bf b2 00 00 02 0e 7c
+	  010: 82 00 00 04 2a 00 3c 02
  000000018000aa80 (rva: 0000aa80): 00000001800032a0 - 0000000180003305
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
  000000018000aaa8 (rva: 0000aaa8): 0000000180003320 - 0000000180003360
 	Version: 1, Flags: none
@@ -867,15 +871,15 @@
 	Version: 1, Flags: none
 	Nbr codes: 8, Prologue size: 0x14, Frame offset: 0x0, Frame reg: none
 	  pc+0x14: save rsi at rsp + 0x40
 	  pc+0x14: save rbp at rsp + 0x38
 	  pc+0x14: save rbx at rsp + 0x30
 	  pc+0x14: alloc small area: rsp = rsp - 0x20
 	  pc+0x10: push rdi
- 000000018000b154 (rva: 0000b154): 0000000180003510 - 00000001800035c1
+ 000000018000b1c8 (rva: 0000b1c8): 0000000180003510 - 00000001800035c1
 	Version: 1, Flags: none
 	Nbr codes: 8, Prologue size: 0x15, Frame offset: 0x0, Frame reg: none
 	  pc+0x15: save rdi at rsp + 0x40
 	  pc+0x15: save rsi at rsp + 0x38
 	  pc+0x15: save rbx at rsp + 0x30
 	  pc+0x15: alloc small area: rsp = rsp - 0x20
 	  pc+0x11: push r14
@@ -886,15 +890,15 @@
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rdi
  000000018000af64 (rva: 0000af64): 00000001800036f0 - 0000000180003725
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 2, Prologue size: 0x15, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x60
 	  pc+0x02: push rbx
-	Handler: 0000000180007134.
+	Handler: 00000001800073f4.
 	User data:
 	  000: 58 00 00 00
  000000018000af74 (rva: 0000af74): 0000000180003725 - 0000000180003784
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: save rdi at rsp + 0x78
 	Chain: start: 00000000000036f0, end: 0000000000003725
@@ -906,26 +910,26 @@
 	Chain: start: 00000000000036f0, end: 0000000000003725
 	 unwind data: 000000000000af64.
  000000018000af9c (rva: 0000af9c): 00000001800037c3 - 00000001800037d8
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 	Chain: start: 00000000000036f0, end: 0000000000003725
 	 unwind data: 000000000000af64.
- 000000018000b11c (rva: 0000b11c): 0000000180003820 - 00000001800038bd
+ 000000018000b190 (rva: 0000b190): 0000000180003820 - 00000001800038bd
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 4, Prologue size: 0x11, Frame offset: 0x0, Frame reg: none
 	  pc+0x11: alloc small area: rsp = rsp - 0x20
 	  pc+0x0d: push rdi
 	  pc+0x0c: push rsi
 	  pc+0x0b: push rbx
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: 30 b1 00 00 38 3d b1 00 00 40 b1 00 00 4f b1 00
-	  010: 00 04 08 10 02 00 00 02 48 b1 00 00 02 01 80 10
-	  020: 83 00 00 02 7e 00 00 00
+	  000: a4 b1 00 00 38 b1 b1 00 00 b4 b1 00 00 c3 b1 00
+	  010: 00 04 08 10 02 00 00 02 bc b1 00 00 02 01 80 d0
+	  020: 85 00 00 02 7e 00 00 00
  000000018000aab4 (rva: 0000aab4): 00000001800038f0 - 0000000180003910
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x48
  000000018000aab4 also used for function at 0000000180003910
  000000018000aabc (rva: 0000aabc): 0000000180003950 - 0000000180003961
 	Version: 1, Flags: none
@@ -981,18 +985,18 @@
 	  pc+0x1b: save rbx at rsp + 0x60
 	  pc+0x1b: alloc small area: rsp = rsp - 0x30
 	  pc+0x17: push r15
 	  pc+0x15: push r14
 	  pc+0x13: push r12
 	  pc+0x11: push rdi
 	  pc+0x10: push rsi
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: 50 b0 00 00 28 59 b0 00 00 76 b0 00 00 0a 0e 40
-	  010: 83 00 00 2c 70 2c 00 00 d0 36 80 83 00 00 8a 80
+	  000: 50 b0 00 00 28 59 b0 00 00 76 b0 00 00 0a 0e 00
+	  010: 86 00 00 2c 70 2c 00 00 d0 36 40 86 00 00 8a 80
 	  020: 2c 00 00 d0 ba e0 2d 00 00 40 08 4c 00 cc 06 2a
 	  030: 08 95 02 0a
  000000018000ae14 (rva: 0000ae14): 0000000180003e20 - 0000000180003ed0
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0f: save rsi at rsp + 0x38
 	  pc+0x0f: save rbx at rsp + 0x30
@@ -1006,210 +1010,237 @@
 	  pc+0x0c: push r15
 	  pc+0x0a: push r14
 	  pc+0x08: push r13
 	  pc+0x06: push r12
 	  pc+0x04: push rdi
 	  pc+0x03: push rsi
 	  pc+0x02: push rbx
-	Handler: 00000001800071b0.
+	Handler: 0000000180007470.
 	User data:
 	  000: 48 ad 00 00 93 01 00 00 38 55 ad 00 00 6c ad 00
 	  010: 00 81 ad 00 00 0a 0a 20 2c 00 00 c1 04 3a 20 2c
 	  020: 00 00 41 03 3a a0 2c 00 00 50 30 38 02 06 06 08
-	  030: 74 ad 00 00 02 13 12 70 e1 00 00 d0 83 00 00 75
+	  030: 74 ad 00 00 02 13 12 70 e1 00 00 90 86 00 00 75
 	  040: 13 10 88 00 2e 02 38 04 36 06 4d 09 08 11 0c 00
 	  050: 5e 08 34 00
- 000000018000aaa8 (rva: 0000aaa8): 0000000180004590 - 00000001800045d4
+ 000000018000aaa8 (rva: 0000aaa8): 0000000180004590 - 00000001800045d7
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save rbx at rsp + 0x30
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rdi
- 000000018000b080 (rva: 0000b080): 00000001800045e0 - 0000000180004671
+ 000000018000b080 (rva: 0000b080): 00000001800045e0 - 0000000180004648
 	Version: 1, Flags: none
-	Nbr codes: 6, Prologue size: 0x10, Frame offset: 0x0, Frame reg: none
-	  pc+0x10: save rsi at rsp + 0x78
-	  pc+0x10: save rbx at rsp + 0x70
-	  pc+0x10: alloc small area: rsp = rsp - 0x50
-	  pc+0x0c: push r14
- 000000018000b090 (rva: 0000b090): 0000000180004671 - 00000001800046d1
+	Nbr codes: 4, Prologue size: 0x09, Frame offset: 0x0, Frame reg: none
+	  pc+0x09: alloc small area: rsp = rsp - 0x50
+	  pc+0x05: push r14
+	  pc+0x03: push rsi
+	  pc+0x02: push rbx
+ 000000018000b08c (rva: 0000b08c): 0000000180004648 - 0000000180004709
 	Version: 1, Flags: UNW_FLAG_CHAININFO
-	Nbr codes: 4, Prologue size: 0x0e, Frame offset: 0x0, Frame reg: none
-	  pc+0x0e: save rdi at rsp + 0x68
-	  pc+0x05: save rbp at rsp + 0x60
-	Chain: start: 00000000000045e0, end: 0000000000004671
+	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
+	  pc+0x05: save rdi at rsp + 0x78
+	Chain: start: 00000000000045e0, end: 0000000000004648
 	 unwind data: 000000000000b080.
- 000000018000b0a8 (rva: 0000b0a8): 00000001800046d1 - 00000001800046e2
+ 000000018000b0a0 (rva: 0000b0a0): 0000000180004709 - 000000018000475f
+	Version: 1, Flags: UNW_FLAG_CHAININFO
+	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
+	  pc+0x05: save rbp at rsp + 0x70
+	Chain: start: 0000000000004648, end: 0000000000004709
+	 unwind data: 000000000000b08c.
+ 000000018000b0b4 (rva: 0000b0b4): 000000018000475f - 0000000180004764
+	Version: 1, Flags: UNW_FLAG_CHAININFO
+	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
+	Chain: start: 0000000000004648, end: 0000000000004709
+	 unwind data: 000000000000b08c.
+ 000000018000b0c4 (rva: 0000b0c4): 0000000180004764 - 000000018000476d
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
-	Chain: start: 00000000000045e0, end: 0000000000004671
+	Chain: start: 00000000000045e0, end: 0000000000004648
 	 unwind data: 000000000000b080.
- 000000018000aabc (rva: 0000aabc): 00000001800046f0 - 0000000180004733
+ 000000018000aabc (rva: 0000aabc): 0000000180004770 - 00000001800047b3
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000018000aabc also used for function at 0000000180004740
- 000000018000aabc also used for function at 0000000180004780
- 000000018000acc8 (rva: 0000acc8): 00000001800047e0 - 000000018000482d
+ 000000018000aabc also used for function at 00000001800047c0
+ 000000018000aabc also used for function at 0000000180004800
+ 000000018000acc8 (rva: 0000acc8): 0000000180004860 - 00000001800048ad
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0f: alloc large area: rsp = rsp - 0x178
 	  pc+0x03: push rsi
 	  pc+0x02: push rbp
- 000000018000acd4 (rva: 0000acd4): 000000018000482d - 0000000180004bb8
+ 000000018000acd4 (rva: 0000acd4): 00000001800048ad - 0000000180004c3e
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 22, Prologue size: 0x68, Frame offset: 0x0, Frame reg: none
 	  pc+0x68: save xmm9 at rsp + 0x110
 	  pc+0x5f: save xmm8 at rsp + 0x120
 	  pc+0x56: save xmm7 at rsp + 0x130
 	  pc+0x4e: save xmm6 at rsp + 0x140
 	  pc+0x46: save r15 at rsp + 0x150
 	  pc+0x3e: save r14 at rsp + 0x158
 	  pc+0x36: save rbx at rsp + 0x1a8
 	  pc+0x2a: save xmm10 at rsp + 0x100
 	  pc+0x21: save r13 at rsp + 0x160
 	  pc+0x14: save r12 at rsp + 0x168
 	  pc+0x08: save rdi at rsp + 0x170
-	Chain: start: 00000000000047e0, end: 000000000000482d
+	Chain: start: 0000000000004860, end: 00000000000048ad
 	 unwind data: 000000000000acc8.
- 000000018000ad10 (rva: 0000ad10): 0000000180004bb8 - 0000000180004bc2
+ 000000018000ad10 (rva: 0000ad10): 0000000180004c3e - 0000000180004c48
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
-	Chain: start: 00000000000047e0, end: 000000000000482d
+	Chain: start: 0000000000004860, end: 00000000000048ad
 	 unwind data: 000000000000acc8.
- 000000018000b0b8 (rva: 0000b0b8): 0000000180004bd0 - 0000000180004d9f
+ 000000018000b12c (rva: 0000b12c): 0000000180004c50 - 0000000180004ef3
+	Version: 1, Flags: UNW_FLAG_UHANDLER
+	Nbr codes: 9, Prologue size: 0x1a, Frame offset: 0x0, Frame reg: none
+	  pc+0x1a: alloc small area: rsp = rsp - 0x68
+	  pc+0x16: push r15
+	  pc+0x14: push r14
+	  pc+0x12: push r13
+	  pc+0x10: push r12
+	  pc+0x0e: push rdi
+	  pc+0x0d: push rsi
+	  pc+0x0c: push rbp
+	  pc+0x0b: push rbx
+	Handler: 0000000180008270.
+	User data:
+	  000: 4c b1 00 00 28 55 b1 00 00 72 b1 00 00 0a 0e d0
+	  010: 86 00 00 2c 70 2c 00 00 60 36 10 87 00 00 8a 80
+	  020: 2c 00 00 60 ba e0 2d 00 00 70 0c 56 00 e4 06 3a
+	  030: 08 b0 0a 69 05 00 40 0a
+ 000000018000b0d4 (rva: 0000b0d4): 0000000180004f00 - 00000001800050d2
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 10, Prologue size: 0x19, Frame offset: 0x0, Frame reg: none
 	  pc+0x19: save rbx at rsp + 0xa8
 	  pc+0x19: alloc small area: rsp = rsp - 0x60
 	  pc+0x15: push r15
 	  pc+0x13: push r14
 	  pc+0x11: push r13
 	  pc+0x0f: push r12
 	  pc+0x0d: push rdi
 	  pc+0x0c: push rsi
 	  pc+0x0b: push rbp
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: d8 b0 00 00 28 e1 b0 00 00 00 b1 00 00 0a 0e 10
-	  010: 84 00 00 2c 70 2c 00 00 c1 02 3e 50 84 00 00 92
-	  020: 80 2c 00 00 c1 02 ca e0 2d 00 00 90 0c 54 00 d0
-	  030: 06 32 08 9a 0a 65 02 00 4e 0a 00 00
- 000000018000ab70 (rva: 0000ab70): 0000000180004da0 - 0000000180004e84
+	  000: f4 b0 00 00 28 fd b0 00 00 1c b1 00 00 0a 0e 30
+	  010: 87 00 00 2c 70 2c 00 00 c1 02 3e 70 87 00 00 92
+	  020: 80 2c 00 00 c1 02 ca e0 2d 00 00 90 0c 54 00 d8
+	  030: 06 30 08 a0 0a 59 02 00 4e 0a 00 00
+ 000000018000ab70 (rva: 0000ab70): 00000001800050e0 - 00000001800051c4
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 10, Prologue size: 0x1b, Frame offset: 0x0, Frame reg: none
 	  pc+0x1b: save rbp at rsp + 0x70
 	  pc+0x1b: save rbx at rsp + 0x68
 	  pc+0x1b: alloc small area: rsp = rsp - 0x30
 	  pc+0x17: push r15
 	  pc+0x15: push r14
 	  pc+0x13: push r12
 	  pc+0x11: push rdi
 	  pc+0x10: push rsi
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
-	  000: 90 ab 00 00 28 99 ab 00 00 9f ab 00 00 02 0e 70
-	  010: 84 00 00 02 c9 02 02 00
- 000000018000aabc (rva: 0000aabc): 0000000180004e90 - 0000000180004ea2
+	  000: 90 ab 00 00 28 99 ab 00 00 9f ab 00 00 02 0e 90
+	  010: 87 00 00 02 c9 02 02 00
+ 000000018000aabc (rva: 0000aabc): 00000001800051d0 - 00000001800051e5
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000018000aaa8 (rva: 0000aaa8): 0000000180004eb0 - 0000000180004f00
+ 000000018000aaa8 (rva: 0000aaa8): 00000001800051f0 - 0000000180005240
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save rbx at rsp + 0x30
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rdi
- 000000018000ae24 (rva: 0000ae24): 0000000180004f20 - 0000000180004f80
+ 000000018000ae24 (rva: 0000ae24): 0000000180005260 - 00000001800052c0
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 4, Prologue size: 0x1c, Frame offset: 0x0, Frame reg: none
 	  pc+0x0d: save rbx at rsp + 0xa8
 	  pc+0x0d: alloc small area: rsp = rsp - 0x80
 	  pc+0x06: push rdi
-	Handler: 0000000180007134.
+	Handler: 00000001800073f4.
 	User data:
 	  000: 78 00 00 00
- 000000018000ae38 (rva: 0000ae38): 0000000180004f80 - 00000001800050a2
+ 000000018000ae38 (rva: 0000ae38): 00000001800052c0 - 00000001800053e2
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 2, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: save rsi at rsp + 0xa0
-	Chain: start: 0000000000004f20, end: 0000000000004f80
+	Chain: start: 0000000000005260, end: 00000000000052c0
 	 unwind data: 000000000000ae24.
- 000000018000ae4c (rva: 0000ae4c): 00000001800050a2 - 00000001800050c0
+ 000000018000ae4c (rva: 0000ae4c): 00000001800053e2 - 0000000180005400
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
-	Chain: start: 0000000000004f20, end: 0000000000004f80
+	Chain: start: 0000000000005260, end: 00000000000052c0
 	 unwind data: 000000000000ae24.
- 000000018000aaa8 (rva: 0000aaa8): 00000001800050c0 - 00000001800051a2
+ 000000018000aaa8 (rva: 0000aaa8): 0000000180005400 - 00000001800054e2
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save rbx at rsp + 0x30
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rdi
- 000000018000b028 (rva: 0000b028): 00000001800051b0 - 00000001800051cf
+ 000000018000b028 (rva: 0000b028): 00000001800054f0 - 000000018000550f
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x38
- 000000018000ad9c (rva: 0000ad9c): 0000000180005210 - 000000018000532e
+ 000000018000ae14 (rva: 0000ae14): 0000000180005550 - 00000001800055cc
 	Version: 1, Flags: none
-	Nbr codes: 8, Prologue size: 0x14, Frame offset: 0x0, Frame reg: none
-	  pc+0x14: save rsi at rsp + 0x40
-	  pc+0x14: save rbp at rsp + 0x38
-	  pc+0x14: save rbx at rsp + 0x30
-	  pc+0x14: alloc small area: rsp = rsp - 0x20
-	  pc+0x10: push rdi
- 000000018000b110 (rva: 0000b110): 0000000180005330 - 00000001800053fb
+	Nbr codes: 6, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
+	  pc+0x0f: save rsi at rsp + 0x38
+	  pc+0x0f: save rbx at rsp + 0x30
+	  pc+0x0f: alloc small area: rsp = rsp - 0x20
+	  pc+0x0b: push rdi
+ 000000018000b180 (rva: 0000b180): 00000001800055d0 - 00000001800056a8
 	Version: 1, Flags: none
-	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
-	  pc+0x0a: save rbx at rsp + 0x38
-	  pc+0x0a: alloc small area: rsp = rsp - 0x20
-	  pc+0x06: push rdi
- 000000018000af10 (rva: 0000af10): 0000000180005400 - 00000001800054ca
+	Nbr codes: 5, Prologue size: 0x0b, Frame offset: 0x0, Frame reg: none
+	  pc+0x0b: save rsi at rsp + 0x18
+	  pc+0x0b: save rbx at rsp + 0x10
+	  pc+0x0b: push rdi
+ 000000018000af10 (rva: 0000af10): 00000001800056b0 - 000000018000577a
 	Version: 1, Flags: none
 	Nbr codes: 8, Prologue size: 0x14, Frame offset: 0x0, Frame reg: none
 	  pc+0x14: save rsi at rsp + 0x48
 	  pc+0x14: save rbp at rsp + 0x40
 	  pc+0x14: save rbx at rsp + 0x38
 	  pc+0x14: alloc small area: rsp = rsp - 0x20
 	  pc+0x10: push rdi
- 000000018000af24 (rva: 0000af24): 00000001800054d0 - 00000001800055a5
+ 000000018000af24 (rva: 0000af24): 0000000180005780 - 0000000180005855
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0f: save rsi at rsp + 0x40
 	  pc+0x0f: save rbx at rsp + 0x38
 	  pc+0x0f: alloc small area: rsp = rsp - 0x20
 	  pc+0x0b: push rdi
- 000000018000af34 (rva: 0000af34): 00000001800055b0 - 00000001800055ee
+ 000000018000af34 (rva: 0000af34): 0000000180005860 - 000000018000589e
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x28
 	  pc+0x03: push rsi
 	  pc+0x02: push rbx
- 000000018000af40 (rva: 0000af40): 00000001800055ee - 0000000180005683
+ 000000018000af40 (rva: 0000af40): 000000018000589e - 0000000180005933
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: save rdi at rsp + 0x20
-	Chain: start: 00000000000055b0, end: 00000000000055ee
+	Chain: start: 0000000000005860, end: 000000000000589e
 	 unwind data: 000000000000af34.
- 000000018000af54 (rva: 0000af54): 0000000180005683 - 000000018000568c
+ 000000018000af54 (rva: 0000af54): 0000000180005933 - 000000018000593c
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
-	Chain: start: 00000000000055b0, end: 00000000000055ee
+	Chain: start: 0000000000005860, end: 000000000000589e
 	 unwind data: 000000000000af34.
- 000000018000ab10 (rva: 0000ab10): 0000000180005690 - 0000000180005721
+ 000000018000ab10 (rva: 0000ab10): 0000000180005940 - 00000001800059d1
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save rbx at rsp + 0x80
 	  pc+0x0a: alloc small area: rsp = rsp - 0x70
 	  pc+0x06: push rdi
-	Handler: 0000000180007fb0.
+	Handler: 0000000180008270.
 	User data:
 	  000: 24 ab 00 00 28 2d ab 00 00 34 ab 00 00 02 0a 70
 	  010: 31 00 00 40 04 24 00 16 02 00 00 00
- 000000018000ac14 (rva: 0000ac14): 0000000180005730 - 00000001800068ef
+ 000000018000ac14 (rva: 0000ac14): 00000001800059e0 - 0000000180006baf
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 29, Prologue size: 0x66, Frame offset: 0x0, Frame reg: none
 	  pc+0x55: save xmm13 at rsp + 0x410
 	  pc+0x4d: save xmm12 at rsp + 0x420
 	  pc+0x45: save xmm11 at rsp + 0x430
 	  pc+0x3d: save xmm10 at rsp + 0x440
 	  pc+0x38: save xmm9 at rsp + 0x450
@@ -1221,339 +1252,337 @@
 	  pc+0x26: save rbx at rsp + 0x4c8
 	  pc+0x26: alloc large area: rsp = rsp - 0x490
 	  pc+0x18: push r15
 	  pc+0x16: push r14
 	  pc+0x14: push r13
 	  pc+0x12: push r12
 	  pc+0x10: push rbp
-	Handler: 00000001800071b0.
+	Handler: 0000000180007470.
 	User data:
 	  000: 60 ac 00 00 02 04 00 00 28 69 ac 00 00 9d ac 00
-	  010: 00 10 0e d0 84 00 00 2e 00 85 00 00 2c da 6f 00
+	  010: 00 10 0e f0 87 00 00 2e 20 88 00 00 2c 9a 72 00
 	  020: 00 01 09 92 a0 32 00 00 c0 32 30 32 00 00 01 09
 	  030: 6a a0 2f 00 00 01 0d 3a 70 2d 00 00 01 09 da 70
 	  040: 2d 00 00 c1 0e 20 e4 00 31 03 02 38 04 80 06 64
-	  050: 08 39 03 0a 5c 08 35 0e 0c 11 13 0e 14 0c 15 02
-	  060: 08 11 0a 0c 36 08 b5 07 10 14 08 8d 03 00 00 00
- 000000018000aa80 (rva: 0000aa80): 00000001800068f0 - 0000000180006938
+	  050: 08 39 03 0a 5c 08 35 0e 0c 3d 13 0e 14 0c 15 02
+	  060: 08 21 0a 0c 36 08 b9 07 10 14 08 8d 03 00 00 00
+ 000000018000aa80 (rva: 0000aa80): 0000000180006bb0 - 0000000180006bf8
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
- 000000018000aa80 also used for function at 0000000180006940
- 000000018000ae84 (rva: 0000ae84): 00000001800069a0 - 0000000180006c4b
+ 000000018000aa80 also used for function at 0000000180006c00
+ 000000018000ae84 (rva: 0000ae84): 0000000180006c60 - 0000000180006f0b
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 6, Prologue size: 0x23, Frame offset: 0x0, Frame reg: none
 	  pc+0x15: save rdi at rsp + 0xa0
 	  pc+0x15: save rbx at rsp + 0x98
 	  pc+0x15: alloc small area: rsp = rsp - 0x80
 	  pc+0x0b: push rbp
-	Handler: 00000001800071b0.
+	Handler: 0000000180007470.
 	User data:
 	  000: a0 ae 00 00 7a 00 00 00 28 a9 ae 00 00 b0 ae 00
 	  010: 00 02 0a 70 2d 00 00 b0 04 b1 04 02 79 04 00 00
- 000000018000aa80 (rva: 0000aa80): 0000000180006c50 - 0000000180006c83
+ 000000018000aa80 (rva: 0000aa80): 0000000180006f10 - 0000000180006f43
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
- 000000018000ae5c (rva: 0000ae5c): 0000000180006c83 - 0000000180006c9d
+ 000000018000ae5c (rva: 0000ae5c): 0000000180006f43 - 0000000180006f5d
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: save rdi at rsp + 0x30
-	Chain: start: 0000000000006c50, end: 0000000000006c83
+	Chain: start: 0000000000006f10, end: 0000000000006f43
 	 unwind data: 000000000000aa80.
- 000000018000ae70 (rva: 0000ae70): 0000000180006c9d - 0000000180006cb5
+ 000000018000ae70 (rva: 0000ae70): 0000000180006f5d - 0000000180006f75
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 2, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 	  pc+0x00: save rdi at rsp + 0x30
-	Chain: start: 0000000000006c50, end: 0000000000006c83
+	Chain: start: 0000000000006f10, end: 0000000000006f43
 	 unwind data: 000000000000aa80.
- 000000018000aeb8 (rva: 0000aeb8): 0000000180006cf0 - 0000000180006d43
+ 000000018000aeb8 (rva: 0000aeb8): 0000000180006fb0 - 0000000180007003
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x10, Frame offset: 0x0, Frame reg: none
 	  pc+0x10: save rsi at rsp + 0x48
 	  pc+0x10: save rbp at rsp + 0x40
 	  pc+0x10: alloc small area: rsp = rsp - 0x20
 	  pc+0x0c: push r14
- 000000018000aec8 (rva: 0000aec8): 0000000180006d43 - 0000000180006e52
+ 000000018000aec8 (rva: 0000aec8): 0000000180007003 - 0000000180007112
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save rdi at rsp + 0x38
 	  pc+0x05: save rbx at rsp + 0x30
-	Chain: start: 0000000000006cf0, end: 0000000000006d43
+	Chain: start: 0000000000006fb0, end: 0000000000007003
 	 unwind data: 000000000000aeb8.
- 000000018000aee0 (rva: 0000aee0): 0000000180006e52 - 0000000180006e57
+ 000000018000aee0 (rva: 0000aee0): 0000000180007112 - 0000000180007117
 	Version: 1, Flags: UNW_FLAG_CHAININFO
 	Nbr codes: 4, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 	  pc+0x00: save rdi at rsp + 0x38
 	  pc+0x00: save rbx at rsp + 0x30
-	Chain: start: 0000000000006cf0, end: 0000000000006d43
+	Chain: start: 0000000000006fb0, end: 0000000000007003
 	 unwind data: 000000000000aeb8.
- 000000018000aef8 (rva: 0000aef8): 0000000180006e60 - 0000000180006f34
+ 000000018000aef8 (rva: 0000aef8): 0000000180007120 - 00000001800071f4
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x45, Frame offset: 0x0, Frame reg: none
 	  pc+0x45: save rsi at rsp + 0x38
 	  pc+0x40: save rbp at rsp + 0x30
 	  pc+0x10: save rdi at rsp + 0x48
 	  pc+0x10: save rbx at rsp + 0x40
 	  pc+0x10: alloc small area: rsp = rsp - 0x20
 	  pc+0x0c: push r14
- 000000018000aa80 (rva: 0000aa80): 0000000180006f9c - 0000000180006fd4
+ 000000018000aa80 (rva: 0000aa80): 000000018000725c - 0000000180007294
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
- 000000018000b424 (rva: 0000b424): 0000000180006fec - 0000000180007057
+ 000000018000b498 (rva: 0000b498): 00000001800072ac - 0000000180007317
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 5, Prologue size: 0x18, Frame offset: 0x0, Frame reg: none
 	  pc+0x18: alloc small area: rsp = rsp - 0x38
 	  pc+0x14: push r14
 	  pc+0x12: push rdi
 	  pc+0x11: push rsi
 	  pc+0x10: push rbx
-	Handler: 0000000180007ff8.
+	Handler: 00000001800082b8.
 	User data:
-	  000: 01 00 00 00 1f 70 00 00 4d 70 00 00 6c 85 00 00
+	  000: 01 00 00 00 df 72 00 00 0d 73 00 00 8c 88 00 00
 	  010: 00 00 00 00
- 000000018000b44c (rva: 0000b44c): 0000000180007058 - 00000001800070b9
+ 000000018000b4c0 (rva: 0000b4c0): 0000000180007318 - 0000000180007379
 	Version: 1, Flags: UNW_FLAG_EHANDLER
 	Nbr codes: 8, Prologue size: 0x18, Frame offset: 0x0, Frame reg: none
 	  pc+0x18: save rsi at rsp + 0x80
 	  pc+0x18: save rbx at rsp + 0x78
 	  pc+0x18: alloc small area: rsp = rsp - 0x50
 	  pc+0x14: push r15
 	  pc+0x12: push r14
 	  pc+0x10: push rdi
-	Handler: 0000000180007ff8.
+	Handler: 00000001800082b8.
 	User data:
-	  000: 01 00 00 00 7c 70 00 00 a3 70 00 00 98 85 00 00
-	  010: a3 70 00 00
- 000000018000aa80 (rva: 0000aa80): 00000001800070bc - 00000001800070f8
+	  000: 01 00 00 00 3c 73 00 00 63 73 00 00 b8 88 00 00
+	  010: 63 73 00 00
+ 000000018000aa80 (rva: 0000aa80): 000000018000737c - 00000001800073b8
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
- 000000018000aa80 also used for function at 0000000180007108
- 000000018000aabc (rva: 0000aabc): 0000000180007134 - 0000000180007151
+ 000000018000aa80 also used for function at 00000001800073c8
+ 000000018000aabc (rva: 0000aabc): 00000001800073f4 - 0000000180007411
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000018000b484 (rva: 0000b484): 0000000180007154 - 00000001800071af
+ 000000018000b4f8 (rva: 0000b4f8): 0000000180007414 - 000000018000746f
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x02, Frame offset: 0x0, Frame reg: none
 	  pc+0x02: push rbx
- 000000018000b48c (rva: 0000b48c): 00000001800071b0 - 000000018000722f
+ 000000018000b500 (rva: 0000b500): 0000000180007470 - 00000001800074ef
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x19, Frame offset: 0x0, Frame reg: none
 	  pc+0x19: save rdi at rsp + 0x48
 	  pc+0x19: save rsi at rsp + 0x40
 	  pc+0x19: save rbp at rsp + 0x38
 	  pc+0x19: save rbx at rsp + 0x30
 	  pc+0x19: alloc small area: rsp = rsp - 0x20
 	  pc+0x15: push r14
-	User data:
-	  000: 00 00 00 00
- 000000018000b4a8 (rva: 0000b4a8): 0000000180007240 - 000000018000725e
+ 000000018000b518 (rva: 0000b518): 0000000180007500 - 000000018000751e
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 000000018000aabc (rva: 0000aabc): 000000018000727c - 00000001800072cc
+ 000000018000aabc (rva: 0000aabc): 000000018000753c - 000000018000758c
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000018000b4ac (rva: 0000b4ac): 00000001800072cc - 00000001800073e2
+ 000000018000b51c (rva: 0000b51c): 000000018000758c - 00000001800076a2
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 8, Prologue size: 0x15, Frame offset: 0x0, Frame reg: none
 	  pc+0x15: save rdi at rsp + 0x48
 	  pc+0x15: save rsi at rsp + 0x38
 	  pc+0x15: save rbx at rsp + 0x30
 	  pc+0x15: alloc small area: rsp = rsp - 0x20
 	  pc+0x11: push r14
-	Handler: 0000000180007ff8.
+	Handler: 00000001800082b8.
 	User data:
-	  000: 02 00 00 00 04 73 00 00 73 73 00 00 f7 85 00 00
-	  010: 00 00 00 00 d6 73 00 00 e1 73 00 00 f7 85 00 00
+	  000: 02 00 00 00 c4 75 00 00 33 76 00 00 17 89 00 00
+	  010: 00 00 00 00 96 76 00 00 a1 76 00 00 17 89 00 00
 	  020: 00 00 00 00
- 000000018000b4e8 (rva: 0000b4e8): 00000001800073e4 - 0000000180007468
+ 000000018000b558 (rva: 0000b558): 00000001800076a4 - 0000000180007728
 	Version: 1, Flags: UNW_FLAG_UHANDLER
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save rbx at rsp + 0x40
 	  pc+0x0a: alloc small area: rsp = rsp - 0x30
 	  pc+0x06: push rdi
-	Handler: 0000000180007ff8.
+	Handler: 00000001800082b8.
 	User data:
-	  000: 04 00 00 00 1b 74 00 00 3a 74 00 00 0e 86 00 00
-	  010: 00 00 00 00 10 74 00 00 52 74 00 00 27 86 00 00
-	  020: 00 00 00 00 5b 74 00 00 66 74 00 00 0e 86 00 00
-	  030: 00 00 00 00 5b 74 00 00 67 74 00 00 27 86 00 00
+	  000: 04 00 00 00 db 76 00 00 fa 76 00 00 2e 89 00 00
+	  010: 00 00 00 00 d0 76 00 00 12 77 00 00 47 89 00 00
+	  020: 00 00 00 00 1b 77 00 00 26 77 00 00 2e 89 00 00
+	  030: 00 00 00 00 1b 77 00 00 27 77 00 00 47 89 00 00
 	  040: 00 00 00 00
- 000000018000b53c (rva: 0000b53c): 0000000180007468 - 0000000180007599
+ 000000018000b5ac (rva: 0000b5ac): 0000000180007728 - 0000000180007859
 	Version: 1, Flags: UNW_FLAG_EHANDLER
 	Nbr codes: 6, Prologue size: 0x1a, Frame offset: 0x0, Frame reg: none
 	  pc+0x1a: save rbx at rsp + 0x78
 	  pc+0x1a: alloc small area: rsp = rsp - 0x40
 	  pc+0x16: push r14
 	  pc+0x14: push rdi
 	  pc+0x13: push rsi
-	Handler: 0000000180007ff8.
+	Handler: 00000001800082b8.
 	User data:
-	  000: 01 00 00 00 9d 74 00 00 83 75 00 00 3b 86 00 00
-	  010: 83 75 00 00
- 000000018000ae14 (rva: 0000ae14): 000000018000759c - 00000001800075d9
+	  000: 01 00 00 00 5d 77 00 00 43 78 00 00 5b 89 00 00
+	  010: 43 78 00 00
+ 000000018000ae14 (rva: 0000ae14): 000000018000785c - 0000000180007899
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0f: save rsi at rsp + 0x38
 	  pc+0x0f: save rbx at rsp + 0x30
 	  pc+0x0f: alloc small area: rsp = rsp - 0x20
 	  pc+0x0b: push rdi
- 000000018000aabc (rva: 0000aabc): 00000001800075dc - 0000000180007615
+ 000000018000aabc (rva: 0000aabc): 000000018000789c - 00000001800078d5
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000018000aabc also used for function at 0000000180007618
- 000000018000aabc also used for function at 000000018000764c
- 000000018000aabc also used for function at 0000000180007664
- 000000018000aabc also used for function at 000000018000768c
- 000000018000ad9c (rva: 0000ad9c): 00000001800076a4 - 0000000180007704
+ 000000018000aabc also used for function at 00000001800078d8
+ 000000018000aabc also used for function at 000000018000790c
+ 000000018000aabc also used for function at 0000000180007924
+ 000000018000aabc also used for function at 000000018000794c
+ 000000018000ad9c (rva: 0000ad9c): 0000000180007964 - 00000001800079c4
 	Version: 1, Flags: none
 	Nbr codes: 8, Prologue size: 0x14, Frame offset: 0x0, Frame reg: none
 	  pc+0x14: save rsi at rsp + 0x40
 	  pc+0x14: save rbp at rsp + 0x38
 	  pc+0x14: save rbx at rsp + 0x30
 	  pc+0x14: alloc small area: rsp = rsp - 0x20
 	  pc+0x10: push rdi
- 000000018000aabc (rva: 0000aabc): 0000000180007704 - 0000000180007734
+ 000000018000aabc (rva: 0000aabc): 00000001800079c4 - 00000001800079f4
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000018000aabc also used for function at 0000000180007734
- 000000018000aa80 (rva: 0000aa80): 0000000180007748 - 0000000180007791
+ 000000018000aabc also used for function at 00000001800079f4
+ 000000018000aa80 (rva: 0000aa80): 0000000180007a08 - 0000000180007a51
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
- 000000018000aa80 also used for function at 0000000180007794
- 000000018000b56c (rva: 0000b56c): 0000000180007820 - 00000001800078b8
+ 000000018000aa80 also used for function at 0000000180007a54
+ 000000018000b5dc (rva: 0000b5dc): 0000000180007ae0 - 0000000180007b78
 	Version: 1, Flags: UNW_FLAG_EHANDLER
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x18
-	Handler: 0000000180007ff8.
+	Handler: 00000001800082b8.
 	User data:
-	  000: 01 00 00 00 27 78 00 00 b1 78 00 00 71 86 00 00
-	  010: b1 78 00 00
- 000000018000aa80 (rva: 0000aa80): 00000001800078b8 - 00000001800078dc
+	  000: 01 00 00 00 e7 7a 00 00 71 7b 00 00 91 89 00 00
+	  010: 71 7b 00 00
+ 000000018000aa80 (rva: 0000aa80): 0000000180007b78 - 0000000180007b9c
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
- 000000018000aa80 also used for function at 00000001800078dc
- 000000018000aa80 also used for function at 0000000180007908
- 000000018000aabc (rva: 0000aabc): 0000000180007944 - 000000018000795b
+ 000000018000aa80 also used for function at 0000000180007b9c
+ 000000018000aa80 also used for function at 0000000180007bc8
+ 000000018000aabc (rva: 0000aabc): 0000000180007c04 - 0000000180007c1b
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000018000aab4 (rva: 0000aab4): 0000000180007980 - 00000001800079a0
+ 000000018000aab4 (rva: 0000aab4): 0000000180007c40 - 0000000180007c60
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x48
- 000000018000aa80 (rva: 0000aa80): 00000001800079a8 - 00000001800079dc
+ 000000018000aa80 (rva: 0000aa80): 0000000180007c68 - 0000000180007c9c
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
- 000000018000b594 (rva: 0000b594): 00000001800079dc - 0000000180007aae
+ 000000018000b604 (rva: 0000b604): 0000000180007c9c - 0000000180007d6e
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x09, Frame offset: 0x0, Frame reg: none
 	  pc+0x09: alloc small area: rsp = rsp - 0x38
- 000000018000b59c (rva: 0000b59c): 0000000180007ab0 - 0000000180007b21
+ 000000018000b60c (rva: 0000b60c): 0000000180007d70 - 0000000180007de1
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x40
 	  pc+0x04: push rdi
 	  pc+0x03: push rsi
 	  pc+0x02: push rbx
- 000000018000b5a8 (rva: 0000b5a8): 0000000180007b24 - 0000000180007bd0
+ 000000018000b618 (rva: 0000b618): 0000000180007de4 - 0000000180007e90
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0d, Frame offset: 0x0, Frame reg: none
 	  pc+0x0d: save rbx at rsp + 0x48
 	  pc+0x0d: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbp
- 000000018000aabc (rva: 0000aabc): 0000000180007bd0 - 0000000180007bf3
+ 000000018000aabc (rva: 0000aabc): 0000000180007e90 - 0000000180007eb3
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 000000018000aabc also used for function at 0000000180007c04
- 000000018000b5b4 (rva: 0000b5b4): 0000000180007c30 - 0000000180007d7b
+ 000000018000aabc also used for function at 0000000180007ec4
+ 000000018000b624 (rva: 0000b624): 0000000180007ef0 - 000000018000803b
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x15, Frame offset: 0x0, Frame reg: none
 	  pc+0x15: save rbx at rsp + 0x5d0
 	  pc+0x15: alloc large area: rsp = rsp - 0x5c0
 	  pc+0x06: push rbp
- 000000018000aaa8 (rva: 0000aaa8): 0000000180007d7c - 0000000180007db8
+ 000000018000aaa8 (rva: 0000aaa8): 000000018000803c - 0000000180008078
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save rbx at rsp + 0x30
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rdi
- 000000018000aaa8 also used for function at 0000000180007db8
- 000000018000b5c4 (rva: 0000b5c4): 0000000180007df4 - 0000000180007f95
+ 000000018000aaa8 also used for function at 0000000180008078
+ 000000018000b634 (rva: 0000b634): 00000001800080b4 - 0000000180008255
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0f, Frame offset: 0x0, Frame reg: none
 	  pc+0x0f: save rsi at rsp + 0x30
 	  pc+0x0f: save rbx at rsp + 0x28
 	  pc+0x0f: alloc small area: rsp = rsp - 0x10
 	  pc+0x0b: push rdi
 	User data:
 	  000: 00 00 00 00
- 000000018000b5d8 (rva: 0000b5d8): 0000000180008070 - 0000000180008072
+ 000000018000b648 (rva: 0000b648): 0000000180008330 - 0000000180008332
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 	User data:
 	  000: 00 00 00 00
- 000000018000b5e0 (rva: 0000b5e0): 0000000180008090 - 0000000180008096
+ 000000018000b650 (rva: 0000b650): 0000000180008350 - 0000000180008356
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 	User data:
 	  000: 00 00 00 00 00 00 00 00 50 31 00 00 00 00 00 00
-	  010: 08 b6 00 00 00 00 00 00 00 00 00 00 00 00 00 00
-	  020: 00 00 00 00 03 00 00 00 28 b6 00 00 50 b6 00 00
-	  030: 78 b6 00 00 00 00 00 00 00 00 00 00 00 00 00 00
+	  010: 78 b6 00 00 00 00 00 00 00 00 00 00 00 00 00 00
+	  020: 00 00 00 00 03 00 00 00 98 b6 00 00 c0 b6 00 00
+	  030: e8 b6 00 00 00 00 00 00 00 00 00 00 00 00 00 00
 	  040: 00 00 00 00 00 00 00 00 a0 e0 00 00 00 00 00 00
 	  050: ff ff ff ff 00 00 00 00 18 00 00 00 c0 2a 00 00
 	  060: 00 00 00 00 00 00 00 00 00 00 00 00 10 00 00 00
 	  070: d0 e0 00 00 00 00 00 00 ff ff ff ff 00 00 00 00
 	  080: 18 00 00 00 80 2a 00 00 00 00 00 00 00 00 00 00
 	  090: 00 00 00 00 00 00 00 00 f8 e0 00 00 00 00 00 00
 	  0a0: ff ff ff ff 00 00 00 00 18 00 00 00 a0 2b 00 00
 	  0b0: 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
 	  0c0: 20 e1 00 00 00 00 00 00 ff ff ff ff 00 00 00 00
 	  0d0: 18 00 00 00 e0 2b 00 00 00 00 00 00 00 00 00 00
 	  0e0: 00 00 00 00 00 00 00 00 50 31 00 00 00 00 00 00
-	  0f0: e8 b6 00 00 00 00 00 00 00 00 00 00 00 00 00 00
-	  100: 00 00 00 00 02 00 00 00 00 b7 00 00 78 b6 00 00
+	  0f0: 58 b7 00 00 00 00 00 00 00 00 00 00 00 00 00 00
+	  100: 00 00 00 00 02 00 00 00 70 b7 00 00 e8 b6 00 00
 	  110: 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
 	  120: 48 e1 00 00 00 00 00 00 ff ff ff ff 00 00 00 00
 	  130: 18 00 00 00 30 2b 00 00 00 00 00 00 00 00 00 00
 	  140: 00 00 00 00 00 00 00 00 50 31 00 00 00 00 00 00
-	  150: 48 b7 00 00 00 00 00 00 00 00 00 00 00 00 00 00
-	  160: 00 00 00 00 03 00 00 00 68 b7 00 00 a0 b6 00 00
-	  170: 78 b6 00 00 00 00 00 00 00 00 00 00 00 00 00 00
+	  150: b8 b7 00 00 00 00 00 00 00 00 00 00 00 00 00 00
+	  160: 00 00 00 00 03 00 00 00 d8 b7 00 00 10 b7 00 00
+	  170: e8 b6 00 00 00 00 00 00 00 00 00 00 00 00 00 00
 	  180: 00 00 00 00 00 00 00 00 70 e1 00 00 00 00 00 00
 	  190: ff ff ff ff 00 00 00 00 18 00 00 00 80 28 00 00
 	  1a0: 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
-	  1b0: 50 31 00 00 00 00 00 00 b0 b7 00 00 00 00 00 00
+	  1b0: 50 31 00 00 00 00 00 00 20 b8 00 00 00 00 00 00
 	  1c0: 00 00 00 00 00 00 00 00 00 00 00 00 02 00 00 00
-	  1d0: 50 b6 00 00 78 b6 00 00 00 00 00 00 00 00 00 00
+	  1d0: c0 b6 00 00 e8 b6 00 00 00 00 00 00 00 00 00 00
 	  1e0: 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
-	  1f0: ff ff ff ff 00 00 00 00 34 b8 00 00 01 00 00 00
-	  200: 06 00 00 00 06 00 00 00 f8 b7 00 00 10 b8 00 00
-	  210: 28 b8 00 00 10 10 00 00 40 10 00 00 f0 94 00 00
-	  220: e0 10 00 00 f0 10 00 00 90 56 00 00 52 b8 00 00
-	  230: 7d b8 00 00 a8 b8 00 00 d0 b8 00 00 07 b9 00 00
-	  240: 39 b9 00 00 00 00 01 00 02 00 03 00 04 00 05 00
+	  1f0: ff ff ff ff 00 00 00 00 a4 b8 00 00 01 00 00 00
+	  200: 06 00 00 00 06 00 00 00 68 b8 00 00 80 b8 00 00
+	  210: 98 b8 00 00 10 10 00 00 40 10 00 00 f0 94 00 00
+	  220: e0 10 00 00 f0 10 00 00 40 59 00 00 c2 b8 00 00
+	  230: ed b8 00 00 18 b9 00 00 40 b9 00 00 77 b9 00 00
+	  240: a9 b9 00 00 00 00 01 00 02 00 03 00 04 00 05 00
 	  250: 47 65 6f 64 65 2d 56 69 65 77 61 62 6c 65 73 5f
 	  260: 71 65 6d 5f 70 72 6f 78 79 2e 64 6c 6c 00 3f 3f
 	  270: 30 56 69 65 77 61 62 6c 65 73 51 45 4d 50 72 6f
 	  280: 78 79 4c 69 62 72 61 72 79 40 67 65 6f 64 65 40
 	  290: 40 51 45 41 41 40 58 5a 00 3f 3f 31 56 69 65 77
 	  2a0: 61 62 6c 65 73 51 45 4d 50 72 6f 78 79 4c 69 62
 	  2b0: 72 61 72 79 40 67 65 6f 64 65 40 40 55 45 41 41
@@ -1566,103 +1595,103 @@
 	  320: 58 5a 00 3f 69 6e 69 74 69 61 6c 69 7a 65 40 56
 	  330: 69 65 77 61 62 6c 65 73 51 45 4d 50 72 6f 78 79
 	  340: 4c 69 62 72 61 72 79 40 67 65 6f 64 65 40 40 53
 	  350: 41 58 58 5a 00 3f 73 69 6d 70 6c 69 66 79 40 67
 	  360: 65 6f 64 65 40 40 59 41 5f 4e 41 45 41 56 3f 24
 	  370: 54 72 69 61 6e 67 75 6c 61 74 65 64 53 75 72 66
 	  380: 61 63 65 40 24 30 32 40 31 40 40 5a 00 00 00 00
-	  390: a0 ba 00 00 00 00 00 00 00 00 00 00 80 c1 00 00
-	  3a0: 00 90 00 00 e0 bc 00 00 00 00 00 00 00 00 00 00
-	  3b0: 84 c6 00 00 40 92 00 00 c8 bc 00 00 00 00 00 00
-	  3c0: 00 00 00 00 c4 c7 00 00 28 92 00 00 78 bc 00 00
-	  3d0: 00 00 00 00 00 00 00 00 4c ca 00 00 d8 91 00 00
-	  3e0: e0 bd 00 00 00 00 00 00 00 00 00 00 fe ca 00 00
-	  3f0: 40 93 00 00 60 bb 00 00 00 00 00 00 00 00 00 00
-	  400: 34 d3 00 00 c0 90 00 00 d0 bd 00 00 00 00 00 00
-	  410: 00 00 00 00 66 d4 00 00 30 93 00 00 60 bd 00 00
-	  420: 00 00 00 00 00 00 00 00 7a d4 00 00 c0 92 00 00
-	  430: 40 be 00 00 00 00 00 00 00 00 00 00 5a d6 00 00
-	  440: a0 93 00 00 a8 be 00 00 00 00 00 00 00 00 00 00
-	  450: 7c d6 00 00 08 94 00 00 f8 bd 00 00 00 00 00 00
-	  460: 00 00 00 00 9c d6 00 00 58 93 00 00 30 be 00 00
-	  470: 00 00 00 00 00 00 00 00 c2 d6 00 00 90 93 00 00
-	  480: 10 be 00 00 00 00 00 00 00 00 00 00 e2 d6 00 00
-	  490: 70 93 00 00 e0 ba 00 00 00 00 00 00 00 00 00 00
-	  4a0: 68 d8 00 00 40 90 00 00 00 00 00 00 00 00 00 00
-	  4b0: 00 00 00 00 00 00 00 00 00 00 00 00 48 bf 00 00
-	  4c0: 00 00 00 00 be bf 00 00 00 00 00 00 f4 bf 00 00
-	  4d0: 00 00 00 00 3a c0 00 00 00 00 00 00 a6 c0 00 00
-	  4e0: 00 00 00 00 1e c1 00 00 00 00 00 00 10 bf 00 00
-	  4f0: 00 00 00 00 00 00 00 00 00 00 00 00 54 d8 00 00
-	  500: 00 00 00 00 38 d8 00 00 00 00 00 00 1e d8 00 00
-	  510: 00 00 00 00 08 d8 00 00 00 00 00 00 f2 d7 00 00
-	  520: 00 00 00 00 d8 d7 00 00 00 00 00 00 bc d7 00 00
-	  530: 00 00 00 00 a8 d7 00 00 00 00 00 00 94 d7 00 00
-	  540: 00 00 00 00 76 d7 00 00 00 00 00 00 5a d7 00 00
-	  550: 00 00 00 00 46 d7 00 00 00 00 00 00 2c d7 00 00
-	  560: 00 00 00 00 18 d7 00 00 00 00 00 00 02 d7 00 00
-	  570: 00 00 00 00 00 00 00 00 00 00 00 00 94 d2 00 00
-	  580: 00 00 00 00 58 d2 00 00 00 00 00 00 ec d1 00 00
-	  590: 00 00 00 00 a8 d1 00 00 00 00 00 00 66 d1 00 00
-	  5a0: 00 00 00 00 24 d1 00 00 00 00 00 00 e6 d0 00 00
-	  5b0: 00 00 00 00 b0 d0 00 00 00 00 00 00 70 d0 00 00
-	  5c0: 00 00 00 00 32 d0 00 00 00 00 00 00 fc cf 00 00
-	  5d0: 00 00 00 00 b4 cf 00 00 00 00 00 00 6c cf 00 00
-	  5e0: 00 00 00 00 1c cf 00 00 00 00 00 00 02 d3 00 00
-	  5f0: 00 00 00 00 bc d2 00 00 00 00 00 00 10 cb 00 00
-	  600: 00 00 00 00 2c cb 00 00 00 00 00 00 46 cb 00 00
-	  610: 00 00 00 00 68 cb 00 00 00 00 00 00 8a cb 00 00
-	  620: 00 00 00 00 a8 cb 00 00 00 00 00 00 dc cb 00 00
-	  630: 00 00 00 00 08 cc 00 00 00 00 00 00 5c cc 00 00
-	  640: 00 00 00 00 b0 cc 00 00 00 00 00 00 fc cc 00 00
-	  650: 00 00 00 00 4a cd 00 00 00 00 00 00 86 cd 00 00
-	  660: 00 00 00 00 c2 cd 00 00 00 00 00 00 0e ce 00 00
-	  670: 00 00 00 00 50 ce 00 00 00 00 00 00 98 ce 00 00
-	  680: 00 00 00 00 dc ce 00 00 00 00 00 00 00 00 00 00
-	  690: 00 00 00 00 dc c7 00 00 00 00 00 00 1a c8 00 00
-	  6a0: 00 00 00 00 52 c8 00 00 00 00 00 00 d8 c9 00 00
-	  6b0: 00 00 00 00 62 c9 00 00 00 00 00 00 1a c9 00 00
-	  6c0: 00 00 00 00 b8 c8 00 00 00 00 00 00 8a c8 00 00
-	  6d0: 00 00 00 00 6e c8 00 00 00 00 00 00 00 00 00 00
-	  6e0: 00 00 00 00 32 c7 00 00 00 00 00 00 98 c6 00 00
-	  6f0: 00 00 00 00 00 00 00 00 00 00 00 00 a2 c5 00 00
-	  700: 00 00 00 00 4e c4 00 00 00 00 00 00 3a c6 00 00
-	  710: 00 00 00 00 3e c5 00 00 00 00 00 00 b6 c3 00 00
-	  720: 00 00 00 00 70 c3 00 00 00 00 00 00 40 c3 00 00
-	  730: 00 00 00 00 ee c2 00 00 00 00 00 00 16 c2 00 00
-	  740: 00 00 00 00 ca c1 00 00 00 00 00 00 a2 c1 00 00
-	  750: 00 00 00 00 b2 c4 00 00 00 00 00 00 0c c6 00 00
-	  760: 00 00 00 00 f4 c4 00 00 00 00 00 00 80 c4 00 00
-	  770: 00 00 00 00 00 00 00 00 00 00 00 00 2e d4 00 00
-	  780: 00 00 00 00 46 d4 00 00 00 00 00 00 f0 d3 00 00
-	  790: 00 00 00 00 dc d3 00 00 00 00 00 00 c6 d3 00 00
-	  7a0: 00 00 00 00 ae d3 00 00 00 00 00 00 94 d3 00 00
-	  7b0: 00 00 00 00 7c d3 00 00 00 00 00 00 6a d3 00 00
-	  7c0: 00 00 00 00 58 d3 00 00 00 00 00 00 10 d4 00 00
-	  7d0: 00 00 00 00 fa d3 00 00 00 00 00 00 e6 d3 00 00
-	  7e0: 00 00 00 00 00 00 00 00 00 00 00 00 42 d3 00 00
-	  7f0: 00 00 00 00 00 00 00 00 00 00 00 00 98 ca 00 00
-	  800: 00 00 00 00 60 ca 00 00 00 00 00 00 00 00 00 00
-	  810: 00 00 00 00 3a d5 00 00 00 00 00 00 48 d5 00 00
-	  820: 00 00 00 00 00 00 00 00 00 00 00 00 6c d5 00 00
-	  830: 00 00 00 00 78 d5 00 00 00 00 00 00 52 d6 00 00
-	  840: 00 00 00 00 00 00 00 00 00 00 00 00 58 d5 00 00
-	  850: 00 00 00 00 00 00 00 00 00 00 00 00 3a d6 00 00
-	  860: 00 00 00 00 48 d6 00 00 00 00 00 00 06 d6 00 00
-	  870: 00 00 00 00 8c d4 00 00 00 00 00 00 82 d5 00 00
-	  880: 00 00 00 00 ae d5 00 00 00 00 00 00 22 d6 00 00
-	  890: 00 00 00 00 c8 d5 00 00 00 00 00 00 9c d5 00 00
-	  8a0: 00 00 00 00 ea d5 00 00 00 00 00 00 8e d5 00 00
-	  8b0: 00 00 00 00 60 d5 00 00 00 00 00 00 00 00 00 00
-	  8c0: 00 00 00 00 26 d5 00 00 00 00 00 00 1c d5 00 00
-	  8d0: 00 00 00 00 10 d5 00 00 00 00 00 00 06 d5 00 00
-	  8e0: 00 00 00 00 fe d4 00 00 00 00 00 00 30 d5 00 00
-	  8f0: 00 00 00 00 ec d4 00 00 00 00 00 00 e4 d4 00 00
-	  900: 00 00 00 00 da d4 00 00 00 00 00 00 d0 d4 00 00
-	  910: 00 00 00 00 b2 d4 00 00 00 00 00 00 f6 d4 00 00
+	  390: 10 bb 00 00 00 00 00 00 00 00 00 00 f0 c1 00 00
+	  3a0: 00 90 00 00 50 bd 00 00 00 00 00 00 00 00 00 00
+	  3b0: f4 c6 00 00 40 92 00 00 38 bd 00 00 00 00 00 00
+	  3c0: 00 00 00 00 34 c8 00 00 28 92 00 00 e8 bc 00 00
+	  3d0: 00 00 00 00 00 00 00 00 bc ca 00 00 d8 91 00 00
+	  3e0: 50 be 00 00 00 00 00 00 00 00 00 00 6e cb 00 00
+	  3f0: 40 93 00 00 d0 bb 00 00 00 00 00 00 00 00 00 00
+	  400: a4 d3 00 00 c0 90 00 00 40 be 00 00 00 00 00 00
+	  410: 00 00 00 00 d6 d4 00 00 30 93 00 00 d0 bd 00 00
+	  420: 00 00 00 00 00 00 00 00 ea d4 00 00 c0 92 00 00
+	  430: b0 be 00 00 00 00 00 00 00 00 00 00 ca d6 00 00
+	  440: a0 93 00 00 18 bf 00 00 00 00 00 00 00 00 00 00
+	  450: ec d6 00 00 08 94 00 00 68 be 00 00 00 00 00 00
+	  460: 00 00 00 00 0c d7 00 00 58 93 00 00 a0 be 00 00
+	  470: 00 00 00 00 00 00 00 00 32 d7 00 00 90 93 00 00
+	  480: 80 be 00 00 00 00 00 00 00 00 00 00 52 d7 00 00
+	  490: 70 93 00 00 50 bb 00 00 00 00 00 00 00 00 00 00
+	  4a0: d8 d8 00 00 40 90 00 00 00 00 00 00 00 00 00 00
+	  4b0: 00 00 00 00 00 00 00 00 00 00 00 00 b8 bf 00 00
+	  4c0: 00 00 00 00 2e c0 00 00 00 00 00 00 64 c0 00 00
+	  4d0: 00 00 00 00 aa c0 00 00 00 00 00 00 16 c1 00 00
+	  4e0: 00 00 00 00 8e c1 00 00 00 00 00 00 80 bf 00 00
+	  4f0: 00 00 00 00 00 00 00 00 00 00 00 00 c4 d8 00 00
+	  500: 00 00 00 00 a8 d8 00 00 00 00 00 00 8e d8 00 00
+	  510: 00 00 00 00 78 d8 00 00 00 00 00 00 62 d8 00 00
+	  520: 00 00 00 00 48 d8 00 00 00 00 00 00 2c d8 00 00
+	  530: 00 00 00 00 18 d8 00 00 00 00 00 00 04 d8 00 00
+	  540: 00 00 00 00 e6 d7 00 00 00 00 00 00 ca d7 00 00
+	  550: 00 00 00 00 b6 d7 00 00 00 00 00 00 9c d7 00 00
+	  560: 00 00 00 00 88 d7 00 00 00 00 00 00 72 d7 00 00
+	  570: 00 00 00 00 00 00 00 00 00 00 00 00 04 d3 00 00
+	  580: 00 00 00 00 c8 d2 00 00 00 00 00 00 5c d2 00 00
+	  590: 00 00 00 00 18 d2 00 00 00 00 00 00 d6 d1 00 00
+	  5a0: 00 00 00 00 94 d1 00 00 00 00 00 00 56 d1 00 00
+	  5b0: 00 00 00 00 20 d1 00 00 00 00 00 00 e0 d0 00 00
+	  5c0: 00 00 00 00 a2 d0 00 00 00 00 00 00 6c d0 00 00
+	  5d0: 00 00 00 00 24 d0 00 00 00 00 00 00 dc cf 00 00
+	  5e0: 00 00 00 00 8c cf 00 00 00 00 00 00 72 d3 00 00
+	  5f0: 00 00 00 00 2c d3 00 00 00 00 00 00 80 cb 00 00
+	  600: 00 00 00 00 9c cb 00 00 00 00 00 00 b6 cb 00 00
+	  610: 00 00 00 00 d8 cb 00 00 00 00 00 00 fa cb 00 00
+	  620: 00 00 00 00 18 cc 00 00 00 00 00 00 4c cc 00 00
+	  630: 00 00 00 00 78 cc 00 00 00 00 00 00 cc cc 00 00
+	  640: 00 00 00 00 20 cd 00 00 00 00 00 00 6c cd 00 00
+	  650: 00 00 00 00 ba cd 00 00 00 00 00 00 f6 cd 00 00
+	  660: 00 00 00 00 32 ce 00 00 00 00 00 00 7e ce 00 00
+	  670: 00 00 00 00 c0 ce 00 00 00 00 00 00 08 cf 00 00
+	  680: 00 00 00 00 4c cf 00 00 00 00 00 00 00 00 00 00
+	  690: 00 00 00 00 4c c8 00 00 00 00 00 00 8a c8 00 00
+	  6a0: 00 00 00 00 c2 c8 00 00 00 00 00 00 48 ca 00 00
+	  6b0: 00 00 00 00 d2 c9 00 00 00 00 00 00 8a c9 00 00
+	  6c0: 00 00 00 00 28 c9 00 00 00 00 00 00 fa c8 00 00
+	  6d0: 00 00 00 00 de c8 00 00 00 00 00 00 00 00 00 00
+	  6e0: 00 00 00 00 a2 c7 00 00 00 00 00 00 08 c7 00 00
+	  6f0: 00 00 00 00 00 00 00 00 00 00 00 00 12 c6 00 00
+	  700: 00 00 00 00 be c4 00 00 00 00 00 00 aa c6 00 00
+	  710: 00 00 00 00 ae c5 00 00 00 00 00 00 26 c4 00 00
+	  720: 00 00 00 00 e0 c3 00 00 00 00 00 00 b0 c3 00 00
+	  730: 00 00 00 00 5e c3 00 00 00 00 00 00 86 c2 00 00
+	  740: 00 00 00 00 3a c2 00 00 00 00 00 00 12 c2 00 00
+	  750: 00 00 00 00 22 c5 00 00 00 00 00 00 7c c6 00 00
+	  760: 00 00 00 00 64 c5 00 00 00 00 00 00 f0 c4 00 00
+	  770: 00 00 00 00 00 00 00 00 00 00 00 00 9e d4 00 00
+	  780: 00 00 00 00 b6 d4 00 00 00 00 00 00 60 d4 00 00
+	  790: 00 00 00 00 4c d4 00 00 00 00 00 00 36 d4 00 00
+	  7a0: 00 00 00 00 1e d4 00 00 00 00 00 00 04 d4 00 00
+	  7b0: 00 00 00 00 ec d3 00 00 00 00 00 00 da d3 00 00
+	  7c0: 00 00 00 00 c8 d3 00 00 00 00 00 00 80 d4 00 00
+	  7d0: 00 00 00 00 6a d4 00 00 00 00 00 00 56 d4 00 00
+	  7e0: 00 00 00 00 00 00 00 00 00 00 00 00 b2 d3 00 00
+	  7f0: 00 00 00 00 00 00 00 00 00 00 00 00 08 cb 00 00
+	  800: 00 00 00 00 d0 ca 00 00 00 00 00 00 00 00 00 00
+	  810: 00 00 00 00 aa d5 00 00 00 00 00 00 b8 d5 00 00
+	  820: 00 00 00 00 00 00 00 00 00 00 00 00 dc d5 00 00
+	  830: 00 00 00 00 e8 d5 00 00 00 00 00 00 c2 d6 00 00
+	  840: 00 00 00 00 00 00 00 00 00 00 00 00 c8 d5 00 00
+	  850: 00 00 00 00 00 00 00 00 00 00 00 00 aa d6 00 00
+	  860: 00 00 00 00 b8 d6 00 00 00 00 00 00 76 d6 00 00
+	  870: 00 00 00 00 fc d4 00 00 00 00 00 00 f2 d5 00 00
+	  880: 00 00 00 00 1e d6 00 00 00 00 00 00 92 d6 00 00
+	  890: 00 00 00 00 38 d6 00 00 00 00 00 00 0c d6 00 00
+	  8a0: 00 00 00 00 5a d6 00 00 00 00 00 00 fe d5 00 00
+	  8b0: 00 00 00 00 d0 d5 00 00 00 00 00 00 00 00 00 00
+	  8c0: 00 00 00 00 96 d5 00 00 00 00 00 00 8c d5 00 00
+	  8d0: 00 00 00 00 80 d5 00 00 00 00 00 00 76 d5 00 00
+	  8e0: 00 00 00 00 6e d5 00 00 00 00 00 00 a0 d5 00 00
+	  8f0: 00 00 00 00 5c d5 00 00 00 00 00 00 54 d5 00 00
+	  900: 00 00 00 00 4a d5 00 00 00 00 00 00 40 d5 00 00
+	  910: 00 00 00 00 22 d5 00 00 00 00 00 00 66 d5 00 00
 	  920: 00 00 00 00 00 00 00 00 00 00 00 00 3c 00 3f 69
 	  930: 6e 69 74 69 61 6c 69 7a 65 40 43 6f 6d 6d 6f 6e
 	  940: 4d 6f 64 69 66 69 65 72 53 75 72 66 61 63 65 4c
 	  950: 69 62 72 61 72 79 40 67 65 6f 64 65 40 40 53 41
 	  960: 58 58 5a 00 27 00 3f 3f 30 3f 24 54 72 69 61 6e
 	  970: 67 75 6c 61 74 65 64 53 75 72 66 61 63 65 4d 6f
 	  980: 64 69 66 69 65 72 40 24 30 32 40 67 65 6f 64 65
@@ -1696,95 +1725,95 @@
 	  b40: 73 5f 63 6f 6c 6c 61 70 73 65 5f 65 64 67 65 5f
 	  b50: 76 61 6c 69 64 40 24 30 32 40 67 65 6f 64 65 40
 	  b60: 40 59 41 5f 4e 41 45 42 56 3f 24 54 72 69 61 6e
 	  b70: 67 75 6c 61 74 65 64 53 75 72 66 61 63 65 40 24
 	  b80: 30 32 40 30 40 49 41 45 42 56 3f 24 50 6f 69 6e
 	  b90: 74 40 24 30 32 40 30 40 40 5a 00 00 47 65 6f 64
 	  ba0: 65 2d 43 6f 6d 6d 6f 6e 5f 6d 6f 64 69 66 69 65
-	  bb0: 72 5f 73 75 72 66 61 63 65 2e 64 6c 6c 00 32 06
+	  bb0: 72 5f 73 75 72 66 61 63 65 2e 64 6c 6c 00 5e 06
 	  bc0: 3f 6e 62 5f 76 65 72 74 69 63 65 73 40 56 65 72
 	  bd0: 74 65 78 53 65 74 40 67 65 6f 64 65 40 40 51 45
-	  be0: 42 41 49 58 5a 00 b9 07 3f 76 65 72 74 65 78 5f
+	  be0: 42 41 49 58 5a 00 e5 07 3f 76 65 72 74 65 78 5f
 	  bf0: 61 74 74 72 69 62 75 74 65 5f 6d 61 6e 61 67 65
 	  c00: 72 40 56 65 72 74 65 78 53 65 74 40 67 65 6f 64
 	  c10: 65 40 40 51 45 42 41 41 45 41 56 41 74 74 72 69
 	  c20: 62 75 74 65 4d 61 6e 61 67 65 72 40 32 40 58 5a
-	  c30: 00 00 b2 03 3f 63 72 65 61 74 65 40 3f 24 54 72
+	  c30: 00 00 de 03 3f 63 72 65 61 74 65 40 3f 24 54 72
 	  c40: 69 61 6e 67 75 6c 61 74 65 64 53 75 72 66 61 63
 	  c50: 65 42 75 69 6c 64 65 72 40 24 30 32 40 67 65 6f
 	  c60: 64 65 40 40 53 41 3f 41 56 3f 24 75 6e 69 71 75
 	  c70: 65 5f 70 74 72 40 56 3f 24 54 72 69 61 6e 67 75
 	  c80: 6c 61 74 65 64 53 75 72 66 61 63 65 42 75 69 6c
 	  c90: 64 65 72 40 24 30 32 40 67 65 6f 64 65 40 40 55
 	  ca0: 3f 24 64 65 66 61 75 6c 74 5f 64 65 6c 65 74 65
 	  cb0: 40 56 3f 24 54 72 69 61 6e 67 75 6c 61 74 65 64
 	  cc0: 53 75 72 66 61 63 65 42 75 69 6c 64 65 72 40 24
 	  cd0: 30 32 40 67 65 6f 64 65 40 40 40 73 74 64 40 40
 	  ce0: 40 73 74 64 40 40 41 45 41 56 3f 24 54 72 69 61
 	  cf0: 6e 67 75 6c 61 74 65 64 53 75 72 66 61 63 65 40
-	  d00: 24 30 32 40 32 40 40 5a 00 00 57 06 3f 70 6f 69
+	  d00: 24 30 32 40 32 40 40 5a 00 00 83 06 3f 70 6f 69
 	  d10: 6e 74 40 3f 24 43 6f 6f 72 64 69 6e 61 74 65 52
 	  d20: 65 66 65 72 65 6e 63 65 53 79 73 74 65 6d 4d 61
 	  d30: 6e 61 67 65 72 73 40 24 30 32 40 67 65 6f 64 65
 	  d40: 40 40 51 45 42 41 41 45 42 56 3f 24 50 6f 69 6e
-	  d50: 74 40 24 30 32 40 32 40 49 40 5a 00 27 06 3f 6e
+	  d50: 74 40 24 30 32 40 32 40 49 40 5a 00 53 06 3f 6e
 	  d60: 62 5f 70 6f 6c 79 67 6f 6e 73 40 3f 24 53 75 72
 	  d70: 66 61 63 65 4d 65 73 68 40 24 30 32 40 67 65 6f
-	  d80: 64 65 40 40 51 45 42 41 49 58 5a 00 0d 05 3f 65
+	  d80: 64 65 40 40 51 45 42 41 49 58 5a 00 39 05 3f 65
 	  d90: 64 67 65 5f 6c 65 6e 67 74 68 40 3f 24 53 75 72
 	  da0: 66 61 63 65 4d 65 73 68 40 24 30 32 40 67 65 6f
 	  db0: 64 65 40 40 51 45 42 41 4e 41 45 42 56 3f 24 61
 	  dc0: 72 72 61 79 40 49 24 30 31 40 73 74 64 40 40 40
-	  dd0: 5a 00 77 06 3f 70 6f 6c 79 67 6f 6e 73 5f 61 72
+	  dd0: 5a 00 a3 06 3f 70 6f 6c 79 67 6f 6e 73 5f 61 72
 	  de0: 6f 75 6e 64 5f 76 65 72 74 65 78 40 3f 24 53 75
 	  df0: 72 66 61 63 65 4d 65 73 68 40 24 30 32 40 67 65
 	  e00: 6f 64 65 40 40 51 45 42 41 41 45 42 56 3f 24 49
 	  e10: 6e 6c 69 6e 65 64 56 65 63 74 6f 72 40 55 50 6f
 	  e20: 6c 79 67 6f 6e 56 65 72 74 65 78 40 67 65 6f 64
 	  e30: 65 40 40 24 30 39 56 3f 24 61 6c 6c 6f 63 61 74
 	  e40: 6f 72 40 55 50 6f 6c 79 67 6f 6e 56 65 72 74 65
 	  e50: 78 40 67 65 6f 64 65 40 40 40 73 74 64 40 40 40
-	  e60: 61 62 73 6c 40 40 49 40 5a 00 22 05 3f 65 6e 61
+	  e60: 61 62 73 6c 40 40 49 40 5a 00 4e 05 3f 65 6e 61
 	  e70: 62 6c 65 5f 65 64 67 65 73 40 3f 24 53 75 72 66
 	  e80: 61 63 65 4d 65 73 68 40 24 30 32 40 67 65 6f 64
-	  e90: 65 40 40 51 45 42 41 58 58 5a 00 00 41 04 3f 64
+	  e90: 65 40 40 51 45 42 41 58 58 5a 00 00 6d 04 3f 64
 	  ea0: 69 73 61 62 6c 65 5f 65 64 67 65 73 40 3f 24 53
 	  eb0: 75 72 66 61 63 65 4d 65 73 68 40 24 30 32 40 67
-	  ec0: 65 6f 64 65 40 40 51 45 42 41 58 58 5a 00 1b 05
+	  ec0: 65 6f 64 65 40 40 51 45 42 41 58 58 5a 00 47 05
 	  ed0: 3f 65 64 67 65 73 40 3f 24 53 75 72 66 61 63 65
 	  ee0: 4d 65 73 68 40 24 30 32 40 67 65 6f 64 65 40 40
 	  ef0: 51 45 42 41 41 45 42 56 3f 24 53 75 72 66 61 63
 	  f00: 65 45 64 67 65 73 40 24 30 32 40 32 40 58 5a 00
-	  f10: 4a 07 3f 74 72 69 61 6e 67 6c 65 40 3f 24 54 72
+	  f10: 76 07 3f 74 72 69 61 6e 67 6c 65 40 3f 24 54 72
 	  f20: 69 61 6e 67 75 6c 61 74 65 64 53 75 72 66 61 63
 	  f30: 65 40 24 30 32 40 67 65 6f 64 65 40 40 51 45 42
 	  f40: 41 3f 41 56 3f 24 54 72 69 61 6e 67 6c 65 40 24
-	  f50: 30 32 40 32 40 49 40 5a 00 00 4a 00 3f 3f 24 73
+	  f50: 30 32 40 32 40 49 40 5a 00 00 51 00 3f 3f 24 73
 	  f60: 61 76 65 5f 74 72 69 61 6e 67 75 6c 61 74 65 64
 	  f70: 5f 73 75 72 66 61 63 65 40 24 30 32 40 67 65 6f
 	  f80: 64 65 40 40 59 41 58 41 45 42 56 3f 24 54 72 69
 	  f90: 61 6e 67 75 6c 61 74 65 64 53 75 72 66 61 63 65
 	  fa0: 40 24 30 32 40 30 40 56 73 74 72 69 6e 67 5f 76
-	  fb0: 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00 35 00
+	  fb0: 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00 3c 00
 	  fc0: 3f 3f 24 70 6f 6c 79 67 6f 6e 5f 76 65 72 74 65
 	  fd0: 78 5f 6e 6f 72 6d 61 6c 40 24 30 32 40 3f 24 53
 	  fe0: 75 72 66 61 63 65 4d 65 73 68 40 24 30 32 40 67
 	  ff0: 65 6f 64 65 40 40 51 45 42 41 3f 41 56 3f 24 6f
 	  1000: 70 74 69 6f 6e 61 6c 40 56 3f 24 56 65 63 74 6f
 	  1010: 72 40 24 30 32 40 67 65 6f 64 65 40 40 40 61 62
-	  1020: 73 6c 40 40 49 40 5a 00 1a 06 3f 6e 62 5f 65 64
+	  1020: 73 6c 40 40 49 40 5a 00 46 06 3f 6e 62 5f 65 64
 	  1030: 67 65 73 40 3f 24 53 75 72 66 61 63 65 45 64 67
 	  1040: 65 73 40 24 30 32 40 67 65 6f 64 65 40 40 51 45
-	  1050: 42 41 49 58 5a 00 13 05 3f 65 64 67 65 5f 76 65
+	  1050: 42 41 49 58 5a 00 3f 05 3f 65 64 67 65 5f 76 65
 	  1060: 72 74 69 63 65 73 40 3f 24 53 75 72 66 61 63 65
 	  1070: 45 64 67 65 73 40 24 30 32 40 67 65 6f 64 65 40
 	  1080: 40 51 45 42 41 41 45 42 56 3f 24 61 72 72 61 79
 	  1090: 40 49 24 30 31 40 73 74 64 40 40 49 40 5a 00 00
 	  10a0: 4f 70 65 6e 47 65 6f 64 65 5f 6d 65 73 68 2e 64
-	  10b0: 6c 6c 00 00 72 02 3f 73 65 74 5f 70 6f 69 6e 74
+	  10b0: 6c 6c 00 00 ad 02 3f 73 65 74 5f 70 6f 69 6e 74
 	  10c0: 40 3f 24 47 65 6e 65 72 69 63 54 72 69 61 6e 67
 	  10d0: 6c 65 40 56 3f 24 72 65 66 65 72 65 6e 63 65 5f
 	  10e0: 77 72 61 70 70 65 72 40 24 24 43 42 56 3f 24 50
 	  10f0: 6f 69 6e 74 40 24 30 32 40 67 65 6f 64 65 40 40
 	  1100: 40 73 74 64 40 40 24 30 32 40 67 65 6f 64 65 40
 	  1110: 40 51 45 41 41 58 49 56 3f 24 72 65 66 65 72 65
 	  1120: 6e 63 65 5f 77 72 61 70 70 65 72 40 24 24 43 42
@@ -1796,47 +1825,47 @@
 	  1180: 70 70 65 72 40 24 24 43 42 56 3f 24 50 6f 69 6e
 	  1190: 74 40 24 30 32 40 67 65 6f 64 65 40 40 40 73 74
 	  11a0: 64 40 40 24 30 32 40 67 65 6f 64 65 40 40 51 45
 	  11b0: 42 41 3f 41 56 3f 24 6f 70 74 69 6f 6e 61 6c 40
 	  11c0: 56 3f 24 56 65 63 74 6f 72 40 24 30 32 40 67 65
 	  11d0: 6f 64 65 40 40 40 61 62 73 6c 40 40 58 5a 00 00
 	  11e0: 4f 70 65 6e 47 65 6f 64 65 5f 67 65 6f 6d 65 74
-	  11f0: 72 79 2e 64 6c 6c 00 00 c0 00 3f 73 65 74 5f 69
+	  11f0: 72 79 2e 64 6c 6c 00 00 c7 00 3f 73 65 74 5f 69
 	  1200: 6e 73 74 61 6e 63 65 40 53 69 6e 67 6c 65 74 6f
 	  1210: 6e 40 67 65 6f 64 65 40 40 43 41 58 41 45 42 56
 	  1220: 74 79 70 65 5f 69 6e 66 6f 40 40 50 45 41 56 31
-	  1230: 32 40 40 5a 00 00 8c 00 3f 69 6e 73 74 61 6e 63
+	  1230: 32 40 40 5a 00 00 8f 00 3f 69 6e 73 74 61 6e 63
 	  1240: 65 40 53 69 6e 67 6c 65 74 6f 6e 40 67 65 6f 64
 	  1250: 65 40 40 43 41 50 45 41 56 31 32 40 41 45 42 56
 	  1260: 74 79 70 65 5f 69 6e 66 6f 40 40 40 5a 00 31 00
 	  1270: 3f 3f 31 4c 69 62 72 61 72 79 40 67 65 6f 64 65
 	  1280: 40 40 55 45 41 41 40 58 5a 00 1a 00 3f 3f 30 4c
 	  1290: 69 62 72 61 72 79 40 67 65 6f 64 65 40 40 49 45
-	  12a0: 41 41 40 58 5a 00 59 00 3f 63 61 6c 6c 5f 69 6e
+	  12a0: 41 41 40 58 5a 00 5b 00 3f 63 61 6c 6c 5f 69 6e
 	  12b0: 69 74 69 61 6c 69 7a 65 40 4c 69 62 72 61 72 79
 	  12c0: 40 67 65 6f 64 65 40 40 49 45 41 41 58 50 45 42
-	  12d0: 44 40 5a 00 95 00 3f 6c 6f 67 5f 64 65 62 75 67
+	  12d0: 44 40 5a 00 98 00 3f 6c 6f 67 5f 64 65 62 75 67
 	  12e0: 40 4c 6f 67 67 65 72 40 67 65 6f 64 65 40 40 43
 	  12f0: 41 58 41 45 42 56 3f 24 62 61 73 69 63 5f 73 74
 	  1300: 72 69 6e 67 40 44 55 3f 24 63 68 61 72 5f 74 72
 	  1310: 61 69 74 73 40 44 40 73 74 64 40 40 56 3f 24 61
 	  1320: 6c 6c 6f 63 61 74 6f 72 40 44 40 32 40 40 73 74
-	  1330: 64 40 40 40 5a 00 66 00 3f 64 65 6c 65 74 65 5f
+	  1330: 64 40 40 40 5a 00 68 00 3f 64 65 6c 65 74 65 5f
 	  1340: 61 74 74 72 69 62 75 74 65 40 41 74 74 72 69 62
 	  1350: 75 74 65 4d 61 6e 61 67 65 72 40 67 65 6f 64 65
 	  1360: 40 40 51 45 41 41 58 56 73 74 72 69 6e 67 5f 76
-	  1370: 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00 79 00
+	  1370: 69 65 77 40 61 62 73 6c 40 40 40 5a 00 00 7b 00
 	  1380: 3f 66 69 6e 64 5f 61 74 74 72 69 62 75 74 65 5f
 	  1390: 62 61 73 65 40 41 74 74 72 69 62 75 74 65 4d 61
 	  13a0: 6e 61 67 65 72 40 67 65 6f 64 65 40 40 41 45 42
 	  13b0: 41 3f 41 56 3f 24 73 68 61 72 65 64 5f 70 74 72
 	  13c0: 40 56 41 74 74 72 69 62 75 74 65 42 61 73 65 40
 	  13d0: 67 65 6f 64 65 40 40 40 73 74 64 40 40 56 73 74
 	  13e0: 72 69 6e 67 5f 76 69 65 77 40 61 62 73 6c 40 40
-	  13f0: 40 5a 00 00 b0 00 3f 72 65 67 69 73 74 65 72 5f
+	  13f0: 40 5a 00 00 b3 00 3f 72 65 67 69 73 74 65 72 5f
 	  1400: 61 74 74 72 69 62 75 74 65 40 41 74 74 72 69 62
 	  1410: 75 74 65 4d 61 6e 61 67 65 72 40 67 65 6f 64 65
 	  1420: 40 40 41 45 41 41 58 56 3f 24 73 68 61 72 65 64
 	  1430: 5f 70 74 72 40 56 41 74 74 72 69 62 75 74 65 42
 	  1440: 61 73 65 40 67 65 6f 64 65 40 40 40 73 74 64 40
 	  1450: 40 56 73 74 72 69 6e 67 5f 76 69 65 77 40 61 62
 	  1460: 73 6c 40 40 40 5a 00 00 4f 70 65 6e 47 65 6f 64
@@ -2063,81 +2092,82 @@
 	  2230: 54 68 72 65 61 64 49 64 00 00 0a 03 47 65 74 53
 	  2240: 79 73 74 65 6d 54 69 6d 65 41 73 46 69 6c 65 54
 	  2250: 69 6d 65 00 34 01 44 69 73 61 62 6c 65 54 68 72
 	  2260: 65 61 64 4c 69 62 72 61 72 79 43 61 6c 6c 73 00
 	  2270: a0 03 49 73 44 65 62 75 67 67 65 72 50 72 65 73
 	  2280: 65 6e 74 00 4b 45 52 4e 45 4c 33 32 2e 64 6c 6c
 	  2290: 00 00
- 000000018000aa78 (rva: 0000aa78): 00000001800080a0 - 00000001800080bd
+ 000000018000aa78 (rva: 0000aa78): 0000000180008360 - 000000018000837d
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbp
- 000000018000ad94 (rva: 0000ad94): 00000001800080e0 - 000000018000811b
+ 000000018000ad94 (rva: 0000ad94): 00000001800083a0 - 00000001800083db
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbp
- 000000018000ad94 also used for function at 0000000180008120
- 000000018000ad94 also used for function at 0000000180008140
- 000000018000ad94 also used for function at 0000000180008170
- 000000018000ad94 also used for function at 00000001800081a0
- 000000018000ad94 also used for function at 00000001800081d0
- 000000018000aa78 (rva: 0000aa78): 0000000180008210 - 0000000180008239
+ 000000018000ad94 also used for function at 00000001800083e0
+ 000000018000ad94 also used for function at 0000000180008400
+ 000000018000ad94 also used for function at 0000000180008430
+ 000000018000ad94 also used for function at 0000000180008460
+ 000000018000ad94 also used for function at 0000000180008490
+ 000000018000aa78 (rva: 0000aa78): 00000001800084d0 - 00000001800084f9
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbp
- 000000018000aa78 also used for function at 0000000180008240
- 000000018000ad94 (rva: 0000ad94): 0000000180008310 - 0000000180008340
+ 000000018000aa78 also used for function at 0000000180008500
+ 000000018000ad94 (rva: 0000ad94): 00000001800085d0 - 0000000180008600
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbp
- 000000018000aa78 (rva: 0000aa78): 0000000180008340 - 000000018000835d
+ 000000018000aa78 (rva: 0000aa78): 0000000180008600 - 000000018000861d
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbp
- 000000018000ad94 (rva: 0000ad94): 00000001800083d0 - 0000000180008402
+ 000000018000ad94 (rva: 0000ad94): 0000000180008690 - 00000001800086c2
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbp
- 000000018000aa78 (rva: 0000aa78): 0000000180008410 - 0000000180008430
+ 000000018000aa78 (rva: 0000aa78): 00000001800086d0 - 00000001800086ed
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbp
- 000000018000aa78 also used for function at 0000000180008470
- 000000018000aa78 also used for function at 00000001800084d0
- 000000018000aa78 also used for function at 000000018000856c
- 000000018000b478 (rva: 0000b478): 0000000180008598 - 00000001800085f7
+ 000000018000aa78 also used for function at 0000000180008730
+ 000000018000aa78 also used for function at 0000000180008790
+ 000000018000aa78 also used for function at 00000001800087f0
+ 000000018000aa78 also used for function at 000000018000888c
+ 000000018000b4ec (rva: 0000b4ec): 00000001800088b8 - 0000000180008917
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x28
 	  pc+0x03: push rbp
 	  pc+0x02: push rbx
- 000000018000aa78 (rva: 0000aa78): 00000001800085f7 - 000000018000860e
+ 000000018000aa78 (rva: 0000aa78): 0000000180008917 - 000000018000892e
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbp
- 000000018000aa78 also used for function at 000000018000860e
- 000000018000aa78 also used for function at 0000000180008627
- 000000018000b564 (rva: 0000b564): 000000018000863b - 0000000180008671
+ 000000018000aa78 also used for function at 000000018000892e
+ 000000018000aa78 also used for function at 0000000180008947
+ 000000018000b5d4 (rva: 0000b5d4): 000000018000895b - 0000000180008991
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x30
 	  pc+0x02: push rbp
- 000000018000b58c (rva: 0000b58c): 0000000180008671 - 0000000180008689
+ 000000018000b5fc (rva: 0000b5fc): 0000000180008991 - 00000001800089a9
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x02, Frame offset: 0x0, Frame reg: none
 	  pc+0x02: push rbp
- 000000018000aa80 (rva: 0000aa80): 000000018000868c - 00000001800086e7
+ 000000018000aa80 (rva: 0000aa80): 00000001800089ac - 0000000180008a07
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x20
 	  pc+0x02: push rbx
 
 
 PE File Base Relocations (interpreted .reloc section contents)
@@ -2201,32 +2231,32 @@
 	reloc   55 offset  770 [9770] DIR64
 	reloc   56 offset  778 [9778] DIR64
 	reloc   57 offset  780 [9780] DIR64
 	reloc   58 offset  788 [9788] DIR64
 	reloc   59 offset  790 [9790] DIR64
 	reloc   60 offset  798 [9798] DIR64
 	reloc   61 offset  7a0 [97a0] DIR64
-	reloc   62 offset  838 [9838] DIR64
+	reloc   62 offset  7a8 [97a8] DIR64
 	reloc   63 offset  840 [9840] DIR64
 	reloc   64 offset  848 [9848] DIR64
 	reloc   65 offset  850 [9850] DIR64
 	reloc   66 offset  858 [9858] DIR64
-	reloc   67 offset  9a0 [99a0] DIR64
-	reloc   68 offset  9a8 [99a8] DIR64
-	reloc   69 offset  9e0 [99e0] DIR64
+	reloc   67 offset  860 [9860] DIR64
+	reloc   68 offset  9c0 [99c0] DIR64
+	reloc   69 offset  9c8 [99c8] DIR64
 	reloc   70 offset  9e8 [99e8] DIR64
-	reloc   71 offset  a68 [9a68] DIR64
-	reloc   72 offset  a80 [9a80] DIR64
-	reloc   73 offset  a88 [9a88] DIR64
-	reloc   74 offset  b10 [9b10] DIR64
-	reloc   75 offset  b28 [9b28] DIR64
-	reloc   76 offset  b30 [9b30] DIR64
-	reloc   77 offset  b38 [9b38] DIR64
-	reloc   78 offset  b40 [9b40] DIR64
-	reloc   79 offset    0 [9000] ABSOLUTE
+	reloc   71 offset  9f0 [99f0] DIR64
+	reloc   72 offset  a78 [9a78] DIR64
+	reloc   73 offset  a90 [9a90] DIR64
+	reloc   74 offset  a98 [9a98] DIR64
+	reloc   75 offset  b20 [9b20] DIR64
+	reloc   76 offset  b38 [9b38] DIR64
+	reloc   77 offset  b40 [9b40] DIR64
+	reloc   78 offset  b48 [9b48] DIR64
+	reloc   79 offset  b50 [9b50] DIR64
 
 Virtual Address: 0000e000 Chunk size 60 (0x3c) Number of fixups 26
 	reloc    0 offset   40 [e040] DIR64
 	reloc    1 offset   68 [e068] DIR64
 	reloc    2 offset   a0 [e0a0] DIR64
 	reloc    3 offset   d0 [e0d0] DIR64
 	reloc    4 offset   f8 [e0f8] DIR64
@@ -2248,53 +2278,53 @@
 	reloc   20 offset  4c0 [e4c0] DIR64
 	reloc   21 offset  508 [e508] DIR64
 	reloc   22 offset  540 [e540] DIR64
 	reloc   23 offset  5a0 [e5a0] DIR64
 	reloc   24 offset  610 [e610] DIR64
 	reloc   25 offset    0 [e000] ABSOLUTE
 
-There is a debug directory in .rdata at 0x1800099f0
+There is a debug directory in .rdata at 0x1800099f8
 
 Type                Size     Rva      Offset
- 13         CoffGrp 000002b8 0000a774 00009374
+ 13         CoffGrp 000002b8 0000a774 00009774
 
 The .rsrc Resource Directory section:
 000  Type Table: Char: 0, Time: 00000000, Ver: 4/0, Num Names: 0, IDs: 1
 010   Entry: ID: 0x000018, Value: 0x80000018
 018    Name Table: Char: 0, Time: 00000000, Ver: 4/0, Num Names: 0, IDs: 1
 028     Entry: ID: 0x000002, Value: 0x80000030
 030      Language Table: Char: 0, Time: 00000000, Ver: 4/0, Num Names: 0, IDs: 1
 040       Entry: ID: 0x000409, Value: 0x000048
 048        Leaf: Addr: 0x010058, Size: 0x00015a, Codepage: 1252
  Resources start at offset: 0x58
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
-  0 .text         000076e7  0000000180001000  0000000180001000  00000400  2**4
+  0 .text         00007a07  0000000180001000  0000000180001000  00000400  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE
-  1 .rdata        00004876  0000000180009000  0000000180009000  00007c00  2**4
+  1 .rdata        000048e6  0000000180009000  0000000180009000  00008000  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  2 .data         00000800  000000018000e000  000000018000e000  0000c600  2**4
+  2 .data         00000800  000000018000e000  000000018000e000  0000ca00  2**4
                   CONTENTS, ALLOC, LOAD, DATA
-  3 .pdata        000008a0  000000018000f000  000000018000f000  0000ce00  2**2
+  3 .pdata        000008d0  000000018000f000  000000018000f000  0000d200  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  4 .rsrc         000001b4  0000000180010000  0000000180010000  0000d800  2**2
+  4 .rsrc         000001b4  0000000180010000  0000000180010000  0000dc00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  5 .reloc        000000e4  0000000180011000  0000000180011000  0000da00  2**2
+  5 .reloc        000000e4  0000000180011000  0000000180011000  0000de00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
 SYMBOL TABLE:
 no symbols
 
 
 
 Disassembly of section .text:
 
 0000000180001000 <.text>:
-   180001000:	lea    0x7685(%rip),%rcx        # 0x18000868c
-   180001007:	jmp    0x180007944
+   180001000:	lea    0x79a5(%rip),%rcx        # 0x1800089ac
+   180001007:	jmp    0x180007c04
    18000100c:	int3
    18000100d:	int3
    18000100e:	int3
    18000100f:	int3
    180001010:	rex push %rbx
    180001012:	sub    $0x20,%rsp
    180001016:	mov    %rcx,%rbx
@@ -2337,34 +2367,34 @@
    180001062:	mov    %edx,%esi
    180001064:	and    $0x1,%esi
    180001067:	test   $0x2,%dl
    18000106a:	je     0x1800010b2
    18000106c:	lea    -0x33(%rip),%r9        # 0x180001040
    180001073:	mov    -0x8(%rcx),%r8
    180001077:	mov    $0x18,%edx
-   18000107c:	call   0x180006fec
+   18000107c:	call   0x1800072ac
    180001081:	test   %esi,%esi
    180001083:	je     0x18000109e
    180001085:	mov    -0x8(%rbx),%rcx
    180001089:	lea    (%rcx,%rcx,2),%rdx
    18000108d:	lea    0x8(,%rdx,8),%rdx
    180001095:	lea    -0x8(%rbx),%rcx
-   180001099:	call   0x180007100
+   180001099:	call   0x1800073c0
    18000109e:	lea    -0x8(%rbx),%rax
    1800010a2:	mov    0x30(%rsp),%rbx
    1800010a7:	mov    0x38(%rsp),%rsi
    1800010ac:	add    $0x20,%rsp
    1800010b0:	pop    %rdi
    1800010b1:	ret
    1800010b2:	call   *0x8130(%rip)        # 0x1800091e8
    1800010b8:	test   %esi,%esi
    1800010ba:	je     0x1800010c9
    1800010bc:	mov    $0x18,%edx
    1800010c1:	mov    %rbx,%rcx
-   1800010c4:	call   0x1800070f8
+   1800010c4:	call   0x1800073b8
    1800010c9:	mov    %rbx,%rax
    1800010cc:	mov    0x30(%rsp),%rbx
    1800010d1:	mov    0x38(%rsp),%rsi
    1800010d6:	add    $0x20,%rsp
    1800010da:	pop    %rdi
    1800010db:	ret
    1800010dc:	int3
@@ -2386,20 +2416,20 @@
    1800010f6:	lea    0xcf6b(%rip),%rcx        # 0x18000e068
    1800010fd:	call   *0x80dd(%rip)        # 0x1800091e0
    180001103:	mov    %rax,%rcx
    180001106:	movl   $0x0,0x20(%rsp)
    18000110e:	lea    0xcf53(%rip),%r9        # 0x18000e068
    180001115:	lea    0xcf24(%rip),%r8        # 0x18000e040
    18000111c:	xor    %edx,%edx
-   18000111e:	call   0x180007fb6
+   18000111e:	call   0x180008276
    180001123:	mov    %rax,%rbx
    180001126:	test   %rax,%rax
    180001129:	jne    0x180001173
    18000112b:	lea    0x18(%rax),%ecx
-   18000112e:	call   0x1800070bc
+   18000112e:	call   0x18000737c
    180001133:	mov    %rax,%rbx
    180001136:	mov    %rax,0x40(%rsp)
    18000113b:	test   %rax,%rax
    18000113e:	je     0x180001161
    180001140:	xorps  %xmm0,%xmm0
    180001143:	xor    %eax,%eax
    180001145:	movups %xmm0,(%rbx)
@@ -2457,15 +2487,15 @@
    180001201:	xorps  %xmm0,%xmm0
    180001204:	movb   $0x1,0x28(%rsp)
    180001209:	lea    0x30(%rsp),%rax
    18000120e:	cmovae 0x30(%rsp),%rax
    180001214:	lea    0x20(%rsp),%rcx
    180001219:	mov    %rax,0x20(%rsp)
    18000121e:	movups %xmm0,(%rdx)
-   180001221:	call   0x180007fc2
+   180001221:	call   0x180008282
    180001226:	mov    0x48(%rsp),%rdx
    18000122b:	lea    0x837e(%rip),%rax        # 0x1800095b0
    180001232:	mov    %rax,(%rbx)
    180001235:	cmp    $0x10,%rdx
    180001239:	jb     0x180001270
    18000123b:	mov    0x30(%rsp),%rcx
    180001240:	inc    %rdx
@@ -2476,21 +2506,21 @@
    180001253:	add    $0x27,%rdx
    180001257:	sub    %rcx,%rax
    18000125a:	add    $0xfffffffffffffff8,%rax
    18000125e:	cmp    $0x1f,%rax
    180001262:	jbe    0x18000126b
    180001264:	call   *0x814e(%rip)        # 0x1800093b8
    18000126a:	int3
-   18000126b:	call   0x1800070f8
+   18000126b:	call   0x1800073b8
    180001270:	lea    0x8379(%rip),%rax        # 0x1800095f0
    180001277:	mov    %rax,(%rbx)
    18000127a:	mov    %rbx,%rax
    18000127d:	mov    0x50(%rsp),%rcx
    180001282:	xor    %rsp,%rcx
-   180001285:	call   0x180007240
+   180001285:	call   0x180007500
    18000128a:	add    $0x60,%rsp
    18000128e:	pop    %rbx
    18000128f:	ret
    180001290:	mov    %rbx,0x10(%rsp)
    180001295:	mov    %rcx,0x8(%rsp)
    18000129a:	push   %rsi
    18000129b:	push   %rdi
@@ -2600,15 +2630,15 @@
    180001402:	mov    (%rsi),%rax
    180001405:	movslq 0x4(%rax),%rcx
    180001409:	add    %rsi,%rcx
    18000140c:	xor    %r8d,%r8d
    18000140f:	mov    %ebx,%edx
    180001411:	call   *0x7ce9(%rip)        # 0x180009100
    180001417:	nop
-   180001418:	call   0x180006f94
+   180001418:	call   0x180007254
    18000141d:	test   %al,%al
    18000141f:	jne    0x18000142b
    180001421:	mov    %r12,%rcx
    180001424:	call   *0x7cc6(%rip)        # 0x1800090f0
    18000142a:	nop
    18000142b:	mov    (%r12),%rax
    18000142f:	movslq 0x4(%rax),%rcx
@@ -2708,20 +2738,20 @@
    18000152d:	mov    %rax,%rcx
    180001530:	cmp    %r8,%r15
    180001533:	jne    0x18000153a
    180001535:	sub    %rdx,%r8
    180001538:	jmp    0x180001553
    18000153a:	mov    %r15,%r8
    18000153d:	sub    %rdx,%r8
-   180001540:	call   0x180007fe0
+   180001540:	call   0x1800082a0
    180001545:	lea    0x4(%r14),%rcx
    180001549:	mov    0x8(%rbx),%r8
    18000154d:	sub    %r15,%r8
    180001550:	mov    %r15,%rdx
-   180001553:	call   0x180007fe0
+   180001553:	call   0x1800082a0
    180001558:	nop
    180001559:	mov    (%rbx),%rcx
    18000155c:	test   %rcx,%rcx
    18000155f:	je     0x180001592
    180001561:	mov    0x10(%rbx),%rdx
    180001565:	sub    %rcx,%rdx
    180001568:	and    $0xfffffffffffffffc,%rdx
@@ -2730,15 +2760,15 @@
    180001575:	add    $0x27,%rdx
    180001579:	mov    -0x8(%rcx),%r8
    18000157d:	sub    %r8,%rcx
    180001580:	lea    -0x8(%rcx),%rax
    180001584:	cmp    $0x1f,%rax
    180001588:	ja     0x1800015b8
    18000158a:	mov    %r8,%rcx
-   18000158d:	call   0x1800070f8
+   18000158d:	call   0x1800073b8
    180001592:	mov    %rsi,(%rbx)
    180001595:	lea    (%rsi,%r12,4),%rcx
    180001599:	mov    %rcx,0x8(%rbx)
    18000159d:	lea    (%rsi,%rdi,4),%rcx
    1800015a1:	mov    %rcx,0x10(%rbx)
    1800015a5:	mov    %r14,%rax
    1800015a8:	add    $0x20,%rsp
@@ -3146,56 +3176,56 @@
    180001b48:	cmp    $0x1000,%rax
    180001b4e:	jb     0x180001b81
    180001b50:	lea    0x27(%rax),%rcx
    180001b54:	cmp    %rax,%rcx
    180001b57:	jbe    0x180001c30
    180001b5d:	jmp    0x180001b69
    180001b5f:	movabs $0x8000000000000027,%rcx
-   180001b69:	call   0x1800070bc
+   180001b69:	call   0x18000737c
    180001b6e:	test   %rax,%rax
    180001b71:	je     0x180001bed
    180001b73:	lea    0x27(%rax),%rdi
    180001b77:	and    $0xffffffffffffffe0,%rdi
    180001b7b:	mov    %rax,-0x8(%rdi)
    180001b7f:	jmp    0x180001b95
    180001b81:	test   %rax,%rax
    180001b84:	je     0x180001b93
    180001b86:	mov    %rax,%rcx
-   180001b89:	call   0x1800070bc
+   180001b89:	call   0x18000737c
    180001b8e:	mov    %rax,%rdi
    180001b91:	jmp    0x180001b95
    180001b93:	xor    %edi,%edi
    180001b95:	mov    %r12,0x10(%rsi)
    180001b99:	mov    %r14,%r8
    180001b9c:	mov    %rbx,0x18(%rsi)
    180001ba0:	mov    %rdi,%rcx
    180001ba3:	cmp    $0x10,%rbp
    180001ba7:	jb     0x180001bf4
    180001ba9:	mov    (%rsi),%rbx
    180001bac:	mov    %rbx,%rdx
-   180001baf:	call   0x180007fda
+   180001baf:	call   0x18000829a
    180001bb4:	lea    0x1(%rbp),%rdx
    180001bb8:	mov    %r15b,(%rdi,%r14,1)
    180001bbc:	movb   $0x0,0x1(%rdi,%r14,1)
    180001bc2:	cmp    $0x1000,%rdx
    180001bc9:	jb     0x180001be3
    180001bcb:	mov    -0x8(%rbx),%rcx
    180001bcf:	add    $0x27,%rdx
    180001bd3:	sub    %rcx,%rbx
    180001bd6:	lea    -0x8(%rbx),%rax
    180001bda:	cmp    $0x1f,%rax
    180001bde:	ja     0x180001bed
    180001be0:	mov    %rcx,%rbx
    180001be3:	mov    %rbx,%rcx
-   180001be6:	call   0x1800070f8
+   180001be6:	call   0x1800073b8
    180001beb:	jmp    0x180001c06
    180001bed:	call   *0x77c5(%rip)        # 0x1800093b8
    180001bf3:	int3
    180001bf4:	mov    %rsi,%rdx
-   180001bf7:	call   0x180007fda
+   180001bf7:	call   0x18000829a
    180001bfc:	mov    %r15b,(%rdi,%r14,1)
    180001c00:	movb   $0x0,0x1(%rdi,%r14,1)
    180001c06:	mov    %rdi,(%rsi)
    180001c09:	mov    %rsi,%rax
    180001c0c:	mov    0x48(%rsp),%rdi
    180001c11:	mov    0x40(%rsp),%rbp
    180001c16:	mov    0x50(%rsp),%r12
@@ -3564,15 +3594,15 @@
    1800020c3:	call   *0x712f(%rip)        # 0x1800091f8
    1800020c9:	nop
    1800020ca:	mov    %r13d,0x20(%rsp)
    1800020cf:	lea    0xc0fa(%rip),%r9        # 0x18000e1d0
    1800020d6:	lea    0xc0c3(%rip),%r8        # 0x18000e1a0
    1800020dd:	xor    %edx,%edx
    1800020df:	mov    0x40(%rsp),%rcx
-   1800020e4:	call   0x180007fb6
+   1800020e4:	call   0x180008276
    1800020e9:	mov    0x48(%rsp),%rbx
    1800020ee:	test   %rax,%rax
    1800020f1:	je     0x180002111
    1800020f3:	mov    %r13,(%rdi)
    1800020f6:	mov    %r13,0x8(%rdi)
    1800020fa:	test   %rbx,%rbx
    1800020fd:	je     0x180002108
@@ -3590,15 +3620,15 @@
    18000212b:	cmpq   $0x0,(%rdi)
    18000212f:	jne    0x180002290
    180002135:	test   %rbx,%rbx
    180002138:	je     0x180002144
    18000213a:	cmpl   $0x2,0x8(%rbx)
    18000213e:	jge    0x1800022da
    180002144:	mov    $0x70,%ecx
-   180002149:	call   0x1800070bc
+   180002149:	call   0x18000737c
    18000214e:	mov    %rax,%rbx
    180002151:	mov    %rax,0xe0(%rsp)
    180002159:	test   %rax,%rax
    18000215c:	je     0x1800021c3
    18000215e:	movzwl 0xf0(%rsp),%ecx
    180002166:	mov    %cx,0x8(%rax)
    18000216a:	mov    %r13,0x10(%rax)
@@ -3621,23 +3651,23 @@
    1800021b8:	call   0x180003820
    1800021bd:	nop
    1800021be:	mov    %r12,(%rbx)
    1800021c1:	jmp    0x1800021c6
    1800021c3:	mov    %r13,%rbx
    1800021c6:	mov    %rbx,0xe0(%rsp)
    1800021ce:	mov    $0x18,%ecx
-   1800021d3:	call   0x1800070bc
+   1800021d3:	call   0x18000737c
    1800021d8:	mov    %rax,0x38(%rsp)
    1800021dd:	test   %rax,%rax
    1800021e0:	je     0x180002206
    1800021e2:	xorps  %xmm0,%xmm0
    1800021e5:	movups %xmm0,(%rax)
    1800021e8:	movl   $0x1,0x8(%rax)
    1800021ef:	movl   $0x1,0xc(%rax)
-   1800021f6:	lea    0x7643(%rip),%rcx        # 0x180009840
+   1800021f6:	lea    0x764b(%rip),%rcx        # 0x180009848
    1800021fd:	mov    %rcx,(%rax)
    180002200:	mov    %rbx,0x10(%rax)
    180002204:	jmp    0x180002209
    180002206:	mov    %r13,%rax
    180002209:	mov    %rbx,(%rdi)
    18000220c:	mov    0x8(%rdi),%rbx
    180002210:	mov    %rax,0x8(%rdi)
@@ -3696,20 +3726,20 @@
    1800022d0:	pop    %r14
    1800022d2:	pop    %r13
    1800022d4:	pop    %r12
    1800022d6:	pop    %rdi
    1800022d7:	pop    %rsi
    1800022d8:	pop    %rbp
    1800022d9:	ret
-   1800022da:	lea    0x75df(%rip),%rdx        # 0x1800098c0
+   1800022da:	lea    0x75ef(%rip),%rdx        # 0x1800098d0
    1800022e1:	lea    0x60(%rsp),%rcx
    1800022e6:	call   0x180001190
-   1800022eb:	lea    0x9436(%rip),%rdx        # 0x18000b728
+   1800022eb:	lea    0x94a6(%rip),%rdx        # 0x18000b798
    1800022f2:	lea    0x60(%rsp),%rcx
-   1800022f7:	call   0x180007fd4
+   1800022f7:	call   0x180008294
    1800022fc:	int3
    1800022fd:	int3
    1800022fe:	int3
    1800022ff:	int3
    180002300:	mov    %rbx,0x8(%rsp)
    180002305:	mov    %rbp,0x10(%rsp)
    18000230a:	mov    %rsi,0x18(%rsp)
@@ -3738,15 +3768,15 @@
    180002357:	mov    %rax,%rbx
    18000235a:	mov    %rax,0x40(%rsp)
    18000235f:	lea    (%rax,%rsi,4),%rdi
    180002363:	mov    %rdi,0x50(%rsp)
    180002368:	lea    0x0(,%rsi,4),%r8
    180002370:	xor    %edx,%edx
    180002372:	mov    %rax,%rcx
-   180002375:	call   0x180007fe6
+   180002375:	call   0x1800082a6
    18000237a:	mov    %rdi,%rbp
    18000237d:	mov    %rdi,%rdx
    180002380:	mov    %rdx,0x48(%rsp)
    180002385:	jmp    0x180002391
    180002387:	mov    0x48(%rsp),%rdx
    18000238c:	mov    0x40(%rsp),%rbx
    180002391:	mov    %r13,0x58(%rsp)
@@ -3759,15 +3789,15 @@
    1800023b3:	cmp    %rax,%rsi
    1800023b6:	jae    0x1800023cc
    1800023b8:	lea    (%rbx,%rsi,4),%rcx
    1800023bc:	cmp    %rdx,%rcx
    1800023bf:	je     0x1800023cc
    1800023c1:	sub    %rdx,%rbp
    1800023c4:	mov    %rbp,%r8
-   1800023c7:	call   0x180007fe0
+   1800023c7:	call   0x1800082a0
    1800023cc:	mov    %r15,%rcx
    1800023cf:	and    $0x1f,%ecx
    1800023d2:	jbe    0x1800023e1
    1800023d4:	mov    $0x1,%eax
    1800023d9:	shl    %cl,%eax
    1800023db:	dec    %eax
    1800023dd:	and    %eax,-0x4(%rbx,%rsi,4)
@@ -3850,15 +3880,15 @@
    180002512:	add    $0xfffffffffffffff8,%rax
    180002516:	cmp    $0x1f,%rax
    18000251a:	jbe    0x180002523
    18000251c:	call   *0x6e96(%rip)        # 0x1800093b8
    180002522:	int3
    180002523:	mov    %rdi,%rdx
    180002526:	mov    %rbx,%rcx
-   180002529:	call   0x1800070f8
+   180002529:	call   0x1800073b8
    18000252e:	lea    0x60(%rsp),%r11
    180002533:	mov    0x30(%r11),%rbx
    180002537:	mov    0x38(%r11),%rbp
    18000253b:	mov    0x40(%r11),%rsi
    18000253f:	mov    %r11,%rsp
    180002542:	pop    %r15
    180002544:	pop    %r14
@@ -3965,15 +3995,15 @@
    1800026c3:	mov    (%rcx,%rdi,8),%rbx
    1800026c7:	test   %rbx,%rbx
    1800026ca:	jne    0x180002733
    1800026cc:	jmp    0x1800026d0
    1800026ce:	xor    %ebx,%ebx
    1800026d0:	cmpb   $0x0,0x24(%rax)
    1800026d4:	je     0x1800026e9
-   1800026d6:	call   0x180006fd4
+   1800026d6:	call   0x180007294
    1800026db:	cmp    0x18(%rax),%rdi
    1800026df:	jae    0x1800026ee
    1800026e1:	mov    0x10(%rax),%rax
    1800026e5:	mov    (%rax,%rdi,8),%rbx
    1800026e9:	test   %rbx,%rbx
    1800026ec:	jne    0x180002733
    1800026ee:	mov    0x48(%rsp),%rbx
@@ -3983,15 +4013,15 @@
    1800026fb:	lea    0x48(%rsp),%rcx
    180002700:	call   *0x6a8a(%rip)        # 0x180009190
    180002706:	cmp    $0xffffffffffffffff,%rax
    18000270a:	je     0x180002749
    18000270c:	mov    0x48(%rsp),%rbx
    180002711:	mov    %rbx,0x50(%rsp)
    180002716:	mov    %rbx,%rcx
-   180002719:	call   0x180006f9c
+   180002719:	call   0x18000725c
    18000271e:	mov    (%rbx),%rax
    180002721:	mov    %rbx,%rcx
    180002724:	call   *0x8(%rax)
    180002727:	mov    0x48(%rsp),%rbx
    18000272c:	mov    %rbx,0xbf05(%rip)        # 0x18000e638
    180002733:	lea    0x40(%rsp),%rcx
    180002738:	call   *0x6a0a(%rip)        # 0x180009148
@@ -4043,29 +4073,29 @@
    1800027e5:	lea    0x0(,%rsi,8),%rcx
    1800027ed:	cmp    $0x1000,%rcx
    1800027f4:	jb     0x18000282d
    1800027f6:	lea    0x27(%rcx),%rax
    1800027fa:	cmp    %rcx,%rax
    1800027fd:	jbe    0x180002876
    1800027ff:	mov    %rax,%rcx
-   180002802:	call   0x1800070bc
+   180002802:	call   0x18000737c
    180002807:	test   %rax,%rax
    18000280a:	je     0x180002826
    18000280c:	lea    0x27(%rax),%rdx
    180002810:	and    $0xffffffffffffffe0,%rdx
    180002814:	mov    %rax,-0x8(%rdx)
    180002818:	mov    %rdx,0x8(%rbx)
    18000281c:	mov    %rsi,0x10(%rbx)
    180002820:	orq    $0x1,(%rbx)
    180002824:	jmp    0x18000284c
    180002826:	call   *0x6b8c(%rip)        # 0x1800093b8
    18000282c:	int3
    18000282d:	test   %rcx,%rcx
    180002830:	je     0x18000283a
-   180002832:	call   0x1800070bc
+   180002832:	call   0x18000737c
    180002837:	mov    %rax,%rdx
    18000283a:	mov    %rdx,0x8(%rbx)
    18000283e:	mov    %rsi,0x10(%rbx)
    180002842:	orq    $0x1,(%rbx)
    180002846:	jmp    0x18000284c
    180002848:	lea    0x8(%rcx),%rdx
    18000284c:	mov    %rdi,%r9
@@ -4092,15 +4122,15 @@
    180002889:	mov    %rdx,%rax
    18000288c:	lea    0x6c95(%rip),%rcx        # 0x180009528
    180002893:	xorps  %xmm0,%xmm0
    180002896:	lea    0x8(%rbx),%rdx
    18000289a:	mov    %rcx,(%rbx)
    18000289d:	lea    0x8(%rax),%rcx
    1800028a1:	movups %xmm0,(%rdx)
-   1800028a4:	call   0x180007fc2
+   1800028a4:	call   0x180008282
    1800028a9:	lea    0x6d40(%rip),%rax        # 0x1800095f0
    1800028b0:	mov    %rax,(%rbx)
    1800028b3:	mov    %rbx,%rax
    1800028b6:	add    $0x20,%rsp
    1800028ba:	pop    %rbx
    1800028bb:	ret
    1800028bc:	int3
@@ -4111,29 +4141,29 @@
    1800028c5:	push   %rbx
    1800028c6:	push   %rsi
    1800028c7:	push   %rdi
    1800028c8:	sub    $0xc0,%rsp
    1800028cf:	mov    %rcx,%rdi
    1800028d2:	mov    %rdx,(%rcx)
    1800028d5:	lea    0xf0(%rsp),%rcx
-   1800028dd:	call   0x180006f58
+   1800028dd:	call   0x180007218
    1800028e2:	mov    (%rax),%r8
    1800028e5:	xor    %ebx,%ebx
    1800028e7:	mov    %rbx,(%rax)
    1800028ea:	mov    %r8,0x8(%rdi)
    1800028ee:	mov    0xf0(%rsp),%rcx
    1800028f6:	test   %rcx,%rcx
    1800028f9:	je     0x180002907
    1800028fb:	mov    (%rcx),%rax
    1800028fe:	lea    0x1(%rbx),%edx
    180002901:	call   *(%rax)
    180002903:	mov    0x8(%rdi),%r8
    180002907:	lea    0x10(%rdi),%rcx
    18000290b:	mov    (%rdi),%rdx
-   18000290e:	call   0x180006f34
+   18000290e:	call   0x1800071f4
    180002913:	nop
    180002914:	mov    %rbx,0x20(%rdi)
    180002918:	mov    %rbx,0x28(%rdi)
    18000291c:	mov    %rbx,0x30(%rdi)
    180002920:	xor    %eax,%eax
    180002922:	mov    %al,0x38(%rdi)
    180002925:	mov    %rbx,0x40(%rdi)
@@ -4233,15 +4263,15 @@
    180002a89:	mov    %rdx,%rax
    180002a8c:	lea    0x6a95(%rip),%rcx        # 0x180009528
    180002a93:	xorps  %xmm0,%xmm0
    180002a96:	lea    0x8(%rbx),%rdx
    180002a9a:	mov    %rcx,(%rbx)
    180002a9d:	lea    0x8(%rax),%rcx
    180002aa1:	movups %xmm0,(%rdx)
-   180002aa4:	call   0x180007fc2
+   180002aa4:	call   0x180008282
    180002aa9:	lea    0x6aa8(%rip),%rax        # 0x180009558
    180002ab0:	mov    %rax,(%rbx)
    180002ab3:	mov    %rbx,%rax
    180002ab6:	add    $0x20,%rsp
    180002aba:	pop    %rbx
    180002abb:	ret
    180002abc:	int3
@@ -4254,15 +4284,15 @@
    180002ac9:	mov    %rdx,%rax
    180002acc:	lea    0x6a55(%rip),%rcx        # 0x180009528
    180002ad3:	xorps  %xmm0,%xmm0
    180002ad6:	lea    0x8(%rbx),%rdx
    180002ada:	mov    %rcx,(%rbx)
    180002add:	lea    0x8(%rax),%rcx
    180002ae1:	movups %xmm0,(%rdx)
-   180002ae4:	call   0x180007fc2
+   180002ae4:	call   0x180008282
    180002ae9:	lea    0x6a80(%rip),%rax        # 0x180009570
    180002af0:	mov    %rax,(%rbx)
    180002af3:	mov    %rbx,%rax
    180002af6:	add    $0x20,%rsp
    180002afa:	pop    %rbx
    180002afb:	ret
    180002afc:	int3
@@ -4297,15 +4327,15 @@
    180002b39:	mov    %rdx,%rax
    180002b3c:	lea    0x69e5(%rip),%rcx        # 0x180009528
    180002b43:	xorps  %xmm0,%xmm0
    180002b46:	lea    0x8(%rbx),%rdx
    180002b4a:	mov    %rcx,(%rbx)
    180002b4d:	lea    0x8(%rax),%rcx
    180002b51:	movups %xmm0,(%rdx)
-   180002b54:	call   0x180007fc2
+   180002b54:	call   0x180008282
    180002b59:	lea    0x6a68(%rip),%rax        # 0x1800095c8
    180002b60:	mov    %rax,(%rbx)
    180002b63:	mov    %rbx,%rax
    180002b66:	add    $0x20,%rsp
    180002b6a:	pop    %rbx
    180002b6b:	ret
    180002b6c:	int3
@@ -4340,15 +4370,15 @@
    180002ba9:	mov    %rdx,%rax
    180002bac:	lea    0x6975(%rip),%rcx        # 0x180009528
    180002bb3:	xorps  %xmm0,%xmm0
    180002bb6:	lea    0x8(%rbx),%rdx
    180002bba:	mov    %rcx,(%rbx)
    180002bbd:	lea    0x8(%rax),%rcx
    180002bc1:	movups %xmm0,(%rdx)
-   180002bc4:	call   0x180007fc2
+   180002bc4:	call   0x180008282
    180002bc9:	mov    %rbx,%rax
    180002bcc:	add    $0x20,%rsp
    180002bd0:	pop    %rbx
    180002bd1:	ret
    180002bd2:	int3
    180002bd3:	int3
    180002bd4:	int3
@@ -4369,15 +4399,15 @@
    180002be9:	mov    %rdx,%rax
    180002bec:	lea    0x6935(%rip),%rcx        # 0x180009528
    180002bf3:	xorps  %xmm0,%xmm0
    180002bf6:	lea    0x8(%rbx),%rdx
    180002bfa:	mov    %rcx,(%rbx)
    180002bfd:	lea    0x8(%rax),%rcx
    180002c01:	movups %xmm0,(%rdx)
-   180002c04:	call   0x180007fc2
+   180002c04:	call   0x180008282
    180002c09:	lea    0x69a0(%rip),%rax        # 0x1800095b0
    180002c10:	mov    %rax,(%rbx)
    180002c13:	mov    %rbx,%rax
    180002c16:	add    $0x20,%rsp
    180002c1a:	pop    %rbx
    180002c1b:	ret
    180002c1c:	int3
@@ -4396,15 +4426,15 @@
    180002c42:	add    $0x27,%rdx
    180002c46:	sub    %r8,%rcx
    180002c49:	lea    -0x8(%rcx),%rax
    180002c4d:	cmp    $0x1f,%rax
    180002c51:	ja     0x180002c64
    180002c53:	mov    %r8,%rcx
    180002c56:	add    $0x28,%rsp
-   180002c5a:	jmp    0x1800070f8
+   180002c5a:	jmp    0x1800073b8
    180002c5f:	add    $0x28,%rsp
    180002c63:	ret
    180002c64:	call   *0x674e(%rip)        # 0x1800093b8
    180002c6a:	int3
    180002c6b:	int3
    180002c6c:	int3
    180002c6d:	int3
@@ -4455,15 +4485,15 @@
    180002cc5:	mov    -0x8(%rcx),%r8
    180002cc9:	add    $0x27,%rdx
    180002ccd:	sub    %r8,%rcx
    180002cd0:	lea    -0x8(%rcx),%rax
    180002cd4:	cmp    $0x1f,%rax
    180002cd8:	ja     0x180002cf5
    180002cda:	mov    %r8,%rcx
-   180002cdd:	call   0x1800070f8
+   180002cdd:	call   0x1800073b8
    180002ce2:	xor    %eax,%eax
    180002ce4:	mov    %rax,(%rbx)
    180002ce7:	mov    %rax,0x8(%rbx)
    180002ceb:	mov    %rax,0x10(%rbx)
    180002cef:	add    $0x20,%rsp
    180002cf3:	pop    %rbx
    180002cf4:	ret
@@ -4520,15 +4550,15 @@
    180002d92:	mov    -0x8(%rcx),%r8
    180002d96:	add    $0x27,%rdx
    180002d9a:	sub    %r8,%rcx
    180002d9d:	lea    -0x8(%rcx),%rax
    180002da1:	cmp    $0x1f,%rax
    180002da5:	ja     0x180002dc8
    180002da7:	mov    %r8,%rcx
-   180002daa:	call   0x1800070f8
+   180002daa:	call   0x1800073b8
    180002daf:	movq   $0x0,0x10(%rbx)
    180002db7:	movq   $0xf,0x18(%rbx)
    180002dbf:	movb   $0x0,(%rbx)
    180002dc2:	add    $0x20,%rsp
    180002dc6:	pop    %rbx
    180002dc7:	ret
    180002dc8:	call   *0x65ea(%rip)        # 0x1800093b8
@@ -4595,15 +4625,15 @@
    180002e70:	mov    -0x8(%rcx),%r8
    180002e74:	add    $0x27,%rdx
    180002e78:	sub    %r8,%rcx
    180002e7b:	lea    -0x8(%rcx),%rax
    180002e7f:	cmp    $0x1f,%rax
    180002e83:	ja     0x180002ea0
    180002e85:	mov    %r8,%rcx
-   180002e88:	call   0x1800070f8
+   180002e88:	call   0x1800073b8
    180002e8d:	xor    %eax,%eax
    180002e8f:	mov    %rax,(%rbx)
    180002e92:	mov    %rax,0x8(%rbx)
    180002e96:	mov    %rax,0x10(%rbx)
    180002e9a:	add    $0x20,%rsp
    180002e9e:	pop    %rbx
    180002e9f:	ret
@@ -4639,15 +4669,15 @@
    180002ef4:	mov    -0x8(%rcx),%r8
    180002ef8:	add    $0x27,%rdx
    180002efc:	sub    %r8,%rcx
    180002eff:	lea    -0x8(%rcx),%rax
    180002f03:	cmp    $0x1f,%rax
    180002f07:	ja     0x180002f24
    180002f09:	mov    %r8,%rcx
-   180002f0c:	call   0x1800070f8
+   180002f0c:	call   0x1800073b8
    180002f11:	xor    %eax,%eax
    180002f13:	mov    %rax,(%rbx)
    180002f16:	mov    %rax,0x8(%rbx)
    180002f1a:	mov    %rax,0x10(%rbx)
    180002f1e:	add    $0x20,%rsp
    180002f22:	pop    %rbx
    180002f23:	ret
@@ -4671,15 +4701,15 @@
    180002f53:	mov    -0x8(%rcx),%r8
    180002f57:	add    $0x27,%rdx
    180002f5b:	sub    %r8,%rcx
    180002f5e:	lea    -0x8(%rcx),%rax
    180002f62:	cmp    $0x1f,%rax
    180002f66:	ja     0x180002f8a
    180002f68:	mov    %r8,%rcx
-   180002f6b:	call   0x1800070f8
+   180002f6b:	call   0x1800073b8
    180002f70:	movq   $0x0,0x20(%rbx)
    180002f78:	movq   $0xf,0x28(%rbx)
    180002f80:	movb   $0x0,0x10(%rbx)
    180002f84:	add    $0x20,%rsp
    180002f88:	pop    %rbx
    180002f89:	ret
    180002f8a:	call   *0x6428(%rip)        # 0x1800093b8
@@ -4725,15 +4755,15 @@
    180002ffa:	mov    -0x8(%rcx),%r8
    180002ffe:	add    $0x27,%rdx
    180003002:	sub    %r8,%rcx
    180003005:	lea    -0x8(%rcx),%rax
    180003009:	cmp    $0x1f,%rax
    18000300d:	ja     0x180003145
    180003013:	mov    %r8,%rcx
-   180003016:	call   0x1800070f8
+   180003016:	call   0x1800073b8
    18000301b:	add    $0x20,%rbx
    18000301f:	add    $0x20,%rsi
    180003023:	cmp    %rbp,%rbx
    180003026:	jne    0x180002fe0
    180003028:	mov    0x50(%rdi),%rbx
    18000302c:	mov    0x60(%rdi),%rdx
    180003030:	sub    %rbx,%rdx
@@ -4744,15 +4774,15 @@
    180003044:	add    $0x27,%rdx
    180003048:	sub    %rcx,%rbx
    18000304b:	lea    -0x8(%rbx),%rax
    18000304f:	cmp    $0x1f,%rax
    180003053:	ja     0x180003145
    180003059:	mov    %rcx,%rbx
    18000305c:	mov    %rbx,%rcx
-   18000305f:	call   0x1800070f8
+   18000305f:	call   0x1800073b8
    180003064:	mov    %r14,0x50(%rdi)
    180003068:	mov    %r14,0x58(%rdi)
    18000306c:	mov    %r14,0x60(%rdi)
    180003070:	mov    0x38(%rdi),%rcx
    180003074:	test   %rcx,%rcx
    180003077:	je     0x1800030ba
    180003079:	mov    0x48(%rdi),%rdx
@@ -4763,15 +4793,15 @@
    18000308d:	mov    -0x8(%rcx),%r8
    180003091:	add    $0x27,%rdx
    180003095:	sub    %r8,%rcx
    180003098:	lea    -0x8(%rcx),%rax
    18000309c:	cmp    $0x1f,%rax
    1800030a0:	ja     0x180003145
    1800030a6:	mov    %r8,%rcx
-   1800030a9:	call   0x1800070f8
+   1800030a9:	call   0x1800073b8
    1800030ae:	mov    %r14,0x38(%rdi)
    1800030b2:	mov    %r14,0x40(%rdi)
    1800030b6:	mov    %r14,0x48(%rdi)
    1800030ba:	testb  $0x1,0x20(%rdi)
    1800030be:	je     0x1800030f2
    1800030c0:	mov    0x30(%rdi),%rdx
    1800030c4:	mov    0x28(%rdi),%rcx
@@ -4781,30 +4811,30 @@
    1800030d5:	mov    -0x8(%rcx),%r8
    1800030d9:	add    $0x27,%rdx
    1800030dd:	sub    %r8,%rcx
    1800030e0:	lea    -0x8(%rcx),%rax
    1800030e4:	cmp    $0x1f,%rax
    1800030e8:	ja     0x180003145
    1800030ea:	mov    %r8,%rcx
-   1800030ed:	call   0x1800070f8
+   1800030ed:	call   0x1800073b8
    1800030f2:	testb  $0x1,0x8(%rdi)
    1800030f6:	je     0x18000312a
    1800030f8:	mov    0x18(%rdi),%rdx
    1800030fc:	mov    0x10(%rdi),%rcx
    180003100:	shl    $0x2,%rdx
    180003104:	cmp    $0x1000,%rdx
    18000310b:	jb     0x180003125
    18000310d:	mov    -0x8(%rcx),%r8
    180003111:	add    $0x27,%rdx
    180003115:	sub    %r8,%rcx
    180003118:	lea    -0x8(%rcx),%rax
    18000311c:	cmp    $0x1f,%rax
    180003120:	ja     0x180003145
    180003122:	mov    %r8,%rcx
-   180003125:	call   0x1800070f8
+   180003125:	call   0x1800073b8
    18000312a:	mov    0x30(%rsp),%rbx
    18000312f:	mov    0x38(%rsp),%rbp
    180003134:	mov    0x40(%rsp),%rsi
    180003139:	mov    0x48(%rsp),%rdi
    18000313e:	add    $0x20,%rsp
    180003142:	pop    %r14
    180003144:	ret
@@ -4813,15 +4843,15 @@
    18000314c:	int3
    18000314d:	int3
    18000314e:	int3
    18000314f:	int3
    180003150:	lea    0x63d1(%rip),%rax        # 0x180009528
    180003157:	mov    %rax,(%rcx)
    18000315a:	add    $0x8,%rcx
-   18000315e:	jmp    0x180007fc8
+   18000315e:	jmp    0x180008288
    180003163:	int3
    180003164:	int3
    180003165:	int3
    180003166:	int3
    180003167:	int3
    180003168:	int3
    180003169:	int3
@@ -4853,15 +4883,15 @@
    1800031b2:	mov    (%rbx),%rax
    1800031b5:	mov    %rbx,%rcx
    1800031b8:	call   *0x8(%rax)
    1800031bb:	mov    0x38(%rsp),%rsi
    1800031c0:	lea    0x20(%rdi),%rcx
    1800031c4:	call   0x180002e30
    1800031c9:	lea    0x10(%rdi),%rcx
-   1800031cd:	call   0x180006f3a
+   1800031cd:	call   0x1800071fa
    1800031d2:	mov    0x8(%rdi),%rcx
    1800031d6:	mov    0x20(%rsp),%rdi
    1800031db:	mov    0x30(%rsp),%rbx
    1800031e0:	test   %rcx,%rcx
    1800031e3:	je     0x1800031f4
    1800031e5:	mov    (%rcx),%rax
    1800031e8:	mov    $0x1,%edx
@@ -4915,15 +4945,15 @@
    180003257:	rex.WB jmp *(%r8)
    18000325a:	add    $0x28,%rsp
    18000325e:	ret
    18000325f:	int3
    180003260:	rex push %rbx
    180003262:	sub    $0x20,%rsp
    180003266:	mov    %rcx,%rbx
-   180003269:	call   0x180006f94
+   180003269:	call   0x180007254
    18000326e:	test   %al,%al
    180003270:	jne    0x18000327c
    180003272:	mov    (%rbx),%rcx
    180003275:	call   *0x5e75(%rip)        # 0x1800090f0
    18000327b:	nop
    18000327c:	mov    (%rbx),%rdx
    18000327f:	mov    (%rdx),%rax
@@ -4986,27 +5016,27 @@
    180003333:	call   0x180002eb0
    180003338:	mov    %rdi,%rcx
    18000333b:	call   0x180002f30
    180003340:	test   $0x1,%bl
    180003343:	je     0x180003352
    180003345:	mov    $0x70,%edx
    18000334a:	mov    %rdi,%rcx
-   18000334d:	call   0x1800070f8
+   18000334d:	call   0x1800073b8
    180003352:	mov    0x30(%rsp),%rbx
    180003357:	mov    %rdi,%rax
    18000335a:	add    $0x20,%rsp
    18000335e:	pop    %rdi
    18000335f:	ret
    180003360:	rex push %rbx
    180003362:	sub    $0x20,%rsp
    180003366:	mov    %rcx,%rbx
    180003369:	test   $0x1,%dl
    18000336c:	je     0x180003378
    18000336e:	mov    $0x18,%edx
-   180003373:	call   0x1800070f8
+   180003373:	call   0x1800073b8
    180003378:	mov    %rbx,%rax
    18000337b:	add    $0x20,%rsp
    18000337f:	pop    %rbx
    180003380:	ret
    180003381:	int3
    180003382:	int3
    180003383:	int3
@@ -5028,15 +5058,15 @@
    18000339a:	mov    %edx,%ebx
    18000339c:	mov    %rcx,%rdi
    18000339f:	call   0x180002d00
    1800033a4:	test   $0x1,%bl
    1800033a7:	je     0x1800033b6
    1800033a9:	mov    $0x98,%edx
    1800033ae:	mov    %rdi,%rcx
-   1800033b1:	call   0x1800070f8
+   1800033b1:	call   0x1800073b8
    1800033b6:	mov    0x30(%rsp),%rbx
    1800033bb:	mov    %rdi,%rax
    1800033be:	add    $0x20,%rsp
    1800033c2:	pop    %rdi
    1800033c3:	ret
    1800033c4:	int3
    1800033c5:	int3
@@ -5057,15 +5087,15 @@
    1800033e1:	mov    %edx,%ebx
    1800033e3:	mov    %rdi,%rcx
    1800033e6:	call   0x1800032a0
    1800033eb:	test   $0x1,%bl
    1800033ee:	je     0x1800033fd
    1800033f0:	mov    $0x118,%edx
    1800033f5:	mov    %rdi,%rcx
-   1800033f8:	call   0x1800070f8
+   1800033f8:	call   0x1800073b8
    1800033fd:	mov    0x30(%rsp),%rbx
    180003402:	mov    %rdi,%rax
    180003405:	add    $0x20,%rsp
    180003409:	pop    %rdi
    18000340a:	ret
    18000340b:	int3
    18000340c:	int3
@@ -5076,20 +5106,20 @@
    180003415:	push   %rdi
    180003416:	sub    $0x20,%rsp
    18000341a:	lea    0x6107(%rip),%rax        # 0x180009528
    180003421:	mov    %rcx,%rdi
    180003424:	mov    %rax,(%rcx)
    180003427:	mov    %edx,%ebx
    180003429:	add    $0x8,%rcx
-   18000342d:	call   0x180007fc8
+   18000342d:	call   0x180008288
    180003432:	test   $0x1,%bl
    180003435:	je     0x180003444
    180003437:	mov    $0x18,%edx
    18000343c:	mov    %rdi,%rcx
-   18000343f:	call   0x1800070f8
+   18000343f:	call   0x1800073b8
    180003444:	mov    0x30(%rsp),%rbx
    180003449:	mov    %rdi,%rax
    18000344c:	add    $0x20,%rsp
    180003450:	pop    %rdi
    180003451:	ret
    180003452:	int3
    180003453:	int3
@@ -5131,15 +5161,15 @@
    1800034b7:	mov    -0x8(%rcx),%r8
    1800034bb:	add    $0x27,%rdx
    1800034bf:	sub    %r8,%rcx
    1800034c2:	lea    -0x8(%rcx),%rax
    1800034c6:	cmp    $0x1f,%rax
    1800034ca:	ja     0x180003502
    1800034cc:	mov    %r8,%rcx
-   1800034cf:	call   0x1800070f8
+   1800034cf:	call   0x1800073b8
    1800034d4:	imul   $0x58,%rbp,%rax
    1800034d8:	mov    0x38(%rsp),%rbp
    1800034dd:	add    %rdi,%rax
    1800034e0:	mov    %rdi,(%rbx)
    1800034e3:	mov    %rax,0x8(%rbx)
    1800034e7:	imul   $0x58,%rsi,%rax
    1800034eb:	mov    0x40(%rsp),%rsi
@@ -5185,15 +5215,15 @@
    18000356c:	mov    -0x8(%rcx),%r8
    180003570:	add    $0x27,%rdx
    180003574:	sub    %r8,%rcx
    180003577:	lea    -0x8(%rcx),%rax
    18000357b:	cmp    $0x1f,%rax
    18000357f:	ja     0x1800035ba
    180003581:	mov    %r8,%rcx
-   180003584:	call   0x1800070f8
+   180003584:	call   0x1800073b8
    180003589:	mov    %rdi,(%rbx)
    18000358c:	lea    (%r14,%r14,4),%rax
    180003590:	lea    (%rdi,%rax,8),%rcx
    180003594:	mov    %rcx,0x8(%rbx)
    180003598:	lea    (%rsi,%rsi,4),%rax
    18000359c:	mov    0x38(%rsp),%rsi
    1800035a1:	lea    (%rdi,%rax,8),%rcx
@@ -5256,15 +5286,15 @@
    18000364e:	add    $0x27,%rdx
    180003652:	sub    %rcx,%r8
    180003655:	lea    -0x8(%r8),%rax
    180003659:	cmp    $0x1f,%rax
    18000365d:	ja     0x1800036a0
    18000365f:	mov    %rcx,%r8
    180003662:	mov    %r8,%rcx
-   180003665:	call   0x1800070f8
+   180003665:	call   0x1800073b8
    18000366a:	xor    %eax,%eax
    18000366c:	mov    %rax,(%rbx)
    18000366f:	mov    %rax,0x8(%rbx)
    180003673:	mov    %rax,0x10(%rbx)
    180003677:	mov    %rdi,%rdx
    18000367a:	mov    %rbx,%rcx
    18000367d:	call   0x180003ab0
@@ -5352,15 +5382,15 @@
    180003761:	cmp    $0x2,%eax
    180003764:	jne    0x1800037bf
    180003766:	movb   $0x0,0x71(%rbx)
    18000376a:	mov    $0x1,%al
    18000376c:	mov    0x78(%rsp),%rdi
    180003771:	mov    0x58(%rsp),%rcx
    180003776:	xor    %rsp,%rcx
-   180003779:	call   0x180007240
+   180003779:	call   0x180007500
    18000377e:	add    $0x60,%rsp
    180003782:	pop    %rbx
    180003783:	ret
    180003784:	movb   $0x0,0x71(%rbx)
    180003788:	mov    0x30(%rsp),%rdi
    18000378d:	lea    0x38(%rsp),%rax
    180003792:	sub    %rax,%rdi
@@ -5376,15 +5406,15 @@
    1800037ba:	sete   %al
    1800037bd:	jmp    0x18000376c
    1800037bf:	xor    %al,%al
    1800037c1:	jmp    0x18000376c
    1800037c3:	mov    $0x1,%al
    1800037c5:	mov    0x58(%rsp),%rcx
    1800037ca:	xor    %rsp,%rcx
-   1800037cd:	call   0x180007240
+   1800037cd:	call   0x180007500
    1800037d2:	add    $0x60,%rsp
    1800037d6:	pop    %rbx
    1800037d7:	ret
    1800037d8:	int3
    1800037d9:	int3
    1800037da:	int3
    1800037db:	int3
@@ -5498,24 +5528,24 @@
    1800038e5:	mov    %rdx,(%rax)
    1800038e8:	mov    0x50(%rcx),%rax
    1800038ec:	mov    %r8d,(%rax)
    1800038ef:	ret
    1800038f0:	sub    $0x48,%rsp
    1800038f4:	lea    0x20(%rsp),%rcx
    1800038f9:	call   0x180002b00
-   1800038fe:	lea    0x7ce3(%rip),%rdx        # 0x18000b5e8
+   1800038fe:	lea    0x7d53(%rip),%rdx        # 0x18000b658
    180003905:	lea    0x20(%rsp),%rcx
-   18000390a:	call   0x180007fd4
+   18000390a:	call   0x180008294
    18000390f:	int3
    180003910:	sub    $0x48,%rsp
    180003914:	lea    0x20(%rsp),%rcx
    180003919:	call   0x180002b70
-   18000391e:	lea    0x7da3(%rip),%rdx        # 0x18000b6c8
+   18000391e:	lea    0x7e13(%rip),%rdx        # 0x18000b738
    180003925:	lea    0x20(%rsp),%rcx
-   18000392a:	call   0x180007fd4
+   18000392a:	call   0x180008294
    18000392f:	int3
    180003930:	mov    0x80(%rcx),%rcx
    180003937:	test   %rcx,%rcx
    18000393a:	je     0x180003943
    18000393c:	rex.W jmp *0x5a1d(%rip)        # 0x180009360
    180003943:	ret
    180003944:	int3
@@ -5527,16 +5557,16 @@
    18000394a:	int3
    18000394b:	int3
    18000394c:	int3
    18000394d:	int3
    18000394e:	int3
    18000394f:	int3
    180003950:	sub    $0x28,%rsp
-   180003954:	lea    0x5f4d(%rip),%rcx        # 0x1800098a8
-   18000395b:	call   0x180006f8e
+   180003954:	lea    0x5f5d(%rip),%rcx        # 0x1800098b8
+   18000395b:	call   0x18000724e
    180003960:	int3
    180003961:	int3
    180003962:	int3
    180003963:	int3
    180003964:	int3
    180003965:	int3
    180003966:	int3
@@ -5547,15 +5577,15 @@
    18000396b:	int3
    18000396c:	int3
    18000396d:	int3
    18000396e:	int3
    18000396f:	int3
    180003970:	sub    $0x28,%rsp
    180003974:	lea    0x5c1d(%rip),%rcx        # 0x180009598
-   18000397b:	call   0x180006f8e
+   18000397b:	call   0x18000724e
    180003980:	int3
    180003981:	int3
    180003982:	int3
    180003983:	int3
    180003984:	int3
    180003985:	int3
    180003986:	int3
@@ -5565,16 +5595,16 @@
    18000398a:	int3
    18000398b:	int3
    18000398c:	int3
    18000398d:	int3
    18000398e:	int3
    18000398f:	int3
    180003990:	sub    $0x28,%rsp
-   180003994:	lea    0x5e8d(%rip),%rcx        # 0x180009828
-   18000399b:	call   0x180006f8e
+   180003994:	lea    0x5e95(%rip),%rcx        # 0x180009830
+   18000399b:	call   0x18000724e
    1800039a0:	int3
    1800039a1:	int3
    1800039a2:	int3
    1800039a3:	int3
    1800039a4:	int3
    1800039a5:	int3
    1800039a6:	int3
@@ -5584,16 +5614,16 @@
    1800039aa:	int3
    1800039ab:	int3
    1800039ac:	int3
    1800039ad:	int3
    1800039ae:	int3
    1800039af:	int3
    1800039b0:	sub    $0x28,%rsp
-   1800039b4:	lea    0x5e6d(%rip),%rcx        # 0x180009828
-   1800039bb:	call   0x180006f8e
+   1800039b4:	lea    0x5e75(%rip),%rcx        # 0x180009830
+   1800039bb:	call   0x18000724e
    1800039c0:	int3
    1800039c1:	int3
    1800039c2:	int3
    1800039c3:	int3
    1800039c4:	int3
    1800039c5:	int3
    1800039c6:	int3
@@ -5613,29 +5643,29 @@
    1800039e3:	lea    0x0(,%rdx,4),%rcx
    1800039eb:	cmp    $0x1000,%rcx
    1800039f2:	jb     0x180003a25
    1800039f4:	lea    0x27(%rcx),%rax
    1800039f8:	cmp    %rcx,%rax
    1800039fb:	jbe    0x180003a3a
    1800039fd:	mov    %rax,%rcx
-   180003a00:	call   0x1800070bc
+   180003a00:	call   0x18000737c
    180003a05:	mov    %rax,%rcx
    180003a08:	test   %rax,%rax
    180003a0b:	je     0x180003a1e
    180003a0d:	add    $0x27,%rax
    180003a11:	and    $0xffffffffffffffe0,%rax
    180003a15:	mov    %rcx,-0x8(%rax)
    180003a19:	add    $0x28,%rsp
    180003a1d:	ret
    180003a1e:	call   *0x5994(%rip)        # 0x1800093b8
    180003a24:	int3
    180003a25:	test   %rcx,%rcx
    180003a28:	je     0x180003a33
    180003a2a:	add    $0x28,%rsp
-   180003a2e:	jmp    0x1800070bc
+   180003a2e:	jmp    0x18000737c
    180003a33:	xor    %eax,%eax
    180003a35:	add    $0x28,%rsp
    180003a39:	ret
    180003a3a:	call   0x1800038f0
    180003a3f:	int3
    180003a40:	sub    $0x28,%rsp
    180003a44:	movabs $0x2e8ba2e8ba2e8ba,%rax
@@ -5644,29 +5674,29 @@
    180003a53:	imul   $0x58,%rdx,%rcx
    180003a57:	cmp    $0x1000,%rcx
    180003a5e:	jb     0x180003a91
    180003a60:	lea    0x27(%rcx),%rax
    180003a64:	cmp    %rcx,%rax
    180003a67:	jbe    0x180003aa6
    180003a69:	mov    %rax,%rcx
-   180003a6c:	call   0x1800070bc
+   180003a6c:	call   0x18000737c
    180003a71:	mov    %rax,%rcx
    180003a74:	test   %rax,%rax
    180003a77:	je     0x180003a8a
    180003a79:	add    $0x27,%rax
    180003a7d:	and    $0xffffffffffffffe0,%rax
    180003a81:	mov    %rcx,-0x8(%rax)
    180003a85:	add    $0x28,%rsp
    180003a89:	ret
    180003a8a:	call   *0x5928(%rip)        # 0x1800093b8
    180003a90:	int3
    180003a91:	test   %rcx,%rcx
    180003a94:	je     0x180003a9f
    180003a96:	add    $0x28,%rsp
-   180003a9a:	jmp    0x1800070bc
+   180003a9a:	jmp    0x18000737c
    180003a9f:	xor    %eax,%eax
    180003aa1:	add    $0x28,%rsp
    180003aa5:	ret
    180003aa6:	call   0x1800038f0
    180003aab:	int3
    180003aac:	int3
    180003aad:	int3
@@ -5680,29 +5710,29 @@
    180003ac7:	lea    0x0(,%rax,8),%rcx
    180003acf:	cmp    $0x1000,%rcx
    180003ad6:	jb     0x180003b09
    180003ad8:	lea    0x27(%rcx),%rax
    180003adc:	cmp    %rcx,%rax
    180003adf:	jbe    0x180003b1e
    180003ae1:	mov    %rax,%rcx
-   180003ae4:	call   0x1800070bc
+   180003ae4:	call   0x18000737c
    180003ae9:	mov    %rax,%rcx
    180003aec:	test   %rax,%rax
    180003aef:	je     0x180003b02
    180003af1:	add    $0x27,%rax
    180003af5:	and    $0xffffffffffffffe0,%rax
    180003af9:	mov    %rcx,-0x8(%rax)
    180003afd:	add    $0x28,%rsp
    180003b01:	ret
    180003b02:	call   *0x58b0(%rip)        # 0x1800093b8
    180003b08:	int3
    180003b09:	test   %rcx,%rcx
    180003b0c:	je     0x180003b17
    180003b0e:	add    $0x28,%rsp
-   180003b12:	jmp    0x1800070bc
+   180003b12:	jmp    0x18000737c
    180003b17:	xor    %eax,%eax
    180003b19:	add    $0x28,%rsp
    180003b1d:	ret
    180003b1e:	call   0x1800038f0
    180003b23:	int3
    180003b24:	int3
    180003b25:	int3
@@ -5730,15 +5760,15 @@
    180003b52:	ja     0x180003b75
    180003b54:	mov    %rcx,%rdi
    180003b57:	cmp    $0x10,%rbp
    180003b5b:	jb     0x180003b60
    180003b5d:	mov    (%rcx),%rdi
    180003b60:	mov    %rsi,0x10(%rcx)
    180003b64:	mov    %rdi,%rcx
-   180003b67:	call   0x180007fe0
+   180003b67:	call   0x1800082a0
    180003b6c:	movb   $0x0,(%rdi,%rsi,1)
    180003b70:	jmp    0x180003c64
    180003b75:	movabs $0x7fffffffffffffff,%rdi
    180003b7f:	cmp    %rdi,%rsi
    180003b82:	ja     0x180003c81
    180003b88:	mov    %rsi,%rcx
    180003b8b:	mov    %r14,0x40(%rsp)
@@ -5759,49 +5789,49 @@
    180003bbc:	cmp    $0x1000,%rax
    180003bc2:	jb     0x180003bf9
    180003bc4:	lea    0x27(%rax),%rcx
    180003bc8:	cmp    %rax,%rcx
    180003bcb:	jbe    0x180003c87
    180003bd1:	jmp    0x180003bdd
    180003bd3:	movabs $0x8000000000000027,%rcx
-   180003bdd:	call   0x1800070bc
+   180003bdd:	call   0x18000737c
    180003be2:	test   %rax,%rax
    180003be5:	je     0x180003c7a
    180003beb:	lea    0x27(%rax),%r14
    180003bef:	and    $0xffffffffffffffe0,%r14
    180003bf3:	mov    %rax,-0x8(%r14)
    180003bf7:	jmp    0x180003c0e
    180003bf9:	test   %rax,%rax
    180003bfc:	je     0x180003c0b
    180003bfe:	mov    %rax,%rcx
-   180003c01:	call   0x1800070bc
+   180003c01:	call   0x18000737c
    180003c06:	mov    %rax,%r14
    180003c09:	jmp    0x180003c0e
    180003c0b:	xor    %r14d,%r14d
    180003c0e:	mov    %rsi,%r8
    180003c11:	mov    %rsi,0x10(%rbx)
    180003c15:	mov    %r15,%rdx
    180003c18:	mov    %rdi,0x18(%rbx)
    180003c1c:	mov    %r14,%rcx
-   180003c1f:	call   0x180007fda
+   180003c1f:	call   0x18000829a
    180003c24:	movb   $0x0,(%r14,%rsi,1)
    180003c29:	cmp    $0x10,%rbp
    180003c2d:	jb     0x180003c5c
    180003c2f:	mov    (%rbx),%rcx
    180003c32:	lea    0x1(%rbp),%rdx
    180003c36:	cmp    $0x1000,%rdx
    180003c3d:	jb     0x180003c57
    180003c3f:	mov    -0x8(%rcx),%r8
    180003c43:	add    $0x27,%rdx
    180003c47:	sub    %r8,%rcx
    180003c4a:	lea    -0x8(%rcx),%rax
    180003c4e:	cmp    $0x1f,%rax
    180003c52:	ja     0x180003c7a
    180003c54:	mov    %r8,%rcx
-   180003c57:	call   0x1800070f8
+   180003c57:	call   0x1800073b8
    180003c5c:	mov    %r14,(%rbx)
    180003c5f:	mov    0x40(%rsp),%r14
    180003c64:	mov    0x50(%rsp),%rbp
    180003c69:	mov    %rbx,%rax
    180003c6c:	mov    0x48(%rsp),%rbx
    180003c71:	add    $0x20,%rsp
    180003c75:	pop    %r15
@@ -5825,15 +5855,15 @@
    180003ca1:	push   %r12
    180003ca3:	push   %r14
    180003ca5:	push   %r15
    180003ca7:	sub    $0x30,%rsp
    180003cab:	mov    %rdx,%r14
    180003cae:	mov    %rcx,%rbp
    180003cb1:	mov    $0x70,%ecx
-   180003cb6:	call   0x1800070bc
+   180003cb6:	call   0x18000737c
    180003cbb:	mov    %rax,%rbx
    180003cbe:	mov    %rax,0x68(%rsp)
    180003cc3:	xor    %esi,%esi
    180003cc5:	test   %rax,%rax
    180003cc8:	je     0x180003d24
    180003cca:	movups 0x30(%rbp),%xmm1
    180003cce:	movups 0x40(%rbp),%xmm2
@@ -5856,24 +5886,24 @@
    180003d19:	lea    0xa(%rsi),%edx
    180003d1c:	call   0x180003820
    180003d21:	nop
    180003d22:	jmp    0x180003d27
    180003d24:	mov    %rsi,%rbx
    180003d27:	mov    %rbx,0x68(%rsp)
    180003d2c:	mov    $0x18,%ecx
-   180003d31:	call   0x1800070bc
+   180003d31:	call   0x18000737c
    180003d36:	mov    %rax,%rdi
    180003d39:	mov    %rax,0x68(%rsp)
    180003d3e:	test   %rax,%rax
    180003d41:	je     0x180003d67
    180003d43:	xorps  %xmm0,%xmm0
    180003d46:	movups %xmm0,(%rax)
    180003d49:	movl   $0x1,0x8(%rax)
    180003d50:	movl   $0x1,0xc(%rax)
-   180003d57:	lea    0x5ae2(%rip),%rax        # 0x180009840
+   180003d57:	lea    0x5aea(%rip),%rax        # 0x180009848
    180003d5e:	mov    %rax,(%rdi)
    180003d61:	mov    %rbx,0x10(%rdi)
    180003d65:	jmp    0x180003d6a
    180003d67:	mov    %rsi,%rdi
    180003d6a:	mov    %rbx,0x20(%rsp)
    180003d6f:	mov    %rdi,0x28(%rsp)
    180003d74:	add    $0x58,%rbp
@@ -5905,15 +5935,15 @@
    180003dd0:	mov    %r8,%rdx
    180003dd3:	mov    %rsi,%rcx
    180003dd6:	call   0x1800035d0
    180003ddb:	mov    (%rsi),%r15
    180003dde:	mov    %r12,%r8
    180003de1:	mov    %rbp,%rdx
    180003de4:	mov    %r15,%rcx
-   180003de7:	call   0x180007fe0
+   180003de7:	call   0x1800082a0
    180003dec:	lea    (%r15,%r12,1),%rax
    180003df0:	mov    %rax,0x8(%rsi)
    180003df4:	mov    %rbx,(%r14)
    180003df7:	mov    %rdi,0x8(%r14)
    180003dfb:	mov    %r14,%rax
    180003dfe:	mov    0x60(%rsp),%rbx
    180003e03:	mov    0x70(%rsp),%rbp
@@ -5991,15 +6021,15 @@
    180003ef0:	movzbl %r8b,%eax
    180003ef4:	inc    %r8b
    180003ef7:	movsd  (%rcx,%rax,8),%xmm0
    180003efc:	mulsd  (%rdx,%rax,8),%xmm0
    180003f01:	addsd  %xmm0,%xmm1
    180003f05:	cmp    %r9b,%r8b
    180003f08:	jne    0x180003ef0
-   180003f0a:	movsd  0x5a6e(%rip),%xmm0        # 0x180009980
+   180003f0a:	movsd  0x5a7e(%rip),%xmm0        # 0x180009990
    180003f12:	subsd  %xmm1,%xmm0
    180003f16:	ret
    180003f17:	int3
    180003f18:	int3
    180003f19:	int3
    180003f1a:	int3
    180003f1b:	int3
@@ -6037,15 +6067,15 @@
    180003f86:	mov    %rax,%rdx
    180003f89:	lea    0xd0(%rsp),%rcx
    180003f91:	call   0x180002750
    180003f96:	nop
    180003f97:	lea    0xd0(%rsp),%r8
    180003f9f:	lea    0x130(%rsp),%rdx
    180003fa7:	lea    0x28(%rsp),%rcx
-   180003fac:	call   0x180004da0
+   180003fac:	call   0x1800050e0
    180003fb1:	nop
    180003fb2:	xorps  %xmm6,%xmm6
    180003fb5:	movsd  %xmm6,0x48(%rsp)
    180003fbb:	movsd  %xmm6,0x50(%rsp)
    180003fc1:	mov    0x48(%rsp),%rax
    180003fc6:	xorps  %xmm0,%xmm0
    180003fc9:	cmp    0x50(%rsp),%rax
@@ -6084,18 +6114,18 @@
    18000405b:	jne    0x180004050
    18000405d:	jmp    0x180004064
    18000405f:	cmp    %rcx,%rax
    180004062:	jne    0x1800040d6
    180004064:	mov    (%rbx),%r8d
    180004067:	lea    0xb0(%rsp),%rdx
    18000406f:	mov    (%r15),%rcx
-   180004072:	call   0x180006f5e
+   180004072:	call   0x18000721e
    180004077:	lea    0x58(%rsp),%rdx
    18000407c:	lea    0xb0(%rsp),%rcx
-   180004084:	call   0x180006f76
+   180004084:	call   0x180007236
    180004089:	cmpb   $0x0,0x58(%rsp)
    18000408e:	je     0x1800040d1
    180004090:	movw   $0x300,0x20(%rsp)
    180004097:	movzwl 0x20(%rsp),%eax
    18000409c:	mov    %ax,0x24(%rsp)
    1800040a1:	movzbl 0x25(%rsp),%edx
    1800040a6:	movzbl %al,%ecx
@@ -6140,26 +6170,26 @@
    18000414b:	jne    0x180004140
    18000414d:	jmp    0x180004158
    18000414f:	cmp    %rcx,%rax
    180004152:	jne    0x1800041e8
    180004158:	mov    (%rbx),%r8d
    18000415b:	lea    0xb0(%rsp),%rdx
    180004163:	mov    (%r15),%rcx
-   180004166:	call   0x180006f5e
+   180004166:	call   0x18000721e
    18000416b:	mov    (%r15),%rcx
    18000416e:	add    $0x18,%rcx
    180004172:	mov    0x0(%r13),%edx
    180004176:	call   *0x50fc(%rip)        # 0x180009278
    18000417c:	movzbl 0x4(%rbx),%edx
    180004180:	mov    %rax,%r8
    180004183:	lea    0xb0(%rsp),%rcx
-   18000418b:	call   0x180006f70
+   18000418b:	call   0x180007230
    180004190:	lea    0x58(%rsp),%rdx
    180004195:	lea    0xb0(%rsp),%rcx
-   18000419d:	call   0x180006f76
+   18000419d:	call   0x180007236
    1800041a2:	cmpb   $0x0,0x58(%rsp)
    1800041a7:	je     0x1800041e3
    1800041a9:	movw   $0x300,0x24(%rsp)
    1800041b0:	movzwl 0x24(%rsp),%eax
    1800041b5:	mov    %ax,0x20(%rsp)
    1800041ba:	movzbl 0x21(%rsp),%edx
    1800041bf:	movzbl %al,%ecx
@@ -6192,19 +6222,19 @@
    18000423a:	xorps  %xmm0,%xmm0
    18000423d:	ucomisd %xmm6,%xmm0
    180004241:	ja     0x18000424c
    180004243:	xorps  %xmm2,%xmm2
    180004246:	sqrtsd %xmm6,%xmm2
    18000424a:	jmp    0x180004257
    18000424c:	movaps %xmm6,%xmm0
-   18000424f:	call   0x180008004
+   18000424f:	call   0x1800082c4
    180004254:	movaps %xmm0,%xmm2
    180004257:	movaps %xmm2,%xmm1
-   18000425a:	andps  0x572f(%rip),%xmm1        # 0x180009990
-   180004261:	comisd 0x56ff(%rip),%xmm1        # 0x180009968
+   18000425a:	andps  0x573f(%rip),%xmm1        # 0x1800099a0
+   180004261:	comisd 0x570f(%rip),%xmm1        # 0x180009978
    180004269:	jbe    0x180004529
    18000426f:	movups 0x98(%rsp),%xmm0
    180004277:	movups %xmm0,0xb0(%rsp)
    18000427f:	movsd  0xa8(%rsp),%xmm1
    180004288:	movsd  %xmm1,0xc0(%rsp)
    180004291:	movw   $0x300,0x24(%rsp)
    180004298:	movzwl 0x24(%rsp),%eax
@@ -6238,15 +6268,15 @@
    180004320:	mov    -0x8(%rcx),%rcx
    180004324:	sub    %rcx,%rax
    180004327:	add    $0xfffffffffffffff8,%rax
    18000432b:	cmp    $0x1f,%rax
    18000432f:	jbe    0x180004338
    180004331:	call   *0x5081(%rip)        # 0x1800093b8
    180004337:	int3
-   180004338:	call   0x1800070f8
+   180004338:	call   0x1800073b8
    18000433d:	xorps  %xmm0,%xmm0
    180004340:	movdqu %xmm0,0x28(%rsp)
    180004346:	movq   $0x0,0x38(%rsp)
    18000434f:	mov    0xd8(%rsp),%rdi
    180004357:	mov    0xd0(%rsp),%rsi
    18000435f:	test   $0x1,%sil
    180004363:	je     0x1800043a6
@@ -6260,15 +6290,15 @@
    180004389:	sub    %rdi,%rax
    18000438c:	add    $0xfffffffffffffff8,%rax
    180004390:	cmp    $0x1f,%rax
    180004394:	jbe    0x18000439d
    180004396:	call   *0x501c(%rip)        # 0x1800093b8
    18000439c:	int3
    18000439d:	mov    %rdi,%rcx
-   1800043a0:	call   0x1800070f8
+   1800043a0:	call   0x1800073b8
    1800043a5:	nop
    1800043a6:	testb  $0x1,0x130(%rsp)
    1800043ae:	je     0x1800043f5
    1800043b0:	mov    0x140(%rsp),%rax
    1800043b8:	lea    0x0(,%rax,8),%rdx
    1800043c0:	mov    0x138(%rsp),%rcx
    1800043c8:	mov    %rcx,%rax
@@ -6278,15 +6308,15 @@
    1800043d8:	mov    -0x8(%rcx),%rcx
    1800043dc:	sub    %rcx,%rax
    1800043df:	add    $0xfffffffffffffff8,%rax
    1800043e3:	cmp    $0x1f,%rax
    1800043e7:	jbe    0x1800043f0
    1800043e9:	call   *0x4fc9(%rip)        # 0x1800093b8
    1800043ef:	int3
-   1800043f0:	call   0x1800070f8
+   1800043f0:	call   0x1800073b8
    1800043f5:	mov    %r12,%rax
    1800043f8:	jmp    0x1800044fe
    1800043fd:	mov    0x28(%rsp),%rcx
    180004402:	test   %rcx,%rcx
    180004405:	je     0x18000445a
    180004407:	mov    0x38(%rsp),%rax
    18000440c:	sub    %rcx,%rax
@@ -6299,15 +6329,15 @@
    18000442b:	mov    -0x8(%rcx),%rcx
    18000442f:	sub    %rcx,%rax
    180004432:	add    $0xfffffffffffffff8,%rax
    180004436:	cmp    $0x1f,%rax
    18000443a:	jbe    0x180004443
    18000443c:	call   *0x4f76(%rip)        # 0x1800093b8
    180004442:	int3
-   180004443:	call   0x1800070f8
+   180004443:	call   0x1800073b8
    180004448:	xorps  %xmm0,%xmm0
    18000444b:	movdqu %xmm0,0x28(%rsp)
    180004451:	movq   $0x0,0x38(%rsp)
    18000445a:	testb  $0x1,0xd0(%rsp)
    180004462:	je     0x1800044aa
    180004464:	mov    0xe0(%rsp),%rax
    18000446c:	lea    0x0(,%rax,8),%rdx
@@ -6319,15 +6349,15 @@
    18000448c:	mov    -0x8(%rcx),%rcx
    180004490:	sub    %rcx,%rax
    180004493:	add    $0xfffffffffffffff8,%rax
    180004497:	cmp    $0x1f,%rax
    18000449b:	jbe    0x1800044a4
    18000449d:	call   *0x4f15(%rip)        # 0x1800093b8
    1800044a3:	int3
-   1800044a4:	call   0x1800070f8
+   1800044a4:	call   0x1800073b8
    1800044a9:	nop
    1800044aa:	testb  $0x1,0x130(%rsp)
    1800044b2:	je     0x1800044f9
    1800044b4:	mov    0x140(%rsp),%rax
    1800044bc:	lea    0x0(,%rax,8),%rdx
    1800044c4:	mov    0x138(%rsp),%rcx
    1800044cc:	mov    %rcx,%rax
@@ -6337,35 +6367,35 @@
    1800044dc:	mov    -0x8(%rcx),%rcx
    1800044e0:	sub    %rcx,%rax
    1800044e3:	add    $0xfffffffffffffff8,%rax
    1800044e7:	cmp    $0x1f,%rax
    1800044eb:	jbe    0x1800044f4
    1800044ed:	call   *0x4ec5(%rip)        # 0x1800093b8
    1800044f3:	int3
-   1800044f4:	call   0x1800070f8
+   1800044f4:	call   0x1800073b8
    1800044f9:	mov    0x40(%rsp),%rax
    1800044fe:	mov    0x190(%rsp),%rcx
    180004506:	xor    %rsp,%rcx
-   180004509:	call   0x180007240
+   180004509:	call   0x180007500
    18000450e:	movaps 0x1a0(%rsp),%xmm6
    180004516:	add    $0x1b0,%rsp
    18000451d:	pop    %r15
    18000451f:	pop    %r14
    180004521:	pop    %r13
    180004523:	pop    %r12
    180004525:	pop    %rdi
    180004526:	pop    %rsi
    180004527:	pop    %rbx
    180004528:	ret
-   180004529:	lea    0x5330(%rip),%rdx        # 0x180009860
+   180004529:	lea    0x5340(%rip),%rdx        # 0x180009870
    180004530:	lea    0x80(%rsp),%rcx
    180004538:	call   0x180001190
-   18000453d:	lea    0x71e4(%rip),%rdx        # 0x18000b728
+   18000453d:	lea    0x7254(%rip),%rdx        # 0x18000b798
    180004544:	lea    0x80(%rsp),%rcx
-   18000454c:	call   0x180007fd4
+   18000454c:	call   0x180008294
    180004551:	int3
    180004552:	int3
    180004553:	int3
    180004554:	int3
    180004555:	int3
    180004556:	int3
    180004557:	int3
@@ -6397,5106 +6427,5308 @@
    18000458f:	int3
    180004590:	mov    %rbx,0x8(%rsp)
    180004595:	push   %rdi
    180004596:	sub    $0x20,%rsp
    18000459a:	mov    (%rcx),%rax
    18000459d:	mov    %rcx,%rdi
    1800045a0:	mov    %r8d,%ebx
-   1800045a3:	call   *0x78(%rax)
-   1800045a6:	lea    (%rbx,%rbx,4),%rcx
-   1800045aa:	mov    0x30(%rsp),%rbx
-   1800045af:	movups (%rax),%xmm1
-   1800045b2:	movups 0x10(%rax),%xmm2
-   1800045b6:	movsd  0x20(%rax),%xmm0
-   1800045bb:	mov    0x58(%rdi),%rax
-   1800045bf:	movups %xmm1,(%rax,%rcx,8)
-   1800045c3:	movups %xmm2,0x10(%rax,%rcx,8)
-   1800045c8:	movsd  %xmm0,0x20(%rax,%rcx,8)
-   1800045ce:	add    $0x20,%rsp
-   1800045d2:	pop    %rdi
-   1800045d3:	ret
-   1800045d4:	int3
-   1800045d5:	int3
-   1800045d6:	int3
+   1800045a3:	call   *0x80(%rax)
+   1800045a9:	lea    (%rbx,%rbx,4),%rcx
+   1800045ad:	mov    0x30(%rsp),%rbx
+   1800045b2:	movups (%rax),%xmm1
+   1800045b5:	movups 0x10(%rax),%xmm2
+   1800045b9:	movsd  0x20(%rax),%xmm0
+   1800045be:	mov    0x58(%rdi),%rax
+   1800045c2:	movups %xmm1,(%rax,%rcx,8)
+   1800045c6:	movups %xmm2,0x10(%rax,%rcx,8)
+   1800045cb:	movsd  %xmm0,0x20(%rax,%rcx,8)
+   1800045d1:	add    $0x20,%rsp
+   1800045d5:	pop    %rdi
+   1800045d6:	ret
    1800045d7:	int3
    1800045d8:	int3
    1800045d9:	int3
    1800045da:	int3
    1800045db:	int3
    1800045dc:	int3
    1800045dd:	int3
    1800045de:	int3
    1800045df:	int3
-   1800045e0:	mov    %rbx,0x18(%rsp)
-   1800045e5:	mov    %rsi,0x20(%rsp)
-   1800045ea:	push   %r14
-   1800045ec:	sub    $0x50,%rsp
-   1800045f0:	mov    %rdx,%rax
-   1800045f3:	mov    %r8d,%ebx
-   1800045f6:	mov    %rcx,%r14
-   1800045f9:	movl   $0x1,0x20(%rsp)
-   180004601:	mov    %rax,%rcx
-   180004604:	lea    0x9bc5(%rip),%r9        # 0x18000e1d0
-   18000460b:	lea    0x9b8e(%rip),%r8        # 0x18000e1a0
-   180004612:	xor    %edx,%edx
-   180004614:	call   0x180007fb6
-   180004619:	mov    %rax,%rsi
-   18000461c:	movups 0x30(%rax),%xmm0
-   180004620:	movups %xmm0,0x30(%r14)
-   180004625:	movups 0x40(%rax),%xmm1
-   180004629:	movups %xmm1,0x40(%r14)
-   18000462e:	movsd  0x50(%rax),%xmm0
-   180004633:	movsd  %xmm0,0x50(%r14)
-   180004639:	test   %ebx,%ebx
-   18000463b:	je     0x1800046d1
-   180004641:	mov    %ebx,%edx
-   180004643:	lea    0x58(%r14),%rcx
-   180004647:	call   0x180005330
-   18000464c:	movl   $0x0,0x30(%rsp)
-   180004654:	mov    %ebx,0x34(%rsp)
-   180004658:	mov    0x30(%rsp),%rax
-   18000465d:	movsd  0x30(%rsp),%xmm0
-   180004663:	shr    $0x20,%rax
-   180004667:	movsd  %xmm0,0x40(%rsp)
-   18000466d:	test   %eax,%eax
-   18000466f:	je     0x1800046d1
-   180004671:	mov    %rbp,0x60(%rsp)
-   180004676:	mov    0x44(%rsp),%ebp
-   18000467a:	mov    %rdi,0x68(%rsp)
-   18000467f:	mov    0x40(%rsp),%edi
-   180004683:	nopl   0x0(%rax)
-   180004687:	nopw   0x0(%rax,%rax,1)
-   180004690:	mov    %edi,%eax
-   180004692:	mov    %edi,%edx
-   180004694:	lea    (%rax,%rax,4),%rcx
-   180004698:	mov    0x58(%r14),%rax
-   18000469c:	lea    (%rax,%rcx,8),%rbx
-   1800046a0:	mov    (%rsi),%rax
-   1800046a3:	mov    %rsi,%rcx
-   1800046a6:	call   *0x78(%rax)
-   1800046a9:	inc    %edi
-   1800046ab:	movups (%rax),%xmm0
-   1800046ae:	movups %xmm0,(%rbx)
-   1800046b1:	movups 0x10(%rax),%xmm1
-   1800046b5:	movups %xmm1,0x10(%rbx)
-   1800046b9:	movsd  0x20(%rax),%xmm0
-   1800046be:	movsd  %xmm0,0x20(%rbx)
-   1800046c3:	cmp    %ebp,%edi
-   1800046c5:	jne    0x180004690
-   1800046c7:	mov    0x68(%rsp),%rdi
-   1800046cc:	mov    0x60(%rsp),%rbp
-   1800046d1:	mov    0x70(%rsp),%rbx
-   1800046d6:	mov    0x78(%rsp),%rsi
-   1800046db:	add    $0x50,%rsp
-   1800046df:	pop    %r14
-   1800046e1:	ret
-   1800046e2:	int3
-   1800046e3:	int3
-   1800046e4:	int3
-   1800046e5:	int3
-   1800046e6:	int3
-   1800046e7:	int3
-   1800046e8:	int3
-   1800046e9:	int3
-   1800046ea:	int3
-   1800046eb:	int3
-   1800046ec:	int3
-   1800046ed:	int3
-   1800046ee:	int3
-   1800046ef:	int3
-   1800046f0:	sub    $0x28,%rsp
-   1800046f4:	mov    %rdx,%rax
-   1800046f7:	lea    0x0(,%r8,4),%rdx
-   1800046ff:	cmp    $0x1000,%rdx
-   180004706:	jb     0x180004720
-   180004708:	mov    -0x8(%rax),%rcx
-   18000470c:	add    $0x27,%rdx
-   180004710:	sub    %rcx,%rax
-   180004713:	add    $0xfffffffffffffff8,%rax
-   180004717:	cmp    $0x1f,%rax
-   18000471b:	ja     0x18000472c
-   18000471d:	mov    %rcx,%rax
-   180004720:	mov    %rax,%rcx
-   180004723:	add    $0x28,%rsp
-   180004727:	jmp    0x1800070f8
-   18000472c:	call   *0x4c86(%rip)        # 0x1800093b8
-   180004732:	int3
-   180004733:	int3
-   180004734:	int3
-   180004735:	int3
-   180004736:	int3
-   180004737:	int3
-   180004738:	int3
-   180004739:	int3
-   18000473a:	int3
-   18000473b:	int3
-   18000473c:	int3
-   18000473d:	int3
-   18000473e:	int3
-   18000473f:	int3
-   180004740:	sub    $0x28,%rsp
-   180004744:	mov    %rdx,%rax
-   180004747:	imul   $0x58,%r8,%rdx
-   18000474b:	cmp    $0x1000,%rdx
-   180004752:	jb     0x18000476c
-   180004754:	mov    -0x8(%rax),%rcx
-   180004758:	add    $0x27,%rdx
-   18000475c:	sub    %rcx,%rax
-   18000475f:	add    $0xfffffffffffffff8,%rax
-   180004763:	cmp    $0x1f,%rax
-   180004767:	ja     0x180004778
-   180004769:	mov    %rcx,%rax
-   18000476c:	mov    %rax,%rcx
-   18000476f:	add    $0x28,%rsp
-   180004773:	jmp    0x1800070f8
-   180004778:	call   *0x4c3a(%rip)        # 0x1800093b8
-   18000477e:	int3
-   18000477f:	int3
-   180004780:	sub    $0x28,%rsp
-   180004784:	mov    %rdx,%rax
-   180004787:	lea    (%r8,%r8,4),%rdx
-   18000478b:	shl    $0x3,%rdx
-   18000478f:	cmp    $0x1000,%rdx
-   180004796:	jb     0x1800047b0
-   180004798:	mov    -0x8(%rax),%rcx
-   18000479c:	add    $0x27,%rdx
-   1800047a0:	sub    %rcx,%rax
-   1800047a3:	add    $0xfffffffffffffff8,%rax
-   1800047a7:	cmp    $0x1f,%rax
-   1800047ab:	ja     0x1800047bc
-   1800047ad:	mov    %rcx,%rax
-   1800047b0:	mov    %rax,%rcx
-   1800047b3:	add    $0x28,%rsp
-   1800047b7:	jmp    0x1800070f8
-   1800047bc:	call   *0x4bf6(%rip)        # 0x1800093b8
-   1800047c2:	int3
-   1800047c3:	int3
-   1800047c4:	int3
-   1800047c5:	int3
-   1800047c6:	int3
-   1800047c7:	int3
-   1800047c8:	int3
-   1800047c9:	int3
-   1800047ca:	int3
-   1800047cb:	int3
-   1800047cc:	int3
-   1800047cd:	int3
-   1800047ce:	int3
-   1800047cf:	int3
-   1800047d0:	mov    %rdx,%rax
-   1800047d3:	lea    0x58(%rcx),%rdx
-   1800047d7:	mov    %rax,%rcx
-   1800047da:	jmp    0x180001ec0
-   1800047df:	int3
-   1800047e0:	rex push %rbp
-   1800047e2:	push   %rsi
-   1800047e3:	lea    -0x78(%rsp),%rbp
-   1800047e8:	sub    $0x178,%rsp
-   1800047ef:	mov    %rcx,%rsi
-   1800047f2:	movl   $0x0,0x40(%rsp)
-   1800047fa:	mov    (%rcx),%rcx
-   1800047fd:	call   *0x4a95(%rip)        # 0x180009298
-   180004803:	mov    %rax,%rcx
-   180004806:	call   *0x4a94(%rip)        # 0x1800092a0
-   18000480c:	mov    %eax,0x44(%rsp)
-   180004810:	mov    0x40(%rsp),%rax
-   180004815:	movsd  0x40(%rsp),%xmm0
-   18000481b:	shr    $0x20,%rax
-   18000481f:	movsd  %xmm0,0x50(%rsp)
-   180004825:	test   %eax,%eax
-   180004827:	je     0x180004bb8
-   18000482d:	mov    %rdi,0x170(%rsp)
-   180004835:	mov    0x50(%rsp),%edi
-   180004839:	mov    %r12,0x168(%rsp)
-   180004841:	mov    0x54(%rsp),%r12d
-   180004846:	mov    %r13,0x160(%rsp)
-   18000484e:	movaps %xmm10,0x100(%rsp)
-   180004857:	xorps  %xmm10,%xmm10
-   18000485b:	mov    %rbx,0x1a8(%rsp)
-   180004863:	mov    %r14,0x158(%rsp)
-   18000486b:	mov    %r15,0x150(%rsp)
-   180004873:	movaps %xmm6,0x140(%rsp)
-   18000487b:	movaps %xmm7,0x130(%rsp)
-   180004883:	movaps %xmm8,0x120(%rsp)
-   18000488c:	movaps %xmm9,0x110(%rsp)
-   180004895:	data16 data16 nopw 0x0(%rax,%rax,1)
-   1800048a0:	mov    %edi,%edx
-   1800048a2:	mov    %edi,0x90(%rbp)
-   1800048a8:	lea    0x10(%rsi),%rcx
-   1800048ac:	call   0x180006f40
-   1800048b1:	test   %al,%al
-   1800048b3:	je     0x180004b52
-   1800048b9:	mov    (%rsi),%rcx
-   1800048bc:	call   *0x49d6(%rip)        # 0x180009298
-   1800048c2:	mov    %rax,%rcx
-   1800048c5:	mov    %edi,%edx
-   1800048c7:	call   *0x4983(%rip)        # 0x180009250
-   1800048cd:	mov    0x40(%rsi),%rcx
-   1800048d1:	mov    %rax,%r14
-   1800048d4:	mov    (%rax),%edx
-   1800048d6:	mov    (%rcx),%r8
-   1800048d9:	call   *0x78(%r8)
-   1800048dd:	mov    0x40(%rsi),%rcx
-   1800048e1:	mov    0x4(%r14),%edx
-   1800048e5:	movups (%rax),%xmm6
-   1800048e8:	movups 0x10(%rax),%xmm0
-   1800048ec:	movsd  0x20(%rax),%xmm1
-   1800048f1:	mov    (%rcx),%rax
-   1800048f4:	movups %xmm6,-0x28(%rbp)
-   1800048f8:	movups %xmm0,-0x18(%rbp)
-   1800048fc:	movsd  %xmm1,-0x8(%rbp)
-   180004901:	call   *0x78(%rax)
-   180004904:	lea    0x4(%r14),%r9
-   180004908:	mov    %r14,%r8
-   18000490b:	lea    0x60(%rsp),%rdx
-   180004910:	mov    %rsi,%rcx
-   180004913:	movups (%rax),%xmm0
-   180004916:	movups 0x10(%rax),%xmm1
-   18000491a:	movups %xmm0,-0x50(%rbp)
-   18000491e:	movsd  0x20(%rax),%xmm0
-   180004923:	movsd  %xmm0,-0x30(%rbp)
-   180004928:	movups %xmm1,-0x40(%rbp)
-   18000492c:	call   0x180003f20
-   180004931:	mov    %r14,%r9
-   180004934:	lea    0x4(%r14),%r8
-   180004938:	lea    -0x78(%rbp),%rdx
-   18000493c:	mov    %rsi,%rcx
-   18000493f:	call   0x180003f20
-   180004944:	movd   %xmm6,%eax
-   180004948:	test   %al,%al
-   18000494a:	je     0x180004ace
-   180004950:	cmpb   $0x0,-0x50(%rbp)
-   180004954:	je     0x180004ace
-   18000495a:	cmpb   $0x0,0x60(%rsp)
-   18000495f:	je     0x180004ace
-   180004965:	cmpb   $0x0,-0x78(%rbp)
-   180004969:	je     0x180004ace
-   18000496f:	lea    0x68(%rsp),%rdx
-   180004974:	lea    -0x20(%rbp),%rcx
-   180004978:	call   0x180003ed0
-   18000497d:	lea    -0x70(%rbp),%rdx
-   180004981:	movaps %xmm0,%xmm7
-   180004984:	lea    -0x48(%rbp),%rcx
-   180004988:	call   0x180003ed0
-   18000498d:	mov    (%rsi),%rcx
-   180004990:	mov    %r14,%rdx
-   180004993:	movaps %xmm0,%xmm8
-   180004997:	call   *0x48cb(%rip)        # 0x180009268
-   18000499d:	comisd %xmm8,%xmm7
-   1800049a2:	movaps %xmm0,%xmm6
-   1800049a5:	jbe    0x1800049ae
-   1800049a7:	mulsd  %xmm8,%xmm6
-   1800049ac:	jmp    0x1800049b2
-   1800049ae:	mulsd  %xmm7,%xmm6
-   1800049b2:	mov    (%rsi),%rcx
-   1800049b5:	mov    %r14,%rdx
-   1800049b8:	movsd  %xmm6,0xa0(%rbp)
-   1800049c0:	call   *0x48a2(%rip)        # 0x180009268
-   1800049c6:	mov    (%rsi),%rcx
-   1800049c9:	movaps %xmm0,%xmm9
-   1800049cd:	add    $0x18,%rcx
-   1800049d1:	movsd  %xmm0,0x98(%rbp)
-   1800049d9:	comisd %xmm7,%xmm8
-   1800049de:	jbe    0x180004a72
-   1800049e4:	mov    (%r14),%edx
-   1800049e7:	call   *0x488b(%rip)        # 0x180009278
-   1800049ed:	mov    0x28(%rsi),%rdx
-   1800049f1:	cmp    0x30(%rsi),%rdx
-   1800049f5:	je     0x180004a3b
-   1800049f7:	movups (%rax),%xmm1
-   1800049fa:	movsd  0x10(%rax),%xmm0
-   1800049ff:	movsd  %xmm6,0x8(%rdx)
-   180004a04:	movsd  %xmm9,0x10(%rdx)
-   180004a0a:	mov    %edi,(%rdx)
-   180004a0c:	movups %xmm1,0x18(%rdx)
-   180004a10:	movups 0x60(%rsp),%xmm1
-   180004a15:	movsd  %xmm0,0x28(%rdx)
-   180004a1a:	movups 0x70(%rsp),%xmm0
-   180004a1f:	movups %xmm1,0x30(%rdx)
-   180004a23:	movsd  -0x80(%rbp),%xmm1
-   180004a28:	movups %xmm0,0x40(%rdx)
-   180004a2c:	movsd  %xmm1,0x50(%rdx)
-   180004a31:	addq   $0x58,0x28(%rsi)
-   180004a36:	jmp    0x180004b40
-   180004a3b:	lea    0x60(%rsp),%rcx
-   180004a40:	mov    %rcx,0x30(%rsp)
-   180004a45:	lea    0xa0(%rbp),%r9
-   180004a4c:	mov    %rax,0x28(%rsp)
-   180004a51:	lea    0x90(%rbp),%r8
-   180004a58:	lea    0x98(%rbp),%rax
-   180004a5f:	lea    0x20(%rsi),%rcx
-   180004a63:	mov    %rax,0x20(%rsp)
-   180004a68:	call   0x1800015d0
-   180004a6d:	jmp    0x180004b40
-   180004a72:	mov    0x4(%r14),%edx
-   180004a76:	call   *0x47fc(%rip)        # 0x180009278
-   180004a7c:	mov    0x28(%rsi),%rdx
-   180004a80:	cmp    0x30(%rsi),%rdx
-   180004a84:	je     0x180004ac5
-   180004a86:	movups (%rax),%xmm1
-   180004a89:	movsd  0x10(%rax),%xmm0
-   180004a8e:	movups %xmm1,0x18(%rdx)
-   180004a92:	mov    %edi,(%rdx)
-   180004a94:	movups -0x78(%rbp),%xmm1
-   180004a98:	movsd  %xmm0,0x28(%rdx)
-   180004a9d:	movups -0x68(%rbp),%xmm0
-   180004aa1:	movups %xmm1,0x30(%rdx)
-   180004aa5:	movsd  -0x58(%rbp),%xmm1
-   180004aaa:	movups %xmm0,0x40(%rdx)
-   180004aae:	movsd  %xmm1,0x50(%rdx)
-   180004ab3:	movsd  %xmm6,0x8(%rdx)
-   180004ab8:	movsd  %xmm9,0x10(%rdx)
-   180004abe:	addq   $0x58,0x28(%rsi)
-   180004ac3:	jmp    0x180004b40
-   180004ac5:	lea    -0x78(%rbp),%rcx
-   180004ac9:	jmp    0x180004a40
-   180004ace:	mov    (%rsi),%rcx
-   180004ad1:	mov    (%r14),%edx
-   180004ad4:	add    $0x18,%rcx
-   180004ad8:	movl   $0x0,0x98(%rbp)
-   180004ae2:	movl   $0x0,0xa0(%rbp)
-   180004aec:	call   *0x4786(%rip)        # 0x180009278
-   180004af2:	mov    0x28(%rsi),%rdx
-   180004af6:	cmp    0x30(%rsi),%rdx
-   180004afa:	je     0x180004b0e
-   180004afc:	movups (%rax),%xmm1
-   180004aff:	movsd  0x10(%rax),%xmm0
-   180004b04:	movups %xmm10,0x8(%rdx)
-   180004b09:	jmp    0x180004a0a
-   180004b0e:	lea    0x60(%rsp),%rcx
-   180004b13:	mov    %rcx,0x30(%rsp)
-   180004b18:	lea    0xa0(%rbp),%r9
-   180004b1f:	mov    %rax,0x28(%rsp)
-   180004b24:	lea    0x90(%rbp),%r8
-   180004b2b:	lea    0x98(%rbp),%rax
-   180004b32:	lea    0x20(%rsi),%rcx
-   180004b36:	mov    %rax,0x20(%rsp)
-   180004b3b:	call   0x180001850
-   180004b40:	mov    0x28(%rsi),%rdx
-   180004b44:	movzbl 0x38(%rsi),%r8d
-   180004b49:	mov    0x20(%rsi),%rcx
-   180004b4d:	call   0x180002560
-   180004b52:	inc    %edi
-   180004b54:	cmp    %r12d,%edi
-   180004b57:	jne    0x1800048a0
-   180004b5d:	movaps 0x100(%rsp),%xmm10
-   180004b66:	movaps 0x110(%rsp),%xmm9
-   180004b6f:	movaps 0x120(%rsp),%xmm8
-   180004b78:	movaps 0x130(%rsp),%xmm7
-   180004b80:	movaps 0x140(%rsp),%xmm6
-   180004b88:	mov    0x150(%rsp),%r15
-   180004b90:	mov    0x158(%rsp),%r14
-   180004b98:	mov    0x160(%rsp),%r13
-   180004ba0:	mov    0x168(%rsp),%r12
-   180004ba8:	mov    0x170(%rsp),%rdi
-   180004bb0:	mov    0x1a8(%rsp),%rbx
-   180004bb8:	add    $0x178,%rsp
-   180004bbf:	pop    %rsi
-   180004bc0:	pop    %rbp
-   180004bc1:	ret
-   180004bc2:	int3
-   180004bc3:	int3
-   180004bc4:	int3
-   180004bc5:	int3
-   180004bc6:	int3
-   180004bc7:	int3
-   180004bc8:	int3
-   180004bc9:	int3
-   180004bca:	int3
-   180004bcb:	int3
-   180004bcc:	int3
-   180004bcd:	int3
-   180004bce:	int3
-   180004bcf:	int3
-   180004bd0:	mov    %rbx,0x10(%rsp)
-   180004bd5:	mov    %rcx,0x8(%rsp)
-   180004bda:	push   %rbp
-   180004bdb:	push   %rsi
-   180004bdc:	push   %rdi
-   180004bdd:	push   %r12
-   180004bdf:	push   %r13
-   180004be1:	push   %r14
-   180004be3:	push   %r15
-   180004be5:	sub    $0x60,%rsp
-   180004be9:	mov    %r9d,%ebp
-   180004bec:	mov    %r8,%r13
-   180004bef:	mov    %rdx,%r15
-   180004bf2:	mov    %rcx,%rbx
-   180004bf5:	mov    $0x70,%ecx
-   180004bfa:	call   0x1800070bc
-   180004bff:	mov    %rax,%rsi
-   180004c02:	mov    %rax,0xb0(%rsp)
-   180004c0a:	test   %rax,%rax
-   180004c0d:	je     0x180004c6a
-   180004c0f:	movups 0x30(%rbx),%xmm1
-   180004c13:	movups 0x40(%rbx),%xmm2
-   180004c17:	movsd  0x50(%rbx),%xmm0
-   180004c1c:	movzwl 0x8(%rbx),%ecx
-   180004c20:	mov    %cx,0x8(%rax)
-   180004c24:	xor    %ebx,%ebx
-   180004c26:	mov    %rbx,0x10(%rax)
-   180004c2a:	mov    %rbx,0x20(%rax)
-   180004c2e:	movq   $0xf,0x28(%rax)
-   180004c36:	mov    %bl,0x10(%rax)
-   180004c39:	lea    0x4ae8(%rip),%rax        # 0x180009728
-   180004c40:	mov    %rax,(%rsi)
-   180004c43:	movups %xmm1,0x30(%rsi)
-   180004c47:	movups %xmm2,0x40(%rsi)
-   180004c4b:	movsd  %xmm0,0x50(%rsi)
-   180004c50:	lea    0x58(%rsi),%rcx
-   180004c54:	mov    %rbx,(%rcx)
-   180004c57:	mov    %rbx,0x8(%rcx)
-   180004c5b:	mov    %rbx,0x10(%rcx)
-   180004c5f:	lea    0xa(%rbx),%edx
-   180004c62:	call   0x180003820
-   180004c67:	nop
-   180004c68:	jmp    0x180004c6e
-   180004c6a:	xor    %ebx,%ebx
-   180004c6c:	mov    %ebx,%esi
-   180004c6e:	mov    %rsi,0xb0(%rsp)
-   180004c76:	mov    $0x18,%ecx
-   180004c7b:	call   0x1800070bc
-   180004c80:	mov    %rax,%r14
-   180004c83:	mov    %rax,0xb0(%rsp)
-   180004c8b:	test   %rax,%rax
-   180004c8e:	je     0x180004cb4
-   180004c90:	xorps  %xmm0,%xmm0
-   180004c93:	movups %xmm0,(%rax)
-   180004c96:	movl   $0x1,0x8(%rax)
-   180004c9d:	movl   $0x1,0xc(%rax)
-   180004ca4:	lea    0x4b95(%rip),%rax        # 0x180009840
-   180004cab:	mov    %rax,(%r14)
-   180004cae:	mov    %rsi,0x10(%r14)
-   180004cb2:	jmp    0x180004cb7
-   180004cb4:	mov    %rbx,%r14
-   180004cb7:	mov    %rsi,0x48(%rsp)
-   180004cbc:	mov    %r14,0x50(%rsp)
-   180004cc1:	lea    0x58(%rsi),%rcx
-   180004cc5:	mov    %rbp,%rdx
-   180004cc8:	call   0x180005330
-   180004ccd:	mov    0x8(%r13),%rax
-   180004cd1:	mov    %ebx,0x20(%rsp)
-   180004cd5:	mov    %eax,0x24(%rsp)
-   180004cd9:	movsd  0x20(%rsp),%xmm0
-   180004cdf:	movsd  %xmm0,0x30(%rsp)
-   180004ce5:	mov    0x28(%rsp),%eax
-   180004ce9:	mov    %eax,0x38(%rsp)
-   180004ced:	mov    0x20(%rsp),%rax
-   180004cf2:	shr    $0x20,%rax
-   180004cf6:	test   %eax,%eax
-   180004cf8:	je     0x180004d5a
-   180004cfa:	mov    0x0(%r13),%r13
-   180004cfe:	mov    0x34(%rsp),%r12d
-   180004d03:	mov    0x30(%rsp),%ebx
-   180004d07:	nopw   0x0(%rax,%rax,1)
-   180004d10:	mov    %ebx,%eax
-   180004d12:	mov    0x0(%r13,%rax,4),%edi
-   180004d17:	cmp    $0xffffffff,%edi
-   180004d1a:	je     0x180004d53
-   180004d1c:	cmp    %ebp,%edi
-   180004d1e:	jae    0x180004d7c
-   180004d20:	mov    0xa0(%rsp),%rcx
-   180004d28:	mov    (%rcx),%rax
-   180004d2b:	mov    %ebx,%edx
-   180004d2d:	call   *0x78(%rax)
-   180004d30:	movups (%rax),%xmm1
-   180004d33:	movups 0x10(%rax),%xmm2
-   180004d37:	movsd  0x20(%rax),%xmm0
-   180004d3c:	lea    (%rdi,%rdi,4),%rcx
-   180004d40:	mov    0x58(%rsi),%rax
-   180004d44:	movups %xmm1,(%rax,%rcx,8)
-   180004d48:	movups %xmm2,0x10(%rax,%rcx,8)
-   180004d4d:	movsd  %xmm0,0x20(%rax,%rcx,8)
-   180004d53:	inc    %ebx
-   180004d55:	cmp    %r12d,%ebx
-   180004d58:	jne    0x180004d10
-   180004d5a:	mov    %rsi,(%r15)
-   180004d5d:	mov    %r14,0x8(%r15)
-   180004d61:	mov    %r15,%rax
-   180004d64:	mov    0xa8(%rsp),%rbx
-   180004d6c:	add    $0x60,%rsp
-   180004d70:	pop    %r15
-   180004d72:	pop    %r14
-   180004d74:	pop    %r13
-   180004d76:	pop    %r12
-   180004d78:	pop    %rdi
-   180004d79:	pop    %rsi
-   180004d7a:	pop    %rbp
-   180004d7b:	ret
-   180004d7c:	lea    0x487d(%rip),%rdx        # 0x180009600
-   180004d83:	lea    0x30(%rsp),%rcx
-   180004d88:	call   0x180001190
-   180004d8d:	lea    0x6994(%rip),%rdx        # 0x18000b728
-   180004d94:	lea    0x30(%rsp),%rcx
-   180004d99:	call   0x180007fd4
-   180004d9e:	int3
-   180004d9f:	int3
-   180004da0:	mov    %rbx,0x10(%rsp)
-   180004da5:	mov    %rbp,0x18(%rsp)
-   180004daa:	mov    %rcx,0x8(%rsp)
-   180004daf:	push   %rsi
-   180004db0:	push   %rdi
-   180004db1:	push   %r12
-   180004db3:	push   %r14
-   180004db5:	push   %r15
-   180004db7:	sub    $0x30,%rsp
-   180004dbb:	mov    %r8,%r15
-   180004dbe:	mov    %rdx,%rax
-   180004dc1:	mov    %rcx,%rdi
-   180004dc4:	xor    %ecx,%ecx
-   180004dc6:	mov    %ecx,0x20(%rsp)
-   180004dca:	mov    %rcx,(%rdi)
-   180004dcd:	mov    %rcx,0x8(%rdi)
-   180004dd1:	mov    %rcx,0x10(%rdi)
-   180004dd5:	movl   $0x1,0x20(%rsp)
-   180004ddd:	lea    0x8(%rdx),%rcx
-   180004de1:	testb  $0x1,(%rdx)
-   180004de4:	je     0x180004df1
-   180004de6:	mov    (%rcx),%rdx
-   180004de9:	mov    %rdx,%rcx
-   180004dec:	mov    %rdx,%rsi
-   180004def:	jmp    0x180004df7
-   180004df1:	mov    %rcx,%rdx
-   180004df4:	mov    %rcx,%rsi
-   180004df7:	mov    (%rax),%rax
-   180004dfa:	shr    %rax
-   180004dfd:	lea    (%rcx,%rax,8),%r12
-   180004e01:	cmp    %r12,%rdx
-   180004e04:	je     0x180004e69
-   180004e06:	testb  $0x1,(%r15)
-   180004e0a:	je     0x180004e18
-   180004e0c:	mov    0x8(%r15),%rcx
-   180004e10:	mov    %rcx,%rdx
-   180004e13:	mov    %rcx,%rbx
-   180004e16:	jmp    0x180004e24
-   180004e18:	lea    0x8(%r15),%rcx
-   180004e1c:	lea    0x8(%r15),%rdx
-   180004e20:	lea    0x8(%r15),%rbx
-   180004e24:	mov    (%r15),%rax
-   180004e27:	shr    %rax
-   180004e2a:	lea    (%rdx,%rax,8),%rbp
-   180004e2e:	cmp    %rbp,%rcx
-   180004e31:	je     0x180004e60
-   180004e33:	mov    (%rsi),%eax
-   180004e35:	cmp    (%rbx),%eax
-   180004e37:	jne    0x180004e57
-   180004e39:	mov    0x8(%rdi),%rdx
-   180004e3d:	cmp    0x10(%rdi),%rdx
-   180004e41:	je     0x180004e4c
-   180004e43:	mov    %eax,(%rdx)
-   180004e45:	addq   $0x4,0x8(%rdi)
-   180004e4a:	jmp    0x180004e57
-   180004e4c:	mov    %rsi,%r8
-   180004e4f:	mov    %rdi,%rcx
-   180004e52:	call   0x180001490
-   180004e57:	add    $0x8,%rbx
-   180004e5b:	cmp    %rbp,%rbx
-   180004e5e:	jne    0x180004e33
-   180004e60:	add    $0x8,%rsi
-   180004e64:	cmp    %r12,%rsi
-   180004e67:	jne    0x180004e06
-   180004e69:	mov    %rdi,%rax
-   180004e6c:	mov    0x68(%rsp),%rbx
-   180004e71:	mov    0x70(%rsp),%rbp
-   180004e76:	add    $0x30,%rsp
-   180004e7a:	pop    %r15
-   180004e7c:	pop    %r14
-   180004e7e:	pop    %r12
-   180004e80:	pop    %rdi
-   180004e81:	pop    %rsi
-   180004e82:	ret
-   180004e83:	int3
-   180004e84:	int3
-   180004e85:	int3
-   180004e86:	int3
-   180004e87:	int3
-   180004e88:	int3
-   180004e89:	int3
-   180004e8a:	int3
-   180004e8b:	int3
-   180004e8c:	int3
-   180004e8d:	int3
-   180004e8e:	int3
-   180004e8f:	int3
-   180004e90:	sub    $0x28,%rsp
-   180004e94:	mov    (%rcx),%rax
-   180004e97:	call   *0x78(%rax)
-   180004e9a:	xorps  %xmm0,%xmm0
-   180004e9d:	add    $0x28,%rsp
-   180004ea1:	ret
-   180004ea2:	int3
-   180004ea3:	int3
-   180004ea4:	int3
-   180004ea5:	int3
-   180004ea6:	int3
-   180004ea7:	int3
-   180004ea8:	int3
-   180004ea9:	int3
-   180004eaa:	int3
-   180004eab:	int3
-   180004eac:	int3
-   180004ead:	int3
-   180004eae:	int3
-   180004eaf:	int3
-   180004eb0:	mov    %rbx,0x8(%rsp)
-   180004eb5:	push   %rdi
-   180004eb6:	sub    $0x20,%rsp
-   180004eba:	mov    %rcx,%rbx
-   180004ebd:	mov    %rdx,%rcx
-   180004ec0:	call   0x180002680
-   180004ec5:	mov    %rax,%rcx
-   180004ec8:	mov    %rax,%rdi
-   180004ecb:	call   *0x429f(%rip)        # 0x180009170
-   180004ed1:	test   %al,%al
-   180004ed3:	je     0x180004ee8
-   180004ed5:	movq   $0x0,0x68(%rbx)
-   180004edd:	mov    0x30(%rsp),%rbx
-   180004ee2:	add    $0x20,%rsp
-   180004ee6:	pop    %rdi
-   180004ee7:	ret
-   180004ee8:	mov    %rbx,%rcx
-   180004eeb:	mov    %rdi,0x68(%rbx)
-   180004eef:	mov    0x30(%rsp),%rbx
-   180004ef4:	add    $0x20,%rsp
-   180004ef8:	pop    %rdi
-   180004ef9:	rex.W jmp *0x42c8(%rip)        # 0x1800091c8
-   180004f00:	xor    %al,%al
-   180004f02:	ret
-   180004f03:	int3
-   180004f04:	int3
-   180004f05:	int3
-   180004f06:	int3
-   180004f07:	int3
-   180004f08:	int3
-   180004f09:	int3
-   180004f0a:	int3
-   180004f0b:	int3
-   180004f0c:	int3
-   180004f0d:	int3
-   180004f0e:	int3
-   180004f0f:	int3
-   180004f10:	mov    $0x1,%al
-   180004f12:	ret
-   180004f13:	int3
-   180004f14:	int3
-   180004f15:	int3
-   180004f16:	int3
-   180004f17:	int3
-   180004f18:	int3
-   180004f19:	int3
-   180004f1a:	int3
-   180004f1b:	int3
-   180004f1c:	int3
-   180004f1d:	int3
-   180004f1e:	int3
-   180004f1f:	int3
-   180004f20:	mov    %rbx,0x20(%rsp)
-   180004f25:	push   %rdi
-   180004f26:	sub    $0x80,%rsp
-   180004f2d:	mov    0x90d4(%rip),%rax        # 0x18000e008
-   180004f34:	xor    %rsp,%rax
-   180004f37:	mov    %rax,0x78(%rsp)
-   180004f3c:	mov    %edx,%edi
-   180004f3e:	mov    %rcx,%rbx
-   180004f41:	cmp    $0xffffffff,%edx
-   180004f44:	jne    0x180004f4d
-   180004f46:	xor    %eax,%eax
-   180004f48:	jmp    0x1800050a2
-   180004f4d:	mov    0x40(%rcx),%rdx
-   180004f51:	mov    (%rdx),%rax
-   180004f54:	test   %rax,%rax
-   180004f57:	je     0x180004f78
-   180004f59:	mov    0x58(%rcx),%rdx
-   180004f5d:	movslq (%rdx),%r8
-   180004f60:	add    %rax,%r8
-   180004f63:	cmp    %r8,%rax
-   180004f66:	jae    0x180004f78
-   180004f68:	call   *0x4252(%rip)        # 0x1800091c0
-   180004f6e:	mov    %dil,(%rax)
-   180004f71:	mov    %edi,%eax
-   180004f73:	jmp    0x1800050a2
-   180004f78:	cmpq   $0x0,0x80(%rcx)
-   180004f80:	mov    %rsi,0xa0(%rsp)
-   180004f88:	je     0x180005095
-   180004f8e:	mov    0x18(%rcx),%r8
-   180004f92:	lea    0x70(%rcx),%rax
-   180004f96:	cmp    %rax,(%r8)
-   180004f99:	jne    0x180004fbb
-   180004f9b:	mov    0x90(%rcx),%rdx
-   180004fa2:	mov    0x88(%rcx),%rcx
-   180004fa9:	mov    %rcx,(%r8)
-   180004fac:	sub    %ecx,%edx
-   180004fae:	mov    0x38(%rbx),%rax
-   180004fb2:	mov    %rcx,(%rax)
-   180004fb5:	mov    0x50(%rbx),%rax
-   180004fb9:	mov    %edx,(%rax)
-   180004fbb:	mov    0x68(%rbx),%rcx
-   180004fbf:	test   %rcx,%rcx
-   180004fc2:	jne    0x180004fe6
-   180004fc4:	mov    0x80(%rbx),%rdx
-   180004fcb:	movsbl %dil,%ecx
-   180004fcf:	call   *0x448b(%rip)        # 0x180009460
-   180004fd5:	mov    $0xffffffff,%ecx
-   180004fda:	cmp    %ecx,%eax
-   180004fdc:	cmovne %edi,%ecx
-   180004fdf:	mov    %ecx,%eax
-   180004fe1:	jmp    0x18000509a
-   180004fe6:	lea    0x48(%rsp),%rax
-   180004feb:	mov    %dil,0x40(%rsp)
-   180004ff0:	mov    %rax,0x38(%rsp)
-   180004ff5:	lea    0x74(%rbx),%rdx
-   180004ff9:	lea    0x78(%rsp),%rax
-   180004ffe:	mov    %rax,0x30(%rsp)
-   180005003:	lea    0x41(%rsp),%r9
-   180005008:	lea    0x58(%rsp),%rax
-   18000500d:	mov    %rax,0x28(%rsp)
-   180005012:	lea    0x40(%rsp),%r8
-   180005017:	lea    0x50(%rsp),%rax
-   18000501c:	mov    %rax,0x20(%rsp)
-   180005021:	call   *0x4159(%rip)        # 0x180009180
-   180005027:	test   %eax,%eax
-   180005029:	je     0x180005055
-   18000502b:	sub    $0x1,%eax
-   18000502e:	je     0x180005055
-   180005030:	cmp    $0x2,%eax
-   180005033:	jne    0x180005095
-   180005035:	movsbl 0x40(%rsp),%ecx
-   18000503a:	mov    0x80(%rbx),%rdx
-   180005041:	call   *0x4419(%rip)        # 0x180009460
-   180005047:	mov    $0xffffffff,%ecx
-   18000504c:	cmp    %ecx,%eax
-   18000504e:	cmovne %edi,%ecx
-   180005051:	mov    %ecx,%eax
-   180005053:	jmp    0x18000509a
-   180005055:	mov    0x48(%rsp),%rsi
-   18000505a:	lea    0x58(%rsp),%rax
-   18000505f:	sub    %rax,%rsi
-   180005062:	je     0x180005083
-   180005064:	mov    0x80(%rbx),%r9
-   18000506b:	lea    0x58(%rsp),%rcx
-   180005070:	mov    %rsi,%r8
-   180005073:	mov    $0x1,%edx
-   180005078:	call   *0x4392(%rip)        # 0x180009410
-   18000507e:	cmp    %rax,%rsi
-   180005081:	jne    0x180005095
-   180005083:	lea    0x40(%rsp),%rax
-   180005088:	movb   $0x1,0x71(%rbx)
-   18000508c:	cmp    %rax,0x50(%rsp)
-   180005091:	mov    %edi,%eax
-   180005093:	jne    0x18000509a
-   180005095:	mov    $0xffffffff,%eax
-   18000509a:	mov    0xa0(%rsp),%rsi
-   1800050a2:	mov    0x78(%rsp),%rcx
-   1800050a7:	xor    %rsp,%rcx
-   1800050aa:	call   0x180007240
-   1800050af:	mov    0xa8(%rsp),%rbx
-   1800050b7:	add    $0x80,%rsp
-   1800050be:	pop    %rdi
-   1800050bf:	ret
-   1800050c0:	mov    %rbx,0x8(%rsp)
-   1800050c5:	push   %rdi
-   1800050c6:	sub    $0x20,%rsp
-   1800050ca:	mov    0x38(%rcx),%rax
-   1800050ce:	mov    %rcx,%rbx
-   1800050d1:	mov    %edx,%edi
-   1800050d3:	mov    (%rax),%rcx
-   1800050d6:	test   %rcx,%rcx
-   1800050d9:	je     0x180005113
-   1800050db:	mov    0x18(%rbx),%rax
-   1800050df:	cmp    %rcx,(%rax)
-   1800050e2:	jae    0x180005113
-   1800050e4:	cmp    $0xffffffff,%edx
-   1800050e7:	je     0x1800050f1
-   1800050e9:	movzbl -0x1(%rcx),%eax
-   1800050ed:	cmp    %edx,%eax
-   1800050ef:	jne    0x180005113
-   1800050f1:	mov    0x50(%rbx),%rax
-   1800050f5:	incl   (%rax)
-   1800050f7:	mov    0x38(%rbx),%rax
-   1800050fb:	decq   (%rax)
-   1800050fe:	xor    %eax,%eax
-   180005100:	cmp    $0xffffffff,%edi
-   180005103:	cmove  %eax,%edi
-   180005106:	mov    %edi,%eax
-   180005108:	mov    0x30(%rsp),%rbx
-   18000510d:	add    $0x20,%rsp
-   180005111:	pop    %rdi
-   180005112:	ret
-   180005113:	mov    0x80(%rbx),%rdx
-   18000511a:	test   %rdx,%rdx
-   18000511d:	je     0x180005192
-   18000511f:	cmp    $0xffffffff,%edi
-   180005122:	je     0x180005192
-   180005124:	cmpq   $0x0,0x68(%rbx)
-   180005129:	jne    0x18000513a
-   18000512b:	movzbl %dil,%ecx
-   18000512f:	call   *0x42fb(%rip)        # 0x180009430
-   180005135:	cmp    $0xffffffff,%eax
-   180005138:	jne    0x180005106
-   18000513a:	mov    0x38(%rbx),%r8
-   18000513e:	lea    0x70(%rbx),%rdx
-   180005142:	cmp    %rdx,(%r8)
-   180005145:	je     0x180005192
-   180005147:	mov    0x18(%rbx),%r9
-   18000514b:	mov    %dil,(%rdx)
-   18000514e:	mov    (%r9),%rax
-   180005151:	cmp    %rdx,%rax
-   180005154:	je     0x18000516e
-   180005156:	mov    %rax,0x88(%rbx)
-   18000515d:	mov    0x50(%rbx),%rax
-   180005161:	movslq (%rax),%rcx
-   180005164:	add    (%r8),%rcx
-   180005167:	mov    %rcx,0x90(%rbx)
-   18000516e:	mov    %rdx,(%r9)
-   180005171:	mov    %ebx,%ecx
-   180005173:	mov    0x38(%rbx),%rax
-   180005177:	sub    %edx,%ecx
-   180005179:	add    $0x71,%ecx
-   18000517c:	mov    %rdx,(%rax)
-   18000517f:	mov    0x50(%rbx),%rax
-   180005183:	mov    %ecx,(%rax)
-   180005185:	mov    %edi,%eax
-   180005187:	mov    0x30(%rsp),%rbx
-   18000518c:	add    $0x20,%rsp
-   180005190:	pop    %rdi
-   180005191:	ret
-   180005192:	mov    0x30(%rsp),%rbx
-   180005197:	mov    $0xffffffff,%eax
-   18000519c:	add    $0x20,%rsp
-   1800051a0:	pop    %rdi
-   1800051a1:	ret
-   1800051a2:	int3
-   1800051a3:	int3
-   1800051a4:	int3
-   1800051a5:	int3
-   1800051a6:	int3
-   1800051a7:	int3
-   1800051a8:	int3
-   1800051a9:	int3
-   1800051aa:	int3
-   1800051ab:	int3
-   1800051ac:	int3
-   1800051ad:	int3
-   1800051ae:	int3
-   1800051af:	int3
-   1800051b0:	sub    $0x38,%rsp
-   1800051b4:	movups (%rdx),%xmm0
-   1800051b7:	add    $0x58,%rcx
-   1800051bb:	lea    0x20(%rsp),%rdx
-   1800051c0:	movaps %xmm0,0x20(%rsp)
-   1800051c5:	call   0x180002300
-   1800051ca:	add    $0x38,%rsp
-   1800051ce:	ret
+   1800045e0:	rex push %rbx
+   1800045e2:	push   %rsi
+   1800045e3:	push   %r14
+   1800045e5:	sub    $0x50,%rsp
+   1800045e9:	mov    %rdx,%rax
+   1800045ec:	mov    %r8d,%ebx
+   1800045ef:	mov    %rcx,%rsi
+   1800045f2:	movl   $0x1,0x20(%rsp)
+   1800045fa:	mov    %rax,%rcx
+   1800045fd:	lea    0x9bcc(%rip),%r9        # 0x18000e1d0
+   180004604:	lea    0x9b95(%rip),%r8        # 0x18000e1a0
+   18000460b:	xor    %edx,%edx
+   18000460d:	call   0x180008276
+   180004612:	mov    %rax,%r14
+   180004615:	movups 0x30(%rax),%xmm0
+   180004619:	movups %xmm0,0x30(%rsi)
+   18000461d:	movups 0x40(%rax),%xmm1
+   180004621:	movups %xmm1,0x40(%rsi)
+   180004625:	movsd  0x50(%rax),%xmm0
+   18000462a:	movsd  %xmm0,0x50(%rsi)
+   18000462f:	test   %ebx,%ebx
+   180004631:	je     0x180004764
+   180004637:	mov    0x60(%rsi),%r8
+   18000463b:	mov    %ebx,%r9d
+   18000463e:	mov    0x58(%rsi),%r11
+   180004642:	mov    %r8,%rcx
+   180004645:	sub    %r11,%rcx
+   180004648:	mov    %rdi,0x78(%rsp)
+   18000464d:	movabs $0x6666666666666667,%rdi
+   180004657:	mov    %rdi,%rax
+   18000465a:	imul   %rcx
+   18000465d:	mov    %rdx,%r10
+   180004660:	sar    $0x4,%r10
+   180004664:	mov    %r10,%rax
+   180004667:	shr    $0x3f,%rax
+   18000466b:	add    %rax,%r10
+   18000466e:	cmp    %r10,%rbx
+   180004671:	jae    0x180004681
+   180004673:	lea    (%rbx,%rbx,4),%rax
+   180004677:	lea    (%r11,%rax,8),%rcx
+   18000467b:	mov    %rcx,0x60(%rsi)
+   18000467f:	jmp    0x1800046e0
+   180004681:	jbe    0x1800046e0
+   180004683:	mov    0x68(%rsi),%rcx
+   180004687:	mov    %rdi,%rax
+   18000468a:	sub    %r11,%rcx
+   18000468d:	imul   %rcx
+   180004690:	sar    $0x4,%rdx
+   180004694:	mov    %rdx,%rax
+   180004697:	shr    $0x3f,%rax
+   18000469b:	add    %rax,%rdx
+   18000469e:	cmp    %rdx,%r9
+   1800046a1:	jbe    0x1800046b9
+   1800046a3:	lea    0x80(%rsp),%r8
+   1800046ab:	mov    %r9,%rdx
+   1800046ae:	lea    0x58(%rsi),%rcx
+   1800046b2:	call   0x180001c40
+   1800046b7:	jmp    0x1800046e0
+   1800046b9:	sub    %r10,%r9
+   1800046bc:	je     0x1800046dc
+   1800046be:	xchg   %ax,%ax
+   1800046c0:	movb   $0x0,(%r8)
+   1800046c4:	xor    %eax,%eax
+   1800046c6:	xorps  %xmm0,%xmm0
+   1800046c9:	movups %xmm0,0x8(%r8)
+   1800046ce:	mov    %rax,0x18(%r8)
+   1800046d2:	add    $0x28,%r8
+   1800046d6:	sub    $0x1,%r9
+   1800046da:	jne    0x1800046c0
+   1800046dc:	mov    %r8,0x60(%rsi)
+   1800046e0:	movl   $0x0,0x30(%rsp)
+   1800046e8:	mov    %ebx,0x34(%rsp)
+   1800046ec:	mov    0x30(%rsp),%rax
+   1800046f1:	movsd  0x30(%rsp),%xmm0
+   1800046f7:	shr    $0x20,%rax
+   1800046fb:	movsd  %xmm0,0x40(%rsp)
+   180004701:	test   %eax,%eax
+   180004703:	je     0x18000475f
+   180004705:	mov    0x40(%rsp),%edi
+   180004709:	mov    %rbp,0x70(%rsp)
+   18000470e:	mov    0x44(%rsp),%ebp
+   180004712:	nopl   0x0(%rax)
+   180004716:	data16 nopw 0x0(%rax,%rax,1)
+   180004720:	mov    %edi,%eax
+   180004722:	mov    %edi,%edx
+   180004724:	lea    (%rax,%rax,4),%rcx
+   180004728:	mov    0x58(%rsi),%rax
+   18000472c:	lea    (%rax,%rcx,8),%rbx
+   180004730:	mov    (%r14),%rax
+   180004733:	mov    %r14,%rcx
+   180004736:	call   *0x80(%rax)
+   18000473c:	inc    %edi
+   18000473e:	movups (%rax),%xmm0
+   180004741:	movups %xmm0,(%rbx)
+   180004744:	movups 0x10(%rax),%xmm1
+   180004748:	movups %xmm1,0x10(%rbx)
+   18000474c:	movsd  0x20(%rax),%xmm0
+   180004751:	movsd  %xmm0,0x20(%rbx)
+   180004756:	cmp    %ebp,%edi
+   180004758:	jne    0x180004720
+   18000475a:	mov    0x70(%rsp),%rbp
+   18000475f:	mov    0x78(%rsp),%rdi
+   180004764:	add    $0x50,%rsp
+   180004768:	pop    %r14
+   18000476a:	pop    %rsi
+   18000476b:	pop    %rbx
+   18000476c:	ret
+   18000476d:	int3
+   18000476e:	int3
+   18000476f:	int3
+   180004770:	sub    $0x28,%rsp
+   180004774:	mov    %rdx,%rax
+   180004777:	lea    0x0(,%r8,4),%rdx
+   18000477f:	cmp    $0x1000,%rdx
+   180004786:	jb     0x1800047a0
+   180004788:	mov    -0x8(%rax),%rcx
+   18000478c:	add    $0x27,%rdx
+   180004790:	sub    %rcx,%rax
+   180004793:	add    $0xfffffffffffffff8,%rax
+   180004797:	cmp    $0x1f,%rax
+   18000479b:	ja     0x1800047ac
+   18000479d:	mov    %rcx,%rax
+   1800047a0:	mov    %rax,%rcx
+   1800047a3:	add    $0x28,%rsp
+   1800047a7:	jmp    0x1800073b8
+   1800047ac:	call   *0x4c06(%rip)        # 0x1800093b8
+   1800047b2:	int3
+   1800047b3:	int3
+   1800047b4:	int3
+   1800047b5:	int3
+   1800047b6:	int3
+   1800047b7:	int3
+   1800047b8:	int3
+   1800047b9:	int3
+   1800047ba:	int3
+   1800047bb:	int3
+   1800047bc:	int3
+   1800047bd:	int3
+   1800047be:	int3
+   1800047bf:	int3
+   1800047c0:	sub    $0x28,%rsp
+   1800047c4:	mov    %rdx,%rax
+   1800047c7:	imul   $0x58,%r8,%rdx
+   1800047cb:	cmp    $0x1000,%rdx
+   1800047d2:	jb     0x1800047ec
+   1800047d4:	mov    -0x8(%rax),%rcx
+   1800047d8:	add    $0x27,%rdx
+   1800047dc:	sub    %rcx,%rax
+   1800047df:	add    $0xfffffffffffffff8,%rax
+   1800047e3:	cmp    $0x1f,%rax
+   1800047e7:	ja     0x1800047f8
+   1800047e9:	mov    %rcx,%rax
+   1800047ec:	mov    %rax,%rcx
+   1800047ef:	add    $0x28,%rsp
+   1800047f3:	jmp    0x1800073b8
+   1800047f8:	call   *0x4bba(%rip)        # 0x1800093b8
+   1800047fe:	int3
+   1800047ff:	int3
+   180004800:	sub    $0x28,%rsp
+   180004804:	mov    %rdx,%rax
+   180004807:	lea    (%r8,%r8,4),%rdx
+   18000480b:	shl    $0x3,%rdx
+   18000480f:	cmp    $0x1000,%rdx
+   180004816:	jb     0x180004830
+   180004818:	mov    -0x8(%rax),%rcx
+   18000481c:	add    $0x27,%rdx
+   180004820:	sub    %rcx,%rax
+   180004823:	add    $0xfffffffffffffff8,%rax
+   180004827:	cmp    $0x1f,%rax
+   18000482b:	ja     0x18000483c
+   18000482d:	mov    %rcx,%rax
+   180004830:	mov    %rax,%rcx
+   180004833:	add    $0x28,%rsp
+   180004837:	jmp    0x1800073b8
+   18000483c:	call   *0x4b76(%rip)        # 0x1800093b8
+   180004842:	int3
+   180004843:	int3
+   180004844:	int3
+   180004845:	int3
+   180004846:	int3
+   180004847:	int3
+   180004848:	int3
+   180004849:	int3
+   18000484a:	int3
+   18000484b:	int3
+   18000484c:	int3
+   18000484d:	int3
+   18000484e:	int3
+   18000484f:	int3
+   180004850:	mov    %rdx,%rax
+   180004853:	lea    0x58(%rcx),%rdx
+   180004857:	mov    %rax,%rcx
+   18000485a:	jmp    0x180001ec0
+   18000485f:	int3
+   180004860:	rex push %rbp
+   180004862:	push   %rsi
+   180004863:	lea    -0x78(%rsp),%rbp
+   180004868:	sub    $0x178,%rsp
+   18000486f:	mov    %rcx,%rsi
+   180004872:	movl   $0x0,0x40(%rsp)
+   18000487a:	mov    (%rcx),%rcx
+   18000487d:	call   *0x4a15(%rip)        # 0x180009298
+   180004883:	mov    %rax,%rcx
+   180004886:	call   *0x4a14(%rip)        # 0x1800092a0
+   18000488c:	mov    %eax,0x44(%rsp)
+   180004890:	mov    0x40(%rsp),%rax
+   180004895:	movsd  0x40(%rsp),%xmm0
+   18000489b:	shr    $0x20,%rax
+   18000489f:	movsd  %xmm0,0x50(%rsp)
+   1800048a5:	test   %eax,%eax
+   1800048a7:	je     0x180004c3e
+   1800048ad:	mov    %rdi,0x170(%rsp)
+   1800048b5:	mov    0x50(%rsp),%edi
+   1800048b9:	mov    %r12,0x168(%rsp)
+   1800048c1:	mov    0x54(%rsp),%r12d
+   1800048c6:	mov    %r13,0x160(%rsp)
+   1800048ce:	movaps %xmm10,0x100(%rsp)
+   1800048d7:	xorps  %xmm10,%xmm10
+   1800048db:	mov    %rbx,0x1a8(%rsp)
+   1800048e3:	mov    %r14,0x158(%rsp)
+   1800048eb:	mov    %r15,0x150(%rsp)
+   1800048f3:	movaps %xmm6,0x140(%rsp)
+   1800048fb:	movaps %xmm7,0x130(%rsp)
+   180004903:	movaps %xmm8,0x120(%rsp)
+   18000490c:	movaps %xmm9,0x110(%rsp)
+   180004915:	data16 data16 nopw 0x0(%rax,%rax,1)
+   180004920:	mov    %edi,%edx
+   180004922:	mov    %edi,0x90(%rbp)
+   180004928:	lea    0x10(%rsi),%rcx
+   18000492c:	call   0x180007200
+   180004931:	test   %al,%al
+   180004933:	je     0x180004bd8
+   180004939:	mov    (%rsi),%rcx
+   18000493c:	call   *0x4956(%rip)        # 0x180009298
+   180004942:	mov    %rax,%rcx
+   180004945:	mov    %edi,%edx
+   180004947:	call   *0x4903(%rip)        # 0x180009250
+   18000494d:	mov    0x40(%rsi),%rcx
+   180004951:	mov    %rax,%r14
+   180004954:	mov    (%rax),%edx
+   180004956:	mov    (%rcx),%r8
+   180004959:	call   *0x80(%r8)
+   180004960:	mov    0x40(%rsi),%rcx
+   180004964:	mov    0x4(%r14),%edx
+   180004968:	movups (%rax),%xmm6
+   18000496b:	movups 0x10(%rax),%xmm0
+   18000496f:	movsd  0x20(%rax),%xmm1
+   180004974:	mov    (%rcx),%rax
+   180004977:	movups %xmm6,-0x28(%rbp)
+   18000497b:	movups %xmm0,-0x18(%rbp)
+   18000497f:	movsd  %xmm1,-0x8(%rbp)
+   180004984:	call   *0x80(%rax)
+   18000498a:	lea    0x4(%r14),%r9
+   18000498e:	mov    %r14,%r8
+   180004991:	lea    0x60(%rsp),%rdx
+   180004996:	mov    %rsi,%rcx
+   180004999:	movups (%rax),%xmm0
+   18000499c:	movups 0x10(%rax),%xmm1
+   1800049a0:	movups %xmm0,-0x50(%rbp)
+   1800049a4:	movsd  0x20(%rax),%xmm0
+   1800049a9:	movsd  %xmm0,-0x30(%rbp)
+   1800049ae:	movups %xmm1,-0x40(%rbp)
+   1800049b2:	call   0x180003f20
+   1800049b7:	mov    %r14,%r9
+   1800049ba:	lea    0x4(%r14),%r8
+   1800049be:	lea    -0x78(%rbp),%rdx
+   1800049c2:	mov    %rsi,%rcx
+   1800049c5:	call   0x180003f20
+   1800049ca:	movd   %xmm6,%eax
+   1800049ce:	test   %al,%al
+   1800049d0:	je     0x180004b54
+   1800049d6:	cmpb   $0x0,-0x50(%rbp)
+   1800049da:	je     0x180004b54
+   1800049e0:	cmpb   $0x0,0x60(%rsp)
+   1800049e5:	je     0x180004b54
+   1800049eb:	cmpb   $0x0,-0x78(%rbp)
+   1800049ef:	je     0x180004b54
+   1800049f5:	lea    0x68(%rsp),%rdx
+   1800049fa:	lea    -0x20(%rbp),%rcx
+   1800049fe:	call   0x180003ed0
+   180004a03:	lea    -0x70(%rbp),%rdx
+   180004a07:	movaps %xmm0,%xmm7
+   180004a0a:	lea    -0x48(%rbp),%rcx
+   180004a0e:	call   0x180003ed0
+   180004a13:	mov    (%rsi),%rcx
+   180004a16:	mov    %r14,%rdx
+   180004a19:	movaps %xmm0,%xmm8
+   180004a1d:	call   *0x4845(%rip)        # 0x180009268
+   180004a23:	comisd %xmm8,%xmm7
+   180004a28:	movaps %xmm0,%xmm6
+   180004a2b:	jbe    0x180004a34
+   180004a2d:	mulsd  %xmm8,%xmm6
+   180004a32:	jmp    0x180004a38
+   180004a34:	mulsd  %xmm7,%xmm6
+   180004a38:	mov    (%rsi),%rcx
+   180004a3b:	mov    %r14,%rdx
+   180004a3e:	movsd  %xmm6,0xa0(%rbp)
+   180004a46:	call   *0x481c(%rip)        # 0x180009268
+   180004a4c:	mov    (%rsi),%rcx
+   180004a4f:	movaps %xmm0,%xmm9
+   180004a53:	add    $0x18,%rcx
+   180004a57:	movsd  %xmm0,0x98(%rbp)
+   180004a5f:	comisd %xmm7,%xmm8
+   180004a64:	jbe    0x180004af8
+   180004a6a:	mov    (%r14),%edx
+   180004a6d:	call   *0x4805(%rip)        # 0x180009278
+   180004a73:	mov    0x28(%rsi),%rdx
+   180004a77:	cmp    0x30(%rsi),%rdx
+   180004a7b:	je     0x180004ac1
+   180004a7d:	movups (%rax),%xmm1
+   180004a80:	movsd  0x10(%rax),%xmm0
+   180004a85:	movsd  %xmm6,0x8(%rdx)
+   180004a8a:	movsd  %xmm9,0x10(%rdx)
+   180004a90:	mov    %edi,(%rdx)
+   180004a92:	movups %xmm1,0x18(%rdx)
+   180004a96:	movups 0x60(%rsp),%xmm1
+   180004a9b:	movsd  %xmm0,0x28(%rdx)
+   180004aa0:	movups 0x70(%rsp),%xmm0
+   180004aa5:	movups %xmm1,0x30(%rdx)
+   180004aa9:	movsd  -0x80(%rbp),%xmm1
+   180004aae:	movups %xmm0,0x40(%rdx)
+   180004ab2:	movsd  %xmm1,0x50(%rdx)
+   180004ab7:	addq   $0x58,0x28(%rsi)
+   180004abc:	jmp    0x180004bc6
+   180004ac1:	lea    0x60(%rsp),%rcx
+   180004ac6:	mov    %rcx,0x30(%rsp)
+   180004acb:	lea    0xa0(%rbp),%r9
+   180004ad2:	mov    %rax,0x28(%rsp)
+   180004ad7:	lea    0x90(%rbp),%r8
+   180004ade:	lea    0x98(%rbp),%rax
+   180004ae5:	lea    0x20(%rsi),%rcx
+   180004ae9:	mov    %rax,0x20(%rsp)
+   180004aee:	call   0x1800015d0
+   180004af3:	jmp    0x180004bc6
+   180004af8:	mov    0x4(%r14),%edx
+   180004afc:	call   *0x4776(%rip)        # 0x180009278
+   180004b02:	mov    0x28(%rsi),%rdx
+   180004b06:	cmp    0x30(%rsi),%rdx
+   180004b0a:	je     0x180004b4b
+   180004b0c:	movups (%rax),%xmm1
+   180004b0f:	movsd  0x10(%rax),%xmm0
+   180004b14:	movups %xmm1,0x18(%rdx)
+   180004b18:	mov    %edi,(%rdx)
+   180004b1a:	movups -0x78(%rbp),%xmm1
+   180004b1e:	movsd  %xmm0,0x28(%rdx)
+   180004b23:	movups -0x68(%rbp),%xmm0
+   180004b27:	movups %xmm1,0x30(%rdx)
+   180004b2b:	movsd  -0x58(%rbp),%xmm1
+   180004b30:	movups %xmm0,0x40(%rdx)
+   180004b34:	movsd  %xmm1,0x50(%rdx)
+   180004b39:	movsd  %xmm6,0x8(%rdx)
+   180004b3e:	movsd  %xmm9,0x10(%rdx)
+   180004b44:	addq   $0x58,0x28(%rsi)
+   180004b49:	jmp    0x180004bc6
+   180004b4b:	lea    -0x78(%rbp),%rcx
+   180004b4f:	jmp    0x180004ac6
+   180004b54:	mov    (%rsi),%rcx
+   180004b57:	mov    (%r14),%edx
+   180004b5a:	add    $0x18,%rcx
+   180004b5e:	movl   $0x0,0x98(%rbp)
+   180004b68:	movl   $0x0,0xa0(%rbp)
+   180004b72:	call   *0x4700(%rip)        # 0x180009278
+   180004b78:	mov    0x28(%rsi),%rdx
+   180004b7c:	cmp    0x30(%rsi),%rdx
+   180004b80:	je     0x180004b94
+   180004b82:	movups (%rax),%xmm1
+   180004b85:	movsd  0x10(%rax),%xmm0
+   180004b8a:	movups %xmm10,0x8(%rdx)
+   180004b8f:	jmp    0x180004a90
+   180004b94:	lea    0x60(%rsp),%rcx
+   180004b99:	mov    %rcx,0x30(%rsp)
+   180004b9e:	lea    0xa0(%rbp),%r9
+   180004ba5:	mov    %rax,0x28(%rsp)
+   180004baa:	lea    0x90(%rbp),%r8
+   180004bb1:	lea    0x98(%rbp),%rax
+   180004bb8:	lea    0x20(%rsi),%rcx
+   180004bbc:	mov    %rax,0x20(%rsp)
+   180004bc1:	call   0x180001850
+   180004bc6:	mov    0x28(%rsi),%rdx
+   180004bca:	movzbl 0x38(%rsi),%r8d
+   180004bcf:	mov    0x20(%rsi),%rcx
+   180004bd3:	call   0x180002560
+   180004bd8:	inc    %edi
+   180004bda:	cmp    %r12d,%edi
+   180004bdd:	jne    0x180004920
+   180004be3:	movaps 0x100(%rsp),%xmm10
+   180004bec:	movaps 0x110(%rsp),%xmm9
+   180004bf5:	movaps 0x120(%rsp),%xmm8
+   180004bfe:	movaps 0x130(%rsp),%xmm7
+   180004c06:	movaps 0x140(%rsp),%xmm6
+   180004c0e:	mov    0x150(%rsp),%r15
+   180004c16:	mov    0x158(%rsp),%r14
+   180004c1e:	mov    0x160(%rsp),%r13
+   180004c26:	mov    0x168(%rsp),%r12
+   180004c2e:	mov    0x170(%rsp),%rdi
+   180004c36:	mov    0x1a8(%rsp),%rbx
+   180004c3e:	add    $0x178,%rsp
+   180004c45:	pop    %rsi
+   180004c46:	pop    %rbp
+   180004c47:	ret
+   180004c48:	int3
+   180004c49:	int3
+   180004c4a:	int3
+   180004c4b:	int3
+   180004c4c:	int3
+   180004c4d:	int3
+   180004c4e:	int3
+   180004c4f:	int3
+   180004c50:	mov    %rdx,0x10(%rsp)
+   180004c55:	mov    %rcx,0x8(%rsp)
+   180004c5a:	push   %rbx
+   180004c5b:	push   %rbp
+   180004c5c:	push   %rsi
+   180004c5d:	push   %rdi
+   180004c5e:	push   %r12
+   180004c60:	push   %r13
+   180004c62:	push   %r14
+   180004c64:	push   %r15
+   180004c66:	sub    $0x68,%rsp
+   180004c6a:	mov    %r9d,%r12d
+   180004c6d:	mov    %r8,%rsi
+   180004c70:	mov    %rdx,%r15
+   180004c73:	mov    %rcx,%r14
+   180004c76:	mov    $0x70,%ecx
+   180004c7b:	call   0x18000737c
+   180004c80:	mov    %rax,%rdi
+   180004c83:	mov    %rax,0xc0(%rsp)
+   180004c8b:	mov    %rax,0x30(%rsp)
+   180004c90:	xor    %ebp,%ebp
+   180004c92:	test   %rax,%rax
+   180004c95:	je     0x180004cf5
+   180004c97:	movups 0x30(%r14),%xmm1
+   180004c9c:	movups 0x40(%r14),%xmm2
+   180004ca1:	movsd  0x50(%r14),%xmm0
+   180004ca7:	movzwl 0x8(%r14),%eax
+   180004cac:	mov    %ax,0x8(%rdi)
+   180004cb0:	mov    %rbp,0x10(%rdi)
+   180004cb4:	mov    %rbp,0x20(%rdi)
+   180004cb8:	movq   $0xf,0x28(%rdi)
+   180004cc0:	mov    %bpl,0x10(%rdi)
+   180004cc4:	lea    0x4a5d(%rip),%rax        # 0x180009728
+   180004ccb:	mov    %rax,(%rdi)
+   180004cce:	movups %xmm1,0x30(%rdi)
+   180004cd2:	movups %xmm2,0x40(%rdi)
+   180004cd6:	movsd  %xmm0,0x50(%rdi)
+   180004cdb:	lea    0x58(%rdi),%rcx
+   180004cdf:	mov    %rbp,(%rcx)
+   180004ce2:	mov    %rbp,0x8(%rcx)
+   180004ce6:	mov    %rbp,0x10(%rcx)
+   180004cea:	lea    0xa(%rbp),%edx
+   180004ced:	call   0x180003820
+   180004cf2:	nop
+   180004cf3:	jmp    0x180004d00
+   180004cf5:	mov    %rbp,%rdi
+   180004cf8:	mov    %rbp,0xc0(%rsp)
+   180004d00:	mov    %rdi,0x30(%rsp)
+   180004d05:	mov    $0x18,%ecx
+   180004d0a:	call   0x18000737c
+   180004d0f:	mov    %rax,0x20(%rsp)
+   180004d14:	test   %rax,%rax
+   180004d17:	je     0x180004d3d
+   180004d19:	xorps  %xmm0,%xmm0
+   180004d1c:	movups %xmm0,(%rax)
+   180004d1f:	movl   $0x1,0x8(%rax)
+   180004d26:	movl   $0x1,0xc(%rax)
+   180004d2d:	lea    0x4b14(%rip),%rcx        # 0x180009848
+   180004d34:	mov    %rcx,(%rax)
+   180004d37:	mov    %rdi,0x10(%rax)
+   180004d3b:	jmp    0x180004d45
+   180004d3d:	mov    %rbp,%rax
+   180004d40:	mov    %rax,0x20(%rsp)
+   180004d45:	mov    %rdi,0x38(%rsp)
+   180004d4a:	mov    %rax,0x40(%rsp)
+   180004d4f:	lea    0x58(%rdi),%rax
+   180004d53:	mov    %rax,0x28(%rsp)
+   180004d58:	mov    %r12,%rdx
+   180004d5b:	lea    0x30(%r14),%r8
+   180004d5f:	mov    %rax,%rcx
+   180004d62:	call   0x1800055d0
+   180004d67:	mov    0x8(%rsi),%rdi
+   180004d6b:	mov    (%rsi),%r8
+   180004d6e:	mov    %r8,%rdx
+   180004d71:	mov    %r8,%rbx
+   180004d74:	cmpb   $0xff,(%r8)
+   180004d78:	jge    0x180004db7
+   180004d7a:	movdqa 0x4c2e(%rip),%xmm2        # 0x1800099b0
+   180004d82:	nopl   0x0(%rax)
+   180004d86:	data16 nopw 0x0(%rax,%rax,1)
+   180004d90:	movdqu (%rdx),%xmm0
+   180004d94:	movdqa %xmm2,%xmm1
+   180004d98:	pcmpgtb %xmm0,%xmm1
+   180004d9c:	pmovmskb %xmm1,%eax
+   180004da0:	inc    %eax
+   180004da2:	bsf    %eax,%ecx
+   180004da5:	add    %rcx,%rdx
+   180004da8:	mov    %rdx,%rbx
+   180004dab:	shl    $0x5,%rcx
+   180004daf:	add    %rcx,%rdi
+   180004db2:	cmpb   $0xff,(%rdx)
+   180004db5:	jl     0x180004d90
+   180004db7:	add    0x18(%rsi),%r8
+   180004dbb:	mov    %r8,0x30(%rsp)
+   180004dc0:	cmp    %r8,%rbx
+   180004dc3:	je     0x180004ea8
+   180004dc9:	mov    %rdi,%r15
+   180004dcc:	nopl   0x0(%rax)
+   180004dd0:	lea    0x10(%r15),%rcx
+   180004dd4:	testb  $0x1,0x8(%r15)
+   180004dd9:	je     0x180004de6
+   180004ddb:	mov    (%rcx),%rdx
+   180004dde:	mov    %rdx,%rcx
+   180004de1:	mov    %rdx,%r14
+   180004de4:	jmp    0x180004dec
+   180004de6:	mov    %rcx,%rdx
+   180004de9:	mov    %rcx,%r14
+   180004dec:	mov    0x8(%r15),%rax
+   180004df0:	shr    %rax
+   180004df3:	lea    (%rcx,%rax,4),%r13
+   180004df7:	cmp    %r13,%rdx
+   180004dfa:	je     0x180004e55
+   180004dfc:	nopl   0x0(%rax)
+   180004e00:	mov    (%r14),%esi
+   180004e03:	cmp    %r12d,%esi
+   180004e06:	jae    0x180004ed0
+   180004e0c:	mov    0xb0(%rsp),%rcx
+   180004e14:	mov    (%rcx),%rax
+   180004e17:	mov    (%r15),%edx
+   180004e1a:	call   *0x80(%rax)
+   180004e20:	movups (%rax),%xmm1
+   180004e23:	movups 0x10(%rax),%xmm2
+   180004e27:	movsd  0x20(%rax),%xmm0
+   180004e2c:	lea    (%rsi,%rsi,4),%rcx
+   180004e30:	mov    0x28(%rsp),%rax
+   180004e35:	mov    (%rax),%rax
+   180004e38:	movups %xmm1,(%rax,%rcx,8)
+   180004e3c:	movups %xmm2,0x10(%rax,%rcx,8)
+   180004e41:	movsd  %xmm0,0x20(%rax,%rcx,8)
+   180004e47:	add    $0x4,%r14
+   180004e4b:	cmp    %r13,%r14
+   180004e4e:	jne    0x180004e00
+   180004e50:	mov    0x30(%rsp),%r8
+   180004e55:	inc    %rbx
+   180004e58:	add    $0x20,%rdi
+   180004e5c:	cmpb   $0xff,(%rbx)
+   180004e5f:	jge    0x180004e94
+   180004e61:	movdqa 0x4b47(%rip),%xmm2        # 0x1800099b0
+   180004e69:	nopl   0x0(%rax)
+   180004e70:	movdqu (%rbx),%xmm0
+   180004e74:	movdqa %xmm2,%xmm1
+   180004e78:	pcmpgtb %xmm0,%xmm1
+   180004e7c:	pmovmskb %xmm1,%eax
+   180004e80:	inc    %eax
+   180004e82:	bsf    %eax,%ecx
+   180004e85:	add    %rcx,%rbx
+   180004e88:	shl    $0x5,%rcx
+   180004e8c:	add    %rcx,%rdi
+   180004e8f:	cmpb   $0xff,(%rbx)
+   180004e92:	jl     0x180004e70
+   180004e94:	mov    %rdi,%r15
+   180004e97:	cmp    %r8,%rbx
+   180004e9a:	jne    0x180004dd0
+   180004ea0:	mov    0xb8(%rsp),%r15
+   180004ea8:	mov    0xc0(%rsp),%rax
+   180004eb0:	mov    %rax,(%r15)
+   180004eb3:	mov    0x20(%rsp),%rax
+   180004eb8:	mov    %rax,0x8(%r15)
+   180004ebc:	mov    %r15,%rax
+   180004ebf:	add    $0x68,%rsp
+   180004ec3:	pop    %r15
+   180004ec5:	pop    %r14
+   180004ec7:	pop    %r13
+   180004ec9:	pop    %r12
+   180004ecb:	pop    %rdi
+   180004ecc:	pop    %rsi
+   180004ecd:	pop    %rbp
+   180004ece:	pop    %rbx
+   180004ecf:	ret
+   180004ed0:	lea    0x4729(%rip),%rdx        # 0x180009600
+   180004ed7:	lea    0x48(%rsp),%rcx
+   180004edc:	call   0x180001190
+   180004ee1:	lea    0x68b0(%rip),%rdx        # 0x18000b798
+   180004ee8:	lea    0x48(%rsp),%rcx
+   180004eed:	call   0x180008294
+   180004ef2:	int3
+   180004ef3:	int3
+   180004ef4:	int3
+   180004ef5:	int3
+   180004ef6:	int3
+   180004ef7:	int3
+   180004ef8:	int3
+   180004ef9:	int3
+   180004efa:	int3
+   180004efb:	int3
+   180004efc:	int3
+   180004efd:	int3
+   180004efe:	int3
+   180004eff:	int3
+   180004f00:	mov    %rbx,0x10(%rsp)
+   180004f05:	mov    %rcx,0x8(%rsp)
+   180004f0a:	push   %rbp
+   180004f0b:	push   %rsi
+   180004f0c:	push   %rdi
+   180004f0d:	push   %r12
+   180004f0f:	push   %r13
+   180004f11:	push   %r14
+   180004f13:	push   %r15
+   180004f15:	sub    $0x60,%rsp
+   180004f19:	mov    %r9d,%ebp
+   180004f1c:	mov    %r8,%r13
+   180004f1f:	mov    %rdx,%r15
+   180004f22:	mov    %rcx,%r14
+   180004f25:	mov    $0x70,%ecx
+   180004f2a:	call   0x18000737c
+   180004f2f:	mov    %rax,%rsi
+   180004f32:	mov    %rax,0xb0(%rsp)
+   180004f3a:	lea    0x30(%r14),%rdi
+   180004f3e:	xor    %ebx,%ebx
+   180004f40:	test   %rax,%rax
+   180004f43:	je     0x180004f9e
+   180004f45:	movups (%rdi),%xmm1
+   180004f48:	movups 0x10(%rdi),%xmm2
+   180004f4c:	movsd  0x20(%rdi),%xmm0
+   180004f51:	movzwl 0x8(%r14),%eax
+   180004f56:	mov    %ax,0x8(%rsi)
+   180004f5a:	mov    %rbx,0x10(%rsi)
+   180004f5e:	mov    %rbx,0x20(%rsi)
+   180004f62:	movq   $0xf,0x28(%rsi)
+   180004f6a:	mov    %bl,0x10(%rsi)
+   180004f6d:	lea    0x47b4(%rip),%rax        # 0x180009728
+   180004f74:	mov    %rax,(%rsi)
+   180004f77:	movups %xmm1,0x30(%rsi)
+   180004f7b:	movups %xmm2,0x40(%rsi)
+   180004f7f:	movsd  %xmm0,0x50(%rsi)
+   180004f84:	lea    0x58(%rsi),%rcx
+   180004f88:	mov    %rbx,(%rcx)
+   180004f8b:	mov    %rbx,0x8(%rcx)
+   180004f8f:	mov    %rbx,0x10(%rcx)
+   180004f93:	lea    0xa(%rbx),%edx
+   180004f96:	call   0x180003820
+   180004f9b:	nop
+   180004f9c:	jmp    0x180004fa1
+   180004f9e:	mov    %rbx,%rsi
+   180004fa1:	mov    %rsi,0xb0(%rsp)
+   180004fa9:	mov    $0x18,%ecx
+   180004fae:	call   0x18000737c
+   180004fb3:	mov    %rax,%r14
+   180004fb6:	mov    %rax,0xb0(%rsp)
+   180004fbe:	test   %rax,%rax
+   180004fc1:	je     0x180004fe7
+   180004fc3:	xorps  %xmm0,%xmm0
+   180004fc6:	movups %xmm0,(%rax)
+   180004fc9:	movl   $0x1,0x8(%rax)
+   180004fd0:	movl   $0x1,0xc(%rax)
+   180004fd7:	lea    0x486a(%rip),%rax        # 0x180009848
+   180004fde:	mov    %rax,(%r14)
+   180004fe1:	mov    %rsi,0x10(%r14)
+   180004fe5:	jmp    0x180004fea
+   180004fe7:	mov    %rbx,%r14
+   180004fea:	mov    %rsi,0x48(%rsp)
+   180004fef:	mov    %r14,0x50(%rsp)
+   180004ff4:	lea    0x58(%rsi),%rcx
+   180004ff8:	mov    %rbp,%rdx
+   180004ffb:	mov    %rdi,%r8
+   180004ffe:	call   0x1800055d0
+   180005003:	mov    0x8(%r13),%rax
+   180005007:	mov    %ebx,0x20(%rsp)
+   18000500b:	mov    %eax,0x24(%rsp)
+   18000500f:	movsd  0x20(%rsp),%xmm0
+   180005015:	movsd  %xmm0,0x30(%rsp)
+   18000501b:	mov    0x28(%rsp),%eax
+   18000501f:	mov    %eax,0x38(%rsp)
+   180005023:	mov    0x20(%rsp),%rax
+   180005028:	shr    $0x20,%rax
+   18000502c:	test   %eax,%eax
+   18000502e:	je     0x18000508d
+   180005030:	mov    0x0(%r13),%r13
+   180005034:	mov    0x34(%rsp),%r12d
+   180005039:	mov    0x30(%rsp),%ebx
+   18000503d:	nopl   (%rax)
+   180005040:	mov    %ebx,%eax
+   180005042:	mov    0x0(%r13,%rax,4),%edi
+   180005047:	cmp    $0xffffffff,%edi
+   18000504a:	je     0x180005086
+   18000504c:	cmp    %ebp,%edi
+   18000504e:	jae    0x1800050af
+   180005050:	mov    0xa0(%rsp),%rcx
+   180005058:	mov    (%rcx),%rax
+   18000505b:	mov    %ebx,%edx
+   18000505d:	call   *0x80(%rax)
+   180005063:	movups (%rax),%xmm1
+   180005066:	movups 0x10(%rax),%xmm2
+   18000506a:	movsd  0x20(%rax),%xmm0
+   18000506f:	lea    (%rdi,%rdi,4),%rcx
+   180005073:	mov    0x58(%rsi),%rax
+   180005077:	movups %xmm1,(%rax,%rcx,8)
+   18000507b:	movups %xmm2,0x10(%rax,%rcx,8)
+   180005080:	movsd  %xmm0,0x20(%rax,%rcx,8)
+   180005086:	inc    %ebx
+   180005088:	cmp    %r12d,%ebx
+   18000508b:	jne    0x180005040
+   18000508d:	mov    %rsi,(%r15)
+   180005090:	mov    %r14,0x8(%r15)
+   180005094:	mov    %r15,%rax
+   180005097:	mov    0xa8(%rsp),%rbx
+   18000509f:	add    $0x60,%rsp
+   1800050a3:	pop    %r15
+   1800050a5:	pop    %r14
+   1800050a7:	pop    %r13
+   1800050a9:	pop    %r12
+   1800050ab:	pop    %rdi
+   1800050ac:	pop    %rsi
+   1800050ad:	pop    %rbp
+   1800050ae:	ret
+   1800050af:	lea    0x454a(%rip),%rdx        # 0x180009600
+   1800050b6:	lea    0x30(%rsp),%rcx
+   1800050bb:	call   0x180001190
+   1800050c0:	lea    0x66d1(%rip),%rdx        # 0x18000b798
+   1800050c7:	lea    0x30(%rsp),%rcx
+   1800050cc:	call   0x180008294
+   1800050d1:	int3
+   1800050d2:	int3
+   1800050d3:	int3
+   1800050d4:	int3
+   1800050d5:	int3
+   1800050d6:	int3
+   1800050d7:	int3
+   1800050d8:	int3
+   1800050d9:	int3
+   1800050da:	int3
+   1800050db:	int3
+   1800050dc:	int3
+   1800050dd:	int3
+   1800050de:	int3
+   1800050df:	int3
+   1800050e0:	mov    %rbx,0x10(%rsp)
+   1800050e5:	mov    %rbp,0x18(%rsp)
+   1800050ea:	mov    %rcx,0x8(%rsp)
+   1800050ef:	push   %rsi
+   1800050f0:	push   %rdi
+   1800050f1:	push   %r12
+   1800050f3:	push   %r14
+   1800050f5:	push   %r15
+   1800050f7:	sub    $0x30,%rsp
+   1800050fb:	mov    %r8,%r15
+   1800050fe:	mov    %rdx,%rax
+   180005101:	mov    %rcx,%rdi
+   180005104:	xor    %ecx,%ecx
+   180005106:	mov    %ecx,0x20(%rsp)
+   18000510a:	mov    %rcx,(%rdi)
+   18000510d:	mov    %rcx,0x8(%rdi)
+   180005111:	mov    %rcx,0x10(%rdi)
+   180005115:	movl   $0x1,0x20(%rsp)
+   18000511d:	lea    0x8(%rdx),%rcx
+   180005121:	testb  $0x1,(%rdx)
+   180005124:	je     0x180005131
+   180005126:	mov    (%rcx),%rdx
+   180005129:	mov    %rdx,%rcx
+   18000512c:	mov    %rdx,%rsi
+   18000512f:	jmp    0x180005137
+   180005131:	mov    %rcx,%rdx
+   180005134:	mov    %rcx,%rsi
+   180005137:	mov    (%rax),%rax
+   18000513a:	shr    %rax
+   18000513d:	lea    (%rcx,%rax,8),%r12
+   180005141:	cmp    %r12,%rdx
+   180005144:	je     0x1800051a9
+   180005146:	testb  $0x1,(%r15)
+   18000514a:	je     0x180005158
+   18000514c:	mov    0x8(%r15),%rcx
+   180005150:	mov    %rcx,%rdx
+   180005153:	mov    %rcx,%rbx
+   180005156:	jmp    0x180005164
+   180005158:	lea    0x8(%r15),%rcx
+   18000515c:	lea    0x8(%r15),%rdx
+   180005160:	lea    0x8(%r15),%rbx
+   180005164:	mov    (%r15),%rax
+   180005167:	shr    %rax
+   18000516a:	lea    (%rdx,%rax,8),%rbp
+   18000516e:	cmp    %rbp,%rcx
+   180005171:	je     0x1800051a0
+   180005173:	mov    (%rsi),%eax
+   180005175:	cmp    (%rbx),%eax
+   180005177:	jne    0x180005197
+   180005179:	mov    0x8(%rdi),%rdx
+   18000517d:	cmp    0x10(%rdi),%rdx
+   180005181:	je     0x18000518c
+   180005183:	mov    %eax,(%rdx)
+   180005185:	addq   $0x4,0x8(%rdi)
+   18000518a:	jmp    0x180005197
+   18000518c:	mov    %rsi,%r8
+   18000518f:	mov    %rdi,%rcx
+   180005192:	call   0x180001490
+   180005197:	add    $0x8,%rbx
+   18000519b:	cmp    %rbp,%rbx
+   18000519e:	jne    0x180005173
+   1800051a0:	add    $0x8,%rsi
+   1800051a4:	cmp    %r12,%rsi
+   1800051a7:	jne    0x180005146
+   1800051a9:	mov    %rdi,%rax
+   1800051ac:	mov    0x68(%rsp),%rbx
+   1800051b1:	mov    0x70(%rsp),%rbp
+   1800051b6:	add    $0x30,%rsp
+   1800051ba:	pop    %r15
+   1800051bc:	pop    %r14
+   1800051be:	pop    %r12
+   1800051c0:	pop    %rdi
+   1800051c1:	pop    %rsi
+   1800051c2:	ret
+   1800051c3:	int3
+   1800051c4:	int3
+   1800051c5:	int3
+   1800051c6:	int3
+   1800051c7:	int3
+   1800051c8:	int3
+   1800051c9:	int3
+   1800051ca:	int3
+   1800051cb:	int3
+   1800051cc:	int3
+   1800051cd:	int3
+   1800051ce:	int3
    1800051cf:	int3
-   1800051d0:	mov    0x68(%rcx),%r8
-   1800051d4:	add    $0x58,%rcx
-   1800051d8:	mov    %edx,%r9d
-   1800051db:	movabs $0x6666666666666667,%rax
-   1800051e5:	sub    (%rcx),%r8
-   1800051e8:	imul   %r8
-   1800051eb:	sar    $0x4,%rdx
-   1800051ef:	mov    %rdx,%rax
-   1800051f2:	shr    $0x3f,%rax
-   1800051f6:	add    %rax,%rdx
-   1800051f9:	cmp    %rdx,%r9
-   1800051fc:	jbe    0x180005206
-   1800051fe:	mov    %r9d,%edx
-   180005201:	jmp    0x180003820
-   180005206:	ret
-   180005207:	int3
-   180005208:	int3
-   180005209:	int3
-   18000520a:	int3
-   18000520b:	int3
-   18000520c:	int3
-   18000520d:	int3
-   18000520e:	int3
-   18000520f:	int3
-   180005210:	mov    %rbx,0x8(%rsp)
-   180005215:	mov    %rbp,0x10(%rsp)
-   18000521a:	mov    %rsi,0x18(%rsp)
-   18000521f:	push   %rdi
-   180005220:	sub    $0x20,%rsp
-   180005224:	mov    0x68(%rcx),%r8
-   180005228:	movabs $0x6666666666666667,%rbp
-   180005232:	sub    0x58(%rcx),%r8
-   180005236:	mov    %rbp,%rax
-   180005239:	mov    %edx,%r9d
-   18000523c:	mov    %rcx,%rsi
-   18000523f:	imul   %r8
-   180005242:	mov    %r9d,%ebx
-   180005245:	sar    $0x4,%rdx
-   180005249:	mov    %rdx,%rax
-   18000524c:	shr    $0x3f,%rax
-   180005250:	add    %rax,%rdx
-   180005253:	cmp    %rdx,%r9
-   180005256:	jbe    0x180005275
-   180005258:	lea    (%rdx,%rdx,1),%eax
-   18000525b:	cmp    %eax,%r9d
-   18000525e:	cmovb  %eax,%r9d
-   180005262:	mov    %r9d,%eax
-   180005265:	cmp    %rdx,%rax
-   180005268:	jbe    0x180005275
-   18000526a:	mov    %eax,%edx
-   18000526c:	add    $0x58,%rcx
-   180005270:	call   0x180003820
-   180005275:	mov    0x60(%rsi),%rcx
-   180005279:	lea    0x30(%rsi),%r8
-   18000527d:	mov    0x58(%rsi),%r11
-   180005281:	mov    %rcx,%rdx
-   180005284:	sub    %r11,%rdx
-   180005287:	mov    %rbp,%rax
-   18000528a:	imul   %rdx
-   18000528d:	mov    %rdx,%r10
-   180005290:	sar    $0x4,%r10
-   180005294:	mov    %r10,%rax
-   180005297:	shr    $0x3f,%rax
-   18000529b:	add    %rax,%r10
-   18000529e:	cmp    %r10,%rbx
-   1800052a1:	jae    0x1800052ad
-   1800052a3:	lea    (%rbx,%rbx,4),%rax
-   1800052a7:	lea    (%r11,%rax,8),%rcx
-   1800052ab:	jmp    0x180005315
-   1800052ad:	jbe    0x180005319
-   1800052af:	mov    0x68(%rsi),%r9
-   1800052b3:	mov    %rbp,%rax
-   1800052b6:	sub    %r11,%r9
-   1800052b9:	imul   %r9
-   1800052bc:	sar    $0x4,%rdx
-   1800052c0:	mov    %rdx,%rax
-   1800052c3:	shr    $0x3f,%rax
-   1800052c7:	add    %rax,%rdx
-   1800052ca:	cmp    %rdx,%rbx
-   1800052cd:	jbe    0x1800052dd
-   1800052cf:	mov    %rbx,%rdx
-   1800052d2:	lea    0x58(%rsi),%rcx
-   1800052d6:	call   0x180001d80
-   1800052db:	jmp    0x180005319
-   1800052dd:	sub    %r10,%rbx
-   1800052e0:	je     0x180005315
-   1800052e2:	nopl   0x0(%rax)
-   1800052e6:	data16 nopw 0x0(%rax,%rax,1)
-   1800052f0:	movups (%r8),%xmm0
-   1800052f4:	movups %xmm0,(%rcx)
-   1800052f7:	movups 0x10(%r8),%xmm1
-   1800052fc:	movups %xmm1,0x10(%rcx)
-   180005300:	movsd  0x20(%r8),%xmm0
-   180005306:	movsd  %xmm0,0x20(%rcx)
-   18000530b:	add    $0x28,%rcx
-   18000530f:	sub    $0x1,%rbx
-   180005313:	jne    0x1800052f0
-   180005315:	mov    %rcx,0x60(%rsi)
-   180005319:	mov    0x30(%rsp),%rbx
-   18000531e:	mov    0x38(%rsp),%rbp
-   180005323:	mov    0x40(%rsp),%rsi
-   180005328:	add    $0x20,%rsp
-   18000532c:	pop    %rdi
-   18000532d:	ret
-   18000532e:	int3
-   18000532f:	int3
-   180005330:	mov    %rbx,0x10(%rsp)
-   180005335:	push   %rdi
-   180005336:	sub    $0x20,%rsp
-   18000533a:	mov    0x8(%rcx),%r8
-   18000533e:	mov    %rdx,%r9
-   180005341:	mov    (%rcx),%rbx
-   180005344:	mov    %r8,%rdx
-   180005347:	sub    %rbx,%rdx
-   18000534a:	movabs $0x6666666666666667,%rdi
-   180005354:	mov    %rdi,%rax
-   180005357:	mov    %rcx,%r10
-   18000535a:	imul   %rdx
-   18000535d:	mov    %rdx,%r11
-   180005360:	sar    $0x4,%r11
-   180005364:	mov    %r11,%rax
-   180005367:	shr    $0x3f,%rax
-   18000536b:	add    %rax,%r11
-   18000536e:	cmp    %r11,%r9
-   180005371:	jae    0x18000538a
-   180005373:	lea    (%r9,%r9,4),%rax
-   180005377:	lea    (%rbx,%rax,8),%rcx
-   18000537b:	mov    %rcx,0x8(%r10)
-   18000537f:	mov    0x38(%rsp),%rbx
-   180005384:	add    $0x20,%rsp
-   180005388:	pop    %rdi
-   180005389:	ret
-   18000538a:	jbe    0x1800053f0
-   18000538c:	mov    0x10(%rcx),%rcx
-   180005390:	mov    %rdi,%rax
-   180005393:	sub    %rbx,%rcx
-   180005396:	imul   %rcx
-   180005399:	sar    $0x4,%rdx
-   18000539d:	mov    %rdx,%rax
-   1800053a0:	shr    $0x3f,%rax
-   1800053a4:	add    %rax,%rdx
-   1800053a7:	cmp    %rdx,%r9
-   1800053aa:	jbe    0x1800053c7
-   1800053ac:	lea    0x30(%rsp),%r8
-   1800053b1:	mov    %r9,%rdx
-   1800053b4:	mov    %r10,%rcx
-   1800053b7:	call   0x180001c40
-   1800053bc:	mov    0x38(%rsp),%rbx
-   1800053c1:	add    $0x20,%rsp
-   1800053c5:	pop    %rdi
-   1800053c6:	ret
-   1800053c7:	sub    %r11,%r9
-   1800053ca:	je     0x1800053ec
-   1800053cc:	nopl   0x0(%rax)
-   1800053d0:	movb   $0x0,(%r8)
-   1800053d4:	xor    %eax,%eax
-   1800053d6:	xorps  %xmm0,%xmm0
-   1800053d9:	movups %xmm0,0x8(%r8)
-   1800053de:	mov    %rax,0x18(%r8)
-   1800053e2:	add    $0x28,%r8
-   1800053e6:	sub    $0x1,%r9
-   1800053ea:	jne    0x1800053d0
-   1800053ec:	mov    %r8,0x8(%r10)
-   1800053f0:	mov    0x38(%rsp),%rbx
-   1800053f5:	add    $0x20,%rsp
-   1800053f9:	pop    %rdi
-   1800053fa:	ret
-   1800053fb:	int3
-   1800053fc:	int3
-   1800053fd:	int3
-   1800053fe:	int3
-   1800053ff:	int3
-   180005400:	mov    %rbx,0x10(%rsp)
-   180005405:	mov    %rbp,0x18(%rsp)
-   18000540a:	mov    %rsi,0x20(%rsp)
-   18000540f:	push   %rdi
-   180005410:	sub    $0x20,%rsp
-   180005414:	mov    0x38(%rcx),%r10
-   180005418:	lea    0x70(%rcx),%rax
-   18000541c:	mov    %r9d,%ebp
-   18000541f:	mov    %r8,%rsi
-   180005422:	mov    %rdx,%rbx
-   180005425:	mov    %rcx,%rdi
-   180005428:	cmp    %rax,(%r10)
-   18000542b:	jne    0x18000543d
-   18000542d:	cmp    $0x1,%r9d
-   180005431:	jne    0x18000543d
-   180005433:	cmpq   $0x0,0x68(%rcx)
-   180005438:	jne    0x18000543d
-   18000543a:	dec    %rsi
-   18000543d:	cmpq   $0x0,0x80(%rcx)
-   180005445:	je     0x18000549d
-   180005447:	call   0x1800036f0
-   18000544c:	test   %al,%al
-   18000544e:	je     0x18000549d
-   180005450:	test   %rsi,%rsi
-   180005453:	jne    0x18000545a
-   180005455:	cmp    $0x1,%ebp
-   180005458:	je     0x180005471
-   18000545a:	mov    0x80(%rdi),%rcx
-   180005461:	mov    %ebp,%r8d
-   180005464:	mov    %rsi,%rdx
-   180005467:	call   *0x3fab(%rip)        # 0x180009418
-   18000546d:	test   %eax,%eax
-   18000546f:	jne    0x18000549d
-   180005471:	mov    0x80(%rdi),%rcx
-   180005478:	lea    0x30(%rsp),%rdx
-   18000547d:	call   *0x3fb5(%rip)        # 0x180009438
-   180005483:	test   %eax,%eax
-   180005485:	jne    0x18000549d
-   180005487:	mov    %rdi,%rcx
-   18000548a:	call   0x1800038c0
-   18000548f:	mov    0x30(%rsp),%rcx
-   180005494:	mov    0x74(%rdi),%rax
-   180005498:	mov    %rcx,(%rbx)
-   18000549b:	jmp    0x1800054a6
-   18000549d:	movq   $0xffffffffffffffff,(%rbx)
-   1800054a4:	xor    %eax,%eax
-   1800054a6:	mov    0x40(%rsp),%rbp
-   1800054ab:	mov    0x48(%rsp),%rsi
-   1800054b0:	movq   $0x0,0x8(%rbx)
-   1800054b8:	mov    %rax,0x10(%rbx)
-   1800054bc:	mov    %rbx,%rax
-   1800054bf:	mov    0x38(%rsp),%rbx
-   1800054c4:	add    $0x20,%rsp
-   1800054c8:	pop    %rdi
-   1800054c9:	ret
-   1800054ca:	int3
-   1800054cb:	int3
-   1800054cc:	int3
-   1800054cd:	int3
-   1800054ce:	int3
-   1800054cf:	int3
-   1800054d0:	mov    %rbx,0x10(%rsp)
-   1800054d5:	mov    %rsi,0x18(%rsp)
-   1800054da:	push   %rdi
-   1800054db:	sub    $0x20,%rsp
-   1800054df:	mov    0x8(%r8),%rax
-   1800054e3:	mov    %r8,%rsi
-   1800054e6:	add    (%r8),%rax
-   1800054e9:	mov    %rdx,%rbx
-   1800054ec:	cmpq   $0x0,0x80(%rcx)
-   1800054f4:	mov    %rcx,%rdi
-   1800054f7:	mov    %rax,0x30(%rsp)
-   1800054fc:	je     0x18000557d
-   1800054fe:	call   0x1800036f0
-   180005503:	test   %al,%al
-   180005505:	je     0x18000557d
-   180005507:	mov    0x80(%rdi),%rcx
-   18000550e:	lea    0x30(%rsp),%rdx
-   180005513:	call   *0x3f07(%rip)        # 0x180009420
-   180005519:	test   %eax,%eax
-   18000551b:	jne    0x18000557d
-   18000551d:	mov    0x18(%rdi),%r8
-   180005521:	lea    0x70(%rdi),%rax
-   180005525:	mov    0x10(%rsi),%rcx
-   180005529:	mov    %rcx,0x74(%rdi)
-   18000552d:	cmp    %rax,(%r8)
-   180005530:	jne    0x180005556
-   180005532:	mov    0x88(%rdi),%rcx
-   180005539:	mov    0x90(%rdi),%rdx
-   180005540:	mov    %rcx,(%r8)
-   180005543:	sub    %ecx,%edx
-   180005545:	mov    0x38(%rdi),%rax
-   180005549:	mov    %rcx,(%rax)
-   18000554c:	mov    0x50(%rdi),%rax
-   180005550:	mov    %edx,(%rax)
-   180005552:	mov    0x74(%rdi),%rcx
-   180005556:	mov    0x30(%rsp),%rax
-   18000555b:	mov    %rax,(%rbx)
-   18000555e:	mov    %rbx,%rax
-   180005561:	movq   $0x0,0x8(%rbx)
-   180005569:	mov    %rcx,0x10(%rbx)
-   18000556d:	mov    0x38(%rsp),%rbx
-   180005572:	mov    0x40(%rsp),%rsi
-   180005577:	add    $0x20,%rsp
-   18000557b:	pop    %rdi
-   18000557c:	ret
-   18000557d:	mov    0x40(%rsp),%rsi
-   180005582:	xor    %eax,%eax
-   180005584:	movq   $0xffffffffffffffff,(%rbx)
-   18000558b:	movq   $0x0,0x8(%rbx)
-   180005593:	mov    %rax,0x10(%rbx)
-   180005597:	mov    %rbx,%rax
-   18000559a:	mov    0x38(%rsp),%rbx
-   18000559f:	add    $0x20,%rsp
-   1800055a3:	pop    %rdi
-   1800055a4:	ret
-   1800055a5:	int3
-   1800055a6:	int3
-   1800055a7:	int3
-   1800055a8:	int3
-   1800055a9:	int3
-   1800055aa:	int3
-   1800055ab:	int3
-   1800055ac:	int3
-   1800055ad:	int3
-   1800055ae:	int3
-   1800055af:	int3
-   1800055b0:	rex push %rbx
-   1800055b2:	push   %rsi
-   1800055b3:	sub    $0x28,%rsp
-   1800055b7:	xor    %esi,%esi
-   1800055b9:	mov    %r8,%r9
-   1800055bc:	mov    %rcx,%rbx
-   1800055bf:	test   %rdx,%rdx
-   1800055c2:	jne    0x1800055cd
-   1800055c4:	test   %r8,%r8
-   1800055c7:	lea    0x4(%rsi),%r8d
-   1800055cb:	je     0x1800055d0
-   1800055cd:	mov    %esi,%r8d
-   1800055d0:	mov    0x80(%rcx),%rcx
-   1800055d7:	test   %rcx,%rcx
-   1800055da:	je     0x180005683
-   1800055e0:	call   *0x3e22(%rip)        # 0x180009408
-   1800055e6:	test   %eax,%eax
-   1800055e8:	jne    0x180005683
-   1800055ee:	mov    %rdi,0x20(%rsp)
-   1800055f3:	mov    %rbx,%rcx
-   1800055f6:	mov    0x80(%rbx),%rdi
-   1800055fd:	movb   $0x1,0x7c(%rbx)
-   180005601:	mov    %sil,0x71(%rbx)
-   180005605:	call   *0x3bbd(%rip)        # 0x1800091c8
-   18000560b:	test   %rdi,%rdi
-   18000560e:	je     0x18000565e
-   180005610:	lea    0x50(%rsp),%r9
-   180005615:	mov    %rsi,0x40(%rsp)
-   18000561a:	lea    0x48(%rsp),%r8
-   18000561f:	mov    %rsi,0x48(%rsp)
-   180005624:	lea    0x40(%rsp),%rdx
-   180005629:	mov    %rsi,0x50(%rsp)
-   18000562e:	mov    %rdi,%rcx
-   180005631:	call   *0x3e21(%rip)        # 0x180009458
-   180005637:	mov    0x40(%rsp),%rax
-   18000563c:	mov    %rax,0x18(%rbx)
-   180005640:	mov    %rax,0x20(%rbx)
-   180005644:	mov    0x48(%rsp),%rax
-   180005649:	mov    %rax,0x38(%rbx)
-   18000564d:	mov    %rax,0x40(%rbx)
-   180005651:	mov    0x50(%rsp),%rax
-   180005656:	mov    %rax,0x50(%rbx)
-   18000565a:	mov    %rax,0x58(%rbx)
-   18000565e:	mov    %rdi,0x80(%rbx)
-   180005665:	mov    0x8fc4(%rip),%rax        # 0x18000e630
-   18000566c:	mov    0x20(%rsp),%rdi
-   180005671:	mov    %rax,0x74(%rbx)
-   180005675:	mov    %rbx,%rax
-   180005678:	mov    %rsi,0x68(%rbx)
-   18000567c:	add    $0x28,%rsp
-   180005680:	pop    %rsi
-   180005681:	pop    %rbx
-   180005682:	ret
-   180005683:	xor    %eax,%eax
-   180005685:	add    $0x28,%rsp
-   180005689:	pop    %rsi
-   18000568a:	pop    %rbx
-   18000568b:	ret
-   18000568c:	int3
-   18000568d:	int3
-   18000568e:	int3
-   18000568f:	int3
-   180005690:	mov    %rbx,0x8(%rsp)
-   180005695:	push   %rdi
-   180005696:	sub    $0x70,%rsp
-   18000569a:	mov    %rcx,%rdx
-   18000569d:	lea    0x20(%rsp),%rcx
-   1800056a2:	call   0x1800028c0
-   1800056a7:	nop
-   1800056a8:	lea    0x20(%rsp),%rcx
-   1800056ad:	call   0x180005730
-   1800056b2:	nop
-   1800056b3:	mov    0x68(%rsp),%rbx
-   1800056b8:	test   %rbx,%rbx
-   1800056bb:	je     0x1800056e9
-   1800056bd:	mov    $0xffffffff,%edi
-   1800056c2:	mov    %edi,%eax
-   1800056c4:	lock xadd %eax,0x8(%rbx)
-   1800056c9:	cmp    $0x1,%eax
-   1800056cc:	jne    0x1800056e9
-   1800056ce:	mov    (%rbx),%rax
-   1800056d1:	mov    %rbx,%rcx
-   1800056d4:	call   *(%rax)
-   1800056d6:	lock xadd %edi,0xc(%rbx)
-   1800056db:	cmp    $0x1,%edi
-   1800056de:	jne    0x1800056e9
-   1800056e0:	mov    (%rbx),%rax
-   1800056e3:	mov    %rbx,%rcx
-   1800056e6:	call   *0x8(%rax)
-   1800056e9:	lea    0x40(%rsp),%rcx
-   1800056ee:	call   0x180002e30
-   1800056f3:	lea    0x30(%rsp),%rcx
-   1800056f8:	call   0x180006f3a
-   1800056fd:	mov    0x28(%rsp),%rcx
-   180005702:	test   %rcx,%rcx
-   180005705:	je     0x180005711
-   180005707:	mov    (%rcx),%rax
-   18000570a:	mov    $0x1,%edx
-   18000570f:	call   *(%rax)
-   180005711:	mov    $0x1,%al
-   180005713:	mov    0x80(%rsp),%rbx
-   18000571b:	add    $0x70,%rsp
-   18000571f:	pop    %rdi
-   180005720:	ret
-   180005721:	int3
-   180005722:	int3
-   180005723:	int3
-   180005724:	int3
-   180005725:	int3
-   180005726:	int3
-   180005727:	int3
-   180005728:	int3
-   180005729:	int3
-   18000572a:	int3
-   18000572b:	int3
-   18000572c:	int3
-   18000572d:	int3
-   18000572e:	int3
-   18000572f:	int3
-   180005730:	mov    %rsp,%rax
-   180005733:	mov    %rbx,0x10(%rax)
-   180005737:	mov    %rsi,0x18(%rax)
-   18000573b:	mov    %rdi,0x20(%rax)
-   18000573f:	push   %rbp
-   180005740:	push   %r12
-   180005742:	push   %r13
-   180005744:	push   %r14
-   180005746:	push   %r15
-   180005748:	lea    -0x3b8(%rax),%rbp
-   18000574f:	sub    $0x490,%rsp
-   180005756:	movaps %xmm6,-0x38(%rax)
-   18000575a:	movaps %xmm7,-0x48(%rax)
-   18000575e:	movaps %xmm8,-0x58(%rax)
-   180005763:	movaps %xmm9,-0x68(%rax)
-   180005768:	movaps %xmm10,-0x78(%rax)
-   18000576d:	movaps %xmm11,-0x88(%rax)
-   180005775:	movaps %xmm12,-0x98(%rax)
-   18000577d:	movaps %xmm13,-0xa8(%rax)
-   180005785:	mov    0x887c(%rip),%rax        # 0x18000e008
-   18000578c:	xor    %rsp,%rax
-   18000578f:	mov    %rax,0x300(%rbp)
-   180005796:	mov    %rcx,%r15
-   180005799:	xor    %edi,%edi
-   18000579b:	mov    %edi,0x48(%rsp)
-   18000579f:	mov    (%rcx),%rcx
-   1800057a2:	call   *0x3ac8(%rip)        # 0x180009270
-   1800057a8:	mov    %eax,%r14d
-   1800057ab:	mov    %eax,0x50(%rsp)
-   1800057af:	mov    (%r15),%rcx
-   1800057b2:	call   *0x3ad8(%rip)        # 0x180009290
-   1800057b8:	mov    %edi,0x140(%rbp)
-   1800057be:	mov    %eax,0x144(%rbp)
-   1800057c4:	movsd  0x140(%rbp),%xmm0
-   1800057cc:	movsd  %xmm0,0x190(%rbp)
-   1800057d4:	mov    0x148(%rbp),%ecx
-   1800057da:	mov    %ecx,0x198(%rbp)
-   1800057e0:	mov    0x140(%rbp),%rcx
-   1800057e7:	shr    $0x20,%rcx
-   1800057eb:	test   %ecx,%ecx
-   1800057ed:	je     0x180005843
-   1800057ef:	mov    0x194(%rbp),%edi
-   1800057f5:	mov    0x190(%rbp),%ebx
-   1800057fb:	nopl   0x0(%rax,%rax,1)
-   180005800:	mov    %ebx,%r8d
-   180005803:	lea    0x1c0(%rbp),%rdx
-   18000580a:	mov    (%r15),%rcx
-   18000580d:	call   0x180006f6a
-   180005812:	movups (%rax),%xmm1
-   180005815:	movups 0x10(%rax),%xmm2
-   180005819:	movsd  0x20(%rax),%xmm0
-   18000581e:	mov    0x40(%r15),%rcx
-   180005822:	mov    %ebx,%eax
-   180005824:	lea    (%rax,%rax,4),%rdx
-   180005828:	mov    0x58(%rcx),%rax
-   18000582c:	movups %xmm1,(%rax,%rdx,8)
-   180005830:	movups %xmm2,0x10(%rax,%rdx,8)
-   180005835:	movsd  %xmm0,0x20(%rax,%rdx,8)
-   18000583b:	inc    %ebx
-   18000583d:	cmp    %edi,%ebx
-   18000583f:	jne    0x180005800
-   180005841:	xor    %edi,%edi
-   180005843:	mov    %r15,%rcx
-   180005846:	call   0x1800047e0
-   18000584b:	lea    0x3ebe(%rip),%rax        # 0x180009710
-   180005852:	mov    %rax,0x60(%rsp)
-   180005857:	lea    0x3eba(%rip),%rax        # 0x180009718
-   18000585e:	mov    %rax,0x70(%rsp)
-   180005863:	lea    0x18(%rbp),%rcx
-   180005867:	call   *0x388b(%rip)        # 0x1800090f8
-   18000586d:	nop
-   18000586e:	movl   $0x1,0x48(%rsp)
-   180005876:	xor    %r8d,%r8d
-   180005879:	lea    0x78(%rsp),%rdx
-   18000587e:	lea    0x60(%rsp),%rcx
-   180005883:	call   *0x3847(%rip)        # 0x1800090d0
-   180005889:	nop
-   18000588a:	mov    0x60(%rsp),%rax
-   18000588f:	movslq 0x4(%rax),%rcx
-   180005893:	lea    0x3e6e(%rip),%rax        # 0x180009708
-   18000589a:	mov    %rax,0x60(%rsp,%rcx,1)
-   18000589f:	mov    0x60(%rsp),%rax
-   1800058a4:	movslq 0x4(%rax),%rcx
-   1800058a8:	lea    -0xb8(%rcx),%edx
-   1800058ae:	mov    %edx,0x5c(%rsp,%rcx,1)
-   1800058b2:	lea    0x78(%rsp),%rax
-   1800058b7:	mov    %rax,0x140(%rbp)
-   1800058be:	lea    0x78(%rsp),%rcx
-   1800058c3:	call   *0x38cf(%rip)        # 0x180009198
-   1800058c9:	nop
-   1800058ca:	lea    0x3db7(%rip),%rax        # 0x180009688
-   1800058d1:	mov    %rax,0x78(%rsp)
-   1800058d6:	movb   $0x0,-0xc(%rbp)
-   1800058da:	movb   $0x0,-0x17(%rbp)
-   1800058de:	lea    0x78(%rsp),%rcx
-   1800058e3:	call   *0x38df(%rip)        # 0x1800091c8
-   1800058e9:	mov    %rdi,-0x8(%rbp)
-   1800058ed:	mov    0x8d3c(%rip),%rax        # 0x18000e630
-   1800058f4:	mov    %rax,-0x14(%rbp)
-   1800058f8:	mov    %rdi,-0x20(%rbp)
-   1800058fc:	mov    $0xa,%edx
-   180005901:	lea    0x36(%rdx),%r8d
-   180005905:	lea    0x3e9c(%rip),%rcx        # 0x1800097a8
-   18000590c:	call   0x180006fe0
-   180005911:	mov    %rax,%rbx
-   180005914:	test   %rax,%rax
-   180005917:	jne    0x18000593b
-   180005919:	mov    0x60(%rsp),%rax
-   18000591e:	movslq 0x4(%rax),%rcx
-   180005922:	lea    0x60(%rsp),%rax
-   180005927:	add    %rax,%rcx
-   18000592a:	xor    %r8d,%r8d
-   18000592d:	lea    0x2(%rbx),%edx
-   180005930:	call   *0x37ca(%rip)        # 0x180009100
-   180005936:	jmp    0x180005a39
-   18000593b:	movb   $0x1,-0xc(%rbp)
-   18000593f:	movb   $0x0,-0x17(%rbp)
-   180005943:	lea    0x78(%rsp),%rcx
-   180005948:	call   *0x387a(%rip)        # 0x1800091c8
-   18000594e:	mov    %rdi,0x48(%rsp)
-   180005953:	mov    %rdi,0x40(%rsp)
-   180005958:	mov    %rdi,0x190(%rbp)
-   18000595f:	lea    0x190(%rbp),%r9
-   180005966:	lea    0x40(%rsp),%r8
-   18000596b:	lea    0x48(%rsp),%rdx
-   180005970:	mov    %rbx,%rcx
-   180005973:	call   *0x3adf(%rip)        # 0x180009458
-   180005979:	mov    0x190(%rbp),%r9
-   180005980:	mov    %r9,0x30(%rsp)
-   180005985:	mov    0x40(%rsp),%r8
-   18000598a:	mov    %r8,0x28(%rsp)
-   18000598f:	mov    0x48(%rsp),%rdx
-   180005994:	mov    %rdx,0x20(%rsp)
-   180005999:	lea    0x78(%rsp),%rcx
-   18000599e:	call   *0x3784(%rip)        # 0x180009128
-   1800059a4:	mov    %rbx,-0x8(%rbp)
-   1800059a8:	mov    0x8c81(%rip),%rax        # 0x18000e630
-   1800059af:	mov    %rax,-0x14(%rbp)
-   1800059b3:	mov    %rdi,-0x20(%rbp)
-   1800059b7:	lea    0x140(%rbp),%rdx
-   1800059be:	lea    0x78(%rsp),%rcx
-   1800059c3:	call   *0x37df(%rip)        # 0x1800091a8
-   1800059c9:	nop
-   1800059ca:	mov    %rax,%rcx
-   1800059cd:	call   0x180002680
-   1800059d2:	mov    %rax,%rbx
-   1800059d5:	mov    %rax,%rcx
-   1800059d8:	call   *0x3792(%rip)        # 0x180009170
-   1800059de:	test   %al,%al
-   1800059e0:	je     0x1800059e8
-   1800059e2:	mov    %rdi,-0x20(%rbp)
-   1800059e6:	jmp    0x1800059f8
-   1800059e8:	mov    %rbx,-0x20(%rbp)
-   1800059ec:	lea    0x78(%rsp),%rcx
-   1800059f1:	call   *0x37d1(%rip)        # 0x1800091c8
-   1800059f7:	nop
-   1800059f8:	mov    0x148(%rbp),%rcx
-   1800059ff:	test   %rcx,%rcx
-   180005a02:	je     0x180005a1d
-   180005a04:	mov    (%rcx),%rax
-   180005a07:	call   *0x10(%rax)
-   180005a0a:	test   %rax,%rax
-   180005a0d:	je     0x180005a1d
-   180005a0f:	mov    (%rax),%r8
-   180005a12:	mov    $0x1,%edx
-   180005a17:	mov    %rax,%rcx
-   180005a1a:	call   *(%r8)
-   180005a1d:	mov    0x60(%rsp),%rax
-   180005a22:	movslq 0x4(%rax),%rcx
-   180005a26:	lea    0x60(%rsp),%rax
-   180005a2b:	add    %rax,%rcx
-   180005a2e:	xor    %r8d,%r8d
-   180005a31:	xor    %edx,%edx
-   180005a33:	call   *0x36cf(%rip)        # 0x180009108
-   180005a39:	lea    0x3d80(%rip),%rdx        # 0x1800097c0
-   180005a40:	lea    0x70(%rsp),%rcx
-   180005a45:	call   0x180001290
-   180005a4a:	mov    %rax,%rcx
-   180005a4d:	lea    0x3d64(%rip),%rdx        # 0x1800097b8
-   180005a54:	call   0x180001290
-   180005a59:	xorps  %xmm10,%xmm10
-   180005a5d:	xorps  %xmm11,%xmm11
-   180005a61:	mov    0x28(%r15),%r9
-   180005a65:	mov    0x20(%r15),%r8
-   180005a69:	mov    $0xfffffffffffffff0,%r13
-   180005a70:	lea    0x3d61(%rip),%rsi        # 0x1800097d8
-   180005a77:	cmp    %r9,%r8
-   180005a7a:	je     0x18000649f
-   180005a80:	lea    0x10(%r15),%rsi
-   180005a84:	movsd  0x3ee3(%rip),%xmm12        # 0x180009970
-   180005a8d:	movsd  0x3ee2(%rip),%xmm13        # 0x180009978
-   180005a96:	movabs $0x2e8ba2e8ba2e8ba3,%r10
-   180005aa0:	movups (%r8),%xmm0
-   180005aa4:	movaps %xmm0,0xe0(%rbp)
-   180005aab:	movups 0x10(%r8),%xmm1
-   180005ab0:	movaps %xmm1,0xf0(%rbp)
-   180005ab7:	movups 0x20(%r8),%xmm0
-   180005abc:	movaps %xmm0,0x100(%rbp)
-   180005ac3:	movups 0x30(%r8),%xmm1
-   180005ac8:	movaps %xmm1,0x110(%rbp)
-   180005acf:	movups 0x40(%r8),%xmm0
-   180005ad4:	movaps %xmm0,0x120(%rbp)
-   180005adb:	movsd  0x50(%r8),%xmm1
-   180005ae1:	movsd  %xmm1,0x130(%rbp)
-   180005ae9:	mov    %r9,%rcx
-   180005aec:	sub    %r8,%rcx
-   180005aef:	mov    %r10,%rax
-   180005af2:	imul   %rcx
-   180005af5:	sar    $0x4,%rdx
-   180005af9:	mov    %rdx,%rax
-   180005afc:	shr    $0x3f,%rax
-   180005b00:	add    %rax,%rdx
-   180005b03:	cmp    $0x2,%rdx
-   180005b07:	jl     0x180005d14
-   180005b0d:	lea    -0x58(%r9),%rcx
-   180005b11:	movups (%rcx),%xmm4
-   180005b14:	movups 0x10(%rcx),%xmm3
-   180005b18:	movaps %xmm3,0x90(%rbp)
-   180005b1f:	movups 0x20(%rcx),%xmm5
-   180005b23:	movups 0x30(%rcx),%xmm6
-   180005b27:	movups 0x40(%rcx),%xmm7
-   180005b2b:	movsd  0x50(%rcx),%xmm8
-   180005b31:	movups (%r8),%xmm0
-   180005b35:	movups %xmm0,(%rcx)
-   180005b38:	movups 0x10(%r8),%xmm1
-   180005b3d:	movups %xmm1,0x10(%rcx)
-   180005b41:	movups 0x20(%r8),%xmm0
-   180005b46:	movups %xmm0,0x20(%rcx)
-   180005b4a:	movups 0x30(%r8),%xmm1
-   180005b4f:	movups %xmm1,0x30(%rcx)
-   180005b53:	movups 0x40(%r8),%xmm0
-   180005b58:	movups %xmm0,0x40(%rcx)
-   180005b5c:	movsd  0x50(%r8),%xmm1
-   180005b62:	movsd  %xmm1,0x50(%rcx)
-   180005b67:	sub    %r8,%rcx
-   180005b6a:	mov    %r10,%rax
-   180005b6d:	imul   %rcx
-   180005b70:	sar    $0x4,%rdx
-   180005b74:	mov    %rdx,%rax
-   180005b77:	shr    $0x3f,%rax
-   180005b7b:	add    %rax,%rdx
-   180005b7e:	mov    %rdi,%r10
-   180005b81:	mov    %rdi,%r9
-   180005b84:	lea    -0x1(%rdx),%r11
-   180005b88:	sar    %r11
-   180005b8b:	test   %r11,%r11
-   180005b8e:	jle    0x180005c0e
-   180005b90:	lea    (%r9,%r9,1),%rcx
-   180005b94:	imul   $0x58,%rcx,%rax
-   180005b98:	mov    %rdi,%r9
-   180005b9b:	movsd  0xc0(%rax,%r8,1),%xmm0
-   180005ba5:	comisd 0x68(%rax,%r8,1),%xmm0
-   180005bac:	setb   %r9b
-   180005bb0:	inc    %rcx
-   180005bb3:	add    %rcx,%r9
-   180005bb6:	imul   $0x58,%r9,%rax
-   180005bba:	imul   $0x58,%r10,%rcx
-   180005bbe:	movups (%rax,%r8,1),%xmm0
-   180005bc3:	movups %xmm0,(%rcx,%r8,1)
-   180005bc8:	movups 0x10(%rax,%r8,1),%xmm1
-   180005bce:	movups %xmm1,0x10(%rcx,%r8,1)
-   180005bd4:	movups 0x20(%rax,%r8,1),%xmm0
-   180005bda:	movups %xmm0,0x20(%rcx,%r8,1)
-   180005be0:	movups 0x30(%rax,%r8,1),%xmm1
-   180005be6:	movups %xmm1,0x30(%rcx,%r8,1)
-   180005bec:	movups 0x40(%rax,%r8,1),%xmm0
-   180005bf2:	movups %xmm0,0x40(%rcx,%r8,1)
-   180005bf8:	movsd  0x50(%rax,%r8,1),%xmm1
-   180005bff:	movsd  %xmm1,0x50(%rcx,%r8,1)
-   180005c06:	mov    %r9,%r10
-   180005c09:	cmp    %r11,%r9
-   180005c0c:	jl     0x180005b90
-   180005c0e:	cmp    %r11,%r10
-   180005c11:	jne    0x180005c6d
-   180005c13:	test   $0x1,%dl
-   180005c16:	jne    0x180005c6d
-   180005c18:	imul   $0x58,%rdx,%rax
-   180005c1c:	imul   $0x58,%r10,%rcx
-   180005c20:	movups -0x58(%rax,%r8,1),%xmm0
-   180005c26:	movups %xmm0,(%rcx,%r8,1)
-   180005c2b:	movups -0x48(%rax,%r8,1),%xmm1
-   180005c31:	movups %xmm1,0x10(%rcx,%r8,1)
-   180005c37:	movups -0x38(%rax,%r8,1),%xmm0
-   180005c3d:	movups %xmm0,0x20(%rcx,%r8,1)
-   180005c43:	movups -0x28(%rax,%r8,1),%xmm1
-   180005c49:	movups %xmm1,0x30(%rcx,%r8,1)
-   180005c4f:	movups -0x18(%rax,%r8,1),%xmm0
-   180005c55:	movups %xmm0,0x40(%rcx,%r8,1)
-   180005c5b:	movsd  -0x8(%rax,%r8,1),%xmm1
-   180005c62:	movsd  %xmm1,0x50(%rcx,%r8,1)
-   180005c69:	lea    -0x1(%rdx),%r10
-   180005c6d:	test   %r10,%r10
-   180005c70:	jle    0x180005cec
-   180005c72:	movsd  0x90(%rbp),%xmm2
-   180005c7a:	nopw   0x0(%rax,%rax,1)
-   180005c80:	lea    -0x1(%r10),%rdx
-   180005c84:	sar    %rdx
-   180005c87:	imul   $0x58,%rdx,%rcx
-   180005c8b:	movsd  0x10(%rcx,%r8,1),%xmm0
-   180005c92:	comisd %xmm2,%xmm0
-   180005c96:	jb     0x180005cec
-   180005c98:	imul   $0x58,%r10,%rax
-   180005c9c:	movups (%rcx,%r8,1),%xmm0
-   180005ca1:	movups %xmm0,(%rax,%r8,1)
-   180005ca6:	movups 0x10(%rcx,%r8,1),%xmm1
-   180005cac:	movups %xmm1,0x10(%rax,%r8,1)
-   180005cb2:	movups 0x20(%rcx,%r8,1),%xmm0
-   180005cb8:	movups %xmm0,0x20(%rax,%r8,1)
-   180005cbe:	movups 0x30(%rcx,%r8,1),%xmm1
-   180005cc4:	movups %xmm1,0x30(%rax,%r8,1)
-   180005cca:	movups 0x40(%rcx,%r8,1),%xmm0
-   180005cd0:	movups %xmm0,0x40(%rax,%r8,1)
-   180005cd6:	movsd  0x50(%rcx,%r8,1),%xmm1
-   180005cdd:	movsd  %xmm1,0x50(%rax,%r8,1)
-   180005ce4:	mov    %rdx,%r10
-   180005ce7:	test   %rdx,%rdx
-   180005cea:	jg     0x180005c80
-   180005cec:	imul   $0x58,%r10,%rax
-   180005cf0:	movups %xmm4,(%rax,%r8,1)
-   180005cf5:	movups %xmm3,0x10(%rax,%r8,1)
-   180005cfb:	movups %xmm5,0x20(%rax,%r8,1)
-   180005d01:	movups %xmm6,0x30(%rax,%r8,1)
-   180005d07:	movups %xmm7,0x40(%rax,%r8,1)
-   180005d0d:	movsd  %xmm8,0x50(%rax,%r8,1)
-   180005d14:	addq   $0xffffffffffffffa8,0x28(%r15)
-   180005d19:	movsd  0xe8(%rbp),%xmm11
-   180005d22:	mov    0xe0(%rbp),%edx
-   180005d28:	mov    %rsi,%rcx
-   180005d2b:	call   0x180006f40
-   180005d30:	test   %al,%al
-   180005d32:	je     0x180006487
-   180005d38:	comisd %xmm12,%xmm11
-   180005d3d:	jbe    0x180005d4a
-   180005d3f:	comisd %xmm11,%xmm13
-   180005d44:	ja     0x180006487
-   180005d4a:	lea    0xf8(%rbp),%r8
-   180005d51:	mov    0xe0(%rbp),%edx
-   180005d57:	mov    (%r15),%rcx
-   180005d5a:	call   0x180006f52
-   180005d5f:	test   %al,%al
-   180005d61:	je     0x180006487
-   180005d67:	lea    0xf8(%rbp),%r9
-   180005d6e:	mov    0xe0(%rbp),%r8d
-   180005d75:	lea    0x240(%rbp),%rdx
-   180005d7c:	mov    %rsi,%rcx
-   180005d7f:	call   0x180006f46
-   180005d84:	nop
-   180005d85:	movsd  %xmm10,0x190(%rbp)
-   180005d8e:	movsd  %xmm10,0x40(%rsp)
-   180005d95:	mov    0x190(%rbp),%rax
-   180005d9c:	xorps  %xmm0,%xmm0
-   180005d9f:	cmp    0x40(%rsp),%rax
-   180005da4:	jne    0x180005db1
-   180005da6:	xor    %eax,%eax
-   180005da8:	mov    %rax,0x2c0(%rbp)
-   180005daf:	jmp    0x180005dba
-   180005db1:	movsd  %xmm10,0x2c0(%rbp)
-   180005dba:	cmpb   $0x0,0x110(%rbp)
-   180005dc1:	je     0x180005dea
-   180005dc3:	movups 0x118(%rbp),%xmm0
-   180005dca:	movups %xmm0,0x140(%rbp)
-   180005dd1:	movsd  0x128(%rbp),%xmm1
-   180005dd9:	movsd  %xmm1,0x150(%rbp)
-   180005de1:	lea    0x140(%rbp),%rax
-   180005de8:	jmp    0x180005e08
-   180005dea:	movups %xmm0,0x190(%rbp)
-   180005df1:	movsd  0x2c0(%rbp),%xmm0
-   180005df9:	movsd  %xmm0,0x1a0(%rbp)
-   180005e01:	lea    0x190(%rbp),%rax
-   180005e08:	movb   $0x1,0x160(%rbp)
-   180005e0f:	movups (%rax),%xmm0
-   180005e12:	movups %xmm0,0x168(%rbp)
-   180005e19:	movsd  0x10(%rax),%xmm2
-   180005e1e:	mov    0x40(%r15),%rcx
-   180005e22:	mov    0x240(%rbp),%eax
-   180005e28:	lea    (%rax,%rax,4),%rdx
-   180005e2c:	mov    0x58(%rcx),%rax
-   180005e30:	movups 0x160(%rbp),%xmm0
-   180005e37:	movups %xmm0,(%rax,%rdx,8)
-   180005e3b:	movups 0x170(%rbp),%xmm1
-   180005e42:	unpcklpd %xmm2,%xmm1
-   180005e46:	movups %xmm1,0x170(%rbp)
-   180005e4d:	movups %xmm1,0x10(%rax,%rdx,8)
-   180005e52:	movsd  0x180(%rbp),%xmm0
-   180005e5a:	movsd  %xmm0,0x20(%rax,%rdx,8)
-   180005e60:	mov    0x290(%rbp),%rdi
-   180005e67:	mov    0x298(%rbp),%rax
-   180005e6e:	mov    %rax,0x140(%rbp)
-   180005e75:	cmp    %rax,%rdi
-   180005e78:	je     0x18000618a
-   180005e7e:	xchg   %ax,%ax
-   180005e80:	mov    (%rdi),%r14d
-   180005e83:	mov    %r14d,0x48(%rsp)
-   180005e88:	mov    %r14d,%edx
-   180005e8b:	mov    %rsi,%rcx
-   180005e8e:	call   0x180006f40
-   180005e93:	test   %al,%al
-   180005e95:	je     0x180006166
-   180005e9b:	mov    (%r15),%rcx
-   180005e9e:	call   *0x33f4(%rip)        # 0x180009298
-   180005ea4:	mov    %rax,%rcx
-   180005ea7:	mov    %r14d,%edx
-   180005eaa:	call   *0x33a0(%rip)        # 0x180009250
-   180005eb0:	mov    %rax,%rsi
-   180005eb3:	mov    0x40(%r15),%rcx
-   180005eb7:	mov    (%rcx),%r8
-   180005eba:	mov    (%rax),%edx
-   180005ebc:	call   *0x78(%r8)
-   180005ec0:	movups (%rax),%xmm6
-   180005ec3:	movups %xmm6,0x1c0(%rbp)
-   180005eca:	movups 0x10(%rax),%xmm0
-   180005ece:	movups %xmm0,0x1d0(%rbp)
-   180005ed5:	movsd  0x20(%rax),%xmm1
-   180005eda:	movsd  %xmm1,0x1e0(%rbp)
-   180005ee2:	mov    0x40(%r15),%rcx
-   180005ee6:	mov    (%rcx),%rax
-   180005ee9:	mov    0x4(%rsi),%edx
-   180005eec:	call   *0x78(%rax)
-   180005eef:	movups (%rax),%xmm0
-   180005ef2:	movups %xmm0,0x2d0(%rbp)
-   180005ef9:	movups 0x10(%rax),%xmm1
-   180005efd:	movups %xmm1,0x2e0(%rbp)
-   180005f04:	movsd  0x20(%rax),%xmm0
-   180005f09:	movsd  %xmm0,0x2f0(%rbp)
-   180005f11:	lea    0x4(%rsi),%r9
-   180005f15:	mov    %rsi,%r8
-   180005f18:	lea    0x208(%rbp),%rdx
-   180005f1f:	mov    %r15,%rcx
-   180005f22:	call   0x180003f20
-   180005f27:	mov    %rsi,%r9
-   180005f2a:	lea    0x4(%rsi),%r8
-   180005f2e:	lea    0x160(%rbp),%rdx
-   180005f35:	mov    %r15,%rcx
-   180005f38:	call   0x180003f20
-   180005f3d:	movd   %xmm6,%eax
-   180005f41:	test   %al,%al
-   180005f43:	je     0x1800060e9
-   180005f49:	cmpb   $0x0,0x2d0(%rbp)
-   180005f50:	je     0x1800060e9
-   180005f56:	cmpb   $0x0,0x208(%rbp)
-   180005f5d:	je     0x1800060e9
-   180005f63:	cmpb   $0x0,0x160(%rbp)
-   180005f6a:	je     0x1800060e9
-   180005f70:	lea    0x210(%rbp),%rdx
-   180005f77:	lea    0x1c8(%rbp),%rcx
-   180005f7e:	call   0x180003ed0
-   180005f83:	movaps %xmm0,%xmm7
-   180005f86:	lea    0x168(%rbp),%rdx
-   180005f8d:	lea    0x2d8(%rbp),%rcx
-   180005f94:	call   0x180003ed0
-   180005f99:	movaps %xmm0,%xmm8
-   180005f9d:	mov    (%r15),%rcx
-   180005fa0:	mov    %rsi,%rdx
-   180005fa3:	call   *0x32bf(%rip)        # 0x180009268
-   180005fa9:	movaps %xmm0,%xmm6
-   180005fac:	comisd %xmm8,%xmm7
-   180005fb1:	jbe    0x180005fba
-   180005fb3:	mulsd  %xmm8,%xmm6
-   180005fb8:	jmp    0x180005fbe
-   180005fba:	mulsd  %xmm7,%xmm6
-   180005fbe:	movsd  %xmm6,0x40(%rsp)
-   180005fc4:	mov    %rsi,%rdx
-   180005fc7:	mov    (%r15),%rcx
-   180005fca:	call   *0x3298(%rip)        # 0x180009268
-   180005fd0:	movaps %xmm0,%xmm9
-   180005fd4:	movsd  %xmm0,0x190(%rbp)
-   180005fdc:	mov    (%r15),%rcx
-   180005fdf:	add    $0x18,%rcx
-   180005fe3:	comisd %xmm7,%xmm8
-   180005fe8:	jbe    0x180006081
-   180005fee:	mov    (%rsi),%edx
-   180005ff0:	call   *0x3282(%rip)        # 0x180009278
-   180005ff6:	mov    0x28(%r15),%rdx
-   180005ffa:	cmp    0x30(%r15),%rdx
-   180005ffe:	je     0x18000604c
-   180006000:	movups (%rax),%xmm1
-   180006003:	movsd  0x10(%rax),%xmm0
-   180006008:	movsd  %xmm6,0x8(%rdx)
-   18000600d:	movsd  %xmm9,0x10(%rdx)
-   180006013:	mov    %r14d,(%rdx)
-   180006016:	movups %xmm1,0x18(%rdx)
-   18000601a:	movsd  %xmm0,0x28(%rdx)
-   18000601f:	movups 0x208(%rbp),%xmm1
-   180006026:	movups %xmm1,0x30(%rdx)
-   18000602a:	movups 0x218(%rbp),%xmm0
-   180006031:	movups %xmm0,0x40(%rdx)
-   180006035:	movsd  0x228(%rbp),%xmm1
-   18000603d:	movsd  %xmm1,0x50(%rdx)
-   180006042:	addq   $0x58,0x28(%r15)
-   180006047:	jmp    0x180006150
-   18000604c:	lea    0x208(%rbp),%rcx
-   180006053:	mov    %rcx,0x30(%rsp)
-   180006058:	mov    %rax,0x28(%rsp)
-   18000605d:	lea    0x190(%rbp),%rax
-   180006064:	mov    %rax,0x20(%rsp)
-   180006069:	lea    0x40(%rsp),%r9
-   18000606e:	lea    0x48(%rsp),%r8
-   180006073:	lea    0x20(%r15),%rcx
-   180006077:	call   0x1800015d0
-   18000607c:	jmp    0x180006150
-   180006081:	mov    0x4(%rsi),%edx
-   180006084:	call   *0x31ee(%rip)        # 0x180009278
-   18000608a:	mov    0x28(%r15),%rdx
-   18000608e:	cmp    0x30(%r15),%rdx
-   180006092:	je     0x1800060dd
-   180006094:	movups (%rax),%xmm1
-   180006097:	movsd  0x10(%rax),%xmm0
-   18000609c:	mov    %r14d,(%rdx)
-   18000609f:	movsd  %xmm6,0x8(%rdx)
-   1800060a4:	movsd  %xmm9,0x10(%rdx)
-   1800060aa:	movups %xmm1,0x18(%rdx)
-   1800060ae:	movsd  %xmm0,0x28(%rdx)
-   1800060b3:	movups 0x160(%rbp),%xmm1
-   1800060ba:	movups %xmm1,0x30(%rdx)
-   1800060be:	movups 0x170(%rbp),%xmm0
-   1800060c5:	movups %xmm0,0x40(%rdx)
-   1800060c9:	movsd  0x180(%rbp),%xmm1
-   1800060d1:	movsd  %xmm1,0x50(%rdx)
-   1800060d6:	addq   $0x58,0x28(%r15)
-   1800060db:	jmp    0x180006150
-   1800060dd:	lea    0x160(%rbp),%rcx
-   1800060e4:	jmp    0x180006053
-   1800060e9:	xor    %eax,%eax
-   1800060eb:	mov    %eax,0x40(%rsp)
-   1800060ef:	mov    %eax,0x190(%rbp)
-   1800060f5:	mov    (%r15),%rcx
-   1800060f8:	add    $0x18,%rcx
-   1800060fc:	mov    (%rsi),%edx
-   1800060fe:	call   *0x3174(%rip)        # 0x180009278
-   180006104:	mov    0x28(%r15),%rdx
-   180006108:	cmp    0x30(%r15),%rdx
-   18000610c:	je     0x180006120
-   18000610e:	movups (%rax),%xmm1
-   180006111:	movsd  0x10(%rax),%xmm0
-   180006116:	movups %xmm10,0x8(%rdx)
-   18000611b:	jmp    0x180006013
-   180006120:	lea    0x208(%rbp),%rcx
-   180006127:	mov    %rcx,0x30(%rsp)
-   18000612c:	mov    %rax,0x28(%rsp)
-   180006131:	lea    0x40(%rsp),%rax
-   180006136:	mov    %rax,0x20(%rsp)
-   18000613b:	lea    0x190(%rbp),%r9
-   180006142:	lea    0x48(%rsp),%r8
-   180006147:	lea    0x20(%r15),%rcx
-   18000614b:	call   0x180001850
-   180006150:	mov    0x28(%r15),%rdx
-   180006154:	movzbl 0x38(%r15),%r8d
-   180006159:	mov    0x20(%r15),%rcx
-   18000615d:	call   0x180002560
-   180006162:	lea    0x10(%r15),%rsi
-   180006166:	add    $0x20,%rdi
-   18000616a:	cmp    0x140(%rbp),%rdi
-   180006171:	jne    0x180005e80
-   180006177:	mov    0x290(%rbp),%rdi
-   18000617e:	mov    0x50(%rsp),%r14d
-   180006183:	mov    $0xfffffffffffffff0,%r13
-   18000618a:	add    $0xfffffffe,%r14d
-   18000618e:	mov    %r14d,0x50(%rsp)
-   180006193:	mov    $0xd1b71759,%eax
-   180006198:	mul    %r14d
-   18000619b:	shr    $0xd,%edx
-   18000619e:	imul   $0x2710,%edx,%ecx
-   1800061a4:	cmp    %ecx,%r14d
-   1800061a7:	jne    0x1800062d8
-   1800061ad:	lea    0x170(%rbp),%rdx
-   1800061b4:	mov    %r14d,%ecx
-   1800061b7:	call   0x180006f7c
-   1800061bc:	lea    0x160(%rbp),%rdx
-   1800061c3:	mov    %r13,%rcx
-   1800061c6:	sub    %rdx,%rcx
-   1800061c9:	add    %rcx,%rax
-   1800061cc:	lea    0x170(%rbp),%rcx
-   1800061d3:	mov    %rcx,0x160(%rbp)
-   1800061da:	mov    %rax,0x168(%rbp)
-   1800061e1:	lea    0x35f0(%rip),%rcx        # 0x1800097d8
-   1800061e8:	mov    %rcx,0x208(%rbp)
-   1800061ef:	mov    %rcx,%rax
-   1800061f2:	inc    %rax
-   1800061f5:	cmpb   $0x0,(%rax)
-   1800061f8:	jne    0x1800061f2
-   1800061fa:	sub    %rcx,%rax
-   1800061fd:	mov    %rax,0x210(%rbp)
-   180006204:	lea    0x35d5(%rip),%rcx        # 0x1800097e0
-   18000620b:	mov    %rcx,0x190(%rbp)
-   180006212:	mov    %rcx,%rax
-   180006215:	inc    %rax
-   180006218:	cmpb   $0x0,(%rax)
-   18000621b:	jne    0x180006215
-   18000621d:	sub    %rcx,%rax
-   180006220:	mov    %rax,0x198(%rbp)
-   180006227:	lea    0x160(%rbp),%r9
-   18000622e:	lea    0x208(%rbp),%r8
-   180006235:	lea    0x190(%rbp),%rdx
-   18000623c:	lea    0x140(%rbp),%rcx
-   180006243:	call   0x180006f82
-   180006248:	nop
-   180006249:	mov    %rax,%rcx
-   18000624c:	call   *0x2fb6(%rip)        # 0x180009208
-   180006252:	nop
-   180006253:	mov    0x158(%rbp),%rdx
-   18000625a:	cmp    $0x10,%rdx
-   18000625e:	jb     0x180006294
-   180006260:	inc    %rdx
-   180006263:	mov    0x140(%rbp),%rcx
-   18000626a:	mov    %rcx,%rax
-   18000626d:	cmp    $0x1000,%rdx
-   180006274:	jb     0x18000628f
-   180006276:	add    $0x27,%rdx
-   18000627a:	mov    -0x8(%rcx),%rcx
-   18000627e:	sub    %rcx,%rax
-   180006281:	add    $0xfffffffffffffff8,%rax
-   180006285:	cmp    $0x1f,%rax
-   180006289:	ja     0x18000655c
-   18000628f:	call   0x1800070f8
-   180006294:	mov    %r14d,%edx
-   180006297:	lea    0x70(%rsp),%rcx
-   18000629c:	call   *0x2e46(%rip)        # 0x1800090e8
-   1800062a2:	mov    %rax,%rcx
-   1800062a5:	lea    0x3548(%rip),%rdx        # 0x1800097f4
-   1800062ac:	call   0x180001290
-   1800062b1:	mov    %rax,%rcx
-   1800062b4:	movsd  0xe8(%rbp),%xmm1
-   1800062bc:	call   *0x2e1e(%rip)        # 0x1800090e0
-   1800062c2:	mov    %rax,%rcx
-   1800062c5:	lea    0x34ec(%rip),%rdx        # 0x1800097b8
-   1800062cc:	call   0x180001290
-   1800062d1:	mov    0x290(%rbp),%rdi
-   1800062d8:	test   %rdi,%rdi
-   1800062db:	je     0x180006393
-   1800062e1:	mov    0x298(%rbp),%rsi
-   1800062e8:	cmp    %rsi,%rdi
-   1800062eb:	je     0x180006344
-   1800062ed:	lea    0x10(%rdi),%rbx
-   1800062f1:	testb  $0x1,-0x8(%rbx)
-   1800062f5:	je     0x180006330
-   1800062f7:	mov    0x8(%rbx),%rax
-   1800062fb:	mov    (%rbx),%rcx
-   1800062fe:	lea    0x0(,%rax,4),%rdx
-   180006306:	cmp    $0x1000,%rdx
-   18000630d:	jb     0x18000632b
-   18000630f:	add    $0x27,%rdx
-   180006313:	mov    -0x8(%rcx),%r8
-   180006317:	sub    %r8,%rcx
-   18000631a:	lea    -0x8(%rcx),%rax
-   18000631e:	cmp    $0x1f,%rax
-   180006322:	ja     0x180006563
-   180006328:	mov    %r8,%rcx
-   18000632b:	call   0x1800070f8
-   180006330:	add    $0x20,%rbx
-   180006334:	lea    -0x10(%rbx),%rax
-   180006338:	cmp    %rsi,%rax
-   18000633b:	jne    0x1800062f1
-   18000633d:	mov    0x290(%rbp),%rdi
-   180006344:	mov    0x2a0(%rbp),%rdx
-   18000634b:	sub    %rdi,%rdx
-   18000634e:	and    $0xffffffffffffffe0,%rdx
-   180006352:	mov    %rdi,%rax
-   180006355:	cmp    $0x1000,%rdx
-   18000635c:	jb     0x180006377
-   18000635e:	add    $0x27,%rdx
-   180006362:	mov    -0x8(%rdi),%rdi
-   180006366:	sub    %rdi,%rax
-   180006369:	add    $0xfffffffffffffff8,%rax
-   18000636d:	cmp    $0x1f,%rax
-   180006371:	ja     0x180006563
-   180006377:	mov    %rdi,%rcx
-   18000637a:	call   0x1800070f8
-   18000637f:	xorps  %xmm0,%xmm0
-   180006382:	movdqa %xmm0,0x290(%rbp)
-   18000638a:	xor    %edi,%edi
-   18000638c:	mov    %rdi,0x2a0(%rbp)
-   180006393:	mov    0x278(%rbp),%rcx
-   18000639a:	test   %rcx,%rcx
-   18000639d:	je     0x1800063f1
-   18000639f:	mov    0x288(%rbp),%rax
-   1800063a6:	sub    %rcx,%rax
-   1800063a9:	sar    $0x3,%rax
-   1800063ad:	lea    0x0(,%rax,8),%rdx
-   1800063b5:	mov    %rcx,%rax
-   1800063b8:	cmp    $0x1000,%rdx
-   1800063bf:	jb     0x1800063da
-   1800063c1:	add    $0x27,%rdx
-   1800063c5:	mov    -0x8(%rcx),%rcx
-   1800063c9:	sub    %rcx,%rax
-   1800063cc:	add    $0xfffffffffffffff8,%rax
-   1800063d0:	cmp    $0x1f,%rax
-   1800063d4:	ja     0x180006563
-   1800063da:	call   0x1800070f8
-   1800063df:	mov    %rdi,0x278(%rbp)
-   1800063e6:	xorps  %xmm0,%xmm0
-   1800063e9:	movdqa %xmm0,0x280(%rbp)
-   1800063f1:	testb  $0x1,0x260(%rbp)
-   1800063f8:	je     0x18000643a
-   1800063fa:	mov    0x270(%rbp),%rax
-   180006401:	lea    0x0(,%rax,4),%rdx
-   180006409:	mov    0x268(%rbp),%rcx
-   180006410:	mov    %rcx,%rax
-   180006413:	cmp    $0x1000,%rdx
-   18000641a:	jb     0x180006435
-   18000641c:	add    $0x27,%rdx
-   180006420:	mov    -0x8(%rcx),%rcx
-   180006424:	sub    %rcx,%rax
-   180006427:	add    $0xfffffffffffffff8,%rax
-   18000642b:	cmp    $0x1f,%rax
-   18000642f:	ja     0x180006563
-   180006435:	call   0x1800070f8
-   18000643a:	testb  $0x1,0x248(%rbp)
-   180006441:	je     0x180006483
-   180006443:	mov    0x258(%rbp),%rax
-   18000644a:	lea    0x0(,%rax,4),%rdx
-   180006452:	mov    0x250(%rbp),%rcx
-   180006459:	mov    %rcx,%rax
-   18000645c:	cmp    $0x1000,%rdx
-   180006463:	jb     0x18000647e
-   180006465:	add    $0x27,%rdx
-   180006469:	mov    -0x8(%rcx),%rcx
-   18000646d:	sub    %rcx,%rax
-   180006470:	add    $0xfffffffffffffff8,%rax
-   180006474:	cmp    $0x1f,%rax
-   180006478:	ja     0x180006563
-   18000647e:	call   0x1800070f8
-   180006483:	lea    0x10(%r15),%rsi
-   180006487:	mov    0x28(%r15),%r9
-   18000648b:	mov    0x20(%r15),%r8
-   18000648f:	cmp    %r9,%r8
-   180006492:	jne    0x180005a96
-   180006498:	lea    0x3339(%rip),%rsi        # 0x1800097d8
-   18000649f:	mov    %r14d,%edx
-   1800064a2:	lea    0x70(%rsp),%rcx
-   1800064a7:	call   *0x2c3b(%rip)        # 0x1800090e8
-   1800064ad:	mov    %rax,%rcx
-   1800064b0:	lea    0x333d(%rip),%rdx        # 0x1800097f4
-   1800064b7:	call   0x180001290
-   1800064bc:	mov    %rax,%rcx
-   1800064bf:	movaps %xmm11,%xmm1
-   1800064c3:	call   *0x2c17(%rip)        # 0x1800090e0
-   1800064c9:	mov    %rax,%rcx
-   1800064cc:	lea    0x32e5(%rip),%rdx        # 0x1800097b8
-   1800064d3:	call   0x180001290
-   1800064d8:	cmpq   $0x0,-0x8(%rbp)
-   1800064dd:	je     0x18000656a
-   1800064e3:	mov    -0x70(%rbp),%rax
-   1800064e7:	lea    -0x18(%rbp),%rcx
-   1800064eb:	cmp    %rcx,(%rax)
-   1800064ee:	jne    0x18000650a
-   1800064f0:	mov    0x8(%rbp),%rdx
-   1800064f4:	mov    0x0(%rbp),%rcx
-   1800064f8:	mov    %rcx,(%rax)
-   1800064fb:	mov    -0x50(%rbp),%rax
-   1800064ff:	mov    %rcx,(%rax)
-   180006502:	sub    %ecx,%edx
-   180006504:	mov    -0x38(%rbp),%rax
-   180006508:	mov    %edx,(%rax)
-   18000650a:	lea    0x78(%rsp),%rbx
-   18000650f:	lea    0x78(%rsp),%rcx
-   180006514:	call   0x1800036f0
-   180006519:	test   %al,%al
-   18000651b:	cmove  %rdi,%rbx
-   18000651f:	mov    -0x8(%rbp),%rcx
-   180006523:	call   *0x2f27(%rip)        # 0x180009450
-   180006529:	test   %eax,%eax
-   18000652b:	cmovne %rdi,%rbx
-   18000652f:	movb   $0x0,-0xc(%rbp)
-   180006533:	movb   $0x0,-0x17(%rbp)
-   180006537:	lea    0x78(%rsp),%rcx
-   18000653c:	call   *0x2c86(%rip)        # 0x1800091c8
-   180006542:	mov    %rdi,-0x8(%rbp)
-   180006546:	mov    0x80e3(%rip),%rax        # 0x18000e630
-   18000654d:	mov    %rax,-0x14(%rbp)
-   180006551:	mov    %rdi,-0x20(%rbp)
-   180006555:	test   %rbx,%rbx
-   180006558:	jne    0x1800065ae
-   18000655a:	jmp    0x180006590
-   18000655c:	call   *0x2e56(%rip)        # 0x1800093b8
-   180006562:	nop
-   180006563:	call   *0x2e4f(%rip)        # 0x1800093b8
-   180006569:	int3
-   18000656a:	movb   $0x0,-0xc(%rbp)
-   18000656e:	movb   $0x0,-0x17(%rbp)
-   180006572:	lea    0x78(%rsp),%rcx
-   180006577:	call   *0x2c4b(%rip)        # 0x1800091c8
-   18000657d:	mov    %rdi,-0x8(%rbp)
-   180006581:	mov    0x80a8(%rip),%rax        # 0x18000e630
-   180006588:	mov    %rax,-0x14(%rbp)
-   18000658c:	mov    %rdi,-0x20(%rbp)
-   180006590:	mov    0x60(%rsp),%rax
-   180006595:	movslq 0x4(%rax),%rcx
-   180006599:	lea    0x60(%rsp),%rax
-   18000659e:	add    %rax,%rcx
-   1800065a1:	xor    %r8d,%r8d
-   1800065a4:	lea    0x2(%r8),%edx
-   1800065a8:	call   *0x2b52(%rip)        # 0x180009100
-   1800065ae:	lea    0x10(%r15),%rcx
-   1800065b2:	lea    0x1c0(%rbp),%rdx
-   1800065b9:	call   0x180006f4c
-   1800065be:	mov    0x1f0(%rbp),%rcx
-   1800065c5:	test   %rcx,%rcx
-   1800065c8:	je     0x18000661c
-   1800065ca:	mov    0x200(%rbp),%rax
-   1800065d1:	sub    %rcx,%rax
-   1800065d4:	sar    $0x2,%rax
-   1800065d8:	lea    0x0(,%rax,4),%rdx
-   1800065e0:	mov    %rcx,%rax
-   1800065e3:	cmp    $0x1000,%rdx
-   1800065ea:	jb     0x180006605
-   1800065ec:	add    $0x27,%rdx
-   1800065f0:	mov    -0x8(%rcx),%rcx
-   1800065f4:	sub    %rcx,%rax
-   1800065f7:	add    $0xfffffffffffffff8,%rax
-   1800065fb:	cmp    $0x1f,%rax
-   1800065ff:	ja     0x1800066b9
-   180006605:	call   0x1800070f8
-   18000660a:	mov    %rdi,0x1f0(%rbp)
-   180006611:	xorps  %xmm0,%xmm0
-   180006614:	movdqu %xmm0,0x1f8(%rbp)
-   18000661c:	mov    0x1d8(%rbp),%rcx
-   180006623:	test   %rcx,%rcx
-   180006626:	je     0x180006676
-   180006628:	mov    0x1e8(%rbp),%rax
-   18000662f:	sub    %rcx,%rax
-   180006632:	sar    $0x2,%rax
-   180006636:	lea    0x0(,%rax,4),%rdx
-   18000663e:	mov    %rcx,%rax
-   180006641:	cmp    $0x1000,%rdx
-   180006648:	jb     0x18000665f
-   18000664a:	add    $0x27,%rdx
-   18000664e:	mov    -0x8(%rcx),%rcx
-   180006652:	sub    %rcx,%rax
-   180006655:	add    $0xfffffffffffffff8,%rax
-   180006659:	cmp    $0x1f,%rax
-   18000665d:	ja     0x1800066b9
-   18000665f:	call   0x1800070f8
-   180006664:	mov    %rdi,0x1d8(%rbp)
-   18000666b:	xorps  %xmm0,%xmm0
-   18000666e:	movdqu %xmm0,0x1e0(%rbp)
-   180006676:	mov    0x1c0(%rbp),%rcx
-   18000667d:	test   %rcx,%rcx
-   180006680:	je     0x1800066c5
-   180006682:	mov    0x1d0(%rbp),%rax
-   180006689:	sub    %rcx,%rax
-   18000668c:	sar    $0x2,%rax
-   180006690:	lea    0x0(,%rax,4),%rdx
-   180006698:	mov    %rcx,%rax
-   18000669b:	cmp    $0x1000,%rdx
-   1800066a2:	jb     0x1800066c0
-   1800066a4:	add    $0x27,%rdx
-   1800066a8:	mov    -0x8(%rcx),%rcx
-   1800066ac:	sub    %rcx,%rax
-   1800066af:	add    $0xfffffffffffffff8,%rax
-   1800066b3:	cmp    $0x1f,%rax
-   1800066b7:	jbe    0x1800066c0
-   1800066b9:	call   *0x2cf9(%rip)        # 0x1800093b8
-   1800066bf:	int3
-   1800066c0:	call   0x1800070f8
-   1800066c5:	mov    (%r15),%rcx
-   1800066c8:	call   *0x2ba2(%rip)        # 0x180009270
-   1800066ce:	lea    0x1d0(%rbp),%rdx
-   1800066d5:	mov    %eax,%ecx
-   1800066d7:	call   0x180006f7c
-   1800066dc:	lea    0x1c0(%rbp),%rcx
-   1800066e3:	sub    %rcx,%r13
-   1800066e6:	add    %r13,%rax
-   1800066e9:	lea    0x1d0(%rbp),%rcx
-   1800066f0:	mov    %rcx,0x1c0(%rbp)
-   1800066f7:	mov    %rax,0x1c8(%rbp)
-   1800066fe:	mov    %rsi,0x2d0(%rbp)
-   180006705:	mov    %rsi,%rax
-   180006708:	inc    %rax
-   18000670b:	cmpb   $0x0,(%rax)
-   18000670e:	jne    0x180006708
-   180006710:	sub    %rsi,%rax
-   180006713:	mov    %rax,0x2d8(%rbp)
-   18000671a:	lea    0x30d7(%rip),%rcx        # 0x1800097f8
-   180006721:	mov    %rcx,0x160(%rbp)
-   180006728:	mov    %rcx,%rax
-   18000672b:	nopl   0x0(%rax,%rax,1)
-   180006730:	inc    %rax
-   180006733:	cmpb   $0x0,(%rax)
-   180006736:	jne    0x180006730
-   180006738:	sub    %rcx,%rax
-   18000673b:	mov    %rax,0x168(%rbp)
-   180006742:	lea    0x1c0(%rbp),%r9
-   180006749:	lea    0x2d0(%rbp),%r8
-   180006750:	lea    0x160(%rbp),%rdx
-   180006757:	lea    0x2b0(%rbp),%rcx
-   18000675e:	call   0x180006f82
-   180006763:	nop
-   180006764:	mov    %rax,%rcx
-   180006767:	call   *0x2a9b(%rip)        # 0x180009208
-   18000676d:	nop
-   18000676e:	mov    0x2c8(%rbp),%rdx
-   180006775:	cmp    $0x10,%rdx
-   180006779:	jb     0x1800067b2
-   18000677b:	inc    %rdx
-   18000677e:	mov    0x2b0(%rbp),%rcx
-   180006785:	mov    %rcx,%rax
-   180006788:	cmp    $0x1000,%rdx
-   18000678f:	jb     0x1800067ad
-   180006791:	add    $0x27,%rdx
-   180006795:	mov    -0x8(%rcx),%rcx
-   180006799:	sub    %rcx,%rax
-   18000679c:	add    $0xfffffffffffffff8,%rax
-   1800067a0:	cmp    $0x1f,%rax
-   1800067a4:	jbe    0x1800067ad
-   1800067a6:	call   *0x2c0c(%rip)        # 0x1800093b8
-   1800067ac:	int3
-   1800067ad:	call   0x1800070f8
-   1800067b2:	mov    (%r15),%rcx
-   1800067b5:	call   *0x2af5(%rip)        # 0x1800092b0
-   1800067bb:	lea    0x2eae(%rip),%rcx        # 0x180009670
-   1800067c2:	mov    %rcx,0x140(%rbp)
-   1800067c9:	mov    %rcx,%rax
-   1800067cc:	cmpb   $0x0,0x2e9d(%rip)        # 0x180009670
-   1800067d3:	je     0x1800067dd
-   1800067d5:	inc    %rax
-   1800067d8:	cmpb   $0x0,(%rax)
-   1800067db:	jne    0x1800067d5
-   1800067dd:	sub    %rcx,%rax
-   1800067e0:	mov    %rax,0x148(%rbp)
-   1800067e7:	movaps 0x140(%rbp),%xmm0
-   1800067ee:	movdqa %xmm0,0x140(%rbp)
-   1800067f6:	mov    (%r15),%rcx
-   1800067f9:	call   *0x2a89(%rip)        # 0x180009288
-   1800067ff:	mov    %rax,%rcx
-   180006802:	lea    0x140(%rbp),%rdx
-   180006809:	call   *0x29f1(%rip)        # 0x180009200
-   18000680f:	lea    0x2ffa(%rip),%rcx        # 0x180009810
-   180006816:	mov    %rcx,0x140(%rbp)
-   18000681d:	mov    %rcx,%rax
-   180006820:	inc    %rax
-   180006823:	cmpb   $0x0,(%rax)
-   180006826:	jne    0x180006820
-   180006828:	sub    %rcx,%rax
-   18000682b:	mov    %rax,0x148(%rbp)
-   180006832:	movaps 0x140(%rbp),%xmm0
-   180006839:	movdqa %xmm0,0x140(%rbp)
-   180006841:	lea    0x140(%rbp),%rdx
-   180006848:	mov    (%r15),%rcx
-   18000684b:	call   0x180006f64
-   180006850:	nop
-   180006851:	mov    0x60(%rsp),%rax
-   180006856:	movslq 0x4(%rax),%rcx
-   18000685a:	lea    0x2ea7(%rip),%rax        # 0x180009708
-   180006861:	mov    %rax,0x60(%rsp,%rcx,1)
-   180006866:	mov    0x60(%rsp),%rax
-   18000686b:	movslq 0x4(%rax),%rcx
-   18000686f:	lea    -0xb8(%rcx),%edx
-   180006875:	mov    %edx,0x5c(%rsp,%rcx,1)
-   180006879:	lea    0x78(%rsp),%rcx
-   18000687e:	call   0x180002d00
-   180006883:	lea    -0x80(%rbp),%rcx
-   180006887:	call   *0x283b(%rip)        # 0x1800090c8
-   18000688d:	lea    0x18(%rbp),%rcx
-   180006891:	call   *0x2879(%rip)        # 0x180009110
-   180006897:	mov    0x300(%rbp),%rcx
-   18000689e:	xor    %rsp,%rcx
-   1800068a1:	call   0x180007240
-   1800068a6:	lea    0x490(%rsp),%r11
-   1800068ae:	mov    0x38(%r11),%rbx
-   1800068b2:	mov    0x40(%r11),%rsi
-   1800068b6:	mov    0x48(%r11),%rdi
-   1800068ba:	movaps -0x10(%r11),%xmm6
-   1800068bf:	movaps -0x20(%r11),%xmm7
-   1800068c4:	movaps -0x30(%r11),%xmm8
-   1800068c9:	movaps -0x40(%r11),%xmm9
-   1800068ce:	movaps -0x50(%r11),%xmm10
-   1800068d3:	movaps -0x60(%r11),%xmm11
-   1800068d8:	movaps -0x70(%r11),%xmm12
-   1800068dd:	movaps -0x80(%r11),%xmm13
-   1800068e2:	mov    %r11,%rsp
-   1800068e5:	pop    %r15
-   1800068e7:	pop    %r14
-   1800068e9:	pop    %r13
-   1800068eb:	pop    %r12
-   1800068ed:	pop    %rbp
-   1800068ee:	ret
-   1800068ef:	int3
-   1800068f0:	rex push %rbx
-   1800068f2:	sub    $0x20,%rsp
-   1800068f6:	cmpq   $0x0,0x80(%rcx)
-   1800068fe:	mov    %rcx,%rbx
-   180006901:	je     0x180006930
-   180006903:	mov    (%rcx),%r8
-   180006906:	mov    $0xffffffff,%edx
-   18000690b:	call   *0x18(%r8)
-   18000690f:	cmp    $0xffffffff,%eax
-   180006912:	je     0x180006930
-   180006914:	mov    0x80(%rbx),%rcx
-   18000691b:	call   *0x2b27(%rip)        # 0x180009448
-   180006921:	test   %eax,%eax
-   180006923:	jns    0x180006930
-   180006925:	mov    $0xffffffff,%eax
-   18000692a:	add    $0x20,%rsp
-   18000692e:	pop    %rbx
-   18000692f:	ret
-   180006930:	xor    %eax,%eax
-   180006932:	add    $0x20,%rsp
-   180006936:	pop    %rbx
-   180006937:	ret
-   180006938:	int3
-   180006939:	int3
-   18000693a:	int3
-   18000693b:	int3
-   18000693c:	int3
-   18000693d:	int3
-   18000693e:	int3
-   18000693f:	int3
-   180006940:	rex push %rbx
-   180006942:	sub    $0x20,%rsp
-   180006946:	mov    %rdx,%rbx
-   180006949:	lea    0x78e8(%rip),%rcx        # 0x18000e238
-   180006950:	lea    0x7cf9(%rip),%rdx        # 0x18000e650
-   180006957:	call   0x180007fce
-   18000695c:	mov    %rax,(%rbx)
-   18000695f:	test   %rax,%rax
-   180006962:	je     0x180006988
-   180006964:	cmpb   $0x0,(%rax)
-   180006967:	mov    %rax,%rcx
-   18000696a:	je     0x180006978
-   18000696c:	nopl   0x0(%rax)
-   180006970:	inc    %rcx
-   180006973:	cmpb   $0x0,(%rcx)
-   180006976:	jne    0x180006970
-   180006978:	sub    %rax,%rcx
-   18000697b:	mov    %rbx,%rax
-   18000697e:	mov    %rcx,0x8(%rbx)
-   180006982:	add    $0x20,%rsp
-   180006986:	pop    %rbx
-   180006987:	ret
-   180006988:	movq   $0x0,0x8(%rbx)
-   180006990:	mov    %rbx,%rax
-   180006993:	add    $0x20,%rsp
-   180006997:	pop    %rbx
-   180006998:	ret
-   180006999:	int3
-   18000699a:	int3
-   18000699b:	int3
-   18000699c:	int3
-   18000699d:	int3
-   18000699e:	int3
-   18000699f:	int3
-   1800069a0:	mov    %rbx,0x10(%rsp)
-   1800069a5:	mov    %rdi,0x18(%rsp)
-   1800069aa:	push   %rbp
-   1800069ab:	mov    %rsp,%rbp
-   1800069ae:	sub    $0x80,%rsp
-   1800069b5:	mov    0x764c(%rip),%rax        # 0x18000e008
-   1800069bc:	xor    %rsp,%rax
-   1800069bf:	mov    %rax,-0x8(%rbp)
-   1800069c3:	mov    %rcx,%rdi
-   1800069c6:	mov    0x38(%rcx),%rax
-   1800069ca:	mov    (%rax),%rcx
-   1800069cd:	test   %rcx,%rcx
-   1800069d0:	je     0x1800069fe
-   1800069d2:	mov    0x50(%rdi),%rdx
-   1800069d6:	movslq (%rdx),%r8
-   1800069d9:	lea    (%rcx,%r8,1),%rax
-   1800069dd:	cmp    %rax,%rcx
-   1800069e0:	jae    0x1800069fe
-   1800069e2:	lea    -0x1(%r8),%eax
-   1800069e6:	mov    %eax,(%rdx)
-   1800069e8:	mov    0x38(%rdi),%rcx
-   1800069ec:	mov    (%rcx),%rdx
-   1800069ef:	lea    0x1(%rdx),%rax
-   1800069f3:	mov    %rax,(%rcx)
-   1800069f6:	movzbl (%rdx),%eax
-   1800069f9:	jmp    0x180006c2a
-   1800069fe:	cmpq   $0x0,0x80(%rdi)
-   180006a06:	jne    0x180006a12
-   180006a08:	mov    $0xffffffff,%eax
-   180006a0d:	jmp    0x180006c2a
-   180006a12:	mov    0x18(%rdi),%r8
-   180006a16:	lea    0x70(%rdi),%rax
-   180006a1a:	cmp    %rax,(%r8)
-   180006a1d:	jne    0x180006a3f
-   180006a1f:	mov    0x90(%rdi),%rdx
-   180006a26:	mov    0x88(%rdi),%rcx
-   180006a2d:	mov    %rcx,(%r8)
-   180006a30:	mov    0x38(%rdi),%rax
-   180006a34:	mov    %rcx,(%rax)
-   180006a37:	sub    %ecx,%edx
-   180006a39:	mov    0x50(%rdi),%rax
-   180006a3d:	mov    %edx,(%rax)
-   180006a3f:	mov    0x80(%rdi),%rcx
-   180006a46:	cmpq   $0x0,0x68(%rdi)
-   180006a4b:	jne    0x180006a69
-   180006a4d:	call   *0x29ed(%rip)        # 0x180009440
-   180006a53:	cmp    $0xffffffff,%eax
-   180006a56:	mov    $0xffffffff,%ebx
-   180006a5b:	je     0x180006c28
-   180006a61:	movzbl %al,%ebx
-   180006a64:	jmp    0x180006c28
-   180006a69:	xor    %eax,%eax
-   180006a6b:	mov    %rax,-0x28(%rbp)
-   180006a6f:	mov    %rax,-0x18(%rbp)
-   180006a73:	movq   $0xf,-0x10(%rbp)
-   180006a7b:	mov    %al,-0x28(%rbp)
-   180006a7e:	call   *0x29bc(%rip)        # 0x180009440
-   180006a84:	cmp    $0xffffffff,%eax
-   180006a87:	mov    %eax,%r8d
-   180006a8a:	je     0x180006be5
-   180006a90:	mov    -0x18(%rbp),%rcx
-   180006a94:	mov    -0x10(%rbp),%rdx
-   180006a98:	cmp    %rdx,%rcx
-   180006a9b:	jae    0x180006abd
-   180006a9d:	lea    0x1(%rcx),%rax
-   180006aa1:	mov    %rax,-0x18(%rbp)
-   180006aa5:	lea    -0x28(%rbp),%rax
-   180006aa9:	cmp    $0x10,%rdx
-   180006aad:	cmovae -0x28(%rbp),%rax
-   180006ab2:	mov    %r8b,(%rax,%rcx,1)
-   180006ab6:	movb   $0x0,0x1(%rax,%rcx,1)
-   180006abb:	jmp    0x180006ad1
-   180006abd:	movzbl %r8b,%r9d
-   180006ac1:	xor    %r8d,%r8d
-   180006ac4:	lea    0x1(%r8),%edx
-   180006ac8:	lea    -0x28(%rbp),%rcx
-   180006acc:	call   0x180001ad0
-   180006ad1:	lea    -0x28(%rbp),%rdx
-   180006ad5:	cmpq   $0x10,-0x10(%rbp)
-   180006ada:	cmovae -0x28(%rbp),%rdx
-   180006adf:	lea    -0x28(%rbp),%r8
-   180006ae3:	cmovae -0x28(%rbp),%r8
-   180006ae8:	mov    -0x18(%rbp),%r9
-   180006aec:	add    %rdx,%r9
-   180006aef:	lea    -0x30(%rbp),%rax
-   180006af3:	mov    %rax,0x38(%rsp)
-   180006af8:	lea    -0x3f(%rbp),%rax
-   180006afc:	mov    %rax,0x30(%rsp)
-   180006b01:	lea    -0x40(%rbp),%rax
-   180006b05:	mov    %rax,0x28(%rsp)
-   180006b0a:	lea    -0x38(%rbp),%rax
-   180006b0e:	mov    %rax,0x20(%rsp)
-   180006b13:	lea    0x74(%rdi),%rdx
-   180006b17:	mov    0x68(%rdi),%rcx
-   180006b1b:	call   *0x2657(%rip)        # 0x180009178
-   180006b21:	test   %eax,%eax
-   180006b23:	je     0x180006b2a
-   180006b25:	sub    $0x1,%eax
-   180006b28:	jne    0x180006b81
-   180006b2a:	lea    -0x40(%rbp),%rax
-   180006b2e:	cmp    %rax,-0x30(%rbp)
-   180006b32:	lea    -0x28(%rbp),%rax
-   180006b36:	jne    0x180006b99
-   180006b38:	cmpq   $0x10,-0x10(%rbp)
-   180006b3d:	cmovae -0x28(%rbp),%rax
-   180006b42:	mov    -0x38(%rbp),%r10
-   180006b46:	sub    %rax,%r10
-   180006b49:	mov    -0x18(%rbp),%r8
-   180006b4d:	cmp    %r10,%r8
-   180006b50:	cmovb  %r8,%r10
-   180006b54:	lea    -0x28(%rbp),%rcx
-   180006b58:	cmpq   $0x10,-0x10(%rbp)
-   180006b5d:	cmovae -0x28(%rbp),%rcx
-   180006b62:	sub    %r10,%r8
-   180006b65:	mov    %r8,-0x18(%rbp)
-   180006b69:	inc    %r8
-   180006b6c:	lea    (%rcx,%r10,1),%rdx
-   180006b70:	call   0x180007fe0
-   180006b75:	mov    0x80(%rdi),%rcx
-   180006b7c:	jmp    0x180006a7e
-   180006b81:	cmp    $0x2,%eax
-   180006b84:	jne    0x180006be5
-   180006b86:	lea    -0x28(%rbp),%rax
-   180006b8a:	cmpq   $0x10,-0x10(%rbp)
-   180006b8f:	cmovae -0x28(%rbp),%rax
-   180006b94:	movsbl (%rax),%ebx
-   180006b97:	jmp    0x180006bea
-   180006b99:	cmpq   $0x10,-0x10(%rbp)
-   180006b9e:	cmovae -0x28(%rbp),%rax
-   180006ba3:	mov    -0x18(%rbp),%rbx
-   180006ba7:	mov    -0x38(%rbp),%rcx
-   180006bab:	sub    %rcx,%rbx
-   180006bae:	add    %rax,%rbx
-   180006bb1:	test   %rbx,%rbx
-   180006bb4:	jle    0x180006bdf
-   180006bb6:	data16 nopw 0x0(%rax,%rax,1)
-   180006bc0:	dec    %rbx
-   180006bc3:	movsbl (%rbx,%rcx,1),%ecx
-   180006bc7:	mov    0x80(%rdi),%rdx
-   180006bce:	call   *0x285c(%rip)        # 0x180009430
-   180006bd4:	test   %rbx,%rbx
-   180006bd7:	jle    0x180006bdf
-   180006bd9:	mov    -0x38(%rbp),%rcx
-   180006bdd:	jmp    0x180006bc0
-   180006bdf:	movzbl -0x40(%rbp),%ebx
-   180006be3:	jmp    0x180006bea
-   180006be5:	mov    $0xffffffff,%ebx
-   180006bea:	mov    -0x10(%rbp),%rdx
-   180006bee:	cmp    $0x10,%rdx
-   180006bf2:	jb     0x180006c28
-   180006bf4:	inc    %rdx
-   180006bf7:	mov    -0x28(%rbp),%rcx
-   180006bfb:	mov    %rcx,%rax
-   180006bfe:	cmp    $0x1000,%rdx
-   180006c05:	jb     0x180006c23
-   180006c07:	add    $0x27,%rdx
-   180006c0b:	mov    -0x8(%rcx),%rcx
-   180006c0f:	sub    %rcx,%rax
-   180006c12:	add    $0xfffffffffffffff8,%rax
-   180006c16:	cmp    $0x1f,%rax
-   180006c1a:	jbe    0x180006c23
-   180006c1c:	call   *0x2796(%rip)        # 0x1800093b8
-   180006c22:	int3
-   180006c23:	call   0x1800070f8
-   180006c28:	mov    %ebx,%eax
-   180006c2a:	mov    -0x8(%rbp),%rcx
-   180006c2e:	xor    %rsp,%rcx
-   180006c31:	call   0x180007240
-   180006c36:	lea    0x80(%rsp),%r11
-   180006c3e:	mov    0x18(%r11),%rbx
-   180006c42:	mov    0x20(%r11),%rdi
-   180006c46:	mov    %r11,%rsp
-   180006c49:	pop    %rbp
-   180006c4a:	ret
-   180006c4b:	int3
-   180006c4c:	int3
-   180006c4d:	int3
-   180006c4e:	int3
-   180006c4f:	int3
-   180006c50:	rex push %rbx
-   180006c52:	sub    $0x20,%rsp
-   180006c56:	mov    0x38(%rcx),%rax
-   180006c5a:	mov    %rcx,%rbx
-   180006c5d:	mov    (%rax),%rcx
-   180006c60:	test   %rcx,%rcx
-   180006c63:	je     0x180006c7d
-   180006c65:	mov    0x50(%rbx),%rax
-   180006c69:	movslq (%rax),%rdx
-   180006c6c:	add    %rcx,%rdx
-   180006c6f:	cmp    %rdx,%rcx
-   180006c72:	jae    0x180006c7d
-   180006c74:	movzbl (%rcx),%eax
-   180006c77:	add    $0x20,%rsp
-   180006c7b:	pop    %rbx
-   180006c7c:	ret
-   180006c7d:	mov    (%rbx),%rax
-   180006c80:	mov    %rbx,%rcx
-   180006c83:	mov    %rdi,0x30(%rsp)
-   180006c88:	call   *0x38(%rax)
-   180006c8b:	mov    %eax,%edi
-   180006c8d:	cmp    $0xffffffff,%eax
-   180006c90:	jne    0x180006c9d
-   180006c92:	mov    0x30(%rsp),%rdi
-   180006c97:	add    $0x20,%rsp
-   180006c9b:	pop    %rbx
-   180006c9c:	ret
-   180006c9d:	mov    (%rbx),%rax
-   180006ca0:	mov    %edi,%edx
-   180006ca2:	mov    %rbx,%rcx
-   180006ca5:	call   *0x20(%rax)
-   180006ca8:	mov    %edi,%eax
-   180006caa:	mov    0x30(%rsp),%rdi
-   180006caf:	add    $0x20,%rsp
-   180006cb3:	pop    %rbx
-   180006cb4:	ret
-   180006cb5:	int3
-   180006cb6:	int3
-   180006cb7:	int3
-   180006cb8:	int3
-   180006cb9:	int3
-   180006cba:	int3
-   180006cbb:	int3
-   180006cbc:	int3
-   180006cbd:	int3
-   180006cbe:	int3
-   180006cbf:	int3
-   180006cc0:	mov    %edx,%eax
-   180006cc2:	lea    (%rax,%rax,4),%rdx
-   180006cc6:	mov    0x58(%rcx),%rax
-   180006cca:	lea    (%rax,%rdx,8),%rax
-   180006cce:	ret
-   180006ccf:	int3
-   180006cd0:	mov    0x8(%rcx),%rdx
-   180006cd4:	lea    0x285d(%rip),%rax        # 0x180009538
-   180006cdb:	test   %rdx,%rdx
-   180006cde:	cmovne %rdx,%rax
-   180006ce2:	ret
-   180006ce3:	int3
-   180006ce4:	int3
-   180006ce5:	int3
-   180006ce6:	int3
-   180006ce7:	int3
-   180006ce8:	int3
-   180006ce9:	int3
-   180006cea:	int3
-   180006ceb:	int3
-   180006cec:	int3
-   180006ced:	int3
-   180006cee:	int3
-   180006cef:	int3
-   180006cf0:	mov    %rbp,0x18(%rsp)
-   180006cf5:	mov    %rsi,0x20(%rsp)
-   180006cfa:	push   %r14
-   180006cfc:	sub    $0x20,%rsp
-   180006d00:	mov    %r8,%rbp
-   180006d03:	mov    %rdx,%r14
-   180006d06:	mov    %rcx,%rsi
-   180006d09:	test   %r8,%r8
-   180006d0c:	jg     0x180006d21
-   180006d0e:	xor    %eax,%eax
-   180006d10:	mov    0x40(%rsp),%rbp
-   180006d15:	mov    0x48(%rsp),%rsi
-   180006d1a:	add    $0x20,%rsp
-   180006d1e:	pop    %r14
-   180006d20:	ret
-   180006d21:	cmpq   $0x0,0x68(%rcx)
-   180006d26:	je     0x180006d3f
-   180006d28:	mov    0x40(%rsp),%rbp
-   180006d2d:	mov    0x48(%rsp),%rsi
-   180006d32:	add    $0x20,%rsp
-   180006d36:	pop    %r14
-   180006d38:	rex.W jmp *0x23e1(%rip)        # 0x180009120
-   180006d3f:	mov    0x38(%rcx),%rax
-   180006d43:	mov    %rbx,0x30(%rsp)
-   180006d48:	mov    %rdi,0x38(%rsp)
-   180006d4d:	mov    %rbp,%rdi
-   180006d50:	mov    (%rax),%rdx
-   180006d53:	test   %rdx,%rdx
-   180006d56:	je     0x180006d60
-   180006d58:	mov    0x50(%rcx),%rax
-   180006d5c:	mov    (%rax),%ecx
-   180006d5e:	jmp    0x180006d62
-   180006d60:	xor    %ecx,%ecx
-   180006d62:	movslq %ecx,%rax
-   180006d65:	test   %ecx,%ecx
-   180006d67:	je     0x180006d94
-   180006d69:	cmp    %rbp,%rax
-   180006d6c:	mov    %rbp,%rbx
-   180006d6f:	mov    %r14,%rcx
-   180006d72:	cmovb  %rax,%rbx
-   180006d76:	mov    %rbx,%r8
-   180006d79:	call   0x180007fda
-   180006d7e:	mov    0x50(%rsi),%rax
-   180006d82:	add    %rbx,%r14
-   180006d85:	sub    %rbx,%rdi
-   180006d88:	sub    %ebx,(%rax)
-   180006d8a:	mov    0x38(%rsi),%rcx
-   180006d8e:	movslq %ebx,%rax
-   180006d91:	add    %rax,(%rcx)
-   180006d94:	cmpq   $0x0,0x80(%rsi)
-   180006d9c:	mov    %rdi,%rbx
-   180006d9f:	je     0x180006e31
-   180006da5:	mov    0x18(%rsi),%r8
-   180006da9:	lea    0x70(%rsi),%rax
-   180006dad:	cmp    %rax,(%r8)
-   180006db0:	jne    0x180006dd2
-   180006db2:	mov    0x88(%rsi),%rcx
-   180006db9:	mov    0x90(%rsi),%rdx
-   180006dc0:	mov    %rcx,(%r8)
-   180006dc3:	sub    %ecx,%edx
-   180006dc5:	mov    0x38(%rsi),%rax
-   180006dc9:	mov    %rcx,(%rax)
-   180006dcc:	mov    0x50(%rsi),%rax
-   180006dd0:	mov    %edx,(%rax)
-   180006dd2:	cmp    $0xfff,%rdi
-   180006dd9:	jbe    0x180006e11
-   180006ddb:	nopl   0x0(%rax,%rax,1)
-   180006de0:	mov    0x80(%rsi),%r9
-   180006de7:	mov    $0x1,%edx
-   180006dec:	mov    $0xfff,%r8d
-   180006df2:	mov    %r14,%rcx
-   180006df5:	call   *0x262d(%rip)        # 0x180009428
-   180006dfb:	sub    %rax,%rdi
-   180006dfe:	add    %rax,%r14
-   180006e01:	mov    %rdi,%rbx
-   180006e04:	cmp    $0xfff,%rax
-   180006e0a:	jne    0x180006e52
-   180006e0c:	cmp    %rax,%rdi
-   180006e0f:	ja     0x180006de0
-   180006e11:	test   %rbx,%rbx
-   180006e14:	je     0x180006e31
-   180006e16:	mov    0x80(%rsi),%r9
-   180006e1d:	mov    %rdi,%r8
-   180006e20:	mov    $0x1,%edx
-   180006e25:	mov    %r14,%rcx
-   180006e28:	call   *0x25fa(%rip)        # 0x180009428
-   180006e2e:	sub    %rax,%rbx
-   180006e31:	sub    %rbx,%rbp
-   180006e34:	mov    0x30(%rsp),%rbx
-   180006e39:	mov    %rbp,%rax
-   180006e3c:	mov    0x40(%rsp),%rbp
-   180006e41:	mov    0x38(%rsp),%rdi
-   180006e46:	mov    0x48(%rsp),%rsi
-   180006e4b:	add    $0x20,%rsp
-   180006e4f:	pop    %r14
-   180006e51:	ret
-   180006e52:	sub    %rdi,%rbp
-   180006e55:	jmp    0x180006e34
-   180006e57:	int3
-   180006e58:	int3
-   180006e59:	int3
-   180006e5a:	int3
-   180006e5b:	int3
-   180006e5c:	int3
-   180006e5d:	int3
-   180006e5e:	int3
-   180006e5f:	int3
-   180006e60:	mov    %rbx,0x18(%rsp)
-   180006e65:	mov    %rdi,0x20(%rsp)
-   180006e6a:	push   %r14
-   180006e6c:	sub    $0x20,%rsp
-   180006e70:	cmpq   $0x0,0x68(%rcx)
-   180006e75:	mov    %r8,%rbx
-   180006e78:	mov    %rdx,%r14
-   180006e7b:	mov    %rcx,%rdi
-   180006e7e:	je     0x180006e97
-   180006e80:	mov    0x40(%rsp),%rbx
-   180006e85:	mov    0x48(%rsp),%rdi
-   180006e8a:	add    $0x20,%rsp
-   180006e8e:	pop    %r14
-   180006e90:	rex.W jmp *0x2281(%rip)        # 0x180009118
-   180006e97:	mov    0x40(%rcx),%rax
-   180006e9b:	mov    %rbp,0x30(%rsp)
-   180006ea0:	mov    %rsi,0x38(%rsp)
-   180006ea5:	mov    %rbx,%rsi
-   180006ea8:	mov    (%rax),%r9
-   180006eab:	test   %r9,%r9
-   180006eae:	je     0x180006eb8
-   180006eb0:	mov    0x58(%rcx),%rax
-   180006eb4:	mov    (%rax),%ecx
-   180006eb6:	jmp    0x180006eba
-   180006eb8:	xor    %ecx,%ecx
-   180006eba:	movslq %ecx,%rbp
-   180006ebd:	test   %rbx,%rbx
-   180006ec0:	jle    0x180006f13
-   180006ec2:	test   %ecx,%ecx
-   180006ec4:	jle    0x180006ef3
-   180006ec6:	cmp    %rbp,%rbx
-   180006ec9:	mov    %r9,%rcx
-   180006ecc:	cmovl  %rbx,%rbp
-   180006ed0:	mov    %rbp,%r8
-   180006ed3:	call   0x180007fda
-   180006ed8:	mov    0x58(%rdi),%rax
-   180006edc:	sub    %rbp,%rbx
-   180006edf:	add    %rbp,%r14
-   180006ee2:	sub    %ebp,(%rax)
-   180006ee4:	mov    0x40(%rdi),%rcx
-   180006ee8:	movslq %ebp,%rax
-   180006eeb:	add    %rax,(%rcx)
-   180006eee:	test   %rbx,%rbx
-   180006ef1:	jle    0x180006f13
-   180006ef3:	mov    0x80(%rdi),%r9
-   180006efa:	test   %r9,%r9
-   180006efd:	je     0x180006f13
-   180006eff:	mov    %rbx,%r8
-   180006f02:	mov    $0x1,%edx
-   180006f07:	mov    %r14,%rcx
-   180006f0a:	call   *0x2500(%rip)        # 0x180009410
-   180006f10:	sub    %rax,%rbx
-   180006f13:	mov    0x30(%rsp),%rbp
-   180006f18:	sub    %rbx,%rsi
-   180006f1b:	mov    0x40(%rsp),%rbx
-   180006f20:	mov    %rsi,%rax
-   180006f23:	mov    0x38(%rsp),%rsi
-   180006f28:	mov    0x48(%rsp),%rdi
-   180006f2d:	add    $0x20,%rsp
-   180006f31:	pop    %r14
-   180006f33:	ret
-   180006f34:	jmp    *0x20c6(%rip)        # 0x180009000
-   180006f3a:	jmp    *0x20c8(%rip)        # 0x180009008
-   180006f40:	jmp    *0x20ca(%rip)        # 0x180009010
-   180006f46:	jmp    *0x20cc(%rip)        # 0x180009018
-   180006f4c:	jmp    *0x20ce(%rip)        # 0x180009020
-   180006f52:	jmp    *0x20d0(%rip)        # 0x180009028
-   180006f58:	jmp    *0x2322(%rip)        # 0x180009280
-   180006f5e:	jmp    *0x2344(%rip)        # 0x1800092a8
-   180006f64:	jmp    *0x22ee(%rip)        # 0x180009258
-   180006f6a:	jmp    *0x22d0(%rip)        # 0x180009240
-   180006f70:	jmp    *0x22ba(%rip)        # 0x180009230
-   180006f76:	jmp    *0x22ac(%rip)        # 0x180009228
-   180006f7c:	jmp    *0x23c6(%rip)        # 0x180009348
-   180006f82:	jmp    *0x23b8(%rip)        # 0x180009340
-   180006f88:	jmp    *0x21ba(%rip)        # 0x180009148
-   180006f8e:	jmp    *0x21bc(%rip)        # 0x180009150
-   180006f94:	jmp    *0x21be(%rip)        # 0x180009158
-   180006f9a:	int3
-   180006f9b:	int3
-   180006f9c:	rex push %rbx
-   180006f9e:	sub    $0x20,%rsp
-   180006fa2:	mov    %rcx,%rbx
-   180006fa5:	mov    $0x10,%ecx
-   180006faa:	call   0x1800070bc
-   180006faf:	mov    %rax,0x38(%rsp)
-   180006fb4:	test   %rax,%rax
-   180006fb7:	je     0x180006fc7
-   180006fb9:	mov    0x7680(%rip),%rdx        # 0x18000e640
-   180006fc0:	mov    %rdx,(%rax)
-   180006fc3:	mov    %rbx,0x8(%rax)
-   180006fc7:	mov    %rax,0x7672(%rip)        # 0x18000e640
-   180006fce:	add    $0x20,%rsp
-   180006fd2:	pop    %rbx
-   180006fd3:	ret
-   180006fd4:	jmp    *0x218e(%rip)        # 0x180009168
-   180006fda:	jmp    *0x21c0(%rip)        # 0x1800091a0
-   180006fe0:	jmp    *0x20da(%rip)        # 0x1800090c0
-   180006fe6:	jmp    *0x214c(%rip)        # 0x180009138
-   180006fec:	mov    %rsp,%rax
-   180006fef:	mov    %r9,0x20(%rax)
-   180006ff3:	mov    %r8,0x18(%rax)
-   180006ff7:	mov    %rdx,0x10(%rax)
-   180006ffb:	push   %rbx
-   180006ffc:	push   %rsi
-   180006ffd:	push   %rdi
-   180006ffe:	push   %r14
-   180007000:	sub    $0x38,%rsp
-   180007004:	mov    %r9,%r14
-   180007007:	mov    %r8,%rbx
-   18000700a:	mov    %rdx,%rsi
-   18000700d:	movb   $0x0,-0x38(%rax)
-   180007011:	mov    %rdx,%rdi
-   180007014:	imul   %r8,%rdi
-   180007018:	add    %rcx,%rdi
-   18000701b:	mov    %rdi,0x8(%rax)
-   18000701f:	mov    %rbx,%rax
-   180007022:	dec    %rbx
-   180007025:	mov    %rbx,0x70(%rsp)
-   18000702a:	test   %rax,%rax
-   18000702d:	je     0x180007048
-   18000702f:	sub    %rsi,%rdi
-   180007032:	mov    %rdi,0x60(%rsp)
-   180007037:	mov    %rdi,%rcx
-   18000703a:	mov    %r14,%rax
-   18000703d:	mov    0x243c(%rip),%rdx        # 0x180009480
-   180007044:	call   *%rdx
-   180007046:	jmp    0x18000701f
-   180007048:	movb   $0x1,0x20(%rsp)
-   18000704d:	add    $0x38,%rsp
-   180007051:	pop    %r14
-   180007053:	pop    %rdi
-   180007054:	pop    %rsi
-   180007055:	pop    %rbx
-   180007056:	ret
-   180007057:	int3
-   180007058:	mov    %rbx,0x10(%rsp)
-   18000705d:	mov    %rsi,0x18(%rsp)
-   180007062:	mov    %rcx,0x8(%rsp)
-   180007067:	push   %rdi
-   180007068:	push   %r14
-   18000706a:	push   %r15
-   18000706c:	sub    $0x50,%rsp
-   180007070:	mov    %r9,%r14
-   180007073:	mov    %r8,%rsi
-   180007076:	mov    %rdx,%r15
-   180007079:	mov    %rcx,%rdi
-   18000707c:	xor    %ebx,%ebx
-   18000707e:	mov    %rbx,0x38(%rsp)
-   180007083:	cmp    %rsi,%rbx
-   180007086:	je     0x1800070a1
-   180007088:	sub    %r15,%rdi
-   18000708b:	mov    %rdi,0x70(%rsp)
-   180007090:	mov    %rdi,%rcx
-   180007093:	mov    %r14,%rax
-   180007096:	call   *0x23e4(%rip)        # 0x180009480
-   18000709c:	inc    %rbx
-   18000709f:	jmp    0x18000707e
-   1800070a1:	jmp    0x1800070a3
-   1800070a3:	lea    0x50(%rsp),%r11
-   1800070a8:	mov    0x28(%r11),%rbx
-   1800070ac:	mov    0x30(%r11),%rsi
-   1800070b0:	mov    %r11,%rsp
-   1800070b3:	pop    %r15
-   1800070b5:	pop    %r14
-   1800070b7:	pop    %rdi
-   1800070b8:	ret
-   1800070b9:	int3
-   1800070ba:	int3
-   1800070bb:	int3
-   1800070bc:	rex push %rbx
-   1800070be:	sub    $0x20,%rsp
-   1800070c2:	mov    %rcx,%rbx
-   1800070c5:	jmp    0x1800070d6
-   1800070c7:	mov    %rbx,%rcx
-   1800070ca:	call   0x180008010
-   1800070cf:	test   %eax,%eax
-   1800070d1:	je     0x1800070e6
-   1800070d3:	mov    %rbx,%rcx
-   1800070d6:	call   0x180008016
-   1800070db:	test   %rax,%rax
-   1800070de:	je     0x1800070c7
-   1800070e0:	add    $0x20,%rsp
-   1800070e4:	pop    %rbx
-   1800070e5:	ret
-   1800070e6:	cmp    $0xffffffffffffffff,%rbx
-   1800070ea:	je     0x1800070f2
-   1800070ec:	call   0x180007980
-   1800070f1:	int3
-   1800070f2:	call   0x1800038f0
-   1800070f7:	int3
-   1800070f8:	jmp    0x1800079a0
-   1800070fd:	int3
-   1800070fe:	int3
-   1800070ff:	int3
-   180007100:	jmp    0x1800070f8
-   180007105:	int3
-   180007106:	int3
-   180007107:	int3
-   180007108:	rex push %rbx
-   18000710a:	sub    $0x20,%rsp
-   18000710e:	lea    0x2893(%rip),%rax        # 0x1800099a8
-   180007115:	mov    %rcx,%rbx
-   180007118:	mov    %rax,(%rcx)
-   18000711b:	test   $0x1,%dl
-   18000711e:	je     0x18000712a
-   180007120:	mov    $0x18,%edx
-   180007125:	call   0x1800070f8
-   18000712a:	mov    %rbx,%rax
-   18000712d:	add    $0x20,%rsp
-   180007131:	pop    %rbx
-   180007132:	ret
-   180007133:	int3
-   180007134:	sub    $0x28,%rsp
-   180007138:	mov    0x38(%r9),%r8
-   18000713c:	mov    %rdx,%rcx
-   18000713f:	mov    %r9,%rdx
-   180007142:	call   0x180007154
-   180007147:	mov    $0x1,%eax
-   18000714c:	add    $0x28,%rsp
-   180007150:	ret
-   180007151:	int3
-   180007152:	int3
-   180007153:	int3
-   180007154:	rex push %rbx
-   180007156:	mov    (%r8),%r11d
-   180007159:	mov    %rdx,%rbx
-   18000715c:	and    $0xfffffff8,%r11d
-   180007160:	mov    %rcx,%r9
-   180007163:	testb  $0x4,(%r8)
-   180007167:	mov    %rcx,%r10
-   18000716a:	je     0x18000717f
-   18000716c:	mov    0x8(%r8),%eax
-   180007170:	movslq 0x4(%r8),%r10
-   180007174:	neg    %eax
-   180007176:	add    %rcx,%r10
-   180007179:	movslq %eax,%rcx
-   18000717c:	and    %rcx,%r10
-   18000717f:	movslq %r11d,%rax
-   180007182:	mov    (%rax,%r10,1),%rdx
-   180007186:	mov    0x10(%rbx),%rax
-   18000718a:	mov    0x8(%rax),%ecx
-   18000718d:	mov    0x8(%rbx),%rax
-   180007191:	testb  $0xf,0x3(%rcx,%rax,1)
-   180007196:	je     0x1800071a3
-   180007198:	movzbl 0x3(%rcx,%rax,1),%eax
-   18000719d:	and    $0xfffffff0,%eax
-   1800071a0:	add    %rax,%r9
-   1800071a3:	xor    %rdx,%r9
-   1800071a6:	mov    %r9,%rcx
-   1800071a9:	pop    %rbx
-   1800071aa:	jmp    0x180007240
-   1800071af:	int3
-   1800071b0:	mov    %rsp,%rax
-   1800071b3:	mov    %rbx,0x8(%rax)
-   1800071b7:	mov    %rbp,0x10(%rax)
-   1800071bb:	mov    %rsi,0x18(%rax)
-   1800071bf:	mov    %rdi,0x20(%rax)
-   1800071c3:	push   %r14
-   1800071c5:	sub    $0x20,%rsp
-   1800071c9:	mov    0x38(%r9),%rbx
-   1800071cd:	mov    %rdx,%rsi
-   1800071d0:	mov    %r8,%r14
-   1800071d3:	mov    %rcx,%rbp
-   1800071d6:	mov    %r9,%rdx
-   1800071d9:	mov    %rsi,%rcx
-   1800071dc:	mov    %r9,%rdi
-   1800071df:	lea    0x4(%rbx),%r8
-   1800071e3:	call   0x180007154
-   1800071e8:	mov    0x4(%rbp),%eax
-   1800071eb:	and    $0x66,%al
-   1800071ed:	neg    %al
-   1800071ef:	mov    $0x1,%eax
-   1800071f4:	sbb    %r8d,%r8d
-   1800071f7:	neg    %r8d
-   1800071fa:	add    %eax,%r8d
-   1800071fd:	test   %r8d,0x4(%rbx)
-   180007201:	je     0x180007214
-   180007203:	mov    %rdi,%r9
-   180007206:	mov    %r14,%r8
-   180007209:	mov    %rsi,%rdx
-   18000720c:	mov    %rbp,%rcx
-   18000720f:	call   0x180007fb0
-   180007214:	mov    0x30(%rsp),%rbx
-   180007219:	mov    0x38(%rsp),%rbp
-   18000721e:	mov    0x40(%rsp),%rsi
-   180007223:	mov    0x48(%rsp),%rdi
-   180007228:	add    $0x20,%rsp
-   18000722c:	pop    %r14
-   18000722e:	ret
-   18000722f:	int3
-   180007230:	int3
-   180007231:	int3
-   180007232:	int3
-   180007233:	int3
-   180007234:	int3
-   180007235:	int3
-   180007236:	data16 nopw 0x0(%rax,%rax,1)
-   180007240:	cmp    0x6dc1(%rip),%rcx        # 0x18000e008
-   180007247:	jne    0x180007259
-   180007249:	rol    $0x10,%rcx
-   18000724d:	test   $0xffff,%cx
-   180007252:	jne    0x180007255
-   180007254:	ret
-   180007255:	ror    $0x10,%rcx
-   180007259:	jmp    0x1800079dc
-   18000725e:	int3
-   18000725f:	int3
-   180007260:	lea    0x73e9(%rip),%rcx        # 0x18000e650
-   180007267:	rex.W jmp *0x1e42(%rip)        # 0x1800090b0
-   18000726e:	int3
-   18000726f:	int3
-   180007270:	lea    0x73d9(%rip),%rcx        # 0x18000e650
-   180007277:	jmp    0x180007ffe
-   18000727c:	sub    $0x28,%rsp
-   180007280:	test   %edx,%edx
-   180007282:	je     0x1800072bd
-   180007284:	sub    $0x1,%edx
-   180007287:	je     0x1800072b1
-   180007289:	sub    $0x1,%edx
-   18000728c:	je     0x1800072a4
-   18000728e:	cmp    $0x1,%edx
-   180007291:	je     0x18000729d
-   180007293:	mov    $0x1,%eax
-   180007298:	add    $0x28,%rsp
-   18000729c:	ret
-   18000729d:	call   0x18000768c
-   1800072a2:	jmp    0x1800072a9
-   1800072a4:	call   0x180007664
-   1800072a9:	movzbl %al,%eax
-   1800072ac:	add    $0x28,%rsp
-   1800072b0:	ret
-   1800072b1:	mov    %r8,%rdx
-   1800072b4:	add    $0x28,%rsp
-   1800072b8:	jmp    0x1800072cc
-   1800072bd:	test   %r8,%r8
-   1800072c0:	setne  %cl
-   1800072c3:	add    $0x28,%rsp
-   1800072c7:	jmp    0x1800073e4
-   1800072cc:	mov    %rbx,0x8(%rsp)
-   1800072d1:	mov    %rsi,0x10(%rsp)
-   1800072d6:	mov    %rdi,0x20(%rsp)
-   1800072db:	push   %r14
-   1800072dd:	sub    $0x20,%rsp
-   1800072e1:	mov    %rdx,%rsi
-   1800072e4:	mov    %rcx,%r14
-   1800072e7:	xor    %ecx,%ecx
-   1800072e9:	call   0x180007748
-   1800072ee:	test   %al,%al
-   1800072f0:	je     0x1800073be
-   1800072f6:	call   0x1800075dc
-   1800072fb:	mov    %al,%bl
-   1800072fd:	mov    %al,0x40(%rsp)
-   180007301:	mov    $0x1,%dil
-   180007304:	cmpl   $0x0,0x735d(%rip)        # 0x18000e668
-   18000730b:	jne    0x1800073d6
-   180007311:	movl   $0x1,0x734d(%rip)        # 0x18000e668
-   18000731b:	call   0x18000764c
-   180007320:	test   %al,%al
-   180007322:	je     0x180007373
-   180007324:	call   0x180007d7c
-   180007329:	call   0x180007260
-   18000732e:	call   0x180007c04
-   180007333:	lea    0x217e(%rip),%rdx        # 0x1800094b8
-   18000733a:	lea    0x216f(%rip),%rcx        # 0x1800094b0
-   180007341:	call   0x180008022
-   180007346:	test   %eax,%eax
-   180007348:	jne    0x180007373
-   18000734a:	call   0x180007618
-   18000734f:	test   %al,%al
-   180007351:	je     0x180007373
-   180007353:	lea    0x214e(%rip),%rdx        # 0x1800094a8
-   18000735a:	lea    0x2137(%rip),%rcx        # 0x180009498
-   180007361:	call   0x18000801c
-   180007366:	movl   $0x2,0x72f8(%rip)        # 0x18000e668
-   180007370:	xor    %dil,%dil
-   180007373:	mov    %bl,%cl
-   180007375:	call   0x1800078b8
-   18000737a:	test   %dil,%dil
-   18000737d:	jne    0x1800073be
-   18000737f:	call   0x180007c20
-   180007384:	mov    %rax,%rbx
-   180007387:	cmpq   $0x0,(%rax)
-   18000738b:	je     0x1800073b1
-   18000738d:	mov    %rax,%rcx
-   180007390:	call   0x180007820
-   180007395:	test   %al,%al
-   180007397:	je     0x1800073b1
-   180007399:	mov    %rsi,%r8
-   18000739c:	mov    $0x2,%edx
-   1800073a1:	mov    %r14,%rcx
-   1800073a4:	mov    (%rbx),%rax
-   1800073a7:	mov    0x20d2(%rip),%r9        # 0x180009480
-   1800073ae:	call   *%r9
-   1800073b1:	incl   0x72a9(%rip)        # 0x18000e660
-   1800073b7:	mov    $0x1,%eax
-   1800073bc:	jmp    0x1800073c0
-   1800073be:	xor    %eax,%eax
-   1800073c0:	mov    0x30(%rsp),%rbx
-   1800073c5:	mov    0x38(%rsp),%rsi
-   1800073ca:	mov    0x48(%rsp),%rdi
-   1800073cf:	add    $0x20,%rsp
-   1800073d3:	pop    %r14
-   1800073d5:	ret
-   1800073d6:	mov    $0x7,%ecx
-   1800073db:	call   0x180007c30
-   1800073e0:	nop
-   1800073e1:	int3
-   1800073e2:	int3
-   1800073e3:	int3
-   1800073e4:	mov    %rbx,0x8(%rsp)
-   1800073e9:	push   %rdi
-   1800073ea:	sub    $0x30,%rsp
-   1800073ee:	mov    %cl,%dil
-   1800073f1:	mov    0x7269(%rip),%eax        # 0x18000e660
-   1800073f7:	test   %eax,%eax
-   1800073f9:	jg     0x180007408
-   1800073fb:	xor    %eax,%eax
-   1800073fd:	mov    0x40(%rsp),%rbx
-   180007402:	add    $0x30,%rsp
-   180007406:	pop    %rdi
-   180007407:	ret
-   180007408:	dec    %eax
-   18000740a:	mov    %eax,0x7250(%rip)        # 0x18000e660
-   180007410:	call   0x1800075dc
-   180007415:	mov    %al,%bl
-   180007417:	mov    %al,0x20(%rsp)
-   18000741b:	cmpl   $0x2,0x7246(%rip)        # 0x18000e668
-   180007422:	jne    0x18000745b
-   180007424:	call   0x180007704
-   180007429:	call   0x180007270
-   18000742e:	call   0x180007db8
-   180007433:	andl   $0x0,0x722e(%rip)        # 0x18000e668
-   18000743a:	mov    %bl,%cl
-   18000743c:	call   0x1800078b8
-   180007441:	xor    %edx,%edx
-   180007443:	mov    %dil,%cl
-   180007446:	call   0x1800078dc
-   18000744b:	neg    %al
-   18000744d:	sbb    %ebx,%ebx
-   18000744f:	and    $0x1,%ebx
-   180007452:	call   0x180007734
-   180007457:	mov    %ebx,%eax
-   180007459:	jmp    0x1800073fd
-   18000745b:	mov    $0x7,%ecx
-   180007460:	call   0x180007c30
-   180007465:	nop
-   180007466:	nop
-   180007467:	int3
-   180007468:	mov    %rsp,%rax
-   18000746b:	mov    %rbx,0x20(%rax)
-   18000746f:	mov    %r8,0x18(%rax)
-   180007473:	mov    %edx,0x10(%rax)
-   180007476:	mov    %rcx,0x8(%rax)
-   18000747a:	push   %rsi
-   18000747b:	push   %rdi
-   18000747c:	push   %r14
-   18000747e:	sub    $0x40,%rsp
-   180007482:	mov    %r8,%rsi
-   180007485:	mov    %edx,%edi
-   180007487:	mov    %rcx,%r14
-   18000748a:	test   %edx,%edx
-   18000748c:	jne    0x18000749d
-   18000748e:	cmp    %edx,0x71cc(%rip)        # 0x18000e660
-   180007494:	jg     0x18000749d
-   180007496:	xor    %eax,%eax
-   180007498:	jmp    0x18000758b
-   18000749d:	lea    -0x1(%rdx),%eax
-   1800074a0:	cmp    $0x1,%eax
-   1800074a3:	ja     0x1800074ea
-   1800074a5:	mov    0x2504(%rip),%rax        # 0x1800099b0
-   1800074ac:	test   %rax,%rax
-   1800074af:	jne    0x1800074bb
-   1800074b1:	movl   $0x1,0x30(%rsp)
-   1800074b9:	jmp    0x1800074cf
-   1800074bb:	call   *0x1fbf(%rip)        # 0x180009480
-   1800074c1:	mov    %eax,%ebx
-   1800074c3:	mov    %eax,0x30(%rsp)
-   1800074c7:	test   %eax,%eax
-   1800074c9:	je     0x180007581
-   1800074cf:	mov    %rsi,%r8
-   1800074d2:	mov    %edi,%edx
-   1800074d4:	mov    %r14,%rcx
-   1800074d7:	call   0x18000727c
-   1800074dc:	mov    %eax,%ebx
-   1800074de:	mov    %eax,0x30(%rsp)
-   1800074e2:	test   %eax,%eax
-   1800074e4:	je     0x180007581
-   1800074ea:	mov    %rsi,%r8
-   1800074ed:	mov    %edi,%edx
-   1800074ef:	mov    %r14,%rcx
-   1800074f2:	call   0x180007bd0
-   1800074f7:	mov    %eax,%ebx
-   1800074f9:	mov    %eax,0x30(%rsp)
-   1800074fd:	cmp    $0x1,%edi
-   180007500:	jne    0x180007538
-   180007502:	test   %eax,%eax
-   180007504:	jne    0x180007538
-   180007506:	mov    %rsi,%r8
-   180007509:	xor    %edx,%edx
-   18000750b:	mov    %r14,%rcx
-   18000750e:	call   0x180007bd0
-   180007513:	test   %rsi,%rsi
-   180007516:	setne  %cl
-   180007519:	call   0x1800073e4
-   18000751e:	mov    0x248b(%rip),%rax        # 0x1800099b0
-   180007525:	test   %rax,%rax
-   180007528:	je     0x180007538
-   18000752a:	mov    %rsi,%r8
-   18000752d:	xor    %edx,%edx
-   18000752f:	mov    %r14,%rcx
-   180007532:	call   *0x1f48(%rip)        # 0x180009480
-   180007538:	test   %edi,%edi
-   18000753a:	je     0x180007541
-   18000753c:	cmp    $0x3,%edi
-   18000753f:	jne    0x180007581
-   180007541:	mov    %rsi,%r8
-   180007544:	mov    %edi,%edx
-   180007546:	mov    %r14,%rcx
-   180007549:	call   0x18000727c
-   18000754e:	mov    %eax,%ebx
-   180007550:	mov    %eax,0x30(%rsp)
-   180007554:	test   %eax,%eax
-   180007556:	je     0x180007581
-   180007558:	mov    0x2451(%rip),%rax        # 0x1800099b0
-   18000755f:	test   %rax,%rax
-   180007562:	jne    0x18000756d
-   180007564:	lea    0x1(%rax),%ebx
-   180007567:	mov    %ebx,0x30(%rsp)
-   18000756b:	jmp    0x180007581
-   18000756d:	mov    %rsi,%r8
-   180007570:	mov    %edi,%edx
-   180007572:	mov    %r14,%rcx
-   180007575:	call   *0x1f05(%rip)        # 0x180009480
-   18000757b:	mov    %eax,%ebx
-   18000757d:	mov    %eax,0x30(%rsp)
-   180007581:	jmp    0x180007589
-   180007583:	xor    %ebx,%ebx
-   180007585:	mov    %ebx,0x30(%rsp)
-   180007589:	mov    %ebx,%eax
-   18000758b:	mov    0x78(%rsp),%rbx
-   180007590:	add    $0x40,%rsp
-   180007594:	pop    %r14
-   180007596:	pop    %rdi
-   180007597:	pop    %rsi
-   180007598:	ret
-   180007599:	int3
-   18000759a:	int3
-   18000759b:	int3
-   18000759c:	mov    %rbx,0x8(%rsp)
-   1800075a1:	mov    %rsi,0x10(%rsp)
-   1800075a6:	push   %rdi
-   1800075a7:	sub    $0x20,%rsp
-   1800075ab:	mov    %r8,%rdi
-   1800075ae:	mov    %edx,%ebx
-   1800075b0:	mov    %rcx,%rsi
-   1800075b3:	cmp    $0x1,%edx
-   1800075b6:	jne    0x1800075bd
-   1800075b8:	call   0x180007b24
-   1800075bd:	mov    %rdi,%r8
-   1800075c0:	mov    %ebx,%edx
-   1800075c2:	mov    %rsi,%rcx
-   1800075c5:	mov    0x30(%rsp),%rbx
-   1800075ca:	mov    0x38(%rsp),%rsi
-   1800075cf:	add    $0x20,%rsp
-   1800075d3:	pop    %rdi
-   1800075d4:	jmp    0x180007468
-   1800075d9:	int3
-   1800075da:	int3
-   1800075db:	int3
-   1800075dc:	sub    $0x28,%rsp
-   1800075e0:	call   0x180007fa0
-   1800075e5:	test   %eax,%eax
-   1800075e7:	je     0x18000760a
-   1800075e9:	mov    %gs:0x30,%rax
-   1800075f2:	mov    0x8(%rax),%rcx
-   1800075f6:	jmp    0x1800075fd
-   1800075f8:	cmp    %rax,%rcx
-   1800075fb:	je     0x180007611
-   1800075fd:	xor    %eax,%eax
-   1800075ff:	lock cmpxchg %rcx,0x7068(%rip)        # 0x18000e670
-   180007608:	jne    0x1800075f8
-   18000760a:	xor    %al,%al
-   18000760c:	add    $0x28,%rsp
-   180007610:	ret
-   180007611:	mov    $0x1,%al
-   180007613:	jmp    0x18000760c
-   180007615:	int3
-   180007616:	int3
-   180007617:	int3
-   180007618:	sub    $0x28,%rsp
-   18000761c:	call   0x180007fa0
-   180007621:	test   %eax,%eax
-   180007623:	je     0x18000762c
-   180007625:	call   0x180007df4
-   18000762a:	jmp    0x180007645
-   18000762c:	call   0x180007f98
-   180007631:	mov    %eax,%ecx
-   180007633:	call   0x18000802e
-   180007638:	test   %eax,%eax
-   18000763a:	je     0x180007640
-   18000763c:	xor    %al,%al
-   18000763e:	jmp    0x180007647
-   180007640:	call   0x180008034
-   180007645:	mov    $0x1,%al
-   180007647:	add    $0x28,%rsp
-   18000764b:	ret
-   18000764c:	sub    $0x28,%rsp
-   180007650:	xor    %ecx,%ecx
-   180007652:	call   0x180007794
-   180007657:	test   %al,%al
-   180007659:	setne  %al
-   18000765c:	add    $0x28,%rsp
-   180007660:	ret
-   180007661:	int3
-   180007662:	int3
-   180007663:	int3
-   180007664:	sub    $0x28,%rsp
-   180007668:	call   0x180004f10
-   18000766d:	test   %al,%al
-   18000766f:	jne    0x180007675
-   180007671:	xor    %al,%al
-   180007673:	jmp    0x180007687
-   180007675:	call   0x180004f10
-   18000767a:	test   %al,%al
-   18000767c:	jne    0x180007685
-   18000767e:	call   0x180004f10
-   180007683:	jmp    0x180007671
-   180007685:	mov    $0x1,%al
-   180007687:	add    $0x28,%rsp
-   18000768b:	ret
-   18000768c:	sub    $0x28,%rsp
-   180007690:	call   0x180004f10
-   180007695:	call   0x180004f10
-   18000769a:	mov    $0x1,%al
-   18000769c:	add    $0x28,%rsp
-   1800076a0:	ret
+   1800051d0:	sub    $0x28,%rsp
+   1800051d4:	mov    (%rcx),%rax
+   1800051d7:	call   *0x80(%rax)
+   1800051dd:	xorps  %xmm0,%xmm0
+   1800051e0:	add    $0x28,%rsp
+   1800051e4:	ret
+   1800051e5:	int3
+   1800051e6:	int3
+   1800051e7:	int3
+   1800051e8:	int3
+   1800051e9:	int3
+   1800051ea:	int3
+   1800051eb:	int3
+   1800051ec:	int3
+   1800051ed:	int3
+   1800051ee:	int3
+   1800051ef:	int3
+   1800051f0:	mov    %rbx,0x8(%rsp)
+   1800051f5:	push   %rdi
+   1800051f6:	sub    $0x20,%rsp
+   1800051fa:	mov    %rcx,%rbx
+   1800051fd:	mov    %rdx,%rcx
+   180005200:	call   0x180002680
+   180005205:	mov    %rax,%rcx
+   180005208:	mov    %rax,%rdi
+   18000520b:	call   *0x3f5f(%rip)        # 0x180009170
+   180005211:	test   %al,%al
+   180005213:	je     0x180005228
+   180005215:	movq   $0x0,0x68(%rbx)
+   18000521d:	mov    0x30(%rsp),%rbx
+   180005222:	add    $0x20,%rsp
+   180005226:	pop    %rdi
+   180005227:	ret
+   180005228:	mov    %rbx,%rcx
+   18000522b:	mov    %rdi,0x68(%rbx)
+   18000522f:	mov    0x30(%rsp),%rbx
+   180005234:	add    $0x20,%rsp
+   180005238:	pop    %rdi
+   180005239:	rex.W jmp *0x3f88(%rip)        # 0x1800091c8
+   180005240:	xor    %al,%al
+   180005242:	ret
+   180005243:	int3
+   180005244:	int3
+   180005245:	int3
+   180005246:	int3
+   180005247:	int3
+   180005248:	int3
+   180005249:	int3
+   18000524a:	int3
+   18000524b:	int3
+   18000524c:	int3
+   18000524d:	int3
+   18000524e:	int3
+   18000524f:	int3
+   180005250:	mov    $0x1,%al
+   180005252:	ret
+   180005253:	int3
+   180005254:	int3
+   180005255:	int3
+   180005256:	int3
+   180005257:	int3
+   180005258:	int3
+   180005259:	int3
+   18000525a:	int3
+   18000525b:	int3
+   18000525c:	int3
+   18000525d:	int3
+   18000525e:	int3
+   18000525f:	int3
+   180005260:	mov    %rbx,0x20(%rsp)
+   180005265:	push   %rdi
+   180005266:	sub    $0x80,%rsp
+   18000526d:	mov    0x8d94(%rip),%rax        # 0x18000e008
+   180005274:	xor    %rsp,%rax
+   180005277:	mov    %rax,0x78(%rsp)
+   18000527c:	mov    %edx,%edi
+   18000527e:	mov    %rcx,%rbx
+   180005281:	cmp    $0xffffffff,%edx
+   180005284:	jne    0x18000528d
+   180005286:	xor    %eax,%eax
+   180005288:	jmp    0x1800053e2
+   18000528d:	mov    0x40(%rcx),%rdx
+   180005291:	mov    (%rdx),%rax
+   180005294:	test   %rax,%rax
+   180005297:	je     0x1800052b8
+   180005299:	mov    0x58(%rcx),%rdx
+   18000529d:	movslq (%rdx),%r8
+   1800052a0:	add    %rax,%r8
+   1800052a3:	cmp    %r8,%rax
+   1800052a6:	jae    0x1800052b8
+   1800052a8:	call   *0x3f12(%rip)        # 0x1800091c0
+   1800052ae:	mov    %dil,(%rax)
+   1800052b1:	mov    %edi,%eax
+   1800052b3:	jmp    0x1800053e2
+   1800052b8:	cmpq   $0x0,0x80(%rcx)
+   1800052c0:	mov    %rsi,0xa0(%rsp)
+   1800052c8:	je     0x1800053d5
+   1800052ce:	mov    0x18(%rcx),%r8
+   1800052d2:	lea    0x70(%rcx),%rax
+   1800052d6:	cmp    %rax,(%r8)
+   1800052d9:	jne    0x1800052fb
+   1800052db:	mov    0x90(%rcx),%rdx
+   1800052e2:	mov    0x88(%rcx),%rcx
+   1800052e9:	mov    %rcx,(%r8)
+   1800052ec:	sub    %ecx,%edx
+   1800052ee:	mov    0x38(%rbx),%rax
+   1800052f2:	mov    %rcx,(%rax)
+   1800052f5:	mov    0x50(%rbx),%rax
+   1800052f9:	mov    %edx,(%rax)
+   1800052fb:	mov    0x68(%rbx),%rcx
+   1800052ff:	test   %rcx,%rcx
+   180005302:	jne    0x180005326
+   180005304:	mov    0x80(%rbx),%rdx
+   18000530b:	movsbl %dil,%ecx
+   18000530f:	call   *0x414b(%rip)        # 0x180009460
+   180005315:	mov    $0xffffffff,%ecx
+   18000531a:	cmp    %ecx,%eax
+   18000531c:	cmovne %edi,%ecx
+   18000531f:	mov    %ecx,%eax
+   180005321:	jmp    0x1800053da
+   180005326:	lea    0x48(%rsp),%rax
+   18000532b:	mov    %dil,0x40(%rsp)
+   180005330:	mov    %rax,0x38(%rsp)
+   180005335:	lea    0x74(%rbx),%rdx
+   180005339:	lea    0x78(%rsp),%rax
+   18000533e:	mov    %rax,0x30(%rsp)
+   180005343:	lea    0x41(%rsp),%r9
+   180005348:	lea    0x58(%rsp),%rax
+   18000534d:	mov    %rax,0x28(%rsp)
+   180005352:	lea    0x40(%rsp),%r8
+   180005357:	lea    0x50(%rsp),%rax
+   18000535c:	mov    %rax,0x20(%rsp)
+   180005361:	call   *0x3e19(%rip)        # 0x180009180
+   180005367:	test   %eax,%eax
+   180005369:	je     0x180005395
+   18000536b:	sub    $0x1,%eax
+   18000536e:	je     0x180005395
+   180005370:	cmp    $0x2,%eax
+   180005373:	jne    0x1800053d5
+   180005375:	movsbl 0x40(%rsp),%ecx
+   18000537a:	mov    0x80(%rbx),%rdx
+   180005381:	call   *0x40d9(%rip)        # 0x180009460
+   180005387:	mov    $0xffffffff,%ecx
+   18000538c:	cmp    %ecx,%eax
+   18000538e:	cmovne %edi,%ecx
+   180005391:	mov    %ecx,%eax
+   180005393:	jmp    0x1800053da
+   180005395:	mov    0x48(%rsp),%rsi
+   18000539a:	lea    0x58(%rsp),%rax
+   18000539f:	sub    %rax,%rsi
+   1800053a2:	je     0x1800053c3
+   1800053a4:	mov    0x80(%rbx),%r9
+   1800053ab:	lea    0x58(%rsp),%rcx
+   1800053b0:	mov    %rsi,%r8
+   1800053b3:	mov    $0x1,%edx
+   1800053b8:	call   *0x4052(%rip)        # 0x180009410
+   1800053be:	cmp    %rax,%rsi
+   1800053c1:	jne    0x1800053d5
+   1800053c3:	lea    0x40(%rsp),%rax
+   1800053c8:	movb   $0x1,0x71(%rbx)
+   1800053cc:	cmp    %rax,0x50(%rsp)
+   1800053d1:	mov    %edi,%eax
+   1800053d3:	jne    0x1800053da
+   1800053d5:	mov    $0xffffffff,%eax
+   1800053da:	mov    0xa0(%rsp),%rsi
+   1800053e2:	mov    0x78(%rsp),%rcx
+   1800053e7:	xor    %rsp,%rcx
+   1800053ea:	call   0x180007500
+   1800053ef:	mov    0xa8(%rsp),%rbx
+   1800053f7:	add    $0x80,%rsp
+   1800053fe:	pop    %rdi
+   1800053ff:	ret
+   180005400:	mov    %rbx,0x8(%rsp)
+   180005405:	push   %rdi
+   180005406:	sub    $0x20,%rsp
+   18000540a:	mov    0x38(%rcx),%rax
+   18000540e:	mov    %rcx,%rbx
+   180005411:	mov    %edx,%edi
+   180005413:	mov    (%rax),%rcx
+   180005416:	test   %rcx,%rcx
+   180005419:	je     0x180005453
+   18000541b:	mov    0x18(%rbx),%rax
+   18000541f:	cmp    %rcx,(%rax)
+   180005422:	jae    0x180005453
+   180005424:	cmp    $0xffffffff,%edx
+   180005427:	je     0x180005431
+   180005429:	movzbl -0x1(%rcx),%eax
+   18000542d:	cmp    %edx,%eax
+   18000542f:	jne    0x180005453
+   180005431:	mov    0x50(%rbx),%rax
+   180005435:	incl   (%rax)
+   180005437:	mov    0x38(%rbx),%rax
+   18000543b:	decq   (%rax)
+   18000543e:	xor    %eax,%eax
+   180005440:	cmp    $0xffffffff,%edi
+   180005443:	cmove  %eax,%edi
+   180005446:	mov    %edi,%eax
+   180005448:	mov    0x30(%rsp),%rbx
+   18000544d:	add    $0x20,%rsp
+   180005451:	pop    %rdi
+   180005452:	ret
+   180005453:	mov    0x80(%rbx),%rdx
+   18000545a:	test   %rdx,%rdx
+   18000545d:	je     0x1800054d2
+   18000545f:	cmp    $0xffffffff,%edi
+   180005462:	je     0x1800054d2
+   180005464:	cmpq   $0x0,0x68(%rbx)
+   180005469:	jne    0x18000547a
+   18000546b:	movzbl %dil,%ecx
+   18000546f:	call   *0x3fbb(%rip)        # 0x180009430
+   180005475:	cmp    $0xffffffff,%eax
+   180005478:	jne    0x180005446
+   18000547a:	mov    0x38(%rbx),%r8
+   18000547e:	lea    0x70(%rbx),%rdx
+   180005482:	cmp    %rdx,(%r8)
+   180005485:	je     0x1800054d2
+   180005487:	mov    0x18(%rbx),%r9
+   18000548b:	mov    %dil,(%rdx)
+   18000548e:	mov    (%r9),%rax
+   180005491:	cmp    %rdx,%rax
+   180005494:	je     0x1800054ae
+   180005496:	mov    %rax,0x88(%rbx)
+   18000549d:	mov    0x50(%rbx),%rax
+   1800054a1:	movslq (%rax),%rcx
+   1800054a4:	add    (%r8),%rcx
+   1800054a7:	mov    %rcx,0x90(%rbx)
+   1800054ae:	mov    %rdx,(%r9)
+   1800054b1:	mov    %ebx,%ecx
+   1800054b3:	mov    0x38(%rbx),%rax
+   1800054b7:	sub    %edx,%ecx
+   1800054b9:	add    $0x71,%ecx
+   1800054bc:	mov    %rdx,(%rax)
+   1800054bf:	mov    0x50(%rbx),%rax
+   1800054c3:	mov    %ecx,(%rax)
+   1800054c5:	mov    %edi,%eax
+   1800054c7:	mov    0x30(%rsp),%rbx
+   1800054cc:	add    $0x20,%rsp
+   1800054d0:	pop    %rdi
+   1800054d1:	ret
+   1800054d2:	mov    0x30(%rsp),%rbx
+   1800054d7:	mov    $0xffffffff,%eax
+   1800054dc:	add    $0x20,%rsp
+   1800054e0:	pop    %rdi
+   1800054e1:	ret
+   1800054e2:	int3
+   1800054e3:	int3
+   1800054e4:	int3
+   1800054e5:	int3
+   1800054e6:	int3
+   1800054e7:	int3
+   1800054e8:	int3
+   1800054e9:	int3
+   1800054ea:	int3
+   1800054eb:	int3
+   1800054ec:	int3
+   1800054ed:	int3
+   1800054ee:	int3
+   1800054ef:	int3
+   1800054f0:	sub    $0x38,%rsp
+   1800054f4:	movups (%rdx),%xmm0
+   1800054f7:	add    $0x58,%rcx
+   1800054fb:	lea    0x20(%rsp),%rdx
+   180005500:	movaps %xmm0,0x20(%rsp)
+   180005505:	call   0x180002300
+   18000550a:	add    $0x38,%rsp
+   18000550e:	ret
+   18000550f:	int3
+   180005510:	mov    0x68(%rcx),%r8
+   180005514:	add    $0x58,%rcx
+   180005518:	mov    %edx,%r9d
+   18000551b:	movabs $0x6666666666666667,%rax
+   180005525:	sub    (%rcx),%r8
+   180005528:	imul   %r8
+   18000552b:	sar    $0x4,%rdx
+   18000552f:	mov    %rdx,%rax
+   180005532:	shr    $0x3f,%rax
+   180005536:	add    %rax,%rdx
+   180005539:	cmp    %rdx,%r9
+   18000553c:	jbe    0x180005546
+   18000553e:	mov    %r9d,%edx
+   180005541:	jmp    0x180003820
+   180005546:	ret
+   180005547:	int3
+   180005548:	int3
+   180005549:	int3
+   18000554a:	int3
+   18000554b:	int3
+   18000554c:	int3
+   18000554d:	int3
+   18000554e:	int3
+   18000554f:	int3
+   180005550:	mov    %rbx,0x8(%rsp)
+   180005555:	mov    %rsi,0x10(%rsp)
+   18000555a:	push   %rdi
+   18000555b:	sub    $0x20,%rsp
+   18000555f:	mov    0x68(%rcx),%r8
+   180005563:	movabs $0x6666666666666667,%rax
+   18000556d:	sub    0x58(%rcx),%r8
+   180005571:	mov    %rcx,%rdi
+   180005574:	mov    %edx,%r9d
+   180005577:	imul   %r8
+   18000557a:	mov    %r9d,%esi
+   18000557d:	sar    $0x4,%rdx
+   180005581:	mov    %rdx,%rax
+   180005584:	shr    $0x3f,%rax
+   180005588:	add    %rax,%rdx
+   18000558b:	cmp    %rdx,%r9
+   18000558e:	jbe    0x1800055ad
+   180005590:	lea    (%rdx,%rdx,1),%eax
+   180005593:	cmp    %eax,%r9d
+   180005596:	cmovb  %eax,%r9d
+   18000559a:	mov    %r9d,%eax
+   18000559d:	cmp    %rdx,%rax
+   1800055a0:	jbe    0x1800055ad
+   1800055a2:	mov    %eax,%edx
+   1800055a4:	add    $0x58,%rcx
+   1800055a8:	call   0x180003820
+   1800055ad:	lea    0x30(%rdi),%r8
+   1800055b1:	mov    %rsi,%rdx
+   1800055b4:	lea    0x58(%rdi),%rcx
+   1800055b8:	mov    0x30(%rsp),%rbx
+   1800055bd:	mov    0x38(%rsp),%rsi
+   1800055c2:	add    $0x20,%rsp
+   1800055c6:	pop    %rdi
+   1800055c7:	jmp    0x1800055d0
+   1800055cc:	int3
+   1800055cd:	int3
+   1800055ce:	int3
+   1800055cf:	int3
+   1800055d0:	mov    %rbx,0x8(%rsp)
+   1800055d5:	mov    %rsi,0x10(%rsp)
+   1800055da:	push   %rdi
+   1800055db:	mov    0x8(%rcx),%r9
+   1800055df:	mov    %rdx,%r10
+   1800055e2:	mov    (%rcx),%rdi
+   1800055e5:	mov    %r9,%rdx
+   1800055e8:	sub    %rdi,%rdx
+   1800055eb:	movabs $0x6666666666666667,%rsi
+   1800055f5:	mov    %rsi,%rax
+   1800055f8:	mov    %rcx,%r11
+   1800055fb:	imul   %rdx
+   1800055fe:	mov    %rdx,%rbx
+   180005601:	sar    $0x4,%rbx
+   180005605:	mov    %rbx,%rax
+   180005608:	shr    $0x3f,%rax
+   18000560c:	add    %rax,%rbx
+   18000560f:	cmp    %rbx,%r10
+   180005612:	jae    0x18000562c
+   180005614:	lea    (%r10,%r10,4),%rax
+   180005618:	lea    (%rdi,%rax,8),%rcx
+   18000561c:	mov    %rcx,0x8(%r11)
+   180005620:	mov    0x10(%rsp),%rbx
+   180005625:	mov    0x18(%rsp),%rsi
+   18000562a:	pop    %rdi
+   18000562b:	ret
+   18000562c:	jbe    0x18000569c
+   18000562e:	mov    0x10(%rcx),%rcx
+   180005632:	mov    %rsi,%rax
+   180005635:	sub    %rdi,%rcx
+   180005638:	imul   %rcx
+   18000563b:	sar    $0x4,%rdx
+   18000563f:	mov    %rdx,%rax
+   180005642:	shr    $0x3f,%rax
+   180005646:	add    %rax,%rdx
+   180005649:	cmp    %rdx,%r10
+   18000564c:	jbe    0x180005664
+   18000564e:	mov    %r10,%rdx
+   180005651:	mov    %r11,%rcx
+   180005654:	mov    0x10(%rsp),%rbx
+   180005659:	mov    0x18(%rsp),%rsi
+   18000565e:	pop    %rdi
+   18000565f:	jmp    0x180001d80
+   180005664:	sub    %rbx,%r10
+   180005667:	je     0x180005698
+   180005669:	nopl   0x0(%rax)
+   180005670:	movups (%r8),%xmm0
+   180005674:	movups %xmm0,(%r9)
+   180005678:	movups 0x10(%r8),%xmm1
+   18000567d:	movups %xmm1,0x10(%r9)
+   180005682:	movsd  0x20(%r8),%xmm0
+   180005688:	movsd  %xmm0,0x20(%r9)
+   18000568e:	add    $0x28,%r9
+   180005692:	sub    $0x1,%r10
+   180005696:	jne    0x180005670
+   180005698:	mov    %r9,0x8(%r11)
+   18000569c:	mov    0x10(%rsp),%rbx
+   1800056a1:	mov    0x18(%rsp),%rsi
+   1800056a6:	pop    %rdi
+   1800056a7:	ret
+   1800056a8:	int3
+   1800056a9:	int3
+   1800056aa:	int3
+   1800056ab:	int3
+   1800056ac:	int3
+   1800056ad:	int3
+   1800056ae:	int3
+   1800056af:	int3
+   1800056b0:	mov    %rbx,0x10(%rsp)
+   1800056b5:	mov    %rbp,0x18(%rsp)
+   1800056ba:	mov    %rsi,0x20(%rsp)
+   1800056bf:	push   %rdi
+   1800056c0:	sub    $0x20,%rsp
+   1800056c4:	mov    0x38(%rcx),%r10
+   1800056c8:	lea    0x70(%rcx),%rax
+   1800056cc:	mov    %r9d,%ebp
+   1800056cf:	mov    %r8,%rsi
+   1800056d2:	mov    %rdx,%rbx
+   1800056d5:	mov    %rcx,%rdi
+   1800056d8:	cmp    %rax,(%r10)
+   1800056db:	jne    0x1800056ed
+   1800056dd:	cmp    $0x1,%r9d
+   1800056e1:	jne    0x1800056ed
+   1800056e3:	cmpq   $0x0,0x68(%rcx)
+   1800056e8:	jne    0x1800056ed
+   1800056ea:	dec    %rsi
+   1800056ed:	cmpq   $0x0,0x80(%rcx)
+   1800056f5:	je     0x18000574d
+   1800056f7:	call   0x1800036f0
+   1800056fc:	test   %al,%al
+   1800056fe:	je     0x18000574d
+   180005700:	test   %rsi,%rsi
+   180005703:	jne    0x18000570a
+   180005705:	cmp    $0x1,%ebp
+   180005708:	je     0x180005721
+   18000570a:	mov    0x80(%rdi),%rcx
+   180005711:	mov    %ebp,%r8d
+   180005714:	mov    %rsi,%rdx
+   180005717:	call   *0x3cfb(%rip)        # 0x180009418
+   18000571d:	test   %eax,%eax
+   18000571f:	jne    0x18000574d
+   180005721:	mov    0x80(%rdi),%rcx
+   180005728:	lea    0x30(%rsp),%rdx
+   18000572d:	call   *0x3d05(%rip)        # 0x180009438
+   180005733:	test   %eax,%eax
+   180005735:	jne    0x18000574d
+   180005737:	mov    %rdi,%rcx
+   18000573a:	call   0x1800038c0
+   18000573f:	mov    0x30(%rsp),%rcx
+   180005744:	mov    0x74(%rdi),%rax
+   180005748:	mov    %rcx,(%rbx)
+   18000574b:	jmp    0x180005756
+   18000574d:	movq   $0xffffffffffffffff,(%rbx)
+   180005754:	xor    %eax,%eax
+   180005756:	mov    0x40(%rsp),%rbp
+   18000575b:	mov    0x48(%rsp),%rsi
+   180005760:	movq   $0x0,0x8(%rbx)
+   180005768:	mov    %rax,0x10(%rbx)
+   18000576c:	mov    %rbx,%rax
+   18000576f:	mov    0x38(%rsp),%rbx
+   180005774:	add    $0x20,%rsp
+   180005778:	pop    %rdi
+   180005779:	ret
+   18000577a:	int3
+   18000577b:	int3
+   18000577c:	int3
+   18000577d:	int3
+   18000577e:	int3
+   18000577f:	int3
+   180005780:	mov    %rbx,0x10(%rsp)
+   180005785:	mov    %rsi,0x18(%rsp)
+   18000578a:	push   %rdi
+   18000578b:	sub    $0x20,%rsp
+   18000578f:	mov    0x8(%r8),%rax
+   180005793:	mov    %r8,%rsi
+   180005796:	add    (%r8),%rax
+   180005799:	mov    %rdx,%rbx
+   18000579c:	cmpq   $0x0,0x80(%rcx)
+   1800057a4:	mov    %rcx,%rdi
+   1800057a7:	mov    %rax,0x30(%rsp)
+   1800057ac:	je     0x18000582d
+   1800057ae:	call   0x1800036f0
+   1800057b3:	test   %al,%al
+   1800057b5:	je     0x18000582d
+   1800057b7:	mov    0x80(%rdi),%rcx
+   1800057be:	lea    0x30(%rsp),%rdx
+   1800057c3:	call   *0x3c57(%rip)        # 0x180009420
+   1800057c9:	test   %eax,%eax
+   1800057cb:	jne    0x18000582d
+   1800057cd:	mov    0x18(%rdi),%r8
+   1800057d1:	lea    0x70(%rdi),%rax
+   1800057d5:	mov    0x10(%rsi),%rcx
+   1800057d9:	mov    %rcx,0x74(%rdi)
+   1800057dd:	cmp    %rax,(%r8)
+   1800057e0:	jne    0x180005806
+   1800057e2:	mov    0x88(%rdi),%rcx
+   1800057e9:	mov    0x90(%rdi),%rdx
+   1800057f0:	mov    %rcx,(%r8)
+   1800057f3:	sub    %ecx,%edx
+   1800057f5:	mov    0x38(%rdi),%rax
+   1800057f9:	mov    %rcx,(%rax)
+   1800057fc:	mov    0x50(%rdi),%rax
+   180005800:	mov    %edx,(%rax)
+   180005802:	mov    0x74(%rdi),%rcx
+   180005806:	mov    0x30(%rsp),%rax
+   18000580b:	mov    %rax,(%rbx)
+   18000580e:	mov    %rbx,%rax
+   180005811:	movq   $0x0,0x8(%rbx)
+   180005819:	mov    %rcx,0x10(%rbx)
+   18000581d:	mov    0x38(%rsp),%rbx
+   180005822:	mov    0x40(%rsp),%rsi
+   180005827:	add    $0x20,%rsp
+   18000582b:	pop    %rdi
+   18000582c:	ret
+   18000582d:	mov    0x40(%rsp),%rsi
+   180005832:	xor    %eax,%eax
+   180005834:	movq   $0xffffffffffffffff,(%rbx)
+   18000583b:	movq   $0x0,0x8(%rbx)
+   180005843:	mov    %rax,0x10(%rbx)
+   180005847:	mov    %rbx,%rax
+   18000584a:	mov    0x38(%rsp),%rbx
+   18000584f:	add    $0x20,%rsp
+   180005853:	pop    %rdi
+   180005854:	ret
+   180005855:	int3
+   180005856:	int3
+   180005857:	int3
+   180005858:	int3
+   180005859:	int3
+   18000585a:	int3
+   18000585b:	int3
+   18000585c:	int3
+   18000585d:	int3
+   18000585e:	int3
+   18000585f:	int3
+   180005860:	rex push %rbx
+   180005862:	push   %rsi
+   180005863:	sub    $0x28,%rsp
+   180005867:	xor    %esi,%esi
+   180005869:	mov    %r8,%r9
+   18000586c:	mov    %rcx,%rbx
+   18000586f:	test   %rdx,%rdx
+   180005872:	jne    0x18000587d
+   180005874:	test   %r8,%r8
+   180005877:	lea    0x4(%rsi),%r8d
+   18000587b:	je     0x180005880
+   18000587d:	mov    %esi,%r8d
+   180005880:	mov    0x80(%rcx),%rcx
+   180005887:	test   %rcx,%rcx
+   18000588a:	je     0x180005933
+   180005890:	call   *0x3b72(%rip)        # 0x180009408
+   180005896:	test   %eax,%eax
+   180005898:	jne    0x180005933
+   18000589e:	mov    %rdi,0x20(%rsp)
+   1800058a3:	mov    %rbx,%rcx
+   1800058a6:	mov    0x80(%rbx),%rdi
+   1800058ad:	movb   $0x1,0x7c(%rbx)
+   1800058b1:	mov    %sil,0x71(%rbx)
+   1800058b5:	call   *0x390d(%rip)        # 0x1800091c8
+   1800058bb:	test   %rdi,%rdi
+   1800058be:	je     0x18000590e
+   1800058c0:	lea    0x50(%rsp),%r9
+   1800058c5:	mov    %rsi,0x40(%rsp)
+   1800058ca:	lea    0x48(%rsp),%r8
+   1800058cf:	mov    %rsi,0x48(%rsp)
+   1800058d4:	lea    0x40(%rsp),%rdx
+   1800058d9:	mov    %rsi,0x50(%rsp)
+   1800058de:	mov    %rdi,%rcx
+   1800058e1:	call   *0x3b71(%rip)        # 0x180009458
+   1800058e7:	mov    0x40(%rsp),%rax
+   1800058ec:	mov    %rax,0x18(%rbx)
+   1800058f0:	mov    %rax,0x20(%rbx)
+   1800058f4:	mov    0x48(%rsp),%rax
+   1800058f9:	mov    %rax,0x38(%rbx)
+   1800058fd:	mov    %rax,0x40(%rbx)
+   180005901:	mov    0x50(%rsp),%rax
+   180005906:	mov    %rax,0x50(%rbx)
+   18000590a:	mov    %rax,0x58(%rbx)
+   18000590e:	mov    %rdi,0x80(%rbx)
+   180005915:	mov    0x8d14(%rip),%rax        # 0x18000e630
+   18000591c:	mov    0x20(%rsp),%rdi
+   180005921:	mov    %rax,0x74(%rbx)
+   180005925:	mov    %rbx,%rax
+   180005928:	mov    %rsi,0x68(%rbx)
+   18000592c:	add    $0x28,%rsp
+   180005930:	pop    %rsi
+   180005931:	pop    %rbx
+   180005932:	ret
+   180005933:	xor    %eax,%eax
+   180005935:	add    $0x28,%rsp
+   180005939:	pop    %rsi
+   18000593a:	pop    %rbx
+   18000593b:	ret
+   18000593c:	int3
+   18000593d:	int3
+   18000593e:	int3
+   18000593f:	int3
+   180005940:	mov    %rbx,0x8(%rsp)
+   180005945:	push   %rdi
+   180005946:	sub    $0x70,%rsp
+   18000594a:	mov    %rcx,%rdx
+   18000594d:	lea    0x20(%rsp),%rcx
+   180005952:	call   0x1800028c0
+   180005957:	nop
+   180005958:	lea    0x20(%rsp),%rcx
+   18000595d:	call   0x1800059e0
+   180005962:	nop
+   180005963:	mov    0x68(%rsp),%rbx
+   180005968:	test   %rbx,%rbx
+   18000596b:	je     0x180005999
+   18000596d:	mov    $0xffffffff,%edi
+   180005972:	mov    %edi,%eax
+   180005974:	lock xadd %eax,0x8(%rbx)
+   180005979:	cmp    $0x1,%eax
+   18000597c:	jne    0x180005999
+   18000597e:	mov    (%rbx),%rax
+   180005981:	mov    %rbx,%rcx
+   180005984:	call   *(%rax)
+   180005986:	lock xadd %edi,0xc(%rbx)
+   18000598b:	cmp    $0x1,%edi
+   18000598e:	jne    0x180005999
+   180005990:	mov    (%rbx),%rax
+   180005993:	mov    %rbx,%rcx
+   180005996:	call   *0x8(%rax)
+   180005999:	lea    0x40(%rsp),%rcx
+   18000599e:	call   0x180002e30
+   1800059a3:	lea    0x30(%rsp),%rcx
+   1800059a8:	call   0x1800071fa
+   1800059ad:	mov    0x28(%rsp),%rcx
+   1800059b2:	test   %rcx,%rcx
+   1800059b5:	je     0x1800059c1
+   1800059b7:	mov    (%rcx),%rax
+   1800059ba:	mov    $0x1,%edx
+   1800059bf:	call   *(%rax)
+   1800059c1:	mov    $0x1,%al
+   1800059c3:	mov    0x80(%rsp),%rbx
+   1800059cb:	add    $0x70,%rsp
+   1800059cf:	pop    %rdi
+   1800059d0:	ret
+   1800059d1:	int3
+   1800059d2:	int3
+   1800059d3:	int3
+   1800059d4:	int3
+   1800059d5:	int3
+   1800059d6:	int3
+   1800059d7:	int3
+   1800059d8:	int3
+   1800059d9:	int3
+   1800059da:	int3
+   1800059db:	int3
+   1800059dc:	int3
+   1800059dd:	int3
+   1800059de:	int3
+   1800059df:	int3
+   1800059e0:	mov    %rsp,%rax
+   1800059e3:	mov    %rbx,0x10(%rax)
+   1800059e7:	mov    %rsi,0x18(%rax)
+   1800059eb:	mov    %rdi,0x20(%rax)
+   1800059ef:	push   %rbp
+   1800059f0:	push   %r12
+   1800059f2:	push   %r13
+   1800059f4:	push   %r14
+   1800059f6:	push   %r15
+   1800059f8:	lea    -0x3b8(%rax),%rbp
+   1800059ff:	sub    $0x490,%rsp
+   180005a06:	movaps %xmm6,-0x38(%rax)
+   180005a0a:	movaps %xmm7,-0x48(%rax)
+   180005a0e:	movaps %xmm8,-0x58(%rax)
+   180005a13:	movaps %xmm9,-0x68(%rax)
+   180005a18:	movaps %xmm10,-0x78(%rax)
+   180005a1d:	movaps %xmm11,-0x88(%rax)
+   180005a25:	movaps %xmm12,-0x98(%rax)
+   180005a2d:	movaps %xmm13,-0xa8(%rax)
+   180005a35:	mov    0x85cc(%rip),%rax        # 0x18000e008
+   180005a3c:	xor    %rsp,%rax
+   180005a3f:	mov    %rax,0x300(%rbp)
+   180005a46:	mov    %rcx,%r15
+   180005a49:	xor    %edi,%edi
+   180005a4b:	mov    %edi,0x48(%rsp)
+   180005a4f:	mov    (%rcx),%rcx
+   180005a52:	call   *0x3818(%rip)        # 0x180009270
+   180005a58:	mov    %eax,%r14d
+   180005a5b:	mov    %eax,0x50(%rsp)
+   180005a5f:	mov    (%r15),%rcx
+   180005a62:	call   *0x3828(%rip)        # 0x180009290
+   180005a68:	mov    %edi,0x140(%rbp)
+   180005a6e:	mov    %eax,0x144(%rbp)
+   180005a74:	movsd  0x140(%rbp),%xmm0
+   180005a7c:	movsd  %xmm0,0x190(%rbp)
+   180005a84:	mov    0x148(%rbp),%ecx
+   180005a8a:	mov    %ecx,0x198(%rbp)
+   180005a90:	mov    0x140(%rbp),%rcx
+   180005a97:	shr    $0x20,%rcx
+   180005a9b:	test   %ecx,%ecx
+   180005a9d:	je     0x180005af3
+   180005a9f:	mov    0x194(%rbp),%edi
+   180005aa5:	mov    0x190(%rbp),%ebx
+   180005aab:	nopl   0x0(%rax,%rax,1)
+   180005ab0:	mov    %ebx,%r8d
+   180005ab3:	lea    0x1c0(%rbp),%rdx
+   180005aba:	mov    (%r15),%rcx
+   180005abd:	call   0x18000722a
+   180005ac2:	movups (%rax),%xmm1
+   180005ac5:	movups 0x10(%rax),%xmm2
+   180005ac9:	movsd  0x20(%rax),%xmm0
+   180005ace:	mov    0x40(%r15),%rcx
+   180005ad2:	mov    %ebx,%eax
+   180005ad4:	lea    (%rax,%rax,4),%rdx
+   180005ad8:	mov    0x58(%rcx),%rax
+   180005adc:	movups %xmm1,(%rax,%rdx,8)
+   180005ae0:	movups %xmm2,0x10(%rax,%rdx,8)
+   180005ae5:	movsd  %xmm0,0x20(%rax,%rdx,8)
+   180005aeb:	inc    %ebx
+   180005aed:	cmp    %edi,%ebx
+   180005aef:	jne    0x180005ab0
+   180005af1:	xor    %edi,%edi
+   180005af3:	mov    %r15,%rcx
+   180005af6:	call   0x180004860
+   180005afb:	lea    0x3c0e(%rip),%rax        # 0x180009710
+   180005b02:	mov    %rax,0x60(%rsp)
+   180005b07:	lea    0x3c0a(%rip),%rax        # 0x180009718
+   180005b0e:	mov    %rax,0x70(%rsp)
+   180005b13:	lea    0x18(%rbp),%rcx
+   180005b17:	call   *0x35db(%rip)        # 0x1800090f8
+   180005b1d:	nop
+   180005b1e:	movl   $0x1,0x48(%rsp)
+   180005b26:	xor    %r8d,%r8d
+   180005b29:	lea    0x78(%rsp),%rdx
+   180005b2e:	lea    0x60(%rsp),%rcx
+   180005b33:	call   *0x3597(%rip)        # 0x1800090d0
+   180005b39:	nop
+   180005b3a:	mov    0x60(%rsp),%rax
+   180005b3f:	movslq 0x4(%rax),%rcx
+   180005b43:	lea    0x3bbe(%rip),%rax        # 0x180009708
+   180005b4a:	mov    %rax,0x60(%rsp,%rcx,1)
+   180005b4f:	mov    0x60(%rsp),%rax
+   180005b54:	movslq 0x4(%rax),%rcx
+   180005b58:	lea    -0xb8(%rcx),%edx
+   180005b5e:	mov    %edx,0x5c(%rsp,%rcx,1)
+   180005b62:	lea    0x78(%rsp),%rax
+   180005b67:	mov    %rax,0x140(%rbp)
+   180005b6e:	lea    0x78(%rsp),%rcx
+   180005b73:	call   *0x361f(%rip)        # 0x180009198
+   180005b79:	nop
+   180005b7a:	lea    0x3b07(%rip),%rax        # 0x180009688
+   180005b81:	mov    %rax,0x78(%rsp)
+   180005b86:	movb   $0x0,-0xc(%rbp)
+   180005b8a:	movb   $0x0,-0x17(%rbp)
+   180005b8e:	lea    0x78(%rsp),%rcx
+   180005b93:	call   *0x362f(%rip)        # 0x1800091c8
+   180005b99:	mov    %rdi,-0x8(%rbp)
+   180005b9d:	mov    0x8a8c(%rip),%rax        # 0x18000e630
+   180005ba4:	mov    %rax,-0x14(%rbp)
+   180005ba8:	mov    %rdi,-0x20(%rbp)
+   180005bac:	mov    $0xa,%edx
+   180005bb1:	lea    0x36(%rdx),%r8d
+   180005bb5:	lea    0x3bf4(%rip),%rcx        # 0x1800097b0
+   180005bbc:	call   0x1800072a0
+   180005bc1:	mov    %rax,%rbx
+   180005bc4:	test   %rax,%rax
+   180005bc7:	jne    0x180005beb
+   180005bc9:	mov    0x60(%rsp),%rax
+   180005bce:	movslq 0x4(%rax),%rcx
+   180005bd2:	lea    0x60(%rsp),%rax
+   180005bd7:	add    %rax,%rcx
+   180005bda:	xor    %r8d,%r8d
+   180005bdd:	lea    0x2(%rbx),%edx
+   180005be0:	call   *0x351a(%rip)        # 0x180009100
+   180005be6:	jmp    0x180005ce9
+   180005beb:	movb   $0x1,-0xc(%rbp)
+   180005bef:	movb   $0x0,-0x17(%rbp)
+   180005bf3:	lea    0x78(%rsp),%rcx
+   180005bf8:	call   *0x35ca(%rip)        # 0x1800091c8
+   180005bfe:	mov    %rdi,0x48(%rsp)
+   180005c03:	mov    %rdi,0x40(%rsp)
+   180005c08:	mov    %rdi,0x190(%rbp)
+   180005c0f:	lea    0x190(%rbp),%r9
+   180005c16:	lea    0x40(%rsp),%r8
+   180005c1b:	lea    0x48(%rsp),%rdx
+   180005c20:	mov    %rbx,%rcx
+   180005c23:	call   *0x382f(%rip)        # 0x180009458
+   180005c29:	mov    0x190(%rbp),%r9
+   180005c30:	mov    %r9,0x30(%rsp)
+   180005c35:	mov    0x40(%rsp),%r8
+   180005c3a:	mov    %r8,0x28(%rsp)
+   180005c3f:	mov    0x48(%rsp),%rdx
+   180005c44:	mov    %rdx,0x20(%rsp)
+   180005c49:	lea    0x78(%rsp),%rcx
+   180005c4e:	call   *0x34d4(%rip)        # 0x180009128
+   180005c54:	mov    %rbx,-0x8(%rbp)
+   180005c58:	mov    0x89d1(%rip),%rax        # 0x18000e630
+   180005c5f:	mov    %rax,-0x14(%rbp)
+   180005c63:	mov    %rdi,-0x20(%rbp)
+   180005c67:	lea    0x140(%rbp),%rdx
+   180005c6e:	lea    0x78(%rsp),%rcx
+   180005c73:	call   *0x352f(%rip)        # 0x1800091a8
+   180005c79:	nop
+   180005c7a:	mov    %rax,%rcx
+   180005c7d:	call   0x180002680
+   180005c82:	mov    %rax,%rbx
+   180005c85:	mov    %rax,%rcx
+   180005c88:	call   *0x34e2(%rip)        # 0x180009170
+   180005c8e:	test   %al,%al
+   180005c90:	je     0x180005c98
+   180005c92:	mov    %rdi,-0x20(%rbp)
+   180005c96:	jmp    0x180005ca8
+   180005c98:	mov    %rbx,-0x20(%rbp)
+   180005c9c:	lea    0x78(%rsp),%rcx
+   180005ca1:	call   *0x3521(%rip)        # 0x1800091c8
+   180005ca7:	nop
+   180005ca8:	mov    0x148(%rbp),%rcx
+   180005caf:	test   %rcx,%rcx
+   180005cb2:	je     0x180005ccd
+   180005cb4:	mov    (%rcx),%rax
+   180005cb7:	call   *0x10(%rax)
+   180005cba:	test   %rax,%rax
+   180005cbd:	je     0x180005ccd
+   180005cbf:	mov    (%rax),%r8
+   180005cc2:	mov    $0x1,%edx
+   180005cc7:	mov    %rax,%rcx
+   180005cca:	call   *(%r8)
+   180005ccd:	mov    0x60(%rsp),%rax
+   180005cd2:	movslq 0x4(%rax),%rcx
+   180005cd6:	lea    0x60(%rsp),%rax
+   180005cdb:	add    %rax,%rcx
+   180005cde:	xor    %r8d,%r8d
+   180005ce1:	xor    %edx,%edx
+   180005ce3:	call   *0x341f(%rip)        # 0x180009108
+   180005ce9:	lea    0x3ad8(%rip),%rdx        # 0x1800097c8
+   180005cf0:	lea    0x70(%rsp),%rcx
+   180005cf5:	call   0x180001290
+   180005cfa:	mov    %rax,%rcx
+   180005cfd:	lea    0x3abc(%rip),%rdx        # 0x1800097c0
+   180005d04:	call   0x180001290
+   180005d09:	xorps  %xmm10,%xmm10
+   180005d0d:	xorps  %xmm11,%xmm11
+   180005d11:	mov    0x28(%r15),%r9
+   180005d15:	mov    0x20(%r15),%r8
+   180005d19:	mov    $0xfffffffffffffff0,%r13
+   180005d20:	lea    0x3ab9(%rip),%rsi        # 0x1800097e0
+   180005d27:	cmp    %r9,%r8
+   180005d2a:	je     0x18000675e
+   180005d30:	lea    0x10(%r15),%rsi
+   180005d34:	movsd  0x3c43(%rip),%xmm12        # 0x180009980
+   180005d3d:	movsd  0x3c42(%rip),%xmm13        # 0x180009988
+   180005d46:	movabs $0x2e8ba2e8ba2e8ba3,%r10
+   180005d50:	movups (%r8),%xmm0
+   180005d54:	movaps %xmm0,0xe0(%rbp)
+   180005d5b:	movups 0x10(%r8),%xmm1
+   180005d60:	movaps %xmm1,0xf0(%rbp)
+   180005d67:	movups 0x20(%r8),%xmm0
+   180005d6c:	movaps %xmm0,0x100(%rbp)
+   180005d73:	movups 0x30(%r8),%xmm1
+   180005d78:	movaps %xmm1,0x110(%rbp)
+   180005d7f:	movups 0x40(%r8),%xmm0
+   180005d84:	movaps %xmm0,0x120(%rbp)
+   180005d8b:	movsd  0x50(%r8),%xmm1
+   180005d91:	movsd  %xmm1,0x130(%rbp)
+   180005d99:	mov    %r9,%rcx
+   180005d9c:	sub    %r8,%rcx
+   180005d9f:	mov    %r10,%rax
+   180005da2:	imul   %rcx
+   180005da5:	sar    $0x4,%rdx
+   180005da9:	mov    %rdx,%rax
+   180005dac:	shr    $0x3f,%rax
+   180005db0:	add    %rax,%rdx
+   180005db3:	cmp    $0x2,%rdx
+   180005db7:	jl     0x180005fc4
+   180005dbd:	lea    -0x58(%r9),%rcx
+   180005dc1:	movups (%rcx),%xmm4
+   180005dc4:	movups 0x10(%rcx),%xmm3
+   180005dc8:	movaps %xmm3,0x90(%rbp)
+   180005dcf:	movups 0x20(%rcx),%xmm5
+   180005dd3:	movups 0x30(%rcx),%xmm6
+   180005dd7:	movups 0x40(%rcx),%xmm7
+   180005ddb:	movsd  0x50(%rcx),%xmm8
+   180005de1:	movups (%r8),%xmm0
+   180005de5:	movups %xmm0,(%rcx)
+   180005de8:	movups 0x10(%r8),%xmm1
+   180005ded:	movups %xmm1,0x10(%rcx)
+   180005df1:	movups 0x20(%r8),%xmm0
+   180005df6:	movups %xmm0,0x20(%rcx)
+   180005dfa:	movups 0x30(%r8),%xmm1
+   180005dff:	movups %xmm1,0x30(%rcx)
+   180005e03:	movups 0x40(%r8),%xmm0
+   180005e08:	movups %xmm0,0x40(%rcx)
+   180005e0c:	movsd  0x50(%r8),%xmm1
+   180005e12:	movsd  %xmm1,0x50(%rcx)
+   180005e17:	sub    %r8,%rcx
+   180005e1a:	mov    %r10,%rax
+   180005e1d:	imul   %rcx
+   180005e20:	sar    $0x4,%rdx
+   180005e24:	mov    %rdx,%rax
+   180005e27:	shr    $0x3f,%rax
+   180005e2b:	add    %rax,%rdx
+   180005e2e:	mov    %rdi,%r10
+   180005e31:	mov    %rdi,%r9
+   180005e34:	lea    -0x1(%rdx),%r11
+   180005e38:	sar    %r11
+   180005e3b:	test   %r11,%r11
+   180005e3e:	jle    0x180005ebe
+   180005e40:	lea    (%r9,%r9,1),%rcx
+   180005e44:	imul   $0x58,%rcx,%rax
+   180005e48:	mov    %rdi,%r9
+   180005e4b:	movsd  0xc0(%rax,%r8,1),%xmm0
+   180005e55:	comisd 0x68(%rax,%r8,1),%xmm0
+   180005e5c:	setb   %r9b
+   180005e60:	inc    %rcx
+   180005e63:	add    %rcx,%r9
+   180005e66:	imul   $0x58,%r9,%rax
+   180005e6a:	imul   $0x58,%r10,%rcx
+   180005e6e:	movups (%rax,%r8,1),%xmm0
+   180005e73:	movups %xmm0,(%rcx,%r8,1)
+   180005e78:	movups 0x10(%rax,%r8,1),%xmm1
+   180005e7e:	movups %xmm1,0x10(%rcx,%r8,1)
+   180005e84:	movups 0x20(%rax,%r8,1),%xmm0
+   180005e8a:	movups %xmm0,0x20(%rcx,%r8,1)
+   180005e90:	movups 0x30(%rax,%r8,1),%xmm1
+   180005e96:	movups %xmm1,0x30(%rcx,%r8,1)
+   180005e9c:	movups 0x40(%rax,%r8,1),%xmm0
+   180005ea2:	movups %xmm0,0x40(%rcx,%r8,1)
+   180005ea8:	movsd  0x50(%rax,%r8,1),%xmm1
+   180005eaf:	movsd  %xmm1,0x50(%rcx,%r8,1)
+   180005eb6:	mov    %r9,%r10
+   180005eb9:	cmp    %r11,%r9
+   180005ebc:	jl     0x180005e40
+   180005ebe:	cmp    %r11,%r10
+   180005ec1:	jne    0x180005f1d
+   180005ec3:	test   $0x1,%dl
+   180005ec6:	jne    0x180005f1d
+   180005ec8:	imul   $0x58,%rdx,%rax
+   180005ecc:	imul   $0x58,%r10,%rcx
+   180005ed0:	movups -0x58(%rax,%r8,1),%xmm0
+   180005ed6:	movups %xmm0,(%rcx,%r8,1)
+   180005edb:	movups -0x48(%rax,%r8,1),%xmm1
+   180005ee1:	movups %xmm1,0x10(%rcx,%r8,1)
+   180005ee7:	movups -0x38(%rax,%r8,1),%xmm0
+   180005eed:	movups %xmm0,0x20(%rcx,%r8,1)
+   180005ef3:	movups -0x28(%rax,%r8,1),%xmm1
+   180005ef9:	movups %xmm1,0x30(%rcx,%r8,1)
+   180005eff:	movups -0x18(%rax,%r8,1),%xmm0
+   180005f05:	movups %xmm0,0x40(%rcx,%r8,1)
+   180005f0b:	movsd  -0x8(%rax,%r8,1),%xmm1
+   180005f12:	movsd  %xmm1,0x50(%rcx,%r8,1)
+   180005f19:	lea    -0x1(%rdx),%r10
+   180005f1d:	test   %r10,%r10
+   180005f20:	jle    0x180005f9c
+   180005f22:	movsd  0x90(%rbp),%xmm2
+   180005f2a:	nopw   0x0(%rax,%rax,1)
+   180005f30:	lea    -0x1(%r10),%rdx
+   180005f34:	sar    %rdx
+   180005f37:	imul   $0x58,%rdx,%rcx
+   180005f3b:	movsd  0x10(%rcx,%r8,1),%xmm0
+   180005f42:	comisd %xmm2,%xmm0
+   180005f46:	jb     0x180005f9c
+   180005f48:	imul   $0x58,%r10,%rax
+   180005f4c:	movups (%rcx,%r8,1),%xmm0
+   180005f51:	movups %xmm0,(%rax,%r8,1)
+   180005f56:	movups 0x10(%rcx,%r8,1),%xmm1
+   180005f5c:	movups %xmm1,0x10(%rax,%r8,1)
+   180005f62:	movups 0x20(%rcx,%r8,1),%xmm0
+   180005f68:	movups %xmm0,0x20(%rax,%r8,1)
+   180005f6e:	movups 0x30(%rcx,%r8,1),%xmm1
+   180005f74:	movups %xmm1,0x30(%rax,%r8,1)
+   180005f7a:	movups 0x40(%rcx,%r8,1),%xmm0
+   180005f80:	movups %xmm0,0x40(%rax,%r8,1)
+   180005f86:	movsd  0x50(%rcx,%r8,1),%xmm1
+   180005f8d:	movsd  %xmm1,0x50(%rax,%r8,1)
+   180005f94:	mov    %rdx,%r10
+   180005f97:	test   %rdx,%rdx
+   180005f9a:	jg     0x180005f30
+   180005f9c:	imul   $0x58,%r10,%rax
+   180005fa0:	movups %xmm4,(%rax,%r8,1)
+   180005fa5:	movups %xmm3,0x10(%rax,%r8,1)
+   180005fab:	movups %xmm5,0x20(%rax,%r8,1)
+   180005fb1:	movups %xmm6,0x30(%rax,%r8,1)
+   180005fb7:	movups %xmm7,0x40(%rax,%r8,1)
+   180005fbd:	movsd  %xmm8,0x50(%rax,%r8,1)
+   180005fc4:	addq   $0xffffffffffffffa8,0x28(%r15)
+   180005fc9:	movsd  0xe8(%rbp),%xmm11
+   180005fd2:	mov    0xe0(%rbp),%edx
+   180005fd8:	mov    %rsi,%rcx
+   180005fdb:	call   0x180007200
+   180005fe0:	test   %al,%al
+   180005fe2:	je     0x180006746
+   180005fe8:	comisd %xmm12,%xmm11
+   180005fed:	jbe    0x180005ffa
+   180005fef:	comisd %xmm11,%xmm13
+   180005ff4:	ja     0x180006746
+   180005ffa:	lea    0xf8(%rbp),%r8
+   180006001:	mov    0xe0(%rbp),%edx
+   180006007:	mov    (%r15),%rcx
+   18000600a:	call   0x180007212
+   18000600f:	test   %al,%al
+   180006011:	je     0x180006746
+   180006017:	lea    0xf8(%rbp),%r9
+   18000601e:	mov    0xe0(%rbp),%r8d
+   180006025:	lea    0x240(%rbp),%rdx
+   18000602c:	mov    %rsi,%rcx
+   18000602f:	call   0x180007206
+   180006034:	nop
+   180006035:	movsd  %xmm10,0x190(%rbp)
+   18000603e:	movsd  %xmm10,0x40(%rsp)
+   180006045:	mov    0x190(%rbp),%rax
+   18000604c:	xorps  %xmm0,%xmm0
+   18000604f:	cmp    0x40(%rsp),%rax
+   180006054:	jne    0x180006061
+   180006056:	xor    %eax,%eax
+   180006058:	mov    %rax,0x2c0(%rbp)
+   18000605f:	jmp    0x18000606a
+   180006061:	movsd  %xmm10,0x2c0(%rbp)
+   18000606a:	cmpb   $0x0,0x110(%rbp)
+   180006071:	je     0x18000609a
+   180006073:	movups 0x118(%rbp),%xmm0
+   18000607a:	movups %xmm0,0x140(%rbp)
+   180006081:	movsd  0x128(%rbp),%xmm1
+   180006089:	movsd  %xmm1,0x150(%rbp)
+   180006091:	lea    0x140(%rbp),%rax
+   180006098:	jmp    0x1800060b8
+   18000609a:	movups %xmm0,0x190(%rbp)
+   1800060a1:	movsd  0x2c0(%rbp),%xmm0
+   1800060a9:	movsd  %xmm0,0x1a0(%rbp)
+   1800060b1:	lea    0x190(%rbp),%rax
+   1800060b8:	movb   $0x1,0x160(%rbp)
+   1800060bf:	movups (%rax),%xmm0
+   1800060c2:	movups %xmm0,0x168(%rbp)
+   1800060c9:	movsd  0x10(%rax),%xmm2
+   1800060ce:	mov    0x40(%r15),%rcx
+   1800060d2:	mov    0x240(%rbp),%eax
+   1800060d8:	lea    (%rax,%rax,4),%rdx
+   1800060dc:	mov    0x58(%rcx),%rax
+   1800060e0:	movups 0x160(%rbp),%xmm0
+   1800060e7:	movups %xmm0,(%rax,%rdx,8)
+   1800060eb:	movups 0x170(%rbp),%xmm1
+   1800060f2:	unpcklpd %xmm2,%xmm1
+   1800060f6:	movups %xmm1,0x170(%rbp)
+   1800060fd:	movups %xmm1,0x10(%rax,%rdx,8)
+   180006102:	movsd  0x180(%rbp),%xmm0
+   18000610a:	movsd  %xmm0,0x20(%rax,%rdx,8)
+   180006110:	mov    0x290(%rbp),%rdi
+   180006117:	mov    0x298(%rbp),%rax
+   18000611e:	mov    %rax,0x140(%rbp)
+   180006125:	cmp    %rax,%rdi
+   180006128:	je     0x180006440
+   18000612e:	xchg   %ax,%ax
+   180006130:	mov    (%rdi),%r14d
+   180006133:	mov    %r14d,0x48(%rsp)
+   180006138:	mov    %r14d,%edx
+   18000613b:	mov    %rsi,%rcx
+   18000613e:	call   0x180007200
+   180006143:	test   %al,%al
+   180006145:	je     0x18000641c
+   18000614b:	mov    (%r15),%rcx
+   18000614e:	call   *0x3144(%rip)        # 0x180009298
+   180006154:	mov    %rax,%rcx
+   180006157:	mov    %r14d,%edx
+   18000615a:	call   *0x30f0(%rip)        # 0x180009250
+   180006160:	mov    %rax,%rsi
+   180006163:	mov    0x40(%r15),%rcx
+   180006167:	mov    (%rcx),%r8
+   18000616a:	mov    (%rax),%edx
+   18000616c:	call   *0x80(%r8)
+   180006173:	movups (%rax),%xmm6
+   180006176:	movups %xmm6,0x1c0(%rbp)
+   18000617d:	movups 0x10(%rax),%xmm0
+   180006181:	movups %xmm0,0x1d0(%rbp)
+   180006188:	movsd  0x20(%rax),%xmm1
+   18000618d:	movsd  %xmm1,0x1e0(%rbp)
+   180006195:	mov    0x40(%r15),%rcx
+   180006199:	mov    (%rcx),%rax
+   18000619c:	mov    0x4(%rsi),%edx
+   18000619f:	call   *0x80(%rax)
+   1800061a5:	movups (%rax),%xmm0
+   1800061a8:	movups %xmm0,0x2d0(%rbp)
+   1800061af:	movups 0x10(%rax),%xmm1
+   1800061b3:	movups %xmm1,0x2e0(%rbp)
+   1800061ba:	movsd  0x20(%rax),%xmm0
+   1800061bf:	movsd  %xmm0,0x2f0(%rbp)
+   1800061c7:	lea    0x4(%rsi),%r9
+   1800061cb:	mov    %rsi,%r8
+   1800061ce:	lea    0x208(%rbp),%rdx
+   1800061d5:	mov    %r15,%rcx
+   1800061d8:	call   0x180003f20
+   1800061dd:	mov    %rsi,%r9
+   1800061e0:	lea    0x4(%rsi),%r8
+   1800061e4:	lea    0x160(%rbp),%rdx
+   1800061eb:	mov    %r15,%rcx
+   1800061ee:	call   0x180003f20
+   1800061f3:	movd   %xmm6,%eax
+   1800061f7:	test   %al,%al
+   1800061f9:	je     0x18000639f
+   1800061ff:	cmpb   $0x0,0x2d0(%rbp)
+   180006206:	je     0x18000639f
+   18000620c:	cmpb   $0x0,0x208(%rbp)
+   180006213:	je     0x18000639f
+   180006219:	cmpb   $0x0,0x160(%rbp)
+   180006220:	je     0x18000639f
+   180006226:	lea    0x210(%rbp),%rdx
+   18000622d:	lea    0x1c8(%rbp),%rcx
+   180006234:	call   0x180003ed0
+   180006239:	movaps %xmm0,%xmm7
+   18000623c:	lea    0x168(%rbp),%rdx
+   180006243:	lea    0x2d8(%rbp),%rcx
+   18000624a:	call   0x180003ed0
+   18000624f:	movaps %xmm0,%xmm8
+   180006253:	mov    (%r15),%rcx
+   180006256:	mov    %rsi,%rdx
+   180006259:	call   *0x3009(%rip)        # 0x180009268
+   18000625f:	movaps %xmm0,%xmm6
+   180006262:	comisd %xmm8,%xmm7
+   180006267:	jbe    0x180006270
+   180006269:	mulsd  %xmm8,%xmm6
+   18000626e:	jmp    0x180006274
+   180006270:	mulsd  %xmm7,%xmm6
+   180006274:	movsd  %xmm6,0x40(%rsp)
+   18000627a:	mov    %rsi,%rdx
+   18000627d:	mov    (%r15),%rcx
+   180006280:	call   *0x2fe2(%rip)        # 0x180009268
+   180006286:	movaps %xmm0,%xmm9
+   18000628a:	movsd  %xmm0,0x190(%rbp)
+   180006292:	mov    (%r15),%rcx
+   180006295:	add    $0x18,%rcx
+   180006299:	comisd %xmm7,%xmm8
+   18000629e:	jbe    0x180006337
+   1800062a4:	mov    (%rsi),%edx
+   1800062a6:	call   *0x2fcc(%rip)        # 0x180009278
+   1800062ac:	mov    0x28(%r15),%rdx
+   1800062b0:	cmp    0x30(%r15),%rdx
+   1800062b4:	je     0x180006302
+   1800062b6:	movups (%rax),%xmm1
+   1800062b9:	movsd  0x10(%rax),%xmm0
+   1800062be:	movsd  %xmm6,0x8(%rdx)
+   1800062c3:	movsd  %xmm9,0x10(%rdx)
+   1800062c9:	mov    %r14d,(%rdx)
+   1800062cc:	movups %xmm1,0x18(%rdx)
+   1800062d0:	movsd  %xmm0,0x28(%rdx)
+   1800062d5:	movups 0x208(%rbp),%xmm1
+   1800062dc:	movups %xmm1,0x30(%rdx)
+   1800062e0:	movups 0x218(%rbp),%xmm0
+   1800062e7:	movups %xmm0,0x40(%rdx)
+   1800062eb:	movsd  0x228(%rbp),%xmm1
+   1800062f3:	movsd  %xmm1,0x50(%rdx)
+   1800062f8:	addq   $0x58,0x28(%r15)
+   1800062fd:	jmp    0x180006406
+   180006302:	lea    0x208(%rbp),%rcx
+   180006309:	mov    %rcx,0x30(%rsp)
+   18000630e:	mov    %rax,0x28(%rsp)
+   180006313:	lea    0x190(%rbp),%rax
+   18000631a:	mov    %rax,0x20(%rsp)
+   18000631f:	lea    0x40(%rsp),%r9
+   180006324:	lea    0x48(%rsp),%r8
+   180006329:	lea    0x20(%r15),%rcx
+   18000632d:	call   0x1800015d0
+   180006332:	jmp    0x180006406
+   180006337:	mov    0x4(%rsi),%edx
+   18000633a:	call   *0x2f38(%rip)        # 0x180009278
+   180006340:	mov    0x28(%r15),%rdx
+   180006344:	cmp    0x30(%r15),%rdx
+   180006348:	je     0x180006393
+   18000634a:	movups (%rax),%xmm1
+   18000634d:	movsd  0x10(%rax),%xmm0
+   180006352:	mov    %r14d,(%rdx)
+   180006355:	movsd  %xmm6,0x8(%rdx)
+   18000635a:	movsd  %xmm9,0x10(%rdx)
+   180006360:	movups %xmm1,0x18(%rdx)
+   180006364:	movsd  %xmm0,0x28(%rdx)
+   180006369:	movups 0x160(%rbp),%xmm1
+   180006370:	movups %xmm1,0x30(%rdx)
+   180006374:	movups 0x170(%rbp),%xmm0
+   18000637b:	movups %xmm0,0x40(%rdx)
+   18000637f:	movsd  0x180(%rbp),%xmm1
+   180006387:	movsd  %xmm1,0x50(%rdx)
+   18000638c:	addq   $0x58,0x28(%r15)
+   180006391:	jmp    0x180006406
+   180006393:	lea    0x160(%rbp),%rcx
+   18000639a:	jmp    0x180006309
+   18000639f:	xor    %eax,%eax
+   1800063a1:	mov    %eax,0x40(%rsp)
+   1800063a5:	mov    %eax,0x190(%rbp)
+   1800063ab:	mov    (%r15),%rcx
+   1800063ae:	add    $0x18,%rcx
+   1800063b2:	mov    (%rsi),%edx
+   1800063b4:	call   *0x2ebe(%rip)        # 0x180009278
+   1800063ba:	mov    0x28(%r15),%rdx
+   1800063be:	cmp    0x30(%r15),%rdx
+   1800063c2:	je     0x1800063d6
+   1800063c4:	movups (%rax),%xmm1
+   1800063c7:	movsd  0x10(%rax),%xmm0
+   1800063cc:	movups %xmm10,0x8(%rdx)
+   1800063d1:	jmp    0x1800062c9
+   1800063d6:	lea    0x208(%rbp),%rcx
+   1800063dd:	mov    %rcx,0x30(%rsp)
+   1800063e2:	mov    %rax,0x28(%rsp)
+   1800063e7:	lea    0x40(%rsp),%rax
+   1800063ec:	mov    %rax,0x20(%rsp)
+   1800063f1:	lea    0x190(%rbp),%r9
+   1800063f8:	lea    0x48(%rsp),%r8
+   1800063fd:	lea    0x20(%r15),%rcx
+   180006401:	call   0x180001850
+   180006406:	mov    0x28(%r15),%rdx
+   18000640a:	movzbl 0x38(%r15),%r8d
+   18000640f:	mov    0x20(%r15),%rcx
+   180006413:	call   0x180002560
+   180006418:	lea    0x10(%r15),%rsi
+   18000641c:	add    $0x20,%rdi
+   180006420:	cmp    0x140(%rbp),%rdi
+   180006427:	jne    0x180006130
+   18000642d:	mov    0x290(%rbp),%rdi
+   180006434:	mov    0x50(%rsp),%r14d
+   180006439:	mov    $0xfffffffffffffff0,%r13
+   180006440:	add    $0xfffffffe,%r14d
+   180006444:	mov    %r14d,0x50(%rsp)
+   180006449:	mov    $0xd1b71759,%eax
+   18000644e:	mul    %r14d
+   180006451:	shr    $0xd,%edx
+   180006454:	imul   $0x2710,%edx,%ecx
+   18000645a:	cmp    %ecx,%r14d
+   18000645d:	jne    0x180006593
+   180006463:	lea    0x170(%rbp),%rdx
+   18000646a:	mov    %r14d,%ecx
+   18000646d:	call   0x18000723c
+   180006472:	lea    0x160(%rbp),%rdx
+   180006479:	mov    %r13,%rcx
+   18000647c:	sub    %rdx,%rcx
+   18000647f:	add    %rcx,%rax
+   180006482:	lea    0x170(%rbp),%rcx
+   180006489:	mov    %rcx,0x160(%rbp)
+   180006490:	mov    %rax,0x168(%rbp)
+   180006497:	lea    0x3342(%rip),%rcx        # 0x1800097e0
+   18000649e:	mov    %rcx,0x208(%rbp)
+   1800064a5:	mov    %rcx,%rax
+   1800064a8:	inc    %rax
+   1800064ab:	cmpb   $0x0,(%rax)
+   1800064ae:	jne    0x1800064a8
+   1800064b0:	sub    %rcx,%rax
+   1800064b3:	mov    %rax,0x210(%rbp)
+   1800064ba:	lea    0x3327(%rip),%rcx        # 0x1800097e8
+   1800064c1:	mov    %rcx,0x190(%rbp)
+   1800064c8:	mov    %rcx,%rax
+   1800064cb:	nopl   0x0(%rax,%rax,1)
+   1800064d0:	inc    %rax
+   1800064d3:	cmpb   $0x0,(%rax)
+   1800064d6:	jne    0x1800064d0
+   1800064d8:	sub    %rcx,%rax
+   1800064db:	mov    %rax,0x198(%rbp)
+   1800064e2:	lea    0x160(%rbp),%r9
+   1800064e9:	lea    0x208(%rbp),%r8
+   1800064f0:	lea    0x190(%rbp),%rdx
+   1800064f7:	lea    0x140(%rbp),%rcx
+   1800064fe:	call   0x180007242
+   180006503:	nop
+   180006504:	mov    %rax,%rcx
+   180006507:	call   *0x2cfb(%rip)        # 0x180009208
+   18000650d:	nop
+   18000650e:	mov    0x158(%rbp),%rdx
+   180006515:	cmp    $0x10,%rdx
+   180006519:	jb     0x18000654f
+   18000651b:	inc    %rdx
+   18000651e:	mov    0x140(%rbp),%rcx
+   180006525:	mov    %rcx,%rax
+   180006528:	cmp    $0x1000,%rdx
+   18000652f:	jb     0x18000654a
+   180006531:	add    $0x27,%rdx
+   180006535:	mov    -0x8(%rcx),%rcx
+   180006539:	sub    %rcx,%rax
+   18000653c:	add    $0xfffffffffffffff8,%rax
+   180006540:	cmp    $0x1f,%rax
+   180006544:	ja     0x18000681b
+   18000654a:	call   0x1800073b8
+   18000654f:	mov    %r14d,%edx
+   180006552:	lea    0x70(%rsp),%rcx
+   180006557:	call   *0x2b8b(%rip)        # 0x1800090e8
+   18000655d:	mov    %rax,%rcx
+   180006560:	lea    0x3295(%rip),%rdx        # 0x1800097fc
+   180006567:	call   0x180001290
+   18000656c:	mov    %rax,%rcx
+   18000656f:	movsd  0xe8(%rbp),%xmm1
+   180006577:	call   *0x2b63(%rip)        # 0x1800090e0
+   18000657d:	mov    %rax,%rcx
+   180006580:	lea    0x3239(%rip),%rdx        # 0x1800097c0
+   180006587:	call   0x180001290
+   18000658c:	mov    0x290(%rbp),%rdi
+   180006593:	test   %rdi,%rdi
+   180006596:	je     0x180006652
+   18000659c:	mov    0x298(%rbp),%rsi
+   1800065a3:	cmp    %rsi,%rdi
+   1800065a6:	je     0x180006603
+   1800065a8:	lea    0x10(%rdi),%rbx
+   1800065ac:	nopl   0x0(%rax)
+   1800065b0:	testb  $0x1,-0x8(%rbx)
+   1800065b4:	je     0x1800065ef
+   1800065b6:	mov    0x8(%rbx),%rax
+   1800065ba:	mov    (%rbx),%rcx
+   1800065bd:	lea    0x0(,%rax,4),%rdx
+   1800065c5:	cmp    $0x1000,%rdx
+   1800065cc:	jb     0x1800065ea
+   1800065ce:	add    $0x27,%rdx
+   1800065d2:	mov    -0x8(%rcx),%r8
+   1800065d6:	sub    %r8,%rcx
+   1800065d9:	lea    -0x8(%rcx),%rax
+   1800065dd:	cmp    $0x1f,%rax
+   1800065e1:	ja     0x180006822
+   1800065e7:	mov    %r8,%rcx
+   1800065ea:	call   0x1800073b8
+   1800065ef:	add    $0x20,%rbx
+   1800065f3:	lea    -0x10(%rbx),%rax
+   1800065f7:	cmp    %rsi,%rax
+   1800065fa:	jne    0x1800065b0
+   1800065fc:	mov    0x290(%rbp),%rdi
+   180006603:	mov    0x2a0(%rbp),%rdx
+   18000660a:	sub    %rdi,%rdx
+   18000660d:	and    $0xffffffffffffffe0,%rdx
+   180006611:	mov    %rdi,%rax
+   180006614:	cmp    $0x1000,%rdx
+   18000661b:	jb     0x180006636
+   18000661d:	add    $0x27,%rdx
+   180006621:	mov    -0x8(%rdi),%rdi
+   180006625:	sub    %rdi,%rax
+   180006628:	add    $0xfffffffffffffff8,%rax
+   18000662c:	cmp    $0x1f,%rax
+   180006630:	ja     0x180006822
+   180006636:	mov    %rdi,%rcx
+   180006639:	call   0x1800073b8
+   18000663e:	xorps  %xmm0,%xmm0
+   180006641:	movdqa %xmm0,0x290(%rbp)
+   180006649:	xor    %edi,%edi
+   18000664b:	mov    %rdi,0x2a0(%rbp)
+   180006652:	mov    0x278(%rbp),%rcx
+   180006659:	test   %rcx,%rcx
+   18000665c:	je     0x1800066b0
+   18000665e:	mov    0x288(%rbp),%rax
+   180006665:	sub    %rcx,%rax
+   180006668:	sar    $0x3,%rax
+   18000666c:	lea    0x0(,%rax,8),%rdx
+   180006674:	mov    %rcx,%rax
+   180006677:	cmp    $0x1000,%rdx
+   18000667e:	jb     0x180006699
+   180006680:	add    $0x27,%rdx
+   180006684:	mov    -0x8(%rcx),%rcx
+   180006688:	sub    %rcx,%rax
+   18000668b:	add    $0xfffffffffffffff8,%rax
+   18000668f:	cmp    $0x1f,%rax
+   180006693:	ja     0x180006822
+   180006699:	call   0x1800073b8
+   18000669e:	mov    %rdi,0x278(%rbp)
+   1800066a5:	xorps  %xmm0,%xmm0
+   1800066a8:	movdqa %xmm0,0x280(%rbp)
+   1800066b0:	testb  $0x1,0x260(%rbp)
+   1800066b7:	je     0x1800066f9
+   1800066b9:	mov    0x270(%rbp),%rax
+   1800066c0:	lea    0x0(,%rax,4),%rdx
+   1800066c8:	mov    0x268(%rbp),%rcx
+   1800066cf:	mov    %rcx,%rax
+   1800066d2:	cmp    $0x1000,%rdx
+   1800066d9:	jb     0x1800066f4
+   1800066db:	add    $0x27,%rdx
+   1800066df:	mov    -0x8(%rcx),%rcx
+   1800066e3:	sub    %rcx,%rax
+   1800066e6:	add    $0xfffffffffffffff8,%rax
+   1800066ea:	cmp    $0x1f,%rax
+   1800066ee:	ja     0x180006822
+   1800066f4:	call   0x1800073b8
+   1800066f9:	testb  $0x1,0x248(%rbp)
+   180006700:	je     0x180006742
+   180006702:	mov    0x258(%rbp),%rax
+   180006709:	lea    0x0(,%rax,4),%rdx
+   180006711:	mov    0x250(%rbp),%rcx
+   180006718:	mov    %rcx,%rax
+   18000671b:	cmp    $0x1000,%rdx
+   180006722:	jb     0x18000673d
+   180006724:	add    $0x27,%rdx
+   180006728:	mov    -0x8(%rcx),%rcx
+   18000672c:	sub    %rcx,%rax
+   18000672f:	add    $0xfffffffffffffff8,%rax
+   180006733:	cmp    $0x1f,%rax
+   180006737:	ja     0x180006822
+   18000673d:	call   0x1800073b8
+   180006742:	lea    0x10(%r15),%rsi
+   180006746:	mov    0x28(%r15),%r9
+   18000674a:	mov    0x20(%r15),%r8
+   18000674e:	cmp    %r9,%r8
+   180006751:	jne    0x180005d46
+   180006757:	lea    0x3082(%rip),%rsi        # 0x1800097e0
+   18000675e:	mov    %r14d,%edx
+   180006761:	lea    0x70(%rsp),%rcx
+   180006766:	call   *0x297c(%rip)        # 0x1800090e8
+   18000676c:	mov    %rax,%rcx
+   18000676f:	lea    0x3086(%rip),%rdx        # 0x1800097fc
+   180006776:	call   0x180001290
+   18000677b:	mov    %rax,%rcx
+   18000677e:	movaps %xmm11,%xmm1
+   180006782:	call   *0x2958(%rip)        # 0x1800090e0
+   180006788:	mov    %rax,%rcx
+   18000678b:	lea    0x302e(%rip),%rdx        # 0x1800097c0
+   180006792:	call   0x180001290
+   180006797:	cmpq   $0x0,-0x8(%rbp)
+   18000679c:	je     0x180006829
+   1800067a2:	mov    -0x70(%rbp),%rax
+   1800067a6:	lea    -0x18(%rbp),%rcx
+   1800067aa:	cmp    %rcx,(%rax)
+   1800067ad:	jne    0x1800067c9
+   1800067af:	mov    0x8(%rbp),%rdx
+   1800067b3:	mov    0x0(%rbp),%rcx
+   1800067b7:	mov    %rcx,(%rax)
+   1800067ba:	mov    -0x50(%rbp),%rax
+   1800067be:	mov    %rcx,(%rax)
+   1800067c1:	sub    %ecx,%edx
+   1800067c3:	mov    -0x38(%rbp),%rax
+   1800067c7:	mov    %edx,(%rax)
+   1800067c9:	lea    0x78(%rsp),%rbx
+   1800067ce:	lea    0x78(%rsp),%rcx
+   1800067d3:	call   0x1800036f0
+   1800067d8:	test   %al,%al
+   1800067da:	cmove  %rdi,%rbx
+   1800067de:	mov    -0x8(%rbp),%rcx
+   1800067e2:	call   *0x2c68(%rip)        # 0x180009450
+   1800067e8:	test   %eax,%eax
+   1800067ea:	cmovne %rdi,%rbx
+   1800067ee:	movb   $0x0,-0xc(%rbp)
+   1800067f2:	movb   $0x0,-0x17(%rbp)
+   1800067f6:	lea    0x78(%rsp),%rcx
+   1800067fb:	call   *0x29c7(%rip)        # 0x1800091c8
+   180006801:	mov    %rdi,-0x8(%rbp)
+   180006805:	mov    0x7e24(%rip),%rax        # 0x18000e630
+   18000680c:	mov    %rax,-0x14(%rbp)
+   180006810:	mov    %rdi,-0x20(%rbp)
+   180006814:	test   %rbx,%rbx
+   180006817:	jne    0x18000686d
+   180006819:	jmp    0x18000684f
+   18000681b:	call   *0x2b97(%rip)        # 0x1800093b8
+   180006821:	nop
+   180006822:	call   *0x2b90(%rip)        # 0x1800093b8
+   180006828:	int3
+   180006829:	movb   $0x0,-0xc(%rbp)
+   18000682d:	movb   $0x0,-0x17(%rbp)
+   180006831:	lea    0x78(%rsp),%rcx
+   180006836:	call   *0x298c(%rip)        # 0x1800091c8
+   18000683c:	mov    %rdi,-0x8(%rbp)
+   180006840:	mov    0x7de9(%rip),%rax        # 0x18000e630
+   180006847:	mov    %rax,-0x14(%rbp)
+   18000684b:	mov    %rdi,-0x20(%rbp)
+   18000684f:	mov    0x60(%rsp),%rax
+   180006854:	movslq 0x4(%rax),%rcx
+   180006858:	lea    0x60(%rsp),%rax
+   18000685d:	add    %rax,%rcx
+   180006860:	xor    %r8d,%r8d
+   180006863:	lea    0x2(%r8),%edx
+   180006867:	call   *0x2893(%rip)        # 0x180009100
+   18000686d:	lea    0x10(%r15),%rcx
+   180006871:	lea    0x1c0(%rbp),%rdx
+   180006878:	call   0x18000720c
+   18000687d:	mov    0x1f0(%rbp),%rcx
+   180006884:	test   %rcx,%rcx
+   180006887:	je     0x1800068db
+   180006889:	mov    0x200(%rbp),%rax
+   180006890:	sub    %rcx,%rax
+   180006893:	sar    $0x2,%rax
+   180006897:	lea    0x0(,%rax,4),%rdx
+   18000689f:	mov    %rcx,%rax
+   1800068a2:	cmp    $0x1000,%rdx
+   1800068a9:	jb     0x1800068c4
+   1800068ab:	add    $0x27,%rdx
+   1800068af:	mov    -0x8(%rcx),%rcx
+   1800068b3:	sub    %rcx,%rax
+   1800068b6:	add    $0xfffffffffffffff8,%rax
+   1800068ba:	cmp    $0x1f,%rax
+   1800068be:	ja     0x180006978
+   1800068c4:	call   0x1800073b8
+   1800068c9:	mov    %rdi,0x1f0(%rbp)
+   1800068d0:	xorps  %xmm0,%xmm0
+   1800068d3:	movdqu %xmm0,0x1f8(%rbp)
+   1800068db:	mov    0x1d8(%rbp),%rcx
+   1800068e2:	test   %rcx,%rcx
+   1800068e5:	je     0x180006935
+   1800068e7:	mov    0x1e8(%rbp),%rax
+   1800068ee:	sub    %rcx,%rax
+   1800068f1:	sar    $0x2,%rax
+   1800068f5:	lea    0x0(,%rax,4),%rdx
+   1800068fd:	mov    %rcx,%rax
+   180006900:	cmp    $0x1000,%rdx
+   180006907:	jb     0x18000691e
+   180006909:	add    $0x27,%rdx
+   18000690d:	mov    -0x8(%rcx),%rcx
+   180006911:	sub    %rcx,%rax
+   180006914:	add    $0xfffffffffffffff8,%rax
+   180006918:	cmp    $0x1f,%rax
+   18000691c:	ja     0x180006978
+   18000691e:	call   0x1800073b8
+   180006923:	mov    %rdi,0x1d8(%rbp)
+   18000692a:	xorps  %xmm0,%xmm0
+   18000692d:	movdqu %xmm0,0x1e0(%rbp)
+   180006935:	mov    0x1c0(%rbp),%rcx
+   18000693c:	test   %rcx,%rcx
+   18000693f:	je     0x180006984
+   180006941:	mov    0x1d0(%rbp),%rax
+   180006948:	sub    %rcx,%rax
+   18000694b:	sar    $0x2,%rax
+   18000694f:	lea    0x0(,%rax,4),%rdx
+   180006957:	mov    %rcx,%rax
+   18000695a:	cmp    $0x1000,%rdx
+   180006961:	jb     0x18000697f
+   180006963:	add    $0x27,%rdx
+   180006967:	mov    -0x8(%rcx),%rcx
+   18000696b:	sub    %rcx,%rax
+   18000696e:	add    $0xfffffffffffffff8,%rax
+   180006972:	cmp    $0x1f,%rax
+   180006976:	jbe    0x18000697f
+   180006978:	call   *0x2a3a(%rip)        # 0x1800093b8
+   18000697e:	int3
+   18000697f:	call   0x1800073b8
+   180006984:	mov    (%r15),%rcx
+   180006987:	call   *0x28e3(%rip)        # 0x180009270
+   18000698d:	lea    0x1d0(%rbp),%rdx
+   180006994:	mov    %eax,%ecx
+   180006996:	call   0x18000723c
+   18000699b:	lea    0x1c0(%rbp),%rcx
+   1800069a2:	sub    %rcx,%r13
+   1800069a5:	add    %r13,%rax
+   1800069a8:	lea    0x1d0(%rbp),%rcx
+   1800069af:	mov    %rcx,0x1c0(%rbp)
+   1800069b6:	mov    %rax,0x1c8(%rbp)
+   1800069bd:	mov    %rsi,0x2d0(%rbp)
+   1800069c4:	mov    %rsi,%rax
+   1800069c7:	inc    %rax
+   1800069ca:	cmpb   $0x0,(%rax)
+   1800069cd:	jne    0x1800069c7
+   1800069cf:	sub    %rsi,%rax
+   1800069d2:	mov    %rax,0x2d8(%rbp)
+   1800069d9:	lea    0x2e20(%rip),%rcx        # 0x180009800
+   1800069e0:	mov    %rcx,0x160(%rbp)
+   1800069e7:	mov    %rcx,%rax
+   1800069ea:	nopw   0x0(%rax,%rax,1)
+   1800069f0:	inc    %rax
+   1800069f3:	cmpb   $0x0,(%rax)
+   1800069f6:	jne    0x1800069f0
+   1800069f8:	sub    %rcx,%rax
+   1800069fb:	mov    %rax,0x168(%rbp)
+   180006a02:	lea    0x1c0(%rbp),%r9
+   180006a09:	lea    0x2d0(%rbp),%r8
+   180006a10:	lea    0x160(%rbp),%rdx
+   180006a17:	lea    0x2b0(%rbp),%rcx
+   180006a1e:	call   0x180007242
+   180006a23:	nop
+   180006a24:	mov    %rax,%rcx
+   180006a27:	call   *0x27db(%rip)        # 0x180009208
+   180006a2d:	nop
+   180006a2e:	mov    0x2c8(%rbp),%rdx
+   180006a35:	cmp    $0x10,%rdx
+   180006a39:	jb     0x180006a72
+   180006a3b:	inc    %rdx
+   180006a3e:	mov    0x2b0(%rbp),%rcx
+   180006a45:	mov    %rcx,%rax
+   180006a48:	cmp    $0x1000,%rdx
+   180006a4f:	jb     0x180006a6d
+   180006a51:	add    $0x27,%rdx
+   180006a55:	mov    -0x8(%rcx),%rcx
+   180006a59:	sub    %rcx,%rax
+   180006a5c:	add    $0xfffffffffffffff8,%rax
+   180006a60:	cmp    $0x1f,%rax
+   180006a64:	jbe    0x180006a6d
+   180006a66:	call   *0x294c(%rip)        # 0x1800093b8
+   180006a6c:	int3
+   180006a6d:	call   0x1800073b8
+   180006a72:	mov    (%r15),%rcx
+   180006a75:	call   *0x2835(%rip)        # 0x1800092b0
+   180006a7b:	lea    0x2bee(%rip),%rcx        # 0x180009670
+   180006a82:	mov    %rcx,0x140(%rbp)
+   180006a89:	mov    %rcx,%rax
+   180006a8c:	cmpb   $0x0,0x2bdd(%rip)        # 0x180009670
+   180006a93:	je     0x180006a9d
+   180006a95:	inc    %rax
+   180006a98:	cmpb   $0x0,(%rax)
+   180006a9b:	jne    0x180006a95
+   180006a9d:	sub    %rcx,%rax
+   180006aa0:	mov    %rax,0x148(%rbp)
+   180006aa7:	movaps 0x140(%rbp),%xmm0
+   180006aae:	movdqa %xmm0,0x140(%rbp)
+   180006ab6:	mov    (%r15),%rcx
+   180006ab9:	call   *0x27c9(%rip)        # 0x180009288
+   180006abf:	mov    %rax,%rcx
+   180006ac2:	lea    0x140(%rbp),%rdx
+   180006ac9:	call   *0x2731(%rip)        # 0x180009200
+   180006acf:	lea    0x2d42(%rip),%rcx        # 0x180009818
+   180006ad6:	mov    %rcx,0x140(%rbp)
+   180006add:	mov    %rcx,%rax
+   180006ae0:	inc    %rax
+   180006ae3:	cmpb   $0x0,(%rax)
+   180006ae6:	jne    0x180006ae0
+   180006ae8:	sub    %rcx,%rax
+   180006aeb:	mov    %rax,0x148(%rbp)
+   180006af2:	movaps 0x140(%rbp),%xmm0
+   180006af9:	movdqa %xmm0,0x140(%rbp)
+   180006b01:	lea    0x140(%rbp),%rdx
+   180006b08:	mov    (%r15),%rcx
+   180006b0b:	call   0x180007224
+   180006b10:	nop
+   180006b11:	mov    0x60(%rsp),%rax
+   180006b16:	movslq 0x4(%rax),%rcx
+   180006b1a:	lea    0x2be7(%rip),%rax        # 0x180009708
+   180006b21:	mov    %rax,0x60(%rsp,%rcx,1)
+   180006b26:	mov    0x60(%rsp),%rax
+   180006b2b:	movslq 0x4(%rax),%rcx
+   180006b2f:	lea    -0xb8(%rcx),%edx
+   180006b35:	mov    %edx,0x5c(%rsp,%rcx,1)
+   180006b39:	lea    0x78(%rsp),%rcx
+   180006b3e:	call   0x180002d00
+   180006b43:	lea    -0x80(%rbp),%rcx
+   180006b47:	call   *0x257b(%rip)        # 0x1800090c8
+   180006b4d:	lea    0x18(%rbp),%rcx
+   180006b51:	call   *0x25b9(%rip)        # 0x180009110
+   180006b57:	mov    0x300(%rbp),%rcx
+   180006b5e:	xor    %rsp,%rcx
+   180006b61:	call   0x180007500
+   180006b66:	lea    0x490(%rsp),%r11
+   180006b6e:	mov    0x38(%r11),%rbx
+   180006b72:	mov    0x40(%r11),%rsi
+   180006b76:	mov    0x48(%r11),%rdi
+   180006b7a:	movaps -0x10(%r11),%xmm6
+   180006b7f:	movaps -0x20(%r11),%xmm7
+   180006b84:	movaps -0x30(%r11),%xmm8
+   180006b89:	movaps -0x40(%r11),%xmm9
+   180006b8e:	movaps -0x50(%r11),%xmm10
+   180006b93:	movaps -0x60(%r11),%xmm11
+   180006b98:	movaps -0x70(%r11),%xmm12
+   180006b9d:	movaps -0x80(%r11),%xmm13
+   180006ba2:	mov    %r11,%rsp
+   180006ba5:	pop    %r15
+   180006ba7:	pop    %r14
+   180006ba9:	pop    %r13
+   180006bab:	pop    %r12
+   180006bad:	pop    %rbp
+   180006bae:	ret
+   180006baf:	int3
+   180006bb0:	rex push %rbx
+   180006bb2:	sub    $0x20,%rsp
+   180006bb6:	cmpq   $0x0,0x80(%rcx)
+   180006bbe:	mov    %rcx,%rbx
+   180006bc1:	je     0x180006bf0
+   180006bc3:	mov    (%rcx),%r8
+   180006bc6:	mov    $0xffffffff,%edx
+   180006bcb:	call   *0x18(%r8)
+   180006bcf:	cmp    $0xffffffff,%eax
+   180006bd2:	je     0x180006bf0
+   180006bd4:	mov    0x80(%rbx),%rcx
+   180006bdb:	call   *0x2867(%rip)        # 0x180009448
+   180006be1:	test   %eax,%eax
+   180006be3:	jns    0x180006bf0
+   180006be5:	mov    $0xffffffff,%eax
+   180006bea:	add    $0x20,%rsp
+   180006bee:	pop    %rbx
+   180006bef:	ret
+   180006bf0:	xor    %eax,%eax
+   180006bf2:	add    $0x20,%rsp
+   180006bf6:	pop    %rbx
+   180006bf7:	ret
+   180006bf8:	int3
+   180006bf9:	int3
+   180006bfa:	int3
+   180006bfb:	int3
+   180006bfc:	int3
+   180006bfd:	int3
+   180006bfe:	int3
+   180006bff:	int3
+   180006c00:	rex push %rbx
+   180006c02:	sub    $0x20,%rsp
+   180006c06:	mov    %rdx,%rbx
+   180006c09:	lea    0x7628(%rip),%rcx        # 0x18000e238
+   180006c10:	lea    0x7a39(%rip),%rdx        # 0x18000e650
+   180006c17:	call   0x18000828e
+   180006c1c:	mov    %rax,(%rbx)
+   180006c1f:	test   %rax,%rax
+   180006c22:	je     0x180006c48
+   180006c24:	cmpb   $0x0,(%rax)
+   180006c27:	mov    %rax,%rcx
+   180006c2a:	je     0x180006c38
+   180006c2c:	nopl   0x0(%rax)
+   180006c30:	inc    %rcx
+   180006c33:	cmpb   $0x0,(%rcx)
+   180006c36:	jne    0x180006c30
+   180006c38:	sub    %rax,%rcx
+   180006c3b:	mov    %rbx,%rax
+   180006c3e:	mov    %rcx,0x8(%rbx)
+   180006c42:	add    $0x20,%rsp
+   180006c46:	pop    %rbx
+   180006c47:	ret
+   180006c48:	movq   $0x0,0x8(%rbx)
+   180006c50:	mov    %rbx,%rax
+   180006c53:	add    $0x20,%rsp
+   180006c57:	pop    %rbx
+   180006c58:	ret
+   180006c59:	int3
+   180006c5a:	int3
+   180006c5b:	int3
+   180006c5c:	int3
+   180006c5d:	int3
+   180006c5e:	int3
+   180006c5f:	int3
+   180006c60:	mov    %rbx,0x10(%rsp)
+   180006c65:	mov    %rdi,0x18(%rsp)
+   180006c6a:	push   %rbp
+   180006c6b:	mov    %rsp,%rbp
+   180006c6e:	sub    $0x80,%rsp
+   180006c75:	mov    0x738c(%rip),%rax        # 0x18000e008
+   180006c7c:	xor    %rsp,%rax
+   180006c7f:	mov    %rax,-0x8(%rbp)
+   180006c83:	mov    %rcx,%rdi
+   180006c86:	mov    0x38(%rcx),%rax
+   180006c8a:	mov    (%rax),%rcx
+   180006c8d:	test   %rcx,%rcx
+   180006c90:	je     0x180006cbe
+   180006c92:	mov    0x50(%rdi),%rdx
+   180006c96:	movslq (%rdx),%r8
+   180006c99:	lea    (%rcx,%r8,1),%rax
+   180006c9d:	cmp    %rax,%rcx
+   180006ca0:	jae    0x180006cbe
+   180006ca2:	lea    -0x1(%r8),%eax
+   180006ca6:	mov    %eax,(%rdx)
+   180006ca8:	mov    0x38(%rdi),%rcx
+   180006cac:	mov    (%rcx),%rdx
+   180006caf:	lea    0x1(%rdx),%rax
+   180006cb3:	mov    %rax,(%rcx)
+   180006cb6:	movzbl (%rdx),%eax
+   180006cb9:	jmp    0x180006eea
+   180006cbe:	cmpq   $0x0,0x80(%rdi)
+   180006cc6:	jne    0x180006cd2
+   180006cc8:	mov    $0xffffffff,%eax
+   180006ccd:	jmp    0x180006eea
+   180006cd2:	mov    0x18(%rdi),%r8
+   180006cd6:	lea    0x70(%rdi),%rax
+   180006cda:	cmp    %rax,(%r8)
+   180006cdd:	jne    0x180006cff
+   180006cdf:	mov    0x90(%rdi),%rdx
+   180006ce6:	mov    0x88(%rdi),%rcx
+   180006ced:	mov    %rcx,(%r8)
+   180006cf0:	mov    0x38(%rdi),%rax
+   180006cf4:	mov    %rcx,(%rax)
+   180006cf7:	sub    %ecx,%edx
+   180006cf9:	mov    0x50(%rdi),%rax
+   180006cfd:	mov    %edx,(%rax)
+   180006cff:	mov    0x80(%rdi),%rcx
+   180006d06:	cmpq   $0x0,0x68(%rdi)
+   180006d0b:	jne    0x180006d29
+   180006d0d:	call   *0x272d(%rip)        # 0x180009440
+   180006d13:	cmp    $0xffffffff,%eax
+   180006d16:	mov    $0xffffffff,%ebx
+   180006d1b:	je     0x180006ee8
+   180006d21:	movzbl %al,%ebx
+   180006d24:	jmp    0x180006ee8
+   180006d29:	xor    %eax,%eax
+   180006d2b:	mov    %rax,-0x28(%rbp)
+   180006d2f:	mov    %rax,-0x18(%rbp)
+   180006d33:	movq   $0xf,-0x10(%rbp)
+   180006d3b:	mov    %al,-0x28(%rbp)
+   180006d3e:	call   *0x26fc(%rip)        # 0x180009440
+   180006d44:	cmp    $0xffffffff,%eax
+   180006d47:	mov    %eax,%r8d
+   180006d4a:	je     0x180006ea5
+   180006d50:	mov    -0x18(%rbp),%rcx
+   180006d54:	mov    -0x10(%rbp),%rdx
+   180006d58:	cmp    %rdx,%rcx
+   180006d5b:	jae    0x180006d7d
+   180006d5d:	lea    0x1(%rcx),%rax
+   180006d61:	mov    %rax,-0x18(%rbp)
+   180006d65:	lea    -0x28(%rbp),%rax
+   180006d69:	cmp    $0x10,%rdx
+   180006d6d:	cmovae -0x28(%rbp),%rax
+   180006d72:	mov    %r8b,(%rax,%rcx,1)
+   180006d76:	movb   $0x0,0x1(%rax,%rcx,1)
+   180006d7b:	jmp    0x180006d91
+   180006d7d:	movzbl %r8b,%r9d
+   180006d81:	xor    %r8d,%r8d
+   180006d84:	lea    0x1(%r8),%edx
+   180006d88:	lea    -0x28(%rbp),%rcx
+   180006d8c:	call   0x180001ad0
+   180006d91:	lea    -0x28(%rbp),%rdx
+   180006d95:	cmpq   $0x10,-0x10(%rbp)
+   180006d9a:	cmovae -0x28(%rbp),%rdx
+   180006d9f:	lea    -0x28(%rbp),%r8
+   180006da3:	cmovae -0x28(%rbp),%r8
+   180006da8:	mov    -0x18(%rbp),%r9
+   180006dac:	add    %rdx,%r9
+   180006daf:	lea    -0x30(%rbp),%rax
+   180006db3:	mov    %rax,0x38(%rsp)
+   180006db8:	lea    -0x3f(%rbp),%rax
+   180006dbc:	mov    %rax,0x30(%rsp)
+   180006dc1:	lea    -0x40(%rbp),%rax
+   180006dc5:	mov    %rax,0x28(%rsp)
+   180006dca:	lea    -0x38(%rbp),%rax
+   180006dce:	mov    %rax,0x20(%rsp)
+   180006dd3:	lea    0x74(%rdi),%rdx
+   180006dd7:	mov    0x68(%rdi),%rcx
+   180006ddb:	call   *0x2397(%rip)        # 0x180009178
+   180006de1:	test   %eax,%eax
+   180006de3:	je     0x180006dea
+   180006de5:	sub    $0x1,%eax
+   180006de8:	jne    0x180006e41
+   180006dea:	lea    -0x40(%rbp),%rax
+   180006dee:	cmp    %rax,-0x30(%rbp)
+   180006df2:	lea    -0x28(%rbp),%rax
+   180006df6:	jne    0x180006e59
+   180006df8:	cmpq   $0x10,-0x10(%rbp)
+   180006dfd:	cmovae -0x28(%rbp),%rax
+   180006e02:	mov    -0x38(%rbp),%r10
+   180006e06:	sub    %rax,%r10
+   180006e09:	mov    -0x18(%rbp),%r8
+   180006e0d:	cmp    %r10,%r8
+   180006e10:	cmovb  %r8,%r10
+   180006e14:	lea    -0x28(%rbp),%rcx
+   180006e18:	cmpq   $0x10,-0x10(%rbp)
+   180006e1d:	cmovae -0x28(%rbp),%rcx
+   180006e22:	sub    %r10,%r8
+   180006e25:	mov    %r8,-0x18(%rbp)
+   180006e29:	inc    %r8
+   180006e2c:	lea    (%rcx,%r10,1),%rdx
+   180006e30:	call   0x1800082a0
+   180006e35:	mov    0x80(%rdi),%rcx
+   180006e3c:	jmp    0x180006d3e
+   180006e41:	cmp    $0x2,%eax
+   180006e44:	jne    0x180006ea5
+   180006e46:	lea    -0x28(%rbp),%rax
+   180006e4a:	cmpq   $0x10,-0x10(%rbp)
+   180006e4f:	cmovae -0x28(%rbp),%rax
+   180006e54:	movsbl (%rax),%ebx
+   180006e57:	jmp    0x180006eaa
+   180006e59:	cmpq   $0x10,-0x10(%rbp)
+   180006e5e:	cmovae -0x28(%rbp),%rax
+   180006e63:	mov    -0x18(%rbp),%rbx
+   180006e67:	mov    -0x38(%rbp),%rcx
+   180006e6b:	sub    %rcx,%rbx
+   180006e6e:	add    %rax,%rbx
+   180006e71:	test   %rbx,%rbx
+   180006e74:	jle    0x180006e9f
+   180006e76:	data16 nopw 0x0(%rax,%rax,1)
+   180006e80:	dec    %rbx
+   180006e83:	movsbl (%rbx,%rcx,1),%ecx
+   180006e87:	mov    0x80(%rdi),%rdx
+   180006e8e:	call   *0x259c(%rip)        # 0x180009430
+   180006e94:	test   %rbx,%rbx
+   180006e97:	jle    0x180006e9f
+   180006e99:	mov    -0x38(%rbp),%rcx
+   180006e9d:	jmp    0x180006e80
+   180006e9f:	movzbl -0x40(%rbp),%ebx
+   180006ea3:	jmp    0x180006eaa
+   180006ea5:	mov    $0xffffffff,%ebx
+   180006eaa:	mov    -0x10(%rbp),%rdx
+   180006eae:	cmp    $0x10,%rdx
+   180006eb2:	jb     0x180006ee8
+   180006eb4:	inc    %rdx
+   180006eb7:	mov    -0x28(%rbp),%rcx
+   180006ebb:	mov    %rcx,%rax
+   180006ebe:	cmp    $0x1000,%rdx
+   180006ec5:	jb     0x180006ee3
+   180006ec7:	add    $0x27,%rdx
+   180006ecb:	mov    -0x8(%rcx),%rcx
+   180006ecf:	sub    %rcx,%rax
+   180006ed2:	add    $0xfffffffffffffff8,%rax
+   180006ed6:	cmp    $0x1f,%rax
+   180006eda:	jbe    0x180006ee3
+   180006edc:	call   *0x24d6(%rip)        # 0x1800093b8
+   180006ee2:	int3
+   180006ee3:	call   0x1800073b8
+   180006ee8:	mov    %ebx,%eax
+   180006eea:	mov    -0x8(%rbp),%rcx
+   180006eee:	xor    %rsp,%rcx
+   180006ef1:	call   0x180007500
+   180006ef6:	lea    0x80(%rsp),%r11
+   180006efe:	mov    0x18(%r11),%rbx
+   180006f02:	mov    0x20(%r11),%rdi
+   180006f06:	mov    %r11,%rsp
+   180006f09:	pop    %rbp
+   180006f0a:	ret
+   180006f0b:	int3
+   180006f0c:	int3
+   180006f0d:	int3
+   180006f0e:	int3
+   180006f0f:	int3
+   180006f10:	rex push %rbx
+   180006f12:	sub    $0x20,%rsp
+   180006f16:	mov    0x38(%rcx),%rax
+   180006f1a:	mov    %rcx,%rbx
+   180006f1d:	mov    (%rax),%rcx
+   180006f20:	test   %rcx,%rcx
+   180006f23:	je     0x180006f3d
+   180006f25:	mov    0x50(%rbx),%rax
+   180006f29:	movslq (%rax),%rdx
+   180006f2c:	add    %rcx,%rdx
+   180006f2f:	cmp    %rdx,%rcx
+   180006f32:	jae    0x180006f3d
+   180006f34:	movzbl (%rcx),%eax
+   180006f37:	add    $0x20,%rsp
+   180006f3b:	pop    %rbx
+   180006f3c:	ret
+   180006f3d:	mov    (%rbx),%rax
+   180006f40:	mov    %rbx,%rcx
+   180006f43:	mov    %rdi,0x30(%rsp)
+   180006f48:	call   *0x38(%rax)
+   180006f4b:	mov    %eax,%edi
+   180006f4d:	cmp    $0xffffffff,%eax
+   180006f50:	jne    0x180006f5d
+   180006f52:	mov    0x30(%rsp),%rdi
+   180006f57:	add    $0x20,%rsp
+   180006f5b:	pop    %rbx
+   180006f5c:	ret
+   180006f5d:	mov    (%rbx),%rax
+   180006f60:	mov    %edi,%edx
+   180006f62:	mov    %rbx,%rcx
+   180006f65:	call   *0x20(%rax)
+   180006f68:	mov    %edi,%eax
+   180006f6a:	mov    0x30(%rsp),%rdi
+   180006f6f:	add    $0x20,%rsp
+   180006f73:	pop    %rbx
+   180006f74:	ret
+   180006f75:	int3
+   180006f76:	int3
+   180006f77:	int3
+   180006f78:	int3
+   180006f79:	int3
+   180006f7a:	int3
+   180006f7b:	int3
+   180006f7c:	int3
+   180006f7d:	int3
+   180006f7e:	int3
+   180006f7f:	int3
+   180006f80:	mov    %edx,%eax
+   180006f82:	lea    (%rax,%rax,4),%rdx
+   180006f86:	mov    0x58(%rcx),%rax
+   180006f8a:	lea    (%rax,%rdx,8),%rax
+   180006f8e:	ret
+   180006f8f:	int3
+   180006f90:	mov    0x8(%rcx),%rdx
+   180006f94:	lea    0x259d(%rip),%rax        # 0x180009538
+   180006f9b:	test   %rdx,%rdx
+   180006f9e:	cmovne %rdx,%rax
+   180006fa2:	ret
+   180006fa3:	int3
+   180006fa4:	int3
+   180006fa5:	int3
+   180006fa6:	int3
+   180006fa7:	int3
+   180006fa8:	int3
+   180006fa9:	int3
+   180006faa:	int3
+   180006fab:	int3
+   180006fac:	int3
+   180006fad:	int3
+   180006fae:	int3
+   180006faf:	int3
+   180006fb0:	mov    %rbp,0x18(%rsp)
+   180006fb5:	mov    %rsi,0x20(%rsp)
+   180006fba:	push   %r14
+   180006fbc:	sub    $0x20,%rsp
+   180006fc0:	mov    %r8,%rbp
+   180006fc3:	mov    %rdx,%r14
+   180006fc6:	mov    %rcx,%rsi
+   180006fc9:	test   %r8,%r8
+   180006fcc:	jg     0x180006fe1
+   180006fce:	xor    %eax,%eax
+   180006fd0:	mov    0x40(%rsp),%rbp
+   180006fd5:	mov    0x48(%rsp),%rsi
+   180006fda:	add    $0x20,%rsp
+   180006fde:	pop    %r14
+   180006fe0:	ret
+   180006fe1:	cmpq   $0x0,0x68(%rcx)
+   180006fe6:	je     0x180006fff
+   180006fe8:	mov    0x40(%rsp),%rbp
+   180006fed:	mov    0x48(%rsp),%rsi
+   180006ff2:	add    $0x20,%rsp
+   180006ff6:	pop    %r14
+   180006ff8:	rex.W jmp *0x2121(%rip)        # 0x180009120
+   180006fff:	mov    0x38(%rcx),%rax
+   180007003:	mov    %rbx,0x30(%rsp)
+   180007008:	mov    %rdi,0x38(%rsp)
+   18000700d:	mov    %rbp,%rdi
+   180007010:	mov    (%rax),%rdx
+   180007013:	test   %rdx,%rdx
+   180007016:	je     0x180007020
+   180007018:	mov    0x50(%rcx),%rax
+   18000701c:	mov    (%rax),%ecx
+   18000701e:	jmp    0x180007022
+   180007020:	xor    %ecx,%ecx
+   180007022:	movslq %ecx,%rax
+   180007025:	test   %ecx,%ecx
+   180007027:	je     0x180007054
+   180007029:	cmp    %rbp,%rax
+   18000702c:	mov    %rbp,%rbx
+   18000702f:	mov    %r14,%rcx
+   180007032:	cmovb  %rax,%rbx
+   180007036:	mov    %rbx,%r8
+   180007039:	call   0x18000829a
+   18000703e:	mov    0x50(%rsi),%rax
+   180007042:	add    %rbx,%r14
+   180007045:	sub    %rbx,%rdi
+   180007048:	sub    %ebx,(%rax)
+   18000704a:	mov    0x38(%rsi),%rcx
+   18000704e:	movslq %ebx,%rax
+   180007051:	add    %rax,(%rcx)
+   180007054:	cmpq   $0x0,0x80(%rsi)
+   18000705c:	mov    %rdi,%rbx
+   18000705f:	je     0x1800070f1
+   180007065:	mov    0x18(%rsi),%r8
+   180007069:	lea    0x70(%rsi),%rax
+   18000706d:	cmp    %rax,(%r8)
+   180007070:	jne    0x180007092
+   180007072:	mov    0x88(%rsi),%rcx
+   180007079:	mov    0x90(%rsi),%rdx
+   180007080:	mov    %rcx,(%r8)
+   180007083:	sub    %ecx,%edx
+   180007085:	mov    0x38(%rsi),%rax
+   180007089:	mov    %rcx,(%rax)
+   18000708c:	mov    0x50(%rsi),%rax
+   180007090:	mov    %edx,(%rax)
+   180007092:	cmp    $0xfff,%rdi
+   180007099:	jbe    0x1800070d1
+   18000709b:	nopl   0x0(%rax,%rax,1)
+   1800070a0:	mov    0x80(%rsi),%r9
+   1800070a7:	mov    $0x1,%edx
+   1800070ac:	mov    $0xfff,%r8d
+   1800070b2:	mov    %r14,%rcx
+   1800070b5:	call   *0x236d(%rip)        # 0x180009428
+   1800070bb:	sub    %rax,%rdi
+   1800070be:	add    %rax,%r14
+   1800070c1:	mov    %rdi,%rbx
+   1800070c4:	cmp    $0xfff,%rax
+   1800070ca:	jne    0x180007112
+   1800070cc:	cmp    %rax,%rdi
+   1800070cf:	ja     0x1800070a0
+   1800070d1:	test   %rbx,%rbx
+   1800070d4:	je     0x1800070f1
+   1800070d6:	mov    0x80(%rsi),%r9
+   1800070dd:	mov    %rdi,%r8
+   1800070e0:	mov    $0x1,%edx
+   1800070e5:	mov    %r14,%rcx
+   1800070e8:	call   *0x233a(%rip)        # 0x180009428
+   1800070ee:	sub    %rax,%rbx
+   1800070f1:	sub    %rbx,%rbp
+   1800070f4:	mov    0x30(%rsp),%rbx
+   1800070f9:	mov    %rbp,%rax
+   1800070fc:	mov    0x40(%rsp),%rbp
+   180007101:	mov    0x38(%rsp),%rdi
+   180007106:	mov    0x48(%rsp),%rsi
+   18000710b:	add    $0x20,%rsp
+   18000710f:	pop    %r14
+   180007111:	ret
+   180007112:	sub    %rdi,%rbp
+   180007115:	jmp    0x1800070f4
+   180007117:	int3
+   180007118:	int3
+   180007119:	int3
+   18000711a:	int3
+   18000711b:	int3
+   18000711c:	int3
+   18000711d:	int3
+   18000711e:	int3
+   18000711f:	int3
+   180007120:	mov    %rbx,0x18(%rsp)
+   180007125:	mov    %rdi,0x20(%rsp)
+   18000712a:	push   %r14
+   18000712c:	sub    $0x20,%rsp
+   180007130:	cmpq   $0x0,0x68(%rcx)
+   180007135:	mov    %r8,%rbx
+   180007138:	mov    %rdx,%r14
+   18000713b:	mov    %rcx,%rdi
+   18000713e:	je     0x180007157
+   180007140:	mov    0x40(%rsp),%rbx
+   180007145:	mov    0x48(%rsp),%rdi
+   18000714a:	add    $0x20,%rsp
+   18000714e:	pop    %r14
+   180007150:	rex.W jmp *0x1fc1(%rip)        # 0x180009118
+   180007157:	mov    0x40(%rcx),%rax
+   18000715b:	mov    %rbp,0x30(%rsp)
+   180007160:	mov    %rsi,0x38(%rsp)
+   180007165:	mov    %rbx,%rsi
+   180007168:	mov    (%rax),%r9
+   18000716b:	test   %r9,%r9
+   18000716e:	je     0x180007178
+   180007170:	mov    0x58(%rcx),%rax
+   180007174:	mov    (%rax),%ecx
+   180007176:	jmp    0x18000717a
+   180007178:	xor    %ecx,%ecx
+   18000717a:	movslq %ecx,%rbp
+   18000717d:	test   %rbx,%rbx
+   180007180:	jle    0x1800071d3
+   180007182:	test   %ecx,%ecx
+   180007184:	jle    0x1800071b3
+   180007186:	cmp    %rbp,%rbx
+   180007189:	mov    %r9,%rcx
+   18000718c:	cmovl  %rbx,%rbp
+   180007190:	mov    %rbp,%r8
+   180007193:	call   0x18000829a
+   180007198:	mov    0x58(%rdi),%rax
+   18000719c:	sub    %rbp,%rbx
+   18000719f:	add    %rbp,%r14
+   1800071a2:	sub    %ebp,(%rax)
+   1800071a4:	mov    0x40(%rdi),%rcx
+   1800071a8:	movslq %ebp,%rax
+   1800071ab:	add    %rax,(%rcx)
+   1800071ae:	test   %rbx,%rbx
+   1800071b1:	jle    0x1800071d3
+   1800071b3:	mov    0x80(%rdi),%r9
+   1800071ba:	test   %r9,%r9
+   1800071bd:	je     0x1800071d3
+   1800071bf:	mov    %rbx,%r8
+   1800071c2:	mov    $0x1,%edx
+   1800071c7:	mov    %r14,%rcx
+   1800071ca:	call   *0x2240(%rip)        # 0x180009410
+   1800071d0:	sub    %rax,%rbx
+   1800071d3:	mov    0x30(%rsp),%rbp
+   1800071d8:	sub    %rbx,%rsi
+   1800071db:	mov    0x40(%rsp),%rbx
+   1800071e0:	mov    %rsi,%rax
+   1800071e3:	mov    0x38(%rsp),%rsi
+   1800071e8:	mov    0x48(%rsp),%rdi
+   1800071ed:	add    $0x20,%rsp
+   1800071f1:	pop    %r14
+   1800071f3:	ret
+   1800071f4:	jmp    *0x1e06(%rip)        # 0x180009000
+   1800071fa:	jmp    *0x1e08(%rip)        # 0x180009008
+   180007200:	jmp    *0x1e0a(%rip)        # 0x180009010
+   180007206:	jmp    *0x1e0c(%rip)        # 0x180009018
+   18000720c:	jmp    *0x1e0e(%rip)        # 0x180009020
+   180007212:	jmp    *0x1e10(%rip)        # 0x180009028
+   180007218:	jmp    *0x2062(%rip)        # 0x180009280
+   18000721e:	jmp    *0x2084(%rip)        # 0x1800092a8
+   180007224:	jmp    *0x202e(%rip)        # 0x180009258
+   18000722a:	jmp    *0x2010(%rip)        # 0x180009240
+   180007230:	jmp    *0x1ffa(%rip)        # 0x180009230
+   180007236:	jmp    *0x1fec(%rip)        # 0x180009228
+   18000723c:	jmp    *0x2106(%rip)        # 0x180009348
+   180007242:	jmp    *0x20f8(%rip)        # 0x180009340
+   180007248:	jmp    *0x1efa(%rip)        # 0x180009148
+   18000724e:	jmp    *0x1efc(%rip)        # 0x180009150
+   180007254:	jmp    *0x1efe(%rip)        # 0x180009158
+   18000725a:	int3
+   18000725b:	int3
+   18000725c:	rex push %rbx
+   18000725e:	sub    $0x20,%rsp
+   180007262:	mov    %rcx,%rbx
+   180007265:	mov    $0x10,%ecx
+   18000726a:	call   0x18000737c
+   18000726f:	mov    %rax,0x38(%rsp)
+   180007274:	test   %rax,%rax
+   180007277:	je     0x180007287
+   180007279:	mov    0x73c0(%rip),%rdx        # 0x18000e640
+   180007280:	mov    %rdx,(%rax)
+   180007283:	mov    %rbx,0x8(%rax)
+   180007287:	mov    %rax,0x73b2(%rip)        # 0x18000e640
+   18000728e:	add    $0x20,%rsp
+   180007292:	pop    %rbx
+   180007293:	ret
+   180007294:	jmp    *0x1ece(%rip)        # 0x180009168
+   18000729a:	jmp    *0x1f00(%rip)        # 0x1800091a0
+   1800072a0:	jmp    *0x1e1a(%rip)        # 0x1800090c0
+   1800072a6:	jmp    *0x1e8c(%rip)        # 0x180009138
+   1800072ac:	mov    %rsp,%rax
+   1800072af:	mov    %r9,0x20(%rax)
+   1800072b3:	mov    %r8,0x18(%rax)
+   1800072b7:	mov    %rdx,0x10(%rax)
+   1800072bb:	push   %rbx
+   1800072bc:	push   %rsi
+   1800072bd:	push   %rdi
+   1800072be:	push   %r14
+   1800072c0:	sub    $0x38,%rsp
+   1800072c4:	mov    %r9,%r14
+   1800072c7:	mov    %r8,%rbx
+   1800072ca:	mov    %rdx,%rsi
+   1800072cd:	movb   $0x0,-0x38(%rax)
+   1800072d1:	mov    %rdx,%rdi
+   1800072d4:	imul   %r8,%rdi
+   1800072d8:	add    %rcx,%rdi
+   1800072db:	mov    %rdi,0x8(%rax)
+   1800072df:	mov    %rbx,%rax
+   1800072e2:	dec    %rbx
+   1800072e5:	mov    %rbx,0x70(%rsp)
+   1800072ea:	test   %rax,%rax
+   1800072ed:	je     0x180007308
+   1800072ef:	sub    %rsi,%rdi
+   1800072f2:	mov    %rdi,0x60(%rsp)
+   1800072f7:	mov    %rdi,%rcx
+   1800072fa:	mov    %r14,%rax
+   1800072fd:	mov    0x217c(%rip),%rdx        # 0x180009480
+   180007304:	call   *%rdx
+   180007306:	jmp    0x1800072df
+   180007308:	movb   $0x1,0x20(%rsp)
+   18000730d:	add    $0x38,%rsp
+   180007311:	pop    %r14
+   180007313:	pop    %rdi
+   180007314:	pop    %rsi
+   180007315:	pop    %rbx
+   180007316:	ret
+   180007317:	int3
+   180007318:	mov    %rbx,0x10(%rsp)
+   18000731d:	mov    %rsi,0x18(%rsp)
+   180007322:	mov    %rcx,0x8(%rsp)
+   180007327:	push   %rdi
+   180007328:	push   %r14
+   18000732a:	push   %r15
+   18000732c:	sub    $0x50,%rsp
+   180007330:	mov    %r9,%r14
+   180007333:	mov    %r8,%rsi
+   180007336:	mov    %rdx,%r15
+   180007339:	mov    %rcx,%rdi
+   18000733c:	xor    %ebx,%ebx
+   18000733e:	mov    %rbx,0x38(%rsp)
+   180007343:	cmp    %rsi,%rbx
+   180007346:	je     0x180007361
+   180007348:	sub    %r15,%rdi
+   18000734b:	mov    %rdi,0x70(%rsp)
+   180007350:	mov    %rdi,%rcx
+   180007353:	mov    %r14,%rax
+   180007356:	call   *0x2124(%rip)        # 0x180009480
+   18000735c:	inc    %rbx
+   18000735f:	jmp    0x18000733e
+   180007361:	jmp    0x180007363
+   180007363:	lea    0x50(%rsp),%r11
+   180007368:	mov    0x28(%r11),%rbx
+   18000736c:	mov    0x30(%r11),%rsi
+   180007370:	mov    %r11,%rsp
+   180007373:	pop    %r15
+   180007375:	pop    %r14
+   180007377:	pop    %rdi
+   180007378:	ret
+   180007379:	int3
+   18000737a:	int3
+   18000737b:	int3
+   18000737c:	rex push %rbx
+   18000737e:	sub    $0x20,%rsp
+   180007382:	mov    %rcx,%rbx
+   180007385:	jmp    0x180007396
+   180007387:	mov    %rbx,%rcx
+   18000738a:	call   0x1800082d0
+   18000738f:	test   %eax,%eax
+   180007391:	je     0x1800073a6
+   180007393:	mov    %rbx,%rcx
+   180007396:	call   0x1800082d6
+   18000739b:	test   %rax,%rax
+   18000739e:	je     0x180007387
+   1800073a0:	add    $0x20,%rsp
+   1800073a4:	pop    %rbx
+   1800073a5:	ret
+   1800073a6:	cmp    $0xffffffffffffffff,%rbx
+   1800073aa:	je     0x1800073b2
+   1800073ac:	call   0x180007c40
+   1800073b1:	int3
+   1800073b2:	call   0x1800038f0
+   1800073b7:	int3
+   1800073b8:	jmp    0x180007c60
+   1800073bd:	int3
+   1800073be:	int3
+   1800073bf:	int3
+   1800073c0:	jmp    0x1800073b8
+   1800073c5:	int3
+   1800073c6:	int3
+   1800073c7:	int3
+   1800073c8:	rex push %rbx
+   1800073ca:	sub    $0x20,%rsp
+   1800073ce:	lea    0x25f3(%rip),%rax        # 0x1800099c8
+   1800073d5:	mov    %rcx,%rbx
+   1800073d8:	mov    %rax,(%rcx)
+   1800073db:	test   $0x1,%dl
+   1800073de:	je     0x1800073ea
+   1800073e0:	mov    $0x18,%edx
+   1800073e5:	call   0x1800073b8
+   1800073ea:	mov    %rbx,%rax
+   1800073ed:	add    $0x20,%rsp
+   1800073f1:	pop    %rbx
+   1800073f2:	ret
+   1800073f3:	int3
+   1800073f4:	sub    $0x28,%rsp
+   1800073f8:	mov    0x38(%r9),%r8
+   1800073fc:	mov    %rdx,%rcx
+   1800073ff:	mov    %r9,%rdx
+   180007402:	call   0x180007414
+   180007407:	mov    $0x1,%eax
+   18000740c:	add    $0x28,%rsp
+   180007410:	ret
+   180007411:	int3
+   180007412:	int3
+   180007413:	int3
+   180007414:	rex push %rbx
+   180007416:	mov    (%r8),%r11d
+   180007419:	mov    %rdx,%rbx
+   18000741c:	and    $0xfffffff8,%r11d
+   180007420:	mov    %rcx,%r9
+   180007423:	testb  $0x4,(%r8)
+   180007427:	mov    %rcx,%r10
+   18000742a:	je     0x18000743f
+   18000742c:	mov    0x8(%r8),%eax
+   180007430:	movslq 0x4(%r8),%r10
+   180007434:	neg    %eax
+   180007436:	add    %rcx,%r10
+   180007439:	movslq %eax,%rcx
+   18000743c:	and    %rcx,%r10
+   18000743f:	movslq %r11d,%rax
+   180007442:	mov    (%rax,%r10,1),%rdx
+   180007446:	mov    0x10(%rbx),%rax
+   18000744a:	mov    0x8(%rax),%ecx
+   18000744d:	mov    0x8(%rbx),%rax
+   180007451:	testb  $0xf,0x3(%rcx,%rax,1)
+   180007456:	je     0x180007463
+   180007458:	movzbl 0x3(%rcx,%rax,1),%eax
+   18000745d:	and    $0xfffffff0,%eax
+   180007460:	add    %rax,%r9
+   180007463:	xor    %rdx,%r9
+   180007466:	mov    %r9,%rcx
+   180007469:	pop    %rbx
+   18000746a:	jmp    0x180007500
+   18000746f:	int3
+   180007470:	mov    %rsp,%rax
+   180007473:	mov    %rbx,0x8(%rax)
+   180007477:	mov    %rbp,0x10(%rax)
+   18000747b:	mov    %rsi,0x18(%rax)
+   18000747f:	mov    %rdi,0x20(%rax)
+   180007483:	push   %r14
+   180007485:	sub    $0x20,%rsp
+   180007489:	mov    0x38(%r9),%rbx
+   18000748d:	mov    %rdx,%rsi
+   180007490:	mov    %r8,%r14
+   180007493:	mov    %rcx,%rbp
+   180007496:	mov    %r9,%rdx
+   180007499:	mov    %rsi,%rcx
+   18000749c:	mov    %r9,%rdi
+   18000749f:	lea    0x4(%rbx),%r8
+   1800074a3:	call   0x180007414
+   1800074a8:	mov    0x4(%rbp),%eax
+   1800074ab:	and    $0x66,%al
+   1800074ad:	neg    %al
+   1800074af:	mov    $0x1,%eax
+   1800074b4:	sbb    %r8d,%r8d
+   1800074b7:	neg    %r8d
+   1800074ba:	add    %eax,%r8d
+   1800074bd:	test   %r8d,0x4(%rbx)
+   1800074c1:	je     0x1800074d4
+   1800074c3:	mov    %rdi,%r9
+   1800074c6:	mov    %r14,%r8
+   1800074c9:	mov    %rsi,%rdx
+   1800074cc:	mov    %rbp,%rcx
+   1800074cf:	call   0x180008270
+   1800074d4:	mov    0x30(%rsp),%rbx
+   1800074d9:	mov    0x38(%rsp),%rbp
+   1800074de:	mov    0x40(%rsp),%rsi
+   1800074e3:	mov    0x48(%rsp),%rdi
+   1800074e8:	add    $0x20,%rsp
+   1800074ec:	pop    %r14
+   1800074ee:	ret
+   1800074ef:	int3
+   1800074f0:	int3
+   1800074f1:	int3
+   1800074f2:	int3
+   1800074f3:	int3
+   1800074f4:	int3
+   1800074f5:	int3
+   1800074f6:	data16 nopw 0x0(%rax,%rax,1)
+   180007500:	cmp    0x6b01(%rip),%rcx        # 0x18000e008
+   180007507:	jne    0x180007519
+   180007509:	rol    $0x10,%rcx
+   18000750d:	test   $0xffff,%cx
+   180007512:	jne    0x180007515
+   180007514:	ret
+   180007515:	ror    $0x10,%rcx
+   180007519:	jmp    0x180007c9c
+   18000751e:	int3
+   18000751f:	int3
+   180007520:	lea    0x7129(%rip),%rcx        # 0x18000e650
+   180007527:	rex.W jmp *0x1b82(%rip)        # 0x1800090b0
+   18000752e:	int3
+   18000752f:	int3
+   180007530:	lea    0x7119(%rip),%rcx        # 0x18000e650
+   180007537:	jmp    0x1800082be
+   18000753c:	sub    $0x28,%rsp
+   180007540:	test   %edx,%edx
+   180007542:	je     0x18000757d
+   180007544:	sub    $0x1,%edx
+   180007547:	je     0x180007571
+   180007549:	sub    $0x1,%edx
+   18000754c:	je     0x180007564
+   18000754e:	cmp    $0x1,%edx
+   180007551:	je     0x18000755d
+   180007553:	mov    $0x1,%eax
+   180007558:	add    $0x28,%rsp
+   18000755c:	ret
+   18000755d:	call   0x18000794c
+   180007562:	jmp    0x180007569
+   180007564:	call   0x180007924
+   180007569:	movzbl %al,%eax
+   18000756c:	add    $0x28,%rsp
+   180007570:	ret
+   180007571:	mov    %r8,%rdx
+   180007574:	add    $0x28,%rsp
+   180007578:	jmp    0x18000758c
+   18000757d:	test   %r8,%r8
+   180007580:	setne  %cl
+   180007583:	add    $0x28,%rsp
+   180007587:	jmp    0x1800076a4
+   18000758c:	mov    %rbx,0x8(%rsp)
+   180007591:	mov    %rsi,0x10(%rsp)
+   180007596:	mov    %rdi,0x20(%rsp)
+   18000759b:	push   %r14
+   18000759d:	sub    $0x20,%rsp
+   1800075a1:	mov    %rdx,%rsi
+   1800075a4:	mov    %rcx,%r14
+   1800075a7:	xor    %ecx,%ecx
+   1800075a9:	call   0x180007a08
+   1800075ae:	test   %al,%al
+   1800075b0:	je     0x18000767e
+   1800075b6:	call   0x18000789c
+   1800075bb:	mov    %al,%bl
+   1800075bd:	mov    %al,0x40(%rsp)
+   1800075c1:	mov    $0x1,%dil
+   1800075c4:	cmpl   $0x0,0x709d(%rip)        # 0x18000e668
+   1800075cb:	jne    0x180007696
+   1800075d1:	movl   $0x1,0x708d(%rip)        # 0x18000e668
+   1800075db:	call   0x18000790c
+   1800075e0:	test   %al,%al
+   1800075e2:	je     0x180007633
+   1800075e4:	call   0x18000803c
+   1800075e9:	call   0x180007520
+   1800075ee:	call   0x180007ec4
+   1800075f3:	lea    0x1ebe(%rip),%rdx        # 0x1800094b8
+   1800075fa:	lea    0x1eaf(%rip),%rcx        # 0x1800094b0
+   180007601:	call   0x1800082e2
+   180007606:	test   %eax,%eax
+   180007608:	jne    0x180007633
+   18000760a:	call   0x1800078d8
+   18000760f:	test   %al,%al
+   180007611:	je     0x180007633
+   180007613:	lea    0x1e8e(%rip),%rdx        # 0x1800094a8
+   18000761a:	lea    0x1e77(%rip),%rcx        # 0x180009498
+   180007621:	call   0x1800082dc
+   180007626:	movl   $0x2,0x7038(%rip)        # 0x18000e668
+   180007630:	xor    %dil,%dil
+   180007633:	mov    %bl,%cl
+   180007635:	call   0x180007b78
+   18000763a:	test   %dil,%dil
+   18000763d:	jne    0x18000767e
+   18000763f:	call   0x180007ee0
+   180007644:	mov    %rax,%rbx
+   180007647:	cmpq   $0x0,(%rax)
+   18000764b:	je     0x180007671
+   18000764d:	mov    %rax,%rcx
+   180007650:	call   0x180007ae0
+   180007655:	test   %al,%al
+   180007657:	je     0x180007671
+   180007659:	mov    %rsi,%r8
+   18000765c:	mov    $0x2,%edx
+   180007661:	mov    %r14,%rcx
+   180007664:	mov    (%rbx),%rax
+   180007667:	mov    0x1e12(%rip),%r9        # 0x180009480
+   18000766e:	call   *%r9
+   180007671:	incl   0x6fe9(%rip)        # 0x18000e660
+   180007677:	mov    $0x1,%eax
+   18000767c:	jmp    0x180007680
+   18000767e:	xor    %eax,%eax
+   180007680:	mov    0x30(%rsp),%rbx
+   180007685:	mov    0x38(%rsp),%rsi
+   18000768a:	mov    0x48(%rsp),%rdi
+   18000768f:	add    $0x20,%rsp
+   180007693:	pop    %r14
+   180007695:	ret
+   180007696:	mov    $0x7,%ecx
+   18000769b:	call   0x180007ef0
+   1800076a0:	nop
    1800076a1:	int3
    1800076a2:	int3
    1800076a3:	int3
    1800076a4:	mov    %rbx,0x8(%rsp)
-   1800076a9:	mov    %rbp,0x10(%rsp)
-   1800076ae:	mov    %rsi,0x18(%rsp)
-   1800076b3:	push   %rdi
-   1800076b4:	sub    $0x20,%rsp
-   1800076b8:	mov    %r9,%rdi
-   1800076bb:	mov    %r8,%rsi
-   1800076be:	mov    %edx,%ebx
-   1800076c0:	mov    %rcx,%rbp
-   1800076c3:	call   0x180007fa0
-   1800076c8:	test   %eax,%eax
-   1800076ca:	jne    0x1800076e2
-   1800076cc:	cmp    $0x1,%ebx
-   1800076cf:	jne    0x1800076e2
-   1800076d1:	mov    %rsi,%r8
-   1800076d4:	xor    %edx,%edx
-   1800076d6:	mov    %rbp,%rcx
-   1800076d9:	mov    %rdi,%rax
-   1800076dc:	call   *0x1d9e(%rip)        # 0x180009480
-   1800076e2:	mov    0x58(%rsp),%rdx
-   1800076e7:	mov    0x50(%rsp),%ecx
-   1800076eb:	mov    0x30(%rsp),%rbx
-   1800076f0:	mov    0x38(%rsp),%rbp
-   1800076f5:	mov    0x40(%rsp),%rsi
-   1800076fa:	add    $0x20,%rsp
-   1800076fe:	pop    %rdi
-   1800076ff:	jmp    0x180008028
-   180007704:	sub    $0x28,%rsp
-   180007708:	call   0x180007fa0
-   18000770d:	test   %eax,%eax
-   18000770f:	je     0x180007721
-   180007711:	lea    0x6f68(%rip),%rcx        # 0x18000e680
-   180007718:	add    $0x28,%rsp
-   18000771c:	jmp    0x180008046
-   180007721:	call   0x1800037e0
-   180007726:	test   %eax,%eax
-   180007728:	jne    0x18000772f
-   18000772a:	call   0x180008052
-   18000772f:	add    $0x28,%rsp
-   180007733:	ret
-   180007734:	sub    $0x28,%rsp
-   180007738:	xor    %ecx,%ecx
-   18000773a:	call   0x180004f10
-   18000773f:	add    $0x28,%rsp
-   180007743:	jmp    0x180004f10
-   180007748:	rex push %rbx
-   18000774a:	sub    $0x20,%rsp
-   18000774e:	movzbl 0x6f23(%rip),%eax        # 0x18000e678
-   180007755:	test   %ecx,%ecx
-   180007757:	mov    $0x1,%ebx
-   18000775c:	cmove  %ebx,%eax
-   18000775f:	mov    %al,0x6f13(%rip)        # 0x18000e678
-   180007765:	call   0x180007df4
-   18000776a:	call   0x180004f10
-   18000776f:	test   %al,%al
-   180007771:	jne    0x180007777
-   180007773:	xor    %al,%al
-   180007775:	jmp    0x18000778b
-   180007777:	call   0x180004f10
-   18000777c:	test   %al,%al
-   18000777e:	jne    0x180007789
-   180007780:	xor    %ecx,%ecx
-   180007782:	call   0x180004f10
-   180007787:	jmp    0x180007773
-   180007789:	mov    %bl,%al
-   18000778b:	add    $0x20,%rsp
-   18000778f:	pop    %rbx
-   180007790:	ret
-   180007791:	int3
-   180007792:	int3
-   180007793:	int3
-   180007794:	rex push %rbx
-   180007796:	sub    $0x20,%rsp
-   18000779a:	cmpb   $0x0,0x6ed8(%rip)        # 0x18000e679
-   1800077a1:	mov    %ecx,%ebx
-   1800077a3:	jne    0x18000780c
-   1800077a5:	cmp    $0x1,%ecx
-   1800077a8:	ja     0x180007814
-   1800077aa:	call   0x180007fa0
-   1800077af:	test   %eax,%eax
-   1800077b1:	je     0x1800077db
-   1800077b3:	test   %ebx,%ebx
-   1800077b5:	jne    0x1800077db
-   1800077b7:	lea    0x6ec2(%rip),%rcx        # 0x18000e680
-   1800077be:	call   0x18000803a
-   1800077c3:	test   %eax,%eax
-   1800077c5:	jne    0x1800077d7
-   1800077c7:	lea    0x6eca(%rip),%rcx        # 0x18000e698
-   1800077ce:	call   0x18000803a
-   1800077d3:	test   %eax,%eax
-   1800077d5:	je     0x180007805
-   1800077d7:	xor    %al,%al
-   1800077d9:	jmp    0x18000780e
-   1800077db:	movdqa 0x21dd(%rip),%xmm0        # 0x1800099c0
-   1800077e3:	or     $0xffffffffffffffff,%rax
-   1800077e7:	movdqu %xmm0,0x6e91(%rip)        # 0x18000e680
-   1800077ef:	mov    %rax,0x6e9a(%rip)        # 0x18000e690
-   1800077f6:	movdqu %xmm0,0x6e9a(%rip)        # 0x18000e698
-   1800077fe:	mov    %rax,0x6ea3(%rip)        # 0x18000e6a8
-   180007805:	movb   $0x1,0x6e6d(%rip)        # 0x18000e679
-   18000780c:	mov    $0x1,%al
-   18000780e:	add    $0x20,%rsp
-   180007812:	pop    %rbx
-   180007813:	ret
-   180007814:	mov    $0x5,%ecx
-   180007819:	call   0x180007c30
-   18000781e:	int3
-   18000781f:	int3
-   180007820:	sub    $0x18,%rsp
-   180007824:	mov    %rcx,%r8
-   180007827:	mov    $0x5a4d,%eax
-   18000782c:	cmp    %ax,-0x7833(%rip)        # 0x180000000
-   180007833:	jne    0x1800078ad
-   180007835:	movslq -0x7800(%rip),%rcx        # 0x18000003c
-   18000783c:	lea    -0x7843(%rip),%rdx        # 0x180000000
-   180007843:	add    %rdx,%rcx
-   180007846:	cmpl   $0x4550,(%rcx)
-   18000784c:	jne    0x1800078ad
-   18000784e:	mov    $0x20b,%eax
-   180007853:	cmp    %ax,0x18(%rcx)
-   180007857:	jne    0x1800078ad
-   180007859:	sub    %rdx,%r8
-   18000785c:	movzwl 0x14(%rcx),%eax
-   180007860:	lea    0x18(%rcx),%rdx
-   180007864:	add    %rax,%rdx
-   180007867:	movzwl 0x6(%rcx),%eax
-   18000786b:	lea    (%rax,%rax,4),%rcx
-   18000786f:	lea    (%rdx,%rcx,8),%r9
-   180007873:	mov    %rdx,(%rsp)
-   180007877:	cmp    %r9,%rdx
-   18000787a:	je     0x180007894
-   18000787c:	mov    0xc(%rdx),%ecx
-   18000787f:	cmp    %rcx,%r8
-   180007882:	jb     0x18000788e
-   180007884:	mov    0x8(%rdx),%eax
-   180007887:	add    %ecx,%eax
-   180007889:	cmp    %rax,%r8
-   18000788c:	jb     0x180007896
-   18000788e:	add    $0x28,%rdx
-   180007892:	jmp    0x180007873
-   180007894:	xor    %edx,%edx
-   180007896:	test   %rdx,%rdx
-   180007899:	jne    0x18000789f
-   18000789b:	xor    %al,%al
-   18000789d:	jmp    0x1800078b3
-   18000789f:	cmpl   $0x0,0x24(%rdx)
-   1800078a3:	jge    0x1800078a9
-   1800078a5:	xor    %al,%al
-   1800078a7:	jmp    0x1800078b3
-   1800078a9:	mov    $0x1,%al
-   1800078ab:	jmp    0x1800078b3
-   1800078ad:	xor    %al,%al
-   1800078af:	jmp    0x1800078b3
-   1800078b1:	xor    %al,%al
-   1800078b3:	add    $0x18,%rsp
-   1800078b7:	ret
-   1800078b8:	rex push %rbx
-   1800078ba:	sub    $0x20,%rsp
-   1800078be:	mov    %cl,%bl
-   1800078c0:	call   0x180007fa0
-   1800078c5:	xor    %edx,%edx
-   1800078c7:	test   %eax,%eax
-   1800078c9:	je     0x1800078d6
-   1800078cb:	test   %bl,%bl
-   1800078cd:	jne    0x1800078d6
-   1800078cf:	xchg   %rdx,0x6d9a(%rip)        # 0x18000e670
-   1800078d6:	add    $0x20,%rsp
-   1800078da:	pop    %rbx
-   1800078db:	ret
-   1800078dc:	rex push %rbx
-   1800078de:	sub    $0x20,%rsp
-   1800078e2:	cmpb   $0x0,0x6d8f(%rip)        # 0x18000e678
-   1800078e9:	mov    %cl,%bl
-   1800078eb:	je     0x1800078f1
-   1800078ed:	test   %dl,%dl
-   1800078ef:	jne    0x1800078fd
-   1800078f1:	call   0x180004f10
-   1800078f6:	mov    %bl,%cl
-   1800078f8:	call   0x180004f10
-   1800078fd:	mov    $0x1,%al
-   1800078ff:	add    $0x20,%rsp
-   180007903:	pop    %rbx
-   180007904:	ret
-   180007905:	int3
-   180007906:	int3
-   180007907:	int3
-   180007908:	rex push %rbx
-   18000790a:	sub    $0x20,%rsp
-   18000790e:	cmpq   $0xffffffffffffffff,0x6d6a(%rip)        # 0x18000e680
-   180007916:	mov    %rcx,%rbx
-   180007919:	jne    0x180007922
-   18000791b:	call   0x18000804c
-   180007920:	jmp    0x180007931
-   180007922:	mov    %rbx,%rdx
-   180007925:	lea    0x6d54(%rip),%rcx        # 0x18000e680
-   18000792c:	call   0x180008040
-   180007931:	xor    %edx,%edx
-   180007933:	test   %eax,%eax
-   180007935:	cmove  %rbx,%rdx
-   180007939:	mov    %rdx,%rax
-   18000793c:	add    $0x20,%rsp
-   180007940:	pop    %rbx
-   180007941:	ret
-   180007942:	int3
-   180007943:	int3
-   180007944:	sub    $0x28,%rsp
-   180007948:	call   0x180007908
-   18000794d:	neg    %rax
-   180007950:	sbb    %eax,%eax
-   180007952:	neg    %eax
-   180007954:	dec    %eax
-   180007956:	add    $0x28,%rsp
-   18000795a:	ret
-   18000795b:	int3
-   18000795c:	ret    $0x0
-   18000795f:	int3
-   180007960:	andq   $0x0,0x10(%rcx)
-   180007965:	lea    0x2064(%rip),%rax        # 0x1800099d0
-   18000796c:	mov    %rax,0x8(%rcx)
-   180007970:	lea    0x1be1(%rip),%rax        # 0x180009558
-   180007977:	mov    %rax,(%rcx)
-   18000797a:	mov    %rcx,%rax
-   18000797d:	ret
-   18000797e:	int3
-   18000797f:	int3
-   180007980:	sub    $0x48,%rsp
-   180007984:	lea    0x20(%rsp),%rcx
-   180007989:	call   0x180007960
-   18000798e:	lea    0x3dfb(%rip),%rdx        # 0x18000b790
-   180007995:	lea    0x20(%rsp),%rcx
-   18000799a:	call   0x180007fd4
-   18000799f:	int3
-   1800079a0:	jmp    0x180008058
-   1800079a5:	int3
-   1800079a6:	int3
-   1800079a7:	int3
-   1800079a8:	rex push %rbx
-   1800079aa:	sub    $0x20,%rsp
-   1800079ae:	mov    %rcx,%rbx
-   1800079b1:	xor    %ecx,%ecx
-   1800079b3:	call   *0x16cf(%rip)        # 0x180009088
-   1800079b9:	mov    %rbx,%rcx
-   1800079bc:	call   *0x16ce(%rip)        # 0x180009090
-   1800079c2:	call   *0x16b8(%rip)        # 0x180009080
-   1800079c8:	mov    %rax,%rcx
-   1800079cb:	mov    $0xc0000409,%edx
-   1800079d0:	add    $0x20,%rsp
-   1800079d4:	pop    %rbx
-   1800079d5:	rex.W jmp *0x169c(%rip)        # 0x180009078
-   1800079dc:	mov    %rcx,0x8(%rsp)
-   1800079e1:	sub    $0x38,%rsp
-   1800079e5:	mov    $0x17,%ecx
-   1800079ea:	call   *0x1680(%rip)        # 0x180009070
-   1800079f0:	test   %eax,%eax
-   1800079f2:	je     0x1800079fb
-   1800079f4:	mov    $0x2,%ecx
-   1800079f9:	int    $0x29
-   1800079fb:	lea    0x6d5e(%rip),%rcx        # 0x18000e760
-   180007a02:	call   0x180007ab0
-   180007a07:	mov    0x38(%rsp),%rax
-   180007a0c:	mov    %rax,0x6e45(%rip)        # 0x18000e858
-   180007a13:	lea    0x38(%rsp),%rax
-   180007a18:	add    $0x8,%rax
-   180007a1c:	mov    %rax,0x6dd5(%rip)        # 0x18000e7f8
-   180007a23:	mov    0x6e2e(%rip),%rax        # 0x18000e858
-   180007a2a:	mov    %rax,0x6c9f(%rip)        # 0x18000e6d0
-   180007a31:	mov    0x40(%rsp),%rax
-   180007a36:	mov    %rax,0x6da3(%rip)        # 0x18000e7e0
-   180007a3d:	movl   $0xc0000409,0x6c79(%rip)        # 0x18000e6c0
-   180007a47:	movl   $0x1,0x6c73(%rip)        # 0x18000e6c4
-   180007a51:	movl   $0x1,0x6c7d(%rip)        # 0x18000e6d8
-   180007a5b:	mov    $0x8,%eax
-   180007a60:	imul   $0x0,%rax,%rax
-   180007a64:	lea    0x6c75(%rip),%rcx        # 0x18000e6e0
-   180007a6b:	movq   $0x2,(%rcx,%rax,1)
-   180007a73:	mov    $0x8,%eax
-   180007a78:	imul   $0x0,%rax,%rax
-   180007a7c:	mov    0x6585(%rip),%rcx        # 0x18000e008
-   180007a83:	mov    %rcx,0x20(%rsp,%rax,1)
-   180007a88:	mov    $0x8,%eax
-   180007a8d:	imul   $0x1,%rax,%rax
-   180007a91:	mov    0x6568(%rip),%rcx        # 0x18000e000
-   180007a98:	mov    %rcx,0x20(%rsp,%rax,1)
-   180007a9d:	lea    0x1f3c(%rip),%rcx        # 0x1800099e0
-   180007aa4:	call   0x1800079a8
-   180007aa9:	add    $0x38,%rsp
-   180007aad:	ret
-   180007aae:	int3
-   180007aaf:	int3
-   180007ab0:	rex push %rbx
-   180007ab2:	push   %rsi
-   180007ab3:	push   %rdi
-   180007ab4:	sub    $0x40,%rsp
-   180007ab8:	mov    %rcx,%rbx
-   180007abb:	call   *0x15e7(%rip)        # 0x1800090a8
-   180007ac1:	mov    0xf8(%rbx),%rsi
-   180007ac8:	xor    %edi,%edi
-   180007aca:	xor    %r8d,%r8d
-   180007acd:	lea    0x60(%rsp),%rdx
-   180007ad2:	mov    %rsi,%rcx
-   180007ad5:	call   *0x15c5(%rip)        # 0x1800090a0
-   180007adb:	test   %rax,%rax
-   180007ade:	je     0x180007b19
-   180007ae0:	andq   $0x0,0x38(%rsp)
-   180007ae6:	lea    0x68(%rsp),%rcx
-   180007aeb:	mov    0x60(%rsp),%rdx
-   180007af0:	mov    %rax,%r9
-   180007af3:	mov    %rcx,0x30(%rsp)
-   180007af8:	mov    %rsi,%r8
-   180007afb:	lea    0x70(%rsp),%rcx
-   180007b00:	mov    %rcx,0x28(%rsp)
-   180007b05:	xor    %ecx,%ecx
-   180007b07:	mov    %rbx,0x20(%rsp)
-   180007b0c:	call   *0x1586(%rip)        # 0x180009098
-   180007b12:	inc    %edi
-   180007b14:	cmp    $0x2,%edi
-   180007b17:	jl     0x180007aca
-   180007b19:	add    $0x40,%rsp
-   180007b1d:	pop    %rdi
-   180007b1e:	pop    %rsi
-   180007b1f:	pop    %rbx
-   180007b20:	ret
-   180007b21:	int3
-   180007b22:	int3
-   180007b23:	int3
-   180007b24:	mov    %rbx,0x20(%rsp)
-   180007b29:	push   %rbp
-   180007b2a:	mov    %rsp,%rbp
-   180007b2d:	sub    $0x20,%rsp
-   180007b31:	mov    0x64d0(%rip),%rax        # 0x18000e008
-   180007b38:	movabs $0x2b992ddfa232,%rbx
-   180007b42:	cmp    %rbx,%rax
-   180007b45:	jne    0x180007bbb
-   180007b47:	andq   $0x0,0x18(%rbp)
-   180007b4c:	lea    0x18(%rbp),%rcx
-   180007b50:	call   *0x14fa(%rip)        # 0x180009050
-   180007b56:	mov    0x18(%rbp),%rax
-   180007b5a:	mov    %rax,0x10(%rbp)
-   180007b5e:	call   *0x14f4(%rip)        # 0x180009058
-   180007b64:	mov    %eax,%eax
-   180007b66:	xor    %rax,0x10(%rbp)
-   180007b6a:	call   *0x14f0(%rip)        # 0x180009060
-   180007b70:	mov    %eax,%eax
-   180007b72:	lea    0x20(%rbp),%rcx
-   180007b76:	xor    %rax,0x10(%rbp)
-   180007b7a:	call   *0x14e8(%rip)        # 0x180009068
-   180007b80:	mov    0x20(%rbp),%eax
-   180007b83:	lea    0x10(%rbp),%rcx
-   180007b87:	shl    $0x20,%rax
-   180007b8b:	xor    0x20(%rbp),%rax
-   180007b8f:	xor    0x10(%rbp),%rax
-   180007b93:	xor    %rcx,%rax
-   180007b96:	movabs $0xffffffffffff,%rcx
-   180007ba0:	and    %rcx,%rax
-   180007ba3:	movabs $0x2b992ddfa233,%rcx
-   180007bad:	cmp    %rbx,%rax
-   180007bb0:	cmove  %rcx,%rax
-   180007bb4:	mov    %rax,0x644d(%rip)        # 0x18000e008
-   180007bbb:	mov    0x48(%rsp),%rbx
-   180007bc0:	not    %rax
-   180007bc3:	mov    %rax,0x6436(%rip)        # 0x18000e000
-   180007bca:	add    $0x20,%rsp
-   180007bce:	pop    %rbp
-   180007bcf:	ret
-   180007bd0:	sub    $0x28,%rsp
-   180007bd4:	cmp    $0x1,%edx
-   180007bd7:	jne    0x180007be9
-   180007bd9:	cmpq   $0x0,0x1dcf(%rip)        # 0x1800099b0
-   180007be1:	jne    0x180007be9
-   180007be3:	call   *0x145f(%rip)        # 0x180009048
-   180007be9:	mov    $0x1,%eax
-   180007bee:	add    $0x28,%rsp
-   180007bf2:	ret
-   180007bf3:	int3
-   180007bf4:	lea    0x7035(%rip),%rax        # 0x18000ec30
-   180007bfb:	ret
-   180007bfc:	lea    0x7035(%rip),%rax        # 0x18000ec38
-   180007c03:	ret
+   1800076a9:	push   %rdi
+   1800076aa:	sub    $0x30,%rsp
+   1800076ae:	mov    %cl,%dil
+   1800076b1:	mov    0x6fa9(%rip),%eax        # 0x18000e660
+   1800076b7:	test   %eax,%eax
+   1800076b9:	jg     0x1800076c8
+   1800076bb:	xor    %eax,%eax
+   1800076bd:	mov    0x40(%rsp),%rbx
+   1800076c2:	add    $0x30,%rsp
+   1800076c6:	pop    %rdi
+   1800076c7:	ret
+   1800076c8:	dec    %eax
+   1800076ca:	mov    %eax,0x6f90(%rip)        # 0x18000e660
+   1800076d0:	call   0x18000789c
+   1800076d5:	mov    %al,%bl
+   1800076d7:	mov    %al,0x20(%rsp)
+   1800076db:	cmpl   $0x2,0x6f86(%rip)        # 0x18000e668
+   1800076e2:	jne    0x18000771b
+   1800076e4:	call   0x1800079c4
+   1800076e9:	call   0x180007530
+   1800076ee:	call   0x180008078
+   1800076f3:	andl   $0x0,0x6f6e(%rip)        # 0x18000e668
+   1800076fa:	mov    %bl,%cl
+   1800076fc:	call   0x180007b78
+   180007701:	xor    %edx,%edx
+   180007703:	mov    %dil,%cl
+   180007706:	call   0x180007b9c
+   18000770b:	neg    %al
+   18000770d:	sbb    %ebx,%ebx
+   18000770f:	and    $0x1,%ebx
+   180007712:	call   0x1800079f4
+   180007717:	mov    %ebx,%eax
+   180007719:	jmp    0x1800076bd
+   18000771b:	mov    $0x7,%ecx
+   180007720:	call   0x180007ef0
+   180007725:	nop
+   180007726:	nop
+   180007727:	int3
+   180007728:	mov    %rsp,%rax
+   18000772b:	mov    %rbx,0x20(%rax)
+   18000772f:	mov    %r8,0x18(%rax)
+   180007733:	mov    %edx,0x10(%rax)
+   180007736:	mov    %rcx,0x8(%rax)
+   18000773a:	push   %rsi
+   18000773b:	push   %rdi
+   18000773c:	push   %r14
+   18000773e:	sub    $0x40,%rsp
+   180007742:	mov    %r8,%rsi
+   180007745:	mov    %edx,%edi
+   180007747:	mov    %rcx,%r14
+   18000774a:	test   %edx,%edx
+   18000774c:	jne    0x18000775d
+   18000774e:	cmp    %edx,0x6f0c(%rip)        # 0x18000e660
+   180007754:	jg     0x18000775d
+   180007756:	xor    %eax,%eax
+   180007758:	jmp    0x18000784b
+   18000775d:	lea    -0x1(%rdx),%eax
+   180007760:	cmp    $0x1,%eax
+   180007763:	ja     0x1800077aa
+   180007765:	mov    0x2264(%rip),%rax        # 0x1800099d0
+   18000776c:	test   %rax,%rax
+   18000776f:	jne    0x18000777b
+   180007771:	movl   $0x1,0x30(%rsp)
+   180007779:	jmp    0x18000778f
+   18000777b:	call   *0x1cff(%rip)        # 0x180009480
+   180007781:	mov    %eax,%ebx
+   180007783:	mov    %eax,0x30(%rsp)
+   180007787:	test   %eax,%eax
+   180007789:	je     0x180007841
+   18000778f:	mov    %rsi,%r8
+   180007792:	mov    %edi,%edx
+   180007794:	mov    %r14,%rcx
+   180007797:	call   0x18000753c
+   18000779c:	mov    %eax,%ebx
+   18000779e:	mov    %eax,0x30(%rsp)
+   1800077a2:	test   %eax,%eax
+   1800077a4:	je     0x180007841
+   1800077aa:	mov    %rsi,%r8
+   1800077ad:	mov    %edi,%edx
+   1800077af:	mov    %r14,%rcx
+   1800077b2:	call   0x180007e90
+   1800077b7:	mov    %eax,%ebx
+   1800077b9:	mov    %eax,0x30(%rsp)
+   1800077bd:	cmp    $0x1,%edi
+   1800077c0:	jne    0x1800077f8
+   1800077c2:	test   %eax,%eax
+   1800077c4:	jne    0x1800077f8
+   1800077c6:	mov    %rsi,%r8
+   1800077c9:	xor    %edx,%edx
+   1800077cb:	mov    %r14,%rcx
+   1800077ce:	call   0x180007e90
+   1800077d3:	test   %rsi,%rsi
+   1800077d6:	setne  %cl
+   1800077d9:	call   0x1800076a4
+   1800077de:	mov    0x21eb(%rip),%rax        # 0x1800099d0
+   1800077e5:	test   %rax,%rax
+   1800077e8:	je     0x1800077f8
+   1800077ea:	mov    %rsi,%r8
+   1800077ed:	xor    %edx,%edx
+   1800077ef:	mov    %r14,%rcx
+   1800077f2:	call   *0x1c88(%rip)        # 0x180009480
+   1800077f8:	test   %edi,%edi
+   1800077fa:	je     0x180007801
+   1800077fc:	cmp    $0x3,%edi
+   1800077ff:	jne    0x180007841
+   180007801:	mov    %rsi,%r8
+   180007804:	mov    %edi,%edx
+   180007806:	mov    %r14,%rcx
+   180007809:	call   0x18000753c
+   18000780e:	mov    %eax,%ebx
+   180007810:	mov    %eax,0x30(%rsp)
+   180007814:	test   %eax,%eax
+   180007816:	je     0x180007841
+   180007818:	mov    0x21b1(%rip),%rax        # 0x1800099d0
+   18000781f:	test   %rax,%rax
+   180007822:	jne    0x18000782d
+   180007824:	lea    0x1(%rax),%ebx
+   180007827:	mov    %ebx,0x30(%rsp)
+   18000782b:	jmp    0x180007841
+   18000782d:	mov    %rsi,%r8
+   180007830:	mov    %edi,%edx
+   180007832:	mov    %r14,%rcx
+   180007835:	call   *0x1c45(%rip)        # 0x180009480
+   18000783b:	mov    %eax,%ebx
+   18000783d:	mov    %eax,0x30(%rsp)
+   180007841:	jmp    0x180007849
+   180007843:	xor    %ebx,%ebx
+   180007845:	mov    %ebx,0x30(%rsp)
+   180007849:	mov    %ebx,%eax
+   18000784b:	mov    0x78(%rsp),%rbx
+   180007850:	add    $0x40,%rsp
+   180007854:	pop    %r14
+   180007856:	pop    %rdi
+   180007857:	pop    %rsi
+   180007858:	ret
+   180007859:	int3
+   18000785a:	int3
+   18000785b:	int3
+   18000785c:	mov    %rbx,0x8(%rsp)
+   180007861:	mov    %rsi,0x10(%rsp)
+   180007866:	push   %rdi
+   180007867:	sub    $0x20,%rsp
+   18000786b:	mov    %r8,%rdi
+   18000786e:	mov    %edx,%ebx
+   180007870:	mov    %rcx,%rsi
+   180007873:	cmp    $0x1,%edx
+   180007876:	jne    0x18000787d
+   180007878:	call   0x180007de4
+   18000787d:	mov    %rdi,%r8
+   180007880:	mov    %ebx,%edx
+   180007882:	mov    %rsi,%rcx
+   180007885:	mov    0x30(%rsp),%rbx
+   18000788a:	mov    0x38(%rsp),%rsi
+   18000788f:	add    $0x20,%rsp
+   180007893:	pop    %rdi
+   180007894:	jmp    0x180007728
+   180007899:	int3
+   18000789a:	int3
+   18000789b:	int3
+   18000789c:	sub    $0x28,%rsp
+   1800078a0:	call   0x180008260
+   1800078a5:	test   %eax,%eax
+   1800078a7:	je     0x1800078ca
+   1800078a9:	mov    %gs:0x30,%rax
+   1800078b2:	mov    0x8(%rax),%rcx
+   1800078b6:	jmp    0x1800078bd
+   1800078b8:	cmp    %rax,%rcx
+   1800078bb:	je     0x1800078d1
+   1800078bd:	xor    %eax,%eax
+   1800078bf:	lock cmpxchg %rcx,0x6da8(%rip)        # 0x18000e670
+   1800078c8:	jne    0x1800078b8
+   1800078ca:	xor    %al,%al
+   1800078cc:	add    $0x28,%rsp
+   1800078d0:	ret
+   1800078d1:	mov    $0x1,%al
+   1800078d3:	jmp    0x1800078cc
+   1800078d5:	int3
+   1800078d6:	int3
+   1800078d7:	int3
+   1800078d8:	sub    $0x28,%rsp
+   1800078dc:	call   0x180008260
+   1800078e1:	test   %eax,%eax
+   1800078e3:	je     0x1800078ec
+   1800078e5:	call   0x1800080b4
+   1800078ea:	jmp    0x180007905
+   1800078ec:	call   0x180008258
+   1800078f1:	mov    %eax,%ecx
+   1800078f3:	call   0x1800082ee
+   1800078f8:	test   %eax,%eax
+   1800078fa:	je     0x180007900
+   1800078fc:	xor    %al,%al
+   1800078fe:	jmp    0x180007907
+   180007900:	call   0x1800082f4
+   180007905:	mov    $0x1,%al
+   180007907:	add    $0x28,%rsp
+   18000790b:	ret
+   18000790c:	sub    $0x28,%rsp
+   180007910:	xor    %ecx,%ecx
+   180007912:	call   0x180007a54
+   180007917:	test   %al,%al
+   180007919:	setne  %al
+   18000791c:	add    $0x28,%rsp
+   180007920:	ret
+   180007921:	int3
+   180007922:	int3
+   180007923:	int3
+   180007924:	sub    $0x28,%rsp
+   180007928:	call   0x180005250
+   18000792d:	test   %al,%al
+   18000792f:	jne    0x180007935
+   180007931:	xor    %al,%al
+   180007933:	jmp    0x180007947
+   180007935:	call   0x180005250
+   18000793a:	test   %al,%al
+   18000793c:	jne    0x180007945
+   18000793e:	call   0x180005250
+   180007943:	jmp    0x180007931
+   180007945:	mov    $0x1,%al
+   180007947:	add    $0x28,%rsp
+   18000794b:	ret
+   18000794c:	sub    $0x28,%rsp
+   180007950:	call   0x180005250
+   180007955:	call   0x180005250
+   18000795a:	mov    $0x1,%al
+   18000795c:	add    $0x28,%rsp
+   180007960:	ret
+   180007961:	int3
+   180007962:	int3
+   180007963:	int3
+   180007964:	mov    %rbx,0x8(%rsp)
+   180007969:	mov    %rbp,0x10(%rsp)
+   18000796e:	mov    %rsi,0x18(%rsp)
+   180007973:	push   %rdi
+   180007974:	sub    $0x20,%rsp
+   180007978:	mov    %r9,%rdi
+   18000797b:	mov    %r8,%rsi
+   18000797e:	mov    %edx,%ebx
+   180007980:	mov    %rcx,%rbp
+   180007983:	call   0x180008260
+   180007988:	test   %eax,%eax
+   18000798a:	jne    0x1800079a2
+   18000798c:	cmp    $0x1,%ebx
+   18000798f:	jne    0x1800079a2
+   180007991:	mov    %rsi,%r8
+   180007994:	xor    %edx,%edx
+   180007996:	mov    %rbp,%rcx
+   180007999:	mov    %rdi,%rax
+   18000799c:	call   *0x1ade(%rip)        # 0x180009480
+   1800079a2:	mov    0x58(%rsp),%rdx
+   1800079a7:	mov    0x50(%rsp),%ecx
+   1800079ab:	mov    0x30(%rsp),%rbx
+   1800079b0:	mov    0x38(%rsp),%rbp
+   1800079b5:	mov    0x40(%rsp),%rsi
+   1800079ba:	add    $0x20,%rsp
+   1800079be:	pop    %rdi
+   1800079bf:	jmp    0x1800082e8
+   1800079c4:	sub    $0x28,%rsp
+   1800079c8:	call   0x180008260
+   1800079cd:	test   %eax,%eax
+   1800079cf:	je     0x1800079e1
+   1800079d1:	lea    0x6ca8(%rip),%rcx        # 0x18000e680
+   1800079d8:	add    $0x28,%rsp
+   1800079dc:	jmp    0x180008306
+   1800079e1:	call   0x1800037e0
+   1800079e6:	test   %eax,%eax
+   1800079e8:	jne    0x1800079ef
+   1800079ea:	call   0x180008312
+   1800079ef:	add    $0x28,%rsp
+   1800079f3:	ret
+   1800079f4:	sub    $0x28,%rsp
+   1800079f8:	xor    %ecx,%ecx
+   1800079fa:	call   0x180005250
+   1800079ff:	add    $0x28,%rsp
+   180007a03:	jmp    0x180005250
+   180007a08:	rex push %rbx
+   180007a0a:	sub    $0x20,%rsp
+   180007a0e:	movzbl 0x6c63(%rip),%eax        # 0x18000e678
+   180007a15:	test   %ecx,%ecx
+   180007a17:	mov    $0x1,%ebx
+   180007a1c:	cmove  %ebx,%eax
+   180007a1f:	mov    %al,0x6c53(%rip)        # 0x18000e678
+   180007a25:	call   0x1800080b4
+   180007a2a:	call   0x180005250
+   180007a2f:	test   %al,%al
+   180007a31:	jne    0x180007a37
+   180007a33:	xor    %al,%al
+   180007a35:	jmp    0x180007a4b
+   180007a37:	call   0x180005250
+   180007a3c:	test   %al,%al
+   180007a3e:	jne    0x180007a49
+   180007a40:	xor    %ecx,%ecx
+   180007a42:	call   0x180005250
+   180007a47:	jmp    0x180007a33
+   180007a49:	mov    %bl,%al
+   180007a4b:	add    $0x20,%rsp
+   180007a4f:	pop    %rbx
+   180007a50:	ret
+   180007a51:	int3
+   180007a52:	int3
+   180007a53:	int3
+   180007a54:	rex push %rbx
+   180007a56:	sub    $0x20,%rsp
+   180007a5a:	cmpb   $0x0,0x6c18(%rip)        # 0x18000e679
+   180007a61:	mov    %ecx,%ebx
+   180007a63:	jne    0x180007acc
+   180007a65:	cmp    $0x1,%ecx
+   180007a68:	ja     0x180007ad4
+   180007a6a:	call   0x180008260
+   180007a6f:	test   %eax,%eax
+   180007a71:	je     0x180007a9b
+   180007a73:	test   %ebx,%ebx
+   180007a75:	jne    0x180007a9b
+   180007a77:	lea    0x6c02(%rip),%rcx        # 0x18000e680
+   180007a7e:	call   0x1800082fa
+   180007a83:	test   %eax,%eax
+   180007a85:	jne    0x180007a97
+   180007a87:	lea    0x6c0a(%rip),%rcx        # 0x18000e698
+   180007a8e:	call   0x1800082fa
+   180007a93:	test   %eax,%eax
+   180007a95:	je     0x180007ac5
+   180007a97:	xor    %al,%al
+   180007a99:	jmp    0x180007ace
+   180007a9b:	movdqa 0x1f0d(%rip),%xmm0        # 0x1800099b0
+   180007aa3:	or     $0xffffffffffffffff,%rax
+   180007aa7:	movdqu %xmm0,0x6bd1(%rip)        # 0x18000e680
+   180007aaf:	mov    %rax,0x6bda(%rip)        # 0x18000e690
+   180007ab6:	movdqu %xmm0,0x6bda(%rip)        # 0x18000e698
+   180007abe:	mov    %rax,0x6be3(%rip)        # 0x18000e6a8
+   180007ac5:	movb   $0x1,0x6bad(%rip)        # 0x18000e679
+   180007acc:	mov    $0x1,%al
+   180007ace:	add    $0x20,%rsp
+   180007ad2:	pop    %rbx
+   180007ad3:	ret
+   180007ad4:	mov    $0x5,%ecx
+   180007ad9:	call   0x180007ef0
+   180007ade:	int3
+   180007adf:	int3
+   180007ae0:	sub    $0x18,%rsp
+   180007ae4:	mov    %rcx,%r8
+   180007ae7:	mov    $0x5a4d,%eax
+   180007aec:	cmp    %ax,-0x7af3(%rip)        # 0x180000000
+   180007af3:	jne    0x180007b6d
+   180007af5:	movslq -0x7ac0(%rip),%rcx        # 0x18000003c
+   180007afc:	lea    -0x7b03(%rip),%rdx        # 0x180000000
+   180007b03:	add    %rdx,%rcx
+   180007b06:	cmpl   $0x4550,(%rcx)
+   180007b0c:	jne    0x180007b6d
+   180007b0e:	mov    $0x20b,%eax
+   180007b13:	cmp    %ax,0x18(%rcx)
+   180007b17:	jne    0x180007b6d
+   180007b19:	sub    %rdx,%r8
+   180007b1c:	movzwl 0x14(%rcx),%eax
+   180007b20:	lea    0x18(%rcx),%rdx
+   180007b24:	add    %rax,%rdx
+   180007b27:	movzwl 0x6(%rcx),%eax
+   180007b2b:	lea    (%rax,%rax,4),%rcx
+   180007b2f:	lea    (%rdx,%rcx,8),%r9
+   180007b33:	mov    %rdx,(%rsp)
+   180007b37:	cmp    %r9,%rdx
+   180007b3a:	je     0x180007b54
+   180007b3c:	mov    0xc(%rdx),%ecx
+   180007b3f:	cmp    %rcx,%r8
+   180007b42:	jb     0x180007b4e
+   180007b44:	mov    0x8(%rdx),%eax
+   180007b47:	add    %ecx,%eax
+   180007b49:	cmp    %rax,%r8
+   180007b4c:	jb     0x180007b56
+   180007b4e:	add    $0x28,%rdx
+   180007b52:	jmp    0x180007b33
+   180007b54:	xor    %edx,%edx
+   180007b56:	test   %rdx,%rdx
+   180007b59:	jne    0x180007b5f
+   180007b5b:	xor    %al,%al
+   180007b5d:	jmp    0x180007b73
+   180007b5f:	cmpl   $0x0,0x24(%rdx)
+   180007b63:	jge    0x180007b69
+   180007b65:	xor    %al,%al
+   180007b67:	jmp    0x180007b73
+   180007b69:	mov    $0x1,%al
+   180007b6b:	jmp    0x180007b73
+   180007b6d:	xor    %al,%al
+   180007b6f:	jmp    0x180007b73
+   180007b71:	xor    %al,%al
+   180007b73:	add    $0x18,%rsp
+   180007b77:	ret
+   180007b78:	rex push %rbx
+   180007b7a:	sub    $0x20,%rsp
+   180007b7e:	mov    %cl,%bl
+   180007b80:	call   0x180008260
+   180007b85:	xor    %edx,%edx
+   180007b87:	test   %eax,%eax
+   180007b89:	je     0x180007b96
+   180007b8b:	test   %bl,%bl
+   180007b8d:	jne    0x180007b96
+   180007b8f:	xchg   %rdx,0x6ada(%rip)        # 0x18000e670
+   180007b96:	add    $0x20,%rsp
+   180007b9a:	pop    %rbx
+   180007b9b:	ret
+   180007b9c:	rex push %rbx
+   180007b9e:	sub    $0x20,%rsp
+   180007ba2:	cmpb   $0x0,0x6acf(%rip)        # 0x18000e678
+   180007ba9:	mov    %cl,%bl
+   180007bab:	je     0x180007bb1
+   180007bad:	test   %dl,%dl
+   180007baf:	jne    0x180007bbd
+   180007bb1:	call   0x180005250
+   180007bb6:	mov    %bl,%cl
+   180007bb8:	call   0x180005250
+   180007bbd:	mov    $0x1,%al
+   180007bbf:	add    $0x20,%rsp
+   180007bc3:	pop    %rbx
+   180007bc4:	ret
+   180007bc5:	int3
+   180007bc6:	int3
+   180007bc7:	int3
+   180007bc8:	rex push %rbx
+   180007bca:	sub    $0x20,%rsp
+   180007bce:	cmpq   $0xffffffffffffffff,0x6aaa(%rip)        # 0x18000e680
+   180007bd6:	mov    %rcx,%rbx
+   180007bd9:	jne    0x180007be2
+   180007bdb:	call   0x18000830c
+   180007be0:	jmp    0x180007bf1
+   180007be2:	mov    %rbx,%rdx
+   180007be5:	lea    0x6a94(%rip),%rcx        # 0x18000e680
+   180007bec:	call   0x180008300
+   180007bf1:	xor    %edx,%edx
+   180007bf3:	test   %eax,%eax
+   180007bf5:	cmove  %rbx,%rdx
+   180007bf9:	mov    %rdx,%rax
+   180007bfc:	add    $0x20,%rsp
+   180007c00:	pop    %rbx
+   180007c01:	ret
+   180007c02:	int3
+   180007c03:	int3
    180007c04:	sub    $0x28,%rsp
-   180007c08:	call   0x180007bf4
-   180007c0d:	orq    $0x24,(%rax)
-   180007c11:	call   0x180007bfc
-   180007c16:	orq    $0x2,(%rax)
-   180007c1a:	add    $0x28,%rsp
-   180007c1e:	ret
+   180007c08:	call   0x180007bc8
+   180007c0d:	neg    %rax
+   180007c10:	sbb    %eax,%eax
+   180007c12:	neg    %eax
+   180007c14:	dec    %eax
+   180007c16:	add    $0x28,%rsp
+   180007c1a:	ret
+   180007c1b:	int3
+   180007c1c:	ret    $0x0
    180007c1f:	int3
-   180007c20:	lea    0x7021(%rip),%rax        # 0x18000ec48
-   180007c27:	ret
-   180007c28:	andl   $0x0,0x7011(%rip)        # 0x18000ec40
-   180007c2f:	ret
-   180007c30:	mov    %rbx,0x8(%rsp)
-   180007c35:	push   %rbp
-   180007c36:	lea    -0x4c0(%rsp),%rbp
-   180007c3e:	sub    $0x5c0,%rsp
-   180007c45:	mov    %ecx,%ebx
-   180007c47:	mov    $0x17,%ecx
-   180007c4c:	call   *0x141e(%rip)        # 0x180009070
-   180007c52:	test   %eax,%eax
-   180007c54:	je     0x180007c5a
-   180007c56:	mov    %ebx,%ecx
-   180007c58:	int    $0x29
-   180007c5a:	mov    $0x3,%ecx
-   180007c5f:	call   0x180007c28
-   180007c64:	xor    %edx,%edx
-   180007c66:	lea    -0x10(%rbp),%rcx
-   180007c6a:	mov    $0x4d0,%r8d
-   180007c70:	call   0x180007fe6
-   180007c75:	lea    -0x10(%rbp),%rcx
-   180007c79:	call   *0x1429(%rip)        # 0x1800090a8
-   180007c7f:	mov    0xe8(%rbp),%rbx
-   180007c86:	lea    0x4d8(%rbp),%rdx
-   180007c8d:	mov    %rbx,%rcx
-   180007c90:	xor    %r8d,%r8d
-   180007c93:	call   *0x1407(%rip)        # 0x1800090a0
-   180007c99:	test   %rax,%rax
-   180007c9c:	je     0x180007cda
-   180007c9e:	andq   $0x0,0x38(%rsp)
-   180007ca4:	lea    0x4e0(%rbp),%rcx
-   180007cab:	mov    0x4d8(%rbp),%rdx
-   180007cb2:	mov    %rax,%r9
-   180007cb5:	mov    %rcx,0x30(%rsp)
-   180007cba:	mov    %rbx,%r8
-   180007cbd:	lea    0x4e8(%rbp),%rcx
-   180007cc4:	mov    %rcx,0x28(%rsp)
-   180007cc9:	lea    -0x10(%rbp),%rcx
-   180007ccd:	mov    %rcx,0x20(%rsp)
-   180007cd2:	xor    %ecx,%ecx
-   180007cd4:	call   *0x13be(%rip)        # 0x180009098
-   180007cda:	mov    0x4c8(%rbp),%rax
-   180007ce1:	lea    0x50(%rsp),%rcx
-   180007ce6:	mov    %rax,0xe8(%rbp)
-   180007ced:	xor    %edx,%edx
-   180007cef:	lea    0x4c8(%rbp),%rax
-   180007cf6:	mov    $0x98,%r8d
-   180007cfc:	add    $0x8,%rax
-   180007d00:	mov    %rax,0x88(%rbp)
-   180007d07:	call   0x180007fe6
-   180007d0c:	mov    0x4c8(%rbp),%rax
-   180007d13:	mov    %rax,0x60(%rsp)
-   180007d18:	movl   $0x40000015,0x50(%rsp)
-   180007d20:	movl   $0x1,0x54(%rsp)
-   180007d28:	call   *0x1312(%rip)        # 0x180009040
-   180007d2e:	cmp    $0x1,%eax
-   180007d31:	lea    0x50(%rsp),%rax
-   180007d36:	mov    %rax,0x40(%rsp)
-   180007d3b:	lea    -0x10(%rbp),%rax
-   180007d3f:	sete   %bl
-   180007d42:	mov    %rax,0x48(%rsp)
-   180007d47:	xor    %ecx,%ecx
-   180007d49:	call   *0x1339(%rip)        # 0x180009088
-   180007d4f:	lea    0x40(%rsp),%rcx
-   180007d54:	call   *0x1336(%rip)        # 0x180009090
-   180007d5a:	test   %eax,%eax
-   180007d5c:	jne    0x180007d6a
-   180007d5e:	test   %bl,%bl
-   180007d60:	jne    0x180007d6a
-   180007d62:	lea    0x3(%rax),%ecx
-   180007d65:	call   0x180007c28
-   180007d6a:	mov    0x5d0(%rsp),%rbx
-   180007d72:	add    $0x5c0,%rsp
-   180007d79:	pop    %rbp
-   180007d7a:	ret
-   180007d7b:	int3
-   180007d7c:	mov    %rbx,0x8(%rsp)
-   180007d81:	push   %rdi
-   180007d82:	sub    $0x20,%rsp
-   180007d86:	lea    0x2cab(%rip),%rbx        # 0x18000aa38
-   180007d8d:	lea    0x2ca4(%rip),%rdi        # 0x18000aa38
-   180007d94:	jmp    0x180007da8
-   180007d96:	mov    (%rbx),%rax
-   180007d99:	test   %rax,%rax
-   180007d9c:	je     0x180007da4
-   180007d9e:	call   *0x16dc(%rip)        # 0x180009480
-   180007da4:	add    $0x8,%rbx
-   180007da8:	cmp    %rdi,%rbx
-   180007dab:	jb     0x180007d96
-   180007dad:	mov    0x30(%rsp),%rbx
-   180007db2:	add    $0x20,%rsp
-   180007db6:	pop    %rdi
-   180007db7:	ret
-   180007db8:	mov    %rbx,0x8(%rsp)
-   180007dbd:	push   %rdi
-   180007dbe:	sub    $0x20,%rsp
-   180007dc2:	lea    0x2c7f(%rip),%rbx        # 0x18000aa48
-   180007dc9:	lea    0x2c78(%rip),%rdi        # 0x18000aa48
-   180007dd0:	jmp    0x180007de4
-   180007dd2:	mov    (%rbx),%rax
-   180007dd5:	test   %rax,%rax
-   180007dd8:	je     0x180007de0
-   180007dda:	call   *0x16a0(%rip)        # 0x180009480
-   180007de0:	add    $0x8,%rbx
-   180007de4:	cmp    %rdi,%rbx
-   180007de7:	jb     0x180007dd2
-   180007de9:	mov    0x30(%rsp),%rbx
-   180007dee:	add    $0x20,%rsp
-   180007df2:	pop    %rdi
-   180007df3:	ret
-   180007df4:	mov    %rbx,0x10(%rsp)
-   180007df9:	mov    %rsi,0x18(%rsp)
-   180007dfe:	push   %rdi
-   180007dff:	sub    $0x10,%rsp
-   180007e03:	xor    %eax,%eax
-   180007e05:	xor    %ecx,%ecx
-   180007e07:	cpuid
-   180007e09:	mov    %ecx,%r8d
-   180007e0c:	xor    %r11d,%r11d
-   180007e0f:	mov    %ebx,%r9d
-   180007e12:	xor    $0x6c65746e,%r8d
-   180007e19:	xor    $0x756e6547,%r9d
-   180007e20:	mov    %edx,%r10d
-   180007e23:	mov    %eax,%esi
-   180007e25:	xor    %ecx,%ecx
-   180007e27:	lea    0x1(%r11),%eax
-   180007e2b:	or     %r8d,%r9d
-   180007e2e:	cpuid
-   180007e30:	xor    $0x49656e69,%r10d
-   180007e37:	mov    %eax,(%rsp)
-   180007e3a:	or     %r10d,%r9d
-   180007e3d:	mov    %ebx,0x4(%rsp)
-   180007e41:	mov    %ecx,%edi
-   180007e43:	mov    %ecx,0x8(%rsp)
-   180007e47:	mov    %edx,0xc(%rsp)
-   180007e4b:	jne    0x180007e9d
-   180007e4d:	orq    $0xffffffffffffffff,0x61cb(%rip)        # 0x18000e020
-   180007e55:	and    $0xfff3ff0,%eax
-   180007e5a:	cmp    $0x106c0,%eax
-   180007e5f:	je     0x180007e89
-   180007e61:	cmp    $0x20660,%eax
-   180007e66:	je     0x180007e89
-   180007e68:	cmp    $0x20670,%eax
-   180007e6d:	je     0x180007e89
-   180007e6f:	add    $0xfffcf9b0,%eax
-   180007e74:	cmp    $0x20,%eax
-   180007e77:	ja     0x180007e9d
-   180007e79:	movabs $0x100010001,%rcx
-   180007e83:	bt     %rax,%rcx
-   180007e87:	jae    0x180007e9d
-   180007e89:	mov    0x6db4(%rip),%r8d        # 0x18000ec44
-   180007e90:	or     $0x1,%r8d
-   180007e94:	mov    %r8d,0x6da9(%rip)        # 0x18000ec44
-   180007e9b:	jmp    0x180007ea4
-   180007e9d:	mov    0x6da0(%rip),%r8d        # 0x18000ec44
-   180007ea4:	mov    $0x7,%eax
-   180007ea9:	lea    -0x5(%rax),%r9d
-   180007ead:	cmp    %eax,%esi
-   180007eaf:	jl     0x180007ed7
-   180007eb1:	xor    %ecx,%ecx
-   180007eb3:	cpuid
-   180007eb5:	mov    %eax,(%rsp)
-   180007eb8:	mov    %ebx,%r11d
-   180007ebb:	mov    %ebx,0x4(%rsp)
-   180007ebf:	mov    %ecx,0x8(%rsp)
-   180007ec3:	mov    %edx,0xc(%rsp)
-   180007ec7:	bt     $0x9,%ebx
-   180007ecb:	jae    0x180007ed7
-   180007ecd:	or     %r9d,%r8d
-   180007ed0:	mov    %r8d,0x6d6d(%rip)        # 0x18000ec44
-   180007ed7:	movl   $0x1,0x6137(%rip)        # 0x18000e018
-   180007ee1:	mov    %r9d,0x6134(%rip)        # 0x18000e01c
-   180007ee8:	bt     $0x14,%edi
-   180007eec:	jae    0x180007f83
-   180007ef2:	mov    %r9d,0x611f(%rip)        # 0x18000e018
-   180007ef9:	mov    $0x6,%ebx
-   180007efe:	mov    %ebx,0x6118(%rip)        # 0x18000e01c
-   180007f04:	bt     $0x1b,%edi
-   180007f08:	jae    0x180007f83
-   180007f0a:	bt     $0x1c,%edi
-   180007f0e:	jae    0x180007f83
-   180007f10:	xor    %ecx,%ecx
-   180007f12:	xgetbv
-   180007f15:	shl    $0x20,%rdx
-   180007f19:	or     %rax,%rdx
-   180007f1c:	mov    %rdx,0x20(%rsp)
-   180007f21:	mov    0x20(%rsp),%rax
-   180007f26:	and    %bl,%al
-   180007f28:	cmp    %bl,%al
-   180007f2a:	jne    0x180007f83
-   180007f2c:	mov    0x60ea(%rip),%eax        # 0x18000e01c
-   180007f32:	or     $0x8,%eax
-   180007f35:	movl   $0x3,0x60d9(%rip)        # 0x18000e018
-   180007f3f:	mov    %eax,0x60d7(%rip)        # 0x18000e01c
-   180007f45:	test   $0x20,%r11b
-   180007f49:	je     0x180007f83
-   180007f4b:	or     $0x20,%eax
-   180007f4e:	movl   $0x5,0x60c0(%rip)        # 0x18000e018
-   180007f58:	mov    %eax,0x60be(%rip)        # 0x18000e01c
-   180007f5e:	mov    $0xd0030000,%eax
-   180007f63:	and    %eax,%r11d
-   180007f66:	cmp    %eax,%r11d
-   180007f69:	jne    0x180007f83
-   180007f6b:	mov    0x20(%rsp),%rax
-   180007f70:	and    $0xe0,%al
-   180007f72:	cmp    $0xe0,%al
-   180007f74:	jne    0x180007f83
-   180007f76:	orl    $0x40,0x609f(%rip)        # 0x18000e01c
-   180007f7d:	mov    %ebx,0x6095(%rip)        # 0x18000e018
-   180007f83:	mov    0x28(%rsp),%rbx
-   180007f88:	xor    %eax,%eax
-   180007f8a:	mov    0x30(%rsp),%rsi
-   180007f8f:	add    $0x10,%rsp
-   180007f93:	pop    %rdi
-   180007f94:	ret
-   180007f95:	int3
-   180007f96:	int3
-   180007f97:	int3
-   180007f98:	mov    $0x1,%eax
-   180007f9d:	ret
-   180007f9e:	int3
-   180007f9f:	int3
-   180007fa0:	xor    %eax,%eax
-   180007fa2:	cmp    %eax,0x6088(%rip)        # 0x18000e030
-   180007fa8:	setne  %al
-   180007fab:	ret
-   180007fac:	int3
-   180007fad:	int3
-   180007fae:	int3
-   180007faf:	int3
-   180007fb0:	jmp    *0x137a(%rip)        # 0x180009330
-   180007fb6:	jmp    *0x134c(%rip)        # 0x180009308
-   180007fbc:	jmp    *0x133e(%rip)        # 0x180009300
-   180007fc2:	jmp    *0x1330(%rip)        # 0x1800092f8
-   180007fc8:	jmp    *0x1322(%rip)        # 0x1800092f0
-   180007fce:	jmp    *0x1314(%rip)        # 0x1800092e8
-   180007fd4:	jmp    *0x1306(%rip)        # 0x1800092e0
-   180007fda:	jmp    *0x12f8(%rip)        # 0x1800092d8
-   180007fe0:	jmp    *0x133a(%rip)        # 0x180009320
-   180007fe6:	jmp    *0x12e4(%rip)        # 0x1800092d0
-   180007fec:	jmp    *0x1326(%rip)        # 0x180009318
-   180007ff2:	jmp    *0x1318(%rip)        # 0x180009310
-   180007ff8:	jmp    *0x12c2(%rip)        # 0x1800092c0
-   180007ffe:	jmp    *0x12c4(%rip)        # 0x1800092c8
-   180008004:	jmp    *0x1386(%rip)        # 0x180009390
-   18000800a:	jmp    *0x13e8(%rip)        # 0x1800093f8
-   180008010:	jmp    *0x135a(%rip)        # 0x180009370
-   180008016:	jmp    *0x135c(%rip)        # 0x180009378
-   18000801c:	jmp    *0x139e(%rip)        # 0x1800093c0
-   180008022:	jmp    *0x13c8(%rip)        # 0x1800093f0
-   180008028:	jmp    *0x13b2(%rip)        # 0x1800093e0
-   18000802e:	jmp    *0x1394(%rip)        # 0x1800093c8
-   180008034:	jmp    *0x139e(%rip)        # 0x1800093d8
-   18000803a:	jmp    *0x13a8(%rip)        # 0x1800093e8
-   180008040:	jmp    *0x136a(%rip)        # 0x1800093b0
-   180008046:	jmp    *0x1384(%rip)        # 0x1800093d0
-   18000804c:	jmp    *0x134e(%rip)        # 0x1800093a0
-   180008052:	jmp    *0x1350(%rip)        # 0x1800093a8
-   180008058:	jmp    *0x1322(%rip)        # 0x180009380
-   18000805e:	int3
-   18000805f:	int3
-   180008060:	int3
-   180008061:	int3
-   180008062:	int3
-   180008063:	int3
-   180008064:	int3
-   180008065:	int3
-   180008066:	data16 nopw 0x0(%rax,%rax,1)
-   180008070:	jmp    *%rax
-   180008072:	int3
-   180008073:	int3
-   180008074:	int3
-   180008075:	int3
-   180008076:	int3
-   180008077:	int3
-   180008078:	int3
-   180008079:	int3
-   18000807a:	int3
-   18000807b:	int3
-   18000807c:	int3
-   18000807d:	int3
-   18000807e:	int3
-   18000807f:	int3
-   180008080:	int3
-   180008081:	int3
-   180008082:	int3
-   180008083:	int3
-   180008084:	int3
-   180008085:	int3
-   180008086:	data16 nopw 0x0(%rax,%rax,1)
-   180008090:	jmp    *0x13ea(%rip)        # 0x180009480
-   180008096:	int3
-   180008097:	int3
-   180008098:	int3
-   180008099:	int3
-   18000809a:	int3
-   18000809b:	int3
-   18000809c:	int3
-   18000809d:	int3
-   18000809e:	int3
-   18000809f:	int3
-   1800080a0:	rex push %rbp
-   1800080a2:	sub    $0x20,%rsp
-   1800080a6:	mov    %rdx,%rbp
-   1800080a9:	mov    $0x18,%edx
-   1800080ae:	mov    0x40(%rbp),%rcx
-   1800080b2:	call   0x1800070f8
-   1800080b7:	add    $0x20,%rsp
-   1800080bb:	pop    %rbp
-   1800080bc:	ret
-   1800080bd:	int3
-   1800080be:	int3
-   1800080bf:	int3
-   1800080c0:	lea    0x20(%rdx),%rcx
-   1800080c7:	jmp    0x180003260
-   1800080cc:	int3
-   1800080cd:	int3
-   1800080ce:	int3
-   1800080cf:	int3
-   1800080d0:	lea    0x20(%rdx),%rcx
-   1800080d7:	jmp    0x180003200
-   1800080dc:	int3
-   1800080dd:	int3
-   1800080de:	int3
-   1800080df:	int3
-   1800080e0:	mov    %rdx,0x10(%rsp)
-   1800080e5:	push   %rbp
-   1800080e6:	sub    $0x20,%rsp
-   1800080ea:	mov    %rdx,%rbp
-   1800080ed:	mov    0x60(%rbp),%rdx
-   1800080f1:	mov    (%rdx),%rax
-   1800080f4:	movslq 0x4(%rax),%rcx
-   1800080f8:	add    %rdx,%rcx
-   1800080fb:	mov    $0x1,%r8b
-   1800080fe:	mov    $0x4,%edx
-   180008103:	call   *0xff7(%rip)        # 0x180009100
-   180008109:	nop
-   18000810a:	movabs $0x0,%rax
-   180008114:	add    $0x20,%rsp
-   180008118:	pop    %rbp
-   180008119:	ret
-   18000811a:	int3
-   18000811b:	int3
-   18000811c:	int3
-   18000811d:	int3
-   18000811e:	int3
-   18000811f:	int3
-   180008120:	mov    %rdx,0x10(%rsp)
-   180008125:	push   %rbp
-   180008126:	sub    $0x20,%rsp
-   18000812a:	mov    %rdx,%rbp
-   18000812d:	xor    %edx,%edx
-   18000812f:	xor    %ecx,%ecx
-   180008131:	call   0x180007fd4
-   180008136:	nop
-   180008137:	int3
-   180008138:	int3
-   180008139:	int3
-   18000813a:	int3
-   18000813b:	int3
-   18000813c:	int3
-   18000813d:	int3
-   18000813e:	int3
-   18000813f:	int3
-   180008140:	mov    %rdx,0x10(%rsp)
-   180008145:	push   %rbp
-   180008146:	sub    $0x20,%rsp
-   18000814a:	mov    %rdx,%rbp
-   18000814d:	mov    0x68(%rbp),%r8
-   180008151:	mov    0x78(%rbp),%rdx
-   180008155:	mov    0x60(%rbp),%rcx
-   180008159:	call   0x1800046f0
-   18000815e:	xor    %edx,%edx
-   180008160:	xor    %ecx,%ecx
-   180008162:	call   0x180007fd4
-   180008167:	nop
-   180008168:	int3
-   180008169:	int3
-   18000816a:	int3
-   18000816b:	int3
-   18000816c:	int3
-   18000816d:	int3
-   18000816e:	int3
-   18000816f:	int3
-   180008170:	mov    %rdx,0x10(%rsp)
-   180008175:	push   %rbp
-   180008176:	sub    $0x20,%rsp
-   18000817a:	mov    %rdx,%rbp
-   18000817d:	mov    0x78(%rbp),%r8
-   180008181:	mov    0x20(%rbp),%rdx
-   180008185:	mov    0x70(%rbp),%rcx
-   180008189:	call   0x180004740
-   18000818e:	xor    %edx,%edx
-   180008190:	xor    %ecx,%ecx
-   180008192:	call   0x180007fd4
-   180008197:	nop
-   180008198:	int3
-   180008199:	int3
-   18000819a:	int3
-   18000819b:	int3
-   18000819c:	int3
-   18000819d:	int3
-   18000819e:	int3
-   18000819f:	int3
-   1800081a0:	mov    %rdx,0x10(%rsp)
-   1800081a5:	push   %rbp
-   1800081a6:	sub    $0x20,%rsp
-   1800081aa:	mov    %rdx,%rbp
-   1800081ad:	mov    0x40(%rbp),%rcx
-   1800081b1:	call   0x1800037f0
-   1800081b6:	mov    %rax,%rcx
-   1800081b9:	mov    0x48(%rbp),%r8
-   1800081bd:	mov    0x58(%rbp),%rdx
-   1800081c1:	call   0x180004780
-   1800081c6:	xor    %edx,%edx
-   1800081c8:	xor    %ecx,%ecx
-   1800081ca:	call   0x180007fd4
-   1800081cf:	nop
-   1800081d0:	mov    %rdx,0x10(%rsp)
-   1800081d5:	push   %rbp
-   1800081d6:	sub    $0x20,%rsp
-   1800081da:	mov    %rdx,%rbp
-   1800081dd:	mov    0x50(%rbp),%rcx
-   1800081e1:	call   0x1800037f0
-   1800081e6:	mov    %rax,%rcx
-   1800081e9:	mov    0x58(%rbp),%r8
-   1800081ed:	mov    0x68(%rbp),%rdx
-   1800081f1:	call   0x180004780
-   1800081f6:	xor    %edx,%edx
-   1800081f8:	xor    %ecx,%ecx
-   1800081fa:	call   0x180007fd4
-   1800081ff:	nop
-   180008200:	lea    0x40(%rdx),%rcx
-   180008207:	jmp    0x180002de0
-   18000820c:	int3
-   18000820d:	int3
-   18000820e:	int3
-   18000820f:	int3
-   180008210:	rex push %rbp
-   180008212:	sub    $0x20,%rsp
-   180008216:	mov    %rdx,%rbp
-   180008219:	mov    0x30(%rbp),%eax
-   18000821c:	and    $0x1,%eax
-   18000821f:	test   %eax,%eax
-   180008221:	je     0x180008233
-   180008223:	andl   $0xfffffffe,0x30(%rbp)
-   180008227:	mov    0xd8(%rbp),%rcx
-   18000822e:	call   0x180002de0
-   180008233:	add    $0x20,%rsp
-   180008237:	pop    %rbp
-   180008238:	ret
-   180008239:	int3
-   18000823a:	int3
-   18000823b:	int3
-   18000823c:	int3
-   18000823d:	int3
-   18000823e:	int3
-   18000823f:	int3
-   180008240:	rex push %rbp
-   180008242:	sub    $0x20,%rsp
-   180008246:	mov    %rdx,%rbp
-   180008249:	mov    $0x70,%edx
-   18000824e:	mov    0xe0(%rbp),%rcx
-   180008255:	call   0x1800070f8
-   18000825a:	add    $0x20,%rsp
-   18000825e:	pop    %rbp
-   18000825f:	ret
-   180008260:	mov    0xe0(%rdx),%rcx
-   180008267:	jmp    0x180002c70
+   180007c20:	andq   $0x0,0x10(%rcx)
+   180007c25:	lea    0x1dac(%rip),%rax        # 0x1800099d8
+   180007c2c:	mov    %rax,0x8(%rcx)
+   180007c30:	lea    0x1921(%rip),%rax        # 0x180009558
+   180007c37:	mov    %rax,(%rcx)
+   180007c3a:	mov    %rcx,%rax
+   180007c3d:	ret
+   180007c3e:	int3
+   180007c3f:	int3
+   180007c40:	sub    $0x48,%rsp
+   180007c44:	lea    0x20(%rsp),%rcx
+   180007c49:	call   0x180007c20
+   180007c4e:	lea    0x3bab(%rip),%rdx        # 0x18000b800
+   180007c55:	lea    0x20(%rsp),%rcx
+   180007c5a:	call   0x180008294
+   180007c5f:	int3
+   180007c60:	jmp    0x180008318
+   180007c65:	int3
+   180007c66:	int3
+   180007c67:	int3
+   180007c68:	rex push %rbx
+   180007c6a:	sub    $0x20,%rsp
+   180007c6e:	mov    %rcx,%rbx
+   180007c71:	xor    %ecx,%ecx
+   180007c73:	call   *0x140f(%rip)        # 0x180009088
+   180007c79:	mov    %rbx,%rcx
+   180007c7c:	call   *0x140e(%rip)        # 0x180009090
+   180007c82:	call   *0x13f8(%rip)        # 0x180009080
+   180007c88:	mov    %rax,%rcx
+   180007c8b:	mov    $0xc0000409,%edx
+   180007c90:	add    $0x20,%rsp
+   180007c94:	pop    %rbx
+   180007c95:	rex.W jmp *0x13dc(%rip)        # 0x180009078
+   180007c9c:	mov    %rcx,0x8(%rsp)
+   180007ca1:	sub    $0x38,%rsp
+   180007ca5:	mov    $0x17,%ecx
+   180007caa:	call   *0x13c0(%rip)        # 0x180009070
+   180007cb0:	test   %eax,%eax
+   180007cb2:	je     0x180007cbb
+   180007cb4:	mov    $0x2,%ecx
+   180007cb9:	int    $0x29
+   180007cbb:	lea    0x6a9e(%rip),%rcx        # 0x18000e760
+   180007cc2:	call   0x180007d70
+   180007cc7:	mov    0x38(%rsp),%rax
+   180007ccc:	mov    %rax,0x6b85(%rip)        # 0x18000e858
+   180007cd3:	lea    0x38(%rsp),%rax
+   180007cd8:	add    $0x8,%rax
+   180007cdc:	mov    %rax,0x6b15(%rip)        # 0x18000e7f8
+   180007ce3:	mov    0x6b6e(%rip),%rax        # 0x18000e858
+   180007cea:	mov    %rax,0x69df(%rip)        # 0x18000e6d0
+   180007cf1:	mov    0x40(%rsp),%rax
+   180007cf6:	mov    %rax,0x6ae3(%rip)        # 0x18000e7e0
+   180007cfd:	movl   $0xc0000409,0x69b9(%rip)        # 0x18000e6c0
+   180007d07:	movl   $0x1,0x69b3(%rip)        # 0x18000e6c4
+   180007d11:	movl   $0x1,0x69bd(%rip)        # 0x18000e6d8
+   180007d1b:	mov    $0x8,%eax
+   180007d20:	imul   $0x0,%rax,%rax
+   180007d24:	lea    0x69b5(%rip),%rcx        # 0x18000e6e0
+   180007d2b:	movq   $0x2,(%rcx,%rax,1)
+   180007d33:	mov    $0x8,%eax
+   180007d38:	imul   $0x0,%rax,%rax
+   180007d3c:	mov    0x62c5(%rip),%rcx        # 0x18000e008
+   180007d43:	mov    %rcx,0x20(%rsp,%rax,1)
+   180007d48:	mov    $0x8,%eax
+   180007d4d:	imul   $0x1,%rax,%rax
+   180007d51:	mov    0x62a8(%rip),%rcx        # 0x18000e000
+   180007d58:	mov    %rcx,0x20(%rsp,%rax,1)
+   180007d5d:	lea    0x1c84(%rip),%rcx        # 0x1800099e8
+   180007d64:	call   0x180007c68
+   180007d69:	add    $0x38,%rsp
+   180007d6d:	ret
+   180007d6e:	int3
+   180007d6f:	int3
+   180007d70:	rex push %rbx
+   180007d72:	push   %rsi
+   180007d73:	push   %rdi
+   180007d74:	sub    $0x40,%rsp
+   180007d78:	mov    %rcx,%rbx
+   180007d7b:	call   *0x1327(%rip)        # 0x1800090a8
+   180007d81:	mov    0xf8(%rbx),%rsi
+   180007d88:	xor    %edi,%edi
+   180007d8a:	xor    %r8d,%r8d
+   180007d8d:	lea    0x60(%rsp),%rdx
+   180007d92:	mov    %rsi,%rcx
+   180007d95:	call   *0x1305(%rip)        # 0x1800090a0
+   180007d9b:	test   %rax,%rax
+   180007d9e:	je     0x180007dd9
+   180007da0:	andq   $0x0,0x38(%rsp)
+   180007da6:	lea    0x68(%rsp),%rcx
+   180007dab:	mov    0x60(%rsp),%rdx
+   180007db0:	mov    %rax,%r9
+   180007db3:	mov    %rcx,0x30(%rsp)
+   180007db8:	mov    %rsi,%r8
+   180007dbb:	lea    0x70(%rsp),%rcx
+   180007dc0:	mov    %rcx,0x28(%rsp)
+   180007dc5:	xor    %ecx,%ecx
+   180007dc7:	mov    %rbx,0x20(%rsp)
+   180007dcc:	call   *0x12c6(%rip)        # 0x180009098
+   180007dd2:	inc    %edi
+   180007dd4:	cmp    $0x2,%edi
+   180007dd7:	jl     0x180007d8a
+   180007dd9:	add    $0x40,%rsp
+   180007ddd:	pop    %rdi
+   180007dde:	pop    %rsi
+   180007ddf:	pop    %rbx
+   180007de0:	ret
+   180007de1:	int3
+   180007de2:	int3
+   180007de3:	int3
+   180007de4:	mov    %rbx,0x20(%rsp)
+   180007de9:	push   %rbp
+   180007dea:	mov    %rsp,%rbp
+   180007ded:	sub    $0x20,%rsp
+   180007df1:	mov    0x6210(%rip),%rax        # 0x18000e008
+   180007df8:	movabs $0x2b992ddfa232,%rbx
+   180007e02:	cmp    %rbx,%rax
+   180007e05:	jne    0x180007e7b
+   180007e07:	andq   $0x0,0x18(%rbp)
+   180007e0c:	lea    0x18(%rbp),%rcx
+   180007e10:	call   *0x123a(%rip)        # 0x180009050
+   180007e16:	mov    0x18(%rbp),%rax
+   180007e1a:	mov    %rax,0x10(%rbp)
+   180007e1e:	call   *0x1234(%rip)        # 0x180009058
+   180007e24:	mov    %eax,%eax
+   180007e26:	xor    %rax,0x10(%rbp)
+   180007e2a:	call   *0x1230(%rip)        # 0x180009060
+   180007e30:	mov    %eax,%eax
+   180007e32:	lea    0x20(%rbp),%rcx
+   180007e36:	xor    %rax,0x10(%rbp)
+   180007e3a:	call   *0x1228(%rip)        # 0x180009068
+   180007e40:	mov    0x20(%rbp),%eax
+   180007e43:	lea    0x10(%rbp),%rcx
+   180007e47:	shl    $0x20,%rax
+   180007e4b:	xor    0x20(%rbp),%rax
+   180007e4f:	xor    0x10(%rbp),%rax
+   180007e53:	xor    %rcx,%rax
+   180007e56:	movabs $0xffffffffffff,%rcx
+   180007e60:	and    %rcx,%rax
+   180007e63:	movabs $0x2b992ddfa233,%rcx
+   180007e6d:	cmp    %rbx,%rax
+   180007e70:	cmove  %rcx,%rax
+   180007e74:	mov    %rax,0x618d(%rip)        # 0x18000e008
+   180007e7b:	mov    0x48(%rsp),%rbx
+   180007e80:	not    %rax
+   180007e83:	mov    %rax,0x6176(%rip)        # 0x18000e000
+   180007e8a:	add    $0x20,%rsp
+   180007e8e:	pop    %rbp
+   180007e8f:	ret
+   180007e90:	sub    $0x28,%rsp
+   180007e94:	cmp    $0x1,%edx
+   180007e97:	jne    0x180007ea9
+   180007e99:	cmpq   $0x0,0x1b2f(%rip)        # 0x1800099d0
+   180007ea1:	jne    0x180007ea9
+   180007ea3:	call   *0x119f(%rip)        # 0x180009048
+   180007ea9:	mov    $0x1,%eax
+   180007eae:	add    $0x28,%rsp
+   180007eb2:	ret
+   180007eb3:	int3
+   180007eb4:	lea    0x6d75(%rip),%rax        # 0x18000ec30
+   180007ebb:	ret
+   180007ebc:	lea    0x6d75(%rip),%rax        # 0x18000ec38
+   180007ec3:	ret
+   180007ec4:	sub    $0x28,%rsp
+   180007ec8:	call   0x180007eb4
+   180007ecd:	orq    $0x24,(%rax)
+   180007ed1:	call   0x180007ebc
+   180007ed6:	orq    $0x2,(%rax)
+   180007eda:	add    $0x28,%rsp
+   180007ede:	ret
+   180007edf:	int3
+   180007ee0:	lea    0x6d61(%rip),%rax        # 0x18000ec48
+   180007ee7:	ret
+   180007ee8:	andl   $0x0,0x6d51(%rip)        # 0x18000ec40
+   180007eef:	ret
+   180007ef0:	mov    %rbx,0x8(%rsp)
+   180007ef5:	push   %rbp
+   180007ef6:	lea    -0x4c0(%rsp),%rbp
+   180007efe:	sub    $0x5c0,%rsp
+   180007f05:	mov    %ecx,%ebx
+   180007f07:	mov    $0x17,%ecx
+   180007f0c:	call   *0x115e(%rip)        # 0x180009070
+   180007f12:	test   %eax,%eax
+   180007f14:	je     0x180007f1a
+   180007f16:	mov    %ebx,%ecx
+   180007f18:	int    $0x29
+   180007f1a:	mov    $0x3,%ecx
+   180007f1f:	call   0x180007ee8
+   180007f24:	xor    %edx,%edx
+   180007f26:	lea    -0x10(%rbp),%rcx
+   180007f2a:	mov    $0x4d0,%r8d
+   180007f30:	call   0x1800082a6
+   180007f35:	lea    -0x10(%rbp),%rcx
+   180007f39:	call   *0x1169(%rip)        # 0x1800090a8
+   180007f3f:	mov    0xe8(%rbp),%rbx
+   180007f46:	lea    0x4d8(%rbp),%rdx
+   180007f4d:	mov    %rbx,%rcx
+   180007f50:	xor    %r8d,%r8d
+   180007f53:	call   *0x1147(%rip)        # 0x1800090a0
+   180007f59:	test   %rax,%rax
+   180007f5c:	je     0x180007f9a
+   180007f5e:	andq   $0x0,0x38(%rsp)
+   180007f64:	lea    0x4e0(%rbp),%rcx
+   180007f6b:	mov    0x4d8(%rbp),%rdx
+   180007f72:	mov    %rax,%r9
+   180007f75:	mov    %rcx,0x30(%rsp)
+   180007f7a:	mov    %rbx,%r8
+   180007f7d:	lea    0x4e8(%rbp),%rcx
+   180007f84:	mov    %rcx,0x28(%rsp)
+   180007f89:	lea    -0x10(%rbp),%rcx
+   180007f8d:	mov    %rcx,0x20(%rsp)
+   180007f92:	xor    %ecx,%ecx
+   180007f94:	call   *0x10fe(%rip)        # 0x180009098
+   180007f9a:	mov    0x4c8(%rbp),%rax
+   180007fa1:	lea    0x50(%rsp),%rcx
+   180007fa6:	mov    %rax,0xe8(%rbp)
+   180007fad:	xor    %edx,%edx
+   180007faf:	lea    0x4c8(%rbp),%rax
+   180007fb6:	mov    $0x98,%r8d
+   180007fbc:	add    $0x8,%rax
+   180007fc0:	mov    %rax,0x88(%rbp)
+   180007fc7:	call   0x1800082a6
+   180007fcc:	mov    0x4c8(%rbp),%rax
+   180007fd3:	mov    %rax,0x60(%rsp)
+   180007fd8:	movl   $0x40000015,0x50(%rsp)
+   180007fe0:	movl   $0x1,0x54(%rsp)
+   180007fe8:	call   *0x1052(%rip)        # 0x180009040
+   180007fee:	cmp    $0x1,%eax
+   180007ff1:	lea    0x50(%rsp),%rax
+   180007ff6:	mov    %rax,0x40(%rsp)
+   180007ffb:	lea    -0x10(%rbp),%rax
+   180007fff:	sete   %bl
+   180008002:	mov    %rax,0x48(%rsp)
+   180008007:	xor    %ecx,%ecx
+   180008009:	call   *0x1079(%rip)        # 0x180009088
+   18000800f:	lea    0x40(%rsp),%rcx
+   180008014:	call   *0x1076(%rip)        # 0x180009090
+   18000801a:	test   %eax,%eax
+   18000801c:	jne    0x18000802a
+   18000801e:	test   %bl,%bl
+   180008020:	jne    0x18000802a
+   180008022:	lea    0x3(%rax),%ecx
+   180008025:	call   0x180007ee8
+   18000802a:	mov    0x5d0(%rsp),%rbx
+   180008032:	add    $0x5c0,%rsp
+   180008039:	pop    %rbp
+   18000803a:	ret
+   18000803b:	int3
+   18000803c:	mov    %rbx,0x8(%rsp)
+   180008041:	push   %rdi
+   180008042:	sub    $0x20,%rsp
+   180008046:	lea    0x29eb(%rip),%rbx        # 0x18000aa38
+   18000804d:	lea    0x29e4(%rip),%rdi        # 0x18000aa38
+   180008054:	jmp    0x180008068
+   180008056:	mov    (%rbx),%rax
+   180008059:	test   %rax,%rax
+   18000805c:	je     0x180008064
+   18000805e:	call   *0x141c(%rip)        # 0x180009480
+   180008064:	add    $0x8,%rbx
+   180008068:	cmp    %rdi,%rbx
+   18000806b:	jb     0x180008056
+   18000806d:	mov    0x30(%rsp),%rbx
+   180008072:	add    $0x20,%rsp
+   180008076:	pop    %rdi
+   180008077:	ret
+   180008078:	mov    %rbx,0x8(%rsp)
+   18000807d:	push   %rdi
+   18000807e:	sub    $0x20,%rsp
+   180008082:	lea    0x29bf(%rip),%rbx        # 0x18000aa48
+   180008089:	lea    0x29b8(%rip),%rdi        # 0x18000aa48
+   180008090:	jmp    0x1800080a4
+   180008092:	mov    (%rbx),%rax
+   180008095:	test   %rax,%rax
+   180008098:	je     0x1800080a0
+   18000809a:	call   *0x13e0(%rip)        # 0x180009480
+   1800080a0:	add    $0x8,%rbx
+   1800080a4:	cmp    %rdi,%rbx
+   1800080a7:	jb     0x180008092
+   1800080a9:	mov    0x30(%rsp),%rbx
+   1800080ae:	add    $0x20,%rsp
+   1800080b2:	pop    %rdi
+   1800080b3:	ret
+   1800080b4:	mov    %rbx,0x10(%rsp)
+   1800080b9:	mov    %rsi,0x18(%rsp)
+   1800080be:	push   %rdi
+   1800080bf:	sub    $0x10,%rsp
+   1800080c3:	xor    %eax,%eax
+   1800080c5:	xor    %ecx,%ecx
+   1800080c7:	cpuid
+   1800080c9:	mov    %ecx,%r8d
+   1800080cc:	xor    %r11d,%r11d
+   1800080cf:	mov    %ebx,%r9d
+   1800080d2:	xor    $0x6c65746e,%r8d
+   1800080d9:	xor    $0x756e6547,%r9d
+   1800080e0:	mov    %edx,%r10d
+   1800080e3:	mov    %eax,%esi
+   1800080e5:	xor    %ecx,%ecx
+   1800080e7:	lea    0x1(%r11),%eax
+   1800080eb:	or     %r8d,%r9d
+   1800080ee:	cpuid
+   1800080f0:	xor    $0x49656e69,%r10d
+   1800080f7:	mov    %eax,(%rsp)
+   1800080fa:	or     %r10d,%r9d
+   1800080fd:	mov    %ebx,0x4(%rsp)
+   180008101:	mov    %ecx,%edi
+   180008103:	mov    %ecx,0x8(%rsp)
+   180008107:	mov    %edx,0xc(%rsp)
+   18000810b:	jne    0x18000815d
+   18000810d:	orq    $0xffffffffffffffff,0x5f0b(%rip)        # 0x18000e020
+   180008115:	and    $0xfff3ff0,%eax
+   18000811a:	cmp    $0x106c0,%eax
+   18000811f:	je     0x180008149
+   180008121:	cmp    $0x20660,%eax
+   180008126:	je     0x180008149
+   180008128:	cmp    $0x20670,%eax
+   18000812d:	je     0x180008149
+   18000812f:	add    $0xfffcf9b0,%eax
+   180008134:	cmp    $0x20,%eax
+   180008137:	ja     0x18000815d
+   180008139:	movabs $0x100010001,%rcx
+   180008143:	bt     %rax,%rcx
+   180008147:	jae    0x18000815d
+   180008149:	mov    0x6af4(%rip),%r8d        # 0x18000ec44
+   180008150:	or     $0x1,%r8d
+   180008154:	mov    %r8d,0x6ae9(%rip)        # 0x18000ec44
+   18000815b:	jmp    0x180008164
+   18000815d:	mov    0x6ae0(%rip),%r8d        # 0x18000ec44
+   180008164:	mov    $0x7,%eax
+   180008169:	lea    -0x5(%rax),%r9d
+   18000816d:	cmp    %eax,%esi
+   18000816f:	jl     0x180008197
+   180008171:	xor    %ecx,%ecx
+   180008173:	cpuid
+   180008175:	mov    %eax,(%rsp)
+   180008178:	mov    %ebx,%r11d
+   18000817b:	mov    %ebx,0x4(%rsp)
+   18000817f:	mov    %ecx,0x8(%rsp)
+   180008183:	mov    %edx,0xc(%rsp)
+   180008187:	bt     $0x9,%ebx
+   18000818b:	jae    0x180008197
+   18000818d:	or     %r9d,%r8d
+   180008190:	mov    %r8d,0x6aad(%rip)        # 0x18000ec44
+   180008197:	movl   $0x1,0x5e77(%rip)        # 0x18000e018
+   1800081a1:	mov    %r9d,0x5e74(%rip)        # 0x18000e01c
+   1800081a8:	bt     $0x14,%edi
+   1800081ac:	jae    0x180008243
+   1800081b2:	mov    %r9d,0x5e5f(%rip)        # 0x18000e018
+   1800081b9:	mov    $0x6,%ebx
+   1800081be:	mov    %ebx,0x5e58(%rip)        # 0x18000e01c
+   1800081c4:	bt     $0x1b,%edi
+   1800081c8:	jae    0x180008243
+   1800081ca:	bt     $0x1c,%edi
+   1800081ce:	jae    0x180008243
+   1800081d0:	xor    %ecx,%ecx
+   1800081d2:	xgetbv
+   1800081d5:	shl    $0x20,%rdx
+   1800081d9:	or     %rax,%rdx
+   1800081dc:	mov    %rdx,0x20(%rsp)
+   1800081e1:	mov    0x20(%rsp),%rax
+   1800081e6:	and    %bl,%al
+   1800081e8:	cmp    %bl,%al
+   1800081ea:	jne    0x180008243
+   1800081ec:	mov    0x5e2a(%rip),%eax        # 0x18000e01c
+   1800081f2:	or     $0x8,%eax
+   1800081f5:	movl   $0x3,0x5e19(%rip)        # 0x18000e018
+   1800081ff:	mov    %eax,0x5e17(%rip)        # 0x18000e01c
+   180008205:	test   $0x20,%r11b
+   180008209:	je     0x180008243
+   18000820b:	or     $0x20,%eax
+   18000820e:	movl   $0x5,0x5e00(%rip)        # 0x18000e018
+   180008218:	mov    %eax,0x5dfe(%rip)        # 0x18000e01c
+   18000821e:	mov    $0xd0030000,%eax
+   180008223:	and    %eax,%r11d
+   180008226:	cmp    %eax,%r11d
+   180008229:	jne    0x180008243
+   18000822b:	mov    0x20(%rsp),%rax
+   180008230:	and    $0xe0,%al
+   180008232:	cmp    $0xe0,%al
+   180008234:	jne    0x180008243
+   180008236:	orl    $0x40,0x5ddf(%rip)        # 0x18000e01c
+   18000823d:	mov    %ebx,0x5dd5(%rip)        # 0x18000e018
+   180008243:	mov    0x28(%rsp),%rbx
+   180008248:	xor    %eax,%eax
+   18000824a:	mov    0x30(%rsp),%rsi
+   18000824f:	add    $0x10,%rsp
+   180008253:	pop    %rdi
+   180008254:	ret
+   180008255:	int3
+   180008256:	int3
+   180008257:	int3
+   180008258:	mov    $0x1,%eax
+   18000825d:	ret
+   18000825e:	int3
+   18000825f:	int3
+   180008260:	xor    %eax,%eax
+   180008262:	cmp    %eax,0x5dc8(%rip)        # 0x18000e030
+   180008268:	setne  %al
+   18000826b:	ret
    18000826c:	int3
    18000826d:	int3
    18000826e:	int3
    18000826f:	int3
-   180008270:	mov    0xe0(%rdx),%rcx
-   180008277:	add    $0x58,%rcx
-   18000827b:	jmp    0x180002eb0
-   180008280:	lea    0xe0(%rdx),%rcx
-   180008287:	jmp    0x180002c80
-   18000828c:	int3
-   18000828d:	int3
-   18000828e:	int3
-   18000828f:	int3
-   180008290:	lea    0x40(%rdx),%rcx
-   180008297:	jmp    0x180002ca0
-   18000829c:	int3
-   18000829d:	int3
-   18000829e:	int3
-   18000829f:	int3
-   1800082a0:	lea    0x40(%rdx),%rcx
-   1800082a7:	rex.W jmp *0xe9a(%rip)        # 0x180009148
-   1800082ae:	int3
-   1800082af:	int3
-   1800082b0:	lea    0x50(%rdx),%rcx
-   1800082b7:	jmp    0x180002c80
-   1800082bc:	int3
-   1800082bd:	int3
-   1800082be:	int3
-   1800082bf:	int3
-   1800082c0:	mov    0x30(%rdx),%rcx
-   1800082c7:	jmp    0x180002c20
-   1800082cc:	int3
-   1800082cd:	int3
-   1800082ce:	int3
-   1800082cf:	int3
-   1800082d0:	mov    0xe0(%rdx),%rcx
-   1800082d7:	add    $0x8,%rcx
-   1800082db:	jmp    0x180002c80
-   1800082e0:	mov    0xe0(%rdx),%rcx
-   1800082e7:	add    $0x10,%rcx
-   1800082eb:	jmp    0x180006f3a
-   1800082f0:	mov    0xe0(%rdx),%rcx
-   1800082f7:	add    $0x20,%rcx
-   1800082fb:	jmp    0x180002dd0
-   180008300:	mov    0xe0(%rdx),%rcx
-   180008307:	add    $0x40,%rcx
-   18000830b:	jmp    0x180002de0
-   180008310:	mov    %rdx,0x10(%rsp)
-   180008315:	push   %rbp
-   180008316:	sub    $0x20,%rsp
-   18000831a:	mov    %rdx,%rbp
-   18000831d:	mov    0x40(%rbp),%rcx
-   180008321:	call   0x1800037f0
-   180008326:	mov    %rax,%rcx
-   180008329:	mov    0x48(%rbp),%r8
-   18000832d:	mov    0x50(%rbp),%rdx
-   180008331:	call   0x180004780
-   180008336:	xor    %edx,%edx
-   180008338:	xor    %ecx,%ecx
-   18000833a:	call   0x180007fd4
-   18000833f:	nop
-   180008340:	rex push %rbp
-   180008342:	sub    $0x20,%rsp
-   180008346:	mov    %rdx,%rbp
-   180008349:	mov    $0x70,%edx
-   18000834e:	mov    0x68(%rbp),%rcx
-   180008352:	call   0x1800070f8
-   180008357:	add    $0x20,%rsp
-   18000835b:	pop    %rbp
-   18000835c:	ret
+   180008270:	jmp    *0x10ba(%rip)        # 0x180009330
+   180008276:	jmp    *0x108c(%rip)        # 0x180009308
+   18000827c:	jmp    *0x107e(%rip)        # 0x180009300
+   180008282:	jmp    *0x1070(%rip)        # 0x1800092f8
+   180008288:	jmp    *0x1062(%rip)        # 0x1800092f0
+   18000828e:	jmp    *0x1054(%rip)        # 0x1800092e8
+   180008294:	jmp    *0x1046(%rip)        # 0x1800092e0
+   18000829a:	jmp    *0x1038(%rip)        # 0x1800092d8
+   1800082a0:	jmp    *0x107a(%rip)        # 0x180009320
+   1800082a6:	jmp    *0x1024(%rip)        # 0x1800092d0
+   1800082ac:	jmp    *0x1066(%rip)        # 0x180009318
+   1800082b2:	jmp    *0x1058(%rip)        # 0x180009310
+   1800082b8:	jmp    *0x1002(%rip)        # 0x1800092c0
+   1800082be:	jmp    *0x1004(%rip)        # 0x1800092c8
+   1800082c4:	jmp    *0x10c6(%rip)        # 0x180009390
+   1800082ca:	jmp    *0x1128(%rip)        # 0x1800093f8
+   1800082d0:	jmp    *0x109a(%rip)        # 0x180009370
+   1800082d6:	jmp    *0x109c(%rip)        # 0x180009378
+   1800082dc:	jmp    *0x10de(%rip)        # 0x1800093c0
+   1800082e2:	jmp    *0x1108(%rip)        # 0x1800093f0
+   1800082e8:	jmp    *0x10f2(%rip)        # 0x1800093e0
+   1800082ee:	jmp    *0x10d4(%rip)        # 0x1800093c8
+   1800082f4:	jmp    *0x10de(%rip)        # 0x1800093d8
+   1800082fa:	jmp    *0x10e8(%rip)        # 0x1800093e8
+   180008300:	jmp    *0x10aa(%rip)        # 0x1800093b0
+   180008306:	jmp    *0x10c4(%rip)        # 0x1800093d0
+   18000830c:	jmp    *0x108e(%rip)        # 0x1800093a0
+   180008312:	jmp    *0x1090(%rip)        # 0x1800093a8
+   180008318:	jmp    *0x1062(%rip)        # 0x180009380
+   18000831e:	int3
+   18000831f:	int3
+   180008320:	int3
+   180008321:	int3
+   180008322:	int3
+   180008323:	int3
+   180008324:	int3
+   180008325:	int3
+   180008326:	data16 nopw 0x0(%rax,%rax,1)
+   180008330:	jmp    *%rax
+   180008332:	int3
+   180008333:	int3
+   180008334:	int3
+   180008335:	int3
+   180008336:	int3
+   180008337:	int3
+   180008338:	int3
+   180008339:	int3
+   18000833a:	int3
+   18000833b:	int3
+   18000833c:	int3
+   18000833d:	int3
+   18000833e:	int3
+   18000833f:	int3
+   180008340:	int3
+   180008341:	int3
+   180008342:	int3
+   180008343:	int3
+   180008344:	int3
+   180008345:	int3
+   180008346:	data16 nopw 0x0(%rax,%rax,1)
+   180008350:	jmp    *0x112a(%rip)        # 0x180009480
+   180008356:	int3
+   180008357:	int3
+   180008358:	int3
+   180008359:	int3
+   18000835a:	int3
+   18000835b:	int3
+   18000835c:	int3
    18000835d:	int3
    18000835e:	int3
    18000835f:	int3
-   180008360:	lea    0x20(%rdx),%rcx
-   180008367:	jmp    0x180002de0
-   18000836c:	int3
-   18000836d:	int3
-   18000836e:	int3
-   18000836f:	int3
-   180008370:	mov    0x68(%rdx),%rcx
-   180008377:	jmp    0x180002c70
-   18000837c:	int3
+   180008360:	rex push %rbp
+   180008362:	sub    $0x20,%rsp
+   180008366:	mov    %rdx,%rbp
+   180008369:	mov    $0x18,%edx
+   18000836e:	mov    0x40(%rbp),%rcx
+   180008372:	call   0x1800073b8
+   180008377:	add    $0x20,%rsp
+   18000837b:	pop    %rbp
+   18000837c:	ret
    18000837d:	int3
    18000837e:	int3
    18000837f:	int3
-   180008380:	mov    0x68(%rdx),%rcx
-   180008387:	add    $0x58,%rcx
-   18000838b:	jmp    0x180002eb0
-   180008390:	lea    0x68(%rdx),%rcx
-   180008397:	jmp    0x180002c80
+   180008380:	lea    0x20(%rdx),%rcx
+   180008387:	jmp    0x180003260
+   18000838c:	int3
+   18000838d:	int3
+   18000838e:	int3
+   18000838f:	int3
+   180008390:	lea    0x20(%rdx),%rcx
+   180008397:	jmp    0x180003200
    18000839c:	int3
    18000839d:	int3
    18000839e:	int3
    18000839f:	int3
-   1800083a0:	lea    0x130(%rdx),%rcx
-   1800083a7:	jmp    0x180002c20
-   1800083ac:	int3
-   1800083ad:	int3
-   1800083ae:	int3
-   1800083af:	int3
-   1800083b0:	lea    0xd0(%rdx),%rcx
-   1800083b7:	jmp    0x180002c20
-   1800083bc:	int3
-   1800083bd:	int3
-   1800083be:	int3
-   1800083bf:	int3
-   1800083c0:	lea    0x28(%rdx),%rcx
-   1800083c7:	jmp    0x180002ca0
-   1800083cc:	int3
-   1800083cd:	int3
-   1800083ce:	int3
-   1800083cf:	int3
-   1800083d0:	mov    %rdx,0x10(%rsp)
-   1800083d5:	push   %rbp
-   1800083d6:	sub    $0x20,%rsp
-   1800083da:	mov    %rdx,%rbp
-   1800083dd:	mov    0x40(%rbp),%rax
-   1800083e1:	movb   $0x0,(%rax)
-   1800083e4:	xorps  %xmm0,%xmm0
-   1800083e7:	xor    %ecx,%ecx
-   1800083e9:	movups %xmm0,0x8(%rax)
-   1800083ed:	mov    %rcx,0x18(%rax)
-   1800083f1:	movabs $0x0,%rax
-   1800083fb:	add    $0x20,%rsp
-   1800083ff:	pop    %rbp
-   180008400:	ret
-   180008401:	int3
-   180008402:	int3
-   180008403:	int3
-   180008404:	int3
-   180008405:	int3
-   180008406:	int3
-   180008407:	int3
-   180008408:	int3
-   180008409:	int3
-   18000840a:	int3
-   18000840b:	int3
-   18000840c:	int3
-   18000840d:	int3
-   18000840e:	int3
-   18000840f:	int3
-   180008410:	rex push %rbp
-   180008412:	sub    $0x20,%rsp
-   180008416:	mov    %rdx,%rbp
-   180008419:	mov    $0x70,%edx
-   18000841e:	mov    0xb0(%rbp),%rcx
-   180008425:	call   0x1800070f8
-   18000842a:	add    $0x20,%rsp
-   18000842e:	pop    %rbp
-   18000842f:	ret
-   180008430:	lea    0x48(%rdx),%rcx
-   180008437:	jmp    0x180002de0
-   18000843c:	int3
-   18000843d:	int3
-   18000843e:	int3
-   18000843f:	int3
-   180008440:	mov    0xb0(%rdx),%rcx
-   180008447:	jmp    0x180002c70
-   18000844c:	int3
-   18000844d:	int3
-   18000844e:	int3
-   18000844f:	int3
-   180008450:	mov    0xb0(%rdx),%rcx
-   180008457:	add    $0x58,%rcx
-   18000845b:	jmp    0x180002eb0
-   180008460:	lea    0xb0(%rdx),%rcx
-   180008467:	jmp    0x180002c80
-   18000846c:	int3
-   18000846d:	int3
-   18000846e:	int3
-   18000846f:	int3
-   180008470:	rex push %rbp
-   180008472:	sub    $0x20,%rsp
-   180008476:	mov    %rdx,%rbp
-   180008479:	mov    0x20(%rbp),%eax
-   18000847c:	and    $0x1,%eax
-   18000847f:	test   %eax,%eax
-   180008481:	je     0x180008490
-   180008483:	andl   $0xfffffffe,0x20(%rbp)
-   180008487:	mov    0x60(%rbp),%rcx
-   18000848b:	call   0x180002ca0
-   180008490:	add    $0x20,%rsp
-   180008494:	pop    %rbp
-   180008495:	ret
-   180008496:	int3
-   180008497:	int3
-   180008498:	int3
-   180008499:	int3
-   18000849a:	int3
-   18000849b:	int3
-   18000849c:	int3
-   18000849d:	int3
-   18000849e:	int3
-   18000849f:	int3
-   1800084a0:	lea    0x20(%rdx),%rcx
-   1800084a7:	jmp    0x180003170
-   1800084ac:	int3
-   1800084ad:	int3
-   1800084ae:	int3
-   1800084af:	int3
-   1800084b0:	lea    0x60(%rdx),%rcx
-   1800084b7:	jmp    0x1800032a0
-   1800084bc:	int3
-   1800084bd:	int3
-   1800084be:	int3
-   1800084bf:	int3
-   1800084c0:	lea    0x340(%rdx),%rcx
-   1800084c7:	jmp    0x180002fa0
+   1800083a0:	mov    %rdx,0x10(%rsp)
+   1800083a5:	push   %rbp
+   1800083a6:	sub    $0x20,%rsp
+   1800083aa:	mov    %rdx,%rbp
+   1800083ad:	mov    0x60(%rbp),%rdx
+   1800083b1:	mov    (%rdx),%rax
+   1800083b4:	movslq 0x4(%rax),%rcx
+   1800083b8:	add    %rdx,%rcx
+   1800083bb:	mov    $0x1,%r8b
+   1800083be:	mov    $0x4,%edx
+   1800083c3:	call   *0xd37(%rip)        # 0x180009100
+   1800083c9:	nop
+   1800083ca:	movabs $0x0,%rax
+   1800083d4:	add    $0x20,%rsp
+   1800083d8:	pop    %rbp
+   1800083d9:	ret
+   1800083da:	int3
+   1800083db:	int3
+   1800083dc:	int3
+   1800083dd:	int3
+   1800083de:	int3
+   1800083df:	int3
+   1800083e0:	mov    %rdx,0x10(%rsp)
+   1800083e5:	push   %rbp
+   1800083e6:	sub    $0x20,%rsp
+   1800083ea:	mov    %rdx,%rbp
+   1800083ed:	xor    %edx,%edx
+   1800083ef:	xor    %ecx,%ecx
+   1800083f1:	call   0x180008294
+   1800083f6:	nop
+   1800083f7:	int3
+   1800083f8:	int3
+   1800083f9:	int3
+   1800083fa:	int3
+   1800083fb:	int3
+   1800083fc:	int3
+   1800083fd:	int3
+   1800083fe:	int3
+   1800083ff:	int3
+   180008400:	mov    %rdx,0x10(%rsp)
+   180008405:	push   %rbp
+   180008406:	sub    $0x20,%rsp
+   18000840a:	mov    %rdx,%rbp
+   18000840d:	mov    0x68(%rbp),%r8
+   180008411:	mov    0x78(%rbp),%rdx
+   180008415:	mov    0x60(%rbp),%rcx
+   180008419:	call   0x180004770
+   18000841e:	xor    %edx,%edx
+   180008420:	xor    %ecx,%ecx
+   180008422:	call   0x180008294
+   180008427:	nop
+   180008428:	int3
+   180008429:	int3
+   18000842a:	int3
+   18000842b:	int3
+   18000842c:	int3
+   18000842d:	int3
+   18000842e:	int3
+   18000842f:	int3
+   180008430:	mov    %rdx,0x10(%rsp)
+   180008435:	push   %rbp
+   180008436:	sub    $0x20,%rsp
+   18000843a:	mov    %rdx,%rbp
+   18000843d:	mov    0x78(%rbp),%r8
+   180008441:	mov    0x20(%rbp),%rdx
+   180008445:	mov    0x70(%rbp),%rcx
+   180008449:	call   0x1800047c0
+   18000844e:	xor    %edx,%edx
+   180008450:	xor    %ecx,%ecx
+   180008452:	call   0x180008294
+   180008457:	nop
+   180008458:	int3
+   180008459:	int3
+   18000845a:	int3
+   18000845b:	int3
+   18000845c:	int3
+   18000845d:	int3
+   18000845e:	int3
+   18000845f:	int3
+   180008460:	mov    %rdx,0x10(%rsp)
+   180008465:	push   %rbp
+   180008466:	sub    $0x20,%rsp
+   18000846a:	mov    %rdx,%rbp
+   18000846d:	mov    0x40(%rbp),%rcx
+   180008471:	call   0x1800037f0
+   180008476:	mov    %rax,%rcx
+   180008479:	mov    0x48(%rbp),%r8
+   18000847d:	mov    0x58(%rbp),%rdx
+   180008481:	call   0x180004800
+   180008486:	xor    %edx,%edx
+   180008488:	xor    %ecx,%ecx
+   18000848a:	call   0x180008294
+   18000848f:	nop
+   180008490:	mov    %rdx,0x10(%rsp)
+   180008495:	push   %rbp
+   180008496:	sub    $0x20,%rsp
+   18000849a:	mov    %rdx,%rbp
+   18000849d:	mov    0x50(%rbp),%rcx
+   1800084a1:	call   0x1800037f0
+   1800084a6:	mov    %rax,%rcx
+   1800084a9:	mov    0x58(%rbp),%r8
+   1800084ad:	mov    0x68(%rbp),%rdx
+   1800084b1:	call   0x180004800
+   1800084b6:	xor    %edx,%edx
+   1800084b8:	xor    %ecx,%ecx
+   1800084ba:	call   0x180008294
+   1800084bf:	nop
+   1800084c0:	lea    0x40(%rdx),%rcx
+   1800084c7:	jmp    0x180002de0
    1800084cc:	int3
    1800084cd:	int3
    1800084ce:	int3
    1800084cf:	int3
    1800084d0:	rex push %rbp
    1800084d2:	sub    $0x20,%rsp
    1800084d6:	mov    %rdx,%rbp
-   1800084d9:	mov    0x48(%rbp),%eax
+   1800084d9:	mov    0x30(%rbp),%eax
    1800084dc:	and    $0x1,%eax
    1800084df:	test   %eax,%eax
-   1800084e1:	je     0x1800084f8
-   1800084e3:	andl   $0xfffffffe,0x48(%rbp)
-   1800084e7:	lea    0x60(%rbp),%rcx
-   1800084eb:	add    $0xb8,%rcx
-   1800084f2:	call   *0xc18(%rip)        # 0x180009110
-   1800084f8:	add    $0x20,%rsp
-   1800084fc:	pop    %rbp
-   1800084fd:	ret
+   1800084e1:	je     0x1800084f3
+   1800084e3:	andl   $0xfffffffe,0x30(%rbp)
+   1800084e7:	mov    0xd8(%rbp),%rcx
+   1800084ee:	call   0x180002de0
+   1800084f3:	add    $0x20,%rsp
+   1800084f7:	pop    %rbp
+   1800084f8:	ret
+   1800084f9:	int3
+   1800084fa:	int3
+   1800084fb:	int3
+   1800084fc:	int3
+   1800084fd:	int3
    1800084fe:	int3
    1800084ff:	int3
-   180008500:	lea    0x60(%rdx),%rcx
-   180008507:	add    $0x20,%rcx
-   18000850b:	rex.W jmp *0xbb6(%rip)        # 0x1800090c8
-   180008512:	int3
-   180008513:	int3
-   180008514:	int3
-   180008515:	int3
-   180008516:	int3
-   180008517:	int3
-   180008518:	int3
-   180008519:	int3
-   18000851a:	int3
-   18000851b:	int3
-   18000851c:	int3
-   18000851d:	int3
-   18000851e:	int3
-   18000851f:	int3
-   180008520:	mov    0x240(%rdx),%rcx
-   180008527:	rex.W jmp *0xc72(%rip)        # 0x1800091a0
+   180008500:	rex push %rbp
+   180008502:	sub    $0x20,%rsp
+   180008506:	mov    %rdx,%rbp
+   180008509:	mov    $0x70,%edx
+   18000850e:	mov    0xe0(%rbp),%rcx
+   180008515:	call   0x1800073b8
+   18000851a:	add    $0x20,%rsp
+   18000851e:	pop    %rbp
+   18000851f:	ret
+   180008520:	mov    0xe0(%rdx),%rcx
+   180008527:	jmp    0x180002c70
+   18000852c:	int3
+   18000852d:	int3
    18000852e:	int3
    18000852f:	int3
-   180008530:	lea    0x240(%rdx),%rcx
-   180008537:	jmp    0x180003230
-   18000853c:	int3
-   18000853d:	int3
-   18000853e:	int3
-   18000853f:	int3
-   180008540:	lea    0x240(%rdx),%rcx
-   180008547:	jmp    0x180002d70
+   180008530:	mov    0xe0(%rdx),%rcx
+   180008537:	add    $0x58,%rcx
+   18000853b:	jmp    0x180002eb0
+   180008540:	lea    0xe0(%rdx),%rcx
+   180008547:	jmp    0x180002c80
    18000854c:	int3
    18000854d:	int3
    18000854e:	int3
    18000854f:	int3
-   180008550:	lea    0x3b0(%rdx),%rcx
-   180008557:	jmp    0x180002d70
+   180008550:	lea    0x40(%rdx),%rcx
+   180008557:	jmp    0x180002ca0
    18000855c:	int3
    18000855d:	int3
    18000855e:	int3
    18000855f:	int3
-   180008560:	lea    0x58(%rdx),%rcx
-   180008567:	jmp    0x180002d70
-   18000856c:	rex push %rbp
-   18000856e:	sub    $0x20,%rsp
-   180008572:	mov    %rdx,%rbp
-   180008575:	cmpb   $0x0,0x20(%rbp)
-   180008579:	jne    0x180008591
-   18000857b:	mov    0x78(%rbp),%r9
-   18000857f:	mov    0x70(%rbp),%r8
-   180008583:	mov    0x68(%rbp),%rdx
-   180008587:	mov    0x60(%rbp),%rcx
-   18000858b:	call   0x180007058
-   180008590:	nop
-   180008591:	add    $0x20,%rsp
-   180008595:	pop    %rbp
-   180008596:	ret
-   180008597:	int3
-   180008598:	rex push %rbx
-   18000859a:	push   %rbp
-   18000859b:	sub    $0x28,%rsp
-   18000859f:	mov    %rdx,%rbp
-   1800085a2:	mov    %rcx,0x40(%rbp)
-   1800085a6:	mov    %rcx,0x30(%rbp)
-   1800085aa:	mov    0x30(%rbp),%rax
-   1800085ae:	mov    (%rax),%rcx
-   1800085b1:	mov    %rcx,0x28(%rbp)
-   1800085b5:	mov    0x28(%rbp),%rax
-   1800085b9:	cmpl   $0xe06d7363,(%rax)
-   1800085bf:	je     0x1800085cd
-   1800085c1:	movl   $0x0,0x20(%rbp)
-   1800085c8:	mov    0x20(%rbp),%eax
-   1800085cb:	jmp    0x1800085ef
-   1800085cd:	call   0x180007fec
-   1800085d2:	mov    0x28(%rbp),%rcx
-   1800085d6:	mov    %rcx,(%rax)
-   1800085d9:	mov    0x30(%rbp),%rax
-   1800085dd:	mov    0x8(%rax),%rbx
-   1800085e1:	call   0x180007ff2
-   1800085e6:	mov    %rbx,(%rax)
-   1800085e9:	call   0x18000800a
-   1800085ee:	nop
-   1800085ef:	add    $0x28,%rsp
-   1800085f3:	pop    %rbp
-   1800085f4:	pop    %rbx
-   1800085f5:	ret
-   1800085f6:	int3
-   1800085f7:	rex push %rbp
-   1800085f9:	sub    $0x20,%rsp
-   1800085fd:	mov    %rdx,%rbp
-   180008600:	mov    0x40(%rbp),%cl
-   180008603:	add    $0x20,%rsp
-   180008607:	pop    %rbp
-   180008608:	jmp    0x1800078b8
-   18000860d:	int3
-   18000860e:	rex push %rbp
-   180008610:	sub    $0x20,%rsp
-   180008614:	mov    %rdx,%rbp
-   180008617:	mov    0x20(%rbp),%cl
-   18000861a:	call   0x1800078b8
-   18000861f:	nop
-   180008620:	add    $0x20,%rsp
-   180008624:	pop    %rbp
-   180008625:	ret
-   180008626:	int3
-   180008627:	rex push %rbp
-   180008629:	sub    $0x20,%rsp
-   18000862d:	mov    %rdx,%rbp
-   180008630:	add    $0x20,%rsp
-   180008634:	pop    %rbp
-   180008635:	jmp    0x180007734
-   18000863a:	int3
-   18000863b:	rex push %rbp
-   18000863d:	sub    $0x30,%rsp
-   180008641:	mov    %rdx,%rbp
-   180008644:	mov    (%rcx),%rax
-   180008647:	mov    (%rax),%edx
-   180008649:	mov    %rcx,0x28(%rsp)
-   18000864e:	mov    %edx,0x20(%rsp)
-   180008652:	lea    -0x13dd(%rip),%r9        # 0x18000727c
-   180008659:	mov    0x70(%rbp),%r8
-   18000865d:	mov    0x68(%rbp),%edx
-   180008660:	mov    0x60(%rbp),%rcx
-   180008664:	call   0x1800076a4
-   180008669:	nop
-   18000866a:	add    $0x30,%rsp
-   18000866e:	pop    %rbp
-   18000866f:	ret
-   180008670:	int3
-   180008671:	rex push %rbp
-   180008673:	mov    %rdx,%rbp
-   180008676:	mov    (%rcx),%rax
-   180008679:	xor    %ecx,%ecx
-   18000867b:	cmpl   $0xc0000005,(%rax)
-   180008681:	sete   %cl
-   180008684:	mov    %ecx,%eax
-   180008686:	pop    %rbp
-   180008687:	ret
-   180008688:	int3
-   180008689:	int3
-   18000868a:	int3
-   18000868b:	int3
-   18000868c:	rex push %rbx
-   18000868e:	sub    $0x20,%rsp
-   180008692:	jmp    0x1800086d5
-   180008694:	mov    (%rbx),%rax
-   180008697:	mov    0x8(%rbx),%rcx
-   18000869b:	mov    %rax,0x5f9e(%rip)        # 0x18000e640
-   1800086a2:	mov    (%rcx),%rax
-   1800086a5:	mov    0x10(%rax),%rax
-   1800086a9:	call   *0xdd1(%rip)        # 0x180009480
-   1800086af:	mov    %rax,%rcx
-   1800086b2:	test   %rax,%rax
-   1800086b5:	je     0x1800086c8
-   1800086b7:	mov    (%rax),%rdx
-   1800086ba:	mov    (%rdx),%rax
-   1800086bd:	mov    $0x1,%edx
-   1800086c2:	call   *0xdb8(%rip)        # 0x180009480
-   1800086c8:	mov    $0x10,%edx
-   1800086cd:	mov    %rbx,%rcx
-   1800086d0:	call   0x1800070f8
-   1800086d5:	mov    0x5f64(%rip),%rbx        # 0x18000e640
-   1800086dc:	test   %rbx,%rbx
-   1800086df:	jne    0x180008694
-   1800086e1:	add    $0x20,%rsp
-   1800086e5:	pop    %rbx
-   1800086e6:	ret
+   180008560:	lea    0x40(%rdx),%rcx
+   180008567:	rex.W jmp *0xbda(%rip)        # 0x180009148
+   18000856e:	int3
+   18000856f:	int3
+   180008570:	lea    0x50(%rdx),%rcx
+   180008577:	jmp    0x180002c80
+   18000857c:	int3
+   18000857d:	int3
+   18000857e:	int3
+   18000857f:	int3
+   180008580:	mov    0x30(%rdx),%rcx
+   180008587:	jmp    0x180002c20
+   18000858c:	int3
+   18000858d:	int3
+   18000858e:	int3
+   18000858f:	int3
+   180008590:	mov    0xe0(%rdx),%rcx
+   180008597:	add    $0x8,%rcx
+   18000859b:	jmp    0x180002c80
+   1800085a0:	mov    0xe0(%rdx),%rcx
+   1800085a7:	add    $0x10,%rcx
+   1800085ab:	jmp    0x1800071fa
+   1800085b0:	mov    0xe0(%rdx),%rcx
+   1800085b7:	add    $0x20,%rcx
+   1800085bb:	jmp    0x180002dd0
+   1800085c0:	mov    0xe0(%rdx),%rcx
+   1800085c7:	add    $0x40,%rcx
+   1800085cb:	jmp    0x180002de0
+   1800085d0:	mov    %rdx,0x10(%rsp)
+   1800085d5:	push   %rbp
+   1800085d6:	sub    $0x20,%rsp
+   1800085da:	mov    %rdx,%rbp
+   1800085dd:	mov    0x40(%rbp),%rcx
+   1800085e1:	call   0x1800037f0
+   1800085e6:	mov    %rax,%rcx
+   1800085e9:	mov    0x48(%rbp),%r8
+   1800085ed:	mov    0x50(%rbp),%rdx
+   1800085f1:	call   0x180004800
+   1800085f6:	xor    %edx,%edx
+   1800085f8:	xor    %ecx,%ecx
+   1800085fa:	call   0x180008294
+   1800085ff:	nop
+   180008600:	rex push %rbp
+   180008602:	sub    $0x20,%rsp
+   180008606:	mov    %rdx,%rbp
+   180008609:	mov    $0x70,%edx
+   18000860e:	mov    0x68(%rbp),%rcx
+   180008612:	call   0x1800073b8
+   180008617:	add    $0x20,%rsp
+   18000861b:	pop    %rbp
+   18000861c:	ret
+   18000861d:	int3
+   18000861e:	int3
+   18000861f:	int3
+   180008620:	lea    0x20(%rdx),%rcx
+   180008627:	jmp    0x180002de0
+   18000862c:	int3
+   18000862d:	int3
+   18000862e:	int3
+   18000862f:	int3
+   180008630:	mov    0x68(%rdx),%rcx
+   180008637:	jmp    0x180002c70
+   18000863c:	int3
+   18000863d:	int3
+   18000863e:	int3
+   18000863f:	int3
+   180008640:	mov    0x68(%rdx),%rcx
+   180008647:	add    $0x58,%rcx
+   18000864b:	jmp    0x180002eb0
+   180008650:	lea    0x68(%rdx),%rcx
+   180008657:	jmp    0x180002c80
+   18000865c:	int3
+   18000865d:	int3
+   18000865e:	int3
+   18000865f:	int3
+   180008660:	lea    0x130(%rdx),%rcx
+   180008667:	jmp    0x180002c20
+   18000866c:	int3
+   18000866d:	int3
+   18000866e:	int3
+   18000866f:	int3
+   180008670:	lea    0xd0(%rdx),%rcx
+   180008677:	jmp    0x180002c20
+   18000867c:	int3
+   18000867d:	int3
+   18000867e:	int3
+   18000867f:	int3
+   180008680:	lea    0x28(%rdx),%rcx
+   180008687:	jmp    0x180002ca0
+   18000868c:	int3
+   18000868d:	int3
+   18000868e:	int3
+   18000868f:	int3
+   180008690:	mov    %rdx,0x10(%rsp)
+   180008695:	push   %rbp
+   180008696:	sub    $0x20,%rsp
+   18000869a:	mov    %rdx,%rbp
+   18000869d:	mov    0x40(%rbp),%rax
+   1800086a1:	movb   $0x0,(%rax)
+   1800086a4:	xorps  %xmm0,%xmm0
+   1800086a7:	xor    %ecx,%ecx
+   1800086a9:	movups %xmm0,0x8(%rax)
+   1800086ad:	mov    %rcx,0x18(%rax)
+   1800086b1:	movabs $0x0,%rax
+   1800086bb:	add    $0x20,%rsp
+   1800086bf:	pop    %rbp
+   1800086c0:	ret
+   1800086c1:	int3
+   1800086c2:	int3
+   1800086c3:	int3
+   1800086c4:	int3
+   1800086c5:	int3
+   1800086c6:	int3
+   1800086c7:	int3
+   1800086c8:	int3
+   1800086c9:	int3
+   1800086ca:	int3
+   1800086cb:	int3
+   1800086cc:	int3
+   1800086cd:	int3
+   1800086ce:	int3
+   1800086cf:	int3
+   1800086d0:	rex push %rbp
+   1800086d2:	sub    $0x20,%rsp
+   1800086d6:	mov    %rdx,%rbp
+   1800086d9:	mov    $0x70,%edx
+   1800086de:	mov    0x30(%rbp),%rcx
+   1800086e2:	call   0x1800073b8
+   1800086e7:	add    $0x20,%rsp
+   1800086eb:	pop    %rbp
+   1800086ec:	ret
+   1800086ed:	int3
+   1800086ee:	int3
+   1800086ef:	int3
+   1800086f0:	lea    0x38(%rdx),%rcx
+   1800086f7:	jmp    0x180002de0
+   1800086fc:	int3
+   1800086fd:	int3
+   1800086fe:	int3
+   1800086ff:	int3
+   180008700:	mov    0x30(%rdx),%rcx
+   180008707:	jmp    0x180002c70
+   18000870c:	int3
+   18000870d:	int3
+   18000870e:	int3
+   18000870f:	int3
+   180008710:	mov    0x30(%rdx),%rcx
+   180008717:	add    $0x58,%rcx
+   18000871b:	jmp    0x180002eb0
+   180008720:	lea    0x30(%rdx),%rcx
+   180008727:	jmp    0x180002c80
+   18000872c:	int3
+   18000872d:	int3
+   18000872e:	int3
+   18000872f:	int3
+   180008730:	rex push %rbp
+   180008732:	sub    $0x20,%rsp
+   180008736:	mov    %rdx,%rbp
+   180008739:	mov    $0x70,%edx
+   18000873e:	mov    0xb0(%rbp),%rcx
+   180008745:	call   0x1800073b8
+   18000874a:	add    $0x20,%rsp
+   18000874e:	pop    %rbp
+   18000874f:	ret
+   180008750:	lea    0x48(%rdx),%rcx
+   180008757:	jmp    0x180002de0
+   18000875c:	int3
+   18000875d:	int3
+   18000875e:	int3
+   18000875f:	int3
+   180008760:	mov    0xb0(%rdx),%rcx
+   180008767:	jmp    0x180002c70
+   18000876c:	int3
+   18000876d:	int3
+   18000876e:	int3
+   18000876f:	int3
+   180008770:	mov    0xb0(%rdx),%rcx
+   180008777:	add    $0x58,%rcx
+   18000877b:	jmp    0x180002eb0
+   180008780:	lea    0xb0(%rdx),%rcx
+   180008787:	jmp    0x180002c80
+   18000878c:	int3
+   18000878d:	int3
+   18000878e:	int3
+   18000878f:	int3
+   180008790:	rex push %rbp
+   180008792:	sub    $0x20,%rsp
+   180008796:	mov    %rdx,%rbp
+   180008799:	mov    0x20(%rbp),%eax
+   18000879c:	and    $0x1,%eax
+   18000879f:	test   %eax,%eax
+   1800087a1:	je     0x1800087b0
+   1800087a3:	andl   $0xfffffffe,0x20(%rbp)
+   1800087a7:	mov    0x60(%rbp),%rcx
+   1800087ab:	call   0x180002ca0
+   1800087b0:	add    $0x20,%rsp
+   1800087b4:	pop    %rbp
+   1800087b5:	ret
+   1800087b6:	int3
+   1800087b7:	int3
+   1800087b8:	int3
+   1800087b9:	int3
+   1800087ba:	int3
+   1800087bb:	int3
+   1800087bc:	int3
+   1800087bd:	int3
+   1800087be:	int3
+   1800087bf:	int3
+   1800087c0:	lea    0x20(%rdx),%rcx
+   1800087c7:	jmp    0x180003170
+   1800087cc:	int3
+   1800087cd:	int3
+   1800087ce:	int3
+   1800087cf:	int3
+   1800087d0:	lea    0x60(%rdx),%rcx
+   1800087d7:	jmp    0x1800032a0
+   1800087dc:	int3
+   1800087dd:	int3
+   1800087de:	int3
+   1800087df:	int3
+   1800087e0:	lea    0x340(%rdx),%rcx
+   1800087e7:	jmp    0x180002fa0
+   1800087ec:	int3
+   1800087ed:	int3
+   1800087ee:	int3
+   1800087ef:	int3
+   1800087f0:	rex push %rbp
+   1800087f2:	sub    $0x20,%rsp
+   1800087f6:	mov    %rdx,%rbp
+   1800087f9:	mov    0x48(%rbp),%eax
+   1800087fc:	and    $0x1,%eax
+   1800087ff:	test   %eax,%eax
+   180008801:	je     0x180008818
+   180008803:	andl   $0xfffffffe,0x48(%rbp)
+   180008807:	lea    0x60(%rbp),%rcx
+   18000880b:	add    $0xb8,%rcx
+   180008812:	call   *0x8f8(%rip)        # 0x180009110
+   180008818:	add    $0x20,%rsp
+   18000881c:	pop    %rbp
+   18000881d:	ret
+   18000881e:	int3
+   18000881f:	int3
+   180008820:	lea    0x60(%rdx),%rcx
+   180008827:	add    $0x20,%rcx
+   18000882b:	rex.W jmp *0x896(%rip)        # 0x1800090c8
+   180008832:	int3
+   180008833:	int3
+   180008834:	int3
+   180008835:	int3
+   180008836:	int3
+   180008837:	int3
+   180008838:	int3
+   180008839:	int3
+   18000883a:	int3
+   18000883b:	int3
+   18000883c:	int3
+   18000883d:	int3
+   18000883e:	int3
+   18000883f:	int3
+   180008840:	mov    0x240(%rdx),%rcx
+   180008847:	rex.W jmp *0x952(%rip)        # 0x1800091a0
+   18000884e:	int3
+   18000884f:	int3
+   180008850:	lea    0x240(%rdx),%rcx
+   180008857:	jmp    0x180003230
+   18000885c:	int3
+   18000885d:	int3
+   18000885e:	int3
+   18000885f:	int3
+   180008860:	lea    0x240(%rdx),%rcx
+   180008867:	jmp    0x180002d70
+   18000886c:	int3
+   18000886d:	int3
+   18000886e:	int3
+   18000886f:	int3
+   180008870:	lea    0x3b0(%rdx),%rcx
+   180008877:	jmp    0x180002d70
+   18000887c:	int3
+   18000887d:	int3
+   18000887e:	int3
+   18000887f:	int3
+   180008880:	lea    0x58(%rdx),%rcx
+   180008887:	jmp    0x180002d70
+   18000888c:	rex push %rbp
+   18000888e:	sub    $0x20,%rsp
+   180008892:	mov    %rdx,%rbp
+   180008895:	cmpb   $0x0,0x20(%rbp)
+   180008899:	jne    0x1800088b1
+   18000889b:	mov    0x78(%rbp),%r9
+   18000889f:	mov    0x70(%rbp),%r8
+   1800088a3:	mov    0x68(%rbp),%rdx
+   1800088a7:	mov    0x60(%rbp),%rcx
+   1800088ab:	call   0x180007318
+   1800088b0:	nop
+   1800088b1:	add    $0x20,%rsp
+   1800088b5:	pop    %rbp
+   1800088b6:	ret
+   1800088b7:	int3
+   1800088b8:	rex push %rbx
+   1800088ba:	push   %rbp
+   1800088bb:	sub    $0x28,%rsp
+   1800088bf:	mov    %rdx,%rbp
+   1800088c2:	mov    %rcx,0x40(%rbp)
+   1800088c6:	mov    %rcx,0x30(%rbp)
+   1800088ca:	mov    0x30(%rbp),%rax
+   1800088ce:	mov    (%rax),%rcx
+   1800088d1:	mov    %rcx,0x28(%rbp)
+   1800088d5:	mov    0x28(%rbp),%rax
+   1800088d9:	cmpl   $0xe06d7363,(%rax)
+   1800088df:	je     0x1800088ed
+   1800088e1:	movl   $0x0,0x20(%rbp)
+   1800088e8:	mov    0x20(%rbp),%eax
+   1800088eb:	jmp    0x18000890f
+   1800088ed:	call   0x1800082ac
+   1800088f2:	mov    0x28(%rbp),%rcx
+   1800088f6:	mov    %rcx,(%rax)
+   1800088f9:	mov    0x30(%rbp),%rax
+   1800088fd:	mov    0x8(%rax),%rbx
+   180008901:	call   0x1800082b2
+   180008906:	mov    %rbx,(%rax)
+   180008909:	call   0x1800082ca
+   18000890e:	nop
+   18000890f:	add    $0x28,%rsp
+   180008913:	pop    %rbp
+   180008914:	pop    %rbx
+   180008915:	ret
+   180008916:	int3
+   180008917:	rex push %rbp
+   180008919:	sub    $0x20,%rsp
+   18000891d:	mov    %rdx,%rbp
+   180008920:	mov    0x40(%rbp),%cl
+   180008923:	add    $0x20,%rsp
+   180008927:	pop    %rbp
+   180008928:	jmp    0x180007b78
+   18000892d:	int3
+   18000892e:	rex push %rbp
+   180008930:	sub    $0x20,%rsp
+   180008934:	mov    %rdx,%rbp
+   180008937:	mov    0x20(%rbp),%cl
+   18000893a:	call   0x180007b78
+   18000893f:	nop
+   180008940:	add    $0x20,%rsp
+   180008944:	pop    %rbp
+   180008945:	ret
+   180008946:	int3
+   180008947:	rex push %rbp
+   180008949:	sub    $0x20,%rsp
+   18000894d:	mov    %rdx,%rbp
+   180008950:	add    $0x20,%rsp
+   180008954:	pop    %rbp
+   180008955:	jmp    0x1800079f4
+   18000895a:	int3
+   18000895b:	rex push %rbp
+   18000895d:	sub    $0x30,%rsp
+   180008961:	mov    %rdx,%rbp
+   180008964:	mov    (%rcx),%rax
+   180008967:	mov    (%rax),%edx
+   180008969:	mov    %rcx,0x28(%rsp)
+   18000896e:	mov    %edx,0x20(%rsp)
+   180008972:	lea    -0x143d(%rip),%r9        # 0x18000753c
+   180008979:	mov    0x70(%rbp),%r8
+   18000897d:	mov    0x68(%rbp),%edx
+   180008980:	mov    0x60(%rbp),%rcx
+   180008984:	call   0x180007964
+   180008989:	nop
+   18000898a:	add    $0x30,%rsp
+   18000898e:	pop    %rbp
+   18000898f:	ret
+   180008990:	int3
+   180008991:	rex push %rbp
+   180008993:	mov    %rdx,%rbp
+   180008996:	mov    (%rcx),%rax
+   180008999:	xor    %ecx,%ecx
+   18000899b:	cmpl   $0xc0000005,(%rax)
+   1800089a1:	sete   %cl
+   1800089a4:	mov    %ecx,%eax
+   1800089a6:	pop    %rbp
+   1800089a7:	ret
+   1800089a8:	int3
+   1800089a9:	int3
+   1800089aa:	int3
+   1800089ab:	int3
+   1800089ac:	rex push %rbx
+   1800089ae:	sub    $0x20,%rsp
+   1800089b2:	jmp    0x1800089f5
+   1800089b4:	mov    (%rbx),%rax
+   1800089b7:	mov    0x8(%rbx),%rcx
+   1800089bb:	mov    %rax,0x5c7e(%rip)        # 0x18000e640
+   1800089c2:	mov    (%rcx),%rax
+   1800089c5:	mov    0x10(%rax),%rax
+   1800089c9:	call   *0xab1(%rip)        # 0x180009480
+   1800089cf:	mov    %rax,%rcx
+   1800089d2:	test   %rax,%rax
+   1800089d5:	je     0x1800089e8
+   1800089d7:	mov    (%rax),%rdx
+   1800089da:	mov    (%rdx),%rax
+   1800089dd:	mov    $0x1,%edx
+   1800089e2:	call   *0xa98(%rip)        # 0x180009480
+   1800089e8:	mov    $0x10,%edx
+   1800089ed:	mov    %rbx,%rcx
+   1800089f0:	call   0x1800073b8
+   1800089f5:	mov    0x5c44(%rip),%rbx        # 0x18000e640
+   1800089fc:	test   %rbx,%rbx
+   1800089ff:	jne    0x1800089b4
+   180008a01:	add    $0x20,%rsp
+   180008a05:	pop    %rbx
+   180008a06:	ret
 
 Disassembly of section .rdata:
 
 0000000180009000 <.rdata>:
-   180009000:	movabs $0xbfbe000000000000,%rdi
-   18000900a:	add    %al,(%rax)
+   180009000:	mov    $0xbf,%eax
+   180009005:	add    %al,(%rax)
+   180009007:	add    %ch,(%rsi)
+   180009009:	rolb   $0x0,(%rax)
    18000900c:	add    %al,(%rax)
    18000900e:	add    %al,(%rax)
-   180009010:	hlt
-   180009011:	mov    $0x0,%edi
+   180009010:	rolb   $0x0,%fs:(%rax)
+   180009014:	add    %al,(%rax)
    180009016:	add    %al,(%rax)
-   180009018:	cmp    %al,%al
-   18000901a:	add    %al,(%rax)
+   180009018:	stos   %al,%es:(%rdi)
+   180009019:	rolb   $0x0,(%rax)
    18000901c:	add    %al,(%rax)
    18000901e:	add    %al,(%rax)
-   180009020:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   180009021:	rolb   $0x0,(%rax)
+   180009020:	(bad)
+   180009021:	roll   $0x0,(%rax)
    180009024:	add    %al,(%rax)
    180009026:	add    %al,(%rax)
-   180009028:	(bad)
-   180009029:	roll   $0x0,(%rax)
+   180009028:	mov    %ecx,%es
+   18000902a:	add    %al,(%rax)
    18000902c:	add    %al,(%rax)
    18000902e:	add    %al,(%rax)
-   180009030:	adc    %bh,0x0(%rdi)
+   180009030:	cmpb   $0x0,0x0(%rdi)
 	...
-   18000903e:	add    %al,(%rax)
-   180009040:	push   %rsp
+   18000903f:	add    %al,%ah
    180009041:	fadds  (%rax)
    180009043:	add    %al,(%rax)
    180009045:	add    %al,(%rax)
-   180009047:	add    %bh,(%rax)
-   180009049:	fadds  (%rax)
-   18000904b:	add    %al,(%rax)
+   180009047:	add    %ch,0xd8(%rax)
    18000904d:	add    %al,(%rax)
-   18000904f:	add    %bl,(%rsi)
-   180009051:	fadds  (%rax)
-   180009053:	add    %al,(%rax)
+   18000904f:	add    %cl,0xd8(%rsi)
    180009055:	add    %al,(%rax)
-   180009057:	add    %cl,(%rax)
-   180009059:	fadds  (%rax)
-   18000905b:	add    %al,(%rax)
-   18000905d:	add    %al,(%rax)
-   18000905f:	add    %dh,%dl
-   180009061:	xlat   %ds:(%rbx)
-   180009062:	add    %al,(%rax)
-   180009064:	add    %al,(%rax)
-   180009066:	add    %al,(%rax)
-   180009068:	fcom   %st(7)
+   180009057:	add    %bh,-0x28(%rax)
+   18000905a:	add    %al,(%rax)
+   18000905c:	add    %al,(%rax)
+   18000905e:	add    %al,(%rax)
+   180009060:	(bad)
+   180009061:	fadds  (%rax)
+   180009063:	add    %al,(%rax)
+   180009065:	add    %al,(%rax)
+   180009067:	add    %cl,-0x28(%rax)
    18000906a:	add    %al,(%rax)
    18000906c:	add    %al,(%rax)
    18000906e:	add    %al,(%rax)
-   180009070:	mov    $0xd7,%esp
-   180009075:	add    %al,(%rax)
-   180009077:	add    %ch,0xd7(%rax)
-   18000907d:	add    %al,(%rax)
-   18000907f:	add    %dl,0x0(%rdi,%rdx,8)
+   180009070:	sub    $0xd8,%al
+   180009072:	add    %al,(%rax)
+   180009074:	add    %al,(%rax)
+   180009076:	add    %al,(%rax)
+   180009078:	sbb    %bl,%al
+   18000907a:	add    %al,(%rax)
+   18000907c:	add    %al,(%rax)
+   18000907e:	add    %al,(%rax)
+   180009080:	add    $0xd8,%al
+   180009082:	add    %al,(%rax)
+   180009084:	add    %al,(%rax)
    180009086:	add    %al,(%rax)
-   180009088:	jbe    0x180009061
+   180009088:	out    %al,$0xd7
    18000908a:	add    %al,(%rax)
    18000908c:	add    %al,(%rax)
    18000908e:	add    %al,(%rax)
-   180009090:	pop    %rdx
-   180009091:	xlat   %ds:(%rbx)
-   180009092:	add    %al,(%rax)
-   180009094:	add    %al,(%rax)
-   180009096:	add    %al,(%rax)
-   180009098:	rex.RX xlat %ds:(%rbx)
-   18000909a:	add    %al,(%rax)
-   18000909c:	add    %al,(%rax)
-   18000909e:	add    %al,(%rax)
-   1800090a0:	sub    $0xd7,%al
-   1800090a2:	add    %al,(%rax)
-   1800090a4:	add    %al,(%rax)
+   180009090:	lret   $0xd7
+   180009093:	add    %al,(%rax)
+   180009095:	add    %al,(%rax)
+   180009097:	add    %dh,0xd7(%rsi)
+   18000909d:	add    %al,(%rax)
+   18000909f:	add    %bl,0x0(%rdi,%rdx,8)
    1800090a6:	add    %al,(%rax)
-   1800090a8:	sbb    %dl,%bh
+   1800090a8:	mov    %dl,%bh
    1800090aa:	add    %al,(%rax)
    1800090ac:	add    %al,(%rax)
    1800090ae:	add    %al,(%rax)
-   1800090b0:	add    %bh,%dl
+   1800090b0:	jb     0x180009089
 	...
    1800090be:	add    %al,(%rax)
-   1800090c0:	xchg   %eax,%esp
-   1800090c1:	rolb   %cl,(%rax)
-   1800090c3:	add    %al,(%rax)
-   1800090c5:	add    %al,(%rax)
-   1800090c7:	add    %bl,-0x2e(%rax)
-   1800090ca:	add    %al,(%rax)
+   1800090c0:	add    $0xd3,%al
+   1800090c2:	add    %al,(%rax)
+   1800090c4:	add    %al,(%rax)
+   1800090c6:	add    %al,(%rax)
+   1800090c8:	enter  $0xd2,$0x0
    1800090cc:	add    %al,(%rax)
    1800090ce:	add    %al,(%rax)
-   1800090d0:	in     (%dx),%al
-   1800090d1:	roll   (%rax)
+   1800090d0:	pop    %rsp
+   1800090d1:	rolb   %cl,(%rax)
    1800090d3:	add    %al,(%rax)
    1800090d5:	add    %al,(%rax)
-   1800090d7:	add    %ch,0xd1(%rax)
+   1800090d7:	add    %bl,(%rax)
+   1800090d9:	rolb   %cl,(%rax)
+   1800090db:	add    %al,(%rax)
    1800090dd:	add    %al,(%rax)
-   1800090df:	add    %ah,-0x2f(%rsi)
-   1800090e2:	add    %al,(%rax)
-   1800090e4:	add    %al,(%rax)
-   1800090e6:	add    %al,(%rax)
-   1800090e8:	and    $0xd1,%al
-   1800090ea:	add    %al,(%rax)
-   1800090ec:	add    %al,(%rax)
+   1800090df:	add    %dl,%dh
+   1800090e1:	roll   (%rax)
+   1800090e3:	add    %al,(%rax)
+   1800090e5:	add    %al,(%rax)
+   1800090e7:	add    %dl,0x0(%rcx,%rdx,8)
    1800090ee:	add    %al,(%rax)
-   1800090f0:	out    %al,$0xd0
-   1800090f2:	add    %al,(%rax)
-   1800090f4:	add    %al,(%rax)
-   1800090f6:	add    %al,(%rax)
-   1800090f8:	mov    $0xd0,%al
-   1800090fa:	add    %al,(%rax)
-   1800090fc:	add    %al,(%rax)
-   1800090fe:	add    %al,(%rax)
-   180009100:	jo     0x1800090d2
-   180009102:	add    %al,(%rax)
-   180009104:	add    %al,(%rax)
-   180009106:	add    %al,(%rax)
-   180009108:	xor    %al,%dl
-   18000910a:	add    %al,(%rax)
-   18000910c:	add    %al,(%rax)
-   18000910e:	add    %al,(%rax)
-   180009110:	cld
-   180009111:	iret
-   180009112:	add    %al,(%rax)
-   180009114:	add    %al,(%rax)
-   180009116:	add    %al,(%rax)
-   180009118:	mov    $0xcf,%ah
+   1800090f0:	push   %rsi
+   1800090f1:	roll   (%rax)
+   1800090f3:	add    %al,(%rax)
+   1800090f5:	add    %al,(%rax)
+   1800090f7:	add    %ah,(%rax)
+   1800090f9:	roll   (%rax)
+   1800090fb:	add    %al,(%rax)
+   1800090fd:	add    %al,(%rax)
+   1800090ff:	add    %ah,%al
+   180009101:	rolb   (%rax)
+   180009103:	add    %al,(%rax)
+   180009105:	add    %al,(%rax)
+   180009107:	add    %ah,0xd0(%rdx)
+   18000910d:	add    %al,(%rax)
+   18000910f:	add    %ch,0x0(%rax,%rdx,8)
+   180009113:	add    %al,(%rax)
+   180009115:	add    %al,(%rax)
+   180009117:	add    %ah,(%rax,%rdx,8)
    18000911a:	add    %al,(%rax)
    18000911c:	add    %al,(%rax)
    18000911e:	add    %al,(%rax)
-   180009120:	insb   (%dx),%es:(%rdi)
-   180009121:	iret
+   180009120:	fmul   %st,%st(7)
    180009122:	add    %al,(%rax)
    180009124:	add    %al,(%rax)
    180009126:	add    %al,(%rax)
-   180009128:	sbb    $0xcf,%al
+   180009128:	mov    %cs,%edi
    18000912a:	add    %al,(%rax)
    18000912c:	add    %al,(%rax)
    18000912e:	add    %al,(%rax)
-   180009130:	add    %bl,%dl
+   180009130:	jb     0x180009105
    180009132:	add    %al,(%rax)
    180009134:	add    %al,(%rax)
    180009136:	add    %al,(%rax)
-   180009138:	mov    $0xd2,%esp
-   18000913d:	add    %al,(%rax)
-   18000913f:	add    %dl,(%rax)
-   180009141:	lret
-   180009142:	add    %al,(%rax)
-   180009144:	add    %al,(%rax)
-   180009146:	add    %al,(%rax)
-   180009148:	sub    $0xcb,%al
-   18000914a:	add    %al,(%rax)
-   18000914c:	add    %al,(%rax)
+   180009138:	sub    $0xd3,%al
+   18000913a:	add    %al,(%rax)
+   18000913c:	add    %al,(%rax)
+   18000913e:	add    %al,(%rax)
+   180009140:	or     $0x0,%bl
+   180009143:	add    %al,(%rax)
+   180009145:	add    %al,(%rax)
+   180009147:	add    %bl,0x0(%rbx,%rcx,8)
    18000914e:	add    %al,(%rax)
-   180009150:	rex.RX lret
+   180009150:	mov    $0xcb,%dh
    180009152:	add    %al,(%rax)
    180009154:	add    %al,(%rax)
    180009156:	add    %al,(%rax)
-   180009158:	push   $0xcb
-   18000915d:	add    %al,(%rax)
-   18000915f:	add    %cl,0xcb(%rdx)
-   180009165:	add    %al,(%rax)
-   180009167:	add    %ch,0xcb(%rax)
-   18000916d:	add    %al,(%rax)
-   18000916f:	add    %bl,%ah
-   180009171:	lret
+   180009158:	fmul   %st(3),%st
+   18000915a:	add    %al,(%rax)
+   18000915c:	add    %al,(%rax)
+   18000915e:	add    %al,(%rax)
+   180009160:	cli
+   180009161:	lret
+   180009162:	add    %al,(%rax)
+   180009164:	add    %al,(%rax)
+   180009166:	add    %al,(%rax)
+   180009168:	sbb    %cl,%ah
+   18000916a:	add    %al,(%rax)
+   18000916c:	add    %al,(%rax)
+   18000916e:	add    %al,(%rax)
+   180009170:	rex.WR int3
    180009172:	add    %al,(%rax)
    180009174:	add    %al,(%rax)
    180009176:	add    %al,(%rax)
-   180009178:	or     %cl,%ah
+   180009178:	js     0x180009146
    18000917a:	add    %al,(%rax)
    18000917c:	add    %al,(%rax)
    18000917e:	add    %al,(%rax)
-   180009180:	pop    %rsp
+   180009180:	int3
    180009181:	int3
    180009182:	add    %al,(%rax)
    180009184:	add    %al,(%rax)
    180009186:	add    %al,(%rax)
-   180009188:	mov    $0xcc,%al
+   180009188:	and    %cl,%ch
    18000918a:	add    %al,(%rax)
    18000918c:	add    %al,(%rax)
    18000918e:	add    %al,(%rax)
-   180009190:	cld
-   180009191:	int3
-   180009192:	add    %al,(%rax)
-   180009194:	add    %al,(%rax)
-   180009196:	add    %al,(%rax)
-   180009198:	rex.WX int $0x0
-   18000919b:	add    %al,(%rax)
+   180009190:	insb   (%dx),%es:(%rdi)
+   180009191:	int    $0x0
+   180009193:	add    %al,(%rax)
+   180009195:	add    %al,(%rax)
+   180009197:	add    %bh,0xcd(%rdx)
    18000919d:	add    %al,(%rax)
-   18000919f:	add    %al,0xcd(%rsi)
+   18000919f:	add    %dh,%dh
+   1800091a1:	int    $0x0
+   1800091a3:	add    %al,(%rax)
    1800091a5:	add    %al,(%rax)
-   1800091a7:	add    %al,%dl
-   1800091a9:	int    $0x0
-   1800091ab:	add    %al,(%rax)
-   1800091ad:	add    %al,(%rax)
-   1800091af:	add    %cl,(%rsi)
-   1800091b1:	(bad)
+   1800091a7:	add    %dh,(%rdx)
+   1800091a9:	(bad)
+   1800091aa:	add    %al,(%rax)
+   1800091ac:	add    %al,(%rax)
+   1800091ae:	add    %al,(%rax)
+   1800091b0:	jle    0x180009180
    1800091b2:	add    %al,(%rax)
    1800091b4:	add    %al,(%rax)
    1800091b6:	add    %al,(%rax)
-   1800091b8:	push   %rax
-   1800091b9:	(bad)
-   1800091ba:	add    %al,(%rax)
-   1800091bc:	add    %al,(%rax)
-   1800091be:	add    %al,(%rax)
-   1800091c0:	cwtl
-   1800091c1:	(bad)
+   1800091b8:	ror    $0x0,%dh
+   1800091bb:	add    %al,(%rax)
+   1800091bd:	add    %al,(%rax)
+   1800091bf:	add    %cl,(%rax)
+   1800091c1:	iret
    1800091c2:	add    %al,(%rax)
    1800091c4:	add    %al,(%rax)
    1800091c6:	add    %al,(%rax)
-   1800091c8:	fmul   %st,%st(6)
+   1800091c8:	rex.WR iretq
 	...
    1800091d6:	add    %al,(%rax)
-   1800091d8:	fadd   %st,%st(7)
-   1800091da:	add    %al,(%rax)
-   1800091dc:	add    %al,(%rax)
-   1800091de:	add    %al,(%rax)
-   1800091e0:	sbb    %al,%cl
-   1800091e2:	add    %al,(%rax)
-   1800091e4:	add    %al,(%rax)
-   1800091e6:	add    %al,(%rax)
-   1800091e8:	push   %rdx
+   1800091d8:	rex.WR enter $0x0,$0x0
+   1800091dd:	add    %al,(%rax)
+   1800091df:	add    %cl,0xc8(%rdx)
+   1800091e5:	add    %al,(%rax)
+   1800091e7:	add    %al,%dl
    1800091e9:	enter  $0x0,$0x0
    1800091ed:	add    %al,(%rax)
-   1800091ef:	add    %bl,%al
-   1800091f1:	leave
+   1800091ef:	add    %cl,-0x36(%rax)
    1800091f2:	add    %al,(%rax)
    1800091f4:	add    %al,(%rax)
    1800091f6:	add    %al,(%rax)
-   1800091f8:	(bad)
-   1800091f9:	leave
+   1800091f8:	ror    %cl,%cl
    1800091fa:	add    %al,(%rax)
    1800091fc:	add    %al,(%rax)
    1800091fe:	add    %al,(%rax)
-   180009200:	sbb    %cl,%cl
+   180009200:	mov    %cl,%cl
    180009202:	add    %al,(%rax)
    180009204:	add    %al,(%rax)
    180009206:	add    %al,(%rax)
-   180009208:	mov    $0xc8,%eax
-   18000920d:	add    %al,(%rax)
-   18000920f:	add    %cl,0xc8(%rdx)
+   180009208:	sub    %cl,%cl
+   18000920a:	add    %al,(%rax)
+   18000920c:	add    %al,(%rax)
+   18000920e:	add    %al,(%rax)
+   180009210:	cli
+   180009211:	enter  $0x0,$0x0
    180009215:	add    %al,(%rax)
-   180009217:	add    %ch,-0x38(%rsi)
+   180009217:	add    %bl,%dh
+   180009219:	enter  $0x0,$0x0
 	...
-   180009226:	add    %al,(%rax)
-   180009228:	xor    %bh,%al
-   18000922a:	add    %al,(%rax)
-   18000922c:	add    %al,(%rax)
-   18000922e:	add    %al,(%rax)
-   180009230:	cwtl
-   180009231:	movb   $0x0,(%rax)
-	...
-   180009240:	movabs %al,0x4e000000000000c5
-   180009249:	(bad)
-   18000924a:	add    %al,(%rax)
-   18000924c:	add    %al,(%rax)
-   18000924e:	add    %al,(%rax)
-   180009250:	cmp    %dh,%al
-   180009252:	add    %al,(%rax)
-   180009254:	add    %al,(%rax)
-   180009256:	add    %al,(%rax)
-   180009258:	(bad)
-   18000925c:	add    %al,(%rax)
-   18000925e:	add    %al,(%rax)
-   180009260:	mov    $0xc3,%dh
+   180009225:	add    %al,(%rax)
+   180009227:	add    %ah,0xc7(%rdx)
+   18000922d:	add    %al,(%rax)
+   18000922f:	add    %cl,(%rax)
+   180009231:	movl   $0x0,(%rax)
+	...
+   18000923f:	add    %dl,(%rdx)
+   180009241:	movb   $0x0,(%rax)
+   180009244:	add    %al,(%rax)
+   180009246:	add    %al,(%rax)
+   180009248:	mov    $0xc4,%esi
+   18000924d:	add    %al,(%rax)
+   18000924f:	add    %ch,0xc6(%rdx)
+   180009255:	add    %al,(%rax)
+   180009257:	add    %ch,0xc5(%rsi)
+   18000925d:	add    %al,(%rax)
+   18000925f:	add    %ah,(%rsi)
+   180009261:	(bad)
    180009262:	add    %al,(%rax)
    180009264:	add    %al,(%rax)
    180009266:	add    %al,(%rax)
-   180009268:	jo     0x18000922d
+   180009268:	loopne 0x18000922d
    18000926a:	add    %al,(%rax)
    18000926c:	add    %al,(%rax)
    18000926e:	add    %al,(%rax)
-   180009270:	rex ret
+   180009270:	mov    $0xc3,%al
    180009272:	add    %al,(%rax)
    180009274:	add    %al,(%rax)
    180009276:	add    %al,(%rax)
-   180009278:	out    %al,(%dx)
-   180009279:	ret    $0x0
+   180009278:	pop    %rsi
+   180009279:	ret
+   18000927a:	add    %al,(%rax)
    18000927c:	add    %al,(%rax)
    18000927e:	add    %al,(%rax)
-   180009280:	(bad)
-   180009281:	ret    $0x0
+   180009280:	xchg   %al,%dl
+   180009282:	add    %al,(%rax)
    180009284:	add    %al,(%rax)
    180009286:	add    %al,(%rax)
-   180009288:	lret   $0xc1
-   18000928b:	add    %al,(%rax)
-   18000928d:	add    %al,(%rax)
-   18000928f:	add    %ah,0xc1(%rdx)
-   180009295:	add    %al,(%rax)
-   180009297:	add    %dh,0xc4(%rdx)
-   18000929d:	add    %al,(%rax)
-   18000929f:	add    %cl,(%rsi,%rax,8)
+   180009288:	cmp    %dl,%al
+   18000928a:	add    %al,(%rax)
+   18000928c:	add    %al,(%rax)
+   18000928e:	add    %al,(%rax)
+   180009290:	adc    %dl,%al
+   180009292:	add    %al,(%rax)
+   180009294:	add    %al,(%rax)
+   180009296:	add    %al,(%rax)
+   180009298:	and    %ch,%al
+   18000929a:	add    %al,(%rax)
+   18000929c:	add    %al,(%rax)
+   18000929e:	add    %al,(%rax)
+   1800092a0:	jl     0x180009268
    1800092a2:	add    %al,(%rax)
    1800092a4:	add    %al,(%rax)
    1800092a6:	add    %al,(%rax)
-   1800092a8:	hlt
-   1800092a9:	(bad)
-   1800092aa:	add    %al,(%rax)
+   1800092a8:	(bad)
    1800092ac:	add    %al,(%rax)
    1800092ae:	add    %al,(%rax)
-   1800092b0:	add    $0x0,%ah
+   1800092b0:	lock (bad)
 	...
-   1800092bf:	add    %ch,(%rsi)
+   1800092be:	add    %al,(%rax)
+   1800092c0:	sahf
    1800092c1:	(bad)
    1800092c2:	add    %al,(%rax)
    1800092c4:	add    %al,(%rax)
    1800092c6:	add    %al,(%rax)
-   1800092c8:	rex.RX (bad)
+   1800092c8:	mov    $0xd4,%dh
    1800092ca:	add    %al,(%rax)
    1800092cc:	add    %al,(%rax)
    1800092ce:	add    %al,(%rax)
-   1800092d0:	lock roll %cl,(%rax)
-   1800092d3:	add    %al,(%rax)
-   1800092d5:	add    %al,(%rax)
-   1800092d7:	add    %bl,%ah
-   1800092d9:	roll   %cl,(%rax)
-   1800092db:	add    %al,(%rax)
-   1800092dd:	add    %al,(%rax)
-   1800092df:	add    %al,%dh
-   1800092e1:	roll   %cl,(%rax)
-   1800092e3:	add    %al,(%rax)
-   1800092e5:	add    %al,(%rax)
-   1800092e7:	add    %ch,0xd3(%rsi)
-   1800092ed:	add    %al,(%rax)
-   1800092ef:	add    %dl,0x0(%rbx,%rdx,8)
+   1800092d0:	(bad)
+   1800092d1:	(bad)
+   1800092d2:	add    %al,(%rax)
+   1800092d4:	add    %al,(%rax)
+   1800092d6:	add    %al,(%rax)
+   1800092d8:	rex.WR (bad)
+   1800092da:	add    %al,(%rax)
+   1800092dc:	add    %al,(%rax)
+   1800092de:	add    %al,(%rax)
+   1800092e0:	ss (bad)
+   1800092e2:	add    %al,(%rax)
+   1800092e4:	add    %al,(%rax)
+   1800092e6:	add    %al,(%rax)
+   1800092e8:	(bad)
+   1800092e9:	(bad)
+   1800092ea:	add    %al,(%rax)
+   1800092ec:	add    %al,(%rax)
+   1800092ee:	add    %al,(%rax)
+   1800092f0:	add    $0xd4,%al
+   1800092f2:	add    %al,(%rax)
+   1800092f4:	add    %al,(%rax)
    1800092f6:	add    %al,(%rax)
-   1800092f8:	jl     0x1800092cd
-   1800092fa:	add    %al,(%rax)
-   1800092fc:	add    %al,(%rax)
-   1800092fe:	add    %al,(%rax)
-   180009300:	push   $0xffffffffffffffd3
-   180009302:	add    %al,(%rax)
-   180009304:	add    %al,(%rax)
-   180009306:	add    %al,(%rax)
-   180009308:	pop    %rax
+   1800092f8:	in     (%dx),%al
+   1800092f9:	roll   %cl,(%rax)
+   1800092fb:	add    %al,(%rax)
+   1800092fd:	add    %al,(%rax)
+   1800092ff:	add    %bl,%dl
+   180009301:	roll   %cl,(%rax)
+   180009303:	add    %al,(%rax)
+   180009305:	add    %al,(%rax)
+   180009307:	add    %cl,%al
    180009309:	roll   %cl,(%rax)
    18000930b:	add    %al,(%rax)
    18000930d:	add    %al,(%rax)
-   18000930f:	add    %dl,(%rax)
-   180009311:	(bad)
-   180009312:	add    %al,(%rax)
-   180009314:	add    %al,(%rax)
-   180009316:	add    %al,(%rax)
-   180009318:	cli
-   180009319:	roll   %cl,(%rax)
-   18000931b:	add    %al,(%rax)
-   18000931d:	add    %al,(%rax)
-   18000931f:	add    %ah,%dh
-   180009321:	roll   %cl,(%rax)
+   18000930f:	add    %al,0xd4(%rax)
+   180009315:	add    %al,(%rax)
+   180009317:	add    %ch,-0x2c(%rdx)
+   18000931a:	add    %al,(%rax)
+   18000931c:	add    %al,(%rax)
+   18000931e:	add    %al,(%rax)
+   180009320:	push   %rsi
+   180009321:	(bad)
 	...
-   18000932f:	add    %al,-0x2d(%rdx)
+   18000932e:	add    %al,(%rax)
+   180009330:	mov    $0xd3,%dl
 	...
    18000933e:	add    %al,(%rax)
-   180009340:	cwtl
-   180009341:	lret   $0x0
+   180009340:	or     %cl,%bl
+   180009342:	add    %al,(%rax)
    180009344:	add    %al,(%rax)
    180009346:	add    %al,(%rax)
-   180009348:	(bad)
-   180009349:	lret   $0x0
+   180009348:	ror    %dl
 	...
-   180009358:	cmp    %ch,%dl
+   180009356:	add    %al,(%rax)
+   180009358:	stos   %al,%es:(%rdi)
+   180009359:	(bad)
    18000935a:	add    %al,(%rax)
    18000935c:	add    %al,(%rax)
    18000935e:	add    %al,(%rax)
-   180009360:	rex.W (bad)
+   180009360:	mov    $0xd5,%eax
 	...
-   18000936e:	add    %al,(%rax)
-   180009370:	insb   (%dx),%es:(%rdi)
+   18000936d:	add    %al,(%rax)
+   18000936f:	add    %bl,%ah
    180009371:	(bad)
    180009372:	add    %al,(%rax)
    180009374:	add    %al,(%rax)
    180009376:	add    %al,(%rax)
-   180009378:	js     0x18000934f
-   18000937a:	add    %al,(%rax)
-   18000937c:	add    %al,(%rax)
-   18000937e:	add    %al,(%rax)
-   180009380:	push   %rdx
+   180009378:	call   0x180009452
+   18000937d:	add    %al,(%rax)
+   18000937f:	add    %al,%dl
    180009381:	(bad)
 	...
    18000938e:	add    %al,(%rax)
-   180009390:	pop    %rax
-   180009391:	(bad)
+   180009390:	enter  $0xd5,$0x0
 	...
-   18000939e:	add    %al,(%rax)
-   1800093a0:	cmp    %dh,%dl
+   1800093a0:	stos   %al,%es:(%rdi)
+   1800093a1:	(bad)
    1800093a2:	add    %al,(%rax)
    1800093a4:	add    %al,(%rax)
    1800093a6:	add    %al,(%rax)
-   1800093a8:	rex.W (bad)
-   1800093aa:	add    %al,(%rax)
-   1800093ac:	add    %al,(%rax)
-   1800093ae:	add    %al,(%rax)
-   1800093b0:	(bad)
-   1800093b1:	(bad)
+   1800093a8:	mov    $0xd6,%eax
+   1800093ad:	add    %al,(%rax)
+   1800093af:	add    %dh,-0x2a(%rsi)
    1800093b2:	add    %al,(%rax)
    1800093b4:	add    %al,(%rax)
    1800093b6:	add    %al,(%rax)
-   1800093b8:	mov    %ss,%esp
+   1800093b8:	cld
+   1800093b9:	(bad)
    1800093ba:	add    %al,(%rax)
    1800093bc:	add    %al,(%rax)
    1800093be:	add    %al,(%rax)
-   1800093c0:	(bad)
-   1800093c1:	(bad)
+   1800093c0:	repnz (bad)
    1800093c2:	add    %al,(%rax)
    1800093c4:	add    %al,(%rax)
    1800093c6:	add    %al,(%rax)
-   1800093c8:	scas   %es:(%rdi),%al
+   1800093c8:	(bad)
    1800093c9:	(bad)
    1800093ca:	add    %al,(%rax)
    1800093cc:	add    %al,(%rax)
    1800093ce:	add    %al,(%rax)
-   1800093d0:	and    %dh,%dl
+   1800093d0:	xchg   %eax,%edx
+   1800093d1:	(bad)
    1800093d2:	add    %al,(%rax)
    1800093d4:	add    %al,(%rax)
    1800093d6:	add    %al,(%rax)
-   1800093d8:	enter  $0xd5,$0x0
+   1800093d8:	cmp    %dl,%dh
+   1800093da:	add    %al,(%rax)
    1800093dc:	add    %al,(%rax)
    1800093de:	add    %al,(%rax)
-   1800093e0:	pushf
-   1800093e1:	(bad)
+   1800093e0:	or     $0xd6,%al
    1800093e2:	add    %al,(%rax)
    1800093e4:	add    %al,(%rax)
    1800093e6:	add    %al,(%rax)
-   1800093e8:	(bad)
+   1800093e8:	pop    %rdx
    1800093e9:	(bad)
    1800093ea:	add    %al,(%rax)
    1800093ec:	add    %al,(%rax)
    1800093ee:	add    %al,(%rax)
-   1800093f0:	mov    %ebp,%ss
+   1800093f0:	(bad)
+   1800093f1:	(bad)
    1800093f2:	add    %al,(%rax)
    1800093f4:	add    %al,(%rax)
    1800093f6:	add    %al,(%rax)
-   1800093f8:	(bad)
-   1800093f9:	(bad)
+   1800093f8:	rcl    %ch
 	...
    180009406:	add    %al,(%rax)
-   180009408:	es (bad)
+   180009408:	xchg   %eax,%esi
+   180009409:	(bad)
    18000940a:	add    %al,(%rax)
    18000940c:	add    %al,(%rax)
    18000940e:	add    %al,(%rax)
-   180009410:	sbb    $0xd5,%al
+   180009410:	mov    %ss,%ebp
    180009412:	add    %al,(%rax)
    180009414:	add    %al,(%rax)
    180009416:	add    %al,(%rax)
-   180009418:	adc    %dl,%ch
-   18000941a:	add    %al,(%rax)
-   18000941c:	add    %al,(%rax)
-   18000941e:	add    %al,(%rax)
-   180009420:	(bad)
-   180009421:	(bad)
+   180009418:	adc    $0x0,%ch
+   18000941b:	add    %al,(%rax)
+   18000941d:	add    %al,(%rax)
+   18000941f:	add    %dh,-0x2b(%rsi)
    180009422:	add    %al,(%rax)
    180009424:	add    %al,(%rax)
    180009426:	add    %al,(%rax)
-   180009428:	(bad)
+   180009428:	outsb  %ds:(%rsi),(%dx)
    180009429:	(bad)
    18000942a:	add    %al,(%rax)
    18000942c:	add    %al,(%rax)
    18000942e:	add    %al,(%rax)
-   180009430:	xor    %dl,%ch
-   180009432:	add    %al,(%rax)
-   180009434:	add    %al,(%rax)
-   180009436:	add    %al,(%rax)
-   180009438:	in     (%dx),%al
+   180009430:	movabs 0x5c000000000000d5,%al
    180009439:	(bad)
    18000943a:	add    %al,(%rax)
    18000943c:	add    %al,(%rax)
    18000943e:	add    %al,(%rax)
-   180009440:	in     $0xd4,%al
+   180009440:	push   %rsp
+   180009441:	(bad)
    180009442:	add    %al,(%rax)
    180009444:	add    %al,(%rax)
    180009446:	add    %al,(%rax)
-   180009448:	fcmovbe %st(4),%st
+   180009448:	rex.WX (bad)
    18000944a:	add    %al,(%rax)
    18000944c:	add    %al,(%rax)
    18000944e:	add    %al,(%rax)
-   180009450:	rcl    %ah
+   180009450:	rex (bad)
    180009452:	add    %al,(%rax)
    180009454:	add    %al,(%rax)
    180009456:	add    %al,(%rax)
-   180009458:	mov    $0xd4,%dl
+   180009458:	and    %ch,%dl
    18000945a:	add    %al,(%rax)
    18000945c:	add    %al,(%rax)
    18000945e:	add    %al,(%rax)
-   180009460:	not    %ah
+   180009460:	data16 (bad)
 	...
    18000946e:	add    %al,(%rax)
-   180009470:	pop    %rsp
-   180009471:	jns    0x180009473
-   180009473:	addb   $0x0,(%rcx)
-   180009476:	add    %al,(%rax)
-   180009478:	pop    %rsp
-   180009479:	jns    0x18000947b
-   18000947b:	addb   $0x0,(%rcx)
-   18000947e:	add    %al,(%rax)
-   180009480:	jo     0x180009402
-   180009482:	add    %al,0x1(%rax)
-   180009488:	nop
-   180009489:	addb   $0x80,(%rax)
+   180009470:	sbb    $0x7c,%al
+   180009472:	add    %al,0x1(%rax)
+   180009478:	sbb    $0x7c,%al
+   18000947a:	add    %al,0x1(%rax)
+   180009480:	xor    %al,0x18000(%rbx)
+   180009486:	add    %al,(%rax)
+   180009488:	push   %rax
+   180009489:	addl   $0xffffff80,(%rax)
    18000948c:	add    %eax,(%rax)
    18000948e:	add    %al,(%rax)
-   180009490:	nop
-   180009491:	addb   $0x80,(%rax)
+   180009490:	push   %rax
+   180009491:	addl   $0xffffff80,(%rax)
    180009494:	add    %eax,(%rax)
 	...
    18000949e:	add    %al,(%rax)
    1800094a0:	add    %dl,(%rax)
    1800094a2:	add    %al,0x1(%rax)
 	...
    1800094e8:	sub    %bl,0x180(%rax,%rax,1)
@@ -11520,17 +11752,17 @@
    18000951b:	add    %al,(%rax)
    18000951d:	add    %al,(%rax)
    18000951f:	add    %dh,-0x5f(%rax)
    180009522:	add    %al,0x1(%rax)
    180009528:	adc    %dh,(%rax,%rax,1)
    18000952b:	addb   $0x0,(%rcx)
    18000952e:	add    %al,(%rax)
-   180009530:	shrb   -0x80(%rax,%rax,1)
-   180009534:	add    %eax,(%rax)
-   180009536:	add    %al,(%rax)
+   180009530:	nop
+   180009531:	outsl  %ds:(%rsi),(%dx)
+   180009532:	add    %al,0x1(%rax)
    180009538:	push   %rbp
    180009539:	outsb  %ds:(%rsi),(%dx)
    18000953a:	imul   $0x77,0x6f(%rsi),%ebp
    18000953e:	outsb  %ds:(%rsi),(%dx)
    18000953f:	and    %ah,0x78(%rbp)
    180009542:	movsxd 0x70(%rbp),%esp
    180009545:	je     0x1800095b0
@@ -11538,26 +11770,26 @@
    180009548:	outsb  %ds:(%rsi),(%dx)
    180009549:	add    %al,(%rax)
    18000954b:	add    %al,(%rax)
    18000954d:	add    %al,(%rax)
    18000954f:	add    %ch,%al
    180009551:	movabs 0x3410000000018000,%eax
    18000955a:	add    %al,0x1(%rax)
-   180009560:	shrb   -0x80(%rax,%rax,1)
-   180009564:	add    %eax,(%rax)
-   180009566:	add    %al,(%rax)
+   180009560:	nop
+   180009561:	outsl  %ds:(%rsi),(%dx)
+   180009562:	add    %al,0x1(%rax)
    180009568:	push   $0x18000a2
    18000956d:	add    %al,(%rax)
    18000956f:	add    %dl,(%rax)
    180009571:	xor    $0x0,%al
    180009573:	addb   $0x0,(%rcx)
    180009576:	add    %al,(%rax)
-   180009578:	shrb   -0x80(%rax,%rax,1)
-   18000957c:	add    %eax,(%rax)
-   18000957e:	add    %al,(%rax)
+   180009578:	nop
+   180009579:	outsl  %ds:(%rsi),(%dx)
+   18000957a:	add    %al,0x1(%rax)
    180009580:	(bad)
    180009585:	jb     0x1800095f9
    180009587:	(bad)
    180009588:	jns    0x1800095aa
    18000958a:	outsb  %ds:(%rsi),(%dx)
    18000958b:	gs ja  0x1800095ae
    18000958e:	insb   (%dx),%es:(%rdi)
@@ -11569,37 +11801,37 @@
    18000959a:	jb     0x180009605
    18000959c:	outsb  %ds:(%rsi),(%dx)
    18000959d:	and    %dh,0x6f(%edi,%ebp,2)
    1800095a2:	and    %ch,0x6e(%rdi,%rbp,2)
    1800095a6:	addr32 add %dh,%al
    1800095a9:	movabs %al,0x3410000000018000
    1800095b2:	add    %al,0x1(%rax)
-   1800095b8:	shrb   -0x80(%rax,%rax,1)
-   1800095bc:	add    %eax,(%rax)
-   1800095be:	add    %al,(%rax)
+   1800095b8:	nop
+   1800095b9:	outsl  %ds:(%rsi),(%dx)
+   1800095ba:	add    %al,0x1(%rax)
    1800095c0:	jo     0x180009565
    1800095c2:	add    %al,0x1(%rax)
    1800095c8:	adc    %dh,(%rax,%rax,1)
    1800095cb:	addb   $0x0,(%rcx)
    1800095ce:	add    %al,(%rax)
-   1800095d0:	shrb   -0x80(%rax,%rax,1)
-   1800095d4:	add    %eax,(%rax)
-   1800095d6:	add    %al,(%rax)
+   1800095d0:	nop
+   1800095d1:	outsl  %ds:(%rsi),(%dx)
+   1800095d2:	add    %al,0x1(%rax)
    1800095d8:	(bad)
    1800095dd:	(bad)
    1800095de:	jae    0x180009654
 	...
    1800095e8:	rex movsb %ds:(%rsi),%es:(%rdi)
    1800095ea:	add    %al,0x1(%rax)
    1800095f0:	adc    %dh,(%rax,%rax,1)
    1800095f3:	addb   $0x0,(%rcx)
    1800095f6:	add    %al,(%rax)
-   1800095f8:	shrb   -0x80(%rax,%rax,1)
-   1800095fc:	add    %eax,(%rax)
-   1800095fe:	add    %al,(%rax)
+   1800095f8:	nop
+   1800095f9:	outsl  %ds:(%rsi),(%dx)
+   1800095fa:	add    %al,0x1(%rax)
    180009600:	pop    %rbx
    180009601:	push   %rsi
    180009602:	(bad)
    180009603:	jb     0x18000966e
    180009605:	(bad)
    180009606:	(bad)
    180009607:	insb   (%dx),%es:(%rdi)
@@ -11658,42 +11890,46 @@
    18000968d:	add    %al,(%rax)
    18000968f:	add    %al,(%rax)
    180009691:	cmp    %al,(%rax)
    180009693:	addb   $0x0,(%rcx)
    180009696:	add    %al,(%rax)
    180009698:	xor    %bh,(%rcx)
    18000969a:	add    %al,0x1(%rax)
-   1800096a0:	and    %cl,0x0(%rdi)
-   1800096a3:	addb   $0x0,(%rcx)
-   1800096a6:	add    %al,(%rax)
-   1800096a8:	rclb   $0x80,0x0(%rax)
+   1800096a0:	(bad)
+   1800096a1:	push   %rdx
+   1800096a2:	add    %al,0x1(%rax)
+   1800096a8:	add    %dl,-0x80(%rax,%rax,1)
    1800096ac:	add    %eax,(%rax)
    1800096ae:	add    %al,(%rax)
-   1800096b0:	out    %al,$0x6f
-   1800096b2:	add    %al,0x1(%rax)
-   1800096b8:	push   %rax
-   1800096b9:	insb   (%dx),%es:(%rdi)
-   1800096ba:	add    %al,0x1(%rax)
-   1800096c0:	movabs 0xf000000001800069,%al
-   1800096c9:	insb   (%dx),%es:(%rdi)
+   1800096b0:	cmpsb  %es:(%rdi),%ds:(%rsi)
+   1800096b1:	jb     0x1800096b3
+   1800096b3:	addb   $0x0,(%rcx)
+   1800096b6:	add    %al,(%rax)
+   1800096b8:	adc    %ch,0x0(%rdi)
+   1800096bb:	addb   $0x0,(%rcx)
+   1800096be:	add    %al,(%rax)
+   1800096c0:	(bad)
+   1800096c1:	insb   (%dx),%es:(%rdi)
+   1800096c2:	add    %al,0x1(%rax)
+   1800096c8:	mov    $0x6f,%al
    1800096ca:	add    %al,0x1(%rax)
-   1800096d0:	(bad)
-   1800096d1:	outsb  %ds:(%rsi),(%dx)
-   1800096d2:	add    %al,0x1(%rax)
-   1800096d8:	add    %dl,-0x80(%rax,%rax,1)
-   1800096dc:	add    %eax,(%rax)
-   1800096de:	add    %al,(%rax)
-   1800096e0:	rclb   -0x80(%rax,%rax,1)
+   1800096d0:	and    %dh,0x0(%rcx)
+   1800096d3:	addb   $0x0,(%rcx)
+   1800096d6:	add    %al,(%rax)
+   1800096d8:	mov    $0x56,%al
+   1800096da:	add    %al,0x1(%rax)
+   1800096e0:	adcb   $0x80,0x0(%rdi)
    1800096e4:	add    %eax,(%rax)
    1800096e6:	add    %al,(%rax)
-   1800096e8:	mov    $0x55,%al
+   1800096e8:	(bad)
+   1800096e9:	pop    %rax
    1800096ea:	add    %al,0x1(%rax)
-   1800096f0:	lock push $0x18000
-   1800096f6:	add    %al,(%rax)
-   1800096f8:	mov    $0x4e,%al
+   1800096f0:	mov    $0x6b,%al
+   1800096f2:	add    %al,0x1(%rax)
+   1800096f8:	lock push %rcx
    1800096fa:	add    %al,0x1(%rax)
    180009700:	sbbb   $0x0,0x18000(%rbp)
    180009707:	add    %cl,(%rax)
    180009709:	xor    (%rax),%eax
    18000970b:	addb   $0x0,(%rcx)
    18000970e:	add    %al,(%rax)
    180009710:	add    %al,(%rax)
@@ -11701,323 +11937,324 @@
    180009714:	mov    $0x0,%eax
    180009719:	add    %al,(%rax)
    18000971b:	add    %ch,0x18000000(%rax)
    180009721:	movsl  %ds:(%rsi),%es:(%rdi)
    180009722:	add    %al,0x1(%rax)
    180009728:	and    %dh,(%rbx)
    18000972a:	add    %al,0x1(%rax)
-   180009730:	nop
-   180009731:	rex.WRX add %r8b,0x1(%rax)
-   180009738:	nop
-   180009739:	rex.WRX add %r8b,0x1(%rax)
-   180009740:	add    %cl,0x0(%rdi)
-   180009743:	addb   $0x0,(%rcx)
-   180009746:	add    %al,(%rax)
-   180009748:	adc    %cl,0x0(%rdi)
-   18000974b:	addb   $0x0,(%rcx)
-   18000974e:	add    %al,(%rax)
-   180009750:	rex imul $0x180,(%rax),%eax
-   180009757:	add    %dl,0x180003c(%rax)
-   18000975d:	add    %al,(%rax)
-   18000975f:	add    %ah,%al
-   180009761:	add    %r8b,0x1(%r8)
-   180009768:	rorb   0x0(%rbx)
-   18000976b:	addb   $0x0,(%rcx)
-   18000976e:	add    %al,(%rax)
-   180009770:	adc    %dl,0x0(%rdx)
+   180009730:	rclb   0x0(%rcx)
+   180009733:	addb   $0x0,(%rcx)
+   180009736:	add    %al,(%rax)
+   180009738:	rclb   0x0(%rcx)
+   18000973b:	addb   $0x0,(%rcx)
+   18000973e:	add    %al,(%rax)
+   180009740:	rex push %rdx
+   180009742:	add    %al,0x1(%rax)
+   180009748:	push   %rax
+   180009749:	push   %rdx
+   18000974a:	add    %al,0x1(%rax)
+   180009750:	add    %ch,-0x80(%rax,%rax,1)
+   180009754:	add    %eax,(%rax)
+   180009756:	add    %al,(%rax)
+   180009758:	nop
+   180009759:	cmp    $0x0,%al
+   18000975b:	addb   $0x0,(%rcx)
+   18000975e:	add    %al,(%rax)
+   180009760:	loopne 0x1800097a7
+   180009762:	add    %al,0x1(%rax)
+   180009768:	push   %rax
+   180009769:	rex.WR add %r8b,0x1(%rax)
+   180009770:	add    %cl,0x0(%rdi)
    180009773:	addb   $0x0,(%rcx)
    180009776:	add    %al,(%rax)
-   180009778:	rclb   0x0(%rcx)
-   18000977b:	addb   $0x0,(%rcx)
-   18000977e:	add    %al,(%rax)
-   180009780:	rolb   0x0(%rdi)
+   180009778:	push   %rax
+   180009779:	push   %rbp
+   18000977a:	add    %al,0x1(%rax)
+   180009780:	adc    %dl,0x0(%rbp)
    180009783:	addb   $0x0,(%rcx)
    180009786:	add    %al,(%rax)
-   180009788:	mov    $0x51,%al
-   18000978a:	add    %al,0x1(%rax)
-   180009790:	(bad)
-   180009791:	add    %r8b,0x1(%r8)
-   180009798:	nop
+   180009788:	push   %rax
+   180009789:	rex.W add %al,0x1(%rax)
+   180009790:	lock push %rsp
+   180009792:	add    %al,0x1(%rax)
+   180009798:	(bad)
    180009799:	add    %r8b,0x1(%r8)
-   1800097a0:	shrb   $0x1,-0x80(%rax,%rax,1)
-   1800097a5:	add    %al,(%rax)
-   1800097a7:	add    %ch,0x69(%rbp)
-   1800097aa:	outsb  %ds:(%rsi),(%dx)
-   1800097ab:	pop    %rdi
-   1800097ac:	movsxd 0x73(%rdi),%ebp
-   1800097af:	je     0x180009824
-   1800097b1:	cs movsxd 0x76(%rbx),%esi
-   1800097b5:	add    %al,(%rax)
-   1800097b7:	add    %cl,(%rdx)
-   1800097b9:	add    %al,(%rax)
-   1800097bb:	add    %al,(%rax)
+   1800097a0:	nop
+   1800097a1:	add    %r8b,0x1(%r8)
+   1800097a8:	subb   $0x80,0x0(%rdi)
+   1800097ac:	add    %eax,(%rax)
+   1800097ae:	add    %al,(%rax)
+   1800097b0:	insl   (%dx),%es:(%rdi)
+   1800097b1:	imul   $0x74736f63,0x5f(%rsi),%ebp
+   1800097b8:	jae    0x1800097e8
+   1800097ba:	movsxd 0x76(%rbx),%esi
    1800097bd:	add    %al,(%rax)
-   1800097bf:	add    %ch,0x62(%rsi)
-   1800097c2:	pop    %rdi
-   1800097c3:	je     0x180009837
-   1800097c5:	imul   $0x73656c67,0x6e(%rcx),%esp
-   1800097cc:	sub    $0x6d,%al
-   1800097ce:	imul   $0x74736f63,0x5f(%rsi),%ebp
-   1800097d5:	add    %al,(%rax)
-   1800097d7:	add    %ah,(%rax)
-   1800097d9:	cmp    $0x20,%eax
-   1800097de:	add    %al,(%rax)
-   1800097e0:	outsb  %ds:(%rsi),(%dx)
-   1800097e1:	(bad)
-   1800097e2:	pop    %rdi
-   1800097e3:	(bad)
-   1800097e4:	movsxd 0x76(%rcx,%rbp,2),%esi
-   1800097e8:	gs pop %rdi
-   1800097ea:	jo     0x18000985b
-   1800097ec:	insb   (%dx),%es:(%rdi)
-   1800097ed:	jns    0x180009856
-   1800097ef:	outsl  %ds:(%rsi),(%dx)
-   1800097f0:	outsb  %ds:(%rsi),(%dx)
-   1800097f1:	jae    0x1800097f3
-   1800097f3:	add    %ch,(%rax,%rax,1)
-   1800097f6:	add    %al,(%rax)
-   1800097f8:	insl   (%dx),%es:(%rdi)
-   1800097f9:	gs jae 0x180009864
-   1800097fc:	pop    %rdi
-   1800097fd:	outsb  %ds:(%rsi),(%dx)
-   1800097ff:	(bad)
-   180009800:	pop    %rdi
-   180009801:	jo     0x180009872
-   180009803:	insb   (%dx),%es:(%rdi)
-   180009804:	jns    0x18000986d
-   180009806:	outsl  %ds:(%rsi),(%dx)
-   180009807:	outsb  %ds:(%rsi),(%dx)
-   180009808:	jae    0x180009832
-   18000980a:	sub    %eax,(%rax)
-   18000980c:	add    %al,(%rax)
-   18000980e:	add    %al,(%rax)
-   180009810:	insl   (%dx),%es:(%rdi)
-   180009811:	outsl  %ds:(%rsi),(%dx)
-   180009812:	imul   $0x695f6465,%fs:0x69(%rsi),%esp
-   18000981a:	je     0x180009881
-   18000981c:	jb     0x18000984f
-   18000981e:	outsl  %ds:(%rsi),(%dx)
-   180009820:	addr32 pop %rdi
-   180009822:	je     0x180009897
-   180009824:	xor    0x76(%rax,%rax,1),%sp
-   180009829:	movsxd %gs:0x72(%rdi,%rbp,2),%esi
-   18000982e:	and    %dh,0x6f(%rdi,%rbp,2)
-   180009832:	and    %ch,0x6e(%rdi,%rbp,2)
-   180009836:	addr32 add %bh,%al
-   180009839:	movsl  %ds:(%rsi),%es:(%rdi)
-   18000983a:	add    %al,0x1(%rax)
-   180009840:	shlb   (%rsi)
+   1800097bf:	add    %cl,(%rdx)
+   1800097c1:	add    %al,(%rax)
+   1800097c3:	add    %al,(%rax)
+   1800097c5:	add    %al,(%rax)
+   1800097c7:	add    %ch,0x62(%rsi)
+   1800097ca:	pop    %rdi
+   1800097cb:	je     0x18000983f
+   1800097cd:	imul   $0x73656c67,0x6e(%rcx),%esp
+   1800097d4:	sub    $0x6d,%al
+   1800097d6:	imul   $0x74736f63,0x5f(%rsi),%ebp
+   1800097dd:	add    %al,(%rax)
+   1800097df:	add    %ah,(%rax)
+   1800097e1:	cmp    $0x20,%eax
+   1800097e6:	add    %al,(%rax)
+   1800097e8:	outsb  %ds:(%rsi),(%dx)
+   1800097e9:	(bad)
+   1800097ea:	pop    %rdi
+   1800097eb:	(bad)
+   1800097ec:	movsxd 0x76(%rcx,%rbp,2),%esi
+   1800097f0:	gs pop %rdi
+   1800097f2:	jo     0x180009863
+   1800097f4:	insb   (%dx),%es:(%rdi)
+   1800097f5:	jns    0x18000985e
+   1800097f7:	outsl  %ds:(%rsi),(%dx)
+   1800097f8:	outsb  %ds:(%rsi),(%dx)
+   1800097f9:	jae    0x1800097fb
+   1800097fb:	add    %ch,(%rax,%rax,1)
+   1800097fe:	add    %al,(%rax)
+   180009800:	insl   (%dx),%es:(%rdi)
+   180009801:	gs jae 0x18000986c
+   180009804:	pop    %rdi
+   180009805:	outsb  %ds:(%rsi),(%dx)
+   180009807:	(bad)
+   180009808:	pop    %rdi
+   180009809:	jo     0x18000987a
+   18000980b:	insb   (%dx),%es:(%rdi)
+   18000980c:	jns    0x180009875
+   18000980e:	outsl  %ds:(%rsi),(%dx)
+   18000980f:	outsb  %ds:(%rsi),(%dx)
+   180009810:	jae    0x18000983a
+   180009812:	sub    %eax,(%rax)
+   180009814:	add    %al,(%rax)
+   180009816:	add    %al,(%rax)
+   180009818:	insl   (%dx),%es:(%rdi)
+   180009819:	outsl  %ds:(%rsi),(%dx)
+   18000981a:	imul   $0x695f6465,%fs:0x69(%rsi),%esp
+   180009822:	je     0x180009889
+   180009824:	jb     0x180009857
+   180009826:	outsl  %ds:(%rsi),(%dx)
+   180009828:	addr32 pop %rdi
+   18000982a:	je     0x18000989f
+   18000982c:	xor    0x76(%rax,%rax,1),%sp
+   180009831:	movsxd %gs:0x72(%rdi,%rbp,2),%esi
+   180009836:	and    %dh,0x6f(%rdi,%rbp,2)
+   18000983a:	and    %ch,0x6e(%rdi,%rbp,2)
+   18000983e:	addr32 add %bh,%al
+   180009841:	movsl  %ds:(%rsi),%es:(%rdi)
    180009842:	add    %al,0x1(%rax)
-   180009848:	mov    $0x36,%al
+   180009848:	shlb   (%rsi)
    18000984a:	add    %al,0x1(%rax)
-   180009850:	(bad)
-   180009851:	xor    (%rax),%eax
-   180009853:	addb   $0x0,(%rcx)
-   180009856:	add    %al,(%rax)
-   180009858:	loopne 0x180009891
-   18000985a:	add    %al,0x1(%rax)
-   180009860:	pop    %rbx
-   180009861:	push   %rax
-   180009862:	outsl  %ds:(%rsi),(%dx)
-   180009863:	imul   $0x706f3a3a,0x74(%rsi),%ebp
-   18000986a:	gs jb  0x1800098ce
-   18000986d:	je     0x1800098de
-   18000986f:	jb     0x1800098a0
-   180009871:	pop    %rbp
-   180009872:	and    %al,0x61(%rbx)
-   180009875:	outsb  %ds:(%rsi),(%dx)
-   180009876:	outsb  %ds:(%rsi),(%dx)
-   180009877:	outsl  %ds:(%rsi),(%dx)
-   180009878:	je     0x18000989a
-   18000987a:	imul   $0x50206564,%fs:0x69(%rsi),%esi
-   180009882:	outsl  %ds:(%rsi),(%dx)
-   180009883:	imul   $0x20796220,0x74(%rsi),%ebp
-   18000988a:	jae    0x1800098fb
-   18000988c:	insl   (%dx),%es:(%rdi)
-   18000988d:	gs je  0x1800098f8
-   180009890:	imul   $0x6f6c6320,0x67(%rsi),%ebp
-   180009897:	jae    0x1800098fe
-   180009899:	and    %dh,0x20(%rdi,%rbp,2)
-   18000989d:	jp     0x180009904
-   18000989f:	jb     0x180009910
-   1800098a1:	add    %al,(%rax)
-   1800098a3:	add    %al,(%rax)
-   1800098a5:	add    %al,(%rax)
-   1800098a7:	add    %dh,0x65(%rsi)
-   1800098aa:	movsxd 0x72(%rdi,%rbp,2),%esi
-   1800098ae:	cmp    $0x62,%al
-   1800098b0:	outsl  %ds:(%rsi),(%dx)
-   1800098b1:	outsl  %ds:(%rsi),(%dx)
-   1800098b2:	insb   (%dx),%es:(%rdi)
-   1800098b3:	ds and %dh,0x6f(%rdi,%rbp,2)
-   1800098b8:	and    %ch,0x6e(%rdi,%rbp,2)
-   1800098bc:	add    %al,(%eax)
-   1800098bf:	add    %bl,0x41(%rbx)
-   1800098c2:	je     0x180009938
-   1800098c4:	jb     0x18000992f
-   1800098c6:	(bad)
-   1800098cb:	(bad)
-   1800098cc:	outsb  %ds:(%rsi),(%dx)
-   1800098cd:	(bad)
-   1800098ce:	addr32 gs jb 0x18000990c
-   1800098d2:	cmp    0x69(%rsi),%ah
-   1800098d5:	outsb  %ds:(%rsi),(%dx)
-   1800098d6:	fs pop %rdi
-   1800098d8:	outsl  %ds:(%rsi),(%dx)
-   1800098d9:	jb     0x18000993a
-   1800098db:	movsxd 0x65(%rdx),%esi
-   1800098de:	(bad)
-   1800098df:	je     0x180009946
-   1800098e1:	pop    %rdi
-   1800098e2:	(bad)
-   1800098e3:	je     0x180009959
-   1800098e5:	jb     0x180009950
-   1800098e7:	(bad)
-   1800098ec:	and    %al,0x20(%rdi,%rbp,2)
-   1800098f0:	outsb  %ds:(%rsi),(%dx)
-   1800098f1:	outsl  %ds:(%rsi),(%dx)
-   1800098f2:	je     0x180009914
-   1800098f4:	imul   $0x746e6174,0x73(%rsi),%ebp
-   1800098fb:	imul   $0x6e612065,0x74(%rcx),%esp
-   180009902:	and    %ah,0x74(%rcx)
-   180009905:	je     0x180009979
-   180009907:	imul   $0x69206574,0x75(%rdx),%esp
-   18000990e:	data16 and %ah,0x6e(%rcx)
-   180009912:	and    %ch,0x6e(%rcx)
-   180009915:	jae    0x18000998b
-   180009917:	(bad)
-   180009918:	outsb  %ds:(%rsi),(%dx)
-   180009919:	je     0x180009984
-   18000991b:	(bad)
-   18000991c:	je     0x180009983
-   18000991e:	and    %ah,%fs:0x74(%rcx)
-   180009922:	je     0x180009996
-   180009924:	imul   $0x6f206574,0x75(%rdx),%esp
-   18000992b:	data16 and %dh,0x65(%rax,%rbp,2)
-   180009930:	and    %dh,0x61(%rbx)
-   180009933:	insl   (%dx),%es:(%rdi)
-   180009934:	and    %ch,%gs:0x61(%rsi)
-   180009938:	insl   (%dx),%es:(%rdi)
-   180009939:	and    %dh,%gs:0x69(%rdi)
-   18000993d:	je     0x1800099a7
-   18000993f:	and    %ah,0x66(%rcx,%rbp,2)
-   180009943:	data16 gs jb 0x1800099ac
-   180009947:	outsb  %ds:(%rsi),(%dx)
-   180009948:	je     0x18000996a
-   18000994a:	jae    0x1800099c0
-   18000994c:	outsl  %ds:(%rsi),(%dx)
-   18000994d:	jb     0x1800099b0
-   18000994f:	and    %ah,%gs:0x6c(%ecx)
-   180009954:	jb     0x1800099bb
-   180009956:	(bad)
-   180009957:	fs jns 0x18000997a
-   18000995a:	gs js  0x1800099c6
-   18000995d:	jae    0x1800099d3
-   18000995f:	jae    0x18000998f
-   180009961:	add    %al,(%rax)
-   180009963:	add    %al,(%rax)
-   180009965:	add    %al,(%rax)
-   180009967:	add    %ah,0x4bfeebc2(%rax)
-   18000996d:	rex.W mov $0x39,%spl
-   180009970:	int1
-   180009971:	push   $0xfffffffff8b588e3
-   180009976:	in     $0x3e,%al
-   180009978:	cld
-   180009979:	test   $0x624dd2f1,%eax
-   18000997e:	rex (bad)
-   180009980:	add    %al,(%rax)
-   180009982:	add    %al,(%rax)
-   180009984:	add    %al,(%rax)
-   180009986:	lock (bad)
-	...
-   180009990:	(bad)
-   180009991:	(bad)
-   180009992:	(bad)
-   180009993:	(bad)
-   180009994:	(bad)
-   180009995:	(bad)
-   180009996:	(bad)
-   180009997:	jg     0x180009998
-   180009999:	(bad)
-   18000999a:	(bad)
-   18000999b:	(bad)
-   18000999c:	(bad)
-   18000999d:	(bad)
-   18000999e:	(bad)
-   18000999f:	jg     0x180009a19
-   1800099a1:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   1800099a2:	add    %al,0x1(%rax)
-   1800099a8:	or     %dh,0x0(%rcx)
-   1800099ab:	addb   $0x0,(%rcx)
-	...
-   1800099be:	add    %al,(%rax)
-   1800099c0:	(bad)
-   1800099c1:	(bad)
-   1800099c2:	(bad)
-   1800099c3:	(bad)
-   1800099c4:	(bad)
-   1800099c5:	(bad)
-   1800099c6:	(bad)
-   1800099c7:	(bad)
-   1800099c8:	(bad)
-   1800099c9:	(bad)
-   1800099ca:	(bad)
-   1800099cb:	(bad)
-   1800099cc:	(bad)
-   1800099cd:	(bad)
-   1800099ce:	(bad)
-   1800099cf:	jmp    *0x61(%rdx)
-   1800099d2:	and    %ah,%fs:0x6c(%rcx)
-   1800099d6:	insb   (%dx),%es:(%rdi)
-   1800099d7:	outsl  %ds:(%rsi),(%dx)
-   1800099d8:	movsxd 0x74(%rcx),%esp
-   1800099db:	imul   $0xe6c00000,0x6e(%rdi),%ebp
-   1800099e2:	add    %al,0x1(%rax)
-   1800099e8:	(bad)
-   1800099e9:	out    %eax,$0x0
-   1800099eb:	addb   $0x0,(%rcx)
-   1800099ee:	add    %al,(%rax)
-   1800099f0:	add    %al,(%rax)
-   1800099f2:	add    %al,(%rax)
-   1800099f4:	iret
-   1800099f5:	(bad)
-   1800099f6:	push   %rdx
-   1800099f7:	add    %al,%fs:(%rax)
+   180009850:	mov    $0x36,%al
+   180009852:	add    %al,0x1(%rax)
+   180009858:	(bad)
+   180009859:	xor    (%rax),%eax
+   18000985b:	addb   $0x0,(%rcx)
+   18000985e:	add    %al,(%rax)
+   180009860:	loopne 0x180009899
+   180009862:	add    %al,0x1(%rax)
+	...
+   180009870:	pop    %rbx
+   180009871:	push   %rax
+   180009872:	outsl  %ds:(%rsi),(%dx)
+   180009873:	imul   $0x706f3a3a,0x74(%rsi),%ebp
+   18000987a:	gs jb  0x1800098de
+   18000987d:	je     0x1800098ee
+   18000987f:	jb     0x1800098b0
+   180009881:	pop    %rbp
+   180009882:	and    %al,0x61(%rbx)
+   180009885:	outsb  %ds:(%rsi),(%dx)
+   180009886:	outsb  %ds:(%rsi),(%dx)
+   180009887:	outsl  %ds:(%rsi),(%dx)
+   180009888:	je     0x1800098aa
+   18000988a:	imul   $0x50206564,%fs:0x69(%rsi),%esi
+   180009892:	outsl  %ds:(%rsi),(%dx)
+   180009893:	imul   $0x20796220,0x74(%rsi),%ebp
+   18000989a:	jae    0x18000990b
+   18000989c:	insl   (%dx),%es:(%rdi)
+   18000989d:	gs je  0x180009908
+   1800098a0:	imul   $0x6f6c6320,0x67(%rsi),%ebp
+   1800098a7:	jae    0x18000990e
+   1800098a9:	and    %dh,0x20(%rdi,%rbp,2)
+   1800098ad:	jp     0x180009914
+   1800098af:	jb     0x180009920
+   1800098b1:	add    %al,(%rax)
+   1800098b3:	add    %al,(%rax)
+   1800098b5:	add    %al,(%rax)
+   1800098b7:	add    %dh,0x65(%rsi)
+   1800098ba:	movsxd 0x72(%rdi,%rbp,2),%esi
+   1800098be:	cmp    $0x62,%al
+   1800098c0:	outsl  %ds:(%rsi),(%dx)
+   1800098c1:	outsl  %ds:(%rsi),(%dx)
+   1800098c2:	insb   (%dx),%es:(%rdi)
+   1800098c3:	ds and %dh,0x6f(%rdi,%rbp,2)
+   1800098c8:	and    %ch,0x6e(%rdi,%rbp,2)
+   1800098cc:	add    %al,(%eax)
+   1800098cf:	add    %bl,0x41(%rbx)
+   1800098d2:	je     0x180009948
+   1800098d4:	jb     0x18000993f
+   1800098d6:	(bad)
+   1800098db:	(bad)
+   1800098dc:	outsb  %ds:(%rsi),(%dx)
+   1800098dd:	(bad)
+   1800098de:	addr32 gs jb 0x18000991c
+   1800098e2:	cmp    0x69(%rsi),%ah
+   1800098e5:	outsb  %ds:(%rsi),(%dx)
+   1800098e6:	fs pop %rdi
+   1800098e8:	outsl  %ds:(%rsi),(%dx)
+   1800098e9:	jb     0x18000994a
+   1800098eb:	movsxd 0x65(%rdx),%esi
+   1800098ee:	(bad)
+   1800098ef:	je     0x180009956
+   1800098f1:	pop    %rdi
+   1800098f2:	(bad)
+   1800098f3:	je     0x180009969
+   1800098f5:	jb     0x180009960
+   1800098f7:	(bad)
+   1800098fc:	and    %al,0x20(%rdi,%rbp,2)
+   180009900:	outsb  %ds:(%rsi),(%dx)
+   180009901:	outsl  %ds:(%rsi),(%dx)
+   180009902:	je     0x180009924
+   180009904:	imul   $0x746e6174,0x73(%rsi),%ebp
+   18000990b:	imul   $0x6e612065,0x74(%rcx),%esp
+   180009912:	and    %ah,0x74(%rcx)
+   180009915:	je     0x180009989
+   180009917:	imul   $0x69206574,0x75(%rdx),%esp
+   18000991e:	data16 and %ah,0x6e(%rcx)
+   180009922:	and    %ch,0x6e(%rcx)
+   180009925:	jae    0x18000999b
+   180009927:	(bad)
+   180009928:	outsb  %ds:(%rsi),(%dx)
+   180009929:	je     0x180009994
+   18000992b:	(bad)
+   18000992c:	je     0x180009993
+   18000992e:	and    %ah,%fs:0x74(%rcx)
+   180009932:	je     0x1800099a6
+   180009934:	imul   $0x6f206574,0x75(%rdx),%esp
+   18000993b:	data16 and %dh,0x65(%rax,%rbp,2)
+   180009940:	and    %dh,0x61(%rbx)
+   180009943:	insl   (%dx),%es:(%rdi)
+   180009944:	and    %ch,%gs:0x61(%rsi)
+   180009948:	insl   (%dx),%es:(%rdi)
+   180009949:	and    %dh,%gs:0x69(%rdi)
+   18000994d:	je     0x1800099b7
+   18000994f:	and    %ah,0x66(%rcx,%rbp,2)
+   180009953:	data16 gs jb 0x1800099bc
+   180009957:	outsb  %ds:(%rsi),(%dx)
+   180009958:	je     0x18000997a
+   18000995a:	jae    0x1800099d0
+   18000995c:	outsl  %ds:(%rsi),(%dx)
+   18000995d:	jb     0x1800099c0
+   18000995f:	and    %ah,%gs:0x6c(%ecx)
+   180009964:	jb     0x1800099cb
+   180009966:	(bad)
+   180009967:	fs jns 0x18000998a
+   18000996a:	gs js  0x1800099d6
+   18000996d:	jae    0x1800099e3
+   18000996f:	jae    0x18000999f
+   180009971:	add    %al,(%rax)
+   180009973:	add    %al,(%rax)
+   180009975:	add    %al,(%rax)
+   180009977:	add    %ah,0x4bfeebc2(%rax)
+   18000997d:	rex.W mov $0x39,%spl
+   180009980:	int1
+   180009981:	push   $0xfffffffff8b588e3
+   180009986:	in     $0x3e,%al
+   180009988:	cld
+   180009989:	test   $0x624dd2f1,%eax
+   18000998e:	rex (bad)
+   180009990:	add    %al,(%rax)
+   180009992:	add    %al,(%rax)
+   180009994:	add    %al,(%rax)
+   180009996:	lock (bad)
+	...
+   1800099a0:	(bad)
+   1800099a1:	(bad)
+   1800099a2:	(bad)
+   1800099a3:	(bad)
+   1800099a4:	(bad)
+   1800099a5:	(bad)
+   1800099a6:	(bad)
+   1800099a7:	jg     0x1800099a8
+   1800099a9:	(bad)
+   1800099aa:	(bad)
+   1800099ab:	(bad)
+   1800099ac:	(bad)
+   1800099ad:	(bad)
+   1800099ae:	(bad)
+   1800099af:	jg     0x1800099b0
+   1800099b1:	(bad)
+   1800099b2:	(bad)
+   1800099b3:	(bad)
+   1800099b4:	(bad)
+   1800099b5:	(bad)
+   1800099b6:	(bad)
+   1800099b7:	(bad)
+   1800099b8:	(bad)
+   1800099b9:	(bad)
+   1800099ba:	(bad)
+   1800099bb:	(bad)
+   1800099bc:	(bad)
+   1800099bd:	(bad)
+   1800099be:	(bad)
+   1800099bf:	(bad)
+   1800099c0:	js     0x180009968
+   1800099c2:	add    %al,0x1(%rax)
+   1800099c8:	enter  $0x73,$0x80
+   1800099cc:	add    %eax,(%rax)
+	...
+   1800099d6:	add    %al,(%rax)
+   1800099d8:	(bad)
+   1800099dd:	insb   (%dx),%es:(%rdi)
+   1800099de:	insb   (%dx),%es:(%rdi)
+   1800099df:	outsl  %ds:(%rsi),(%dx)
+   1800099e0:	movsxd 0x74(%rcx),%esp
+   1800099e3:	imul   $0xe6c00000,0x6e(%rdi),%ebp
+   1800099ea:	add    %al,0x1(%rax)
+   1800099f0:	(bad)
+   1800099f1:	out    %eax,$0x0
+   1800099f3:	addb   $0x0,(%rcx)
+   1800099f6:	add    %al,(%rax)
+   1800099f8:	add    %al,(%rax)
    1800099fa:	add    %al,(%rax)
-   1800099fc:	or     $0xb8000000,%eax
-   180009a01:	add    (%rax),%al
-   180009a03:	add    %dh,0x0(%rdi,%riz,4)
-   180009a07:	add    %dh,0x0(%rbx,%rdx,4)
-   180009a0b:	add    %al,(%rax)
-   180009a0d:	add    %al,(%rax)
-   180009a0f:	add    %bh,(%rax)
-   180009a11:	add    %eax,(%rax)
-	...
-   180009a67:	add    %cl,(%rax)
-   180009a69:	loopne 0x180009a6b
-   180009a6b:	addb   $0x0,(%rcx)
-	...
-   180009a7e:	add    %al,(%rax)
-   180009a80:	jo     0x180009a16
-   180009a82:	add    %al,0x1(%rax)
-   180009a88:	adcb   $0x0,0x180(%rax,%rax,1)
-	...
-   180009aa0:	add    %al,(%rcx)
-	...
-   180009b0e:	add    %al,(%rax)
-   180009b10:	in     (%dx),%al
-   180009b11:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   180009b12:	add    %al,0x1(%rax)
-	...
-   180009b28:	js     0x180009abe
-   180009b2a:	add    %al,0x1(%rax)
-   180009b30:	mov    %dl,0x180(%rax,%rax,1)
-   180009b37:	add    %dl,0x1800094(%rax)
-   180009b3d:	add    %al,(%rax)
-   180009b3f:	add    %dh,0x18000e6(%rax)
+   1800099fc:	movabs %al,0xd00000000648844
+   180009a05:	add    %al,(%rax)
+   180009a07:	add    %bh,0x74000002(%rax)
+   180009a0d:	cmpsl  %es:(%rdi),%ds:(%rsi)
+   180009a0e:	add    %al,(%rax)
+   180009a10:	je     0x1800099a9
+	...
+   180009a1e:	add    %al,(%rax)
+   180009a20:	cmp    %al,(%rcx)
+	...
+   180009a76:	add    %al,(%rax)
+   180009a78:	or     %ah,%al
+   180009a7a:	add    %al,0x1(%rax)
+	...
+   180009a90:	jo     0x180009a26
+   180009a92:	add    %al,0x1(%rax)
+   180009a98:	adcb   $0x0,0x180(%rax,%rax,1)
+	...
+   180009ab0:	add    %al,(%rcx)
+	...
+   180009b1e:	add    %al,(%rax)
+   180009b20:	in     (%dx),%al
+   180009b21:	cmpsb  %es:(%rdi),%ds:(%rsi)
+   180009b22:	add    %al,0x1(%rax)
+	...
+   180009b38:	js     0x180009ace
+   180009b3a:	add    %al,0x1(%rax)
+   180009b40:	mov    %dl,0x180(%rax,%rax,1)
+   180009b47:	add    %dl,0x1800094(%rax)
+   180009b4d:	add    %al,(%rax)
+   180009b4f:	add    %dh,0x18000e6(%rax)
 	...
    180009b7d:	add    %al,(%rax)
    180009b7f:	add    %dh,-0x1e(%rax)
    180009b82:	add    %al,(%rax)
    180009b84:	add    %eax,(%rax)
    180009b86:	add    %al,(%rax)
    180009b88:	add    %al,(%rax)
@@ -12807,67 +13044,72 @@
    18000a728:	push   %rdi
    18000a729:	sub    (%rax),%al
    18000a72b:	add    %bh,%bl
    18000a72d:	sub    $0x2e0d0000,%eax
    18000a732:	add    %al,(%rax)
    18000a734:	xchg   %eax,%esi
    18000a735:	xor    %eax,(%rax)
-   18000a737:	add    %ch,-0x3bffffcf(%rax)
-   18000a73d:	push   %rsi
+   18000a737:	add    %ch,0x74000031(%rax)
+   18000a73d:	pop    %rcx
    18000a73e:	add    %al,(%rax)
-   18000a740:	(bad)
-   18000a741:	push   %rsi
-   18000a742:	add    %al,(%rax)
-   18000a744:	loopne 0x18000a6c6
-   18000a746:	add    %al,(%rax)
-   18000a748:	and    %al,-0x7ec00000(%rcx)
-   18000a74e:	add    %al,(%rax)
-   18000a750:	jo     0x18000a6d3
-   18000a752:	add    %al,(%rax)
-   18000a754:	movabs 0x10000081d0000081,%al
-   18000a75d:	addl   $0x0,(%rax)
-   18000a760:	rolb   0x10100000(%rbx)
-   18000a766:	add    %al,(%rax)
-   18000a768:	and    $0x5f,%al
+   18000a740:	xchg   %bl,0x0(%rcx)
+   18000a743:	add    %ah,-0x1fffff7d(%rax)
+   18000a749:	addl   $0x0,(%rax)
+   18000a74c:	add    %al,0x843000(%rax,%rax,1)
+   18000a753:	add    %ah,-0x7c(%rax)
+   18000a756:	add    %al,(%rax)
+   18000a758:	nop
+   18000a759:	test   %al,(%rax)
+   18000a75b:	add    %dl,%al
+   18000a75d:	test   %eax,(%rax)
+   18000a75f:	add    %dl,0x10000086(%rax)
+   18000a765:	adc    %al,(%rax)
+   18000a767:	add    %ah,%ah
+   18000a769:	(bad)
    18000a76a:	add    %al,(%rax)
-   18000a76c:	movabs 0x4cc000080,%al
-   18000a775:	add    %al,(%rax)
-   18000a777:	add    %al,(%rax)
-   18000a779:	adc    %al,(%rax)
-   18000a77b:	add    %dl,(%rax)
-   18000a77d:	add    %al,(%rax)
-   18000a77f:	add    %ch,(%rsi)
-   18000a781:	je     0x18000a7e8
+   18000a76c:	(bad)
+   18000a76d:	addl   $0x0,(%rax)
+   18000a770:	sub    $0x5,%al
+   18000a772:	add    %al,(%rax)
+   18000a774:	add    %al,(%rax)
+   18000a776:	add    %al,(%rax)
+   18000a778:	add    %dl,(%rax)
+   18000a77a:	add    %al,(%rax)
+   18000a77c:	adc    %al,(%rax)
+   18000a77e:	add    %al,(%rax)
+   18000a780:	je,pn  0x18000a7e8
    18000a783:	js     0x18000a7f9
    18000a785:	and    $0x64,%al
    18000a787:	imul   $0x10000000,(%rax),%eax
    18000a78d:	adc    %al,(%rax)
-   18000a78f:	add    %dl,0x70(%rax)
-   18000a792:	add    %al,(%rax)
-   18000a794:	je,pn  0x18000a7fc
+   18000a78f:	add    %dl,(%rax)
+   18000a791:	jae    0x18000a793
+   18000a793:	add    %ch,(%rsi)
+   18000a795:	je     0x18000a7fc
    18000a797:	js     0x18000a80d
    18000a799:	and    $0x6d,%al
    18000a79b:	outsb  %ds:(%rsi),(%dx)
    18000a79c:	add    %al,(%rax)
    18000a79e:	add    %al,(%rax)
-   18000a7a0:	(bad)
-   18000a7a1:	addb   $0x0,(%rax)
-   18000a7a4:	rex add %al,(%rax)
-   18000a7a7:	add    %ch,(%rsi)
-   18000a7a9:	je     0x18000a810
+   18000a7a0:	and    %al,0x400000(%rbx)
+   18000a7a6:	add    %al,(%rax)
+   18000a7a8:	je,pn  0x18000a810
    18000a7ab:	js     0x18000a821
    18000a7ad:	and    $0x6d,%al
    18000a7af:	outsb  %ds:(%rsi),(%dx)
    18000a7b0:	and    $0x30,%al
    18000a7b2:	xor    %al,(%rax)
-   18000a7b4:	movabs 0x2e000005ec000080,%al
-   18000a7bd:	je     0x18000a824
+   18000a7b4:	(bad)
+   18000a7b5:	addl   $0x0,(%rax)
+   18000a7b8:	rex.WR (bad)
+   18000a7ba:	add    %al,(%rax)
+   18000a7bc:	je,pn  0x18000a824
    18000a7bf:	js     0x18000a835
    18000a7c1:	and    $0x78,%al
-   18000a7c3:	add    %cl,0x5b0000(%rsi,%rax,4)
+   18000a7c3:	add    %ch,0x5b0000(%rcx,%rcx,4)
    18000a7ca:	add    %al,(%rax)
    18000a7cc:	je,pn  0x18000a834
    18000a7cf:	js     0x18000a845
    18000a7d1:	and    $0x79,%al
    18000a7d3:	add    %al,%fs:(%rax)
    18000a7d6:	add    %al,(%rax)
    18000a7d8:	add    %dl,0x4700000(%rax)
@@ -13032,54 +13274,56 @@
    18000a94e:	pop    %rdx
    18000a94f:	pop    %rdx
    18000a950:	add    %al,(%rax)
    18000a952:	add    %al,(%rax)
    18000a954:	push   %rax
    18000a955:	stos   %al,%es:(%rdi)
    18000a956:	add    %al,(%rax)
-   18000a958:	cwtl
-   18000a959:	or     (%rax),%eax
+   18000a958:	or     %cl,(%rax,%rax,1)
    18000a95b:	add    %ch,(%rsi)
    18000a95d:	js     0x18000a9c3
    18000a95f:	(bad)
    18000a960:	je     0x18000a9c3
    18000a962:	add    %al,(%rax)
-   18000a964:	call   0x16800aa1e
+   18000a964:	pop    %rax
+   18000a965:	mov    $0x0,%dh
+   18000a967:	add    %ch,%al
    18000a969:	add    %eax,(%rax)
    18000a96b:	add    %ch,(%rsi)
    18000a96d:	js     0x18000a9d3
    18000a96f:	(bad)
    18000a970:	je     0x18000a9d3
    18000a972:	and    $0x78,%al
    18000a974:	add    %al,(%rax)
    18000a976:	add    %al,(%rax)
-   18000a978:	shlb   0x1a40000(%rdi)
+   18000a978:	rex mov $0x1a40000,%eax
    18000a97e:	add    %al,(%rax)
    18000a980:	cs gs fs (bad)
    18000a984:	je     0x18000a9e7
    18000a986:	add    %al,(%rax)
-   18000a988:	je     0x18000a943
+   18000a988:	in     $0xb9,%al
    18000a98a:	add    %al,(%rax)
    18000a98c:	sbb    %al,(%rcx)
    18000a98e:	add    %al,(%rax)
    18000a990:	cs imul $0x322461,0x74(%rcx,%riz,2),%esp
    18000a999:	add    %al,(%rax)
-   18000a99b:	add    %cl,0x140000(%rdx,%rdi,4)
+   18000a99b:	add    %bh,%ah
+   18000a99d:	mov    $0x140000,%edx
    18000a9a2:	add    %al,(%rax)
    18000a9a4:	cs imul $0x332461,0x74(%rcx,%riz,2),%esp
    18000a9ad:	add    %al,(%rax)
-   18000a9af:	add    %ah,0x700000ba(%rax)
-   18000a9b5:	add    $0x0,%al
-   18000a9b7:	add    %ch,(%rsi)
-   18000a9b9:	imul   $0x342461,0x74(%rcx,%riz,2),%esp
+   18000a9af:	add    %dl,(%rax)
+   18000a9b1:	mov    $0x4700000,%ebx
+   18000a9b6:	add    %al,(%rax)
+   18000a9b8:	cs imul $0x342461,0x74(%rcx,%riz,2),%esp
    18000a9c1:	add    %al,(%rax)
-   18000a9c3:	add    %dl,(%rax)
-   18000a9c5:	mov    $0x19660000,%edi
-   18000a9ca:	add    %al,(%rax)
-   18000a9cc:	cs imul $0x362461,0x74(%rcx,%riz,2),%esp
+   18000a9c3:	add    %al,0x660000bf(%rax)
+   18000a9c9:	sbb    %eax,(%rax)
+   18000a9cb:	add    %ch,(%rsi)
+   18000a9cd:	imul   $0x362461,0x74(%rcx,%riz,2),%esp
    18000a9d5:	add    %al,(%rax)
    18000a9d7:	add    %al,(%rax)
    18000a9d9:	loopne 0x18000a9db
    18000a9db:	add    %al,0x0(%rax)
    18000a9de:	add    %al,(%rax)
    18000a9e0:	cs fs (bad)
    18000a9e3:	je     0x18000aa46
@@ -13106,35 +13350,42 @@
    18000aa11:	(bad)
    18000aa12:	add    %al,(%rax)
    18000aa14:	cs (bad)
    18000aa17:	jae    0x18000aa19
    18000aa19:	add    %al,(%rax)
    18000aa1b:	add    %al,(%rax)
    18000aa1d:	lock add %al,(%rax)
-   18000aa20:	movabs 0x746164702e000008,%al
-   18000aa29:	(bad)
+   18000aa20:	rorb   (%rax)
+   18000aa22:	add    %al,(%rax)
+   18000aa24:	jo,pn  0x18000aa8b
+   18000aa27:	(bad)
+   18000aa28:	je     0x18000aa8b
 	...
    18000aa4e:	add    %al,(%rax)
    18000aa50:	adc    %eax,(%rsi)
    18000aa52:	add    (%rax),%al
    18000aa54:	(bad)
    18000aa55:	push   %rdx
    18000aa56:	add    (%rax),%dh
-   18000aa58:	mov    $0x7f,%al
+   18000aa58:	jo     0x18000a9dc
    18000aa5a:	add    %al,(%rax)
    18000aa5c:	(bad)
    18000aa5d:	stos   %al,%es:(%rdi)
    18000aa5e:	add    %al,(%rax)
    18000aa60:	sub    %ch,-0x56(%rcx)
    18000aa63:	add    %al,(%rax)
    18000aa65:	outsl  %ds:(%rsi),(%dx)
    18000aa66:	stos   %al,%es:(%rdi)
    18000aa67:	add    %al,(%rax)
    18000aa69:	add    (%rsi),%cl
-   18000aa6b:	movabs 0x27c001a06000080,%al
+   18000aa6b:	(bad)
+   18000aa6c:	addl   $0x0,(%rax)
+   18000aa6f:	(bad)
+   18000aa70:	sbb    (%rax),%al
+   18000aa72:	jl     0x18000aa76
    18000aa74:	push   %rax
    18000aa75:	add    %al,(%rax)
    18000aa77:	add    %al,(%rcx)
    18000aa79:	(bad)
    18000aa7a:	add    (%rax),%al
    18000aa7c:	(bad)
    18000aa7d:	xor    (%rdx),%al
@@ -13147,20 +13398,18 @@
    18000aa89:	clts
    18000aa8b:	add    %cl,(%rdi)
    18000aa8d:	fs (bad)
    18000aa8f:	add    %cl,(%rdi)
    18000aa91:	xor    $0x6,%al
    18000aa93:	add    %cl,(%rdi)
    18000aa95:	xor    (%rbx),%cl
-   18000aa97:	jo     0x18000aa49
-   18000aa99:	jg     0x18000aa9b
-   18000aa9b:	add    %ah,0x600000aa(%rax)
-   18000aaa1:	movsl  %ds:(%rsi),%es:(%rdi)
-   18000aaa2:	stos   %al,%es:(%rdi)
-   18000aaa3:	add    %al,(%rax)
+   18000aa97:	jo     0x18000ab09
+   18000aa99:	(bad)
+   18000aa9a:	add    %al,(%rax)
+   18000aa9c:	movabs 0xaaa5600000aa,%al
    18000aaa5:	add    0x0(%rax),%bl
    18000aaa8:	add    %ecx,(%rdx)
    18000aaaa:	add    $0x0,%al
    18000aaac:	or     (%rsi,%rax,1),%dh
    18000aaaf:	add    %cl,(%rdx)
    18000aab1:	xor    (%rsi),%al
    18000aab3:	jo     0x18000aab6
@@ -13208,17 +13457,18 @@
    18000ab0d:	stos   %al,%es:(%rdi)
    18000ab0e:	add    %al,(%rax)
    18000ab10:	adc    %ecx,(%rdx)
    18000ab12:	add    $0x0,%al
    18000ab14:	or     (%rax,%rdx,1),%dh
    18000ab17:	add    %cl,(%rdx)
    18000ab19:	rolb   %cl,(%rsi)
-   18000ab1b:	jo     0x18000aacd
-   18000ab1d:	jg     0x18000ab1f
-   18000ab1f:	add    %ah,(%rbx,%rbp,4)
+   18000ab1b:	jo     0x18000ab8d
+   18000ab1d:	(bad)
+   18000ab1e:	add    %al,(%rax)
+   18000ab20:	and    $0xab,%al
    18000ab22:	add    %al,(%rax)
    18000ab24:	sub    %ch,0x340000ab(%rip)        # 0x1b400abd5
    18000ab2a:	stos   %eax,%es:(%rdi)
    18000ab2b:	add    %al,(%rax)
    18000ab2d:	add    (%rdx),%cl
    18000ab2f:	jo     0x18000ab62
    18000ab31:	add    %al,(%rax)
@@ -13234,57 +13484,52 @@
    18000ab4c:	subb   $0x0,0x210000(%rdx)
    18000ab53:	add    %ah,%al
    18000ab55:	sub    $0x2def0000,%eax
    18000ab5a:	add    %al,(%rax)
    18000ab5c:	subb   $0x2,0x15190000(%rdx)
    18000ab63:	add    %al,(%rsi)
    18000ab65:	mov    $0x2,%dl
-   18000ab67:	xor    %dh,(%rcx,%rsi,2)
-   18000ab6a:	add    %al,(%rax)
-   18000ab6c:	push   %rax
-   18000ab6d:	add    %al,(%rax)
-   18000ab6f:	add    %dl,(%rcx)
-   18000ab71:	sbb    (%rdx),%ecx
-   18000ab73:	add    %bl,(%rbx)
-   18000ab75:	push   %rsp
-   18000ab76:	(bad)
-   18000ab77:	add    %bl,(%rbx)
-   18000ab79:	xor    $0xd,%al
-   18000ab7b:	add    %bl,(%rbx)
-   18000ab7d:	push   %rdx
-   18000ab7e:	(bad)
+   18000ab67:	xor    %dh,%ah
+   18000ab69:	jae    0x18000ab6b
+   18000ab6b:	add    %dl,0x0(%rax)
+   18000ab6e:	add    %al,(%rax)
+   18000ab70:	adc    %ebx,(%rbx)
+   18000ab72:	or     (%rax),%al
+   18000ab74:	sbb    0x0(%rsi,%rcx,1),%edx
+   18000ab78:	sbb    0x17521b00(,%rcx,1),%esi
    18000ab7f:	lock adc $0x11c013e0,%eax
    18000ab85:	jo     0x18000ab97
    18000ab87:	(bad)
-   18000ab88:	mov    $0x7f,%al
+   18000ab88:	jo     0x18000ab0c
    18000ab8a:	add    %al,(%rax)
    18000ab8c:	nop
    18000ab8d:	stos   %eax,%es:(%rdi)
    18000ab8e:	add    %al,(%rax)
    18000ab90:	sub    %bl,-0x60ffff55(%rcx)
    18000ab96:	stos   %eax,%es:(%rdi)
    18000ab97:	add    %al,(%rax)
    18000ab99:	add    (%rsi),%cl
-   18000ab9b:	jo     0x18000ab21
-   18000ab9d:	add    %al,(%rax)
-   18000ab9f:	add    %cl,%cl
+   18000ab9b:	nop
+   18000ab9c:	xchg   %eax,(%rax)
+   18000ab9e:	add    %al,(%rdx)
+   18000aba0:	leave
    18000aba1:	add    (%rdx),%al
    18000aba3:	add    %dl,(%rcx)
    18000aba5:	adc    $0x6,%al
    18000aba7:	add    %dl,(%rsp,%riz,2)
    18000abaa:	or     %eax,(%rax)
    18000abac:	adc    $0x34,%al
    18000abae:	or     %al,(%rax)
    18000abb0:	adc    $0x32,%al
-   18000abb2:	adc    %dh,-0x50(%rax)
-   18000abb5:	jg     0x18000abb7
-   18000abb7:	add    %bh,-0x3ad80000(%rbx,%rbp,4)
-   18000abbe:	stos   %eax,%es:(%rdi)
-   18000abbf:	add    %al,(%rax)
-   18000abc1:	int3
+   18000abb2:	adc    %dh,0x70(%rax)
+   18000abb5:	(bad)
+   18000abb6:	add    %al,(%rax)
+   18000abb8:	mov    $0x280000ab,%esp
+   18000abbd:	(bad)
+   18000abc0:	add    %cl,%ah
    18000abc2:	stos   %eax,%es:(%rdi)
    18000abc3:	add    %al,(%rax)
    18000abc5:	add    (%rax,%riz,1),%cl
    18000abc8:	sub    $0x0,%al
    18000abca:	add    %ah,0x6(%rax)
    18000abcd:	leave
    18000abce:	add    (%rdx),%al
@@ -13294,30 +13539,28 @@
    18000abd7:	add    %cl,(%rdi)
    18000abd9:	add    %ebx,(%rax)
    18000abdb:	add    %cl,(%rax)
    18000abdd:	jo     0x18000abe6
    18000abdf:	(bad)
    18000abe0:	(bad)
    18000abe1:	xor    %al,(%rax)
-   18000abe3:	add    %dh,-0x13ffff81(%rax)
+   18000abe3:	add    %dh,-0x7e(%rax)
+   18000abe6:	add    %al,(%rax)
+   18000abe8:	in     (%dx),%al
    18000abe9:	stos   %eax,%es:(%rdi)
    18000abea:	add    %al,(%rax)
    18000abec:	sub    %dh,%ch
    18000abee:	stos   %eax,%es:(%rdi)
    18000abef:	add    %al,(%rax)
-   18000abf1:	or     -0x2ff1f800(%rax,%rax,1),%ch
-   18000abf8:	(bad)
-   18000abf9:	add    %al,(%rax)
-   18000abfb:	loopne,pn 0x18000ab80
-   18000abfe:	add    %al,(%rax)
-   18000ac00:	cs lock (bad)
-   18000ac03:	add    %al,(%rax)
-   18000ac05:	cs add %al,0x3a080000(%rbx)
-   18000ac0c:	add    %ah,0x2(%rdx)
-   18000ac0f:	or     %r13b,%bpl
+   18000abf1:	or     -0x6ff1f800(%rax,%rax,1),%ch
+   18000abf8:	test   %eax,(%rax)
+   18000abfa:	add    %ch,(%rsi)
+   18000abfc:	movabs 0x85b02e000085,%al
+   18000ac05:	cs rolb $0x0,0x3a080000(%rbp)
+   18000ac0d:	(bad)
    18000ac12:	add    $0x0,%al
    18000ac14:	sbb    %esp,0x1d(%rsi)
    18000ac17:	add    %dl,-0x28(%rbp)
    18000ac1a:	add    %cl,-0x38(%r13)
    18000ac1e:	rex.X add %al,-0x48(%rbp)
    18000ac22:	rex.XB add %dil,0x380044a8(%rip)        # 0x1b800f0d1
    18000ac29:	cwtl
@@ -13333,30 +13576,30 @@
    18000ac41:	xor    $0x99,%al
    18000ac43:	add    %ah,(%rsi)
    18000ac45:	add    %edx,0x16f01800(%rdx)
    18000ac4b:	loopne 0x18000ac61
    18000ac4d:	rclb   (%rdx)
    18000ac4f:	rclb   $0x50,(%rax)
    18000ac52:	add    %al,(%rax)
-   18000ac54:	mov    $0x71,%al
+   18000ac54:	jo     0x18000acca
    18000ac56:	add    %al,(%rax)
    18000ac58:	(bad)
    18000ac59:	lods   %ds:(%rsi),%al
    18000ac5a:	add    %al,(%rax)
    18000ac5c:	add    (%rax,%rax,1),%al
    18000ac5f:	add    %ch,(%rax)
-   18000ac61:	imul   $0xd00e1000,0xac9d00(%rax,%rax,1),%ebp
-   18000ac6c:	test   %al,(%rax)
+   18000ac61:	imul   $0xf00e1000,0xac9d00(%rax,%rax,1),%ebp
+   18000ac6c:	xchg   %eax,(%rax)
    18000ac6e:	add    %ch,(%rsi)
-   18000ac70:	add    %al,-0x25d40000(%rbp)
-   18000ac76:	outsl  %ds:(%rsi),(%dx)
-   18000ac77:	add    %al,(%rax)
-   18000ac79:	add    %ecx,(%rcx)
-   18000ac7b:	xchg   %eax,%edx
-   18000ac7c:	movabs 0x323032c0000032,%al
+   18000ac70:	and    %cl,-0x65d40000(%rax)
+   18000ac76:	jb     0x18000ac78
+   18000ac78:	add    %al,(%rcx)
+   18000ac7a:	or     %edx,0x32a0(%rdx)
+   18000ac80:	shlb   $0x30,(%rdx)
+   18000ac83:	xor    (%rax),%al
    18000ac85:	add    %al,(%rcx)
    18000ac87:	or     %ebp,-0x60(%rdx)
    18000ac8a:	(bad)
    18000ac8b:	add    %al,(%rax)
    18000ac8d:	add    %ecx,0x2d703a(%rip)        # 0x1802e1ccd
    18000ac93:	add    %al,(%rcx)
    18000ac95:	or     %ebx,%edx
@@ -13367,20 +13610,20 @@
    18000aca0:	xor    %eax,(%rbx)
    18000aca2:	add    (%rax),%bh
    18000aca4:	add    $0x80,%al
    18000aca6:	(bad)
    18000aca7:	or     %bh,%fs:(%rcx)
    18000acaa:	add    (%rdx),%ecx
    18000acac:	pop    %rsp
-   18000acad:	or     %dh,0x13110c0e(%rip)        # 0x19311b8c1
+   18000acad:	or     %dh,0x133d0c0e(%rip)        # 0x1933db8c1
    18000acb3:	(bad)
    18000acb4:	adc    $0xc,%al
-   18000acb6:	adc    $0xa110802,%eax
+   18000acb6:	adc    $0xa210802,%eax
    18000acbb:	or     $0x36,%al
-   18000acbd:	or     %dh,0x8141007(%rbp)
+   18000acbd:	or     %bh,0x8141007(%rcx)
    18000acc3:	lea    (%rbx),%eax
    18000acc5:	add    %al,(%rax)
    18000acc7:	add    %al,(%rcx)
    18000acc9:	(bad)
    18000accb:	add    %cl,(%rdi)
    18000accd:	add    %ebp,(%rdi)
    18000accf:	add    %al,(%rbx)
@@ -13400,38 +13643,38 @@
    18000acf3:	add    %ch,(%rdx)
    18000acf5:	test   $0x10,%al
    18000acf7:	add    %ah,(%rcx)
    18000acf9:	(bad)
    18000acfa:	sub    $0x0,%al
    18000acfc:	adc    $0xc4,%al
    18000acfe:	sub    $0x2e740800,%eax
-   18000ad03:	add    %ah,%al
-   18000ad05:	rex.RXB add %r8b,(%r8)
-   18000ad08:	sub    $0xc8000048,%eax
-   18000ad0d:	lods   %ds:(%rsi),%al
-   18000ad0e:	add    %al,(%rax)
+   18000ad03:	add    %ah,0x48(%rax)
+   18000ad06:	add    %al,(%rax)
+   18000ad08:	lods   %ds:(%rsi),%eax
+   18000ad09:	rex.W add %al,(%rax)
+   18000ad0c:	enter  $0xac,$0x0
    18000ad10:	and    %eax,(%rax)
    18000ad12:	add    %al,(%rax)
-   18000ad14:	loopne 0x18000ad5d
-   18000ad16:	add    %al,(%rax)
-   18000ad18:	sub    $0xc8000048,%eax
-   18000ad1d:	lods   %ds:(%rsi),%al
-   18000ad1e:	add    %al,(%rax)
+   18000ad14:	(bad)
+   18000ad15:	rex.W add %al,(%rax)
+   18000ad18:	lods   %ds:(%rsi),%eax
+   18000ad19:	rex.W add %al,(%rax)
+   18000ad1c:	enter  $0xac,$0x0
    18000ad20:	sbb    %ebp,0x681b000b(%rip)        # 0x1e81bad31
    18000ad26:	sbb    (%rax),%al
    18000ad28:	adc    (%rcx),%eax
    18000ad2a:	ss add %cl,(%rax,%rsi,8)
    18000ad2e:	or     %al,%ah
    18000ad30:	or     %dl,%al
    18000ad32:	(bad)
    18000ad33:	rolb   $0x3,(%rax,%rsi,2)
    18000ad37:	(bad)
    18000ad38:	add    (%rax),%dh
    18000ad3a:	add    %al,(%rax)
-   18000ad3c:	mov    $0x71,%al
+   18000ad3c:	jo     0x18000adb2
    18000ad3e:	add    %al,(%rax)
    18000ad40:	lods   %ds:(%rsi),%rax
    18000ad42:	add    %al,(%rax)
    18000ad44:	xchg   %eax,%ebx
    18000ad45:	add    %eax,(%rax)
    18000ad47:	add    %bh,(%rax)
    18000ad49:	push   %rbp
@@ -13449,15 +13692,17 @@
    18000ad6c:	add    (%rsi),%al
    18000ad6e:	(bad)
    18000ad6f:	or     %dh,0x0(%rbp,%rbp,4)
    18000ad73:	add    %al,(%rdx)
    18000ad75:	adc    (%rdx),%edx
    18000ad77:	jo     0x18000ad5a
    18000ad79:	add    %al,(%rax)
-   18000ad7b:	rolb   0x13750000(%rbx)
+   18000ad7b:	nop
+   18000ad7c:	xchg   %al,(%rax)
+   18000ad7e:	add    %dh,0x13(%rbp)
    18000ad81:	adc    %cl,0x38022e00(%rax)
    18000ad87:	add    $0x36,%al
    18000ad89:	(bad)
    18000ad8a:	or     %r9,(%r8)
    18000ad8d:	adc    %ecx,(%rax,%rax,1)
    18000ad90:	pop    %rsi
    18000ad91:	or     %dh,(%rax,%rax,1)
@@ -13504,16 +13749,17 @@
    18000adf4:	je     0x18000ae27
    18000adf6:	add    %al,(%rax)
    18000adf8:	mov    $0x190000aa,%esp
    18000adfd:	(bad)
    18000adfe:	add    (%rax),%al
    18000ae00:	(bad)
    18000ae01:	xor    (%rdx),%al
-   18000ae03:	xor    %dh,0xc00007f(%rax)
-   18000ae09:	scas   %es:(%rdi),%al
+   18000ae03:	xor    %dh,-0x7e(%rax)
+   18000ae06:	add    %al,(%rax)
+   18000ae08:	or     $0xae,%al
    18000ae0a:	add    %al,(%rax)
    18000ae0c:	(bad)
    18000ae0d:	adc    %ebp,-0x55fe0000(%rsi)
    18000ae13:	add    %al,(%rcx)
    18000ae15:	clts
    18000ae17:	add    %cl,(%rdi)
    18000ae19:	fs (bad)
@@ -13521,53 +13767,55 @@
    18000ae1d:	xor    $0x6,%al
    18000ae1f:	add    %cl,(%rdi)
    18000ae21:	xor    (%rbx),%cl
    18000ae23:	jo     0x18000ae3e
    18000ae25:	sbb    $0x4,%al
    18000ae27:	add    %cl,0xd001534(%rip)        # 0x18d00c361
    18000ae2d:	repnz (bad)
-   18000ae2f:	jo     0x18000ae65
-   18000ae31:	jno    0x18000ae33
+   18000ae2f:	jo     0x18000ae25
+   18000ae31:	jae    0x18000ae33
    18000ae33:	add    %bh,0x0(%rax)
    18000ae36:	add    %al,(%rax)
    18000ae38:	and    %ecx,(%rax)
    18000ae3a:	add    (%rax),%al
    18000ae3c:	or     %ah,0x0(%rsp,%rdx,1)
-   18000ae40:	and    %cl,0x0(%rdi)
-   18000ae43:	add    %al,0x2400004f(%rax)
-   18000ae49:	scas   %es:(%rdi),%al
+   18000ae40:	(bad)
+   18000ae41:	push   %rdx
+   18000ae42:	add    %al,(%rax)
+   18000ae44:	rclb   $0x0,0x0(%rdx)
+   18000ae48:	and    $0xae,%al
    18000ae4a:	add    %al,(%rax)
    18000ae4c:	and    %eax,(%rax)
    18000ae4e:	add    %al,(%rax)
-   18000ae50:	and    %cl,0x0(%rdi)
-   18000ae53:	add    %al,0x2400004f(%rax)
-   18000ae59:	scas   %es:(%rdi),%al
+   18000ae50:	(bad)
+   18000ae51:	push   %rdx
+   18000ae52:	add    %al,(%rax)
+   18000ae54:	rclb   $0x0,0x0(%rdx)
+   18000ae58:	and    $0xae,%al
    18000ae5a:	add    %al,(%rax)
    18000ae5c:	and    %eax,0x74050002(%rip)        # 0x1f405ae64
    18000ae62:	(bad)
-   18000ae63:	add    %dl,0x6c(%rax)
+   18000ae63:	add    %dl,(%rax)
+   18000ae65:	outsl  %ds:(%rsi),(%dx)
    18000ae66:	add    %al,(%rax)
-   18000ae68:	subl   $0xffffff80,0x0(%rax,%rax,1)
-   18000ae6d:	stos   %al,%es:(%rdi)
-   18000ae6e:	add    %al,(%rax)
-   18000ae70:	and    %eax,(%rax)
-   18000ae72:	add    (%rax),%al
-   18000ae74:	add    %dh,0x0(%rsi,%rax,1)
-   18000ae78:	push   %rax
-   18000ae79:	insb   (%dx),%es:(%rdi)
+   18000ae68:	rex.XB outsl %ds:(%rsi),(%dx)
+   18000ae6a:	add    %al,(%rax)
+   18000ae6c:	subb   $0x2,0x210000(%rdx)
+   18000ae73:	add    %al,(%rax)
+   18000ae75:	je     0x18000ae7d
+   18000ae77:	add    %dl,(%rax)
+   18000ae79:	outsl  %ds:(%rsi),(%dx)
    18000ae7a:	add    %al,(%rax)
-   18000ae7c:	subl   $0xffffff80,0x0(%rax,%rax,1)
-   18000ae81:	stos   %al,%es:(%rdi)
-   18000ae82:	add    %al,(%rax)
-   18000ae84:	sbb    %esp,(%rbx)
-   18000ae86:	(bad)
+   18000ae7c:	rex.XB outsl %ds:(%rsi),(%dx)
+   18000ae7e:	add    %al,(%rax)
+   18000ae80:	subb   $0x6,0x23190000(%rdx)
    18000ae87:	add    %dl,0x15001474(%rip)        # 0x19500c301
    18000ae8d:	xor    $0x13,%al
-   18000ae8f:	add    %dl,-0x4faff40e(%rip)        # 0x13050ba87
-   18000ae95:	jno    0x18000ae97
+   18000ae8f:	add    %dl,0x70500bf2(%rip)        # 0x1f050ba87
+   18000ae95:	je     0x18000ae97
    18000ae97:	add    %ah,0x7a0000ae(%rax)
    18000ae9d:	add    %al,(%rax)
    18000ae9f:	add    %ch,(%rax)
    18000aea1:	test   $0xb00000ae,%eax
    18000aea6:	scas   %es:(%rdi),%al
    18000aea7:	add    %al,(%rax)
    18000aea9:	add    (%rdx),%cl
@@ -13583,29 +13831,25 @@
    18000aebd:	or     %eax,%fs:(%rax)
    18000aec0:	adc    %dl,0x0(%rax,%rcx,1)
    18000aec4:	adc    %dh,(%rdx)
    18000aec6:	or     $0xe0,%al
    18000aec8:	and    %ecx,(%rdx)
    18000aeca:	add    $0x0,%al
    18000aecc:	or     0x0(%rdi,%rax,1),%dh
-   18000aed0:	add    $0xf0000634,%eax
-   18000aed5:	insb   (%dx),%es:(%rdi)
+   18000aed0:	add    $0xb0000634,%eax
+   18000aed5:	outsl  %ds:(%rsi),(%dx)
    18000aed6:	add    %al,(%rax)
-   18000aed8:	rex.XB insl (%dx),%es:(%rdi)
-   18000aeda:	add    %al,(%rax)
-   18000aedc:	mov    $0x210000ae,%eax
+   18000aed8:	add    0x0(%rax),%esi
+   18000aedb:	add    %bh,0x210000ae(%rax)
    18000aee1:	add    %al,(%rax,%rax,1)
    18000aee4:	add    %dh,0x0(%rdi,%rax,1)
    18000aee8:	add    %dh,(%rsi,%rax,1)
-   18000aeeb:	add    %dh,%al
-   18000aeed:	insb   (%dx),%es:(%rdi)
-   18000aeee:	add    %al,(%rax)
-   18000aef0:	rex.XB insl (%dx),%es:(%rdi)
-   18000aef2:	add    %al,(%rax)
-   18000aef4:	mov    $0x10000ae,%eax
+   18000aeeb:	add    %dh,0x300006f(%rax)
+   18000aef1:	jo     0x18000aef3
+   18000aef3:	add    %bh,0x10000ae(%rax)
    18000aef9:	or     (%r8),%r8b
    18000aefc:	rex.RB
    18000aefd:	fs (bad)
    18000aeff:	add    %al,0x54(%rax)
    18000af02:	(bad)
    18000af03:	add    %dl,(%rax)
    18000af05:	je     0x18000af10
@@ -13634,38 +13878,39 @@
    18000af36:	add    (%rax),%eax
    18000af38:	(bad)
    18000af39:	rex.X add 0x2(%rax),%esp
    18000af3d:	xor    %al,(%rax)
    18000af3f:	add    %ah,(%rcx)
    18000af41:	add    $0x74050002,%eax
    18000af46:	add    $0x0,%al
-   18000af48:	mov    $0x55,%al
+   18000af48:	(bad)
+   18000af49:	pop    %rax
    18000af4a:	add    %al,(%rax)
-   18000af4c:	out    %al,(%dx)
-   18000af4d:	push   %rbp
+   18000af4c:	sahf
+   18000af4d:	pop    %rax
    18000af4e:	add    %al,(%rax)
    18000af50:	xor    $0xaf,%al
    18000af52:	add    %al,(%rax)
    18000af54:	and    %eax,(%rax)
    18000af56:	add    %al,(%rax)
-   18000af58:	mov    $0x55,%al
+   18000af58:	(bad)
+   18000af59:	pop    %rax
    18000af5a:	add    %al,(%rax)
-   18000af5c:	out    %al,(%dx)
-   18000af5d:	push   %rbp
+   18000af5c:	sahf
+   18000af5d:	pop    %rax
    18000af5e:	add    %al,(%rax)
    18000af60:	xor    $0xaf,%al
    18000af62:	add    %al,(%rax)
    18000af64:	sbb    %edx,-0x4df9fffe(%rip)        # 0x13206af6c
    18000af6a:	add    (%rax),%dh
-   18000af6c:	xor    $0x71,%al
-   18000af6e:	add    %al,(%rax)
-   18000af70:	pop    %rax
-   18000af71:	add    %al,(%rax)
-   18000af73:	add    %ah,(%rcx)
-   18000af75:	add    $0x74050002,%eax
+   18000af6c:	hlt
+   18000af6d:	jae    0x18000af6f
+   18000af6f:	add    %bl,0x0(%rax)
+   18000af72:	add    %al,(%rax)
+   18000af74:	and    %eax,0x74050002(%rip)        # 0x1f405af7c
    18000af7a:	(bad)
    18000af7c:	lock ss add %al,(%rax)
    18000af80:	and    $0x64000037,%eax
    18000af85:	scas   %es:(%rdi),%eax
    18000af86:	add    %al,(%rax)
    18000af88:	and    %eax,(%rax)
    18000af8a:	add    (%rax),%al
@@ -13687,40 +13932,41 @@
    18000afb3:	add    %dl,(%rsi)
    18000afb5:	push   %rdx
    18000afb6:	adc    %al,%dh
    18000afb8:	adc    %ah,%al
    18000afba:	(bad)
    18000afbb:	rorb   $0xb,(%rax,%rsi,2)
    18000afbf:	(bad)
-   18000afc0:	mov    $0x7f,%al
+   18000afc0:	jo     0x18000af44
    18000afc2:	add    %al,(%rax)
    18000afc4:	enter  $0xaf,$0x0
    18000afc8:	cmp    %dl,%ch
    18000afca:	scas   %es:(%rdi),%eax
    18000afcb:	add    %al,(%rax)
    18000afcd:	out    %al,(%dx)
    18000afce:	scas   %es:(%rdi),%eax
    18000afcf:	add    %al,(%rax)
    18000afd1:	ljmp   *0xa0c0000(%rdi)
    18000afd7:	add    %dh,(%rdx)
    18000afd9:	add    %al,(%rax)
    18000afdb:	cmp    0x32(%rax),%spl
    18000afdf:	add    %al,(%rax)
    18000afe1:	xor    %dil,(%rax)
-   18000afe4:	jle    0x18000afa2
-   18000afe6:	jg     0x18000afe8
-   18000afe8:	add    %ch,(%rsi)
-   18000afea:	mov    $0x200007f,%esp
-   18000afef:	add    $0x4,%al
+   18000afe4:	jle    0x18000b062
+   18000afe6:	(bad)
+   18000afe7:	add    %al,(%rax)
+   18000afe9:	jl,pn  0x18000af6e
+   18000afec:	add    %al,(%rax)
+   18000afee:	add    (%rsp,%rax,1),%al
    18000aff1:	(bad)
    18000aff2:	imulb  0x11020000(%rdi)
-   18000aff8:	and    $0x80,%al
-   18000affb:	add    %al,(%rax)
-   18000affd:	xchg   %eax,%ecx
-   18000affe:	add    $0x5400e20e,%eax
+   18000aff8:	andb   $0x5,-0x6effff7d(%rax)
+   18000afff:	(bad)
+   18000b000:	loop   0x18000b002
+   18000b002:	push   %rsp
    18000b003:	add    0x4c04d806(%rsi),%dh
    18000b009:	or     (%rsi),%ah
    18000b00b:	or     $0x32,%al
    18000b00d:	add    %al,(%rax)
    18000b00f:	add    %al,(%rcx)
    18000b011:	sbb    (%rdx),%cl
    18000b013:	add    %bl,(%rdx)
@@ -13741,4424 +13987,4487 @@
    18000b038:	sbb    (%rsp,%rcx,1),%esi
    18000b03b:	add    %bl,(%rbx)
    18000b03d:	push   %rdx
    18000b03e:	(bad)
    18000b03f:	lock adc $0x11c013e0,%eax
    18000b045:	jo     0x18000b057
    18000b047:	(bad)
-   18000b048:	mov    $0x7f,%al
+   18000b048:	jo     0x18000afcc
    18000b04a:	add    %al,(%rax)
    18000b04c:	push   %rax
    18000b04d:	mov    $0x0,%al
    18000b04f:	add    %ch,(%rax)
    18000b051:	pop    %rcx
    18000b052:	mov    $0x0,%al
    18000b054:	add    %dh,-0x50(%rsi)
    18000b057:	add    %al,(%rax)
    18000b059:	or     (%rsi),%cl
-   18000b05b:	rex addl $0x0,(%rax)
-   18000b05f:	sub    $0x70,%al
+   18000b05b:	add    %al,0x702c0000(%rsi)
    18000b061:	sub    $0x0,%al
    18000b063:	add    %dl,%al
-   18000b065:	ss addb $0x2c,-0x7f760000(%rbx)
-   18000b06d:	add    %al,(%rax)
+   18000b065:	ss rex xchg %al,(%rax)
+   18000b069:	add    %cl,0x2c80(%rdx)
    18000b06f:	sarb   0x2de0(%rdx)
    18000b075:	rex or %cl,-0x34(%rax,%rax,1)
    18000b07a:	(bad)
    18000b07b:	sub    (%rax),%cl
    18000b07d:	xchg   %eax,%ebp
    18000b07e:	add    (%rdx),%cl
-   18000b080:	add    %edx,(%rax)
-   18000b082:	(bad)
-   18000b083:	add    %dl,(%rax)
-   18000b085:	lldt   %fs:(%rax)
-   18000b089:	xor    $0xe,%al
-   18000b08b:	add    %dl,(%rax)
-   18000b08d:	xchg   %eax,%edx
-   18000b08e:	or     $0xe0,%al
-   18000b090:	and    %ecx,(%rsi)
-   18000b092:	add    $0x0,%al
-   18000b094:	(bad)
-   18000b095:	je     0x18000b0a4
-   18000b097:	add    %al,-0x1ffff3ac(%rip)        # 0x16000bcf1
-   18000b09d:	add    %r8b,(%r8)
-   18000b0a0:	jno    0x18000b0e8
-   18000b0a2:	add    %al,(%rax)
-   18000b0a4:	xorb   $0x0,0x210000(%rax)
-   18000b0ab:	add    %ah,%al
-   18000b0ad:	add    %r8b,(%r8)
-   18000b0b0:	jno    0x18000b0f8
-   18000b0b2:	add    %al,(%rax)
-   18000b0b4:	xorb   $0xa,0x19110000(%rax)
-   18000b0bb:	add    %bl,(%rcx)
-   18000b0bd:	xor    $0x15,%al
-   18000b0bf:	add    %bl,(%rcx)
-   18000b0c1:	mov    $0x15,%dl
-   18000b0c3:	lock adc %eax,%esp
-   18000b0c6:	adc    %edx,%eax
-   18000b0c8:	xadd   %cl,0xb600c70(%rip)        # 0x18b60bd3f
-   18000b0cf:	push   %rax
-   18000b0d0:	mov    $0x7f,%al
-   18000b0d2:	add    %al,(%rax)
-   18000b0d4:	fdivs  -0x1ed80000(%rax)
-   18000b0da:	mov    $0x0,%al
-   18000b0dc:	add    %al,(%rax)
-   18000b0de:	mov    $0x0,%cl
-   18000b0e0:	add    %cl,(%rdx)
-   18000b0e2:	(bad)
-   18000b0e3:	adc    %al,0x2c702c00(%rax,%rax,1)
-   18000b0ea:	add    %al,(%rax)
-   18000b0ec:	roll   $0x3e,(%rdx)
-   18000b0ef:	push   %rax
-   18000b0f0:	test   %al,(%rax)
-   18000b0f2:	add    %dl,0x2c80(%rdx)
-   18000b0f8:	roll   $0xca,(%rdx)
-   18000b0fb:	loopne 0x18000b12a
-   18000b0fd:	add    %al,(%rax)
-   18000b0ff:	nop
-   18000b100:	or     $0x54,%al
-   18000b102:	add    %dl,%al
-   18000b104:	(bad)
-   18000b105:	xor    (%rax),%cl
-   18000b107:	(bad)
-   18000b108:	or     0x2(%rbp),%ah
-   18000b10b:	add    %cl,0xa(%rsi)
-   18000b10e:	add    %al,(%rax)
-   18000b110:	add    %ecx,(%rdx)
-   18000b112:	add    $0x0,%al
-   18000b114:	or     (%rdi,%rax,1),%dh
-   18000b117:	add    %cl,(%rdx)
-   18000b119:	xor    (%rsi),%al
-   18000b11b:	jo     0x18000b136
-   18000b11d:	adc    %eax,(%rax,%rax,1)
-   18000b120:	adc    %esi,(%rdx)
-   18000b122:	or     $0xb600c70,%eax
-   18000b127:	xor    %dh,0x3000007f(%rax)
-   18000b12d:	mov    $0x0,%cl
-   18000b12f:	add    %bh,(%rax)
-   18000b131:	cmp    $0x400000b1,%eax
-   18000b136:	mov    $0x0,%cl
-   18000b138:	add    %cl,-0x4f(%rdi)
-   18000b13b:	add    %al,(%rax)
-   18000b13d:	add    $0x8,%al
-   18000b13f:	adc    %al,(%rdx)
-   18000b141:	add    %al,(%rax)
-   18000b143:	add    -0x4f(%rax),%cl
+   18000b080:	add    %ecx,(%rcx)
+   18000b082:	add    $0x0,%al
+   18000b084:	or     %edx,0x6003e005(%rdx)
+   18000b08a:	add    (%rax),%dh
+   18000b08c:	and    %eax,0x74050002(%rip)        # 0x1f405b094
+   18000b092:	verr   %ax
+   18000b095:	add    %r8b,(%r8)
+   18000b098:	rex.W
+   18000b099:	rex.RX add %r8b,(%rax)
+   18000b09c:	xorb   $0x2,0x5210000(%rax)
+   18000b0a3:	add    %al,0x48000e54(%rip)        # 0x1c800befd
+   18000b0a9:	rex.RX add %r8b,(%rax)
+   18000b0ac:	or     %eax,0x0(%rdi)
+   18000b0af:	add    %cl,0x210000(%rax,%rsi,4)
+   18000b0b6:	add    %al,(%rax)
+   18000b0b8:	rex.W
+   18000b0b9:	rex.RX add %r8b,(%rax)
+   18000b0bc:	or     %eax,0x0(%rdi)
+   18000b0bf:	add    %cl,0x210000(%rax,%rsi,4)
+   18000b0c6:	add    %al,(%rax)
+   18000b0c8:	loopne 0x18000b10f
+   18000b0ca:	add    %al,(%rax)
+   18000b0cc:	rex.W
+   18000b0cd:	rex.RX add %r8b,(%rax)
+   18000b0d0:	xorb   $0xa,0x19110000(%rax)
+   18000b0d7:	add    %bl,(%rcx)
+   18000b0d9:	xor    $0x15,%al
+   18000b0db:	add    %bl,(%rcx)
+   18000b0dd:	mov    $0x15,%dl
+   18000b0df:	lock adc %eax,%esp
+   18000b0e2:	adc    %edx,%eax
+   18000b0e4:	xadd   %cl,0xb600c70(%rip)        # 0x18b60bd5b
+   18000b0eb:	push   %rax
+   18000b0ec:	jo     0x18000b070
+   18000b0ee:	add    %al,(%rax)
+   18000b0f0:	hlt
+   18000b0f1:	mov    $0x0,%al
+   18000b0f3:	add    %ch,(%rax)
+   18000b0f5:	std
+   18000b0f6:	mov    $0x0,%al
+   18000b0f8:	add    %bl,(%rcx,%rsi,4)
+   18000b0fb:	add    %al,(%rax)
+   18000b0fd:	or     (%rsi),%cl
+   18000b0ff:	xor    %al,0x702c0000(%rdi)
+   18000b105:	sub    $0x0,%al
+   18000b107:	add    %al,%cl
+   18000b109:	add    (%rsi),%bh
+   18000b10b:	jo     0x18000b094
+   18000b10d:	add    %al,(%rax)
+   18000b10f:	xchg   %eax,%edx
+   18000b110:	subb   $0x0,(%rax,%rax,1)
+   18000b114:	roll   $0xca,(%rdx)
+   18000b117:	loopne 0x18000b146
+   18000b119:	add    %al,(%rax)
+   18000b11b:	nop
+   18000b11c:	or     $0x54,%al
+   18000b11e:	add    %bl,%al
+   18000b120:	(bad)
+   18000b121:	xor    %cl,(%rax)
+   18000b123:	movabs 0xa4e0002590a,%al
+   18000b12c:	adc    %ebx,(%rdx)
+   18000b12e:	or     %eax,(%rax)
+   18000b130:	sbb    %dl,%al
+   18000b132:	(bad)
+   18000b133:	lock adc $0xe0,%al
+   18000b136:	adc    %al,%dl
+   18000b138:	adc    %al,%al
+   18000b13a:	(bad)
+   18000b13b:	jo     0x18000b14a
+   18000b13d:	(bad)
+   18000b13e:	or     $0x50,%al
+   18000b140:	or     (%rax),%esi
+   18000b142:	add    %al,(%rax)
+   18000b144:	jo     0x18000b0c8
    18000b146:	add    %al,(%rax)
-   18000b148:	add    (%rcx),%al
-   18000b14a:	adcb   $0x83,(%rax)
-   18000b14d:	add    %al,(%rax)
-   18000b14f:	add    0x0(%rsi),%bh
-   18000b152:	add    %al,(%rax)
-   18000b154:	add    %edx,0x74150008(%rip)        # 0x1f415b162
-   18000b15a:	or     %al,(%rax)
-   18000b15c:	adc    $0x15000764,%eax
-   18000b161:	xor    $0x6,%al
-   18000b163:	add    %dl,0x11e01132(%rip)        # 0x191e0c29b
-   18000b169:	sbb    $0xc,%al
-   18000b16b:	add    %bl,(%rsp,%riz,2)
-   18000b16e:	adc    $0x0,%al
-   18000b170:	sbb    $0x54,%al
-   18000b172:	adc    (%rax),%eax
-   18000b174:	sbb    $0x34,%al
-   18000b176:	adc    (%rax),%al
-   18000b178:	sbb    $0xb2,%al
-   18000b17a:	sbb    %dh,%al
-   18000b17c:	(bad)
-   18000b17d:	loopne 0x18000b193
-   18000b17f:	rclb   (%rdx)
-   18000b181:	rclb   $0x70,(%rax)
-   18000b184:	mov    $0x7f,%al
-   18000b186:	add    %al,(%rax)
-   18000b188:	mov    %?,-0x6ad80000(%rcx)
-   18000b18e:	mov    $0x0,%cl
-   18000b190:	add    %bl,0xa020000(%rcx,%rsi,4)
-   18000b197:	movabs 0xfd00a4048000002c,%al
-   18000b1a0:	(bad)
-   18000b1a1:	add    (%rax),%al
-   18000b1a3:	add    %dl,(%rcx)
-   18000b1a5:	or     %al,(%rax,%rax,1)
-   18000b1a8:	or     %dh,(%rdx)
-   18000b1aa:	add    $0x70,%al
-   18000b1ac:	add    0x2(%rax),%esp
-   18000b1af:	xor    %dh,-0x47ffff81(%rax)
-   18000b1b5:	mov    $0x0,%cl
-   18000b1b7:	add    %ch,(%rax)
-   18000b1b9:	shll   $0x0,-0x4e320000(%rcx)
-   18000b1c0:	add    %al,(%rdx,%rcx,1)
-   18000b1c3:	mov    %ch,0x0(%rdi)
-   18000b1c6:	add    %al,0x2c8032(%rax)
-   18000b1cc:	add    %ah,-0x2bfda7f8(%rax)
-   18000b1d2:	add    $0x3a,%al
-   18000b1d4:	add    %ch,(%rdx,%rax,1)
-   18000b1d7:	add    %bl,(%rcx)
-   18000b1d9:	adc    $0x8,%al
-   18000b1db:	add    %dl,(%rdx,%rsi,1)
-   18000b1de:	adc    %dh,%al
-   18000b1e0:	(bad)
-   18000b1e1:	loopne 0x18000b1ef
-   18000b1e3:	rorb   (%rdx)
-   18000b1e5:	rorb   $0x70,(%rax)
-   18000b1e8:	(bad)
-   18000b1e9:	(bad)
-   18000b1ea:	(bad)
-   18000b1eb:	xor    %dh,-0xbffff81(%rax)
-   18000b1f1:	mov    $0x0,%cl
-   18000b1f3:	add    %bh,(%rax)
-   18000b1f5:	cmp    $0x10000b1,%eax
-   18000b1fa:	mov    $0x0,%dl
-   18000b1fc:	add    %dl,(%rax)
-   18000b1fe:	mov    $0x0,%dl
-   18000b200:	add    %al,(%rdx)
-   18000b202:	add    %al,(%rax)
-   18000b204:	add    (%rcx),%cl
+   18000b148:	rex.WR mov $0x0,%cl
+   18000b14b:	add    %ch,(%rax)
+   18000b14d:	push   %rbp
+   18000b14e:	mov    $0x0,%cl
+   18000b150:	add    %dh,-0x4f(%rdx)
+   18000b153:	add    %al,(%rax)
+   18000b155:	or     (%rsi),%cl
+   18000b157:	rolb   0x702c0000(%rsi)
+   18000b15d:	sub    $0x0,%al
+   18000b15f:	add    %ah,0x36(%rax)
+   18000b162:	adc    %al,-0x7f760000(%rdi)
+   18000b168:	sub    $0x0,%al
+   18000b16a:	add    %ah,-0x46(%rax)
+   18000b16d:	loopne 0x18000b19c
+   18000b16f:	add    %al,(%rax)
+   18000b171:	jo     0x18000b17f
+   18000b173:	push   %rsi
+   18000b174:	add    %ah,%ah
+   18000b176:	(bad)
+   18000b177:	cmp    (%rax),%cl
+   18000b179:	mov    $0xa,%al
+   18000b17b:	imul   $0xb00050b,0x10a4000(%rip),%eax        # 0x1810af185
+   18000b185:	add    %fs:(%rax),%eax
+   18000b188:	or     (%rdx,%rax,1),%esi
+   18000b18b:	add    %cl,(%rbx)
+   18000b18d:	jo     0x18000b18f
+   18000b18f:	add    %bl,(%rcx)
+   18000b191:	adc    %eax,(%rax,%rax,1)
+   18000b194:	adc    %esi,(%rdx)
+   18000b196:	or     $0xb600c70,%eax
+   18000b19b:	xor    %dh,-0x7e(%rax)
+   18000b19e:	add    %al,(%rax)
+   18000b1a0:	movsb  %ds:(%rsi),%es:(%rdi)
+   18000b1a1:	mov    $0x0,%cl
+   18000b1a3:	add    %bh,(%rax)
+   18000b1a5:	mov    $0xb1,%cl
+   18000b1a7:	add    %al,(%rax)
+   18000b1a9:	mov    $0xb1,%ah
+   18000b1ab:	add    %al,(%rax)
+   18000b1ad:	ret
+   18000b1ae:	mov    $0x0,%cl
+   18000b1b0:	add    %al,(%rax,%rcx,1)
+   18000b1b3:	adc    %al,(%rdx)
+   18000b1b5:	add    %al,(%rax)
+   18000b1b7:	add    0x1020000(%rcx,%rsi,4),%bh
+   18000b1be:	adc    $0x85,%al
+   18000b1c1:	add    %al,(%rax)
+   18000b1c3:	add    0x0(%rsi),%bh
+   18000b1c6:	add    %al,(%rax)
+   18000b1c8:	add    %edx,0x74150008(%rip)        # 0x1f415b1d6
+   18000b1ce:	or     %al,(%rax)
+   18000b1d0:	adc    $0x15000764,%eax
+   18000b1d5:	xor    $0x6,%al
+   18000b1d7:	add    %dl,0x11e01132(%rip)        # 0x191e0c30f
+   18000b1dd:	sbb    $0xc,%al
+   18000b1df:	add    %bl,(%rsp,%riz,2)
+   18000b1e2:	adc    $0x0,%al
+   18000b1e4:	sbb    $0x54,%al
+   18000b1e6:	adc    (%rax),%eax
+   18000b1e8:	sbb    $0x34,%al
+   18000b1ea:	adc    (%rax),%al
+   18000b1ec:	sbb    $0xb2,%al
+   18000b1ee:	sbb    %dh,%al
+   18000b1f0:	(bad)
+   18000b1f1:	loopne 0x18000b207
+   18000b1f3:	rclb   (%rdx)
+   18000b1f5:	rclb   $0x70,(%rax)
+   18000b1f8:	jo     0x18000b17c
+   18000b1fa:	add    %al,(%rax)
+   18000b1fc:	add    %dh,0x9280000(%rdx)
+   18000b202:	mov    $0x0,%dl
+   18000b204:	add    %dl,(%rax)
    18000b206:	mov    $0x0,%dl
    18000b208:	add    %al,(%rdx)
-   18000b20a:	add    %eax,0x8140(%rax)
-   18000b210:	add    %ah,%bh
-   18000b212:	add    %al,(%rax)
-   18000b214:	sbb    %eax,(%rcx,%rax,1)
-   18000b217:	add    %al,(%rdx,%rax,2)
-   18000b21a:	add    %al,(%rax)
-   18000b21c:	mov    $0x7f,%al
-   18000b21e:	add    %al,(%rax)
-   18000b220:	and    $0xb2,%al
-   18000b222:	add    %al,(%rax)
-   18000b224:	(bad)
-   18000b225:	sub    %esi,0x36020000(%rdx)
-   18000b22b:	add    %bl,(%rcx)
-   18000b22d:	(bad)
-   18000b22e:	add    (%rax),%al
-   18000b230:	(bad)
-   18000b231:	xor    (%rdx),%al
-   18000b233:	xor    %dh,0x3c00007f(%rax)
-   18000b239:	mov    $0x0,%dl
-   18000b23b:	add    %ch,0x45(%rax)
-   18000b23e:	mov    $0x0,%dl
-   18000b240:	add    %cl,-0x4e(%rbx)
-   18000b243:	add    %al,(%rax)
-   18000b245:	add    (%rsi),%cl
-   18000b247:	mov    $0x400007f,%esp
-   18000b24c:	sub    (%rax),%al
-   18000b24e:	cmp    $0x2,%al
-   18000b250:	add    %ecx,(%rsi)
-   18000b252:	(bad)
-   18000b253:	add    %cl,(%rsi)
-   18000b255:	xor    $0xb,%al
-   18000b257:	add    %cl,(%rsi)
-   18000b259:	xor    (%rdx),%cl
-   18000b25b:	lock or %ah,%al
+   18000b20a:	or     -0x7fffffd4(%rax),%ah
+   18000b210:	add    $0xa4,%al
+   18000b212:	add    %bh,%ch
+   18000b214:	(bad)
+   18000b215:	add    (%rax),%al
+   18000b217:	add    %dl,(%rcx)
+   18000b219:	or     %al,(%rax,%rax,1)
+   18000b21c:	or     %dh,(%rdx)
+   18000b21e:	add    $0x70,%al
+   18000b220:	add    0x2(%rax),%esp
+   18000b223:	xor    %dh,-0x7e(%rax)
+   18000b226:	add    %al,(%rax)
+   18000b228:	sub    $0xb2,%al
+   18000b22a:	add    %al,(%rax)
+   18000b22c:	sub    %dh,0x420000b2(%rip)        # 0x1c200b2e4
+   18000b232:	mov    $0x0,%dl
+   18000b234:	add    %al,(%rdx,%rcx,1)
+   18000b237:	rex.W jb 0x18000b23a
+   18000b23a:	add    %al,0x2c8032(%rax)
+   18000b240:	add    %ah,-0x2bfda7f8(%rax)
+   18000b246:	add    $0x3a,%al
+   18000b248:	add    %ch,(%rdx,%rax,1)
+   18000b24b:	add    %bl,(%rcx)
+   18000b24d:	adc    $0x8,%al
+   18000b24f:	add    %dl,(%rdx,%rsi,1)
+   18000b252:	adc    %dh,%al
+   18000b254:	(bad)
+   18000b255:	loopne 0x18000b263
+   18000b257:	rorb   (%rdx)
+   18000b259:	rorb   $0x70,(%rax)
+   18000b25c:	(bad)
+   18000b25d:	(bad)
    18000b25e:	(bad)
-   18000b25f:	(bad)
-   18000b260:	and    %edx,(%rbx)
-   18000b262:	(bad)
-   18000b263:	add    %dl,(%rbx)
-   18000b265:	(bad)
-   18000b266:	or     (%rax),%al
-   18000b268:	(bad)
-   18000b269:	je     0x18000b274
-   18000b26b:	add    %al,-0x2ffff7ac(%rip)        # 0x15000bac5
-   18000b271:	sbb    (%rax),%al
-   18000b273:	add    %al,(%rdx)
-   18000b275:	sbb    (%rax),%eax
-   18000b277:	add    %dl,-0x4e(%rax)
-   18000b27a:	add    %al,(%rax)
-   18000b27c:	and    %eax,(%rax)
-   18000b27e:	add    %al,(%rax)
-   18000b280:	rcrb   (%rdx)
+   18000b25f:	xor    %dh,-0x7e(%rax)
+   18000b262:	add    %al,(%rax)
+   18000b264:	push   $0x380000b2
+   18000b269:	mov    $0xb1,%cl
+   18000b26b:	add    %al,(%rax)
+   18000b26d:	jne    0x18000b221
+   18000b26f:	add    %al,(%rax)
+   18000b271:	test   %dh,0x20000(%rdx)
+   18000b277:	add    %al,(%rdx)
+   18000b279:	jge    0x18000b22d
+   18000b27b:	add    %al,(%rax)
+   18000b27d:	add    (%rcx),%al
+   18000b27f:	addb   $0x84,(%rax)
    18000b282:	add    %al,(%rax)
-   18000b284:	add    (%rbx),%bl
+   18000b284:	add    %ah,%bh
    18000b286:	add    %al,(%rax)
-   18000b288:	push   %rax
-   18000b289:	mov    $0x0,%dl
-   18000b28b:	add    %ah,(%rcx)
-   18000b28d:	add    %al,(%rsi)
-   18000b28f:	add    %al,(%rax)
-   18000b291:	(bad)
-   18000b292:	or     (%rax),%al
-   18000b294:	add    %dh,0x0(%rcx,%rcx,1)
-   18000b298:	add    %dl,0x0(%rax,%rcx,1)
-   18000b29c:	rcrb   (%rdx)
-   18000b29e:	add    %al,(%rax)
-   18000b2a0:	add    (%rbx),%bl
-   18000b2a2:	add    %al,(%rax)
-   18000b2a4:	push   %rax
-   18000b2a5:	mov    $0x0,%dl
-   18000b2a7:	add    %dl,(%rcx)
-   18000b2a9:	sbb    $0xb,%al
-   18000b2ab:	add    %bl,(%rsp,%rsi,1)
-   18000b2ae:	sbb    (%rax),%al
-   18000b2b0:	sbb    $0x1,%al
-   18000b2b2:	adc    (%rax),%al
-   18000b2b4:	adc    $0x11e013f0,%eax
-   18000b2b9:	rorb   (%rdi)
-   18000b2bb:	rorb   $0x50,0xb600c70(%rip)        # 0x18b60bf32
-   18000b2c2:	add    %al,(%rax)
-   18000b2c4:	mov    $0x7f,%al
-   18000b2c6:	add    %al,(%rax)
-   18000b2c8:	int3
-   18000b2c9:	mov    $0x0,%dl
-   18000b2cb:	add    %ch,(%rax)
-   18000b2cd:	(bad)
-   18000b2ce:	mov    $0x0,%dl
-   18000b2d0:	add    %bh,%dh
-   18000b2d2:	mov    $0x0,%dl
-   18000b2d4:	add    %cl,(%rsi)
+   18000b288:	sbb    %eax,(%rcx,%rax,1)
+   18000b28b:	add    %al,(%rdx,%rax,2)
+   18000b28e:	add    %al,(%rax)
+   18000b290:	jo     0x18000b214
+   18000b292:	add    %al,(%rax)
+   18000b294:	cwtl
+   18000b295:	mov    $0x0,%dl
+   18000b297:	add    %ah,-0x63(%rax)
+   18000b29a:	mov    $0x0,%dl
+   18000b29c:	add    %al,(%rdx)
+   18000b29e:	ss add %bl,(%rcx)
+   18000b2a1:	(bad)
+   18000b2a2:	add    (%rax),%al
+   18000b2a4:	(bad)
+   18000b2a5:	xor    (%rdx),%al
+   18000b2a7:	xor    %dh,-0x7e(%rax)
+   18000b2aa:	add    %al,(%rax)
+   18000b2ac:	mov    $0xb2,%al
+   18000b2ae:	add    %al,(%rax)
+   18000b2b0:	push   $0xb2b9
+   18000b2b5:	mov    $0x20000b2,%edi
+   18000b2ba:	(bad)
+   18000b2bb:	jl     0x18000b23f
+   18000b2bd:	add    %al,(%rax)
+   18000b2bf:	add    $0x2a,%al
+   18000b2c1:	add    %bh,(%rdx,%rax,1)
+   18000b2c4:	add    %ecx,(%rsi)
+   18000b2c6:	(bad)
+   18000b2c7:	add    %cl,(%rsi)
+   18000b2c9:	xor    $0xb,%al
+   18000b2cb:	add    %cl,(%rsi)
+   18000b2cd:	xor    (%rdx),%cl
+   18000b2cf:	lock or %ah,%al
+   18000b2d2:	(bad)
+   18000b2d3:	(bad)
+   18000b2d4:	and    %edx,(%rbx)
    18000b2d6:	(bad)
-   18000b2d7:	adc    %al,-0x1fd60000(%rdx)
-   18000b2dd:	sub    $0x36800000,%eax
-   18000b2e2:	mov    $0x5e00007f,%esp
-   18000b2e7:	rex (bad)
-   18000b2e9:	add    %al,(%rax)
-   18000b2eb:	sub    $0x70,%al
-   18000b2ed:	sub    $0x0,%al
-   18000b2ef:	add    %al,-0x7d8fc1fd(%rcx)
-   18000b2f5:	add    %al,(%rax)
-   18000b2f7:	loop   0x18000b279
-   18000b2f9:	sub    $0x0,%al
-   18000b2fb:	add    %al,0x2860c03(%rcx)
-   18000b301:	rex.X (bad)
-   18000b303:	lret   $0xde04
-   18000b306:	or     $0x36,%al
-   18000b308:	(bad)
-   18000b309:	leave
-   18000b30a:	add    (%rcx,%rbx,1),%al
-   18000b30d:	and    %ecx,(%rax,%rax,1)
-   18000b310:	and    %ebp,0x3(%rax)
-   18000b313:	add    %bl,(%rsp,%riz,2)
-   18000b316:	adc    %eax,(%rax)
-   18000b318:	sbb    $0x34,%al
-   18000b31a:	adc    %al,(%rax)
-   18000b31c:	sbb    $0x72,%al
-   18000b31e:	sbb    %dh,%al
-   18000b320:	(bad)
-   18000b321:	loopne 0x18000b337
-   18000b323:	rclb   (%rdx)
-   18000b325:	rclb   $0x70,(%rax)
-   18000b328:	mov    $0x7f,%al
-   18000b32a:	add    %al,(%rax)
-   18000b32c:	xor    %dh,0x3d380000(%rbx)
-   18000b332:	mov    $0x0,%cl
-   18000b334:	add    %bh,0x4c0000b3(%rip)        # 0x1cc00b3ed
-   18000b33a:	mov    $0x0,%bl
-   18000b33c:	add    %al,(%rdx)
-   18000b33e:	add    %al,(%rax)
-   18000b340:	add    -0x4d(%rbp),%al
-   18000b343:	add    %al,(%rax)
-   18000b345:	add    (%rcx),%al
-   18000b347:	xorb   $0x0,-0x7f(%rax)
-   18000b34b:	add    %al,(%rdx)
-   18000b34d:	and    %eax,(%rbx)
-   18000b34f:	add    %al,(%rcx)
-   18000b351:	(bad)
-   18000b352:	add    (%rax),%al
-   18000b354:	(bad)
-   18000b355:	add    %edx,(%rbx)
-   18000b357:	add    %ah,(%rcx)
-   18000b359:	sub    %al,(%rsi)
-   18000b35b:	add    %ch,(%rax)
-   18000b35d:	mov    %al,(%rsi)
-   18000b35f:	add    %dl,(%rdx)
-   18000b361:	js     0x18000b36a
-   18000b363:	add    %cl,(%rax)
-   18000b365:	push   $0x25600008
-   18000b36a:	add    %al,(%rax)
-   18000b36c:	movsl  %ds:(%rsi),%es:(%rdi)
-   18000b36d:	and    $0xb3500000,%eax
-   18000b372:	add    %al,(%rax)
-   18000b374:	and    %eax,(%rax)
-   18000b376:	add    %al,(%rax)
-   18000b378:	(bad)
-   18000b379:	and    $0x25a50000,%eax
-   18000b37e:	add    %al,(%rax)
-   18000b380:	push   %rax
-   18000b381:	mov    $0x0,%bl
-   18000b383:	add    %bl,(%rcx)
-   18000b385:	adc    %al,(%rsi)
-   18000b387:	add    %dl,(%rax)
-   18000b389:	xor    (%rax,%rsi,8),%cl
-   18000b38c:	or     %al,%ah
-   18000b38e:	or     %dh,0x7(%rax)
-   18000b391:	(bad)
-   18000b392:	(bad)
-   18000b393:	xor    %dh,-0x63ffff81(%rax)
-   18000b399:	mov    $0x0,%bl
-   18000b39b:	add    %bh,(%rax)
-   18000b39d:	cmp    $0xa90000b1,%eax
-   18000b3a2:	mov    $0x0,%bl
-   18000b3a4:	add    %bh,0x20000b3(%rax)
-   18000b3aa:	add    %al,(%rax)
-   18000b3ac:	add    0x20000b3(%rcx),%dh
-   18000b3b2:	add    %eax,0x81d0(%rax)
-   18000b3b8:	add    0x2(%rcx),%bl
-   18000b3bb:	add    %bl,(%rcx)
-   18000b3bd:	adc    (%rsi),%al
-   18000b3bf:	add    %dl,(%rdx)
-   18000b3c1:	xor    $0xa,%al
-   18000b3c3:	add    %dl,(%rdx)
-   18000b3c5:	xor    (%rsi),%cl
-   18000b3c7:	loopne 0x18000b3d5
-   18000b3c9:	jo     0x18000b3d6
-   18000b3cb:	(bad)
-   18000b3cc:	mov    $0x7f,%al
-   18000b3ce:	add    %al,(%rax)
-   18000b3d0:	(bad)
-   18000b3d1:	mov    $0x0,%bl
-   18000b3d3:	add    %bh,(%rax)
-   18000b3d5:	cmp    $0xe10000b1,%eax
-   18000b3da:	mov    $0x0,%bl
-   18000b3dc:	add    %dh,%al
-   18000b3de:	mov    $0x0,%bl
-   18000b3e0:	add    %al,(%rdx)
-   18000b3e2:	add    %al,(%rax)
-   18000b3e4:	add    %cl,%ch
-   18000b3e6:	mov    $0x0,%bl
-   18000b3e8:	add    %al,(%rdx)
-   18000b3ea:	add    %eax,0x81a0(%rax)
-   18000b3f0:	add    0x2(%rbp),%dl
-   18000b3f3:	add    %bl,(%rcx)
-   18000b3f5:	add    $0x1,%al
-   18000b3f7:	add    %al,(%rdx,%rax,2)
-   18000b3fa:	add    %al,(%rax)
-   18000b3fc:	mov    $0x7f,%al
-   18000b3fe:	add    %al,(%rax)
-   18000b400:	add    $0xb4,%al
-   18000b402:	add    %al,(%rax)
-   18000b404:	cmp    %bh,0x110000b1(%rip)        # 0x19100b4bb
-   18000b40a:	mov    $0x0,%ah
-   18000b40c:	add    %ah,(%rax)
-   18000b40e:	mov    $0x0,%ah
-   18000b410:	add    %al,(%rdx)
-   18000b412:	add    %al,(%rax)
-   18000b414:	add    (%rcx),%bl
-   18000b416:	mov    $0x0,%ah
-   18000b418:	add    %al,(%rdx)
-   18000b41a:	add    %eax,0x8120(%rax)
-   18000b420:	add    %al,(%rax)
-   18000b422:	add    %al,(%rax)
-   18000b424:	adc    %ebx,(%rax)
-   18000b426:	add    $0x14621800,%eax
-   18000b42b:	loopne 0x18000b43f
-   18000b42d:	jo     0x18000b440
-   18000b42f:	(bad)
-   18000b430:	adc    %dh,(%rax)
-   18000b432:	add    %al,(%rax)
-   18000b434:	clc
-   18000b435:	jg     0x18000b437
-   18000b437:	add    %al,(%rcx)
-   18000b439:	add    %al,(%rax)
-   18000b43b:	add    %bl,(%rdi)
-   18000b43d:	jo     0x18000b43f
-   18000b43f:	add    %cl,0x70(%rbp)
+   18000b2d7:	add    %dl,(%rbx)
+   18000b2d9:	(bad)
+   18000b2da:	or     (%rax),%al
+   18000b2dc:	(bad)
+   18000b2dd:	je     0x18000b2e8
+   18000b2df:	add    %al,-0x2ffff7ac(%rip)        # 0x15000bb39
+   18000b2e5:	sbb    (%rax),%al
+   18000b2e7:	add    %al,(%rdx)
+   18000b2e9:	sbb    (%rax),%eax
+   18000b2eb:	add    %al,%ah
+   18000b2ed:	mov    $0x0,%dl
+   18000b2ef:	add    %ah,(%rcx)
+   18000b2f1:	add    %al,(%rax)
+   18000b2f3:	add    %dl,%al
+   18000b2f5:	sbb    (%rax),%al
+   18000b2f7:	add    %al,(%rdx)
+   18000b2f9:	sbb    (%rax),%eax
+   18000b2fb:	add    %al,%ah
+   18000b2fd:	mov    $0x0,%dl
+   18000b2ff:	add    %ah,(%rcx)
+   18000b301:	add    %al,(%rsi)
+   18000b303:	add    %al,(%rax)
+   18000b305:	(bad)
+   18000b306:	or     (%rax),%al
+   18000b308:	add    %dh,0x0(%rcx,%rcx,1)
+   18000b30c:	add    %dl,0x0(%rax,%rcx,1)
+   18000b310:	rcrb   (%rdx)
+   18000b312:	add    %al,(%rax)
+   18000b314:	add    (%rbx),%bl
+   18000b316:	add    %al,(%rax)
+   18000b318:	(bad)
+   18000b319:	mov    $0x0,%dl
+   18000b31b:	add    %dl,(%rcx)
+   18000b31d:	sbb    $0xb,%al
+   18000b31f:	add    %bl,(%rsp,%rsi,1)
+   18000b322:	sbb    (%rax),%al
+   18000b324:	sbb    $0x1,%al
+   18000b326:	adc    (%rax),%al
+   18000b328:	adc    $0x11e013f0,%eax
+   18000b32d:	rorb   (%rdi)
+   18000b32f:	rorb   $0x50,0xb600c70(%rip)        # 0x18b60bfa6
+   18000b336:	add    %al,(%rax)
+   18000b338:	jo     0x18000b2bc
+   18000b33a:	add    %al,(%rax)
+   18000b33c:	rex mov $0x0,%bl
+   18000b33f:	add    %ch,(%rax)
+   18000b341:	rex.WB mov $0x0,%r11b
+   18000b344:	add    %dh,-0x4d(%rdx)
+   18000b347:	add    %al,(%rax)
+   18000b349:	(bad)
+   18000b34a:	(bad)
+   18000b34b:	rolb   0x2de02a00(%rax,%rax,1)
+   18000b352:	add    %al,(%rax)
+   18000b354:	xorb   $0x7c,(%rsi)
+   18000b357:	(bad)
+   18000b358:	add    %al,(%rax)
+   18000b35a:	pop    %rsi
+   18000b35b:	add    %al,0x702c0000(%rbp)
+   18000b361:	sub    $0x0,%al
+   18000b363:	add    %al,-0x7acfc1fd(%rcx)
+   18000b369:	add    %al,(%rax)
+   18000b36b:	loop   0x18000b2ed
+   18000b36d:	sub    $0x0,%al
+   18000b36f:	add    %al,0x2860c03(%rcx)
+   18000b375:	rex.X (bad)
+   18000b377:	lret   $0xde04
+   18000b37a:	or     $0x36,%al
+   18000b37c:	(bad)
+   18000b37d:	leave
+   18000b37e:	add    (%rcx,%rbx,1),%al
+   18000b381:	and    %ecx,(%rax,%rax,1)
+   18000b384:	and    %ebp,0x3(%rax)
+   18000b387:	add    %bl,(%rsp,%riz,2)
+   18000b38a:	adc    %eax,(%rax)
+   18000b38c:	sbb    $0x34,%al
+   18000b38e:	adc    %al,(%rax)
+   18000b390:	sbb    $0x72,%al
+   18000b392:	sbb    %dh,%al
+   18000b394:	(bad)
+   18000b395:	loopne 0x18000b3ab
+   18000b397:	rclb   (%rdx)
+   18000b399:	rclb   $0x70,(%rax)
+   18000b39c:	jo     0x18000b320
+   18000b39e:	add    %al,(%rax)
+   18000b3a0:	movsb  %ds:(%rsi),%es:(%rdi)
+   18000b3a1:	mov    $0x0,%bl
+   18000b3a3:	add    %bh,(%rax)
+   18000b3a5:	mov    $0xb1,%cl
+   18000b3a7:	add    %al,(%rax)
+   18000b3a9:	mov    $0xb3,%cl
+   18000b3ab:	add    %al,(%rax)
+   18000b3ad:	shlb   $0x0,0x20000(%rbx)
+   18000b3b4:	add    0x20000b3(%rcx),%bh
+   18000b3ba:	add    %eax,0x8430(%rax)
+   18000b3c0:	add    (%rcx),%ah
+   18000b3c2:	add    (%rax),%eax
+   18000b3c4:	add    %eax,(%rdi)
+   18000b3c6:	add    (%rax),%al
+   18000b3c8:	(bad)
+   18000b3c9:	add    %edx,(%rbx)
+   18000b3cb:	add    %ah,(%rcx)
+   18000b3cd:	sub    %al,(%rsi)
+   18000b3cf:	add    %ch,(%rax)
+   18000b3d1:	mov    %al,(%rsi)
+   18000b3d3:	add    %dl,(%rdx)
+   18000b3d5:	js     0x18000b3de
+   18000b3d7:	add    %cl,(%rax)
+   18000b3d9:	push   $0x25600008
+   18000b3de:	add    %al,(%rax)
+   18000b3e0:	movsl  %ds:(%rsi),%es:(%rdi)
+   18000b3e1:	and    $0xb3c40000,%eax
+   18000b3e6:	add    %al,(%rax)
+   18000b3e8:	and    %eax,(%rax)
+   18000b3ea:	add    %al,(%rax)
+   18000b3ec:	(bad)
+   18000b3ed:	and    $0x25a50000,%eax
+   18000b3f2:	add    %al,(%rax)
+   18000b3f4:	(bad)
+   18000b3f5:	mov    $0x0,%bl
+   18000b3f7:	add    %bl,(%rcx)
+   18000b3f9:	adc    %al,(%rsi)
+   18000b3fb:	add    %dl,(%rax)
+   18000b3fd:	xor    (%rax,%rsi,8),%cl
+   18000b400:	or     %al,%ah
+   18000b402:	or     %dh,0x7(%rax)
+   18000b405:	(bad)
+   18000b406:	(bad)
+   18000b407:	xor    %dh,-0x7e(%rax)
+   18000b40a:	add    %al,(%rax)
+   18000b40c:	adc    %dh,-0x4e4ec800(%rax,%rax,1)
+   18000b413:	add    %al,(%rax)
+   18000b415:	sbb    $0x2c0000b4,%eax
+   18000b41a:	mov    $0x0,%ah
+   18000b41c:	add    %al,(%rdx)
+   18000b41e:	add    %al,(%rax)
+   18000b420:	add    0x20000b4(%rip),%ah        # 0x18200b4da
+   18000b426:	add    %eax,0x8490(%rax)
+   18000b42c:	add    0x2(%rcx),%bl
+   18000b42f:	add    %bl,(%rcx)
+   18000b431:	adc    (%rsi),%al
+   18000b433:	add    %dl,(%rdx)
+   18000b435:	xor    $0xa,%al
+   18000b437:	add    %dl,(%rdx)
+   18000b439:	xor    (%rsi),%cl
+   18000b43b:	loopne 0x18000b449
+   18000b43d:	jo     0x18000b44a
+   18000b43f:	(bad)
+   18000b440:	jo     0x18000b3c4
    18000b442:	add    %al,(%rax)
-   18000b444:	insb   (%dx),%es:(%rdi)
-   18000b445:	test   %eax,(%rax)
-   18000b447:	add    %al,(%rax)
-   18000b449:	add    %al,(%rax)
-   18000b44b:	add    %cl,(%rcx)
-   18000b44d:	sbb    %cl,(%rax)
-   18000b44f:	add    %bl,(%rax)
-   18000b451:	adc    %al,%fs:(%rax)
-   18000b454:	sbb    %dh,(%rdi,%rcx,1)
-   18000b457:	add    %bl,(%rax)
-   18000b459:	xchg   %eax,%edx
-   18000b45a:	adc    $0xf0,%al
-   18000b45c:	adc    %al,%ah
-   18000b45e:	adc    %dh,-0x8(%rax)
-   18000b461:	jg     0x18000b463
-   18000b463:	add    %al,(%rcx)
-   18000b465:	add    %al,(%rax)
-   18000b467:	add    %bh,0x0(%rax,%rsi,2)
-   18000b46b:	add    %ah,-0x67ffff90(%rbx)
-   18000b471:	test   %eax,(%rax)
-   18000b473:	add    %ah,0x1000070(%rbx)
-   18000b479:	(bad)
-   18000b47a:	add    (%rax),%eax
-   18000b47c:	(bad)
-   18000b47d:	rex.X add 0x2(%rax),%edx
-   18000b481:	xor    %al,(%rax)
-   18000b483:	add    %al,(%rcx)
-   18000b485:	add    (%rcx),%al
+   18000b444:	rex.W mov $0x0,%spl
+   18000b447:	add    %bh,(%rax)
+   18000b449:	mov    $0xb1,%cl
+   18000b44b:	add    %al,(%rax)
+   18000b44d:	push   %rbp
+   18000b44e:	mov    $0x0,%ah
+   18000b450:	add    %ah,0x0(%rsp,%rsi,4)
+   18000b454:	add    %al,(%rdx)
+   18000b456:	add    %al,(%rax)
+   18000b458:	add    -0x4c(%rbp),%bl
+   18000b45b:	add    %al,(%rax)
+   18000b45d:	add    (%rcx),%al
+   18000b45f:	andb   $0x0,-0x7c(%rax)
+   18000b463:	add    %al,(%rdx)
+   18000b465:	push   %rbp
+   18000b466:	add    (%rax),%al
+   18000b468:	sbb    %eax,(%rcx,%rax,1)
+   18000b46b:	add    %al,(%rdx,%rax,2)
+   18000b46e:	add    %al,(%rax)
+   18000b470:	jo     0x18000b3f4
+   18000b472:	add    %al,(%rax)
+   18000b474:	js     0x18000b42a
+   18000b476:	add    %al,(%rax)
+   18000b478:	cmp    %dh,-0x7affff4f(%rcx)
+   18000b47e:	mov    $0x0,%ah
+   18000b480:	add    %dl,0x20000(%rsp,%rsi,4)
    18000b487:	add    %al,(%rdx)
-   18000b489:	xor    %al,(%rax)
-   18000b48b:	add    %al,(%rcx)
-   18000b48d:	sbb    %ecx,(%rdx)
-   18000b48f:	add    %bl,(%rcx)
-   18000b491:	je     0x18000b49c
-   18000b493:	add    %bl,(%rcx)
-   18000b495:	or     %al,%fs:(%rax)
-   18000b498:	sbb    %edx,0x0(%rdi,%rax,1)
-   18000b49c:	sbb    %esi,(%rsi,%rax,1)
-   18000b49f:	add    %bl,(%rcx)
-   18000b4a1:	xor    0xe0(%rip),%dl        # 0x18000b587
-   18000b4a7:	add    %al,(%rcx)
-   18000b4a9:	add    %al,(%rax)
-   18000b4ab:	add    %dl,(%rcx)
-   18000b4ad:	adc    $0x74150008,%eax
-   18000b4b2:	or     %eax,(%rax)
-   18000b4b4:	adc    $0x15000764,%eax
-   18000b4b9:	xor    $0x6,%al
-   18000b4bb:	add    %dl,-0x71feece(%rip)        # 0x178e0c5f3
-   18000b4c1:	jg     0x18000b4c3
-   18000b4c3:	add    %al,(%rdx)
-   18000b4c5:	add    %al,(%rax)
-   18000b4c7:	add    %al,(%rbx,%rsi,2)
-   18000b4ca:	add    %al,(%rax)
-   18000b4cc:	jae    0x18000b541
-   18000b4ce:	add    %al,(%rax)
-   18000b4d0:	testl  $0x73d60000,0x0(%rbp)
+   18000b489:	lea    -0x7ffefe00(%rax,%rax,1),%esi
+   18000b490:	loopne 0x18000b415
+   18000b492:	add    %al,(%rax)
+   18000b494:	add    %al,(%rax)
+   18000b496:	add    %al,(%rax)
+   18000b498:	adc    %ebx,(%rax)
+   18000b49a:	add    $0x14621800,%eax
+   18000b49f:	loopne 0x18000b4b3
+   18000b4a1:	jo     0x18000b4b4
+   18000b4a3:	(bad)
+   18000b4a4:	adc    %dh,(%rax)
+   18000b4a6:	add    %al,(%rax)
+   18000b4a8:	mov    $0x1000082,%eax
+   18000b4ad:	add    %al,(%rax)
+   18000b4af:	add    %bl,%bh
+   18000b4b1:	jb     0x18000b4b3
+   18000b4b3:	add    %cl,-0x73ffff8d(%rip)        # 0x10c00b52c
+   18000b4b9:	mov    %al,(%rax)
+   18000b4bb:	add    %al,(%rax)
+   18000b4bd:	add    %al,(%rax)
+   18000b4bf:	add    %cl,(%rcx)
+   18000b4c1:	sbb    %cl,(%rax)
+   18000b4c3:	add    %bl,(%rax)
+   18000b4c5:	adc    %al,%fs:(%rax)
+   18000b4c8:	sbb    %dh,(%rdi,%rcx,1)
+   18000b4cb:	add    %bl,(%rax)
+   18000b4cd:	xchg   %eax,%edx
+   18000b4ce:	adc    $0xf0,%al
+   18000b4d0:	adc    %al,%ah
+   18000b4d2:	adc    %dh,-0x48(%rax)
+   18000b4d5:	(bad)
+   18000b4d6:	add    %al,(%rax)
+   18000b4d8:	add    %eax,(%rax)
    18000b4da:	add    %al,(%rax)
-   18000b4dc:	loope  0x18000b551
+   18000b4dc:	cmp    $0x73,%al
    18000b4de:	add    %al,(%rax)
-   18000b4e0:	testl  $0xa110000,0x0(%rbp)
-   18000b4ea:	add    $0x0,%al
-   18000b4ec:	or     (%rax,%rcx,1),%dh
-   18000b4ef:	add    %cl,(%rdx)
-   18000b4f1:	push   %rdx
-   18000b4f2:	(bad)
-   18000b4f3:	jo     0x18000b4ed
-   18000b4f5:	jg     0x18000b4f7
-   18000b4f7:	add    %al,(%rax,%rax,1)
-   18000b4fa:	add    %al,(%rax)
-   18000b4fc:	sbb    0x0(%rax,%rax,1),%esi
-   18000b500:	cmp    0x0(%rax,%rax,1),%dh
-   18000b504:	(bad)
-   18000b505:	xchg   %al,(%rax)
-   18000b507:	add    %al,(%rax)
-   18000b509:	add    %al,(%rax)
-   18000b50b:	add    %dl,(%rax)
-   18000b50d:	je     0x18000b50f
-   18000b50f:	add    %dl,0x74(%rdx)
-   18000b512:	add    %al,(%rax)
-   18000b514:	(bad)
-   18000b515:	xchg   %al,(%rax)
-   18000b517:	add    %al,(%rax)
-   18000b519:	add    %al,(%rax)
-   18000b51b:	add    %bl,0x74(%rbx)
-   18000b51e:	add    %al,(%rax)
-   18000b520:	data16 je 0x18000b523
-   18000b523:	add    %cl,(%rsi)
-   18000b525:	xchg   %al,(%rax)
-   18000b527:	add    %al,(%rax)
-   18000b529:	add    %al,(%rax)
-   18000b52b:	add    %bl,0x74(%rbx)
-   18000b52e:	add    %al,(%rax)
-   18000b530:	addr32 je 0x18000b533
-   18000b533:	add    %ah,(%rdi)
-   18000b535:	xchg   %al,(%rax)
-   18000b537:	add    %al,(%rax)
-   18000b539:	add    %al,(%rax)
-   18000b53b:	add    %cl,(%rcx)
-   18000b53d:	sbb    (%rsi),%al
-   18000b53f:	add    %bl,(%rdx)
-   18000b541:	xor    $0xf,%al
-   18000b543:	add    %bl,(%rdx)
-   18000b545:	jb     0x18000b55d
-   18000b547:	loopne 0x18000b55d
-   18000b549:	jo     0x18000b55e
-   18000b54b:	(bad)
-   18000b54c:	clc
-   18000b54d:	jg     0x18000b54f
-   18000b54f:	add    %al,(%rcx)
-   18000b551:	add    %al,(%rax)
-   18000b553:	add    %bl,-0x7cffff8c(%rbp)
-   18000b559:	jne    0x18000b55b
-   18000b55b:	add    %bh,(%rbx)
-   18000b55d:	xchg   %al,(%rax)
-   18000b55f:	add    %al,0x1000075(%rbx)
+   18000b4e0:	movsxd 0x0(%rbx),%esi
+   18000b4e3:	add    %bh,0x63000088(%rax)
+   18000b4e9:	jae    0x18000b4eb
+   18000b4eb:	add    %al,(%rcx)
+   18000b4ed:	(bad)
+   18000b4ee:	add    (%rax),%eax
+   18000b4f0:	(bad)
+   18000b4f1:	rex.X add 0x2(%rax),%edx
+   18000b4f5:	xor    %al,(%rax)
+   18000b4f7:	add    %al,(%rcx)
+   18000b4f9:	add    (%rcx),%al
+   18000b4fb:	add    %al,(%rdx)
+   18000b4fd:	xor    %al,(%rax)
+   18000b4ff:	add    %al,(%rcx)
+   18000b501:	sbb    %ecx,(%rdx)
+   18000b503:	add    %bl,(%rcx)
+   18000b505:	je     0x18000b510
+   18000b507:	add    %bl,(%rcx)
+   18000b509:	or     %al,%fs:(%rax)
+   18000b50c:	sbb    %edx,0x0(%rdi,%rax,1)
+   18000b510:	sbb    %esi,(%rsi,%rax,1)
+   18000b513:	add    %bl,(%rcx)
+   18000b515:	xor    0x1e0(%rip),%dl        # 0x18000b6fb
+   18000b51b:	add    %dl,(%rcx)
+   18000b51d:	adc    $0x74150008,%eax
+   18000b522:	or     %eax,(%rax)
+   18000b524:	adc    $0x15000764,%eax
+   18000b529:	xor    $0x6,%al
+   18000b52b:	add    %dl,-0x471feece(%rip)        # 0x138e0c663
+   18000b531:	(bad)
+   18000b532:	add    %al,(%rax)
+   18000b534:	add    (%rax),%al
+   18000b536:	add    %al,(%rax)
+   18000b538:	(bad)
+   18000b539:	jne    0x18000b53b
+   18000b53b:	add    %dh,(%rbx)
+   18000b53d:	jbe    0x18000b53f
+   18000b53f:	add    %dl,(%rdi)
+   18000b541:	mov    %eax,(%rax)
+   18000b543:	add    %al,(%rax)
+   18000b545:	add    %al,(%rax)
+   18000b547:	add    %dl,-0x5effff8a(%rsi)
+   18000b54d:	jbe    0x18000b54f
+   18000b54f:	add    %dl,(%rdi)
+   18000b551:	mov    %eax,(%rax)
+   18000b553:	add    %al,(%rax)
+   18000b555:	add    %al,(%rax)
+   18000b557:	add    %dl,(%rcx)
+   18000b559:	or     (%rax,%rax,1),%al
+   18000b55c:	or     (%rax,%rcx,1),%dh
+   18000b55f:	add    %cl,(%rdx)
+   18000b561:	push   %rdx
+   18000b562:	(bad)
+   18000b563:	jo     0x18000b51d
    18000b565:	(bad)
-   18000b566:	add    (%rax),%al
-   18000b568:	(bad)
-   18000b569:	push   %rdx
-   18000b56a:	add    0x9(%rax),%dl
-   18000b56d:	add    $0x1,%al
-   18000b56f:	add    %al,(%rdx,%riz,1)
-   18000b572:	add    %al,(%rax)
-   18000b574:	clc
-   18000b575:	jg     0x18000b577
-   18000b577:	add    %al,(%rcx)
+   18000b566:	add    %al,(%rax)
+   18000b568:	add    $0x0,%al
+   18000b56a:	add    %al,(%rax)
+   18000b56c:	(bad)  0x0(%rsi)
+   18000b56f:	add    %bh,%dl
+   18000b571:	jbe    0x18000b573
+   18000b573:	add    %ch,(%rsi)
+   18000b575:	mov    %eax,(%rax)
+   18000b577:	add    %al,(%rax)
    18000b579:	add    %al,(%rax)
-   18000b57b:	add    %ah,(%rdi)
-   18000b57d:	js     0x18000b57f
-   18000b57f:	add    %dh,0x71000078(%rcx)
-   18000b585:	xchg   %al,(%rax)
-   18000b587:	add    %dh,0x1000078(%rcx)
-   18000b58d:	add    (%rcx),%al
-   18000b58f:	add    %al,(%rdx)
-   18000b591:	push   %rax
-   18000b592:	add    %al,(%rax)
-   18000b594:	add    %ecx,(%rcx)
-   18000b596:	add    %eax,(%rax)
-   18000b598:	or     %esp,0x0(%rdx)
-   18000b59b:	add    %al,(%rcx)
-   18000b59d:	or     %al,(%rax,%rax,1)
-   18000b5a0:	or     %dh,0x4(%rdx)
-   18000b5a3:	jo     0x18000b5a8
-   18000b5a5:	(bad)
-   18000b5a6:	add    (%rax),%dh
-   18000b5a8:	add    %ecx,0x340d0004(%rip)        # 0x1b40db5b2
-   18000b5ae:	or     %eax,(%rax)
-   18000b5b0:	or     $0x1500632,%eax
-   18000b5b5:	adc    $0x34150005,%eax
-   18000b5ba:	mov    $0xb8011500,%edx
-   18000b5bf:	add    %al,(%rsi)
-   18000b5c1:	push   %rax
-   18000b5c2:	add    %al,(%rax)
-   18000b5c4:	add    %ecx,(%rdi)
-   18000b5c6:	(bad)
-   18000b5c7:	add    %cl,(%rdi)
-   18000b5c9:	fs (bad)
-   18000b5cb:	add    %cl,(%rdi)
-   18000b5cd:	xor    $0x5,%al
-   18000b5cf:	add    %cl,(%rdi)
-   18000b5d1:	adc    (%rbx),%cl
-   18000b5d3:	jo     0x18000b5d5
-   18000b5d5:	add    %al,(%rax)
-   18000b5d7:	add    %al,(%rcx)
-   18000b5d9:	add    %al,(%rax)
-   18000b5db:	add    %al,(%rax)
-   18000b5dd:	add    %al,(%rax)
-   18000b5df:	add    %al,(%rcx)
-	...
+   18000b57b:	add    %dl,%al
+   18000b57d:	jbe    0x18000b57f
+   18000b57f:	add    %dl,(%rdx)
+   18000b581:	ja     0x18000b583
+   18000b583:	add    %al,-0x77(%rdi)
+   18000b586:	add    %al,(%rax)
+   18000b588:	add    %al,(%rax)
+   18000b58a:	add    %al,(%rax)
+   18000b58c:	sbb    0x0(%rdi),%esi
+   18000b58f:	add    %ah,(%rsi)
+   18000b591:	ja     0x18000b593
+   18000b593:	add    %ch,(%rsi)
+   18000b595:	mov    %eax,(%rax)
+   18000b597:	add    %al,(%rax)
+   18000b599:	add    %al,(%rax)
+   18000b59b:	add    %bl,(%rbx)
+   18000b59d:	ja     0x18000b59f
+   18000b59f:	add    %ah,(%rdi)
+   18000b5a1:	ja     0x18000b5a3
+   18000b5a3:	add    %al,-0x77(%rdi)
+   18000b5a6:	add    %al,(%rax)
+   18000b5a8:	add    %al,(%rax)
+   18000b5aa:	add    %al,(%rax)
+   18000b5ac:	or     %ebx,(%rdx)
+   18000b5ae:	(bad)
+   18000b5af:	add    %bl,(%rdx)
+   18000b5b1:	xor    $0xf,%al
+   18000b5b3:	add    %bl,(%rdx)
+   18000b5b5:	jb     0x18000b5cd
+   18000b5b7:	loopne 0x18000b5cd
+   18000b5b9:	jo     0x18000b5ce
+   18000b5bb:	(bad)
+   18000b5bc:	mov    $0x1000082,%eax
+   18000b5c1:	add    %al,(%rax)
+   18000b5c3:	add    %bl,0x77(%rbp)
+   18000b5c6:	add    %al,(%rax)
+   18000b5c8:	rex.XB js 0x18000b5cb
+   18000b5cb:	add    %bl,-0x77(%rbx)
+   18000b5ce:	add    %al,(%rax)
+   18000b5d0:	rex.XB js 0x18000b5d3
+   18000b5d3:	add    %al,(%rcx)
+   18000b5d5:	(bad)
+   18000b5d6:	add    (%rax),%al
+   18000b5d8:	(bad)
+   18000b5d9:	push   %rdx
+   18000b5da:	add    0x9(%rax),%dl
+   18000b5dd:	add    $0x1,%al
+   18000b5df:	add    %al,(%rdx,%riz,1)
+   18000b5e2:	add    %al,(%rax)
+   18000b5e4:	mov    $0x1000082,%eax
    18000b5e9:	add    %al,(%rax)
-   18000b5eb:	add    %dl,0x31(%rax)
-   18000b5ee:	add    %al,(%rax)
-   18000b5f0:	add    %al,(%rax)
+   18000b5eb:	add    %ah,%bh
+   18000b5ed:	jp     0x18000b5ef
+   18000b5ef:	add    %dh,0x7b(%rcx)
    18000b5f2:	add    %al,(%rax)
-   18000b5f4:	or     %dh,0x0(%rsi)
-	...
-   18000b606:	add    %al,(%rax)
-   18000b608:	add    (%rax),%eax
+   18000b5f4:	xchg   %eax,%ecx
+   18000b5f5:	mov    %eax,(%rax)
+   18000b5f7:	add    %dh,0x7b(%rcx)
+   18000b5fa:	add    %al,(%rax)
+   18000b5fc:	add    %eax,(%rdx)
+   18000b5fe:	add    %eax,(%rax)
+   18000b600:	add    0x0(%rax),%dl
+   18000b603:	add    %al,(%rcx)
+   18000b605:	or     %eax,(%rcx)
+   18000b607:	add    %cl,(%rcx)
+   18000b609:	(bad)
    18000b60a:	add    %al,(%rax)
-   18000b60c:	sub    %dh,-0x49b00000(%rsi)
-   18000b612:	add    %al,(%rax)
-   18000b614:	js     0x18000b5cc
-	...
-   18000b62a:	add    %al,(%rax)
-   18000b62c:	movabs 0xff000000000000e0,%al
-   18000b635:	(bad)
+   18000b60c:	add    %ecx,(%rax)
+   18000b60e:	add    $0x0,%al
+   18000b610:	or     %dh,0x4(%rdx)
+   18000b613:	jo     0x18000b618
+   18000b615:	(bad)
+   18000b616:	add    (%rax),%dh
+   18000b618:	add    %ecx,0x340d0004(%rip)        # 0x1b40db622
+   18000b61e:	or     %eax,(%rax)
+   18000b620:	or     $0x1500632,%eax
+   18000b625:	adc    $0x34150005,%eax
+   18000b62a:	mov    $0xb8011500,%edx
+   18000b62f:	add    %al,(%rsi)
+   18000b631:	push   %rax
+   18000b632:	add    %al,(%rax)
+   18000b634:	add    %ecx,(%rdi)
    18000b636:	(bad)
-   18000b637:	incl   (%rax)
-   18000b639:	add    %al,(%rax)
-   18000b63b:	add    %bl,(%rax)
-   18000b63d:	add    %al,(%rax)
-   18000b63f:	add    %al,%al
-   18000b641:	sub    (%rax),%al
-	...
-   18000b64f:	add    %dl,(%rax)
-   18000b651:	add    %al,(%rax)
-   18000b653:	add    %dl,%al
-   18000b655:	loopne 0x18000b657
-   18000b657:	add    %al,(%rax)
+   18000b637:	add    %cl,(%rdi)
+   18000b639:	fs (bad)
+   18000b63b:	add    %cl,(%rdi)
+   18000b63d:	xor    $0x5,%al
+   18000b63f:	add    %cl,(%rdi)
+   18000b641:	adc    (%rbx),%cl
+   18000b643:	jo     0x18000b645
+   18000b645:	add    %al,(%rax)
+   18000b647:	add    %al,(%rcx)
+   18000b649:	add    %al,(%rax)
+   18000b64b:	add    %al,(%rax)
+   18000b64d:	add    %al,(%rax)
+   18000b64f:	add    %al,(%rcx)
+	...
    18000b659:	add    %al,(%rax)
-   18000b65b:	add    %bh,%bh
-   18000b65d:	(bad)
-   18000b65e:	(bad)
-   18000b65f:	incl   (%rax)
-   18000b661:	add    %al,(%rax)
-   18000b663:	add    %bl,(%rax)
-   18000b665:	add    %al,(%rax)
-   18000b667:	add    %al,0x2a(%rax)
-	...
-   18000b679:	add    %al,(%rax)
-   18000b67b:	add    %bh,%al
-   18000b67d:	loopne 0x18000b67f
-   18000b67f:	add    %al,(%rax)
-   18000b681:	add    %al,(%rax)
-   18000b683:	add    %bh,%bh
-   18000b685:	(bad)
-   18000b686:	(bad)
-   18000b687:	incl   (%rax)
-   18000b689:	add    %al,(%rax)
-   18000b68b:	add    %bl,(%rax)
-   18000b68d:	add    %al,(%rax)
-   18000b68f:	add    %ah,0x2b(%rax)
+   18000b65b:	add    %dl,0x31(%rax)
+   18000b65e:	add    %al,(%rax)
+   18000b660:	add    %al,(%rax)
+   18000b662:	add    %al,(%rax)
+   18000b664:	js     0x18000b61c
+	...
+   18000b676:	add    %al,(%rax)
+   18000b678:	add    (%rax),%eax
+   18000b67a:	add    %al,(%rax)
+   18000b67c:	cwtl
+   18000b67d:	mov    $0x0,%dh
+   18000b67f:	add    %al,%al
+   18000b681:	mov    $0x0,%dh
+   18000b683:	add    %ch,%al
+   18000b685:	mov    $0x0,%dh
 	...
+   18000b69b:	add    %ah,0xe0(%rax)
    18000b6a1:	add    %al,(%rax)
-   18000b6a3:	add    %ah,(%rax)
-   18000b6a5:	loope  0x18000b6a7
-   18000b6a7:	add    %al,(%rax)
+   18000b6a3:	add    %bh,%bh
+   18000b6a5:	(bad)
+   18000b6a6:	(bad)
+   18000b6a7:	incl   (%rax)
    18000b6a9:	add    %al,(%rax)
-   18000b6ab:	add    %bh,%bh
-   18000b6ad:	(bad)
-   18000b6ae:	(bad)
-   18000b6af:	incl   (%rax)
-   18000b6b1:	add    %al,(%rax)
-   18000b6b3:	add    %bl,(%rax)
-   18000b6b5:	add    %al,(%rax)
-   18000b6b7:	add    %ah,%al
-   18000b6b9:	sub    (%rax),%eax
-	...
-   18000b6cb:	add    %dl,0x31(%rax)
-   18000b6ce:	add    %al,(%rax)
-   18000b6d0:	add    %al,(%rax)
-   18000b6d2:	add    %al,(%rax)
-   18000b6d4:	call   0x18000b78f
+   18000b6ab:	add    %bl,(%rax)
+   18000b6ad:	add    %al,(%rax)
+   18000b6af:	add    %al,%al
+   18000b6b1:	sub    (%rax),%al
+	...
+   18000b6bf:	add    %dl,(%rax)
+   18000b6c1:	add    %al,(%rax)
+   18000b6c3:	add    %dl,%al
+   18000b6c5:	loopne 0x18000b6c7
+   18000b6c7:	add    %al,(%rax)
+   18000b6c9:	add    %al,(%rax)
+   18000b6cb:	add    %bh,%bh
+   18000b6cd:	(bad)
+   18000b6ce:	(bad)
+   18000b6cf:	incl   (%rax)
+   18000b6d1:	add    %al,(%rax)
+   18000b6d3:	add    %bl,(%rax)
+   18000b6d5:	add    %al,(%rax)
+   18000b6d7:	add    %al,0x2a(%rax)
 	...
-   18000b6e5:	add    %al,(%rax)
-   18000b6e7:	add    %al,(%rdx)
    18000b6e9:	add    %al,(%rax)
-   18000b6eb:	add    %al,(%rax)
-   18000b6ed:	mov    $0x0,%bh
-   18000b6ef:	add    %bh,-0x4a(%rax)
-	...
-   18000b702:	add    %al,(%rax)
-   18000b704:	rex.W loope 0x18000b707
-   18000b707:	add    %al,(%rax)
-   18000b709:	add    %al,(%rax)
-   18000b70b:	add    %bh,%bh
-   18000b70d:	(bad)
-   18000b70e:	(bad)
-   18000b70f:	incl   (%rax)
+   18000b6eb:	add    %bh,%al
+   18000b6ed:	loopne 0x18000b6ef
+   18000b6ef:	add    %al,(%rax)
+   18000b6f1:	add    %al,(%rax)
+   18000b6f3:	add    %bh,%bh
+   18000b6f5:	(bad)
+   18000b6f6:	(bad)
+   18000b6f7:	incl   (%rax)
+   18000b6f9:	add    %al,(%rax)
+   18000b6fb:	add    %bl,(%rax)
+   18000b6fd:	add    %al,(%rax)
+   18000b6ff:	add    %ah,0x2b(%rax)
+	...
    18000b711:	add    %al,(%rax)
-   18000b713:	add    %bl,(%rax)
-   18000b715:	add    %al,(%rax)
-   18000b717:	add    %dh,(%rax)
-   18000b719:	sub    (%rax),%eax
-	...
-   18000b72b:	add    %dl,0x31(%rax)
-   18000b72e:	add    %al,(%rax)
-   18000b730:	add    %al,(%rax)
-   18000b732:	add    %al,(%rax)
-   18000b734:	rex.W mov $0x0,%dil
-	...
-   18000b747:	add    %al,(%rbx)
-   18000b749:	add    %al,(%rax)
-   18000b74b:	add    %ch,-0x49(%rax)
-   18000b74e:	add    %al,(%rax)
-   18000b750:	movabs 0xb6780000b6,%al
-	...
-   18000b769:	add    %al,(%rax)
-   18000b76b:	add    %dh,-0x1f(%rax)
-   18000b76e:	add    %al,(%rax)
-   18000b770:	add    %al,(%rax)
-   18000b772:	add    %al,(%rax)
-   18000b774:	(bad)
-   18000b775:	(bad)
-   18000b776:	(bad)
-   18000b777:	incl   (%rax)
-   18000b779:	add    %al,(%rax)
-   18000b77b:	add    %bl,(%rax)
-   18000b77d:	add    %al,(%rax)
-   18000b77f:	add    %al,0x28(%rax)
-	...
-   18000b791:	add    %al,(%rax)
-   18000b793:	add    %dl,0x31(%rax)
-   18000b796:	add    %al,(%rax)
-   18000b798:	add    %al,(%rax)
-   18000b79a:	add    %al,(%rax)
-   18000b79c:	mov    $0xb7,%al
-	...
-   18000b7ae:	add    %al,(%rax)
-   18000b7b0:	add    (%rax),%al
-   18000b7b2:	add    %al,(%rax)
-   18000b7b4:	push   %rax
-   18000b7b5:	mov    $0x0,%dh
-   18000b7b7:	add    %bh,-0x4a(%rax)
-	...
-   18000b7d2:	add    %al,(%rax)
-   18000b7d4:	(bad)
-   18000b7d5:	(bad)
-   18000b7d6:	(bad)
-   18000b7d7:	incl   (%rax)
-   18000b7d9:	add    %al,(%rax)
-   18000b7db:	add    %dh,(%rax,%rdi,4)
+   18000b713:	add    %ah,(%rax)
+   18000b715:	loope  0x18000b717
+   18000b717:	add    %al,(%rax)
+   18000b719:	add    %al,(%rax)
+   18000b71b:	add    %bh,%bh
+   18000b71d:	(bad)
+   18000b71e:	(bad)
+   18000b71f:	incl   (%rax)
+   18000b721:	add    %al,(%rax)
+   18000b723:	add    %bl,(%rax)
+   18000b725:	add    %al,(%rax)
+   18000b727:	add    %ah,%al
+   18000b729:	sub    (%rax),%eax
+	...
+   18000b73b:	add    %dl,0x31(%rax)
+   18000b73e:	add    %al,(%rax)
+   18000b740:	add    %al,(%rax)
+   18000b742:	add    %al,(%rax)
+   18000b744:	pop    %rax
+   18000b745:	mov    $0x0,%bh
+	...
+   18000b757:	add    %al,(%rdx)
+   18000b759:	add    %al,(%rax)
+   18000b75b:	add    %dh,-0x49(%rax)
+   18000b75e:	add    %al,(%rax)
+   18000b760:	call   0x18000b81b
+	...
+   18000b771:	add    %al,(%rax)
+   18000b773:	add    %cl,-0x1f(%rax)
+   18000b776:	add    %al,(%rax)
+   18000b778:	add    %al,(%rax)
+   18000b77a:	add    %al,(%rax)
+   18000b77c:	(bad)
+   18000b77d:	(bad)
+   18000b77e:	(bad)
+   18000b77f:	incl   (%rax)
+   18000b781:	add    %al,(%rax)
+   18000b783:	add    %bl,(%rax)
+   18000b785:	add    %al,(%rax)
+   18000b787:	add    %dh,(%rax)
+   18000b789:	sub    (%rax),%eax
+	...
+   18000b79b:	add    %dl,0x31(%rax)
+   18000b79e:	add    %al,(%rax)
+   18000b7a0:	add    %al,(%rax)
+   18000b7a2:	add    %al,(%rax)
+   18000b7a4:	mov    $0xb7,%eax
+	...
+   18000b7b5:	add    %al,(%rax)
+   18000b7b7:	add    %al,(%rbx)
+   18000b7b9:	add    %al,(%rax)
+   18000b7bb:	add    %bl,%al
+   18000b7bd:	mov    $0x0,%bh
+   18000b7bf:	add    %dl,(%rax)
+   18000b7c1:	mov    $0x0,%bh
+   18000b7c3:	add    %ch,%al
+   18000b7c5:	mov    $0x0,%dh
+	...
+   18000b7db:	add    %dh,-0x1f(%rax)
    18000b7de:	add    %al,(%rax)
-   18000b7e0:	add    %eax,(%rax)
+   18000b7e0:	add    %al,(%rax)
    18000b7e2:	add    %al,(%rax)
    18000b7e4:	(bad)
-   18000b7e5:	add    %al,(%rax)
-   18000b7e7:	add    %al,(%rsi)
+   18000b7e5:	(bad)
+   18000b7e6:	(bad)
+   18000b7e7:	incl   (%rax)
    18000b7e9:	add    %al,(%rax)
-   18000b7eb:	add    %bh,%al
-   18000b7ed:	mov    $0x0,%bh
-   18000b7ef:	add    %dl,(%rax)
-   18000b7f1:	mov    $0xb8280000,%eax
-   18000b7f6:	add    %al,(%rax)
-   18000b7f8:	adc    %dl,(%rax)
-   18000b7fa:	add    %al,(%rax)
-   18000b7fc:	rex adc %al,(%rax)
-   18000b7ff:	add    %dh,%al
-   18000b801:	xchg   %eax,%esp
-   18000b802:	add    %al,(%rax)
-   18000b804:	loopne 0x18000b816
+   18000b7eb:	add    %bl,(%rax)
+   18000b7ed:	add    %al,(%rax)
+   18000b7ef:	add    %al,0x28(%rax)
+	...
+   18000b801:	add    %al,(%rax)
+   18000b803:	add    %dl,0x31(%rax)
    18000b806:	add    %al,(%rax)
-   18000b808:	lock adc %al,(%rax)
-   18000b80b:	add    %dl,0x52000056(%rax)
-   18000b811:	mov    $0xb87d0000,%eax
-   18000b816:	add    %al,(%rax)
-   18000b818:	test   $0xb8,%al
-   18000b81a:	add    %al,(%rax)
-   18000b81c:	sarb   -0x46f90000(%rax)
+   18000b808:	add    %al,(%rax)
+   18000b80a:	add    %al,(%rax)
+   18000b80c:	and    %bh,0x0(%rax)
+	...
+   18000b81e:	add    %al,(%rax)
+   18000b820:	add    (%rax),%al
    18000b822:	add    %al,(%rax)
-   18000b824:	cmp    %edi,0x0(%rcx)
-   18000b82a:	add    %eax,(%rax)
-   18000b82c:	add    (%rax),%al
-   18000b82e:	add    (%rax),%eax
-   18000b830:	add    $0x0,%al
-   18000b832:	add    $0x6f654700,%eax
-   18000b837:	fs gs sub $0x77656956,%eax
-   18000b83e:	(bad)
-   18000b83f:	(bad)
-   18000b840:	insb   (%dx),%es:(%rdi)
-   18000b841:	gs jae 0x18000b8a3
-   18000b844:	jno    0x18000b8ab
-   18000b846:	insl   (%dx),%es:(%rdi)
-   18000b847:	pop    %rdi
-   18000b848:	jo     0x18000b8bc
-   18000b84a:	outsl  %ds:(%rsi),(%dx)
-   18000b84b:	js     0x18000b8c6
-   18000b84d:	cs fs insb (%dx),%es:(%rdi)
-   18000b850:	insb   (%dx),%es:(%rdi)
-   18000b851:	add    %bh,(%rdi)
-   18000b853:	(bad)
-   18000b854:	xor    %dl,0x69(%rsi)
-   18000b857:	gs ja  0x18000b8bb
-   18000b85a:	(bad)
-   18000b85b:	insb   (%dx),%es:(%rdi)
-   18000b85c:	gs jae 0x18000b8b0
-   18000b85f:	rex.RB
-   18000b860:	rex.WRB push %r8
-   18000b862:	jb     0x18000b8d3
-   18000b864:	js     0x18000b8df
-   18000b866:	imul   $0x40797261,0x72(%rdx),%r12
-   18000b86e:	outsl  %gs:(%esi),(%dx)
-   18000b871:	fs gs rex
-   18000b874:	rex push %rcx
-   18000b876:	rex.RB
-   18000b877:	rex.B
-   18000b878:	rex.B
-   18000b879:	rex pop %rax
-   18000b87b:	pop    %rdx
-   18000b87c:	add    %bh,(%rdi)
-   18000b87e:	(bad)
-   18000b87f:	xor    %edx,0x69(%rsi)
-   18000b882:	gs ja  0x18000b8e6
-   18000b885:	(bad)
-   18000b886:	insb   (%dx),%es:(%rdi)
-   18000b887:	gs jae 0x18000b8db
-   18000b88a:	rex.RB
-   18000b88b:	rex.WRB push %r8
-   18000b88d:	jb     0x18000b8fe
-   18000b88f:	js     0x18000b90a
-   18000b891:	imul   $0x40797261,0x72(%rdx),%r12
-   18000b899:	outsl  %gs:(%esi),(%dx)
-   18000b89c:	fs gs rex
-   18000b89f:	rex push %rbp
-   18000b8a1:	rex.RB
-   18000b8a2:	rex.B
-   18000b8a3:	rex.B
-   18000b8a4:	rex pop %rax
-   18000b8a6:	pop    %rdx
-   18000b8a7:	add    %bh,(%rdi)
-   18000b8a9:	(bad)
-   18000b8aa:	pop    %rdi
-   18000b8ab:	(bad)
-   18000b8ac:	push   %rsi
-   18000b8ad:	imul   $0x656c6261,0x77(%rbp),%esp
-   18000b8b4:	jae    0x18000b907
-   18000b8b6:	rex.RB
-   18000b8b7:	rex.WRB push %r8
-   18000b8b9:	jb     0x18000b92a
+   18000b824:	shlb   $0x0,-0x49180000(%rsi)
+	...
+   18000b843:	add    %bh,%bh
+   18000b845:	(bad)
+   18000b846:	(bad)
+   18000b847:	incl   (%rax)
+   18000b849:	add    %al,(%rax)
+   18000b84b:	add    %ah,0x10000(%rax,%rdi,4)
+   18000b852:	add    %al,(%rax)
+   18000b854:	(bad)
+   18000b855:	add    %al,(%rax)
+   18000b857:	add    %al,(%rsi)
+   18000b859:	add    %al,(%rax)
+   18000b85b:	add    %ch,-0x48(%rax)
+   18000b85e:	add    %al,(%rax)
+   18000b860:	cmpb   $0x0,-0x47680000(%rax)
+   18000b867:	add    %dl,(%rax)
+   18000b869:	adc    %al,(%rax)
+   18000b86b:	add    %al,0x10(%rax)
+   18000b86e:	add    %al,(%rax)
+   18000b870:	lock xchg %eax,%esp
+   18000b872:	add    %al,(%rax)
+   18000b874:	loopne 0x18000b886
+   18000b876:	add    %al,(%rax)
+   18000b878:	lock adc %al,(%rax)
+   18000b87b:	add    %al,0x59(%rax)
+   18000b87e:	add    %al,(%rax)
+   18000b880:	ret    $0xb8
+   18000b883:	add    %ch,%ch
+   18000b885:	mov    $0xb9180000,%eax
+   18000b88a:	add    %al,(%rax)
+   18000b88c:	rex mov $0xb9770000,%ecx
+   18000b892:	add    %al,(%rax)
+   18000b894:	test   $0xb9,%eax
+   18000b899:	add    %al,(%rcx)
+   18000b89b:	add    %al,(%rdx)
+   18000b89d:	add    %al,(%rbx)
+   18000b89f:	add    %al,(%rax,%rax,1)
+   18000b8a2:	add    $0x6f654700,%eax
+   18000b8a7:	fs gs sub $0x77656956,%eax
+   18000b8ae:	(bad)
+   18000b8af:	(bad)
+   18000b8b0:	insb   (%dx),%es:(%rdi)
+   18000b8b1:	gs jae 0x18000b913
+   18000b8b4:	jno    0x18000b91b
+   18000b8b6:	insl   (%dx),%es:(%rdi)
+   18000b8b7:	pop    %rdi
+   18000b8b8:	jo     0x18000b92c
+   18000b8ba:	outsl  %ds:(%rsi),(%dx)
    18000b8bb:	js     0x18000b936
-   18000b8bd:	imul   $0x40797261,0x72(%rdx),%r12
-   18000b8c5:	outsl  %gs:(%esi),(%dx)
-   18000b8c8:	fs gs rex
-   18000b8cb:	rex
-   18000b8cc:	ss rex.X
-   18000b8ce:	add    %dil,(%rdi)
-   18000b8d1:	outsl  %fs:(%rsi),(%dx)
-   18000b8d3:	pop    %rdi
-   18000b8d4:	imul   $0x6c616974,0x69(%rsi),%ebp
-   18000b8db:	imul   $0x65695640,0x65(%rdx),%edi
-   18000b8e2:	ja     0x18000b945
-   18000b8e4:	(bad)
-   18000b8e5:	insb   (%dx),%es:(%rdi)
-   18000b8e6:	gs jae 0x18000b93a
-   18000b8e9:	rex.RB
-   18000b8ea:	rex.WRB push %r8
-   18000b8ec:	jb     0x18000b95d
-   18000b8ee:	js     0x18000b969
-   18000b8f0:	imul   $0x40797261,0x72(%rdx),%r12
-   18000b8f8:	outsl  %gs:(%esi),(%dx)
-   18000b8fb:	fs gs rex
-   18000b8fe:	rex
-   18000b8ff:	rex.RB
-   18000b900:	rex.RB
-   18000b901:	rex.B
-   18000b902:	pop    %r8
-   18000b904:	pop    %rax
-   18000b905:	pop    %rdx
-   18000b906:	add    %bh,(%rdi)
-   18000b908:	imul   $0x6c616974,0x69(%rsi),%ebp
-   18000b90f:	imul   $0x65695640,0x65(%rdx),%edi
-   18000b916:	ja     0x18000b979
-   18000b918:	(bad)
-   18000b919:	insb   (%dx),%es:(%rdi)
-   18000b91a:	gs jae 0x18000b96e
-   18000b91d:	rex.RB
-   18000b91e:	rex.WRB push %r8
-   18000b920:	jb     0x18000b991
-   18000b922:	js     0x18000b99d
-   18000b924:	imul   $0x40797261,0x72(%rdx),%r12
-   18000b92c:	outsl  %gs:(%esi),(%dx)
-   18000b92f:	fs gs rex
-   18000b932:	rex push %rbx
-   18000b934:	pop    %r8
-   18000b936:	pop    %rax
-   18000b937:	pop    %rdx
-   18000b938:	add    %bh,(%rdi)
-   18000b93a:	jae    0x18000b9a5
-   18000b93c:	insl   (%dx),%es:(%rdi)
-   18000b93d:	jo     0x18000b9ab
-   18000b93f:	imul   $0x6f656740,0x79(%rsi),%esp
-   18000b946:	fs gs rex
-   18000b949:	rex pop %rcx
-   18000b94b:	pop    %r15
-   18000b94d:	rex.WRX
-   18000b94e:	rex.B
-   18000b94f:	rex.RB
-   18000b950:	push   %r14
-   18000b952:	(bad)
-   18000b953:	and    $0x54,%al
-   18000b955:	jb     0x18000b9c0
-   18000b957:	(bad)
-   18000b958:	outsb  %ds:(%rsi),(%dx)
-   18000b959:	addr32 jne 0x18000b9c8
-   18000b95c:	(bad)
-   18000b95d:	je     0x18000b9c4
-   18000b95f:	fs push %rbx
-   18000b961:	jne    0x18000b9d5
-   18000b963:	data16 (bad)
-   18000b965:	movsxd 0x40(%rbp),%esp
-   18000b968:	and    $0x30,%al
-   18000b96a:	xor    0x31(%rax),%al
-   18000b96d:	rex
-   18000b96e:	rex pop %rdx
-   18000b970:	add    %al,(%rax)
-   18000b972:	add    %al,(%rax)
-   18000b974:	movabs 0xba,%al
-   18000b97d:	add    %al,(%rax)
-   18000b97f:	add    %al,0xc1(%rax)
-   18000b985:	nop
-   18000b986:	add    %al,(%rax)
-   18000b988:	loopne 0x18000b946
-	...
-   18000b992:	add    %al,(%rax)
-   18000b994:	test   %al,%dh
-   18000b996:	add    %al,(%rax)
-   18000b998:	rex xchg %eax,%edx
-   18000b99a:	add    %al,(%rax)
-   18000b99c:	enter  $0xbc,$0x0
-	...
-   18000b9a8:	(bad)
-   18000b9a9:	movl   $0x922800,(%rax)
-   18000b9af:	add    %bh,-0x44(%rax)
-	...
-   18000b9ba:	add    %al,(%rax)
-   18000b9bc:	rex.WR lretq $0x0
-   18000b9c0:	fcoms  -0x42200000(%rcx)
-	...
-   18000b9ce:	add    %al,(%rax)
-   18000b9d0:	dec    %dl
-   18000b9d2:	add    %al,(%rax)
-   18000b9d4:	rex xchg %eax,%ebx
-   18000b9d6:	add    %al,(%rax)
-   18000b9d8:	(bad)
-   18000b9d9:	mov    $0x0,%ebx
-   18000b9de:	add    %al,(%rax)
+   18000b8bd:	cs fs insb (%dx),%es:(%rdi)
+   18000b8c0:	insb   (%dx),%es:(%rdi)
+   18000b8c1:	add    %bh,(%rdi)
+   18000b8c3:	(bad)
+   18000b8c4:	xor    %dl,0x69(%rsi)
+   18000b8c7:	gs ja  0x18000b92b
+   18000b8ca:	(bad)
+   18000b8cb:	insb   (%dx),%es:(%rdi)
+   18000b8cc:	gs jae 0x18000b920
+   18000b8cf:	rex.RB
+   18000b8d0:	rex.WRB push %r8
+   18000b8d2:	jb     0x18000b943
+   18000b8d4:	js     0x18000b94f
+   18000b8d6:	imul   $0x40797261,0x72(%rdx),%r12
+   18000b8de:	outsl  %gs:(%esi),(%dx)
+   18000b8e1:	fs gs rex
+   18000b8e4:	rex push %rcx
+   18000b8e6:	rex.RB
+   18000b8e7:	rex.B
+   18000b8e8:	rex.B
+   18000b8e9:	rex pop %rax
+   18000b8eb:	pop    %rdx
+   18000b8ec:	add    %bh,(%rdi)
+   18000b8ee:	(bad)
+   18000b8ef:	xor    %edx,0x69(%rsi)
+   18000b8f2:	gs ja  0x18000b956
+   18000b8f5:	(bad)
+   18000b8f6:	insb   (%dx),%es:(%rdi)
+   18000b8f7:	gs jae 0x18000b94b
+   18000b8fa:	rex.RB
+   18000b8fb:	rex.WRB push %r8
+   18000b8fd:	jb     0x18000b96e
+   18000b8ff:	js     0x18000b97a
+   18000b901:	imul   $0x40797261,0x72(%rdx),%r12
+   18000b909:	outsl  %gs:(%esi),(%dx)
+   18000b90c:	fs gs rex
+   18000b90f:	rex push %rbp
+   18000b911:	rex.RB
+   18000b912:	rex.B
+   18000b913:	rex.B
+   18000b914:	rex pop %rax
+   18000b916:	pop    %rdx
+   18000b917:	add    %bh,(%rdi)
+   18000b919:	(bad)
+   18000b91a:	pop    %rdi
+   18000b91b:	(bad)
+   18000b91c:	push   %rsi
+   18000b91d:	imul   $0x656c6261,0x77(%rbp),%esp
+   18000b924:	jae    0x18000b977
+   18000b926:	rex.RB
+   18000b927:	rex.WRB push %r8
+   18000b929:	jb     0x18000b99a
+   18000b92b:	js     0x18000b9a6
+   18000b92d:	imul   $0x40797261,0x72(%rdx),%r12
+   18000b935:	outsl  %gs:(%esi),(%dx)
+   18000b938:	fs gs rex
+   18000b93b:	rex
+   18000b93c:	ss rex.X
+   18000b93e:	add    %dil,(%rdi)
+   18000b941:	outsl  %fs:(%rsi),(%dx)
+   18000b943:	pop    %rdi
+   18000b944:	imul   $0x6c616974,0x69(%rsi),%ebp
+   18000b94b:	imul   $0x65695640,0x65(%rdx),%edi
+   18000b952:	ja     0x18000b9b5
+   18000b954:	(bad)
+   18000b955:	insb   (%dx),%es:(%rdi)
+   18000b956:	gs jae 0x18000b9aa
+   18000b959:	rex.RB
+   18000b95a:	rex.WRB push %r8
+   18000b95c:	jb     0x18000b9cd
+   18000b95e:	js     0x18000b9d9
+   18000b960:	imul   $0x40797261,0x72(%rdx),%r12
+   18000b968:	outsl  %gs:(%esi),(%dx)
+   18000b96b:	fs gs rex
+   18000b96e:	rex
+   18000b96f:	rex.RB
+   18000b970:	rex.RB
+   18000b971:	rex.B
+   18000b972:	pop    %r8
+   18000b974:	pop    %rax
+   18000b975:	pop    %rdx
+   18000b976:	add    %bh,(%rdi)
+   18000b978:	imul   $0x6c616974,0x69(%rsi),%ebp
+   18000b97f:	imul   $0x65695640,0x65(%rdx),%edi
+   18000b986:	ja     0x18000b9e9
+   18000b988:	(bad)
+   18000b989:	insb   (%dx),%es:(%rdi)
+   18000b98a:	gs jae 0x18000b9de
+   18000b98d:	rex.RB
+   18000b98e:	rex.WRB push %r8
+   18000b990:	jb     0x18000ba01
+   18000b992:	js     0x18000ba0d
+   18000b994:	imul   $0x40797261,0x72(%rdx),%r12
+   18000b99c:	outsl  %gs:(%esi),(%dx)
+   18000b99f:	fs gs rex
+   18000b9a2:	rex push %rbx
+   18000b9a4:	pop    %r8
+   18000b9a6:	pop    %rax
+   18000b9a7:	pop    %rdx
+   18000b9a8:	add    %bh,(%rdi)
+   18000b9aa:	jae    0x18000ba15
+   18000b9ac:	insl   (%dx),%es:(%rdi)
+   18000b9ad:	jo     0x18000ba1b
+   18000b9af:	imul   $0x6f656740,0x79(%rsi),%esp
+   18000b9b6:	fs gs rex
+   18000b9b9:	rex pop %rcx
+   18000b9bb:	pop    %r15
+   18000b9bd:	rex.WRX
+   18000b9be:	rex.B
+   18000b9bf:	rex.RB
+   18000b9c0:	push   %r14
+   18000b9c2:	(bad)
+   18000b9c3:	and    $0x54,%al
+   18000b9c5:	jb     0x18000ba30
+   18000b9c7:	(bad)
+   18000b9c8:	outsb  %ds:(%rsi),(%dx)
+   18000b9c9:	addr32 jne 0x18000ba38
+   18000b9cc:	(bad)
+   18000b9cd:	je     0x18000ba34
+   18000b9cf:	fs push %rbx
+   18000b9d1:	jne    0x18000ba45
+   18000b9d3:	data16 (bad)
+   18000b9d5:	movsxd 0x40(%rbp),%esp
+   18000b9d8:	and    $0x30,%al
+   18000b9da:	xor    0x31(%rax),%al
+   18000b9dd:	rex
+   18000b9de:	rex pop %rdx
    18000b9e0:	add    %al,(%rax)
    18000b9e2:	add    %al,(%rax)
-   18000b9e4:	xor    $0xd3,%al
-   18000b9e6:	add    %al,(%rax)
-   18000b9e8:	rclb   $0x0,-0x42300000(%rax)
-	...
-   18000b9f7:	add    %ah,-0x2c(%rsi)
-   18000b9fa:	add    %al,(%rax)
-   18000b9fc:	xor    %dl,-0x42a00000(%rbx)
-	...
+   18000b9e4:	adc    %bh,0x0(%rbx)
+   18000b9ea:	add    %al,(%rax)
+   18000b9ec:	add    %al,(%rax)
+   18000b9ee:	add    %al,(%rax)
+   18000b9f0:	lock roll $0x0,(%rax)
+   18000b9f4:	add    %dl,-0x42b00000(%rax)
+	...
+   18000ba02:	add    %al,(%rax)
+   18000ba04:	hlt
+   18000ba05:	movb   $0x0,(%rax)
+   18000ba08:	rex xchg %eax,%edx
    18000ba0a:	add    %al,(%rax)
-   18000ba0c:	jp     0x18000b9e2
-   18000ba0e:	add    %al,(%rax)
-   18000ba10:	rclb   $0x0,-0x41c00000(%rdx)
-	...
-   18000ba1f:	add    %bl,-0x2a(%rdx)
-   18000ba22:	add    %al,(%rax)
-   18000ba24:	movabs 0xbea8000093,%al
-   18000ba2d:	add    %al,(%rax)
-   18000ba2f:	add    %al,(%rax)
-   18000ba31:	add    %al,(%rax)
-   18000ba33:	add    %bh,0x0(%rsi,%rdx,8)
-   18000ba37:	add    %cl,(%rax)
-   18000ba39:	xchg   %eax,%esp
+   18000ba0c:	cmp    %bh,0x0(%rbp)
+   18000ba12:	add    %al,(%rax)
+   18000ba14:	add    %al,(%rax)
+   18000ba16:	add    %al,(%rax)
+   18000ba18:	xor    $0xc8,%al
+   18000ba1a:	add    %al,(%rax)
+   18000ba1c:	sub    %dl,-0x43180000(%rdx)
+	...
+   18000ba2a:	add    %al,(%rax)
+   18000ba2c:	mov    $0xd80000ca,%esp
+   18000ba31:	xchg   %eax,%ecx
+   18000ba32:	add    %al,(%rax)
+   18000ba34:	push   %rax
+   18000ba35:	mov    $0x0,%esi
    18000ba3a:	add    %al,(%rax)
-   18000ba3c:	clc
-   18000ba3d:	mov    $0x0,%ebp
+   18000ba3c:	add    %al,(%rax)
+   18000ba3e:	add    %al,(%rax)
+   18000ba40:	outsb  %ds:(%rsi),(%dx)
+   18000ba41:	lret
    18000ba42:	add    %al,(%rax)
-   18000ba44:	add    %al,(%rax)
+   18000ba44:	rex xchg %eax,%ebx
    18000ba46:	add    %al,(%rax)
-   18000ba48:	pushf
-   18000ba49:	(bad)
-   18000ba4a:	add    %al,(%rax)
-   18000ba4c:	pop    %rax
-   18000ba4d:	xchg   %eax,%ebx
+   18000ba48:	sarb   0x0(%rbx)
    18000ba4e:	add    %al,(%rax)
-   18000ba50:	xor    %bh,0x0(%rsi)
-   18000ba56:	add    %al,(%rax)
-   18000ba58:	add    %al,(%rax)
+   18000ba50:	add    %al,(%rax)
+   18000ba52:	add    %al,(%rax)
+   18000ba54:	movsb  %ds:(%rsi),%es:(%rdi)
+   18000ba55:	roll   %cl,(%rax)
+   18000ba57:	add    %al,%al
+   18000ba59:	nop
    18000ba5a:	add    %al,(%rax)
-   18000ba5c:	ret    $0xd6
-   18000ba5f:	add    %dl,0x10000093(%rax)
-   18000ba65:	mov    $0x0,%esi
+   18000ba5c:	rex mov $0x0,%esi
+   18000ba62:	add    %al,(%rax)
+   18000ba64:	add    %al,(%rax)
+   18000ba66:	add    %al,(%rax)
+   18000ba68:	(bad)
+   18000ba69:	(bad)
    18000ba6a:	add    %al,(%rax)
-   18000ba6c:	add    %al,(%rax)
-   18000ba6e:	add    %al,(%rax)
-   18000ba70:	loop   0x18000ba48
-   18000ba72:	add    %al,(%rax)
-   18000ba74:	jo     0x18000ba09
-   18000ba76:	add    %al,(%rax)
-   18000ba78:	loopne 0x18000ba34
-	...
-   18000ba82:	add    %al,(%rax)
-   18000ba84:	push   $0x400000d8
-   18000ba89:	nop
-	...
-   18000ba9e:	add    %al,(%rax)
-   18000baa0:	movabs $0xbfbe000000000000,%rdi
-   18000baaa:	add    %al,(%rax)
-   18000baac:	add    %al,(%rax)
-   18000baae:	add    %al,(%rax)
-   18000bab0:	hlt
-   18000bab1:	mov    $0x0,%edi
-   18000bab6:	add    %al,(%rax)
-   18000bab8:	cmp    %al,%al
+   18000ba6c:	xor    %dl,-0x42300000(%rbx)
+	...
+   18000ba7a:	add    %al,(%rax)
+   18000ba7c:	(bad)
+   18000ba7d:	(bad)
+   18000ba7e:	add    %al,(%rax)
+   18000ba80:	rclb   $0x0,-0x41500000(%rdx)
+	...
+   18000ba8f:	add    %cl,%dl
+   18000ba91:	(bad)
+   18000ba92:	add    %al,(%rax)
+   18000ba94:	movabs 0xbf18000093,%al
+   18000ba9d:	add    %al,(%rax)
+   18000ba9f:	add    %al,(%rax)
+   18000baa1:	add    %al,(%rax)
+   18000baa3:	add    %ch,%ah
+   18000baa5:	(bad)
+   18000baa6:	add    %al,(%rax)
+   18000baa8:	or     %dl,0xbe6800(%rax,%rax,1)
+	...
+   18000bab7:	add    %cl,(%rdi,%rdx,8)
    18000baba:	add    %al,(%rax)
-   18000babc:	add    %al,(%rax)
+   18000babc:	pop    %rax
+   18000babd:	xchg   %eax,%ebx
    18000babe:	add    %al,(%rax)
-   18000bac0:	cmpsb  %es:(%rdi),%ds:(%rsi)
-   18000bac1:	rolb   $0x0,(%rax)
-   18000bac4:	add    %al,(%rax)
-   18000bac6:	add    %al,(%rax)
-   18000bac8:	(bad)
-   18000bac9:	roll   $0x0,(%rax)
-   18000bacc:	add    %al,(%rax)
+   18000bac0:	movabs 0xbe,%al
+   18000bac9:	add    %al,(%rax)
+   18000bacb:	add    %dh,(%rdx)
+   18000bacd:	xlat   %ds:(%rbx)
    18000bace:	add    %al,(%rax)
-   18000bad0:	adc    %bh,0x0(%rdi)
+   18000bad0:	nop
+   18000bad1:	xchg   %eax,%ebx
+   18000bad2:	add    %al,(%rax)
+   18000bad4:	cmpb   $0x0,0x0(%rsi)
+   18000badb:	add    %al,(%rax)
+   18000badd:	add    %al,(%rax)
+   18000badf:	add    %dl,-0x29(%rdx)
+   18000bae2:	add    %al,(%rax)
+   18000bae4:	jo     0x18000ba79
+   18000bae6:	add    %al,(%rax)
+   18000bae8:	push   %rax
+   18000bae9:	mov    $0x0,%ebx
+   18000baee:	add    %al,(%rax)
+   18000baf0:	add    %al,(%rax)
+   18000baf2:	add    %al,(%rax)
+   18000baf4:	fcomp  %st(0)
+   18000baf6:	add    %al,(%rax)
+   18000baf8:	rex nop
 	...
-   18000bade:	add    %al,(%rax)
-   18000bae0:	push   %rsp
-   18000bae1:	fadds  (%rax)
-   18000bae3:	add    %al,(%rax)
-   18000bae5:	add    %al,(%rax)
-   18000bae7:	add    %bh,(%rax)
-   18000bae9:	fadds  (%rax)
-   18000baeb:	add    %al,(%rax)
-   18000baed:	add    %al,(%rax)
-   18000baef:	add    %bl,(%rsi)
-   18000baf1:	fadds  (%rax)
-   18000baf3:	add    %al,(%rax)
-   18000baf5:	add    %al,(%rax)
-   18000baf7:	add    %cl,(%rax)
-   18000baf9:	fadds  (%rax)
-   18000bafb:	add    %al,(%rax)
-   18000bafd:	add    %al,(%rax)
-   18000baff:	add    %dh,%dl
-   18000bb01:	xlat   %ds:(%rbx)
-   18000bb02:	add    %al,(%rax)
-   18000bb04:	add    %al,(%rax)
-   18000bb06:	add    %al,(%rax)
-   18000bb08:	fcom   %st(7)
-   18000bb0a:	add    %al,(%rax)
-   18000bb0c:	add    %al,(%rax)
    18000bb0e:	add    %al,(%rax)
-   18000bb10:	mov    $0xd7,%esp
+   18000bb10:	mov    $0xbf,%eax
    18000bb15:	add    %al,(%rax)
-   18000bb17:	add    %ch,0xd7(%rax)
-   18000bb1d:	add    %al,(%rax)
-   18000bb1f:	add    %dl,0x0(%rdi,%rdx,8)
+   18000bb17:	add    %ch,(%rsi)
+   18000bb19:	rolb   $0x0,(%rax)
+   18000bb1c:	add    %al,(%rax)
+   18000bb1e:	add    %al,(%rax)
+   18000bb20:	rolb   $0x0,%fs:(%rax)
+   18000bb24:	add    %al,(%rax)
    18000bb26:	add    %al,(%rax)
-   18000bb28:	jbe    0x18000bb01
-   18000bb2a:	add    %al,(%rax)
+   18000bb28:	stos   %al,%es:(%rdi)
+   18000bb29:	rolb   $0x0,(%rax)
    18000bb2c:	add    %al,(%rax)
    18000bb2e:	add    %al,(%rax)
-   18000bb30:	pop    %rdx
-   18000bb31:	xlat   %ds:(%rbx)
-   18000bb32:	add    %al,(%rax)
+   18000bb30:	(bad)
+   18000bb31:	roll   $0x0,(%rax)
    18000bb34:	add    %al,(%rax)
    18000bb36:	add    %al,(%rax)
-   18000bb38:	rex.RX xlat %ds:(%rbx)
+   18000bb38:	mov    %ecx,%es
    18000bb3a:	add    %al,(%rax)
    18000bb3c:	add    %al,(%rax)
    18000bb3e:	add    %al,(%rax)
-   18000bb40:	sub    $0xd7,%al
-   18000bb42:	add    %al,(%rax)
-   18000bb44:	add    %al,(%rax)
-   18000bb46:	add    %al,(%rax)
-   18000bb48:	sbb    %dl,%bh
-   18000bb4a:	add    %al,(%rax)
-   18000bb4c:	add    %al,(%rax)
-   18000bb4e:	add    %al,(%rax)
-   18000bb50:	add    %bh,%dl
-	...
-   18000bb5e:	add    %al,(%rax)
-   18000bb60:	xchg   %eax,%esp
-   18000bb61:	rolb   %cl,(%rax)
-   18000bb63:	add    %al,(%rax)
+   18000bb40:	cmpb   $0x0,0x0(%rdi)
+	...
+   18000bb4f:	add    %al,%ah
+   18000bb51:	fadds  (%rax)
+   18000bb53:	add    %al,(%rax)
+   18000bb55:	add    %al,(%rax)
+   18000bb57:	add    %ch,0xd8(%rax)
+   18000bb5d:	add    %al,(%rax)
+   18000bb5f:	add    %cl,0xd8(%rsi)
    18000bb65:	add    %al,(%rax)
-   18000bb67:	add    %bl,-0x2e(%rax)
+   18000bb67:	add    %bh,-0x28(%rax)
    18000bb6a:	add    %al,(%rax)
    18000bb6c:	add    %al,(%rax)
    18000bb6e:	add    %al,(%rax)
-   18000bb70:	in     (%dx),%al
-   18000bb71:	roll   (%rax)
+   18000bb70:	(bad)
+   18000bb71:	fadds  (%rax)
    18000bb73:	add    %al,(%rax)
    18000bb75:	add    %al,(%rax)
-   18000bb77:	add    %ch,0xd1(%rax)
-   18000bb7d:	add    %al,(%rax)
-   18000bb7f:	add    %ah,-0x2f(%rsi)
+   18000bb77:	add    %cl,-0x28(%rax)
+   18000bb7a:	add    %al,(%rax)
+   18000bb7c:	add    %al,(%rax)
+   18000bb7e:	add    %al,(%rax)
+   18000bb80:	sub    $0xd8,%al
    18000bb82:	add    %al,(%rax)
    18000bb84:	add    %al,(%rax)
    18000bb86:	add    %al,(%rax)
-   18000bb88:	and    $0xd1,%al
+   18000bb88:	sbb    %bl,%al
    18000bb8a:	add    %al,(%rax)
    18000bb8c:	add    %al,(%rax)
    18000bb8e:	add    %al,(%rax)
-   18000bb90:	out    %al,$0xd0
+   18000bb90:	add    $0xd8,%al
    18000bb92:	add    %al,(%rax)
    18000bb94:	add    %al,(%rax)
    18000bb96:	add    %al,(%rax)
-   18000bb98:	mov    $0xd0,%al
+   18000bb98:	out    %al,$0xd7
    18000bb9a:	add    %al,(%rax)
    18000bb9c:	add    %al,(%rax)
    18000bb9e:	add    %al,(%rax)
-   18000bba0:	jo     0x18000bb72
-   18000bba2:	add    %al,(%rax)
-   18000bba4:	add    %al,(%rax)
-   18000bba6:	add    %al,(%rax)
-   18000bba8:	xor    %al,%dl
-   18000bbaa:	add    %al,(%rax)
-   18000bbac:	add    %al,(%rax)
-   18000bbae:	add    %al,(%rax)
-   18000bbb0:	cld
-   18000bbb1:	iret
-   18000bbb2:	add    %al,(%rax)
-   18000bbb4:	add    %al,(%rax)
+   18000bba0:	lret   $0xd7
+   18000bba3:	add    %al,(%rax)
+   18000bba5:	add    %al,(%rax)
+   18000bba7:	add    %dh,0xd7(%rsi)
+   18000bbad:	add    %al,(%rax)
+   18000bbaf:	add    %bl,0x0(%rdi,%rdx,8)
    18000bbb6:	add    %al,(%rax)
-   18000bbb8:	mov    $0xcf,%ah
+   18000bbb8:	mov    %dl,%bh
    18000bbba:	add    %al,(%rax)
    18000bbbc:	add    %al,(%rax)
    18000bbbe:	add    %al,(%rax)
-   18000bbc0:	insb   (%dx),%es:(%rdi)
-   18000bbc1:	iret
-   18000bbc2:	add    %al,(%rax)
-   18000bbc4:	add    %al,(%rax)
-   18000bbc6:	add    %al,(%rax)
-   18000bbc8:	sbb    $0xcf,%al
-   18000bbca:	add    %al,(%rax)
-   18000bbcc:	add    %al,(%rax)
+   18000bbc0:	jb     0x18000bb99
+	...
    18000bbce:	add    %al,(%rax)
-   18000bbd0:	add    %bl,%dl
+   18000bbd0:	add    $0xd3,%al
    18000bbd2:	add    %al,(%rax)
    18000bbd4:	add    %al,(%rax)
    18000bbd6:	add    %al,(%rax)
-   18000bbd8:	mov    $0xd2,%esp
-   18000bbdd:	add    %al,(%rax)
-   18000bbdf:	add    %dl,(%rax)
-   18000bbe1:	lret
-   18000bbe2:	add    %al,(%rax)
-   18000bbe4:	add    %al,(%rax)
-   18000bbe6:	add    %al,(%rax)
-   18000bbe8:	sub    $0xcb,%al
-   18000bbea:	add    %al,(%rax)
-   18000bbec:	add    %al,(%rax)
-   18000bbee:	add    %al,(%rax)
-   18000bbf0:	rex.RX lret
-   18000bbf2:	add    %al,(%rax)
-   18000bbf4:	add    %al,(%rax)
-   18000bbf6:	add    %al,(%rax)
-   18000bbf8:	push   $0xcb
-   18000bbfd:	add    %al,(%rax)
-   18000bbff:	add    %cl,0xcb(%rdx)
+   18000bbd8:	enter  $0xd2,$0x0
+   18000bbdc:	add    %al,(%rax)
+   18000bbde:	add    %al,(%rax)
+   18000bbe0:	pop    %rsp
+   18000bbe1:	rolb   %cl,(%rax)
+   18000bbe3:	add    %al,(%rax)
+   18000bbe5:	add    %al,(%rax)
+   18000bbe7:	add    %bl,(%rax)
+   18000bbe9:	rolb   %cl,(%rax)
+   18000bbeb:	add    %al,(%rax)
+   18000bbed:	add    %al,(%rax)
+   18000bbef:	add    %dl,%dh
+   18000bbf1:	roll   (%rax)
+   18000bbf3:	add    %al,(%rax)
+   18000bbf5:	add    %al,(%rax)
+   18000bbf7:	add    %dl,0x0(%rcx,%rdx,8)
+   18000bbfe:	add    %al,(%rax)
+   18000bc00:	push   %rsi
+   18000bc01:	roll   (%rax)
+   18000bc03:	add    %al,(%rax)
    18000bc05:	add    %al,(%rax)
-   18000bc07:	add    %ch,0xcb(%rax)
+   18000bc07:	add    %ah,(%rax)
+   18000bc09:	roll   (%rax)
+   18000bc0b:	add    %al,(%rax)
    18000bc0d:	add    %al,(%rax)
-   18000bc0f:	add    %bl,%ah
-   18000bc11:	lret
-   18000bc12:	add    %al,(%rax)
-   18000bc14:	add    %al,(%rax)
-   18000bc16:	add    %al,(%rax)
-   18000bc18:	or     %cl,%ah
-   18000bc1a:	add    %al,(%rax)
-   18000bc1c:	add    %al,(%rax)
-   18000bc1e:	add    %al,(%rax)
-   18000bc20:	pop    %rsp
-   18000bc21:	int3
-   18000bc22:	add    %al,(%rax)
-   18000bc24:	add    %al,(%rax)
-   18000bc26:	add    %al,(%rax)
-   18000bc28:	mov    $0xcc,%al
+   18000bc0f:	add    %ah,%al
+   18000bc11:	rolb   (%rax)
+   18000bc13:	add    %al,(%rax)
+   18000bc15:	add    %al,(%rax)
+   18000bc17:	add    %ah,0xd0(%rdx)
+   18000bc1d:	add    %al,(%rax)
+   18000bc1f:	add    %ch,0x0(%rax,%rdx,8)
+   18000bc23:	add    %al,(%rax)
+   18000bc25:	add    %al,(%rax)
+   18000bc27:	add    %ah,(%rax,%rdx,8)
    18000bc2a:	add    %al,(%rax)
    18000bc2c:	add    %al,(%rax)
    18000bc2e:	add    %al,(%rax)
-   18000bc30:	cld
-   18000bc31:	int3
+   18000bc30:	fmul   %st,%st(7)
    18000bc32:	add    %al,(%rax)
    18000bc34:	add    %al,(%rax)
    18000bc36:	add    %al,(%rax)
-   18000bc38:	rex.WX int $0x0
-   18000bc3b:	add    %al,(%rax)
-   18000bc3d:	add    %al,(%rax)
-   18000bc3f:	add    %al,0xcd(%rsi)
-   18000bc45:	add    %al,(%rax)
-   18000bc47:	add    %al,%dl
-   18000bc49:	int    $0x0
-   18000bc4b:	add    %al,(%rax)
-   18000bc4d:	add    %al,(%rax)
-   18000bc4f:	add    %cl,(%rsi)
-   18000bc51:	(bad)
-   18000bc52:	add    %al,(%rax)
-   18000bc54:	add    %al,(%rax)
-   18000bc56:	add    %al,(%rax)
-   18000bc58:	push   %rax
-   18000bc59:	(bad)
-   18000bc5a:	add    %al,(%rax)
-   18000bc5c:	add    %al,(%rax)
+   18000bc38:	mov    %cs,%edi
+   18000bc3a:	add    %al,(%rax)
+   18000bc3c:	add    %al,(%rax)
+   18000bc3e:	add    %al,(%rax)
+   18000bc40:	jb     0x18000bc15
+   18000bc42:	add    %al,(%rax)
+   18000bc44:	add    %al,(%rax)
+   18000bc46:	add    %al,(%rax)
+   18000bc48:	sub    $0xd3,%al
+   18000bc4a:	add    %al,(%rax)
+   18000bc4c:	add    %al,(%rax)
+   18000bc4e:	add    %al,(%rax)
+   18000bc50:	or     $0x0,%bl
+   18000bc53:	add    %al,(%rax)
+   18000bc55:	add    %al,(%rax)
+   18000bc57:	add    %bl,0x0(%rbx,%rcx,8)
    18000bc5e:	add    %al,(%rax)
-   18000bc60:	cwtl
-   18000bc61:	(bad)
+   18000bc60:	mov    $0xcb,%dh
    18000bc62:	add    %al,(%rax)
    18000bc64:	add    %al,(%rax)
    18000bc66:	add    %al,(%rax)
-   18000bc68:	fmul   %st,%st(6)
-	...
+   18000bc68:	fmul   %st(3),%st
+   18000bc6a:	add    %al,(%rax)
+   18000bc6c:	add    %al,(%rax)
+   18000bc6e:	add    %al,(%rax)
+   18000bc70:	cli
+   18000bc71:	lret
+   18000bc72:	add    %al,(%rax)
+   18000bc74:	add    %al,(%rax)
    18000bc76:	add    %al,(%rax)
-   18000bc78:	fadd   %st,%st(7)
+   18000bc78:	sbb    %cl,%ah
    18000bc7a:	add    %al,(%rax)
    18000bc7c:	add    %al,(%rax)
    18000bc7e:	add    %al,(%rax)
-   18000bc80:	sbb    %al,%cl
+   18000bc80:	rex.WR int3
    18000bc82:	add    %al,(%rax)
    18000bc84:	add    %al,(%rax)
    18000bc86:	add    %al,(%rax)
-   18000bc88:	push   %rdx
-   18000bc89:	enter  $0x0,$0x0
-   18000bc8d:	add    %al,(%rax)
-   18000bc8f:	add    %bl,%al
-   18000bc91:	leave
+   18000bc88:	js     0x18000bc56
+   18000bc8a:	add    %al,(%rax)
+   18000bc8c:	add    %al,(%rax)
+   18000bc8e:	add    %al,(%rax)
+   18000bc90:	int3
+   18000bc91:	int3
    18000bc92:	add    %al,(%rax)
    18000bc94:	add    %al,(%rax)
    18000bc96:	add    %al,(%rax)
-   18000bc98:	(bad)
-   18000bc99:	leave
+   18000bc98:	and    %cl,%ch
    18000bc9a:	add    %al,(%rax)
    18000bc9c:	add    %al,(%rax)
    18000bc9e:	add    %al,(%rax)
-   18000bca0:	sbb    %cl,%cl
-   18000bca2:	add    %al,(%rax)
-   18000bca4:	add    %al,(%rax)
-   18000bca6:	add    %al,(%rax)
-   18000bca8:	mov    $0xc8,%eax
+   18000bca0:	insb   (%dx),%es:(%rdi)
+   18000bca1:	int    $0x0
+   18000bca3:	add    %al,(%rax)
+   18000bca5:	add    %al,(%rax)
+   18000bca7:	add    %bh,0xcd(%rdx)
    18000bcad:	add    %al,(%rax)
-   18000bcaf:	add    %cl,0xc8(%rdx)
+   18000bcaf:	add    %dh,%dh
+   18000bcb1:	int    $0x0
+   18000bcb3:	add    %al,(%rax)
    18000bcb5:	add    %al,(%rax)
-   18000bcb7:	add    %ch,-0x38(%rsi)
-	...
+   18000bcb7:	add    %dh,(%rdx)
+   18000bcb9:	(bad)
+   18000bcba:	add    %al,(%rax)
+   18000bcbc:	add    %al,(%rax)
+   18000bcbe:	add    %al,(%rax)
+   18000bcc0:	jle    0x18000bc90
+   18000bcc2:	add    %al,(%rax)
+   18000bcc4:	add    %al,(%rax)
    18000bcc6:	add    %al,(%rax)
-   18000bcc8:	xor    %bh,%al
-   18000bcca:	add    %al,(%rax)
-   18000bccc:	add    %al,(%rax)
-   18000bcce:	add    %al,(%rax)
-   18000bcd0:	cwtl
-   18000bcd1:	movb   $0x0,(%rax)
-	...
-   18000bce0:	movabs %al,0x4e000000000000c5
-   18000bce9:	(bad)
-   18000bcea:	add    %al,(%rax)
-   18000bcec:	add    %al,(%rax)
-   18000bcee:	add    %al,(%rax)
-   18000bcf0:	cmp    %dh,%al
-   18000bcf2:	add    %al,(%rax)
-   18000bcf4:	add    %al,(%rax)
-   18000bcf6:	add    %al,(%rax)
-   18000bcf8:	(bad)
-   18000bcfc:	add    %al,(%rax)
-   18000bcfe:	add    %al,(%rax)
-   18000bd00:	mov    $0xc3,%dh
+   18000bcc8:	ror    $0x0,%dh
+   18000bccb:	add    %al,(%rax)
+   18000bccd:	add    %al,(%rax)
+   18000bccf:	add    %cl,(%rax)
+   18000bcd1:	iret
+   18000bcd2:	add    %al,(%rax)
+   18000bcd4:	add    %al,(%rax)
+   18000bcd6:	add    %al,(%rax)
+   18000bcd8:	rex.WR iretq
+	...
+   18000bce6:	add    %al,(%rax)
+   18000bce8:	rex.WR enter $0x0,$0x0
+   18000bced:	add    %al,(%rax)
+   18000bcef:	add    %cl,0xc8(%rdx)
+   18000bcf5:	add    %al,(%rax)
+   18000bcf7:	add    %al,%dl
+   18000bcf9:	enter  $0x0,$0x0
+   18000bcfd:	add    %al,(%rax)
+   18000bcff:	add    %cl,-0x36(%rax)
    18000bd02:	add    %al,(%rax)
    18000bd04:	add    %al,(%rax)
    18000bd06:	add    %al,(%rax)
-   18000bd08:	jo     0x18000bccd
+   18000bd08:	ror    %cl,%cl
    18000bd0a:	add    %al,(%rax)
    18000bd0c:	add    %al,(%rax)
    18000bd0e:	add    %al,(%rax)
-   18000bd10:	rex ret
+   18000bd10:	mov    %cl,%cl
    18000bd12:	add    %al,(%rax)
    18000bd14:	add    %al,(%rax)
    18000bd16:	add    %al,(%rax)
-   18000bd18:	out    %al,(%dx)
-   18000bd19:	ret    $0x0
+   18000bd18:	sub    %cl,%cl
+   18000bd1a:	add    %al,(%rax)
    18000bd1c:	add    %al,(%rax)
    18000bd1e:	add    %al,(%rax)
-   18000bd20:	(bad)
-   18000bd21:	ret    $0x0
-   18000bd24:	add    %al,(%rax)
-   18000bd26:	add    %al,(%rax)
-   18000bd28:	lret   $0xc1
-   18000bd2b:	add    %al,(%rax)
-   18000bd2d:	add    %al,(%rax)
-   18000bd2f:	add    %ah,0xc1(%rdx)
+   18000bd20:	cli
+   18000bd21:	enter  $0x0,$0x0
+   18000bd25:	add    %al,(%rax)
+   18000bd27:	add    %bl,%dh
+   18000bd29:	enter  $0x0,$0x0
+	...
    18000bd35:	add    %al,(%rax)
-   18000bd37:	add    %dh,0xc4(%rdx)
+   18000bd37:	add    %ah,0xc7(%rdx)
    18000bd3d:	add    %al,(%rax)
-   18000bd3f:	add    %cl,(%rsi,%rax,8)
-   18000bd42:	add    %al,(%rax)
-   18000bd44:	add    %al,(%rax)
-   18000bd46:	add    %al,(%rax)
-   18000bd48:	hlt
-   18000bd49:	(bad)
-   18000bd4a:	add    %al,(%rax)
-   18000bd4c:	add    %al,(%rax)
-   18000bd4e:	add    %al,(%rax)
-   18000bd50:	add    $0x0,%ah
-	...
-   18000bd5f:	add    %ch,(%rsi)
-   18000bd61:	(bad)
-   18000bd62:	add    %al,(%rax)
-   18000bd64:	add    %al,(%rax)
-   18000bd66:	add    %al,(%rax)
-   18000bd68:	rex.RX (bad)
-   18000bd6a:	add    %al,(%rax)
-   18000bd6c:	add    %al,(%rax)
-   18000bd6e:	add    %al,(%rax)
-   18000bd70:	lock roll %cl,(%rax)
-   18000bd73:	add    %al,(%rax)
-   18000bd75:	add    %al,(%rax)
-   18000bd77:	add    %bl,%ah
-   18000bd79:	roll   %cl,(%rax)
-   18000bd7b:	add    %al,(%rax)
-   18000bd7d:	add    %al,(%rax)
-   18000bd7f:	add    %al,%dh
-   18000bd81:	roll   %cl,(%rax)
-   18000bd83:	add    %al,(%rax)
-   18000bd85:	add    %al,(%rax)
-   18000bd87:	add    %ch,0xd3(%rsi)
-   18000bd8d:	add    %al,(%rax)
-   18000bd8f:	add    %dl,0x0(%rbx,%rdx,8)
+   18000bd3f:	add    %cl,(%rax)
+   18000bd41:	movl   $0x0,(%rax)
+	...
+   18000bd4f:	add    %dl,(%rdx)
+   18000bd51:	movb   $0x0,(%rax)
+   18000bd54:	add    %al,(%rax)
+   18000bd56:	add    %al,(%rax)
+   18000bd58:	mov    $0xc4,%esi
+   18000bd5d:	add    %al,(%rax)
+   18000bd5f:	add    %ch,0xc6(%rdx)
+   18000bd65:	add    %al,(%rax)
+   18000bd67:	add    %ch,0xc5(%rsi)
+   18000bd6d:	add    %al,(%rax)
+   18000bd6f:	add    %ah,(%rsi)
+   18000bd71:	(bad)
+   18000bd72:	add    %al,(%rax)
+   18000bd74:	add    %al,(%rax)
+   18000bd76:	add    %al,(%rax)
+   18000bd78:	loopne 0x18000bd3d
+   18000bd7a:	add    %al,(%rax)
+   18000bd7c:	add    %al,(%rax)
+   18000bd7e:	add    %al,(%rax)
+   18000bd80:	mov    $0xc3,%al
+   18000bd82:	add    %al,(%rax)
+   18000bd84:	add    %al,(%rax)
+   18000bd86:	add    %al,(%rax)
+   18000bd88:	pop    %rsi
+   18000bd89:	ret
+   18000bd8a:	add    %al,(%rax)
+   18000bd8c:	add    %al,(%rax)
+   18000bd8e:	add    %al,(%rax)
+   18000bd90:	xchg   %al,%dl
+   18000bd92:	add    %al,(%rax)
+   18000bd94:	add    %al,(%rax)
    18000bd96:	add    %al,(%rax)
-   18000bd98:	jl     0x18000bd6d
+   18000bd98:	cmp    %dl,%al
    18000bd9a:	add    %al,(%rax)
    18000bd9c:	add    %al,(%rax)
    18000bd9e:	add    %al,(%rax)
-   18000bda0:	push   $0xffffffffffffffd3
+   18000bda0:	adc    %dl,%al
    18000bda2:	add    %al,(%rax)
    18000bda4:	add    %al,(%rax)
    18000bda6:	add    %al,(%rax)
-   18000bda8:	pop    %rax
-   18000bda9:	roll   %cl,(%rax)
-   18000bdab:	add    %al,(%rax)
-   18000bdad:	add    %al,(%rax)
-   18000bdaf:	add    %dl,(%rax)
-   18000bdb1:	(bad)
+   18000bda8:	and    %ch,%al
+   18000bdaa:	add    %al,(%rax)
+   18000bdac:	add    %al,(%rax)
+   18000bdae:	add    %al,(%rax)
+   18000bdb0:	jl     0x18000bd78
    18000bdb2:	add    %al,(%rax)
    18000bdb4:	add    %al,(%rax)
    18000bdb6:	add    %al,(%rax)
-   18000bdb8:	cli
-   18000bdb9:	roll   %cl,(%rax)
-   18000bdbb:	add    %al,(%rax)
-   18000bdbd:	add    %al,(%rax)
-   18000bdbf:	add    %ah,%dh
-   18000bdc1:	roll   %cl,(%rax)
-	...
-   18000bdcf:	add    %al,-0x2d(%rdx)
-	...
+   18000bdb8:	(bad)
+   18000bdbc:	add    %al,(%rax)
+   18000bdbe:	add    %al,(%rax)
+   18000bdc0:	lock (bad)
+	...
+   18000bdce:	add    %al,(%rax)
+   18000bdd0:	sahf
+   18000bdd1:	(bad)
+   18000bdd2:	add    %al,(%rax)
+   18000bdd4:	add    %al,(%rax)
+   18000bdd6:	add    %al,(%rax)
+   18000bdd8:	mov    $0xd4,%dh
+   18000bdda:	add    %al,(%rax)
+   18000bddc:	add    %al,(%rax)
    18000bdde:	add    %al,(%rax)
-   18000bde0:	cwtl
-   18000bde1:	lret   $0x0
+   18000bde0:	(bad)
+   18000bde1:	(bad)
+   18000bde2:	add    %al,(%rax)
    18000bde4:	add    %al,(%rax)
    18000bde6:	add    %al,(%rax)
-   18000bde8:	(bad)
-   18000bde9:	lret   $0x0
-	...
-   18000bdf8:	cmp    %ch,%dl
+   18000bde8:	rex.WR (bad)
+   18000bdea:	add    %al,(%rax)
+   18000bdec:	add    %al,(%rax)
+   18000bdee:	add    %al,(%rax)
+   18000bdf0:	ss (bad)
+   18000bdf2:	add    %al,(%rax)
+   18000bdf4:	add    %al,(%rax)
+   18000bdf6:	add    %al,(%rax)
+   18000bdf8:	(bad)
+   18000bdf9:	(bad)
    18000bdfa:	add    %al,(%rax)
    18000bdfc:	add    %al,(%rax)
    18000bdfe:	add    %al,(%rax)
-   18000be00:	rex.W (bad)
-	...
-   18000be0e:	add    %al,(%rax)
-   18000be10:	insb   (%dx),%es:(%rdi)
-   18000be11:	(bad)
-   18000be12:	add    %al,(%rax)
-   18000be14:	add    %al,(%rax)
-   18000be16:	add    %al,(%rax)
-   18000be18:	js     0x18000bdef
-   18000be1a:	add    %al,(%rax)
-   18000be1c:	add    %al,(%rax)
-   18000be1e:	add    %al,(%rax)
-   18000be20:	push   %rdx
-   18000be21:	(bad)
-	...
+   18000be00:	add    $0xd4,%al
+   18000be02:	add    %al,(%rax)
+   18000be04:	add    %al,(%rax)
+   18000be06:	add    %al,(%rax)
+   18000be08:	in     (%dx),%al
+   18000be09:	roll   %cl,(%rax)
+   18000be0b:	add    %al,(%rax)
+   18000be0d:	add    %al,(%rax)
+   18000be0f:	add    %bl,%dl
+   18000be11:	roll   %cl,(%rax)
+   18000be13:	add    %al,(%rax)
+   18000be15:	add    %al,(%rax)
+   18000be17:	add    %cl,%al
+   18000be19:	roll   %cl,(%rax)
+   18000be1b:	add    %al,(%rax)
+   18000be1d:	add    %al,(%rax)
+   18000be1f:	add    %al,0xd4(%rax)
+   18000be25:	add    %al,(%rax)
+   18000be27:	add    %ch,-0x2c(%rdx)
+   18000be2a:	add    %al,(%rax)
+   18000be2c:	add    %al,(%rax)
    18000be2e:	add    %al,(%rax)
-   18000be30:	pop    %rax
+   18000be30:	push   %rsi
    18000be31:	(bad)
 	...
    18000be3e:	add    %al,(%rax)
-   18000be40:	cmp    %dh,%dl
-   18000be42:	add    %al,(%rax)
-   18000be44:	add    %al,(%rax)
-   18000be46:	add    %al,(%rax)
-   18000be48:	rex.W (bad)
-   18000be4a:	add    %al,(%rax)
-   18000be4c:	add    %al,(%rax)
+   18000be40:	mov    $0xd3,%dl
+	...
    18000be4e:	add    %al,(%rax)
-   18000be50:	(bad)
-   18000be51:	(bad)
+   18000be50:	or     %cl,%bl
    18000be52:	add    %al,(%rax)
    18000be54:	add    %al,(%rax)
    18000be56:	add    %al,(%rax)
-   18000be58:	mov    %ss,%esp
-   18000be5a:	add    %al,(%rax)
-   18000be5c:	add    %al,(%rax)
-   18000be5e:	add    %al,(%rax)
-   18000be60:	(bad)
-   18000be61:	(bad)
-   18000be62:	add    %al,(%rax)
-   18000be64:	add    %al,(%rax)
+   18000be58:	ror    %dl
+	...
    18000be66:	add    %al,(%rax)
-   18000be68:	scas   %es:(%rdi),%al
+   18000be68:	stos   %al,%es:(%rdi)
    18000be69:	(bad)
    18000be6a:	add    %al,(%rax)
    18000be6c:	add    %al,(%rax)
    18000be6e:	add    %al,(%rax)
-   18000be70:	and    %dh,%dl
-   18000be72:	add    %al,(%rax)
-   18000be74:	add    %al,(%rax)
-   18000be76:	add    %al,(%rax)
-   18000be78:	enter  $0xd5,$0x0
-   18000be7c:	add    %al,(%rax)
-   18000be7e:	add    %al,(%rax)
-   18000be80:	pushf
+   18000be70:	mov    $0xd5,%eax
+	...
+   18000be7d:	add    %al,(%rax)
+   18000be7f:	add    %bl,%ah
    18000be81:	(bad)
    18000be82:	add    %al,(%rax)
    18000be84:	add    %al,(%rax)
    18000be86:	add    %al,(%rax)
-   18000be88:	(bad)
-   18000be89:	(bad)
-   18000be8a:	add    %al,(%rax)
-   18000be8c:	add    %al,(%rax)
-   18000be8e:	add    %al,(%rax)
-   18000be90:	mov    %ebp,%ss
-   18000be92:	add    %al,(%rax)
-   18000be94:	add    %al,(%rax)
-   18000be96:	add    %al,(%rax)
-   18000be98:	(bad)
-   18000be99:	(bad)
-	...
-   18000bea6:	add    %al,(%rax)
-   18000bea8:	es (bad)
-   18000beaa:	add    %al,(%rax)
-   18000beac:	add    %al,(%rax)
-   18000beae:	add    %al,(%rax)
-   18000beb0:	sbb    $0xd5,%al
+   18000be88:	call   0x18000bf62
+   18000be8d:	add    %al,(%rax)
+   18000be8f:	add    %al,%dl
+   18000be91:	(bad)
+	...
+   18000be9e:	add    %al,(%rax)
+   18000bea0:	enter  $0xd5,$0x0
+	...
+   18000beb0:	stos   %al,%es:(%rdi)
+   18000beb1:	(bad)
    18000beb2:	add    %al,(%rax)
    18000beb4:	add    %al,(%rax)
    18000beb6:	add    %al,(%rax)
-   18000beb8:	adc    %dl,%ch
-   18000beba:	add    %al,(%rax)
-   18000bebc:	add    %al,(%rax)
-   18000bebe:	add    %al,(%rax)
-   18000bec0:	(bad)
-   18000bec1:	(bad)
+   18000beb8:	mov    $0xd6,%eax
+   18000bebd:	add    %al,(%rax)
+   18000bebf:	add    %dh,-0x2a(%rsi)
    18000bec2:	add    %al,(%rax)
    18000bec4:	add    %al,(%rax)
    18000bec6:	add    %al,(%rax)
-   18000bec8:	(bad)
+   18000bec8:	cld
    18000bec9:	(bad)
    18000beca:	add    %al,(%rax)
    18000becc:	add    %al,(%rax)
    18000bece:	add    %al,(%rax)
-   18000bed0:	xor    %dl,%ch
+   18000bed0:	repnz (bad)
    18000bed2:	add    %al,(%rax)
    18000bed4:	add    %al,(%rax)
    18000bed6:	add    %al,(%rax)
-   18000bed8:	in     (%dx),%al
+   18000bed8:	(bad)
    18000bed9:	(bad)
    18000beda:	add    %al,(%rax)
    18000bedc:	add    %al,(%rax)
    18000bede:	add    %al,(%rax)
-   18000bee0:	in     $0xd4,%al
+   18000bee0:	xchg   %eax,%edx
+   18000bee1:	(bad)
    18000bee2:	add    %al,(%rax)
    18000bee4:	add    %al,(%rax)
    18000bee6:	add    %al,(%rax)
-   18000bee8:	fcmovbe %st(4),%st
+   18000bee8:	cmp    %dl,%dh
    18000beea:	add    %al,(%rax)
    18000beec:	add    %al,(%rax)
    18000beee:	add    %al,(%rax)
-   18000bef0:	rcl    %ah
+   18000bef0:	or     $0xd6,%al
    18000bef2:	add    %al,(%rax)
    18000bef4:	add    %al,(%rax)
    18000bef6:	add    %al,(%rax)
-   18000bef8:	mov    $0xd4,%dl
+   18000bef8:	pop    %rdx
+   18000bef9:	(bad)
    18000befa:	add    %al,(%rax)
    18000befc:	add    %al,(%rax)
    18000befe:	add    %al,(%rax)
-   18000bf00:	not    %ah
-	...
-   18000bf0e:	add    %al,(%rax)
-   18000bf10:	cmp    $0x0,%al
-   18000bf12:	(bad)
-   18000bf13:	imul   $0x6c616974,0x69(%rsi),%ebp
-   18000bf1a:	imul   $0x6d6f4340,0x65(%rdx),%edi
-   18000bf21:	insl   (%dx),%es:(%rdi)
-   18000bf22:	outsl  %ds:(%rsi),(%dx)
-   18000bf23:	outsb  %ds:(%rsi),(%dx)
-   18000bf24:	rex.WRB outsl %ds:(%rsi),(%dx)
-   18000bf26:	imul   $0x75537265,%fs:0x69(%rsi),%esp
-   18000bf2e:	jb     0x18000bf96
-   18000bf30:	(bad)
-   18000bf31:	movsxd 0x4c(%rbp),%esp
-   18000bf34:	imul   $0x40797261,0x72(%rdx),%esp
-   18000bf3b:	outsl  %gs:(%esi),(%dx)
-   18000bf3e:	fs gs rex
-   18000bf41:	rex push %rbx
-   18000bf43:	pop    %r8
-   18000bf45:	pop    %rax
-   18000bf46:	pop    %rdx
-   18000bf47:	add    %ah,(%rdi)
-   18000bf49:	add    %bh,(%rdi)
-   18000bf4b:	(bad)
-   18000bf4c:	xor    %bh,(%rdi)
-   18000bf4e:	and    $0x54,%al
-   18000bf50:	jb     0x18000bfbb
-   18000bf52:	(bad)
-   18000bf53:	outsb  %ds:(%rsi),(%dx)
-   18000bf54:	addr32 jne 0x18000bfc3
-   18000bf57:	(bad)
-   18000bf58:	je     0x18000bfbf
-   18000bf5a:	fs push %rbx
-   18000bf5c:	jne    0x18000bfd0
-   18000bf5e:	data16 (bad)
-   18000bf60:	movsxd 0x4d(%rbp),%esp
-   18000bf63:	outsl  %ds:(%rsi),(%dx)
-   18000bf64:	imul   $0x24407265,%fs:0x69(%rsi),%esp
-   18000bf6c:	xor    %dh,(%rdx)
-   18000bf6e:	rex
-   18000bf6f:	outsl  %gs:(%esi),(%dx)
-   18000bf72:	fs gs rex
-   18000bf75:	rex push %rcx
-   18000bf77:	rex.RB
-   18000bf78:	rex.B
-   18000bf79:	rex.B
-   18000bf7a:	rex
-   18000bf7b:	rex.B
-   18000bf7c:	rex.RB
-   18000bf7d:	rex.X push %rsi
-   18000bf7f:	(bad)
-   18000bf80:	and    $0x53,%al
-   18000bf82:	jne    0x18000bff6
-   18000bf84:	data16 (bad)
-   18000bf86:	movsxd 0x4d(%rbp),%esp
-   18000bf89:	gs jae 0x18000bff4
-   18000bf8c:	rex and $0x30,%al
-   18000bf8f:	xor    0x31(%rax),%al
-   18000bf92:	rex
-   18000bf93:	rex.B
-   18000bf94:	rex.RB
-   18000bf95:	push   %r14
-   18000bf97:	(bad)
-   18000bf98:	and    $0x54,%al
-   18000bf9a:	jb     0x18000c005
-   18000bf9c:	(bad)
-   18000bf9d:	outsb  %ds:(%rsi),(%dx)
-   18000bf9e:	addr32 jne 0x18000c00d
-   18000bfa1:	(bad)
-   18000bfa2:	je     0x18000c009
-   18000bfa4:	fs push %rbx
-   18000bfa6:	jne    0x18000c01a
-   18000bfa8:	data16 (bad)
-   18000bfaa:	movsxd 0x42(%rbp),%esp
-   18000bfad:	jne    0x18000c018
-   18000bfaf:	insb   (%dx),%es:(%rdi)
-   18000bfb0:	fs gs jb 0x18000bff4
-   18000bfb4:	and    $0x30,%al
-   18000bfb6:	xor    0x31(%rax),%al
-   18000bfb9:	rex
-   18000bfba:	rex pop %rdx
-   18000bfbc:	add    %al,(%rax)
-   18000bfbe:	sub    $0x0,%al
-   18000bfc0:	(bad)
-   18000bfc1:	(bad)
-   18000bfc2:	xor    %edi,(%rdi)
-   18000bfc4:	and    $0x54,%al
-   18000bfc6:	jb     0x18000c031
-   18000bfc8:	(bad)
-   18000bfc9:	outsb  %ds:(%rsi),(%dx)
-   18000bfca:	addr32 jne 0x18000c039
-   18000bfcd:	(bad)
-   18000bfce:	je     0x18000c035
-   18000bfd0:	fs push %rbx
-   18000bfd2:	jne    0x18000c046
-   18000bfd4:	data16 (bad)
-   18000bfd6:	movsxd 0x4d(%rbp),%esp
-   18000bfd9:	outsl  %ds:(%rsi),(%dx)
-   18000bfda:	imul   $0x24407265,%fs:0x69(%rsi),%esp
-   18000bfe2:	xor    %dh,(%rdx)
-   18000bfe4:	rex
-   18000bfe5:	outsl  %gs:(%esi),(%dx)
-   18000bfe8:	fs gs rex
-   18000bfeb:	rex push %rcx
-   18000bfed:	rex.RB
-   18000bfee:	rex.B
-   18000bfef:	rex.B
-   18000bff0:	rex pop %rax
-   18000bff2:	pop    %rdx
-   18000bff3:	add    %al,0x3f(%rax,%rax,1)
-   18000bff7:	imul   $0x65676465,0x5f(%rbx),%esi
-   18000bffe:	pop    %rdi
-   18000bfff:	(bad)
-   18000c000:	movsxd 0x76(%rcx,%rbp,2),%esi
-   18000c004:	gs rex (bad)
-   18000c007:	and    $0x54,%al
-   18000c009:	jb     0x18000c074
-   18000c00b:	(bad)
-   18000c00c:	outsb  %ds:(%rsi),(%dx)
-   18000c00d:	addr32 jne 0x18000c07c
-   18000c010:	(bad)
-   18000c011:	je     0x18000c078
-   18000c013:	fs push %rbx
-   18000c015:	jne    0x18000c089
-   18000c017:	data16 (bad)
-   18000c019:	movsxd 0x4d(%rbp),%esp
-   18000c01c:	outsl  %ds:(%rsi),(%dx)
-   18000c01d:	imul   $0x24407265,%fs:0x69(%rsi),%esp
-   18000c025:	xor    %dh,(%rdx)
-   18000c027:	rex
-   18000c028:	outsl  %gs:(%esi),(%dx)
-   18000c02b:	fs gs rex
-   18000c02e:	rex push %rcx
-   18000c030:	rex.RB
-   18000c031:	rex.X
-   18000c032:	pop    %r15
-   18000c034:	rex.WRX
-   18000c035:	rex.WB
-   18000c036:	rex pop %rdx
-   18000c038:	add    %al,(%rax)
-   18000c03a:	cmp    %eax,(%rax)
-   18000c03c:	(bad)
-   18000c03d:	movsxd 0x6c(%rdi),%ebp
-   18000c040:	insb   (%dx),%es:(%rdi)
-   18000c041:	(bad)
-   18000c042:	jo     0x18000c0b7
-   18000c044:	gs pop %rdi
-   18000c046:	gs fs addr32 gs rex (bad)
-   18000c04c:	and    $0x54,%al
-   18000c04e:	jb     0x18000c0b9
-   18000c050:	(bad)
-   18000c051:	outsb  %ds:(%rsi),(%dx)
-   18000c052:	addr32 jne 0x18000c0c1
-   18000c055:	(bad)
-   18000c056:	je     0x18000c0bd
-   18000c058:	fs push %rbx
-   18000c05a:	jne    0x18000c0ce
-   18000c05c:	data16 (bad)
-   18000c05e:	movsxd 0x4d(%rbp),%esp
-   18000c061:	outsl  %ds:(%rsi),(%dx)
-   18000c062:	imul   $0x24407265,%fs:0x69(%rsi),%esp
-   18000c06a:	xor    %dh,(%rdx)
-   18000c06c:	rex
-   18000c06d:	outsl  %gs:(%esi),(%dx)
-   18000c070:	fs gs rex
-   18000c073:	rex push %rcx
-   18000c075:	rex.RB
-   18000c076:	rex.B
-   18000c077:	rex.B (bad)
-   18000c079:	push   %r13
-   18000c07b:	rex.XB outsl %ds:(%rsi),(%dx)
-   18000c07d:	insb   (%dx),%es:(%rdi)
-   18000c07e:	insb   (%dx),%es:(%rdi)
-   18000c07f:	(bad)
-   18000c080:	jo     0x18000c0f5
-   18000c082:	gs rex.RB
-   18000c084:	fs rex.WB outsb %gs:(%esi),(%dx)
-   18000c089:	outsw  %ds:(%rsi),(%dx)
-   18000c08b:	rex xor %esi,(%rdx)
-   18000c08e:	rex
-   18000c08f:	rex.WB
-   18000c090:	rex.B
-   18000c091:	rex.RB
-   18000c092:	rex.X push %rsi
-   18000c094:	(bad)
-   18000c095:	and    $0x50,%al
-   18000c097:	outsl  %ds:(%rsi),(%dx)
-   18000c098:	imul   $0x32302440,0x74(%rsi),%ebp
-   18000c09f:	rex xor 0x40(%rax),%al
-   18000c0a3:	pop    %rdx
-   18000c0a4:	add    %al,(%rax)
-   18000c0a6:	xor    %al,(%rax)
-   18000c0a8:	(bad)
-   18000c0a9:	movsxd 0x61(%rbp,%riz,2),%ebp
-   18000c0ad:	outsb  %ds:(%rsi),(%dx)
-   18000c0ae:	rex (bad)
-   18000c0b0:	and    $0x54,%al
-   18000c0b2:	jb     0x18000c11d
-   18000c0b4:	(bad)
-   18000c0b5:	outsb  %ds:(%rsi),(%dx)
-   18000c0b6:	addr32 jne 0x18000c125
-   18000c0b9:	(bad)
-   18000c0ba:	je     0x18000c121
-   18000c0bc:	fs push %rbx
-   18000c0be:	jne    0x18000c132
-   18000c0c0:	data16 (bad)
-   18000c0c2:	movsxd 0x4d(%rbp),%esp
-   18000c0c5:	outsl  %ds:(%rsi),(%dx)
-   18000c0c6:	imul   $0x24407265,%fs:0x69(%rsi),%esp
-   18000c0ce:	xor    %dh,(%rdx)
-   18000c0d0:	rex
-   18000c0d1:	outsl  %gs:(%esi),(%dx)
-   18000c0d4:	fs gs rex
-   18000c0d7:	rex push %rcx
-   18000c0d9:	rex.RB
-   18000c0da:	rex.B
-   18000c0db:	rex.B (bad)
-   18000c0dd:	push   %r14
-   18000c0df:	(bad)
-   18000c0e0:	and    $0x74,%al
-   18000c0e2:	jne    0x18000c154
-   18000c0e4:	insb   (%dx),%es:(%rdi)
-   18000c0e5:	gs rex push %rsi
-   18000c0e8:	(bad)
-   18000c0e9:	and    $0x76,%al
-   18000c0eb:	movsxd %gs:0x72(%rdi,%rbp,2),%esi
-   18000c0f0:	rex
-   18000c0f1:	rex.WB push %r14
-   18000c0f3:	(bad)
-   18000c0f4:	and    $0x61,%al
-   18000c0f6:	insb   (%dx),%es:(%rdi)
-   18000c0f7:	insb   (%dx),%es:(%rdi)
-   18000c0f8:	outsl  %ds:(%rsi),(%dx)
-   18000c0f9:	movsxd 0x74(%rcx),%esp
-   18000c0fc:	outsl  %ds:(%rsi),(%dx)
-   18000c0fd:	jb     0x18000c13f
+   18000bf00:	(bad)
+   18000bf01:	(bad)
+   18000bf02:	add    %al,(%rax)
+   18000bf04:	add    %al,(%rax)
+   18000bf06:	add    %al,(%rax)
+   18000bf08:	rcl    %ch
+	...
+   18000bf16:	add    %al,(%rax)
+   18000bf18:	xchg   %eax,%esi
+   18000bf19:	(bad)
+   18000bf1a:	add    %al,(%rax)
+   18000bf1c:	add    %al,(%rax)
+   18000bf1e:	add    %al,(%rax)
+   18000bf20:	mov    %ss,%ebp
+   18000bf22:	add    %al,(%rax)
+   18000bf24:	add    %al,(%rax)
+   18000bf26:	add    %al,(%rax)
+   18000bf28:	adc    $0x0,%ch
+   18000bf2b:	add    %al,(%rax)
+   18000bf2d:	add    %al,(%rax)
+   18000bf2f:	add    %dh,-0x2b(%rsi)
+   18000bf32:	add    %al,(%rax)
+   18000bf34:	add    %al,(%rax)
+   18000bf36:	add    %al,(%rax)
+   18000bf38:	outsb  %ds:(%rsi),(%dx)
+   18000bf39:	(bad)
+   18000bf3a:	add    %al,(%rax)
+   18000bf3c:	add    %al,(%rax)
+   18000bf3e:	add    %al,(%rax)
+   18000bf40:	movabs 0x5c000000000000d5,%al
+   18000bf49:	(bad)
+   18000bf4a:	add    %al,(%rax)
+   18000bf4c:	add    %al,(%rax)
+   18000bf4e:	add    %al,(%rax)
+   18000bf50:	push   %rsp
+   18000bf51:	(bad)
+   18000bf52:	add    %al,(%rax)
+   18000bf54:	add    %al,(%rax)
+   18000bf56:	add    %al,(%rax)
+   18000bf58:	rex.WX (bad)
+   18000bf5a:	add    %al,(%rax)
+   18000bf5c:	add    %al,(%rax)
+   18000bf5e:	add    %al,(%rax)
+   18000bf60:	rex (bad)
+   18000bf62:	add    %al,(%rax)
+   18000bf64:	add    %al,(%rax)
+   18000bf66:	add    %al,(%rax)
+   18000bf68:	and    %ch,%dl
+   18000bf6a:	add    %al,(%rax)
+   18000bf6c:	add    %al,(%rax)
+   18000bf6e:	add    %al,(%rax)
+   18000bf70:	data16 (bad)
+	...
+   18000bf7e:	add    %al,(%rax)
+   18000bf80:	cmp    $0x0,%al
+   18000bf82:	(bad)
+   18000bf83:	imul   $0x6c616974,0x69(%rsi),%ebp
+   18000bf8a:	imul   $0x6d6f4340,0x65(%rdx),%edi
+   18000bf91:	insl   (%dx),%es:(%rdi)
+   18000bf92:	outsl  %ds:(%rsi),(%dx)
+   18000bf93:	outsb  %ds:(%rsi),(%dx)
+   18000bf94:	rex.WRB outsl %ds:(%rsi),(%dx)
+   18000bf96:	imul   $0x75537265,%fs:0x69(%rsi),%esp
+   18000bf9e:	jb     0x18000c006
+   18000bfa0:	(bad)
+   18000bfa1:	movsxd 0x4c(%rbp),%esp
+   18000bfa4:	imul   $0x40797261,0x72(%rdx),%esp
+   18000bfab:	outsl  %gs:(%esi),(%dx)
+   18000bfae:	fs gs rex
+   18000bfb1:	rex push %rbx
+   18000bfb3:	pop    %r8
+   18000bfb5:	pop    %rax
+   18000bfb6:	pop    %rdx
+   18000bfb7:	add    %ah,(%rdi)
+   18000bfb9:	add    %bh,(%rdi)
+   18000bfbb:	(bad)
+   18000bfbc:	xor    %bh,(%rdi)
+   18000bfbe:	and    $0x54,%al
+   18000bfc0:	jb     0x18000c02b
+   18000bfc2:	(bad)
+   18000bfc3:	outsb  %ds:(%rsi),(%dx)
+   18000bfc4:	addr32 jne 0x18000c033
+   18000bfc7:	(bad)
+   18000bfc8:	je     0x18000c02f
+   18000bfca:	fs push %rbx
+   18000bfcc:	jne    0x18000c040
+   18000bfce:	data16 (bad)
+   18000bfd0:	movsxd 0x4d(%rbp),%esp
+   18000bfd3:	outsl  %ds:(%rsi),(%dx)
+   18000bfd4:	imul   $0x24407265,%fs:0x69(%rsi),%esp
+   18000bfdc:	xor    %dh,(%rdx)
+   18000bfde:	rex
+   18000bfdf:	outsl  %gs:(%esi),(%dx)
+   18000bfe2:	fs gs rex
+   18000bfe5:	rex push %rcx
+   18000bfe7:	rex.RB
+   18000bfe8:	rex.B
+   18000bfe9:	rex.B
+   18000bfea:	rex
+   18000bfeb:	rex.B
+   18000bfec:	rex.RB
+   18000bfed:	rex.X push %rsi
+   18000bfef:	(bad)
+   18000bff0:	and    $0x53,%al
+   18000bff2:	jne    0x18000c066
+   18000bff4:	data16 (bad)
+   18000bff6:	movsxd 0x4d(%rbp),%esp
+   18000bff9:	gs jae 0x18000c064
+   18000bffc:	rex and $0x30,%al
+   18000bfff:	xor    0x31(%rax),%al
+   18000c002:	rex
+   18000c003:	rex.B
+   18000c004:	rex.RB
+   18000c005:	push   %r14
+   18000c007:	(bad)
+   18000c008:	and    $0x54,%al
+   18000c00a:	jb     0x18000c075
+   18000c00c:	(bad)
+   18000c00d:	outsb  %ds:(%rsi),(%dx)
+   18000c00e:	addr32 jne 0x18000c07d
+   18000c011:	(bad)
+   18000c012:	je     0x18000c079
+   18000c014:	fs push %rbx
+   18000c016:	jne    0x18000c08a
+   18000c018:	data16 (bad)
+   18000c01a:	movsxd 0x42(%rbp),%esp
+   18000c01d:	jne    0x18000c088
+   18000c01f:	insb   (%dx),%es:(%rdi)
+   18000c020:	fs gs jb 0x18000c064
+   18000c024:	and    $0x30,%al
+   18000c026:	xor    0x31(%rax),%al
+   18000c029:	rex
+   18000c02a:	rex pop %rdx
+   18000c02c:	add    %al,(%rax)
+   18000c02e:	sub    $0x0,%al
+   18000c030:	(bad)
+   18000c031:	(bad)
+   18000c032:	xor    %edi,(%rdi)
+   18000c034:	and    $0x54,%al
+   18000c036:	jb     0x18000c0a1
+   18000c038:	(bad)
+   18000c039:	outsb  %ds:(%rsi),(%dx)
+   18000c03a:	addr32 jne 0x18000c0a9
+   18000c03d:	(bad)
+   18000c03e:	je     0x18000c0a5
+   18000c040:	fs push %rbx
+   18000c042:	jne    0x18000c0b6
+   18000c044:	data16 (bad)
+   18000c046:	movsxd 0x4d(%rbp),%esp
+   18000c049:	outsl  %ds:(%rsi),(%dx)
+   18000c04a:	imul   $0x24407265,%fs:0x69(%rsi),%esp
+   18000c052:	xor    %dh,(%rdx)
+   18000c054:	rex
+   18000c055:	outsl  %gs:(%esi),(%dx)
+   18000c058:	fs gs rex
+   18000c05b:	rex push %rcx
+   18000c05d:	rex.RB
+   18000c05e:	rex.B
+   18000c05f:	rex.B
+   18000c060:	rex pop %rax
+   18000c062:	pop    %rdx
+   18000c063:	add    %al,0x3f(%rax,%rax,1)
+   18000c067:	imul   $0x65676465,0x5f(%rbx),%esi
+   18000c06e:	pop    %rdi
+   18000c06f:	(bad)
+   18000c070:	movsxd 0x76(%rcx,%rbp,2),%esi
+   18000c074:	gs rex (bad)
+   18000c077:	and    $0x54,%al
+   18000c079:	jb     0x18000c0e4
+   18000c07b:	(bad)
+   18000c07c:	outsb  %ds:(%rsi),(%dx)
+   18000c07d:	addr32 jne 0x18000c0ec
+   18000c080:	(bad)
+   18000c081:	je     0x18000c0e8
+   18000c083:	fs push %rbx
+   18000c085:	jne    0x18000c0f9
+   18000c087:	data16 (bad)
+   18000c089:	movsxd 0x4d(%rbp),%esp
+   18000c08c:	outsl  %ds:(%rsi),(%dx)
+   18000c08d:	imul   $0x24407265,%fs:0x69(%rsi),%esp
+   18000c095:	xor    %dh,(%rdx)
+   18000c097:	rex
+   18000c098:	outsl  %gs:(%esi),(%dx)
+   18000c09b:	fs gs rex
+   18000c09e:	rex push %rcx
+   18000c0a0:	rex.RB
+   18000c0a1:	rex.X
+   18000c0a2:	pop    %r15
+   18000c0a4:	rex.WRX
+   18000c0a5:	rex.WB
+   18000c0a6:	rex pop %rdx
+   18000c0a8:	add    %al,(%rax)
+   18000c0aa:	cmp    %eax,(%rax)
+   18000c0ac:	(bad)
+   18000c0ad:	movsxd 0x6c(%rdi),%ebp
+   18000c0b0:	insb   (%dx),%es:(%rdi)
+   18000c0b1:	(bad)
+   18000c0b2:	jo     0x18000c127
+   18000c0b4:	gs pop %rdi
+   18000c0b6:	gs fs addr32 gs rex (bad)
+   18000c0bc:	and    $0x54,%al
+   18000c0be:	jb     0x18000c129
+   18000c0c0:	(bad)
+   18000c0c1:	outsb  %ds:(%rsi),(%dx)
+   18000c0c2:	addr32 jne 0x18000c131
+   18000c0c5:	(bad)
+   18000c0c6:	je     0x18000c12d
+   18000c0c8:	fs push %rbx
+   18000c0ca:	jne    0x18000c13e
+   18000c0cc:	data16 (bad)
+   18000c0ce:	movsxd 0x4d(%rbp),%esp
+   18000c0d1:	outsl  %ds:(%rsi),(%dx)
+   18000c0d2:	imul   $0x24407265,%fs:0x69(%rsi),%esp
+   18000c0da:	xor    %dh,(%rdx)
+   18000c0dc:	rex
+   18000c0dd:	outsl  %gs:(%esi),(%dx)
+   18000c0e0:	fs gs rex
+   18000c0e3:	rex push %rcx
+   18000c0e5:	rex.RB
+   18000c0e6:	rex.B
+   18000c0e7:	rex.B (bad)
+   18000c0e9:	push   %r13
+   18000c0eb:	rex.XB outsl %ds:(%rsi),(%dx)
+   18000c0ed:	insb   (%dx),%es:(%rdi)
+   18000c0ee:	insb   (%dx),%es:(%rdi)
+   18000c0ef:	(bad)
+   18000c0f0:	jo     0x18000c165
+   18000c0f2:	gs rex.RB
+   18000c0f4:	fs rex.WB outsb %gs:(%esi),(%dx)
+   18000c0f9:	outsw  %ds:(%rsi),(%dx)
+   18000c0fb:	rex xor %esi,(%rdx)
+   18000c0fe:	rex
    18000c0ff:	rex.WB
-   18000c100:	rex jae 0x18000c177
-   18000c103:	fs rex
-   18000c105:	rex
-   18000c106:	rex jae 0x18000c17d
-   18000c109:	fs rex
-   18000c10b:	rex push %rsi
-   18000c10d:	xor    %esi,(%rdx)
-   18000c10f:	rex push %rsi
-   18000c111:	xor    %esi,(%rdx)
-   18000c113:	rex
-   18000c114:	rex jae 0x18000c18b
-   18000c117:	fs rex
-   18000c119:	rex pop %rax
-   18000c11b:	pop    %rdx
-   18000c11c:	add    %al,(%rax)
-   18000c11e:	(bad)
-   18000c11f:	add    %bh,(%rdi)
-   18000c121:	(bad)
-   18000c122:	and    $0x69,%al
-   18000c124:	jae    0x18000c185
-   18000c126:	movsxd 0x6c(%rdi),%ebp
-   18000c129:	insb   (%dx),%es:(%rdi)
-   18000c12a:	(bad)
-   18000c12b:	jo     0x18000c1a0
-   18000c12d:	gs pop %rdi
-   18000c12f:	gs fs addr32 gs pop %rdi
-   18000c134:	jbe    0x18000c197
-   18000c136:	insb   (%dx),%es:(%rdi)
-   18000c137:	imul   $0x67403230,0x24(%rax,%rax,2),%esp
-   18000c13f:	outsl  %gs:(%rsi),(%dx)
-   18000c141:	fs gs rex
-   18000c144:	rex pop %rcx
-   18000c146:	pop    %r15
-   18000c148:	rex.WRX
-   18000c149:	rex.B
-   18000c14a:	rex.RB
-   18000c14b:	rex.X push %rsi
-   18000c14d:	(bad)
-   18000c14e:	and    $0x54,%al
-   18000c150:	jb     0x18000c1bb
-   18000c152:	(bad)
-   18000c153:	outsb  %ds:(%rsi),(%dx)
-   18000c154:	addr32 jne 0x18000c1c3
-   18000c157:	(bad)
-   18000c158:	je     0x18000c1bf
-   18000c15a:	fs push %rbx
-   18000c15c:	jne    0x18000c1d0
-   18000c15e:	data16 (bad)
-   18000c160:	movsxd 0x40(%rbp),%esp
-   18000c163:	and    $0x30,%al
-   18000c165:	xor    0x30(%rax),%al
-   18000c168:	rex
-   18000c169:	rex.WB
-   18000c16a:	rex.B
-   18000c16b:	rex.RB
-   18000c16c:	rex.X push %rsi
-   18000c16e:	(bad)
-   18000c16f:	and    $0x50,%al
-   18000c171:	outsl  %ds:(%rsi),(%dx)
-   18000c172:	imul   $0x32302440,0x74(%rsi),%ebp
-   18000c179:	rex xor %al,0x40(%rax)
-   18000c17d:	pop    %rdx
-   18000c17e:	add    %al,(%rax)
-   18000c180:	rex.RXB
-   18000c181:	outsl  %gs:(%rsi),(%dx)
-   18000c183:	fs gs sub $0x6d6d6f43,%eax
-   18000c18a:	outsl  %ds:(%rsi),(%dx)
-   18000c18b:	outsb  %ds:(%rsi),(%dx)
-   18000c18c:	pop    %rdi
-   18000c18d:	insl   (%dx),%es:(%rdi)
-   18000c18e:	outsl  %ds:(%rsi),(%dx)
-   18000c18f:	imul   $0x735f7265,%fs:0x69(%rsi),%esp
-   18000c197:	jne    0x18000c20b
-   18000c199:	data16 (bad)
-   18000c19b:	movsxd 0x2e(%rbp),%esp
-   18000c19e:	fs insb (%dx),%es:(%rdi)
-   18000c1a0:	insb   (%dx),%es:(%rdi)
-   18000c1a1:	add    %dh,(%rdx)
-   18000c1a3:	(bad)
-   18000c1a4:	(bad)
-   18000c1a5:	outsb  %ds:(%rsi),(%dx)
-   18000c1a6:	(bad)
-   18000c1a7:	pop    %rdi
-   18000c1a8:	jbe    0x18000c20f
-   18000c1aa:	jb     0x18000c220
-   18000c1ac:	imul   $0x65564073,0x65(%rbx),%esp
-   18000c1b3:	jb     0x18000c229
-   18000c1b5:	gs js  0x18000c20b
-   18000c1b8:	gs je  0x18000c1fb
-   18000c1bb:	outsl  %gs:(%esi),(%dx)
-   18000c1be:	fs gs rex
-   18000c1c1:	rex push %rcx
-   18000c1c3:	rex.RB
-   18000c1c4:	rex.X
-   18000c1c5:	rex.B
-   18000c1c6:	rex.WB pop %r8
-   18000c1c8:	pop    %rdx
-   18000c1c9:	add    %bh,0x65763f07(%rcx)
-   18000c1cf:	jb     0x18000c245
-   18000c1d1:	gs js  0x18000c233
-   18000c1d4:	(bad)
-   18000c1d5:	je     0x18000c24b
-   18000c1d7:	jb     0x18000c242
-   18000c1d9:	(bad)
-   18000c1de:	insl   (%dx),%es:(%rdi)
-   18000c1df:	(bad)
-   18000c1e0:	outsb  %ds:(%rsi),(%dx)
-   18000c1e1:	(bad)
-   18000c1e2:	addr32 gs jb 0x18000c226
-   18000c1e6:	push   %rsi
-   18000c1e7:	gs jb  0x18000c25e
-   18000c1ea:	gs js  0x18000c240
-   18000c1ed:	gs je  0x18000c230
-   18000c1f0:	outsl  %gs:(%esi),(%dx)
-   18000c1f3:	fs gs rex
-   18000c1f6:	rex push %rcx
-   18000c1f8:	rex.RB
-   18000c1f9:	rex.X
-   18000c1fa:	rex.B
-   18000c1fb:	rex.B
-   18000c1fc:	rex.RB
-   18000c1fd:	push   %r14
-   18000c1ff:	rex.B je 0x18000c276
-   18000c202:	jb     0x18000c26d
-   18000c204:	(bad)
-   18000c209:	(bad)
-   18000c20a:	outsb  %ds:(%rsi),(%dx)
-   18000c20b:	(bad)
-   18000c20c:	addr32 gs jb 0x18000c250
-   18000c210:	xor    0x58(%rax),%al
-   18000c213:	pop    %rdx
-   18000c214:	add    %al,(%rax)
-   18000c216:	mov    $0x3,%dl
-   18000c218:	(bad)
-   18000c219:	movsxd 0x65(%rdx),%esi
-   18000c21c:	(bad)
-   18000c21d:	je     0x18000c284
-   18000c21f:	rex (bad)
-   18000c221:	and    $0x54,%al
-   18000c223:	jb     0x18000c28e
-   18000c225:	(bad)
-   18000c226:	outsb  %ds:(%rsi),(%dx)
-   18000c227:	addr32 jne 0x18000c296
-   18000c22a:	(bad)
-   18000c22b:	je     0x18000c292
-   18000c22d:	fs push %rbx
-   18000c22f:	jne    0x18000c2a3
-   18000c231:	data16 (bad)
-   18000c233:	movsxd 0x42(%rbp),%esp
-   18000c236:	jne    0x18000c2a1
-   18000c238:	insb   (%dx),%es:(%rdi)
-   18000c239:	fs gs jb 0x18000c27d
-   18000c23d:	and    $0x30,%al
-   18000c23f:	xor    0x67(%rax),%al
-   18000c242:	outsl  %gs:(%rsi),(%dx)
-   18000c244:	fs gs rex
-   18000c247:	rex push %rbx
-   18000c249:	rex.B (bad)
-   18000c24b:	push   %r14
-   18000c24d:	(bad)
-   18000c24e:	and    $0x75,%al
+   18000c100:	rex.B
+   18000c101:	rex.RB
+   18000c102:	rex.X push %rsi
+   18000c104:	(bad)
+   18000c105:	and    $0x50,%al
+   18000c107:	outsl  %ds:(%rsi),(%dx)
+   18000c108:	imul   $0x32302440,0x74(%rsi),%ebp
+   18000c10f:	rex xor 0x40(%rax),%al
+   18000c113:	pop    %rdx
+   18000c114:	add    %al,(%rax)
+   18000c116:	xor    %al,(%rax)
+   18000c118:	(bad)
+   18000c119:	movsxd 0x61(%rbp,%riz,2),%ebp
+   18000c11d:	outsb  %ds:(%rsi),(%dx)
+   18000c11e:	rex (bad)
+   18000c120:	and    $0x54,%al
+   18000c122:	jb     0x18000c18d
+   18000c124:	(bad)
+   18000c125:	outsb  %ds:(%rsi),(%dx)
+   18000c126:	addr32 jne 0x18000c195
+   18000c129:	(bad)
+   18000c12a:	je     0x18000c191
+   18000c12c:	fs push %rbx
+   18000c12e:	jne    0x18000c1a2
+   18000c130:	data16 (bad)
+   18000c132:	movsxd 0x4d(%rbp),%esp
+   18000c135:	outsl  %ds:(%rsi),(%dx)
+   18000c136:	imul   $0x24407265,%fs:0x69(%rsi),%esp
+   18000c13e:	xor    %dh,(%rdx)
+   18000c140:	rex
+   18000c141:	outsl  %gs:(%esi),(%dx)
+   18000c144:	fs gs rex
+   18000c147:	rex push %rcx
+   18000c149:	rex.RB
+   18000c14a:	rex.B
+   18000c14b:	rex.B (bad)
+   18000c14d:	push   %r14
+   18000c14f:	(bad)
+   18000c150:	and    $0x74,%al
+   18000c152:	jne    0x18000c1c4
+   18000c154:	insb   (%dx),%es:(%rdi)
+   18000c155:	gs rex push %rsi
+   18000c158:	(bad)
+   18000c159:	and    $0x76,%al
+   18000c15b:	movsxd %gs:0x72(%rdi,%rbp,2),%esi
+   18000c160:	rex
+   18000c161:	rex.WB push %r14
+   18000c163:	(bad)
+   18000c164:	and    $0x61,%al
+   18000c166:	insb   (%dx),%es:(%rdi)
+   18000c167:	insb   (%dx),%es:(%rdi)
+   18000c168:	outsl  %ds:(%rsi),(%dx)
+   18000c169:	movsxd 0x74(%rcx),%esp
+   18000c16c:	outsl  %ds:(%rsi),(%dx)
+   18000c16d:	jb     0x18000c1af
+   18000c16f:	rex.WB
+   18000c170:	rex jae 0x18000c1e7
+   18000c173:	fs rex
+   18000c175:	rex
+   18000c176:	rex jae 0x18000c1ed
+   18000c179:	fs rex
+   18000c17b:	rex push %rsi
+   18000c17d:	xor    %esi,(%rdx)
+   18000c17f:	rex push %rsi
+   18000c181:	xor    %esi,(%rdx)
+   18000c183:	rex
+   18000c184:	rex jae 0x18000c1fb
+   18000c187:	fs rex
+   18000c189:	rex pop %rax
+   18000c18b:	pop    %rdx
+   18000c18c:	add    %al,(%rax)
+   18000c18e:	(bad)
+   18000c18f:	add    %bh,(%rdi)
+   18000c191:	(bad)
+   18000c192:	and    $0x69,%al
+   18000c194:	jae    0x18000c1f5
+   18000c196:	movsxd 0x6c(%rdi),%ebp
+   18000c199:	insb   (%dx),%es:(%rdi)
+   18000c19a:	(bad)
+   18000c19b:	jo     0x18000c210
+   18000c19d:	gs pop %rdi
+   18000c19f:	gs fs addr32 gs pop %rdi
+   18000c1a4:	jbe    0x18000c207
+   18000c1a6:	insb   (%dx),%es:(%rdi)
+   18000c1a7:	imul   $0x67403230,0x24(%rax,%rax,2),%esp
+   18000c1af:	outsl  %gs:(%rsi),(%dx)
+   18000c1b1:	fs gs rex
+   18000c1b4:	rex pop %rcx
+   18000c1b6:	pop    %r15
+   18000c1b8:	rex.WRX
+   18000c1b9:	rex.B
+   18000c1ba:	rex.RB
+   18000c1bb:	rex.X push %rsi
+   18000c1bd:	(bad)
+   18000c1be:	and    $0x54,%al
+   18000c1c0:	jb     0x18000c22b
+   18000c1c2:	(bad)
+   18000c1c3:	outsb  %ds:(%rsi),(%dx)
+   18000c1c4:	addr32 jne 0x18000c233
+   18000c1c7:	(bad)
+   18000c1c8:	je     0x18000c22f
+   18000c1ca:	fs push %rbx
+   18000c1cc:	jne    0x18000c240
+   18000c1ce:	data16 (bad)
+   18000c1d0:	movsxd 0x40(%rbp),%esp
+   18000c1d3:	and    $0x30,%al
+   18000c1d5:	xor    0x30(%rax),%al
+   18000c1d8:	rex
+   18000c1d9:	rex.WB
+   18000c1da:	rex.B
+   18000c1db:	rex.RB
+   18000c1dc:	rex.X push %rsi
+   18000c1de:	(bad)
+   18000c1df:	and    $0x50,%al
+   18000c1e1:	outsl  %ds:(%rsi),(%dx)
+   18000c1e2:	imul   $0x32302440,0x74(%rsi),%ebp
+   18000c1e9:	rex xor %al,0x40(%rax)
+   18000c1ed:	pop    %rdx
+   18000c1ee:	add    %al,(%rax)
+   18000c1f0:	rex.RXB
+   18000c1f1:	outsl  %gs:(%rsi),(%dx)
+   18000c1f3:	fs gs sub $0x6d6d6f43,%eax
+   18000c1fa:	outsl  %ds:(%rsi),(%dx)
+   18000c1fb:	outsb  %ds:(%rsi),(%dx)
+   18000c1fc:	pop    %rdi
+   18000c1fd:	insl   (%dx),%es:(%rdi)
+   18000c1fe:	outsl  %ds:(%rsi),(%dx)
+   18000c1ff:	imul   $0x735f7265,%fs:0x69(%rsi),%esp
+   18000c207:	jne    0x18000c27b
+   18000c209:	data16 (bad)
+   18000c20b:	movsxd 0x2e(%rbp),%esp
+   18000c20e:	fs insb (%dx),%es:(%rdi)
+   18000c210:	insb   (%dx),%es:(%rdi)
+   18000c211:	add    %bl,0x6(%rsi)
+   18000c214:	(bad)
+   18000c215:	outsb  %ds:(%rsi),(%dx)
+   18000c216:	(bad)
+   18000c217:	pop    %rdi
+   18000c218:	jbe    0x18000c27f
+   18000c21a:	jb     0x18000c290
+   18000c21c:	imul   $0x65564073,0x65(%rbx),%esp
+   18000c223:	jb     0x18000c299
+   18000c225:	gs js  0x18000c27b
+   18000c228:	gs je  0x18000c26b
+   18000c22b:	outsl  %gs:(%esi),(%dx)
+   18000c22e:	fs gs rex
+   18000c231:	rex push %rcx
+   18000c233:	rex.RB
+   18000c234:	rex.X
+   18000c235:	rex.B
+   18000c236:	rex.WB pop %r8
+   18000c238:	pop    %rdx
+   18000c239:	add    %ah,%ch
+   18000c23b:	(bad)
+   18000c23c:	(bad)
+   18000c23d:	jbe    0x18000c2a4
+   18000c23f:	jb     0x18000c2b5
+   18000c241:	gs js  0x18000c2a3
+   18000c244:	(bad)
+   18000c245:	je     0x18000c2bb
+   18000c247:	jb     0x18000c2b2
+   18000c249:	(bad)
+   18000c24e:	insl   (%dx),%es:(%rdi)
+   18000c24f:	(bad)
    18000c250:	outsb  %ds:(%rsi),(%dx)
-   18000c251:	imul   $0x74705f65,0x75(%rcx),%esi
-   18000c258:	jb     0x18000c29a
-   18000c25a:	push   %rsi
-   18000c25b:	(bad)
-   18000c25c:	and    $0x54,%al
-   18000c25e:	jb     0x18000c2c9
-   18000c260:	(bad)
-   18000c261:	outsb  %ds:(%rsi),(%dx)
-   18000c262:	addr32 jne 0x18000c2d1
-   18000c265:	(bad)
-   18000c266:	je     0x18000c2cd
-   18000c268:	fs push %rbx
-   18000c26a:	jne    0x18000c2de
-   18000c26c:	data16 (bad)
-   18000c26e:	movsxd 0x42(%rbp),%esp
-   18000c271:	jne    0x18000c2dc
-   18000c273:	insb   (%dx),%es:(%rdi)
-   18000c274:	fs gs jb 0x18000c2b8
-   18000c278:	and    $0x30,%al
-   18000c27a:	xor    0x67(%rax),%al
-   18000c27d:	outsl  %gs:(%rsi),(%dx)
-   18000c27f:	fs gs rex
-   18000c282:	rex push %rbp
-   18000c284:	(bad)
-   18000c285:	and    $0x64,%al
-   18000c287:	gs data16 (bad)
-   18000c28a:	jne    0x18000c2f8
-   18000c28c:	je     0x18000c2ed
-   18000c28e:	fs gs insb (%dx),%es:(%rdi)
-   18000c291:	gs je  0x18000c2f9
-   18000c294:	rex push %rsi
-   18000c296:	(bad)
-   18000c297:	and    $0x54,%al
-   18000c299:	jb     0x18000c304
-   18000c29b:	(bad)
-   18000c29c:	outsb  %ds:(%rsi),(%dx)
-   18000c29d:	addr32 jne 0x18000c30c
-   18000c2a0:	(bad)
-   18000c2a1:	je     0x18000c308
-   18000c2a3:	fs push %rbx
-   18000c2a5:	jne    0x18000c319
-   18000c2a7:	data16 (bad)
-   18000c2a9:	movsxd 0x42(%rbp),%esp
-   18000c2ac:	jne    0x18000c317
-   18000c2ae:	insb   (%dx),%es:(%rdi)
-   18000c2af:	fs gs jb 0x18000c2f3
-   18000c2b3:	and    $0x30,%al
-   18000c2b5:	xor    0x67(%rax),%al
-   18000c2b8:	outsl  %gs:(%rsi),(%dx)
-   18000c2ba:	fs gs rex
-   18000c2bd:	rex
-   18000c2be:	rex jae 0x18000c335
-   18000c2c1:	fs rex
-   18000c2c3:	rex
-   18000c2c4:	rex jae 0x18000c33b
-   18000c2c7:	fs rex
-   18000c2c9:	rex
-   18000c2ca:	rex.B
-   18000c2cb:	rex.RB
-   18000c2cc:	push   %r14
-   18000c2ce:	(bad)
-   18000c2cf:	and    $0x54,%al
-   18000c2d1:	jb     0x18000c33c
-   18000c2d3:	(bad)
-   18000c2d4:	outsb  %ds:(%rsi),(%dx)
-   18000c2d5:	addr32 jne 0x18000c344
-   18000c2d8:	(bad)
-   18000c2d9:	je     0x18000c340
-   18000c2db:	fs push %rbx
-   18000c2dd:	jne    0x18000c351
-   18000c2df:	data16 (bad)
-   18000c2e1:	movsxd 0x40(%rbp),%esp
-   18000c2e4:	and    $0x30,%al
-   18000c2e6:	xor    0x32(%rax),%al
-   18000c2e9:	rex
-   18000c2ea:	rex pop %rdx
-   18000c2ec:	add    %al,(%rax)
-   18000c2ee:	push   %rdi
-   18000c2ef:	(bad)
-   18000c2f0:	(bad)
-   18000c2f1:	jo     0x18000c362
-   18000c2f3:	imul   $0x43243f40,0x74(%rsi),%ebp
-   18000c2fa:	outsl  %ds:(%rsi),(%dx)
-   18000c2fb:	outsl  %ds:(%rsi),(%dx)
-   18000c2fc:	jb     0x18000c362
-   18000c2fe:	imul   $0x65526574,0x61(%rsi),%ebp
-   18000c305:	data16 gs jb 0x18000c36e
-   18000c309:	outsb  %ds:(%rsi),(%dx)
-   18000c30a:	movsxd 0x53(%rbp),%esp
-   18000c30d:	jns    0x18000c382
-   18000c30f:	je     0x18000c376
-   18000c311:	insl   (%dx),%es:(%rdi)
-   18000c312:	rex.WRB (bad)
-   18000c314:	outsb  %ds:(%rsi),(%dx)
-   18000c315:	(bad)
-   18000c316:	addr32 gs jb 0x18000c38d
-   18000c31a:	rex and $0x30,%al
-   18000c31d:	xor    0x67(%rax),%al
-   18000c320:	outsl  %gs:(%rsi),(%dx)
-   18000c322:	fs gs rex
-   18000c325:	rex push %rcx
-   18000c327:	rex.RB
-   18000c328:	rex.X
-   18000c329:	rex.B
-   18000c32a:	rex.B
-   18000c32b:	rex.RB
-   18000c32c:	rex.X push %rsi
-   18000c32e:	(bad)
-   18000c32f:	and    $0x50,%al
-   18000c331:	outsl  %ds:(%rsi),(%dx)
-   18000c332:	imul   $0x32302440,0x74(%rsi),%ebp
-   18000c339:	rex xor 0x49(%rax),%al
-   18000c33d:	rex pop %rdx
-   18000c33f:	add    %ah,(%rdi)
-   18000c341:	(bad)
-   18000c342:	(bad)
-   18000c343:	outsb  %ds:(%rsi),(%dx)
-   18000c344:	(bad)
-   18000c345:	pop    %rdi
-   18000c346:	jo     0x18000c3b7
-   18000c348:	insb   (%dx),%es:(%rdi)
-   18000c349:	jns    0x18000c3b2
-   18000c34b:	outsl  %ds:(%rsi),(%dx)
-   18000c34c:	outsb  %ds:(%rsi),(%dx)
-   18000c34d:	jae    0x18000c38f
-   18000c34f:	(bad)
-   18000c350:	and    $0x53,%al
-   18000c352:	jne    0x18000c3c6
-   18000c354:	data16 (bad)
-   18000c356:	movsxd 0x4d(%rbp),%esp
-   18000c359:	gs jae 0x18000c3c4
-   18000c35c:	rex and $0x30,%al
-   18000c35f:	xor    0x67(%rax),%al
-   18000c362:	outsl  %gs:(%rsi),(%dx)
-   18000c364:	fs gs rex
-   18000c367:	rex push %rcx
-   18000c369:	rex.RB
-   18000c36a:	rex.X
-   18000c36b:	rex.B
-   18000c36c:	rex.WB pop %r8
-   18000c36e:	pop    %rdx
-   18000c36f:	add    %cl,0x64653f05(%rip)        # 0x1e466027a
-   18000c375:	addr32 gs pop %rdi
-   18000c378:	insb   (%dx),%es:(%rdi)
-   18000c379:	outsb  %gs:(%rsi),(%dx)
-   18000c37b:	addr32 je 0x18000c3e6
-   18000c37e:	rex (bad)
-   18000c380:	and    $0x53,%al
-   18000c382:	jne    0x18000c3f6
-   18000c384:	data16 (bad)
-   18000c386:	movsxd 0x4d(%rbp),%esp
-   18000c389:	gs jae 0x18000c3f4
-   18000c38c:	rex and $0x30,%al
-   18000c38f:	xor    0x67(%rax),%al
-   18000c392:	outsl  %gs:(%rsi),(%dx)
-   18000c394:	fs gs rex
-   18000c397:	rex push %rcx
-   18000c399:	rex.RB
-   18000c39a:	rex.X
-   18000c39b:	rex.B
-   18000c39c:	rex.WRX
-   18000c39d:	rex.B
-   18000c39e:	rex.RB
-   18000c39f:	rex.X push %rsi
-   18000c3a1:	(bad)
-   18000c3a2:	and    $0x61,%al
-   18000c3a4:	jb     0x18000c418
-   18000c3a6:	(bad)
-   18000c3a7:	jns    0x18000c3e9
-   18000c3a9:	rex.WB and $0x30,%al
-   18000c3ac:	xor    %eax,0x73(%rax)
-   18000c3af:	je     0x18000c415
-   18000c3b1:	rex
-   18000c3b2:	rex
-   18000c3b3:	rex pop %rdx
-   18000c3b5:	add    %dh,0x6(%rdi)
-   18000c3b8:	(bad)
-   18000c3b9:	jo     0x18000c42a
-   18000c3bb:	insb   (%dx),%es:(%rdi)
-   18000c3bc:	jns    0x18000c425
-   18000c3be:	outsl  %ds:(%rsi),(%dx)
-   18000c3bf:	outsb  %ds:(%rsi),(%dx)
-   18000c3c0:	jae    0x18000c421
-   18000c3c2:	(bad)
-   18000c3c3:	jb     0x18000c434
-   18000c3c5:	jne    0x18000c435
-   18000c3c7:	fs pop %rdi
-   18000c3c9:	jbe    0x18000c430
-   18000c3cb:	jb     0x18000c441
-   18000c3cd:	gs js  0x18000c410
-   18000c3d0:	(bad)
-   18000c3d1:	and    $0x53,%al
-   18000c3d3:	jne    0x18000c447
-   18000c3d5:	data16 (bad)
-   18000c3d7:	movsxd 0x4d(%rbp),%esp
-   18000c3da:	gs jae 0x18000c445
-   18000c3dd:	rex and $0x30,%al
-   18000c3e0:	xor    0x67(%rax),%al
-   18000c3e3:	outsl  %gs:(%rsi),(%dx)
-   18000c3e5:	fs gs rex
-   18000c3e8:	rex push %rcx
-   18000c3ea:	rex.RB
-   18000c3eb:	rex.X
-   18000c3ec:	rex.B
-   18000c3ed:	rex.B
-   18000c3ee:	rex.RB
-   18000c3ef:	rex.X push %rsi
-   18000c3f1:	(bad)
-   18000c3f2:	and    $0x49,%al
-   18000c3f4:	outsb  %ds:(%rsi),(%dx)
-   18000c3f5:	insb   (%dx),%es:(%rdi)
-   18000c3f6:	imul   $0x63655664,0x65(%rsi),%ebp
-   18000c3fd:	je     0x18000c46e
-   18000c3ff:	jb     0x18000c441
-   18000c401:	push   %rbp
-   18000c402:	push   %rax
-   18000c403:	outsl  %ds:(%rsi),(%dx)
-   18000c404:	insb   (%dx),%es:(%rdi)
-   18000c405:	jns    0x18000c46e
-   18000c407:	outsl  %ds:(%rsi),(%dx)
-   18000c408:	outsb  %ds:(%rsi),(%dx)
-   18000c409:	push   %rsi
-   18000c40a:	gs jb  0x18000c481
-   18000c40d:	gs js  0x18000c450
-   18000c410:	outsl  %gs:(%esi),(%dx)
-   18000c413:	fs gs rex
-   18000c416:	rex and $0x30,%al
-   18000c419:	cmp    %edx,0x3f(%rsi)
-   18000c41c:	and    $0x61,%al
-   18000c41e:	insb   (%dx),%es:(%rdi)
-   18000c41f:	insb   (%dx),%es:(%rdi)
-   18000c420:	outsl  %ds:(%rsi),(%dx)
-   18000c421:	movsxd 0x74(%rcx),%esp
-   18000c424:	outsl  %ds:(%rsi),(%dx)
-   18000c425:	jb     0x18000c467
-   18000c427:	push   %rbp
-   18000c428:	push   %rax
-   18000c429:	outsl  %ds:(%rsi),(%dx)
-   18000c42a:	insb   (%dx),%es:(%rdi)
-   18000c42b:	jns    0x18000c494
-   18000c42d:	outsl  %ds:(%rsi),(%dx)
-   18000c42e:	outsb  %ds:(%rsi),(%dx)
-   18000c42f:	push   %rsi
-   18000c430:	gs jb  0x18000c4a7
-   18000c433:	gs js  0x18000c476
-   18000c436:	outsl  %gs:(%esi),(%dx)
-   18000c439:	fs gs rex
-   18000c43c:	rex
-   18000c43d:	rex jae 0x18000c4b4
-   18000c440:	fs rex
-   18000c442:	rex
-   18000c443:	rex (bad)
-   18000c445:	(bad)
-   18000c44a:	rex.WB
-   18000c44b:	rex pop %rdx
-   18000c44d:	add    %ah,(%rdx)
-   18000c44f:	add    $0x616e653f,%eax
-   18000c454:	(bad)
-   18000c455:	insb   (%dx),%es:(%rdi)
-   18000c456:	gs pop %rdi
-   18000c458:	gs fs addr32 gs jae 0x18000c49e
-   18000c45e:	(bad)
-   18000c45f:	and    $0x53,%al
-   18000c461:	jne    0x18000c4d5
-   18000c463:	data16 (bad)
-   18000c465:	movsxd 0x4d(%rbp),%esp
-   18000c468:	gs jae 0x18000c4d3
-   18000c46b:	rex and $0x30,%al
-   18000c46e:	xor    0x67(%rax),%al
-   18000c471:	outsl  %gs:(%rsi),(%dx)
-   18000c473:	fs gs rex
-   18000c476:	rex push %rcx
-   18000c478:	rex.RB
-   18000c479:	rex.X
-   18000c47a:	pop    %r8
-   18000c47c:	pop    %rax
-   18000c47d:	pop    %rdx
-   18000c47e:	add    %al,(%rax)
-   18000c480:	rex.B add $0x3f,%al
-   18000c483:	imul   $0x5f656c62,%fs:0x61(%rbx),%esi
-   18000c48b:	gs fs addr32 gs jae 0x18000c4d1
-   18000c491:	(bad)
-   18000c492:	and    $0x53,%al
-   18000c494:	jne    0x18000c508
-   18000c496:	data16 (bad)
-   18000c498:	movsxd 0x4d(%rbp),%esp
-   18000c49b:	gs jae 0x18000c506
-   18000c49e:	rex and $0x30,%al
-   18000c4a1:	xor    0x67(%rax),%al
-   18000c4a4:	outsl  %gs:(%rsi),(%dx)
-   18000c4a6:	fs gs rex
-   18000c4a9:	rex push %rcx
-   18000c4ab:	rex.RB
-   18000c4ac:	rex.X
-   18000c4ad:	pop    %r8
-   18000c4af:	pop    %rax
-   18000c4b0:	pop    %rdx
-   18000c4b1:	add    %bl,(%rbx)
-   18000c4b3:	add    $0x6764653f,%eax
-   18000c4b8:	gs jae 0x18000c4fb
-   18000c4bb:	(bad)
-   18000c4bc:	and    $0x53,%al
-   18000c4be:	jne    0x18000c532
-   18000c4c0:	data16 (bad)
-   18000c4c2:	movsxd 0x4d(%rbp),%esp
-   18000c4c5:	gs jae 0x18000c530
-   18000c4c8:	rex and $0x30,%al
-   18000c4cb:	xor    0x67(%rax),%al
-   18000c4ce:	outsl  %gs:(%rsi),(%dx)
-   18000c4d0:	fs gs rex
-   18000c4d3:	rex push %rcx
-   18000c4d5:	rex.RB
-   18000c4d6:	rex.X
-   18000c4d7:	rex.B
-   18000c4d8:	rex.B
-   18000c4d9:	rex.RB
-   18000c4da:	rex.X push %rsi
-   18000c4dc:	(bad)
-   18000c4dd:	and    $0x53,%al
-   18000c4df:	jne    0x18000c553
-   18000c4e1:	data16 (bad)
-   18000c4e3:	movsxd 0x45(%rbp),%esp
-   18000c4e6:	fs addr32 gs jae 0x18000c52b
-   18000c4eb:	and    $0x30,%al
-   18000c4ed:	xor    0x32(%rax),%al
-   18000c4f0:	rex pop %rax
-   18000c4f2:	pop    %rdx
-   18000c4f3:	add    %cl,0x7(%rdx)
-   18000c4f6:	(bad)
-   18000c4f7:	je     0x18000c56b
-   18000c4f9:	imul   $0x40656c67,0x6e(%rcx),%esp
-   18000c500:	(bad)
-   18000c501:	and    $0x54,%al
-   18000c503:	jb     0x18000c56e
-   18000c505:	(bad)
-   18000c506:	outsb  %ds:(%rsi),(%dx)
-   18000c507:	addr32 jne 0x18000c576
-   18000c50a:	(bad)
-   18000c50b:	je     0x18000c572
-   18000c50d:	fs push %rbx
-   18000c50f:	jne    0x18000c583
-   18000c511:	data16 (bad)
-   18000c513:	movsxd 0x40(%rbp),%esp
-   18000c516:	and    $0x30,%al
-   18000c518:	xor    0x67(%rax),%al
-   18000c51b:	outsl  %gs:(%rsi),(%dx)
-   18000c51d:	fs gs rex
-   18000c520:	rex push %rcx
-   18000c522:	rex.RB
-   18000c523:	rex.X
-   18000c524:	rex.B (bad)
-   18000c526:	push   %r14
-   18000c528:	(bad)
-   18000c529:	and    $0x54,%al
-   18000c52b:	jb     0x18000c596
-   18000c52d:	(bad)
-   18000c52e:	outsb  %ds:(%rsi),(%dx)
-   18000c52f:	insb   (%dx),%es:(%edi)
-   18000c531:	gs rex and $0x30,%al
-   18000c535:	xor    0x32(%rax),%al
-   18000c538:	rex
-   18000c539:	rex.WB
-   18000c53a:	rex pop %rdx
-   18000c53c:	add    %al,(%rax)
-   18000c53e:	rex.WX add %dil,(%rdi)
-   18000c541:	(bad)
-   18000c542:	and    $0x73,%al
-   18000c544:	(bad)
-   18000c545:	jbe    0x18000c5ac
-   18000c547:	pop    %rdi
-   18000c548:	je     0x18000c5bc
-   18000c54a:	imul   $0x616c7567,0x6e(%rcx),%esp
-   18000c551:	je     0x18000c5b8
-   18000c553:	fs pop %rdi
-   18000c555:	jae    0x18000c5cc
-   18000c557:	jb     0x18000c5bf
-   18000c559:	(bad)
-   18000c55a:	movsxd 0x40(%rbp),%esp
-   18000c55d:	and    $0x30,%al
-   18000c55f:	xor    0x67(%rax),%al
-   18000c562:	outsl  %gs:(%rsi),(%dx)
-   18000c564:	fs gs rex
-   18000c567:	rex pop %rcx
-   18000c569:	pop    %r8
-   18000c56b:	rex.B
-   18000c56c:	rex.RB
-   18000c56d:	rex.X push %rsi
-   18000c56f:	(bad)
-   18000c570:	and    $0x54,%al
-   18000c572:	jb     0x18000c5dd
-   18000c574:	(bad)
-   18000c575:	outsb  %ds:(%rsi),(%dx)
-   18000c576:	addr32 jne 0x18000c5e5
-   18000c579:	(bad)
-   18000c57a:	je     0x18000c5e1
-   18000c57c:	fs push %rbx
-   18000c57e:	jne    0x18000c5f2
-   18000c580:	data16 (bad)
-   18000c582:	movsxd 0x40(%rbp),%esp
-   18000c585:	and    $0x30,%al
-   18000c587:	xor    0x30(%rax),%al
-   18000c58a:	rex push %rsi
-   18000c58c:	jae    0x18000c602
-   18000c58e:	jb     0x18000c5f9
-   18000c590:	outsb  %ds:(%rsi),(%dx)
-   18000c591:	addr32 pop %rdi
-   18000c593:	jbe    0x18000c5fe
-   18000c595:	gs ja  0x18000c5d8
+   18000c251:	(bad)
+   18000c252:	addr32 gs jb 0x18000c296
+   18000c256:	push   %rsi
+   18000c257:	gs jb  0x18000c2ce
+   18000c25a:	gs js  0x18000c2b0
+   18000c25d:	gs je  0x18000c2a0
+   18000c260:	outsl  %gs:(%esi),(%dx)
+   18000c263:	fs gs rex
+   18000c266:	rex push %rcx
+   18000c268:	rex.RB
+   18000c269:	rex.X
+   18000c26a:	rex.B
+   18000c26b:	rex.B
+   18000c26c:	rex.RB
+   18000c26d:	push   %r14
+   18000c26f:	rex.B je 0x18000c2e6
+   18000c272:	jb     0x18000c2dd
+   18000c274:	(bad)
+   18000c279:	(bad)
+   18000c27a:	outsb  %ds:(%rsi),(%dx)
+   18000c27b:	(bad)
+   18000c27c:	addr32 gs jb 0x18000c2c0
+   18000c280:	xor    0x58(%rax),%al
+   18000c283:	pop    %rdx
+   18000c284:	add    %al,(%rax)
+   18000c286:	fiadds (%rbx)
+   18000c288:	(bad)
+   18000c289:	movsxd 0x65(%rdx),%esi
+   18000c28c:	(bad)
+   18000c28d:	je     0x18000c2f4
+   18000c28f:	rex (bad)
+   18000c291:	and    $0x54,%al
+   18000c293:	jb     0x18000c2fe
+   18000c295:	(bad)
+   18000c296:	outsb  %ds:(%rsi),(%dx)
+   18000c297:	addr32 jne 0x18000c306
+   18000c29a:	(bad)
+   18000c29b:	je     0x18000c302
+   18000c29d:	fs push %rbx
+   18000c29f:	jne    0x18000c313
+   18000c2a1:	data16 (bad)
+   18000c2a3:	movsxd 0x42(%rbp),%esp
+   18000c2a6:	jne    0x18000c311
+   18000c2a8:	insb   (%dx),%es:(%rdi)
+   18000c2a9:	fs gs jb 0x18000c2ed
+   18000c2ad:	and    $0x30,%al
+   18000c2af:	xor    0x67(%rax),%al
+   18000c2b2:	outsl  %gs:(%rsi),(%dx)
+   18000c2b4:	fs gs rex
+   18000c2b7:	rex push %rbx
+   18000c2b9:	rex.B (bad)
+   18000c2bb:	push   %r14
+   18000c2bd:	(bad)
+   18000c2be:	and    $0x75,%al
+   18000c2c0:	outsb  %ds:(%rsi),(%dx)
+   18000c2c1:	imul   $0x74705f65,0x75(%rcx),%esi
+   18000c2c8:	jb     0x18000c30a
+   18000c2ca:	push   %rsi
+   18000c2cb:	(bad)
+   18000c2cc:	and    $0x54,%al
+   18000c2ce:	jb     0x18000c339
+   18000c2d0:	(bad)
+   18000c2d1:	outsb  %ds:(%rsi),(%dx)
+   18000c2d2:	addr32 jne 0x18000c341
+   18000c2d5:	(bad)
+   18000c2d6:	je     0x18000c33d
+   18000c2d8:	fs push %rbx
+   18000c2da:	jne    0x18000c34e
+   18000c2dc:	data16 (bad)
+   18000c2de:	movsxd 0x42(%rbp),%esp
+   18000c2e1:	jne    0x18000c34c
+   18000c2e3:	insb   (%dx),%es:(%rdi)
+   18000c2e4:	fs gs jb 0x18000c328
+   18000c2e8:	and    $0x30,%al
+   18000c2ea:	xor    0x67(%rax),%al
+   18000c2ed:	outsl  %gs:(%rsi),(%dx)
+   18000c2ef:	fs gs rex
+   18000c2f2:	rex push %rbp
+   18000c2f4:	(bad)
+   18000c2f5:	and    $0x64,%al
+   18000c2f7:	gs data16 (bad)
+   18000c2fa:	jne    0x18000c368
+   18000c2fc:	je     0x18000c35d
+   18000c2fe:	fs gs insb (%dx),%es:(%rdi)
+   18000c301:	gs je  0x18000c369
+   18000c304:	rex push %rsi
+   18000c306:	(bad)
+   18000c307:	and    $0x54,%al
+   18000c309:	jb     0x18000c374
+   18000c30b:	(bad)
+   18000c30c:	outsb  %ds:(%rsi),(%dx)
+   18000c30d:	addr32 jne 0x18000c37c
+   18000c310:	(bad)
+   18000c311:	je     0x18000c378
+   18000c313:	fs push %rbx
+   18000c315:	jne    0x18000c389
+   18000c317:	data16 (bad)
+   18000c319:	movsxd 0x42(%rbp),%esp
+   18000c31c:	jne    0x18000c387
+   18000c31e:	insb   (%dx),%es:(%rdi)
+   18000c31f:	fs gs jb 0x18000c363
+   18000c323:	and    $0x30,%al
+   18000c325:	xor    0x67(%rax),%al
+   18000c328:	outsl  %gs:(%rsi),(%dx)
+   18000c32a:	fs gs rex
+   18000c32d:	rex
+   18000c32e:	rex jae 0x18000c3a5
+   18000c331:	fs rex
+   18000c333:	rex
+   18000c334:	rex jae 0x18000c3ab
+   18000c337:	fs rex
+   18000c339:	rex
+   18000c33a:	rex.B
+   18000c33b:	rex.RB
+   18000c33c:	push   %r14
+   18000c33e:	(bad)
+   18000c33f:	and    $0x54,%al
+   18000c341:	jb     0x18000c3ac
+   18000c343:	(bad)
+   18000c344:	outsb  %ds:(%rsi),(%dx)
+   18000c345:	addr32 jne 0x18000c3b4
+   18000c348:	(bad)
+   18000c349:	je     0x18000c3b0
+   18000c34b:	fs push %rbx
+   18000c34d:	jne    0x18000c3c1
+   18000c34f:	data16 (bad)
+   18000c351:	movsxd 0x40(%rbp),%esp
+   18000c354:	and    $0x30,%al
+   18000c356:	xor    0x32(%rax),%al
+   18000c359:	rex
+   18000c35a:	rex pop %rdx
+   18000c35c:	add    %al,(%rax)
+   18000c35e:	addl   $0x3f,(%rsi)
+   18000c361:	jo     0x18000c3d2
+   18000c363:	imul   $0x43243f40,0x74(%rsi),%ebp
+   18000c36a:	outsl  %ds:(%rsi),(%dx)
+   18000c36b:	outsl  %ds:(%rsi),(%dx)
+   18000c36c:	jb     0x18000c3d2
+   18000c36e:	imul   $0x65526574,0x61(%rsi),%ebp
+   18000c375:	data16 gs jb 0x18000c3de
+   18000c379:	outsb  %ds:(%rsi),(%dx)
+   18000c37a:	movsxd 0x53(%rbp),%esp
+   18000c37d:	jns    0x18000c3f2
+   18000c37f:	je     0x18000c3e6
+   18000c381:	insl   (%dx),%es:(%rdi)
+   18000c382:	rex.WRB (bad)
+   18000c384:	outsb  %ds:(%rsi),(%dx)
+   18000c385:	(bad)
+   18000c386:	addr32 gs jb 0x18000c3fd
+   18000c38a:	rex and $0x30,%al
+   18000c38d:	xor    0x67(%rax),%al
+   18000c390:	outsl  %gs:(%rsi),(%dx)
+   18000c392:	fs gs rex
+   18000c395:	rex push %rcx
+   18000c397:	rex.RB
+   18000c398:	rex.X
+   18000c399:	rex.B
+   18000c39a:	rex.B
+   18000c39b:	rex.RB
+   18000c39c:	rex.X push %rsi
+   18000c39e:	(bad)
+   18000c39f:	and    $0x50,%al
+   18000c3a1:	outsl  %ds:(%rsi),(%dx)
+   18000c3a2:	imul   $0x32302440,0x74(%rsi),%ebp
+   18000c3a9:	rex xor 0x49(%rax),%al
+   18000c3ad:	rex pop %rdx
+   18000c3af:	add    %dl,0x6(%rbx)
+   18000c3b2:	(bad)
+   18000c3b3:	outsb  %ds:(%rsi),(%dx)
+   18000c3b4:	(bad)
+   18000c3b5:	pop    %rdi
+   18000c3b6:	jo     0x18000c427
+   18000c3b8:	insb   (%dx),%es:(%rdi)
+   18000c3b9:	jns    0x18000c422
+   18000c3bb:	outsl  %ds:(%rsi),(%dx)
+   18000c3bc:	outsb  %ds:(%rsi),(%dx)
+   18000c3bd:	jae    0x18000c3ff
+   18000c3bf:	(bad)
+   18000c3c0:	and    $0x53,%al
+   18000c3c2:	jne    0x18000c436
+   18000c3c4:	data16 (bad)
+   18000c3c6:	movsxd 0x4d(%rbp),%esp
+   18000c3c9:	gs jae 0x18000c434
+   18000c3cc:	rex and $0x30,%al
+   18000c3cf:	xor    0x67(%rax),%al
+   18000c3d2:	outsl  %gs:(%rsi),(%dx)
+   18000c3d4:	fs gs rex
+   18000c3d7:	rex push %rcx
+   18000c3d9:	rex.RB
+   18000c3da:	rex.X
+   18000c3db:	rex.B
+   18000c3dc:	rex.WB pop %r8
+   18000c3de:	pop    %rdx
+   18000c3df:	add    %bh,(%rcx)
+   18000c3e1:	add    $0x6764653f,%eax
+   18000c3e6:	gs pop %rdi
+   18000c3e8:	insb   (%dx),%es:(%rdi)
+   18000c3e9:	outsb  %gs:(%rsi),(%dx)
+   18000c3eb:	addr32 je 0x18000c456
+   18000c3ee:	rex (bad)
+   18000c3f0:	and    $0x53,%al
+   18000c3f2:	jne    0x18000c466
+   18000c3f4:	data16 (bad)
+   18000c3f6:	movsxd 0x4d(%rbp),%esp
+   18000c3f9:	gs jae 0x18000c464
+   18000c3fc:	rex and $0x30,%al
+   18000c3ff:	xor    0x67(%rax),%al
+   18000c402:	outsl  %gs:(%rsi),(%dx)
+   18000c404:	fs gs rex
+   18000c407:	rex push %rcx
+   18000c409:	rex.RB
+   18000c40a:	rex.X
+   18000c40b:	rex.B
+   18000c40c:	rex.WRX
+   18000c40d:	rex.B
+   18000c40e:	rex.RB
+   18000c40f:	rex.X push %rsi
+   18000c411:	(bad)
+   18000c412:	and    $0x61,%al
+   18000c414:	jb     0x18000c488
+   18000c416:	(bad)
+   18000c417:	jns    0x18000c459
+   18000c419:	rex.WB and $0x30,%al
+   18000c41c:	xor    %eax,0x73(%rax)
+   18000c41f:	je     0x18000c485
+   18000c421:	rex
+   18000c422:	rex
+   18000c423:	rex pop %rdx
+   18000c425:	add    %ah,0x6f703f06(%rbx)
+   18000c42b:	insb   (%dx),%es:(%rdi)
+   18000c42c:	jns    0x18000c495
+   18000c42e:	outsl  %ds:(%rsi),(%dx)
+   18000c42f:	outsb  %ds:(%rsi),(%dx)
+   18000c430:	jae    0x18000c491
+   18000c432:	(bad)
+   18000c433:	jb     0x18000c4a4
+   18000c435:	jne    0x18000c4a5
+   18000c437:	fs pop %rdi
+   18000c439:	jbe    0x18000c4a0
+   18000c43b:	jb     0x18000c4b1
+   18000c43d:	gs js  0x18000c480
+   18000c440:	(bad)
+   18000c441:	and    $0x53,%al
+   18000c443:	jne    0x18000c4b7
+   18000c445:	data16 (bad)
+   18000c447:	movsxd 0x4d(%rbp),%esp
+   18000c44a:	gs jae 0x18000c4b5
+   18000c44d:	rex and $0x30,%al
+   18000c450:	xor    0x67(%rax),%al
+   18000c453:	outsl  %gs:(%rsi),(%dx)
+   18000c455:	fs gs rex
+   18000c458:	rex push %rcx
+   18000c45a:	rex.RB
+   18000c45b:	rex.X
+   18000c45c:	rex.B
+   18000c45d:	rex.B
+   18000c45e:	rex.RB
+   18000c45f:	rex.X push %rsi
+   18000c461:	(bad)
+   18000c462:	and    $0x49,%al
+   18000c464:	outsb  %ds:(%rsi),(%dx)
+   18000c465:	insb   (%dx),%es:(%rdi)
+   18000c466:	imul   $0x63655664,0x65(%rsi),%ebp
+   18000c46d:	je     0x18000c4de
+   18000c46f:	jb     0x18000c4b1
+   18000c471:	push   %rbp
+   18000c472:	push   %rax
+   18000c473:	outsl  %ds:(%rsi),(%dx)
+   18000c474:	insb   (%dx),%es:(%rdi)
+   18000c475:	jns    0x18000c4de
+   18000c477:	outsl  %ds:(%rsi),(%dx)
+   18000c478:	outsb  %ds:(%rsi),(%dx)
+   18000c479:	push   %rsi
+   18000c47a:	gs jb  0x18000c4f1
+   18000c47d:	gs js  0x18000c4c0
+   18000c480:	outsl  %gs:(%esi),(%dx)
+   18000c483:	fs gs rex
+   18000c486:	rex and $0x30,%al
+   18000c489:	cmp    %edx,0x3f(%rsi)
+   18000c48c:	and    $0x61,%al
+   18000c48e:	insb   (%dx),%es:(%rdi)
+   18000c48f:	insb   (%dx),%es:(%rdi)
+   18000c490:	outsl  %ds:(%rsi),(%dx)
+   18000c491:	movsxd 0x74(%rcx),%esp
+   18000c494:	outsl  %ds:(%rsi),(%dx)
+   18000c495:	jb     0x18000c4d7
+   18000c497:	push   %rbp
+   18000c498:	push   %rax
+   18000c499:	outsl  %ds:(%rsi),(%dx)
+   18000c49a:	insb   (%dx),%es:(%rdi)
+   18000c49b:	jns    0x18000c504
+   18000c49d:	outsl  %ds:(%rsi),(%dx)
+   18000c49e:	outsb  %ds:(%rsi),(%dx)
+   18000c49f:	push   %rsi
+   18000c4a0:	gs jb  0x18000c517
+   18000c4a3:	gs js  0x18000c4e6
+   18000c4a6:	outsl  %gs:(%esi),(%dx)
+   18000c4a9:	fs gs rex
+   18000c4ac:	rex
+   18000c4ad:	rex jae 0x18000c524
+   18000c4b0:	fs rex
+   18000c4b2:	rex
+   18000c4b3:	rex (bad)
+   18000c4b5:	(bad)
+   18000c4ba:	rex.WB
+   18000c4bb:	rex pop %rdx
+   18000c4bd:	add    %cl,0x5(%rsi)
+   18000c4c0:	(bad)
+   18000c4c1:	outsb  %gs:(%rsi),(%dx)
+   18000c4c3:	(bad)
+   18000c4c4:	(bad)
+   18000c4c5:	insb   (%dx),%es:(%rdi)
+   18000c4c6:	gs pop %rdi
+   18000c4c8:	gs fs addr32 gs jae 0x18000c50e
+   18000c4ce:	(bad)
+   18000c4cf:	and    $0x53,%al
+   18000c4d1:	jne    0x18000c545
+   18000c4d3:	data16 (bad)
+   18000c4d5:	movsxd 0x4d(%rbp),%esp
+   18000c4d8:	gs jae 0x18000c543
+   18000c4db:	rex and $0x30,%al
+   18000c4de:	xor    0x67(%rax),%al
+   18000c4e1:	outsl  %gs:(%rsi),(%dx)
+   18000c4e3:	fs gs rex
+   18000c4e6:	rex push %rcx
+   18000c4e8:	rex.RB
+   18000c4e9:	rex.X
+   18000c4ea:	pop    %r8
+   18000c4ec:	pop    %rax
+   18000c4ed:	pop    %rdx
+   18000c4ee:	add    %al,(%rax)
+   18000c4f0:	insl   (%dx),%es:(%rdi)
+   18000c4f1:	add    $0x3f,%al
+   18000c4f3:	imul   $0x5f656c62,%fs:0x61(%rbx),%esi
+   18000c4fb:	gs fs addr32 gs jae 0x18000c541
+   18000c501:	(bad)
+   18000c502:	and    $0x53,%al
+   18000c504:	jne    0x18000c578
+   18000c506:	data16 (bad)
+   18000c508:	movsxd 0x4d(%rbp),%esp
+   18000c50b:	gs jae 0x18000c576
+   18000c50e:	rex and $0x30,%al
+   18000c511:	xor    0x67(%rax),%al
+   18000c514:	outsl  %gs:(%rsi),(%dx)
+   18000c516:	fs gs rex
+   18000c519:	rex push %rcx
+   18000c51b:	rex.RB
+   18000c51c:	rex.X
+   18000c51d:	pop    %r8
+   18000c51f:	pop    %rax
+   18000c520:	pop    %rdx
+   18000c521:	add    %al,0x5(%rdi)
+   18000c524:	(bad)
+   18000c525:	gs fs addr32 gs jae 0x18000c56b
+   18000c52b:	(bad)
+   18000c52c:	and    $0x53,%al
+   18000c52e:	jne    0x18000c5a2
+   18000c530:	data16 (bad)
+   18000c532:	movsxd 0x4d(%rbp),%esp
+   18000c535:	gs jae 0x18000c5a0
+   18000c538:	rex and $0x30,%al
+   18000c53b:	xor    0x67(%rax),%al
+   18000c53e:	outsl  %gs:(%rsi),(%dx)
+   18000c540:	fs gs rex
+   18000c543:	rex push %rcx
+   18000c545:	rex.RB
+   18000c546:	rex.X
+   18000c547:	rex.B
+   18000c548:	rex.B
+   18000c549:	rex.RB
+   18000c54a:	rex.X push %rsi
+   18000c54c:	(bad)
+   18000c54d:	and    $0x53,%al
+   18000c54f:	jne    0x18000c5c3
+   18000c551:	data16 (bad)
+   18000c553:	movsxd 0x45(%rbp),%esp
+   18000c556:	fs addr32 gs jae 0x18000c59b
+   18000c55b:	and    $0x30,%al
+   18000c55d:	xor    0x32(%rax),%al
+   18000c560:	rex pop %rax
+   18000c562:	pop    %rdx
+   18000c563:	add    %dh,0x7(%rsi)
+   18000c566:	(bad)
+   18000c567:	je     0x18000c5db
+   18000c569:	imul   $0x40656c67,0x6e(%rcx),%esp
+   18000c570:	(bad)
+   18000c571:	and    $0x54,%al
+   18000c573:	jb     0x18000c5de
+   18000c575:	(bad)
+   18000c576:	outsb  %ds:(%rsi),(%dx)
+   18000c577:	addr32 jne 0x18000c5e6
+   18000c57a:	(bad)
+   18000c57b:	je     0x18000c5e2
+   18000c57d:	fs push %rbx
+   18000c57f:	jne    0x18000c5f3
+   18000c581:	data16 (bad)
+   18000c583:	movsxd 0x40(%rbp),%esp
+   18000c586:	and    $0x30,%al
+   18000c588:	xor    0x67(%rax),%al
+   18000c58b:	outsl  %gs:(%rsi),(%dx)
+   18000c58d:	fs gs rex
+   18000c590:	rex push %rcx
+   18000c592:	rex.RB
+   18000c593:	rex.X
+   18000c594:	rex.B (bad)
+   18000c596:	push   %r14
    18000c598:	(bad)
-   18000c599:	(bad)
-   18000c59e:	rex pop %rdx
-   18000c5a0:	add    %al,(%rax)
-   18000c5a2:	xor    $0x243f3f00,%eax
-   18000c5a7:	jo     0x18000c618
-   18000c5a9:	insb   (%dx),%es:(%rdi)
-   18000c5aa:	jns    0x18000c613
-   18000c5ac:	outsl  %ds:(%rsi),(%dx)
-   18000c5ad:	outsb  %ds:(%rsi),(%dx)
-   18000c5ae:	pop    %rdi
-   18000c5af:	jbe    0x18000c616
-   18000c5b1:	jb     0x18000c627
-   18000c5b3:	gs js  0x18000c615
-   18000c5b6:	outsb  %ds:(%rsi),(%dx)
-   18000c5b7:	outsl  %ds:(%rsi),(%dx)
-   18000c5b8:	jb     0x18000c627
-   18000c5ba:	(bad)
-   18000c5bb:	insb   (%dx),%es:(%rdi)
-   18000c5bc:	rex and $0x30,%al
-   18000c5bf:	xor    0x3f(%rax),%al
-   18000c5c2:	and    $0x53,%al
-   18000c5c4:	jne    0x18000c638
-   18000c5c6:	data16 (bad)
-   18000c5c8:	movsxd 0x4d(%rbp),%esp
-   18000c5cb:	gs jae 0x18000c636
-   18000c5ce:	rex and $0x30,%al
-   18000c5d1:	xor    0x67(%rax),%al
-   18000c5d4:	outsl  %gs:(%rsi),(%dx)
-   18000c5d6:	fs gs rex
-   18000c5d9:	rex push %rcx
-   18000c5db:	rex.RB
-   18000c5dc:	rex.X
-   18000c5dd:	rex.B (bad)
-   18000c5df:	push   %r14
-   18000c5e1:	(bad)
-   18000c5e2:	and    $0x6f,%al
-   18000c5e4:	jo     0x18000c65a
-   18000c5e6:	imul   $0x56406c61,0x6e(%rdi),%ebp
-   18000c5ed:	(bad)
-   18000c5ee:	and    $0x56,%al
-   18000c5f0:	movsxd %gs:0x72(%rdi,%rbp,2),%esi
-   18000c5f5:	rex and $0x30,%al
-   18000c5f8:	xor    0x67(%rax),%al
-   18000c5fb:	outsl  %gs:(%rsi),(%dx)
-   18000c5fd:	fs gs rex
-   18000c600:	rex
-   18000c601:	rex (bad)
-   18000c603:	(bad)
-   18000c608:	rex.WB
-   18000c609:	rex pop %rdx
-   18000c60b:	add    %bl,(%rdx)
-   18000c60d:	(bad)
-   18000c60e:	(bad)
-   18000c60f:	outsb  %ds:(%rsi),(%dx)
-   18000c610:	(bad)
-   18000c611:	pop    %rdi
-   18000c612:	gs fs addr32 gs jae 0x18000c658
-   18000c618:	(bad)
-   18000c619:	and    $0x53,%al
-   18000c61b:	jne    0x18000c68f
-   18000c61d:	data16 (bad)
-   18000c61f:	movsxd 0x45(%rbp),%esp
-   18000c622:	fs addr32 gs jae 0x18000c667
-   18000c627:	and    $0x30,%al
-   18000c629:	xor    0x67(%rax),%al
-   18000c62c:	outsl  %gs:(%rsi),(%dx)
-   18000c62e:	fs gs rex
-   18000c631:	rex push %rcx
-   18000c633:	rex.RB
-   18000c634:	rex.X
-   18000c635:	rex.B
-   18000c636:	rex.WB pop %r8
-   18000c638:	pop    %rdx
-   18000c639:	add    %dl,(%rbx)
-   18000c63b:	add    $0x6764653f,%eax
-   18000c640:	gs pop %rdi
-   18000c642:	jbe    0x18000c6a9
-   18000c644:	jb     0x18000c6ba
-   18000c646:	imul   $0x243f4073,0x65(%rbx),%esp
-   18000c64d:	push   %rbx
-   18000c64e:	jne    0x18000c6c2
-   18000c650:	data16 (bad)
-   18000c652:	movsxd 0x45(%rbp),%esp
-   18000c655:	fs addr32 gs jae 0x18000c69a
-   18000c65a:	and    $0x30,%al
-   18000c65c:	xor    0x67(%rax),%al
-   18000c65f:	outsl  %gs:(%rsi),(%dx)
-   18000c661:	fs gs rex
-   18000c664:	rex push %rcx
-   18000c666:	rex.RB
-   18000c667:	rex.X
-   18000c668:	rex.B
-   18000c669:	rex.B
-   18000c66a:	rex.RB
-   18000c66b:	rex.X push %rsi
-   18000c66d:	(bad)
-   18000c66e:	and    $0x61,%al
-   18000c670:	jb     0x18000c6e4
-   18000c672:	(bad)
-   18000c673:	jns    0x18000c6b5
-   18000c675:	rex.WB and $0x30,%al
-   18000c678:	xor    %eax,0x73(%rax)
-   18000c67b:	je     0x18000c6e1
-   18000c67d:	rex
-   18000c67e:	rex
-   18000c67f:	rex.WB
-   18000c680:	rex pop %rdx
-   18000c682:	add    %al,(%rax)
-   18000c684:	rex.WRXB jo 0x18000c6ec
-   18000c687:	outsb  %ds:(%rsi),(%dx)
-   18000c688:	rex.RXB
-   18000c689:	outsl  %gs:(%rsi),(%dx)
-   18000c68b:	fs gs pop %rdi
-   18000c68e:	insl   (%dx),%es:(%rdi)
-   18000c68f:	gs jae 0x18000c6fa
-   18000c692:	cs fs insb (%dx),%es:(%rdi)
-   18000c695:	insb   (%dx),%es:(%rdi)
-   18000c696:	add    %al,(%rax)
-   18000c698:	jb     0x18000c69c
-   18000c69a:	(bad)
-   18000c69b:	jae    0x18000c702
-   18000c69d:	je     0x18000c6fe
-   18000c69f:	jo     0x18000c710
-   18000c6a1:	imul   $0x47243f40,0x74(%rsi),%ebp
-   18000c6a8:	outsb  %gs:(%rsi),(%dx)
-   18000c6aa:	gs jb  0x18000c716
-   18000c6ad:	movsxd 0x69(%rdx,%rsi,2),%edx
-   18000c6b1:	(bad)
-   18000c6b2:	outsb  %ds:(%rsi),(%dx)
-   18000c6b3:	insb   (%dx),%es:(%edi)
-   18000c6b5:	gs rex push %rsi
-   18000c6b8:	(bad)
-   18000c6b9:	and    $0x72,%al
-   18000c6bb:	gs data16 gs jb 0x18000c725
-   18000c6c0:	outsb  %ds:(%rsi),(%dx)
-   18000c6c1:	movsxd 0x5f(%rbp),%esp
-   18000c6c4:	ja     0x18000c738
-   18000c6c6:	(bad)
-   18000c6c7:	jo     0x18000c739
-   18000c6c9:	gs jb  0x18000c70c
-   18000c6cc:	and    $0x24,%al
-   18000c6ce:	rex.XB
-   18000c6cf:	rex.X push %rsi
-   18000c6d1:	(bad)
-   18000c6d2:	and    $0x50,%al
-   18000c6d4:	outsl  %ds:(%rsi),(%dx)
-   18000c6d5:	imul   $0x32302440,0x74(%rsi),%ebp
-   18000c6dc:	rex
-   18000c6dd:	outsl  %gs:(%esi),(%dx)
-   18000c6e0:	fs gs rex
-   18000c6e3:	rex
-   18000c6e4:	rex jae 0x18000c75b
-   18000c6e7:	fs rex
-   18000c6e9:	rex and $0x30,%al
-   18000c6ec:	xor    0x67(%rax),%al
-   18000c6ef:	outsl  %gs:(%rsi),(%dx)
-   18000c6f1:	fs gs rex
-   18000c6f4:	rex push %rcx
-   18000c6f6:	rex.RB
-   18000c6f7:	rex.B
-   18000c6f8:	pop    %r8
-   18000c6fa:	rex.WB push %r14
-   18000c6fc:	(bad)
-   18000c6fd:	and    $0x72,%al
-   18000c6ff:	gs data16 gs jb 0x18000c769
-   18000c704:	outsb  %ds:(%rsi),(%dx)
-   18000c705:	movsxd 0x5f(%rbp),%esp
-   18000c708:	ja     0x18000c77c
-   18000c70a:	(bad)
-   18000c70b:	jo     0x18000c77d
-   18000c70d:	gs jb  0x18000c750
-   18000c710:	and    $0x24,%al
-   18000c712:	rex.XB
-   18000c713:	rex.X push %rsi
-   18000c715:	(bad)
-   18000c716:	and    $0x50,%al
-   18000c718:	outsl  %ds:(%rsi),(%dx)
-   18000c719:	imul   $0x32302440,0x74(%rsi),%ebp
-   18000c720:	rex
-   18000c721:	outsl  %gs:(%esi),(%dx)
-   18000c724:	fs gs rex
-   18000c727:	rex
-   18000c728:	rex jae 0x18000c79f
-   18000c72b:	fs rex
-   18000c72d:	rex
-   18000c72e:	rex pop %rdx
-   18000c730:	add    %al,(%rax)
-   18000c732:	or     (%rax),%eax
-   18000c734:	(bad)
-   18000c735:	(bad)
-   18000c736:	and    $0x6e,%al
-   18000c738:	outsl  %ds:(%rsi),(%dx)
-   18000c739:	jb     0x18000c7a8
-   18000c73b:	(bad)
-   18000c73c:	insb   (%dx),%es:(%rdi)
-   18000c73d:	rex and $0x30,%al
-   18000c740:	xor    0x3f(%rax),%al
-   18000c743:	and    $0x47,%al
-   18000c745:	outsb  %gs:(%rsi),(%dx)
-   18000c747:	gs jb  0x18000c7b3
-   18000c74a:	movsxd 0x69(%rdx,%rsi,2),%edx
-   18000c74e:	(bad)
-   18000c74f:	outsb  %ds:(%rsi),(%dx)
-   18000c750:	insb   (%dx),%es:(%edi)
-   18000c752:	gs rex push %rsi
-   18000c755:	(bad)
-   18000c756:	and    $0x72,%al
-   18000c758:	gs data16 gs jb 0x18000c7c2
-   18000c75d:	outsb  %ds:(%rsi),(%dx)
-   18000c75e:	movsxd 0x5f(%rbp),%esp
-   18000c761:	ja     0x18000c7d5
-   18000c763:	(bad)
-   18000c764:	jo     0x18000c7d6
-   18000c766:	gs jb  0x18000c7a9
-   18000c769:	and    $0x24,%al
-   18000c76b:	rex.XB
-   18000c76c:	rex.X push %rsi
-   18000c76e:	(bad)
-   18000c76f:	and    $0x50,%al
-   18000c771:	outsl  %ds:(%rsi),(%dx)
-   18000c772:	imul   $0x32302440,0x74(%rsi),%ebp
-   18000c779:	rex
-   18000c77a:	outsl  %gs:(%esi),(%dx)
-   18000c77d:	fs gs rex
-   18000c780:	rex
-   18000c781:	rex jae 0x18000c7f8
-   18000c784:	fs rex
-   18000c786:	rex and $0x30,%al
-   18000c789:	xor    0x67(%rax),%al
-   18000c78c:	outsl  %gs:(%rsi),(%dx)
-   18000c78e:	fs gs rex
-   18000c791:	rex push %rcx
-   18000c793:	rex.RB
-   18000c794:	rex.X
-   18000c795:	rex.B (bad)
-   18000c797:	push   %r14
-   18000c799:	(bad)
-   18000c79a:	and    $0x6f,%al
-   18000c79c:	jo     0x18000c812
-   18000c79e:	imul   $0x56406c61,0x6e(%rdi),%ebp
+   18000c599:	and    $0x54,%al
+   18000c59b:	jb     0x18000c606
+   18000c59d:	(bad)
+   18000c59e:	outsb  %ds:(%rsi),(%dx)
+   18000c59f:	insb   (%dx),%es:(%edi)
+   18000c5a1:	gs rex and $0x30,%al
+   18000c5a5:	xor    0x32(%rax),%al
+   18000c5a8:	rex
+   18000c5a9:	rex.WB
+   18000c5aa:	rex pop %rdx
+   18000c5ac:	add    %al,(%rax)
+   18000c5ae:	push   %rcx
+   18000c5af:	add    %bh,(%rdi)
+   18000c5b1:	(bad)
+   18000c5b2:	and    $0x73,%al
+   18000c5b4:	(bad)
+   18000c5b5:	jbe    0x18000c61c
+   18000c5b7:	pop    %rdi
+   18000c5b8:	je     0x18000c62c
+   18000c5ba:	imul   $0x616c7567,0x6e(%rcx),%esp
+   18000c5c1:	je     0x18000c628
+   18000c5c3:	fs pop %rdi
+   18000c5c5:	jae    0x18000c63c
+   18000c5c7:	jb     0x18000c62f
+   18000c5c9:	(bad)
+   18000c5ca:	movsxd 0x40(%rbp),%esp
+   18000c5cd:	and    $0x30,%al
+   18000c5cf:	xor    0x67(%rax),%al
+   18000c5d2:	outsl  %gs:(%rsi),(%dx)
+   18000c5d4:	fs gs rex
+   18000c5d7:	rex pop %rcx
+   18000c5d9:	pop    %r8
+   18000c5db:	rex.B
+   18000c5dc:	rex.RB
+   18000c5dd:	rex.X push %rsi
+   18000c5df:	(bad)
+   18000c5e0:	and    $0x54,%al
+   18000c5e2:	jb     0x18000c64d
+   18000c5e4:	(bad)
+   18000c5e5:	outsb  %ds:(%rsi),(%dx)
+   18000c5e6:	addr32 jne 0x18000c655
+   18000c5e9:	(bad)
+   18000c5ea:	je     0x18000c651
+   18000c5ec:	fs push %rbx
+   18000c5ee:	jne    0x18000c662
+   18000c5f0:	data16 (bad)
+   18000c5f2:	movsxd 0x40(%rbp),%esp
+   18000c5f5:	and    $0x30,%al
+   18000c5f7:	xor    0x30(%rax),%al
+   18000c5fa:	rex push %rsi
+   18000c5fc:	jae    0x18000c672
+   18000c5fe:	jb     0x18000c669
+   18000c600:	outsb  %ds:(%rsi),(%dx)
+   18000c601:	addr32 pop %rdi
+   18000c603:	jbe    0x18000c66e
+   18000c605:	gs ja  0x18000c648
+   18000c608:	(bad)
+   18000c609:	(bad)
+   18000c60e:	rex pop %rdx
+   18000c610:	add    %al,(%rax)
+   18000c612:	cmp    $0x0,%al
+   18000c614:	(bad)
+   18000c615:	(bad)
+   18000c616:	and    $0x70,%al
+   18000c618:	outsl  %ds:(%rsi),(%dx)
+   18000c619:	insb   (%dx),%es:(%rdi)
+   18000c61a:	jns    0x18000c683
+   18000c61c:	outsl  %ds:(%rsi),(%dx)
+   18000c61d:	outsb  %ds:(%rsi),(%dx)
+   18000c61e:	pop    %rdi
+   18000c61f:	jbe    0x18000c686
+   18000c621:	jb     0x18000c697
+   18000c623:	gs js  0x18000c685
+   18000c626:	outsb  %ds:(%rsi),(%dx)
+   18000c627:	outsl  %ds:(%rsi),(%dx)
+   18000c628:	jb     0x18000c697
+   18000c62a:	(bad)
+   18000c62b:	insb   (%dx),%es:(%rdi)
+   18000c62c:	rex and $0x30,%al
+   18000c62f:	xor    0x3f(%rax),%al
+   18000c632:	and    $0x53,%al
+   18000c634:	jne    0x18000c6a8
+   18000c636:	data16 (bad)
+   18000c638:	movsxd 0x4d(%rbp),%esp
+   18000c63b:	gs jae 0x18000c6a6
+   18000c63e:	rex and $0x30,%al
+   18000c641:	xor    0x67(%rax),%al
+   18000c644:	outsl  %gs:(%rsi),(%dx)
+   18000c646:	fs gs rex
+   18000c649:	rex push %rcx
+   18000c64b:	rex.RB
+   18000c64c:	rex.X
+   18000c64d:	rex.B (bad)
+   18000c64f:	push   %r14
+   18000c651:	(bad)
+   18000c652:	and    $0x6f,%al
+   18000c654:	jo     0x18000c6ca
+   18000c656:	imul   $0x56406c61,0x6e(%rdi),%ebp
+   18000c65d:	(bad)
+   18000c65e:	and    $0x56,%al
+   18000c660:	movsxd %gs:0x72(%rdi,%rbp,2),%esi
+   18000c665:	rex and $0x30,%al
+   18000c668:	xor    0x67(%rax),%al
+   18000c66b:	outsl  %gs:(%rsi),(%dx)
+   18000c66d:	fs gs rex
+   18000c670:	rex
+   18000c671:	rex (bad)
+   18000c673:	(bad)
+   18000c678:	rex.WB
+   18000c679:	rex pop %rdx
+   18000c67b:	add    %al,0x6(%rsi)
+   18000c67e:	(bad)
+   18000c67f:	outsb  %ds:(%rsi),(%dx)
+   18000c680:	(bad)
+   18000c681:	pop    %rdi
+   18000c682:	gs fs addr32 gs jae 0x18000c6c8
+   18000c688:	(bad)
+   18000c689:	and    $0x53,%al
+   18000c68b:	jne    0x18000c6ff
+   18000c68d:	data16 (bad)
+   18000c68f:	movsxd 0x45(%rbp),%esp
+   18000c692:	fs addr32 gs jae 0x18000c6d7
+   18000c697:	and    $0x30,%al
+   18000c699:	xor    0x67(%rax),%al
+   18000c69c:	outsl  %gs:(%rsi),(%dx)
+   18000c69e:	fs gs rex
+   18000c6a1:	rex push %rcx
+   18000c6a3:	rex.RB
+   18000c6a4:	rex.X
+   18000c6a5:	rex.B
+   18000c6a6:	rex.WB pop %r8
+   18000c6a8:	pop    %rdx
+   18000c6a9:	add    %bh,(%rdi)
+   18000c6ab:	add    $0x6764653f,%eax
+   18000c6b0:	gs pop %rdi
+   18000c6b2:	jbe    0x18000c719
+   18000c6b4:	jb     0x18000c72a
+   18000c6b6:	imul   $0x243f4073,0x65(%rbx),%esp
+   18000c6bd:	push   %rbx
+   18000c6be:	jne    0x18000c732
+   18000c6c0:	data16 (bad)
+   18000c6c2:	movsxd 0x45(%rbp),%esp
+   18000c6c5:	fs addr32 gs jae 0x18000c70a
+   18000c6ca:	and    $0x30,%al
+   18000c6cc:	xor    0x67(%rax),%al
+   18000c6cf:	outsl  %gs:(%rsi),(%dx)
+   18000c6d1:	fs gs rex
+   18000c6d4:	rex push %rcx
+   18000c6d6:	rex.RB
+   18000c6d7:	rex.X
+   18000c6d8:	rex.B
+   18000c6d9:	rex.B
+   18000c6da:	rex.RB
+   18000c6db:	rex.X push %rsi
+   18000c6dd:	(bad)
+   18000c6de:	and    $0x61,%al
+   18000c6e0:	jb     0x18000c754
+   18000c6e2:	(bad)
+   18000c6e3:	jns    0x18000c725
+   18000c6e5:	rex.WB and $0x30,%al
+   18000c6e8:	xor    %eax,0x73(%rax)
+   18000c6eb:	je     0x18000c751
+   18000c6ed:	rex
+   18000c6ee:	rex
+   18000c6ef:	rex.WB
+   18000c6f0:	rex pop %rdx
+   18000c6f2:	add    %al,(%rax)
+   18000c6f4:	rex.WRXB jo 0x18000c75c
+   18000c6f7:	outsb  %ds:(%rsi),(%dx)
+   18000c6f8:	rex.RXB
+   18000c6f9:	outsl  %gs:(%rsi),(%dx)
+   18000c6fb:	fs gs pop %rdi
+   18000c6fe:	insl   (%dx),%es:(%rdi)
+   18000c6ff:	gs jae 0x18000c76a
+   18000c702:	cs fs insb (%dx),%es:(%rdi)
+   18000c705:	insb   (%dx),%es:(%rdi)
+   18000c706:	add    %al,(%rax)
+   18000c708:	lods   %ds:(%rsi),%eax
+   18000c709:	add    (%rdi),%bh
+   18000c70b:	jae    0x18000c772
+   18000c70d:	je     0x18000c76e
+   18000c70f:	jo     0x18000c780
+   18000c711:	imul   $0x47243f40,0x74(%rsi),%ebp
+   18000c718:	outsb  %gs:(%rsi),(%dx)
+   18000c71a:	gs jb  0x18000c786
+   18000c71d:	movsxd 0x69(%rdx,%rsi,2),%edx
+   18000c721:	(bad)
+   18000c722:	outsb  %ds:(%rsi),(%dx)
+   18000c723:	insb   (%dx),%es:(%edi)
+   18000c725:	gs rex push %rsi
+   18000c728:	(bad)
+   18000c729:	and    $0x72,%al
+   18000c72b:	gs data16 gs jb 0x18000c795
+   18000c730:	outsb  %ds:(%rsi),(%dx)
+   18000c731:	movsxd 0x5f(%rbp),%esp
+   18000c734:	ja     0x18000c7a8
+   18000c736:	(bad)
+   18000c737:	jo     0x18000c7a9
+   18000c739:	gs jb  0x18000c77c
+   18000c73c:	and    $0x24,%al
+   18000c73e:	rex.XB
+   18000c73f:	rex.X push %rsi
+   18000c741:	(bad)
+   18000c742:	and    $0x50,%al
+   18000c744:	outsl  %ds:(%rsi),(%dx)
+   18000c745:	imul   $0x32302440,0x74(%rsi),%ebp
+   18000c74c:	rex
+   18000c74d:	outsl  %gs:(%esi),(%dx)
+   18000c750:	fs gs rex
+   18000c753:	rex
+   18000c754:	rex jae 0x18000c7cb
+   18000c757:	fs rex
+   18000c759:	rex and $0x30,%al
+   18000c75c:	xor    0x67(%rax),%al
+   18000c75f:	outsl  %gs:(%rsi),(%dx)
+   18000c761:	fs gs rex
+   18000c764:	rex push %rcx
+   18000c766:	rex.RB
+   18000c767:	rex.B
+   18000c768:	pop    %r8
+   18000c76a:	rex.WB push %r14
+   18000c76c:	(bad)
+   18000c76d:	and    $0x72,%al
+   18000c76f:	gs data16 gs jb 0x18000c7d9
+   18000c774:	outsb  %ds:(%rsi),(%dx)
+   18000c775:	movsxd 0x5f(%rbp),%esp
+   18000c778:	ja     0x18000c7ec
+   18000c77a:	(bad)
+   18000c77b:	jo     0x18000c7ed
+   18000c77d:	gs jb  0x18000c7c0
+   18000c780:	and    $0x24,%al
+   18000c782:	rex.XB
+   18000c783:	rex.X push %rsi
+   18000c785:	(bad)
+   18000c786:	and    $0x50,%al
+   18000c788:	outsl  %ds:(%rsi),(%dx)
+   18000c789:	imul   $0x32302440,0x74(%rsi),%ebp
+   18000c790:	rex
+   18000c791:	outsl  %gs:(%esi),(%dx)
+   18000c794:	fs gs rex
+   18000c797:	rex
+   18000c798:	rex jae 0x18000c80f
+   18000c79b:	fs rex
+   18000c79d:	rex
+   18000c79e:	rex pop %rdx
+   18000c7a0:	add    %al,(%rax)
+   18000c7a2:	or     (%rax),%eax
+   18000c7a4:	(bad)
    18000c7a5:	(bad)
-   18000c7a6:	and    $0x56,%al
-   18000c7a8:	movsxd %gs:0x72(%rdi,%rbp,2),%esi
+   18000c7a6:	and    $0x6e,%al
+   18000c7a8:	outsl  %ds:(%rsi),(%dx)
+   18000c7a9:	jb     0x18000c818
+   18000c7ab:	(bad)
+   18000c7ac:	insb   (%dx),%es:(%rdi)
    18000c7ad:	rex and $0x30,%al
-   18000c7b0:	xor    0x67(%rax),%al
-   18000c7b3:	outsl  %gs:(%rsi),(%dx)
-   18000c7b5:	fs gs rex
-   18000c7b8:	rex
-   18000c7b9:	rex (bad)
-   18000c7bb:	(bad)
-   18000c7c0:	pop    %rax
-   18000c7c1:	pop    %rdx
-   18000c7c2:	add    %al,(%rax)
-   18000c7c4:	rex.WRXB jo 0x18000c82c
-   18000c7c7:	outsb  %ds:(%rsi),(%dx)
-   18000c7c8:	rex.RXB
-   18000c7c9:	outsl  %gs:(%rsi),(%dx)
-   18000c7cb:	fs gs pop %rdi
-   18000c7ce:	outsl  %gs:(%esi),(%dx)
-   18000c7d1:	insl   (%dx),%es:(%rdi)
-   18000c7d2:	gs je  0x18000c847
-   18000c7d5:	jns    0x18000c805
-   18000c7d7:	fs insb (%dx),%es:(%rdi)
-   18000c7d9:	insb   (%dx),%es:(%rdi)
-   18000c7da:	add    %al,(%rax)
-   18000c7dc:	rolb   $0x3f,(%rax)
-   18000c7df:	jae    0x18000c846
-   18000c7e1:	je     0x18000c842
-   18000c7e3:	imul   $0x636e6174,0x73(%rsi),%ebp
-   18000c7ea:	gs rex push %rbx
-   18000c7ed:	imul   $0x6f74656c,0x67(%rsi),%ebp
-   18000c7f4:	outsb  %ds:(%rsi),(%dx)
-   18000c7f5:	rex
-   18000c7f6:	outsl  %gs:(%esi),(%dx)
-   18000c7f9:	fs gs rex
-   18000c7fc:	rex
-   18000c7fd:	rex.XB
-   18000c7fe:	pop    %r8
-   18000c800:	rex.B
-   18000c801:	rex.RB
-   18000c802:	rex.X push %rsi
-   18000c804:	je     0x18000c87f
-   18000c806:	jo     0x18000c86d
-   18000c808:	pop    %rdi
-   18000c809:	imul   $0x5040406f,0x66(%rsi),%ebp
-   18000c810:	rex.RB
-   18000c811:	push   %r14
-   18000c813:	xor    %esi,(%rdx)
-   18000c815:	rex
-   18000c816:	rex pop %rdx
-   18000c818:	add    %al,(%rax)
-   18000c81a:	mov    %es,(%rax)
-   18000c81c:	(bad)
-   18000c81d:	imul   $0x636e6174,0x73(%rsi),%ebp
-   18000c824:	gs rex push %rbx
-   18000c827:	imul   $0x6f74656c,0x67(%rsi),%ebp
-   18000c82e:	outsb  %ds:(%rsi),(%dx)
-   18000c82f:	rex
-   18000c830:	outsl  %gs:(%esi),(%dx)
-   18000c833:	fs gs rex
-   18000c836:	rex
-   18000c837:	rex.XB
-   18000c838:	push   %r8
-   18000c83a:	rex.RB
-   18000c83b:	push   %r14
-   18000c83d:	xor    %esi,(%rdx)
-   18000c83f:	rex
-   18000c840:	rex.B
-   18000c841:	rex.RB
-   18000c842:	rex.X push %rsi
-   18000c844:	je     0x18000c8bf
-   18000c846:	jo     0x18000c8ad
-   18000c848:	pop    %rdi
-   18000c849:	imul   $0x4040406f,0x66(%rsi),%ebp
-   18000c850:	pop    %rdx
-   18000c851:	add    %dh,(%rcx)
-   18000c853:	add    %bh,(%rdi)
-   18000c855:	(bad)
-   18000c856:	xor    %ecx,0x62(%rcx,%rbp,2)
-   18000c85a:	jb     0x18000c8bd
-   18000c85c:	jb     0x18000c8d7
-   18000c85e:	rex
-   18000c85f:	outsl  %gs:(%esi),(%dx)
-   18000c862:	fs gs rex
-   18000c865:	rex push %rbp
-   18000c867:	rex.RB
-   18000c868:	rex.B
-   18000c869:	rex.B
-   18000c86a:	rex pop %rax
-   18000c86c:	pop    %rdx
-   18000c86d:	add    %bl,(%rdx)
-   18000c86f:	add    %bh,(%rdi)
-   18000c871:	(bad)
-   18000c872:	xor    %cl,0x62(%rcx,%rbp,2)
-   18000c876:	jb     0x18000c8d9
-   18000c878:	jb     0x18000c8f3
-   18000c87a:	rex
-   18000c87b:	outsl  %gs:(%esi),(%dx)
-   18000c87e:	fs gs rex
-   18000c881:	rex
-   18000c882:	rex.WB
-   18000c883:	rex.RB
-   18000c884:	rex.B
-   18000c885:	rex.B
-   18000c886:	rex pop %rax
-   18000c888:	pop    %rdx
-   18000c889:	add    %bl,0x0(%rcx)
+   18000c7b0:	xor    0x3f(%rax),%al
+   18000c7b3:	and    $0x47,%al
+   18000c7b5:	outsb  %gs:(%rsi),(%dx)
+   18000c7b7:	gs jb  0x18000c823
+   18000c7ba:	movsxd 0x69(%rdx,%rsi,2),%edx
+   18000c7be:	(bad)
+   18000c7bf:	outsb  %ds:(%rsi),(%dx)
+   18000c7c0:	insb   (%dx),%es:(%edi)
+   18000c7c2:	gs rex push %rsi
+   18000c7c5:	(bad)
+   18000c7c6:	and    $0x72,%al
+   18000c7c8:	gs data16 gs jb 0x18000c832
+   18000c7cd:	outsb  %ds:(%rsi),(%dx)
+   18000c7ce:	movsxd 0x5f(%rbp),%esp
+   18000c7d1:	ja     0x18000c845
+   18000c7d3:	(bad)
+   18000c7d4:	jo     0x18000c846
+   18000c7d6:	gs jb  0x18000c819
+   18000c7d9:	and    $0x24,%al
+   18000c7db:	rex.XB
+   18000c7dc:	rex.X push %rsi
+   18000c7de:	(bad)
+   18000c7df:	and    $0x50,%al
+   18000c7e1:	outsl  %ds:(%rsi),(%dx)
+   18000c7e2:	imul   $0x32302440,0x74(%rsi),%ebp
+   18000c7e9:	rex
+   18000c7ea:	outsl  %gs:(%esi),(%dx)
+   18000c7ed:	fs gs rex
+   18000c7f0:	rex
+   18000c7f1:	rex jae 0x18000c868
+   18000c7f4:	fs rex
+   18000c7f6:	rex and $0x30,%al
+   18000c7f9:	xor    0x67(%rax),%al
+   18000c7fc:	outsl  %gs:(%rsi),(%dx)
+   18000c7fe:	fs gs rex
+   18000c801:	rex push %rcx
+   18000c803:	rex.RB
+   18000c804:	rex.X
+   18000c805:	rex.B (bad)
+   18000c807:	push   %r14
+   18000c809:	(bad)
+   18000c80a:	and    $0x6f,%al
+   18000c80c:	jo     0x18000c882
+   18000c80e:	imul   $0x56406c61,0x6e(%rdi),%ebp
+   18000c815:	(bad)
+   18000c816:	and    $0x56,%al
+   18000c818:	movsxd %gs:0x72(%rdi,%rbp,2),%esi
+   18000c81d:	rex and $0x30,%al
+   18000c820:	xor    0x67(%rax),%al
+   18000c823:	outsl  %gs:(%rsi),(%dx)
+   18000c825:	fs gs rex
+   18000c828:	rex
+   18000c829:	rex (bad)
+   18000c82b:	(bad)
+   18000c830:	pop    %rax
+   18000c831:	pop    %rdx
+   18000c832:	add    %al,(%rax)
+   18000c834:	rex.WRXB jo 0x18000c89c
+   18000c837:	outsb  %ds:(%rsi),(%dx)
+   18000c838:	rex.RXB
+   18000c839:	outsl  %gs:(%rsi),(%dx)
+   18000c83b:	fs gs pop %rdi
+   18000c83e:	outsl  %gs:(%esi),(%dx)
+   18000c841:	insl   (%dx),%es:(%rdi)
+   18000c842:	gs je  0x18000c8b7
+   18000c845:	jns    0x18000c875
+   18000c847:	fs insb (%dx),%es:(%rdi)
+   18000c849:	insb   (%dx),%es:(%rdi)
+   18000c84a:	add    %al,(%rax)
+   18000c84c:	movl   $0x7465733f,(%rax)
+   18000c852:	pop    %rdi
+   18000c853:	imul   $0x636e6174,0x73(%rsi),%ebp
+   18000c85a:	gs rex push %rbx
+   18000c85d:	imul   $0x6f74656c,0x67(%rsi),%ebp
+   18000c864:	outsb  %ds:(%rsi),(%dx)
+   18000c865:	rex
+   18000c866:	outsl  %gs:(%esi),(%dx)
+   18000c869:	fs gs rex
+   18000c86c:	rex
+   18000c86d:	rex.XB
+   18000c86e:	pop    %r8
+   18000c870:	rex.B
+   18000c871:	rex.RB
+   18000c872:	rex.X push %rsi
+   18000c874:	je     0x18000c8ef
+   18000c876:	jo     0x18000c8dd
+   18000c878:	pop    %rdi
+   18000c879:	imul   $0x5040406f,0x66(%rsi),%ebp
+   18000c880:	rex.RB
+   18000c881:	push   %r14
+   18000c883:	xor    %esi,(%rdx)
+   18000c885:	rex
+   18000c886:	rex pop %rdx
+   18000c888:	add    %al,(%rax)
+   18000c88a:	pop    (%rax)
    18000c88c:	(bad)
-   18000c88d:	movsxd 0x6c(%rcx),%esp
-   18000c890:	insb   (%dx),%es:(%rdi)
-   18000c891:	pop    %rdi
-   18000c892:	imul   $0x6c616974,0x69(%rsi),%ebp
-   18000c899:	imul   $0x62694c40,0x65(%rdx),%edi
-   18000c8a0:	jb     0x18000c903
-   18000c8a2:	jb     0x18000c91d
-   18000c8a4:	rex
-   18000c8a5:	outsl  %gs:(%esi),(%dx)
-   18000c8a8:	fs gs rex
-   18000c8ab:	rex
-   18000c8ac:	rex.WB
-   18000c8ad:	rex.RB
-   18000c8ae:	rex.B
-   18000c8af:	pop    %r8
-   18000c8b1:	push   %rax
-   18000c8b2:	rex.RB
-   18000c8b3:	rex.X
-   18000c8b4:	rex.R
-   18000c8b5:	rex pop %rdx
-   18000c8b7:	add    %dl,0x6f6c3f00(%rbp)
-   18000c8bd:	addr32 pop %rdi
-   18000c8bf:	(bad)
-   18000c8c6:	outsl  %ds:(%rsi),(%dx)
-   18000c8c7:	addr32 addr32 gs jb 0x18000c90c
-   18000c8cc:	outsl  %gs:(%esi),(%dx)
-   18000c8cf:	fs gs rex
-   18000c8d2:	rex
-   18000c8d3:	rex.XB
-   18000c8d4:	pop    %r8
-   18000c8d6:	rex.B
+   18000c88d:	imul   $0x636e6174,0x73(%rsi),%ebp
+   18000c894:	gs rex push %rbx
+   18000c897:	imul   $0x6f74656c,0x67(%rsi),%ebp
+   18000c89e:	outsb  %ds:(%rsi),(%dx)
+   18000c89f:	rex
+   18000c8a0:	outsl  %gs:(%esi),(%dx)
+   18000c8a3:	fs gs rex
+   18000c8a6:	rex
+   18000c8a7:	rex.XB
+   18000c8a8:	push   %r8
+   18000c8aa:	rex.RB
+   18000c8ab:	push   %r14
+   18000c8ad:	xor    %esi,(%rdx)
+   18000c8af:	rex
+   18000c8b0:	rex.B
+   18000c8b1:	rex.RB
+   18000c8b2:	rex.X push %rsi
+   18000c8b4:	je     0x18000c92f
+   18000c8b6:	jo     0x18000c91d
+   18000c8b8:	pop    %rdi
+   18000c8b9:	imul   $0x4040406f,0x66(%rsi),%ebp
+   18000c8c0:	pop    %rdx
+   18000c8c1:	add    %dh,(%rcx)
+   18000c8c3:	add    %bh,(%rdi)
+   18000c8c5:	(bad)
+   18000c8c6:	xor    %ecx,0x62(%rcx,%rbp,2)
+   18000c8ca:	jb     0x18000c92d
+   18000c8cc:	jb     0x18000c947
+   18000c8ce:	rex
+   18000c8cf:	outsl  %gs:(%esi),(%dx)
+   18000c8d2:	fs gs rex
+   18000c8d5:	rex push %rbp
    18000c8d7:	rex.RB
-   18000c8d8:	rex.X push %rsi
-   18000c8da:	(bad)
-   18000c8db:	and    $0x62,%al
-   18000c8dd:	(bad)
-   18000c8de:	jae    0x18000c949
-   18000c8e0:	movsxd 0x73(%rdi),%ebx
-   18000c8e3:	je     0x18000c957
-   18000c8e5:	imul   $0x3f554440,0x67(%rsi),%ebp
-   18000c8ec:	and    $0x63,%al
-   18000c8ee:	push   $0x745f7261
-   18000c8f3:	jb     0x18000c956
-   18000c8f5:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000c8fd:	fs rex
-   18000c8ff:	rex push %rsi
-   18000c901:	(bad)
-   18000c902:	and    $0x61,%al
-   18000c904:	insb   (%dx),%es:(%rdi)
-   18000c905:	insb   (%dx),%es:(%rdi)
-   18000c906:	outsl  %ds:(%rsi),(%dx)
-   18000c907:	movsxd 0x74(%rcx),%esp
-   18000c90a:	outsl  %ds:(%rsi),(%dx)
-   18000c90b:	jb     0x18000c94d
-   18000c90d:	rex.R
-   18000c90e:	rex xor 0x40(%rax),%al
-   18000c912:	jae    0x18000c988
-   18000c914:	fs rex
-   18000c916:	rex
-   18000c917:	rex pop %rdx
-   18000c919:	add    %ah,0x0(%rsi)
-   18000c91c:	(bad)
-   18000c91d:	fs gs insb (%dx),%es:(%rdi)
-   18000c920:	gs je  0x18000c988
-   18000c923:	pop    %rdi
-   18000c924:	(bad)
-   18000c925:	je     0x18000c99b
-   18000c927:	jb     0x18000c992
-   18000c929:	(bad)
-   18000c92e:	rex.B je 0x18000c9a5
-   18000c931:	jb     0x18000c99c
-   18000c933:	(bad)
-   18000c938:	(bad)
-   18000c939:	outsb  %ds:(%rsi),(%dx)
-   18000c93a:	(bad)
-   18000c93b:	addr32 gs jb 0x18000c97f
-   18000c93f:	outsl  %gs:(%esi),(%dx)
-   18000c942:	fs gs rex
-   18000c945:	rex push %rcx
+   18000c8d8:	rex.B
+   18000c8d9:	rex.B
+   18000c8da:	rex pop %rax
+   18000c8dc:	pop    %rdx
+   18000c8dd:	add    %bl,(%rdx)
+   18000c8df:	add    %bh,(%rdi)
+   18000c8e1:	(bad)
+   18000c8e2:	xor    %cl,0x62(%rcx,%rbp,2)
+   18000c8e6:	jb     0x18000c949
+   18000c8e8:	jb     0x18000c963
+   18000c8ea:	rex
+   18000c8eb:	outsl  %gs:(%esi),(%dx)
+   18000c8ee:	fs gs rex
+   18000c8f1:	rex
+   18000c8f2:	rex.WB
+   18000c8f3:	rex.RB
+   18000c8f4:	rex.B
+   18000c8f5:	rex.B
+   18000c8f6:	rex pop %rax
+   18000c8f8:	pop    %rdx
+   18000c8f9:	add    %bl,0x0(%rbx)
+   18000c8fc:	(bad)
+   18000c8fd:	movsxd 0x6c(%rcx),%esp
+   18000c900:	insb   (%dx),%es:(%rdi)
+   18000c901:	pop    %rdi
+   18000c902:	imul   $0x6c616974,0x69(%rsi),%ebp
+   18000c909:	imul   $0x62694c40,0x65(%rdx),%edi
+   18000c910:	jb     0x18000c973
+   18000c912:	jb     0x18000c98d
+   18000c914:	rex
+   18000c915:	outsl  %gs:(%esi),(%dx)
+   18000c918:	fs gs rex
+   18000c91b:	rex
+   18000c91c:	rex.WB
+   18000c91d:	rex.RB
+   18000c91e:	rex.B
+   18000c91f:	pop    %r8
+   18000c921:	push   %rax
+   18000c922:	rex.RB
+   18000c923:	rex.X
+   18000c924:	rex.R
+   18000c925:	rex pop %rdx
+   18000c927:	add    %bl,0x6f6c3f00(%rax)
+   18000c92d:	addr32 pop %rdi
+   18000c92f:	(bad)
+   18000c936:	outsl  %ds:(%rsi),(%dx)
+   18000c937:	addr32 addr32 gs jb 0x18000c97c
+   18000c93c:	outsl  %gs:(%esi),(%dx)
+   18000c93f:	fs gs rex
+   18000c942:	rex
+   18000c943:	rex.XB
+   18000c944:	pop    %r8
+   18000c946:	rex.B
    18000c947:	rex.RB
-   18000c948:	rex.B
-   18000c949:	pop    %r8
-   18000c94b:	push   %rsi
-   18000c94c:	jae    0x18000c9c2
-   18000c94e:	jb     0x18000c9b9
-   18000c950:	outsb  %ds:(%rsi),(%dx)
-   18000c951:	addr32 pop %rdi
-   18000c953:	jbe    0x18000c9be
-   18000c955:	gs ja  0x18000c998
-   18000c958:	(bad)
-   18000c959:	(bad)
-   18000c95e:	rex pop %rdx
-   18000c960:	add    %al,(%rax)
-   18000c962:	jns    0x18000c964
-   18000c964:	(bad)
-   18000c965:	imul   $0x615f,0x64(%rsi),%bp
-   18000c96b:	je     0x18000c9e1
-   18000c96d:	jb     0x18000c9d8
-   18000c96f:	(bad)
-   18000c974:	(bad)
-   18000c976:	jae    0x18000c9dd
-   18000c978:	rex
-   18000c979:	rex.B je 0x18000c9f0
-   18000c97c:	jb     0x18000c9e7
-   18000c97e:	(bad)
-   18000c983:	(bad)
-   18000c984:	outsb  %ds:(%rsi),(%dx)
-   18000c985:	(bad)
-   18000c986:	addr32 gs jb 0x18000c9ca
-   18000c98a:	outsl  %gs:(%esi),(%dx)
-   18000c98d:	fs gs rex
-   18000c990:	rex
-   18000c991:	rex.B
-   18000c992:	rex.RB
-   18000c993:	rex.X
-   18000c994:	rex.B (bad)
-   18000c996:	push   %r14
-   18000c998:	(bad)
-   18000c999:	and    $0x73,%al
-   18000c99b:	push   $0x64657261
-   18000c9a0:	pop    %rdi
-   18000c9a1:	jo     0x18000ca17
-   18000c9a3:	jb     0x18000c9e5
-   18000c9a5:	push   %rsi
-   18000c9a6:	rex.B je 0x18000ca1d
-   18000c9a9:	jb     0x18000ca14
-   18000c9ab:	(bad)
-   18000c9b0:	(bad)
-   18000c9b1:	jae    0x18000ca18
-   18000c9b3:	rex
-   18000c9b4:	outsl  %gs:(%esi),(%dx)
-   18000c9b7:	fs gs rex
-   18000c9ba:	rex
-   18000c9bb:	rex jae 0x18000ca32
-   18000c9be:	fs rex
-   18000c9c0:	rex push %rsi
-   18000c9c2:	jae    0x18000ca38
-   18000c9c4:	jb     0x18000ca2f
-   18000c9c6:	outsb  %ds:(%rsi),(%dx)
-   18000c9c7:	addr32 pop %rdi
-   18000c9c9:	jbe    0x18000ca34
-   18000c9cb:	gs ja  0x18000ca0e
-   18000c9ce:	(bad)
-   18000c9cf:	(bad)
-   18000c9d4:	rex pop %rdx
-   18000c9d6:	add    %al,(%rax)
-   18000c9d8:	mov    $0x0,%al
-   18000c9da:	(bad)
-   18000c9db:	jb     0x18000ca42
-   18000c9dd:	imul   $0x615f7265,0x74(%ebx),%esi
-   18000c9e5:	je     0x18000ca5b
-   18000c9e7:	jb     0x18000ca52
-   18000c9e9:	(bad)
-   18000c9ee:	rex.B je 0x18000ca65
-   18000c9f1:	jb     0x18000ca5c
+   18000c948:	rex.X push %rsi
+   18000c94a:	(bad)
+   18000c94b:	and    $0x62,%al
+   18000c94d:	(bad)
+   18000c94e:	jae    0x18000c9b9
+   18000c950:	movsxd 0x73(%rdi),%ebx
+   18000c953:	je     0x18000c9c7
+   18000c955:	imul   $0x3f554440,0x67(%rsi),%ebp
+   18000c95c:	and    $0x63,%al
+   18000c95e:	push   $0x745f7261
+   18000c963:	jb     0x18000c9c6
+   18000c965:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000c96d:	fs rex
+   18000c96f:	rex push %rsi
+   18000c971:	(bad)
+   18000c972:	and    $0x61,%al
+   18000c974:	insb   (%dx),%es:(%rdi)
+   18000c975:	insb   (%dx),%es:(%rdi)
+   18000c976:	outsl  %ds:(%rsi),(%dx)
+   18000c977:	movsxd 0x74(%rcx),%esp
+   18000c97a:	outsl  %ds:(%rsi),(%dx)
+   18000c97b:	jb     0x18000c9bd
+   18000c97d:	rex.R
+   18000c97e:	rex xor 0x40(%rax),%al
+   18000c982:	jae    0x18000c9f8
+   18000c984:	fs rex
+   18000c986:	rex
+   18000c987:	rex pop %rdx
+   18000c989:	add    %ch,0x0(%rax)
+   18000c98c:	(bad)
+   18000c98d:	fs gs insb (%dx),%es:(%rdi)
+   18000c990:	gs je  0x18000c9f8
+   18000c993:	pop    %rdi
+   18000c994:	(bad)
+   18000c995:	je     0x18000ca0b
+   18000c997:	jb     0x18000ca02
+   18000c999:	(bad)
+   18000c99e:	rex.B je 0x18000ca15
+   18000c9a1:	jb     0x18000ca0c
+   18000c9a3:	(bad)
+   18000c9a8:	(bad)
+   18000c9a9:	outsb  %ds:(%rsi),(%dx)
+   18000c9aa:	(bad)
+   18000c9ab:	addr32 gs jb 0x18000c9ef
+   18000c9af:	outsl  %gs:(%esi),(%dx)
+   18000c9b2:	fs gs rex
+   18000c9b5:	rex push %rcx
+   18000c9b7:	rex.RB
+   18000c9b8:	rex.B
+   18000c9b9:	pop    %r8
+   18000c9bb:	push   %rsi
+   18000c9bc:	jae    0x18000ca32
+   18000c9be:	jb     0x18000ca29
+   18000c9c0:	outsb  %ds:(%rsi),(%dx)
+   18000c9c1:	addr32 pop %rdi
+   18000c9c3:	jbe    0x18000ca2e
+   18000c9c5:	gs ja  0x18000ca08
+   18000c9c8:	(bad)
+   18000c9c9:	(bad)
+   18000c9ce:	rex pop %rdx
+   18000c9d0:	add    %al,(%rax)
+   18000c9d2:	jnp    0x18000c9d4
+   18000c9d4:	(bad)
+   18000c9d5:	imul   $0x615f,0x64(%rsi),%bp
+   18000c9db:	je     0x18000ca51
+   18000c9dd:	jb     0x18000ca48
+   18000c9df:	(bad)
+   18000c9e4:	(bad)
+   18000c9e6:	jae    0x18000ca4d
+   18000c9e8:	rex
+   18000c9e9:	rex.B je 0x18000ca60
+   18000c9ec:	jb     0x18000ca57
+   18000c9ee:	(bad)
    18000c9f3:	(bad)
-   18000c9f8:	(bad)
-   18000c9f9:	outsb  %ds:(%rsi),(%dx)
-   18000c9fa:	(bad)
-   18000c9fb:	addr32 gs jb 0x18000ca3f
-   18000c9ff:	outsl  %gs:(%esi),(%dx)
-   18000ca02:	fs gs rex
-   18000ca05:	rex
-   18000ca06:	rex.B
-   18000ca07:	rex.RB
-   18000ca08:	rex.B
-   18000ca09:	pop    %r8
-   18000ca0b:	push   %rsi
-   18000ca0c:	(bad)
-   18000ca0d:	and    $0x73,%al
-   18000ca0f:	push   $0x64657261
-   18000ca14:	pop    %rdi
-   18000ca15:	jo     0x18000ca8b
-   18000ca17:	jb     0x18000ca59
-   18000ca19:	push   %rsi
-   18000ca1a:	rex.B je 0x18000ca91
-   18000ca1d:	jb     0x18000ca88
-   18000ca1f:	(bad)
-   18000ca24:	(bad)
-   18000ca25:	jae    0x18000ca8c
-   18000ca27:	rex
-   18000ca28:	outsl  %gs:(%esi),(%dx)
-   18000ca2b:	fs gs rex
-   18000ca2e:	rex
-   18000ca2f:	rex jae 0x18000caa6
-   18000ca32:	fs rex
-   18000ca34:	rex push %rsi
-   18000ca36:	jae    0x18000caac
-   18000ca38:	jb     0x18000caa3
-   18000ca3a:	outsb  %ds:(%rsi),(%dx)
-   18000ca3b:	addr32 pop %rdi
-   18000ca3d:	jbe    0x18000caa8
-   18000ca3f:	gs ja  0x18000ca82
-   18000ca42:	(bad)
-   18000ca43:	(bad)
-   18000ca48:	rex pop %rdx
-   18000ca4a:	add    %al,(%rax)
-   18000ca4c:	rex.WRXB jo 0x18000cab4
-   18000ca4f:	outsb  %ds:(%rsi),(%dx)
-   18000ca50:	rex.RXB
-   18000ca51:	outsl  %gs:(%rsi),(%dx)
-   18000ca53:	fs gs pop %rdi
-   18000ca56:	(bad)
-   18000ca58:	jae    0x18000cac3
-   18000ca5a:	movsxd (%rsi),%ebp
-   18000ca5c:	fs insb (%dx),%es:(%rdi)
-   18000ca5e:	insb   (%dx),%es:(%rdi)
-   18000ca5f:	add    %ch,(%rdx)
-   18000ca61:	add    %edi,(%rdi)
-   18000ca63:	rex.RX (bad)
-   18000ca65:	jae    0x18000cadb
-   18000ca67:	rex.WB outsb %ds:(%rsi),(%dx)
-   18000ca69:	je     0x18000cabf
-   18000ca6b:	outsl  %ds:(%rsi),(%dx)
-   18000ca6c:	rex.X jne 0x18000cad5
-   18000ca6f:	data16 gs jb 0x18000cab3
-   18000ca73:	outsb  %ds:(%rsi),(%dx)
-   18000ca74:	jne    0x18000cae3
-   18000ca76:	(bad)
-   18000ca78:	jb     0x18000caed
-   18000ca7a:	pop    %rdi
-   18000ca7b:	imul   $0x616e7265,0x74(%rsi),%ebp
-   18000ca82:	insb   (%dx),%es:(%rdi)
-   18000ca83:	rex (bad)
-   18000ca85:	(bad)
-   18000ca8a:	pop    %rcx
-   18000ca8b:	push   %r8
-   18000ca8d:	rex.RB
-   18000ca8e:	rex.B
-   18000ca8f:	rex.R
-   18000ca90:	rex.WB push %r8
-   18000ca92:	rex.RB
-   18000ca93:	rex.B
-   18000ca94:	rex.R
-   18000ca95:	rex pop %rdx
-   18000ca97:	add    %bl,0x1(%rbx)
-   18000ca9a:	(bad)
-   18000ca9b:	push   %rbx
-   18000ca9c:	je     0x18000cb10
-   18000ca9e:	rex.XB (bad)
-   18000caa0:	je     0x18000cae2
-   18000caa2:	(bad)
-   18000caa3:	(bad)
-   18000caa8:	pop    %rcx
-   18000caa9:	rex.B (bad)
-   18000caab:	push   %r14
-   18000caad:	(bad)
-   18000caae:	and    $0x62,%al
-   18000cab0:	(bad)
-   18000cab1:	jae    0x18000cb1c
-   18000cab3:	movsxd 0x73(%rdi),%ebx
-   18000cab6:	je     0x18000cb2a
-   18000cab8:	imul   $0x3f554440,0x67(%rsi),%ebp
-   18000cabf:	and    $0x63,%al
-   18000cac1:	push   $0x745f7261
-   18000cac6:	jb     0x18000cb29
-   18000cac8:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000cad0:	fs rex
-   18000cad2:	rex push %rsi
-   18000cad4:	(bad)
-   18000cad5:	and    $0x61,%al
-   18000cad7:	insb   (%dx),%es:(%rdi)
-   18000cad8:	insb   (%dx),%es:(%rdi)
-   18000cad9:	outsl  %ds:(%rsi),(%dx)
-   18000cada:	movsxd 0x74(%rcx),%esp
-   18000cadd:	outsl  %ds:(%rsi),(%dx)
-   18000cade:	jb     0x18000cb20
-   18000cae0:	rex.R
-   18000cae1:	rex xor 0x40(%rax),%al
-   18000cae5:	jae    0x18000cb5b
-   18000cae7:	fs rex
-   18000cae9:	rex
-   18000caea:	rex.B
-   18000caeb:	rex.RB
-   18000caec:	rex.X push %rsi
-   18000caee:	rex.B insb (%dx),%es:(%rdi)
-   18000caf0:	jo     0x18000cb5a
-   18000caf2:	(bad)
-   18000caf3:	rex.WRX jne 0x18000cb63
-   18000caf6:	rex xor %eax,0x30(%rax)
-   18000cafa:	xor    %al,0x5a(%rax)
-   18000cafd:	add    %ah,0x62(%rcx)
-   18000cb00:	jae    0x18000cb6e
-   18000cb02:	pop    %rdi
-   18000cb03:	jae    0x18000cb79
-   18000cb05:	jb     0x18000cb70
-   18000cb07:	outsb  %ds:(%rsi),(%dx)
-   18000cb08:	addr32 jae 0x18000cb39
-   18000cb0b:	fs insb (%dx),%es:(%rdi)
-   18000cb0d:	insb   (%dx),%es:(%rdi)
-   18000cb0e:	add    %al,(%rax)
-   18000cb10:	insl   (%dx),%es:(%rdi)
-   18000cb11:	add    %bh,(%rdi)
+   18000c9f4:	outsb  %ds:(%rsi),(%dx)
+   18000c9f5:	(bad)
+   18000c9f6:	addr32 gs jb 0x18000ca3a
+   18000c9fa:	outsl  %gs:(%esi),(%dx)
+   18000c9fd:	fs gs rex
+   18000ca00:	rex
+   18000ca01:	rex.B
+   18000ca02:	rex.RB
+   18000ca03:	rex.X
+   18000ca04:	rex.B (bad)
+   18000ca06:	push   %r14
+   18000ca08:	(bad)
+   18000ca09:	and    $0x73,%al
+   18000ca0b:	push   $0x64657261
+   18000ca10:	pop    %rdi
+   18000ca11:	jo     0x18000ca87
+   18000ca13:	jb     0x18000ca55
+   18000ca15:	push   %rsi
+   18000ca16:	rex.B je 0x18000ca8d
+   18000ca19:	jb     0x18000ca84
+   18000ca1b:	(bad)
+   18000ca20:	(bad)
+   18000ca21:	jae    0x18000ca88
+   18000ca23:	rex
+   18000ca24:	outsl  %gs:(%esi),(%dx)
+   18000ca27:	fs gs rex
+   18000ca2a:	rex
+   18000ca2b:	rex jae 0x18000caa2
+   18000ca2e:	fs rex
+   18000ca30:	rex push %rsi
+   18000ca32:	jae    0x18000caa8
+   18000ca34:	jb     0x18000ca9f
+   18000ca36:	outsb  %ds:(%rsi),(%dx)
+   18000ca37:	addr32 pop %rdi
+   18000ca39:	jbe    0x18000caa4
+   18000ca3b:	gs ja  0x18000ca7e
+   18000ca3e:	(bad)
+   18000ca3f:	(bad)
+   18000ca44:	rex pop %rdx
+   18000ca46:	add    %al,(%rax)
+   18000ca48:	mov    $0x0,%bl
+   18000ca4a:	(bad)
+   18000ca4b:	jb     0x18000cab2
+   18000ca4d:	imul   $0x615f7265,0x74(%ebx),%esi
+   18000ca55:	je     0x18000cacb
+   18000ca57:	jb     0x18000cac2
+   18000ca59:	(bad)
+   18000ca5e:	rex.B je 0x18000cad5
+   18000ca61:	jb     0x18000cacc
+   18000ca63:	(bad)
+   18000ca68:	(bad)
+   18000ca69:	outsb  %ds:(%rsi),(%dx)
+   18000ca6a:	(bad)
+   18000ca6b:	addr32 gs jb 0x18000caaf
+   18000ca6f:	outsl  %gs:(%esi),(%dx)
+   18000ca72:	fs gs rex
+   18000ca75:	rex
+   18000ca76:	rex.B
+   18000ca77:	rex.RB
+   18000ca78:	rex.B
+   18000ca79:	pop    %r8
+   18000ca7b:	push   %rsi
+   18000ca7c:	(bad)
+   18000ca7d:	and    $0x73,%al
+   18000ca7f:	push   $0x64657261
+   18000ca84:	pop    %rdi
+   18000ca85:	jo     0x18000cafb
+   18000ca87:	jb     0x18000cac9
+   18000ca89:	push   %rsi
+   18000ca8a:	rex.B je 0x18000cb01
+   18000ca8d:	jb     0x18000caf8
+   18000ca8f:	(bad)
+   18000ca94:	(bad)
+   18000ca95:	jae    0x18000cafc
+   18000ca97:	rex
+   18000ca98:	outsl  %gs:(%esi),(%dx)
+   18000ca9b:	fs gs rex
+   18000ca9e:	rex
+   18000ca9f:	rex jae 0x18000cb16
+   18000caa2:	fs rex
+   18000caa4:	rex push %rsi
+   18000caa6:	jae    0x18000cb1c
+   18000caa8:	jb     0x18000cb13
+   18000caaa:	outsb  %ds:(%rsi),(%dx)
+   18000caab:	addr32 pop %rdi
+   18000caad:	jbe    0x18000cb18
+   18000caaf:	gs ja  0x18000caf2
+   18000cab2:	(bad)
+   18000cab3:	(bad)
+   18000cab8:	rex pop %rdx
+   18000caba:	add    %al,(%rax)
+   18000cabc:	rex.WRXB jo 0x18000cb24
+   18000cabf:	outsb  %ds:(%rsi),(%dx)
+   18000cac0:	rex.RXB
+   18000cac1:	outsl  %gs:(%rsi),(%dx)
+   18000cac3:	fs gs pop %rdi
+   18000cac6:	(bad)
+   18000cac8:	jae    0x18000cb33
+   18000caca:	movsxd (%rsi),%ebp
+   18000cacc:	fs insb (%dx),%es:(%rdi)
+   18000cace:	insb   (%dx),%es:(%rdi)
+   18000cacf:	add    %ch,(%rdx)
+   18000cad1:	add    %edi,(%rdi)
+   18000cad3:	rex.RX (bad)
+   18000cad5:	jae    0x18000cb4b
+   18000cad7:	rex.WB outsb %ds:(%rsi),(%dx)
+   18000cad9:	je     0x18000cb2f
+   18000cadb:	outsl  %ds:(%rsi),(%dx)
+   18000cadc:	rex.X jne 0x18000cb45
+   18000cadf:	data16 gs jb 0x18000cb23
+   18000cae3:	outsb  %ds:(%rsi),(%dx)
+   18000cae4:	jne    0x18000cb53
+   18000cae6:	(bad)
+   18000cae8:	jb     0x18000cb5d
+   18000caea:	pop    %rdi
+   18000caeb:	imul   $0x616e7265,0x74(%rsi),%ebp
+   18000caf2:	insb   (%dx),%es:(%rdi)
+   18000caf3:	rex (bad)
+   18000caf5:	(bad)
+   18000cafa:	pop    %rcx
+   18000cafb:	push   %r8
+   18000cafd:	rex.RB
+   18000cafe:	rex.B
+   18000caff:	rex.R
+   18000cb00:	rex.WB push %r8
+   18000cb02:	rex.RB
+   18000cb03:	rex.B
+   18000cb04:	rex.R
+   18000cb05:	rex pop %rdx
+   18000cb07:	add    %bl,0x1(%rbx)
+   18000cb0a:	(bad)
+   18000cb0b:	push   %rbx
+   18000cb0c:	je     0x18000cb80
+   18000cb0e:	rex.XB (bad)
+   18000cb10:	je     0x18000cb52
+   18000cb12:	(bad)
    18000cb13:	(bad)
-   18000cb14:	xor    %bl,0x4c(%rdi)
-   18000cb17:	outsl  %ds:(%rsi),(%dx)
-   18000cb18:	movsxd 0x69(%rbx),%ebp
-   18000cb1b:	je     0x18000cb5d
-   18000cb1d:	jae    0x18000cb93
-   18000cb1f:	fs rex
-   18000cb21:	rex push %rcx
-   18000cb23:	rex.RB
-   18000cb24:	rex.B
-   18000cb25:	rex.B
-   18000cb26:	rex
-   18000cb27:	rex.W
-   18000cb28:	rex pop %rdx
-   18000cb2a:	add    %al,(%rax)
-   18000cb2c:	movsl  %ds:(%rsi),%es:(%rdi)
-   18000cb2d:	add    %bh,(%rdi)
-   18000cb2f:	(bad)
-   18000cb30:	xor    %ebx,0x4c(%rdi)
-   18000cb33:	outsl  %ds:(%rsi),(%dx)
-   18000cb34:	movsxd 0x69(%rbx),%ebp
-   18000cb37:	je     0x18000cb79
-   18000cb39:	jae    0x18000cbaf
-   18000cb3b:	fs rex
-   18000cb3d:	rex push %rcx
-   18000cb3f:	rex.RB
-   18000cb40:	rex.B
-   18000cb41:	rex.B
-   18000cb42:	rex pop %rax
-   18000cb44:	pop    %rdx
-   18000cb45:	add    %cl,0x585f3f02(%rsi)
-   18000cb4b:	insb   (%dx),%es:(%rdi)
-   18000cb4c:	outsb  %gs:(%rsi),(%dx)
-   18000cb4e:	addr32 je 0x18000cbb9
-   18000cb51:	pop    %rdi
-   18000cb52:	gs jb  0x18000cbc7
-   18000cb55:	outsl  %ds:(%rsi),(%dx)
-   18000cb56:	jb     0x18000cb98
-   18000cb58:	jae    0x18000cbce
-   18000cb5a:	fs rex
-   18000cb5c:	rex pop %rcx
-   18000cb5e:	pop    %r8
-   18000cb60:	push   %rax
-   18000cb61:	rex.RB
-   18000cb62:	rex.X
-   18000cb63:	rex.R
-   18000cb64:	rex pop %rdx
-   18000cb66:	add    %al,(%rax)
-   18000cb68:	(bad)
-   18000cb69:	add    $0x636e753f,%eax
-   18000cb6e:	(bad)
-   18000cb6f:	jne    0x18000cbd8
-   18000cb71:	push   $0x78655f74
-   18000cb76:	movsxd 0x70(%rbp),%esp
-   18000cb79:	je     0x18000cbe4
-   18000cb7b:	outsl  %ds:(%rsi),(%dx)
-   18000cb7c:	outsb  %ds:(%rsi),(%dx)
-   18000cb7d:	rex jae 0x18000cbf4
-   18000cb80:	fs rex
-   18000cb82:	rex pop %rcx
-   18000cb84:	pop    %r15
-   18000cb86:	rex.WRX pop %rax
-   18000cb88:	pop    %rdx
-   18000cb89:	add    %dh,(%rcx)
-   18000cb8b:	add    %edi,(%rdi)
-   18000cb8d:	(bad)
-   18000cb8e:	imul   $0x6c61636f,0x6c(%rax,%r8,2),%esp
-   18000cb97:	gs rex jae 0x18000cc0f
-   18000cb9b:	fs rex
-   18000cb9d:	rex push %rcx
-   18000cb9f:	rex.RB
-   18000cba0:	rex.B
-   18000cba1:	pop    %r15
-   18000cba3:	rex.WXB pop %r8
-   18000cba5:	pop    %rdx
-   18000cba6:	add    %al,(%rax)
-   18000cba8:	(bad)
-   18000cba9:	add    %edi,(%rdi)
-   18000cbab:	pop    %rdi
-   18000cbac:	rex.RXB
-   18000cbad:	gs je  0x18000cc17
-   18000cbb0:	insb   (%dx),%es:(%rdi)
-   18000cbb1:	outsl  %ds:(%rsi),(%dx)
-   18000cbb2:	(bad)
-   18000cbb7:	movsxd 0x6c(%rcx),%esp
-   18000cbba:	gs rex insb (%dx),%es:(%rdi)
-   18000cbbd:	outsl  %ds:(%rsi),(%dx)
-   18000cbbe:	movsxd 0x6c(%rcx),%esp
-   18000cbc1:	gs rex jae 0x18000cc39
-   18000cbc5:	fs rex
-   18000cbc7:	rex
-   18000cbc8:	rex.XB
-   18000cbc9:	push   %r8
-   18000cbcb:	rex.RB
-   18000cbcc:	push   %r14
-   18000cbce:	pop    %rdi
-   18000cbcf:	rex.WR outsl %ds:(%rsi),(%dx)
-   18000cbd1:	movsxd 0x6d(%rcx),%ebp
-   18000cbd4:	jo     0x18000cc16
-   18000cbd6:	xor    %esi,(%rdx)
-   18000cbd8:	rex pop %rax
-   18000cbda:	pop    %rdx
-   18000cbdb:	add    %bl,0x6c613f02(%rbp)
-   18000cbe1:	ja     0x18000cc44
-   18000cbe3:	jns    0x18000cc58
-   18000cbe5:	pop    %rdi
-   18000cbe6:	outsb  %ds:(%rsi),(%dx)
-   18000cbe7:	outsl  %ds:(%rsi),(%dx)
-   18000cbe8:	movsxd 0x6e(%rdi),%ebp
-   18000cbeb:	jbe    0x18000cc2d
-   18000cbed:	movsxd 0x64(%rdi),%ebp
-   18000cbf0:	movsxd %gs:0x74(%rsi),%esi
-   18000cbf4:	pop    %rdi
-   18000cbf5:	(bad)
-   18000cbf7:	jae    0x18000cc5e
-   18000cbf9:	rex jae 0x18000cc70
-   18000cbfc:	fs rex
-   18000cbfe:	rex push %rcx
-   18000cc00:	rex.RB
-   18000cc01:	rex.X
-   18000cc02:	pop    %r15
-   18000cc04:	rex.WRX pop %rax
-   18000cc06:	pop    %rdx
-   18000cc07:	add    %bh,%dl
-   18000cc09:	add    (%rdi),%edi
-   18000cc0b:	imul   $0x6f63243f,0x40(%rsi),%ebp
-   18000cc12:	fs movsxd %gs:0x74(%rsi),%esi
-   18000cc17:	rex
-   18000cc18:	rex.R
-   18000cc19:	rex.R push %rbp
+   18000cb18:	pop    %rcx
+   18000cb19:	rex.B (bad)
+   18000cb1b:	push   %r14
+   18000cb1d:	(bad)
+   18000cb1e:	and    $0x62,%al
+   18000cb20:	(bad)
+   18000cb21:	jae    0x18000cb8c
+   18000cb23:	movsxd 0x73(%rdi),%ebx
+   18000cb26:	je     0x18000cb9a
+   18000cb28:	imul   $0x3f554440,0x67(%rsi),%ebp
+   18000cb2f:	and    $0x63,%al
+   18000cb31:	push   $0x745f7261
+   18000cb36:	jb     0x18000cb99
+   18000cb38:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000cb40:	fs rex
+   18000cb42:	rex push %rsi
+   18000cb44:	(bad)
+   18000cb45:	and    $0x61,%al
+   18000cb47:	insb   (%dx),%es:(%rdi)
+   18000cb48:	insb   (%dx),%es:(%rdi)
+   18000cb49:	outsl  %ds:(%rsi),(%dx)
+   18000cb4a:	movsxd 0x74(%rcx),%esp
+   18000cb4d:	outsl  %ds:(%rsi),(%dx)
+   18000cb4e:	jb     0x18000cb90
+   18000cb50:	rex.R
+   18000cb51:	rex xor 0x40(%rax),%al
+   18000cb55:	jae    0x18000cbcb
+   18000cb57:	fs rex
+   18000cb59:	rex
+   18000cb5a:	rex.B
+   18000cb5b:	rex.RB
+   18000cb5c:	rex.X push %rsi
+   18000cb5e:	rex.B insb (%dx),%es:(%rdi)
+   18000cb60:	jo     0x18000cbca
+   18000cb62:	(bad)
+   18000cb63:	rex.WRX jne 0x18000cbd3
+   18000cb66:	rex xor %eax,0x30(%rax)
+   18000cb6a:	xor    %al,0x5a(%rax)
+   18000cb6d:	add    %ah,0x62(%rcx)
+   18000cb70:	jae    0x18000cbde
+   18000cb72:	pop    %rdi
+   18000cb73:	jae    0x18000cbe9
+   18000cb75:	jb     0x18000cbe0
+   18000cb77:	outsb  %ds:(%rsi),(%dx)
+   18000cb78:	addr32 jae 0x18000cba9
+   18000cb7b:	fs insb (%dx),%es:(%rdi)
+   18000cb7d:	insb   (%dx),%es:(%rdi)
+   18000cb7e:	add    %al,(%rax)
+   18000cb80:	insl   (%dx),%es:(%rdi)
+   18000cb81:	add    %bh,(%rdi)
+   18000cb83:	(bad)
+   18000cb84:	xor    %bl,0x4c(%rdi)
+   18000cb87:	outsl  %ds:(%rsi),(%dx)
+   18000cb88:	movsxd 0x69(%rbx),%ebp
+   18000cb8b:	je     0x18000cbcd
+   18000cb8d:	jae    0x18000cc03
+   18000cb8f:	fs rex
+   18000cb91:	rex push %rcx
+   18000cb93:	rex.RB
+   18000cb94:	rex.B
+   18000cb95:	rex.B
+   18000cb96:	rex
+   18000cb97:	rex.W
+   18000cb98:	rex pop %rdx
+   18000cb9a:	add    %al,(%rax)
+   18000cb9c:	movsl  %ds:(%rsi),%es:(%rdi)
+   18000cb9d:	add    %bh,(%rdi)
+   18000cb9f:	(bad)
+   18000cba0:	xor    %ebx,0x4c(%rdi)
+   18000cba3:	outsl  %ds:(%rsi),(%dx)
+   18000cba4:	movsxd 0x69(%rbx),%ebp
+   18000cba7:	je     0x18000cbe9
+   18000cba9:	jae    0x18000cc1f
+   18000cbab:	fs rex
+   18000cbad:	rex push %rcx
+   18000cbaf:	rex.RB
+   18000cbb0:	rex.B
+   18000cbb1:	rex.B
+   18000cbb2:	rex pop %rax
+   18000cbb4:	pop    %rdx
+   18000cbb5:	add    %cl,0x585f3f02(%rsi)
+   18000cbbb:	insb   (%dx),%es:(%rdi)
+   18000cbbc:	outsb  %gs:(%rsi),(%dx)
+   18000cbbe:	addr32 je 0x18000cc29
+   18000cbc1:	pop    %rdi
+   18000cbc2:	gs jb  0x18000cc37
+   18000cbc5:	outsl  %ds:(%rsi),(%dx)
+   18000cbc6:	jb     0x18000cc08
+   18000cbc8:	jae    0x18000cc3e
+   18000cbca:	fs rex
+   18000cbcc:	rex pop %rcx
+   18000cbce:	pop    %r8
+   18000cbd0:	push   %rax
+   18000cbd1:	rex.RB
+   18000cbd2:	rex.X
+   18000cbd3:	rex.R
+   18000cbd4:	rex pop %rdx
+   18000cbd6:	add    %al,(%rax)
+   18000cbd8:	(bad)
+   18000cbd9:	add    $0x636e753f,%eax
+   18000cbde:	(bad)
+   18000cbdf:	jne    0x18000cc48
+   18000cbe1:	push   $0x78655f74
+   18000cbe6:	movsxd 0x70(%rbp),%esp
+   18000cbe9:	je     0x18000cc54
+   18000cbeb:	outsl  %ds:(%rsi),(%dx)
+   18000cbec:	outsb  %ds:(%rsi),(%dx)
+   18000cbed:	rex jae 0x18000cc64
+   18000cbf0:	fs rex
+   18000cbf2:	rex pop %rcx
+   18000cbf4:	pop    %r15
+   18000cbf6:	rex.WRX pop %rax
+   18000cbf8:	pop    %rdx
+   18000cbf9:	add    %dh,(%rcx)
+   18000cbfb:	add    %edi,(%rdi)
+   18000cbfd:	(bad)
+   18000cbfe:	imul   $0x6c61636f,0x6c(%rax,%r8,2),%esp
+   18000cc07:	gs rex jae 0x18000cc7f
+   18000cc0b:	fs rex
+   18000cc0d:	rex push %rcx
+   18000cc0f:	rex.RB
+   18000cc10:	rex.B
+   18000cc11:	pop    %r15
+   18000cc13:	rex.WXB pop %r8
+   18000cc15:	pop    %rdx
+   18000cc16:	add    %al,(%rax)
+   18000cc18:	(bad)
+   18000cc19:	add    %edi,(%rdi)
    18000cc1b:	pop    %rdi
-   18000cc1c:	(bad)
-   18000cc22:	gs je  0x18000cc65
-   18000cc25:	rex
-   18000cc26:	rex jae 0x18000cc9d
-   18000cc29:	fs rex
-   18000cc2b:	rex push %rcx
-   18000cc2d:	rex.RB
-   18000cc2e:	rex.X
-   18000cc2f:	rex.B
-   18000cc30:	rex.W
-   18000cc31:	rex.B
-   18000cc32:	rex.RB
-   18000cc33:	push   %r13
-   18000cc35:	pop    %rdi
-   18000cc36:	(bad)
-   18000cc3c:	gs je  0x18000cc7f
-   18000cc3f:	rex push %rax
-   18000cc41:	rex.RB
-   18000cc42:	rex.X
-   18000cc43:	xor    %r8d,0x45(%rcx)
-   18000cc47:	push   %r8
-   18000cc49:	rex.RB
-   18000cc4a:	rex.X
-   18000cc4b:	rex.R push %rax
-   18000cc4d:	rex.RB
-   18000cc4e:	rex.B
-   18000cc4f:	xor    0x45(%rcx),%r8d
-   18000cc53:	push   %r8
-   18000cc55:	rex.RB
-   18000cc56:	rex.B
-   18000cc57:	rex.R
-   18000cc58:	rex pop %rdx
-   18000cc5a:	add    %al,(%rax)
-   18000cc5c:	xor    (%rdi,%rdi,1),%eax
-   18000cc5f:	outsl  %ds:(%rsi),(%dx)
-   18000cc60:	jne    0x18000ccd6
-   18000cc62:	rex (bad)
-   18000cc64:	and    $0x63,%al
-   18000cc66:	outsl  %ds:(%rsi),(%dx)
-   18000cc67:	fs movsxd %gs:0x74(%rsi),%esi
-   18000cc6c:	rex
-   18000cc6d:	rex.R
-   18000cc6e:	rex.R push %rbp
-   18000cc70:	pop    %rdi
-   18000cc71:	(bad)
-   18000cc77:	gs je  0x18000ccba
-   18000cc7a:	rex
-   18000cc7b:	rex jae 0x18000ccf2
-   18000cc7e:	fs rex
-   18000cc80:	rex push %rcx
-   18000cc82:	rex.RB
-   18000cc83:	rex.X
-   18000cc84:	rex.B
-   18000cc85:	rex.W
-   18000cc86:	rex.B
-   18000cc87:	rex.RB
-   18000cc88:	push   %r13
-   18000cc8a:	pop    %rdi
-   18000cc8b:	(bad)
-   18000cc91:	gs je  0x18000ccd4
-   18000cc94:	rex push %rax
-   18000cc96:	rex.RB
-   18000cc97:	rex.X
-   18000cc98:	xor    %r8d,0x45(%rcx)
-   18000cc9c:	push   %r8
-   18000cc9e:	rex.RB
-   18000cc9f:	rex.X
-   18000cca0:	rex.R push %rax
+   18000cc1c:	rex.RXB
+   18000cc1d:	gs je  0x18000cc87
+   18000cc20:	insb   (%dx),%es:(%rdi)
+   18000cc21:	outsl  %ds:(%rsi),(%dx)
+   18000cc22:	(bad)
+   18000cc27:	movsxd 0x6c(%rcx),%esp
+   18000cc2a:	gs rex insb (%dx),%es:(%rdi)
+   18000cc2d:	outsl  %ds:(%rsi),(%dx)
+   18000cc2e:	movsxd 0x6c(%rcx),%esp
+   18000cc31:	gs rex jae 0x18000cca9
+   18000cc35:	fs rex
+   18000cc37:	rex
+   18000cc38:	rex.XB
+   18000cc39:	push   %r8
+   18000cc3b:	rex.RB
+   18000cc3c:	push   %r14
+   18000cc3e:	pop    %rdi
+   18000cc3f:	rex.WR outsl %ds:(%rsi),(%dx)
+   18000cc41:	movsxd 0x6d(%rcx),%ebp
+   18000cc44:	jo     0x18000cc86
+   18000cc46:	xor    %esi,(%rdx)
+   18000cc48:	rex pop %rax
+   18000cc4a:	pop    %rdx
+   18000cc4b:	add    %bl,0x6c613f02(%rbp)
+   18000cc51:	ja     0x18000ccb4
+   18000cc53:	jns    0x18000ccc8
+   18000cc55:	pop    %rdi
+   18000cc56:	outsb  %ds:(%rsi),(%dx)
+   18000cc57:	outsl  %ds:(%rsi),(%dx)
+   18000cc58:	movsxd 0x6e(%rdi),%ebp
+   18000cc5b:	jbe    0x18000cc9d
+   18000cc5d:	movsxd 0x64(%rdi),%ebp
+   18000cc60:	movsxd %gs:0x74(%rsi),%esi
+   18000cc64:	pop    %rdi
+   18000cc65:	(bad)
+   18000cc67:	jae    0x18000ccce
+   18000cc69:	rex jae 0x18000cce0
+   18000cc6c:	fs rex
+   18000cc6e:	rex push %rcx
+   18000cc70:	rex.RB
+   18000cc71:	rex.X
+   18000cc72:	pop    %r15
+   18000cc74:	rex.WRX pop %rax
+   18000cc76:	pop    %rdx
+   18000cc77:	add    %bh,%dl
+   18000cc79:	add    (%rdi),%edi
+   18000cc7b:	imul   $0x6f63243f,0x40(%rsi),%ebp
+   18000cc82:	fs movsxd %gs:0x74(%rsi),%esi
+   18000cc87:	rex
+   18000cc88:	rex.R
+   18000cc89:	rex.R push %rbp
+   18000cc8b:	pop    %rdi
+   18000cc8c:	(bad)
+   18000cc92:	gs je  0x18000ccd5
+   18000cc95:	rex
+   18000cc96:	rex jae 0x18000cd0d
+   18000cc99:	fs rex
+   18000cc9b:	rex push %rcx
+   18000cc9d:	rex.RB
+   18000cc9e:	rex.X
+   18000cc9f:	rex.B
+   18000cca0:	rex.W
+   18000cca1:	rex.B
    18000cca2:	rex.RB
-   18000cca3:	rex.B
-   18000cca4:	xor    0x45(%rcx),%r8d
-   18000cca8:	push   %r8
-   18000ccaa:	rex.RB
-   18000ccab:	rex.B
-   18000ccac:	rex.R
-   18000ccad:	rex pop %rdx
-   18000ccaf:	add    %ah,(%rdi)
-   18000ccb1:	add    $0x736e753f,%eax
-   18000ccb6:	push   $0x40746669
-   18000ccbb:	(bad)
-   18000ccbc:	and    $0x63,%al
-   18000ccbe:	outsl  %ds:(%rsi),(%dx)
-   18000ccbf:	fs movsxd %gs:0x74(%rsi),%esi
-   18000ccc4:	rex
-   18000ccc5:	rex.R
-   18000ccc6:	rex.R push %rbp
-   18000ccc8:	pop    %rdi
-   18000ccc9:	(bad)
-   18000cccf:	gs je  0x18000cd12
-   18000ccd2:	rex
-   18000ccd3:	rex jae 0x18000cd4a
-   18000ccd6:	fs rex
-   18000ccd8:	rex push %rcx
-   18000ccda:	rex.RB
-   18000ccdb:	rex.X
-   18000ccdc:	rex.B
-   18000ccdd:	rex.W
-   18000ccde:	rex.B
-   18000ccdf:	rex.RB
-   18000cce0:	push   %r13
-   18000cce2:	pop    %rdi
-   18000cce3:	(bad)
-   18000cce9:	gs je  0x18000cd2c
-   18000ccec:	rex push %rax
-   18000ccee:	rex.RB
-   18000ccef:	rex.B
-   18000ccf0:	xor    %r8d,0x45(%rcx)
-   18000ccf4:	push   %r8
-   18000ccf6:	rex.RB
-   18000ccf7:	rex.B
-   18000ccf8:	rex.R
-   18000ccf9:	rex pop %rdx
-   18000ccfb:	add    %dh,0x475f3f01(%rcx)
-   18000cd01:	gs je  0x18000cd67
-   18000cd04:	(bad)
-   18000cd05:	je     0x18000cd47
-   18000cd07:	(bad)
-   18000cd08:	and    $0x63,%al
-   18000cd0a:	outsl  %ds:(%rsi),(%dx)
-   18000cd0b:	fs movsxd %gs:0x74(%rsi),%esi
-   18000cd10:	rex
-   18000cd11:	rex.R
-   18000cd12:	rex.R push %rbp
-   18000cd14:	pop    %rdi
-   18000cd15:	(bad)
-   18000cd1b:	gs je  0x18000cd5e
-   18000cd1e:	rex
-   18000cd1f:	rex jae 0x18000cd96
-   18000cd22:	fs rex
-   18000cd24:	rex push %rbx
-   18000cd26:	pop    %r15
-   18000cd28:	rex.WXB push %r8
-   18000cd2a:	rex.RB
-   18000cd2b:	push   %r8
-   18000cd2d:	rex.RB
-   18000cd2e:	rex.X push %rsi
-   18000cd30:	data16 (bad)
-   18000cd32:	movsxd 0x74(%rbp),%esp
-   18000cd35:	rex insb (%dx),%es:(%rdi)
-   18000cd37:	outsl  %ds:(%rsi),(%dx)
-   18000cd38:	movsxd 0x6c(%rcx),%esp
-   18000cd3b:	rex xor %gs:0x50(%rax),%al
-   18000cd40:	rex.RB
-   18000cd41:	rex.X push %rsi
-   18000cd43:	xor    $0x32,%al
-   18000cd45:	rex
-   18000cd46:	rex pop %rdx
-   18000cd48:	add    %al,(%rax)
-   18000cd4a:	(bad)
-   18000cd4b:	add    %bh,(%rdi)
-   18000cd4d:	(bad)
-   18000cd4e:	xor    %bh,(%rdi)
-   18000cd50:	and    $0x62,%al
-   18000cd52:	(bad)
-   18000cd53:	jae    0x18000cdbe
-   18000cd55:	movsxd 0x73(%rdi),%ebx
-   18000cd58:	je     0x18000cdcc
-   18000cd5a:	gs (bad)
-   18000cd5c:	insl   (%dx),%es:(%rdi)
-   18000cd5d:	(bad)
-   18000cd62:	push   %rbp
-   18000cd63:	(bad)
-   18000cd64:	and    $0x63,%al
-   18000cd66:	push   $0x745f7261
-   18000cd6b:	jb     0x18000cdce
-   18000cd6d:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000cd75:	fs rex
-   18000cd77:	rex
-   18000cd78:	rex jae 0x18000cdef
-   18000cd7b:	fs rex
-   18000cd7d:	rex
-   18000cd7e:	rex.WB
-   18000cd7f:	rex.RB
-   18000cd80:	rex.B
-   18000cd81:	rex.B
-   18000cd82:	rex pop %rax
-   18000cd84:	pop    %rdx
-   18000cd85:	add    %cl,0x313f3f00(%rcx)
-   18000cd8b:	(bad)
-   18000cd8c:	and    $0x62,%al
-   18000cd8e:	(bad)
-   18000cd8f:	jae    0x18000cdfa
-   18000cd91:	movsxd 0x73(%rdi),%ebx
-   18000cd94:	je     0x18000ce08
-   18000cd96:	gs (bad)
-   18000cd98:	insl   (%dx),%es:(%rdi)
-   18000cd99:	(bad)
-   18000cd9e:	push   %rbp
-   18000cd9f:	(bad)
-   18000cda0:	and    $0x63,%al
-   18000cda2:	push   $0x745f7261
-   18000cda7:	jb     0x18000ce0a
-   18000cda9:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000cdb1:	fs rex
-   18000cdb3:	rex
-   18000cdb4:	rex jae 0x18000ce2b
-   18000cdb7:	fs rex
-   18000cdb9:	rex push %rbp
-   18000cdbb:	rex.RB
-   18000cdbc:	rex.B
-   18000cdbd:	rex.B
-   18000cdbe:	rex pop %rax
-   18000cdc0:	pop    %rdx
-   18000cdc1:	add    %al,%al
-   18000cdc3:	add    (%rdi),%edi
-   18000cdc5:	addr32 gs je 0x18000ce35
-   18000cdc9:	outsl  %ds:(%rsi),(%dx)
-   18000cdca:	movsxd 0x3f(%rax),%eax
-   18000cdcd:	and    $0x62,%al
-   18000cdcf:	(bad)
-   18000cdd0:	jae    0x18000ce3b
-   18000cdd2:	movsxd 0x73(%rdi),%ebx
-   18000cdd5:	je     0x18000ce49
-   18000cdd7:	gs (bad)
-   18000cdd9:	insl   (%dx),%es:(%rdi)
-   18000cdda:	(bad)
-   18000cddf:	push   %rbp
-   18000cde0:	(bad)
-   18000cde1:	and    $0x63,%al
-   18000cde3:	push   $0x745f7261
-   18000cde8:	jb     0x18000ce4b
-   18000cdea:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000cdf2:	fs rex
-   18000cdf4:	rex
-   18000cdf5:	rex jae 0x18000ce6c
-   18000cdf8:	fs rex
-   18000cdfa:	rex push %rcx
-   18000cdfc:	rex.RB
-   18000cdfd:	rex.X
-   18000cdfe:	rex.B (bad)
-   18000ce00:	push   %r14
-   18000ce02:	insb   (%dx),%es:(%rdi)
-   18000ce03:	outsl  %ds:(%rsi),(%dx)
-   18000ce04:	movsxd 0x6c(%rcx),%esp
-   18000ce07:	rex xor %gs:0x58(%rax),%al
-   18000ce0c:	pop    %rdx
-   18000ce0d:	add    %bl,%dh
-   18000ce0f:	add    $0x3f,%al
-   18000ce11:	jae    0x18000ce83
-   18000ce13:	jne    0x18000ce89
-   18000ce15:	movsxd 0x3f(%rax),%eax
-   18000ce18:	and    $0x62,%al
-   18000ce1a:	(bad)
-   18000ce1b:	jae    0x18000ce86
-   18000ce1d:	movsxd 0x73(%rdi),%ebx
-   18000ce20:	je     0x18000ce94
-   18000ce22:	gs (bad)
-   18000ce24:	insl   (%dx),%es:(%rdi)
-   18000ce25:	(bad)
-   18000ce2a:	push   %rbp
-   18000ce2b:	(bad)
-   18000ce2c:	and    $0x63,%al
-   18000ce2e:	push   $0x745f7261
-   18000ce33:	jb     0x18000ce96
-   18000ce35:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000ce3d:	fs rex
-   18000ce3f:	rex
-   18000ce40:	rex jae 0x18000ceb7
-   18000ce43:	fs rex
-   18000ce45:	rex push %rcx
-   18000ce47:	rex.RB
-   18000ce48:	rex.B
-   18000ce49:	rex.B
-   18000ce4a:	rex.W
-   18000ce4b:	rex.R
-   18000ce4c:	rex pop %rdx
-   18000ce4e:	add    %al,(%rax)
-   18000ce50:	loope  0x18000ce56
-   18000ce52:	(bad)
-   18000ce53:	jae    0x18000cec5
-   18000ce55:	jne    0x18000cecb
-   18000ce57:	outsb  %ds:(%rsi),(%dx)
-   18000ce58:	rex (bad)
-   18000ce5a:	and    $0x62,%al
-   18000ce5c:	(bad)
-   18000ce5d:	jae    0x18000cec8
-   18000ce5f:	movsxd 0x73(%rdi),%ebx
-   18000ce62:	je     0x18000ced6
-   18000ce64:	gs (bad)
-   18000ce66:	insl   (%dx),%es:(%rdi)
-   18000ce67:	(bad)
-   18000ce6c:	push   %rbp
-   18000ce6d:	(bad)
-   18000ce6e:	and    $0x63,%al
-   18000ce70:	push   $0x745f7261
-   18000ce75:	jb     0x18000ced8
-   18000ce77:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000ce7f:	fs rex
-   18000ce81:	rex
-   18000ce82:	rex jae 0x18000cef9
-   18000ce85:	fs rex
-   18000ce87:	rex push %rcx
-   18000ce89:	rex.RB
-   18000ce8a:	rex.B
-   18000ce8b:	pop    %r15
-   18000ce8d:	rex.WX push %rax
-   18000ce8f:	rex.RB
-   18000ce90:	rex.X
-   18000ce91:	rex.R pop %rdi
-   18000ce93:	rex.WX
-   18000ce94:	rex pop %rdx
-   18000ce96:	add    %al,(%rax)
-   18000ce98:	rex.WX add (%rdi),%dil
-   18000ce9b:	pop    %rdi
-   18000ce9c:	push   %rax
-   18000ce9d:	outsb  %ds:(%rsi),(%dx)
-   18000ce9e:	imul   $0x62243f40,0x63(%rsi),%ebp
-   18000cea5:	(bad)
-   18000cea6:	jae    0x18000cf11
-   18000cea8:	movsxd 0x73(%rdi),%ebx
-   18000ceab:	je     0x18000cf1f
-   18000cead:	gs (bad)
-   18000ceaf:	insl   (%dx),%es:(%rdi)
-   18000ceb0:	(bad)
-   18000ceb5:	push   %rbp
-   18000ceb6:	(bad)
-   18000ceb7:	and    $0x63,%al
-   18000ceb9:	push   $0x745f7261
-   18000cebe:	jb     0x18000cf21
-   18000cec0:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000cec8:	fs rex
-   18000ceca:	rex
-   18000cecb:	rex jae 0x18000cf42
-   18000cece:	fs rex
-   18000ced0:	rex
-   18000ced1:	rex.WB
-   18000ced2:	rex.RB
-   18000ced3:	rex.B
-   18000ced4:	push   %r8
-   18000ced6:	rex.RB
-   18000ced7:	rex.B
-   18000ced8:	rex.R pop %rax
-   18000ceda:	pop    %rdx
-   18000cedb:	add    %dh,%ch
-   18000cedd:	add    %edi,(%rdi)
-   18000cedf:	pop    %rdi
-   18000cee0:	rex.WB outsb %ds:(%rsi),(%dx)
-   18000cee2:	imul   $0x73616224,0x3f(%rax,%rax,2),%esi
-   18000ceea:	imul   $0x65727473,0x5f(%rbx),%esp
-   18000cef1:	(bad)
-   18000cef2:	insl   (%dx),%es:(%rdi)
-   18000cef3:	(bad)
-   18000cef8:	push   %rbp
-   18000cef9:	(bad)
-   18000cefa:	and    $0x63,%al
-   18000cefc:	push   $0x745f7261
-   18000cf01:	jb     0x18000cf64
-   18000cf03:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000cf0b:	fs rex
-   18000cf0d:	rex
-   18000cf0e:	rex jae 0x18000cf85
-   18000cf11:	fs rex
-   18000cf13:	rex
-   18000cf14:	rex.WB
-   18000cf15:	rex.RB
-   18000cf16:	rex.B
-   18000cf17:	pop    %r8
-   18000cf19:	pop    %rax
-   18000cf1a:	pop    %rdx
-   18000cf1b:	add    %dh,%ah
-   18000cf1d:	add    %edi,(%rdi)
-   18000cf1f:	pop    %rdi
-   18000cf20:	rex.WB outsb %ds:(%rsi),(%dx)
-   18000cf22:	imul   $0x73616224,0x3f(%rax,%rax,2),%esi
-   18000cf2a:	imul   $0x65727473,0x5f(%rbx),%esp
-   18000cf31:	(bad)
-   18000cf32:	insl   (%dx),%es:(%rdi)
-   18000cf33:	(bad)
-   18000cf38:	push   %rbp
-   18000cf39:	(bad)
-   18000cf3a:	and    $0x63,%al
-   18000cf3c:	push   $0x745f7261
-   18000cf41:	jb     0x18000cfa4
-   18000cf43:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000cf4b:	fs rex
-   18000cf4d:	rex
-   18000cf4e:	rex jae 0x18000cfc5
-   18000cf51:	fs rex
-   18000cf53:	rex
-   18000cf54:	rex.WB
-   18000cf55:	rex.RB
-   18000cf56:	rex.B
-   18000cf57:	pop    %r8
-   18000cf59:	push   %rax
-   18000cf5a:	rex.RB
-   18000cf5b:	push   %r8
-   18000cf5d:	rex.RB
-   18000cf5e:	rex.B
-   18000cf5f:	xor    %r10b,0x45(%rax)
-   18000cf63:	rex.B
-   18000cf64:	rex.W xor %sil,(%rax)
-   18000cf67:	xor    %eax,0x5a(%rax)
-   18000cf6a:	add    %al,(%rax)
-   18000cf6c:	rex.XB add $0x6773783f,%eax
-   18000cf72:	gs je  0x18000cfe3
-   18000cf75:	rex (bad)
-   18000cf77:	and    $0x62,%al
-   18000cf79:	(bad)
-   18000cf7a:	jae    0x18000cfe5
-   18000cf7c:	movsxd 0x73(%rdi),%ebx
-   18000cf7f:	je     0x18000cff3
-   18000cf81:	gs (bad)
-   18000cf83:	insl   (%dx),%es:(%rdi)
-   18000cf84:	(bad)
-   18000cf89:	push   %rbp
-   18000cf8a:	(bad)
-   18000cf8b:	and    $0x63,%al
-   18000cf8d:	push   $0x745f7261
-   18000cf92:	jb     0x18000cff5
-   18000cf94:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000cf9c:	fs rex
-   18000cf9e:	rex
-   18000cf9f:	rex jae 0x18000d016
-   18000cfa2:	fs rex
-   18000cfa4:	rex
-   18000cfa5:	rex.WRB
-   18000cfa6:	rex.RB
-   18000cfa7:	rex.B
-   18000cfa8:	pop    %r15
-   18000cfaa:	rex.WX push %rax
-   18000cfac:	rex.RB
-   18000cfad:	rex.B
-   18000cfae:	rex.R pop %rdi
-   18000cfb0:	rex.WX
-   18000cfb1:	rex pop %rdx
-   18000cfb3:	add    %al,0x5(%rsi)
-   18000cfb6:	(bad)
-   18000cfb7:	js     0x18000d02c
-   18000cfb9:	jo     0x18000d030
-   18000cfbb:	je     0x18000d02b
-   18000cfbd:	rex (bad)
-   18000cfbf:	and    $0x62,%al
-   18000cfc1:	(bad)
-   18000cfc2:	jae    0x18000d02d
-   18000cfc4:	movsxd 0x73(%rdi),%ebx
-   18000cfc7:	je     0x18000d03b
-   18000cfc9:	gs (bad)
-   18000cfcb:	insl   (%dx),%es:(%rdi)
-   18000cfcc:	(bad)
-   18000cfd1:	push   %rbp
-   18000cfd2:	(bad)
-   18000cfd3:	and    $0x63,%al
-   18000cfd5:	push   $0x745f7261
-   18000cfda:	jb     0x18000d03d
-   18000cfdc:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000cfe4:	fs rex
-   18000cfe6:	rex
-   18000cfe7:	rex jae 0x18000d05e
-   18000cfea:	fs rex
-   18000cfec:	rex
-   18000cfed:	rex.WRB
-   18000cfee:	rex.RB
-   18000cfef:	rex.B
-   18000cff0:	pop    %r15
-   18000cff2:	rex.WX push %rax
-   18000cff4:	rex.RB
-   18000cff5:	rex.X
-   18000cff6:	rex.R pop %rdi
-   18000cff8:	rex.WX
-   18000cff9:	rex pop %rdx
-   18000cffb:	add    %bh,0x0(%rbp)
-   18000cffe:	(bad)
-   18000cfff:	(bad)
-   18000d000:	xor    %edi,(%rdi)
-   18000d002:	and    $0x62,%al
-   18000d004:	(bad)
-   18000d005:	jae    0x18000d070
-   18000d007:	movsxd 0x69(%rdi),%ebx
-   18000d00a:	outsl  %ds:(%rsi),(%dx)
-   18000d00b:	jae    0x18000d04d
-   18000d00d:	rex.R push %rbp
-   18000d00f:	(bad)
-   18000d010:	and    $0x63,%al
-   18000d012:	push   $0x745f7261
-   18000d017:	jb     0x18000d07a
-   18000d019:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000d021:	fs rex
-   18000d023:	rex
-   18000d024:	rex jae 0x18000d09b
-   18000d027:	fs rex
-   18000d029:	rex push %rbp
-   18000d02b:	rex.RB
-   18000d02c:	rex.B
-   18000d02d:	rex.B
-   18000d02e:	rex pop %rax
-   18000d030:	pop    %rdx
-   18000d031:	add    %ah,0x6c633f02(%rsi)
-   18000d037:	gs (bad)
-   18000d039:	jb     0x18000d07b
-   18000d03b:	(bad)
-   18000d03c:	and    $0x62,%al
-   18000d03e:	(bad)
-   18000d03f:	jae    0x18000d0aa
-   18000d041:	movsxd 0x69(%rdi),%ebx
-   18000d044:	outsl  %ds:(%rsi),(%dx)
-   18000d045:	jae    0x18000d087
-   18000d047:	rex.R push %rbp
-   18000d049:	(bad)
-   18000d04a:	and    $0x63,%al
-   18000d04c:	push   $0x745f7261
-   18000d051:	jb     0x18000d0b4
-   18000d053:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000d05b:	fs rex
-   18000d05d:	rex
-   18000d05e:	rex jae 0x18000d0d5
-   18000d061:	fs rex
-   18000d063:	rex push %rcx
-   18000d065:	rex.RB
-   18000d066:	rex.B
-   18000d067:	pop    %r8
-   18000d069:	rex.W pop %rdi
-   18000d06b:	rex.WRX
-   18000d06c:	rex pop %rdx
-   18000d06e:	add    %al,(%rax)
-   18000d070:	(bad)
-   18000d073:	jae    0x18000d0da
-   18000d075:	je     0x18000d0ea
-   18000d077:	je     0x18000d0da
-   18000d079:	je     0x18000d0e0
-   18000d07b:	rex (bad)
-   18000d07d:	and    $0x62,%al
+   18000cca3:	push   %r13
+   18000cca5:	pop    %rdi
+   18000cca6:	(bad)
+   18000ccac:	gs je  0x18000ccef
+   18000ccaf:	rex push %rax
+   18000ccb1:	rex.RB
+   18000ccb2:	rex.X
+   18000ccb3:	xor    %r8d,0x45(%rcx)
+   18000ccb7:	push   %r8
+   18000ccb9:	rex.RB
+   18000ccba:	rex.X
+   18000ccbb:	rex.R push %rax
+   18000ccbd:	rex.RB
+   18000ccbe:	rex.B
+   18000ccbf:	xor    0x45(%rcx),%r8d
+   18000ccc3:	push   %r8
+   18000ccc5:	rex.RB
+   18000ccc6:	rex.B
+   18000ccc7:	rex.R
+   18000ccc8:	rex pop %rdx
+   18000ccca:	add    %al,(%rax)
+   18000cccc:	xor    (%rdi,%rdi,1),%eax
+   18000cccf:	outsl  %ds:(%rsi),(%dx)
+   18000ccd0:	jne    0x18000cd46
+   18000ccd2:	rex (bad)
+   18000ccd4:	and    $0x63,%al
+   18000ccd6:	outsl  %ds:(%rsi),(%dx)
+   18000ccd7:	fs movsxd %gs:0x74(%rsi),%esi
+   18000ccdc:	rex
+   18000ccdd:	rex.R
+   18000ccde:	rex.R push %rbp
+   18000cce0:	pop    %rdi
+   18000cce1:	(bad)
+   18000cce7:	gs je  0x18000cd2a
+   18000ccea:	rex
+   18000cceb:	rex jae 0x18000cd62
+   18000ccee:	fs rex
+   18000ccf0:	rex push %rcx
+   18000ccf2:	rex.RB
+   18000ccf3:	rex.X
+   18000ccf4:	rex.B
+   18000ccf5:	rex.W
+   18000ccf6:	rex.B
+   18000ccf7:	rex.RB
+   18000ccf8:	push   %r13
+   18000ccfa:	pop    %rdi
+   18000ccfb:	(bad)
+   18000cd01:	gs je  0x18000cd44
+   18000cd04:	rex push %rax
+   18000cd06:	rex.RB
+   18000cd07:	rex.X
+   18000cd08:	xor    %r8d,0x45(%rcx)
+   18000cd0c:	push   %r8
+   18000cd0e:	rex.RB
+   18000cd0f:	rex.X
+   18000cd10:	rex.R push %rax
+   18000cd12:	rex.RB
+   18000cd13:	rex.B
+   18000cd14:	xor    0x45(%rcx),%r8d
+   18000cd18:	push   %r8
+   18000cd1a:	rex.RB
+   18000cd1b:	rex.B
+   18000cd1c:	rex.R
+   18000cd1d:	rex pop %rdx
+   18000cd1f:	add    %ah,(%rdi)
+   18000cd21:	add    $0x736e753f,%eax
+   18000cd26:	push   $0x40746669
+   18000cd2b:	(bad)
+   18000cd2c:	and    $0x63,%al
+   18000cd2e:	outsl  %ds:(%rsi),(%dx)
+   18000cd2f:	fs movsxd %gs:0x74(%rsi),%esi
+   18000cd34:	rex
+   18000cd35:	rex.R
+   18000cd36:	rex.R push %rbp
+   18000cd38:	pop    %rdi
+   18000cd39:	(bad)
+   18000cd3f:	gs je  0x18000cd82
+   18000cd42:	rex
+   18000cd43:	rex jae 0x18000cdba
+   18000cd46:	fs rex
+   18000cd48:	rex push %rcx
+   18000cd4a:	rex.RB
+   18000cd4b:	rex.X
+   18000cd4c:	rex.B
+   18000cd4d:	rex.W
+   18000cd4e:	rex.B
+   18000cd4f:	rex.RB
+   18000cd50:	push   %r13
+   18000cd52:	pop    %rdi
+   18000cd53:	(bad)
+   18000cd59:	gs je  0x18000cd9c
+   18000cd5c:	rex push %rax
+   18000cd5e:	rex.RB
+   18000cd5f:	rex.B
+   18000cd60:	xor    %r8d,0x45(%rcx)
+   18000cd64:	push   %r8
+   18000cd66:	rex.RB
+   18000cd67:	rex.B
+   18000cd68:	rex.R
+   18000cd69:	rex pop %rdx
+   18000cd6b:	add    %dh,0x475f3f01(%rcx)
+   18000cd71:	gs je  0x18000cdd7
+   18000cd74:	(bad)
+   18000cd75:	je     0x18000cdb7
+   18000cd77:	(bad)
+   18000cd78:	and    $0x63,%al
+   18000cd7a:	outsl  %ds:(%rsi),(%dx)
+   18000cd7b:	fs movsxd %gs:0x74(%rsi),%esi
+   18000cd80:	rex
+   18000cd81:	rex.R
+   18000cd82:	rex.R push %rbp
+   18000cd84:	pop    %rdi
+   18000cd85:	(bad)
+   18000cd8b:	gs je  0x18000cdce
+   18000cd8e:	rex
+   18000cd8f:	rex jae 0x18000ce06
+   18000cd92:	fs rex
+   18000cd94:	rex push %rbx
+   18000cd96:	pop    %r15
+   18000cd98:	rex.WXB push %r8
+   18000cd9a:	rex.RB
+   18000cd9b:	push   %r8
+   18000cd9d:	rex.RB
+   18000cd9e:	rex.X push %rsi
+   18000cda0:	data16 (bad)
+   18000cda2:	movsxd 0x74(%rbp),%esp
+   18000cda5:	rex insb (%dx),%es:(%rdi)
+   18000cda7:	outsl  %ds:(%rsi),(%dx)
+   18000cda8:	movsxd 0x6c(%rcx),%esp
+   18000cdab:	rex xor %gs:0x50(%rax),%al
+   18000cdb0:	rex.RB
+   18000cdb1:	rex.X push %rsi
+   18000cdb3:	xor    $0x32,%al
+   18000cdb5:	rex
+   18000cdb6:	rex pop %rdx
+   18000cdb8:	add    %al,(%rax)
+   18000cdba:	(bad)
+   18000cdbb:	add    %bh,(%rdi)
+   18000cdbd:	(bad)
+   18000cdbe:	xor    %bh,(%rdi)
+   18000cdc0:	and    $0x62,%al
+   18000cdc2:	(bad)
+   18000cdc3:	jae    0x18000ce2e
+   18000cdc5:	movsxd 0x73(%rdi),%ebx
+   18000cdc8:	je     0x18000ce3c
+   18000cdca:	gs (bad)
+   18000cdcc:	insl   (%dx),%es:(%rdi)
+   18000cdcd:	(bad)
+   18000cdd2:	push   %rbp
+   18000cdd3:	(bad)
+   18000cdd4:	and    $0x63,%al
+   18000cdd6:	push   $0x745f7261
+   18000cddb:	jb     0x18000ce3e
+   18000cddd:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000cde5:	fs rex
+   18000cde7:	rex
+   18000cde8:	rex jae 0x18000ce5f
+   18000cdeb:	fs rex
+   18000cded:	rex
+   18000cdee:	rex.WB
+   18000cdef:	rex.RB
+   18000cdf0:	rex.B
+   18000cdf1:	rex.B
+   18000cdf2:	rex pop %rax
+   18000cdf4:	pop    %rdx
+   18000cdf5:	add    %cl,0x313f3f00(%rcx)
+   18000cdfb:	(bad)
+   18000cdfc:	and    $0x62,%al
+   18000cdfe:	(bad)
+   18000cdff:	jae    0x18000ce6a
+   18000ce01:	movsxd 0x73(%rdi),%ebx
+   18000ce04:	je     0x18000ce78
+   18000ce06:	gs (bad)
+   18000ce08:	insl   (%dx),%es:(%rdi)
+   18000ce09:	(bad)
+   18000ce0e:	push   %rbp
+   18000ce0f:	(bad)
+   18000ce10:	and    $0x63,%al
+   18000ce12:	push   $0x745f7261
+   18000ce17:	jb     0x18000ce7a
+   18000ce19:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000ce21:	fs rex
+   18000ce23:	rex
+   18000ce24:	rex jae 0x18000ce9b
+   18000ce27:	fs rex
+   18000ce29:	rex push %rbp
+   18000ce2b:	rex.RB
+   18000ce2c:	rex.B
+   18000ce2d:	rex.B
+   18000ce2e:	rex pop %rax
+   18000ce30:	pop    %rdx
+   18000ce31:	add    %al,%al
+   18000ce33:	add    (%rdi),%edi
+   18000ce35:	addr32 gs je 0x18000cea5
+   18000ce39:	outsl  %ds:(%rsi),(%dx)
+   18000ce3a:	movsxd 0x3f(%rax),%eax
+   18000ce3d:	and    $0x62,%al
+   18000ce3f:	(bad)
+   18000ce40:	jae    0x18000ceab
+   18000ce42:	movsxd 0x73(%rdi),%ebx
+   18000ce45:	je     0x18000ceb9
+   18000ce47:	gs (bad)
+   18000ce49:	insl   (%dx),%es:(%rdi)
+   18000ce4a:	(bad)
+   18000ce4f:	push   %rbp
+   18000ce50:	(bad)
+   18000ce51:	and    $0x63,%al
+   18000ce53:	push   $0x745f7261
+   18000ce58:	jb     0x18000cebb
+   18000ce5a:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000ce62:	fs rex
+   18000ce64:	rex
+   18000ce65:	rex jae 0x18000cedc
+   18000ce68:	fs rex
+   18000ce6a:	rex push %rcx
+   18000ce6c:	rex.RB
+   18000ce6d:	rex.X
+   18000ce6e:	rex.B (bad)
+   18000ce70:	push   %r14
+   18000ce72:	insb   (%dx),%es:(%rdi)
+   18000ce73:	outsl  %ds:(%rsi),(%dx)
+   18000ce74:	movsxd 0x6c(%rcx),%esp
+   18000ce77:	rex xor %gs:0x58(%rax),%al
+   18000ce7c:	pop    %rdx
+   18000ce7d:	add    %bl,%dh
+   18000ce7f:	add    $0x3f,%al
+   18000ce81:	jae    0x18000cef3
+   18000ce83:	jne    0x18000cef9
+   18000ce85:	movsxd 0x3f(%rax),%eax
+   18000ce88:	and    $0x62,%al
+   18000ce8a:	(bad)
+   18000ce8b:	jae    0x18000cef6
+   18000ce8d:	movsxd 0x73(%rdi),%ebx
+   18000ce90:	je     0x18000cf04
+   18000ce92:	gs (bad)
+   18000ce94:	insl   (%dx),%es:(%rdi)
+   18000ce95:	(bad)
+   18000ce9a:	push   %rbp
+   18000ce9b:	(bad)
+   18000ce9c:	and    $0x63,%al
+   18000ce9e:	push   $0x745f7261
+   18000cea3:	jb     0x18000cf06
+   18000cea5:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000cead:	fs rex
+   18000ceaf:	rex
+   18000ceb0:	rex jae 0x18000cf27
+   18000ceb3:	fs rex
+   18000ceb5:	rex push %rcx
+   18000ceb7:	rex.RB
+   18000ceb8:	rex.B
+   18000ceb9:	rex.B
+   18000ceba:	rex.W
+   18000cebb:	rex.R
+   18000cebc:	rex pop %rdx
+   18000cebe:	add    %al,(%rax)
+   18000cec0:	loope  0x18000cec6
+   18000cec2:	(bad)
+   18000cec3:	jae    0x18000cf35
+   18000cec5:	jne    0x18000cf3b
+   18000cec7:	outsb  %ds:(%rsi),(%dx)
+   18000cec8:	rex (bad)
+   18000ceca:	and    $0x62,%al
+   18000cecc:	(bad)
+   18000cecd:	jae    0x18000cf38
+   18000cecf:	movsxd 0x73(%rdi),%ebx
+   18000ced2:	je     0x18000cf46
+   18000ced4:	gs (bad)
+   18000ced6:	insl   (%dx),%es:(%rdi)
+   18000ced7:	(bad)
+   18000cedc:	push   %rbp
+   18000cedd:	(bad)
+   18000cede:	and    $0x63,%al
+   18000cee0:	push   $0x745f7261
+   18000cee5:	jb     0x18000cf48
+   18000cee7:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000ceef:	fs rex
+   18000cef1:	rex
+   18000cef2:	rex jae 0x18000cf69
+   18000cef5:	fs rex
+   18000cef7:	rex push %rcx
+   18000cef9:	rex.RB
+   18000cefa:	rex.B
+   18000cefb:	pop    %r15
+   18000cefd:	rex.WX push %rax
+   18000ceff:	rex.RB
+   18000cf00:	rex.X
+   18000cf01:	rex.R pop %rdi
+   18000cf03:	rex.WX
+   18000cf04:	rex pop %rdx
+   18000cf06:	add    %al,(%rax)
+   18000cf08:	rex.WX add (%rdi),%dil
+   18000cf0b:	pop    %rdi
+   18000cf0c:	push   %rax
+   18000cf0d:	outsb  %ds:(%rsi),(%dx)
+   18000cf0e:	imul   $0x62243f40,0x63(%rsi),%ebp
+   18000cf15:	(bad)
+   18000cf16:	jae    0x18000cf81
+   18000cf18:	movsxd 0x73(%rdi),%ebx
+   18000cf1b:	je     0x18000cf8f
+   18000cf1d:	gs (bad)
+   18000cf1f:	insl   (%dx),%es:(%rdi)
+   18000cf20:	(bad)
+   18000cf25:	push   %rbp
+   18000cf26:	(bad)
+   18000cf27:	and    $0x63,%al
+   18000cf29:	push   $0x745f7261
+   18000cf2e:	jb     0x18000cf91
+   18000cf30:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000cf38:	fs rex
+   18000cf3a:	rex
+   18000cf3b:	rex jae 0x18000cfb2
+   18000cf3e:	fs rex
+   18000cf40:	rex
+   18000cf41:	rex.WB
+   18000cf42:	rex.RB
+   18000cf43:	rex.B
+   18000cf44:	push   %r8
+   18000cf46:	rex.RB
+   18000cf47:	rex.B
+   18000cf48:	rex.R pop %rax
+   18000cf4a:	pop    %rdx
+   18000cf4b:	add    %dh,%ch
+   18000cf4d:	add    %edi,(%rdi)
+   18000cf4f:	pop    %rdi
+   18000cf50:	rex.WB outsb %ds:(%rsi),(%dx)
+   18000cf52:	imul   $0x73616224,0x3f(%rax,%rax,2),%esi
+   18000cf5a:	imul   $0x65727473,0x5f(%rbx),%esp
+   18000cf61:	(bad)
+   18000cf62:	insl   (%dx),%es:(%rdi)
+   18000cf63:	(bad)
+   18000cf68:	push   %rbp
+   18000cf69:	(bad)
+   18000cf6a:	and    $0x63,%al
+   18000cf6c:	push   $0x745f7261
+   18000cf71:	jb     0x18000cfd4
+   18000cf73:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000cf7b:	fs rex
+   18000cf7d:	rex
+   18000cf7e:	rex jae 0x18000cff5
+   18000cf81:	fs rex
+   18000cf83:	rex
+   18000cf84:	rex.WB
+   18000cf85:	rex.RB
+   18000cf86:	rex.B
+   18000cf87:	pop    %r8
+   18000cf89:	pop    %rax
+   18000cf8a:	pop    %rdx
+   18000cf8b:	add    %dh,%ah
+   18000cf8d:	add    %edi,(%rdi)
+   18000cf8f:	pop    %rdi
+   18000cf90:	rex.WB outsb %ds:(%rsi),(%dx)
+   18000cf92:	imul   $0x73616224,0x3f(%rax,%rax,2),%esi
+   18000cf9a:	imul   $0x65727473,0x5f(%rbx),%esp
+   18000cfa1:	(bad)
+   18000cfa2:	insl   (%dx),%es:(%rdi)
+   18000cfa3:	(bad)
+   18000cfa8:	push   %rbp
+   18000cfa9:	(bad)
+   18000cfaa:	and    $0x63,%al
+   18000cfac:	push   $0x745f7261
+   18000cfb1:	jb     0x18000d014
+   18000cfb3:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000cfbb:	fs rex
+   18000cfbd:	rex
+   18000cfbe:	rex jae 0x18000d035
+   18000cfc1:	fs rex
+   18000cfc3:	rex
+   18000cfc4:	rex.WB
+   18000cfc5:	rex.RB
+   18000cfc6:	rex.B
+   18000cfc7:	pop    %r8
+   18000cfc9:	push   %rax
+   18000cfca:	rex.RB
+   18000cfcb:	push   %r8
+   18000cfcd:	rex.RB
+   18000cfce:	rex.B
+   18000cfcf:	xor    %r10b,0x45(%rax)
+   18000cfd3:	rex.B
+   18000cfd4:	rex.W xor %sil,(%rax)
+   18000cfd7:	xor    %eax,0x5a(%rax)
+   18000cfda:	add    %al,(%rax)
+   18000cfdc:	rex.XB add $0x6773783f,%eax
+   18000cfe2:	gs je  0x18000d053
+   18000cfe5:	rex (bad)
+   18000cfe7:	and    $0x62,%al
+   18000cfe9:	(bad)
+   18000cfea:	jae    0x18000d055
+   18000cfec:	movsxd 0x73(%rdi),%ebx
+   18000cfef:	je     0x18000d063
+   18000cff1:	gs (bad)
+   18000cff3:	insl   (%dx),%es:(%rdi)
+   18000cff4:	(bad)
+   18000cff9:	push   %rbp
+   18000cffa:	(bad)
+   18000cffb:	and    $0x63,%al
+   18000cffd:	push   $0x745f7261
+   18000d002:	jb     0x18000d065
+   18000d004:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d00c:	fs rex
+   18000d00e:	rex
+   18000d00f:	rex jae 0x18000d086
+   18000d012:	fs rex
+   18000d014:	rex
+   18000d015:	rex.WRB
+   18000d016:	rex.RB
+   18000d017:	rex.B
+   18000d018:	pop    %r15
+   18000d01a:	rex.WX push %rax
+   18000d01c:	rex.RB
+   18000d01d:	rex.B
+   18000d01e:	rex.R pop %rdi
+   18000d020:	rex.WX
+   18000d021:	rex pop %rdx
+   18000d023:	add    %al,0x5(%rsi)
+   18000d026:	(bad)
+   18000d027:	js     0x18000d09c
+   18000d029:	jo     0x18000d0a0
+   18000d02b:	je     0x18000d09b
+   18000d02d:	rex (bad)
+   18000d02f:	and    $0x62,%al
+   18000d031:	(bad)
+   18000d032:	jae    0x18000d09d
+   18000d034:	movsxd 0x73(%rdi),%ebx
+   18000d037:	je     0x18000d0ab
+   18000d039:	gs (bad)
+   18000d03b:	insl   (%dx),%es:(%rdi)
+   18000d03c:	(bad)
+   18000d041:	push   %rbp
+   18000d042:	(bad)
+   18000d043:	and    $0x63,%al
+   18000d045:	push   $0x745f7261
+   18000d04a:	jb     0x18000d0ad
+   18000d04c:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d054:	fs rex
+   18000d056:	rex
+   18000d057:	rex jae 0x18000d0ce
+   18000d05a:	fs rex
+   18000d05c:	rex
+   18000d05d:	rex.WRB
+   18000d05e:	rex.RB
+   18000d05f:	rex.B
+   18000d060:	pop    %r15
+   18000d062:	rex.WX push %rax
+   18000d064:	rex.RB
+   18000d065:	rex.X
+   18000d066:	rex.R pop %rdi
+   18000d068:	rex.WX
+   18000d069:	rex pop %rdx
+   18000d06b:	add    %bh,0x0(%rbp)
+   18000d06e:	(bad)
+   18000d06f:	(bad)
+   18000d070:	xor    %edi,(%rdi)
+   18000d072:	and    $0x62,%al
+   18000d074:	(bad)
+   18000d075:	jae    0x18000d0e0
+   18000d077:	movsxd 0x69(%rdi),%ebx
+   18000d07a:	outsl  %ds:(%rsi),(%dx)
+   18000d07b:	jae    0x18000d0bd
+   18000d07d:	rex.R push %rbp
    18000d07f:	(bad)
-   18000d080:	jae    0x18000d0eb
-   18000d082:	movsxd 0x69(%rdi),%ebx
-   18000d085:	outsl  %ds:(%rsi),(%dx)
-   18000d086:	jae    0x18000d0c8
-   18000d088:	rex.R push %rbp
-   18000d08a:	(bad)
-   18000d08b:	and    $0x63,%al
-   18000d08d:	push   $0x745f7261
-   18000d092:	jb     0x18000d0f5
-   18000d094:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000d09c:	fs rex
-   18000d09e:	rex
-   18000d09f:	rex jae 0x18000d116
-   18000d0a2:	fs rex
-   18000d0a4:	rex push %rcx
-   18000d0a6:	rex.RB
-   18000d0a7:	rex.B
-   18000d0a8:	pop    %r8
-   18000d0aa:	rex.W pop %rdi
-   18000d0ac:	rex.WRX
-   18000d0ad:	rex pop %rdx
-   18000d0af:	add    %cl,(%rax,%rax,1)
-   18000d0b2:	(bad)
-   18000d0b3:	(bad)
-   18000d0b4:	xor    %bh,(%rdi)
-   18000d0b6:	and    $0x62,%al
-   18000d0b8:	(bad)
-   18000d0b9:	jae    0x18000d124
-   18000d0bb:	movsxd 0x69(%rdi),%ebx
-   18000d0be:	outsl  %ds:(%rsi),(%dx)
-   18000d0bf:	jae    0x18000d101
-   18000d0c1:	rex.R push %rbp
-   18000d0c3:	(bad)
-   18000d0c4:	and    $0x63,%al
-   18000d0c6:	push   $0x745f7261
-   18000d0cb:	jb     0x18000d12e
-   18000d0cd:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000d0d5:	fs rex
-   18000d0d7:	rex
-   18000d0d8:	rex jae 0x18000d14f
-   18000d0db:	fs rex
-   18000d0dd:	rex
-   18000d0de:	rex.WB
-   18000d0df:	rex.RB
-   18000d0e0:	rex.B
-   18000d0e1:	rex.B
-   18000d0e2:	rex pop %rax
-   18000d0e4:	pop    %rdx
-   18000d0e5:	add    %al,0x3f(%rdx,%rax,1)
-   18000d0e9:	pop    %rdi
-   18000d0ea:	rex.WRXB jae 0x18000d153
-   18000d0ed:	js     0x18000d12f
+   18000d080:	and    $0x63,%al
+   18000d082:	push   $0x745f7261
+   18000d087:	jb     0x18000d0ea
+   18000d089:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d091:	fs rex
+   18000d093:	rex
+   18000d094:	rex jae 0x18000d10b
+   18000d097:	fs rex
+   18000d099:	rex push %rbp
+   18000d09b:	rex.RB
+   18000d09c:	rex.B
+   18000d09d:	rex.B
+   18000d09e:	rex pop %rax
+   18000d0a0:	pop    %rdx
+   18000d0a1:	add    %ah,0x6c633f02(%rsi)
+   18000d0a7:	gs (bad)
+   18000d0a9:	jb     0x18000d0eb
+   18000d0ab:	(bad)
+   18000d0ac:	and    $0x62,%al
+   18000d0ae:	(bad)
+   18000d0af:	jae    0x18000d11a
+   18000d0b1:	movsxd 0x69(%rdi),%ebx
+   18000d0b4:	outsl  %ds:(%rsi),(%dx)
+   18000d0b5:	jae    0x18000d0f7
+   18000d0b7:	rex.R push %rbp
+   18000d0b9:	(bad)
+   18000d0ba:	and    $0x63,%al
+   18000d0bc:	push   $0x745f7261
+   18000d0c1:	jb     0x18000d124
+   18000d0c3:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d0cb:	fs rex
+   18000d0cd:	rex
+   18000d0ce:	rex jae 0x18000d145
+   18000d0d1:	fs rex
+   18000d0d3:	rex push %rcx
+   18000d0d5:	rex.RB
+   18000d0d6:	rex.B
+   18000d0d7:	pop    %r8
+   18000d0d9:	rex.W pop %rdi
+   18000d0db:	rex.WRX
+   18000d0dc:	rex pop %rdx
+   18000d0de:	add    %al,(%rax)
+   18000d0e0:	(bad)
+   18000d0e3:	jae    0x18000d14a
+   18000d0e5:	je     0x18000d15a
+   18000d0e7:	je     0x18000d14a
+   18000d0e9:	je     0x18000d150
+   18000d0eb:	rex (bad)
+   18000d0ed:	and    $0x62,%al
    18000d0ef:	(bad)
-   18000d0f0:	and    $0x62,%al
-   18000d0f2:	(bad)
-   18000d0f3:	jae    0x18000d15e
-   18000d0f5:	movsxd 0x6f(%rdi),%ebx
-   18000d0f8:	jae    0x18000d16e
-   18000d0fa:	jb     0x18000d161
-   18000d0fc:	(bad)
-   18000d0fd:	insl   (%dx),%es:(%rdi)
-   18000d0fe:	rex
-   18000d0ff:	rex.R push %rbp
-   18000d101:	(bad)
-   18000d102:	and    $0x63,%al
-   18000d104:	push   $0x745f7261
-   18000d109:	jb     0x18000d16c
-   18000d10b:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000d113:	fs rex
-   18000d115:	rex
-   18000d116:	rex jae 0x18000d18d
-   18000d119:	fs rex
-   18000d11b:	rex push %rcx
-   18000d11d:	rex.RB
-   18000d11e:	rex.B
-   18000d11f:	pop    %r8
-   18000d121:	pop    %rax
-   18000d122:	pop    %rdx
-   18000d123:	add    %al,(%rax)
-   18000d125:	add    %edi,(%rdi)
-   18000d127:	(bad)
-   18000d128:	ss (bad)
-   18000d12a:	and    $0x62,%al
-   18000d12c:	(bad)
-   18000d12d:	jae    0x18000d198
-   18000d12f:	movsxd 0x6f(%rdi),%ebx
-   18000d132:	jae    0x18000d1a8
-   18000d134:	jb     0x18000d19b
-   18000d136:	(bad)
-   18000d137:	insl   (%dx),%es:(%rdi)
-   18000d138:	rex
-   18000d139:	rex.R push %rbp
-   18000d13b:	(bad)
-   18000d13c:	and    $0x63,%al
-   18000d13e:	push   $0x745f7261
-   18000d143:	jb     0x18000d1a6
-   18000d145:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000d14d:	fs rex
-   18000d14f:	rex
-   18000d150:	rex jae 0x18000d1c7
-   18000d153:	fs rex
-   18000d155:	rex push %rcx
-   18000d157:	rex.RB
-   18000d158:	rex.B
-   18000d159:	rex.B
-   18000d15a:	rex.B
-   18000d15b:	rex.RB
-   18000d15c:	push   %r14
-   18000d15e:	xor    %dh,(%rcx)
-   18000d160:	rex
-   18000d161:	rex.WB
-   18000d162:	rex pop %rdx
-   18000d164:	add    %al,(%rax)
-   18000d166:	add    $0x1,%al
-   18000d168:	(bad)
-   18000d169:	(bad)
-   18000d16a:	ss (bad)
-   18000d16c:	and    $0x62,%al
-   18000d16e:	(bad)
-   18000d16f:	jae    0x18000d1da
-   18000d171:	movsxd 0x6f(%rdi),%ebx
-   18000d174:	jae    0x18000d1ea
-   18000d176:	jb     0x18000d1dd
-   18000d178:	(bad)
-   18000d179:	insl   (%dx),%es:(%rdi)
-   18000d17a:	rex
-   18000d17b:	rex.R push %rbp
-   18000d17d:	(bad)
-   18000d17e:	and    $0x63,%al
-   18000d180:	push   $0x745f7261
-   18000d185:	jb     0x18000d1e8
-   18000d187:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000d18f:	fs rex
-   18000d191:	rex
-   18000d192:	rex jae 0x18000d209
-   18000d195:	fs rex
-   18000d197:	rex push %rcx
-   18000d199:	rex.RB
-   18000d19a:	rex.B
-   18000d19b:	rex.B
-   18000d19c:	rex.B
-   18000d19d:	rex.RB
-   18000d19e:	push   %r14
-   18000d1a0:	xor    %dh,(%rcx)
-   18000d1a2:	rex
-   18000d1a3:	rex.WRX
-   18000d1a4:	rex pop %rdx
-   18000d1a6:	add    %al,(%rax)
-   18000d1a8:	push   $0x6c663f03
-   18000d1ad:	jne    0x18000d222
-   18000d1af:	push   $0x62243f40
-   18000d1b4:	(bad)
-   18000d1b5:	jae    0x18000d220
-   18000d1b7:	movsxd 0x6f(%rdi),%ebx
-   18000d1ba:	jae    0x18000d230
-   18000d1bc:	jb     0x18000d223
-   18000d1be:	(bad)
-   18000d1bf:	insl   (%dx),%es:(%rdi)
-   18000d1c0:	rex
-   18000d1c1:	rex.R push %rbp
-   18000d1c3:	(bad)
-   18000d1c4:	and    $0x63,%al
-   18000d1c6:	push   $0x745f7261
-   18000d1cb:	jb     0x18000d22e
-   18000d1cd:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000d1d5:	fs rex
-   18000d1d7:	rex
-   18000d1d8:	rex jae 0x18000d24f
-   18000d1db:	fs rex
-   18000d1dd:	rex push %rcx
-   18000d1df:	rex.RB
-   18000d1e0:	rex.B
-   18000d1e1:	rex.B
-   18000d1e2:	rex.B
-   18000d1e3:	rex.RB
-   18000d1e4:	push   %r14
-   18000d1e6:	xor    %esi,(%rdx)
-   18000d1e8:	rex pop %rax
-   18000d1ea:	pop    %rdx
-   18000d1eb:	add    %dl,(%rbx)
-   18000d1ed:	add    %bh,(%rdi)
-   18000d1ef:	(bad)
-   18000d1f0:	xor    %bh,(%rdi)
-   18000d1f2:	and    $0x62,%al
-   18000d1f4:	(bad)
-   18000d1f5:	jae    0x18000d260
-   18000d1f7:	movsxd 0x69(%rdi),%ebx
-   18000d1fa:	outsl  %ds:(%rsi),(%dx)
-   18000d1fb:	jae    0x18000d271
-   18000d1fd:	jb     0x18000d264
-   18000d1ff:	(bad)
-   18000d200:	insl   (%dx),%es:(%rdi)
+   18000d0f0:	jae    0x18000d15b
+   18000d0f2:	movsxd 0x69(%rdi),%ebx
+   18000d0f5:	outsl  %ds:(%rsi),(%dx)
+   18000d0f6:	jae    0x18000d138
+   18000d0f8:	rex.R push %rbp
+   18000d0fa:	(bad)
+   18000d0fb:	and    $0x63,%al
+   18000d0fd:	push   $0x745f7261
+   18000d102:	jb     0x18000d165
+   18000d104:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d10c:	fs rex
+   18000d10e:	rex
+   18000d10f:	rex jae 0x18000d186
+   18000d112:	fs rex
+   18000d114:	rex push %rcx
+   18000d116:	rex.RB
+   18000d117:	rex.B
+   18000d118:	pop    %r8
+   18000d11a:	rex.W pop %rdi
+   18000d11c:	rex.WRX
+   18000d11d:	rex pop %rdx
+   18000d11f:	add    %cl,(%rax,%rax,1)
+   18000d122:	(bad)
+   18000d123:	(bad)
+   18000d124:	xor    %bh,(%rdi)
+   18000d126:	and    $0x62,%al
+   18000d128:	(bad)
+   18000d129:	jae    0x18000d194
+   18000d12b:	movsxd 0x69(%rdi),%ebx
+   18000d12e:	outsl  %ds:(%rsi),(%dx)
+   18000d12f:	jae    0x18000d171
+   18000d131:	rex.R push %rbp
+   18000d133:	(bad)
+   18000d134:	and    $0x63,%al
+   18000d136:	push   $0x745f7261
+   18000d13b:	jb     0x18000d19e
+   18000d13d:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d145:	fs rex
+   18000d147:	rex
+   18000d148:	rex jae 0x18000d1bf
+   18000d14b:	fs rex
+   18000d14d:	rex
+   18000d14e:	rex.WB
+   18000d14f:	rex.RB
+   18000d150:	rex.B
+   18000d151:	rex.B
+   18000d152:	rex pop %rax
+   18000d154:	pop    %rdx
+   18000d155:	add    %al,0x3f(%rdx,%rax,1)
+   18000d159:	pop    %rdi
+   18000d15a:	rex.WRXB jae 0x18000d1c3
+   18000d15d:	js     0x18000d19f
+   18000d15f:	(bad)
+   18000d160:	and    $0x62,%al
+   18000d162:	(bad)
+   18000d163:	jae    0x18000d1ce
+   18000d165:	movsxd 0x6f(%rdi),%ebx
+   18000d168:	jae    0x18000d1de
+   18000d16a:	jb     0x18000d1d1
+   18000d16c:	(bad)
+   18000d16d:	insl   (%dx),%es:(%rdi)
+   18000d16e:	rex
+   18000d16f:	rex.R push %rbp
+   18000d171:	(bad)
+   18000d172:	and    $0x63,%al
+   18000d174:	push   $0x745f7261
+   18000d179:	jb     0x18000d1dc
+   18000d17b:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d183:	fs rex
+   18000d185:	rex
+   18000d186:	rex jae 0x18000d1fd
+   18000d189:	fs rex
+   18000d18b:	rex push %rcx
+   18000d18d:	rex.RB
+   18000d18e:	rex.B
+   18000d18f:	pop    %r8
+   18000d191:	pop    %rax
+   18000d192:	pop    %rdx
+   18000d193:	add    %al,(%rax)
+   18000d195:	add    %edi,(%rdi)
+   18000d197:	(bad)
+   18000d198:	ss (bad)
+   18000d19a:	and    $0x62,%al
+   18000d19c:	(bad)
+   18000d19d:	jae    0x18000d208
+   18000d19f:	movsxd 0x6f(%rdi),%ebx
+   18000d1a2:	jae    0x18000d218
+   18000d1a4:	jb     0x18000d20b
+   18000d1a6:	(bad)
+   18000d1a7:	insl   (%dx),%es:(%rdi)
+   18000d1a8:	rex
+   18000d1a9:	rex.R push %rbp
+   18000d1ab:	(bad)
+   18000d1ac:	and    $0x63,%al
+   18000d1ae:	push   $0x745f7261
+   18000d1b3:	jb     0x18000d216
+   18000d1b5:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d1bd:	fs rex
+   18000d1bf:	rex
+   18000d1c0:	rex jae 0x18000d237
+   18000d1c3:	fs rex
+   18000d1c5:	rex push %rcx
+   18000d1c7:	rex.RB
+   18000d1c8:	rex.B
+   18000d1c9:	rex.B
+   18000d1ca:	rex.B
+   18000d1cb:	rex.RB
+   18000d1cc:	push   %r14
+   18000d1ce:	xor    %dh,(%rcx)
+   18000d1d0:	rex
+   18000d1d1:	rex.WB
+   18000d1d2:	rex pop %rdx
+   18000d1d4:	add    %al,(%rax)
+   18000d1d6:	add    $0x1,%al
+   18000d1d8:	(bad)
+   18000d1d9:	(bad)
+   18000d1da:	ss (bad)
+   18000d1dc:	and    $0x62,%al
+   18000d1de:	(bad)
+   18000d1df:	jae    0x18000d24a
+   18000d1e1:	movsxd 0x6f(%rdi),%ebx
+   18000d1e4:	jae    0x18000d25a
+   18000d1e6:	jb     0x18000d24d
+   18000d1e8:	(bad)
+   18000d1e9:	insl   (%dx),%es:(%rdi)
+   18000d1ea:	rex
+   18000d1eb:	rex.R push %rbp
+   18000d1ed:	(bad)
+   18000d1ee:	and    $0x63,%al
+   18000d1f0:	push   $0x745f7261
+   18000d1f5:	jb     0x18000d258
+   18000d1f7:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d1ff:	fs rex
    18000d201:	rex
-   18000d202:	rex.R push %rbp
-   18000d204:	(bad)
-   18000d205:	and    $0x63,%al
-   18000d207:	push   $0x745f7261
-   18000d20c:	jb     0x18000d26f
-   18000d20e:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000d216:	fs rex
-   18000d218:	rex
-   18000d219:	rex jae 0x18000d290
-   18000d21c:	fs rex
-   18000d21e:	rex push %rcx
-   18000d220:	rex.RB
-   18000d221:	rex.B
-   18000d222:	rex.B
-   18000d223:	rex push %rax
-   18000d225:	rex.RB
-   18000d226:	push   %r14
-   18000d228:	(bad)
-   18000d229:	and    $0x62,%al
-   18000d22b:	(bad)
-   18000d22c:	jae    0x18000d297
-   18000d22e:	movsxd 0x73(%rdi),%ebx
-   18000d231:	je     0x18000d2a5
-   18000d233:	gs (bad)
-   18000d235:	insl   (%dx),%es:(%rdi)
-   18000d236:	(bad)
-   18000d23b:	push   %rbp
-   18000d23c:	(bad)
-   18000d23d:	and    $0x63,%al
-   18000d23f:	push   $0x745f7261
-   18000d244:	jb     0x18000d2a7
-   18000d246:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000d24e:	fs rex
-   18000d250:	rex
-   18000d251:	rex xor %eax,0x40(%rax)
-   18000d255:	pop    %rdx
-   18000d256:	add    %al,(%rax)
-   18000d258:	addb   $0x3f,(%rax)
-   18000d25b:	(bad)
-   18000d25c:	xor    %edi,(%rdi)
-   18000d25e:	and    $0x62,%al
-   18000d260:	(bad)
-   18000d261:	jae    0x18000d2cc
-   18000d263:	movsxd 0x69(%rdi),%ebx
-   18000d266:	outsl  %ds:(%rsi),(%dx)
-   18000d267:	jae    0x18000d2dd
-   18000d269:	jb     0x18000d2d0
-   18000d26b:	(bad)
-   18000d26c:	insl   (%dx),%es:(%rdi)
-   18000d26d:	rex
-   18000d26e:	rex.R push %rbp
-   18000d270:	(bad)
-   18000d271:	and    $0x63,%al
-   18000d273:	push   $0x745f7261
-   18000d278:	jb     0x18000d2db
-   18000d27a:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000d282:	fs rex
-   18000d284:	rex
-   18000d285:	rex jae 0x18000d2fc
-   18000d288:	fs rex
-   18000d28a:	rex push %rbp
-   18000d28c:	rex.RB
-   18000d28d:	rex.B
-   18000d28e:	rex.B
-   18000d28f:	rex pop %rax
-   18000d291:	pop    %rdx
-   18000d292:	add    %al,(%rax)
-   18000d294:	stos   %eax,%es:(%rdi)
-   18000d295:	add    %edi,(%rdi)
-   18000d297:	pop    %rdi
-   18000d298:	rex.RX imul $0x73406e65,0x70(%rdi),%r13d
-   18000d2a0:	je     0x18000d306
-   18000d2a2:	rex
-   18000d2a3:	rex pop %rcx
-   18000d2a5:	push   %r8
-   18000d2a7:	rex.RB
-   18000d2a8:	push   %r13
-   18000d2aa:	pop    %rdi
-   18000d2ab:	imul   $0x40406675,0x62(%rdi),%ebp
-   18000d2b2:	push   %rax
-   18000d2b3:	rex.RB
-   18000d2b4:	rex.X
-   18000d2b5:	rex.R
-   18000d2b6:	rex.W
-   18000d2b7:	rex.W
-   18000d2b8:	rex pop %rdx
-   18000d2ba:	add    %al,(%rax)
-   18000d2bc:	(bad)
-   18000d2bd:	add    $0x3f,%al
-   18000d2bf:	jae    0x18000d329
-   18000d2c1:	outsl  %ds:(%rsi),(%dx)
-   18000d2c2:	ja     0x18000d331
-   18000d2c4:	(bad)
-   18000d2c5:	outsb  %ds:(%rsi),(%dx)
-   18000d2c6:	jns    0x18000d32b
-   18000d2c8:	rex (bad)
-   18000d2ca:	and    $0x62,%al
-   18000d2cc:	(bad)
-   18000d2cd:	jae    0x18000d338
-   18000d2cf:	movsxd 0x73(%rdi),%ebx
-   18000d2d2:	je     0x18000d346
-   18000d2d4:	gs (bad)
-   18000d2d6:	insl   (%dx),%es:(%rdi)
-   18000d2d7:	(bad)
-   18000d2dc:	push   %rbp
-   18000d2dd:	(bad)
-   18000d2de:	and    $0x63,%al
-   18000d2e0:	push   $0x745f7261
-   18000d2e5:	jb     0x18000d348
-   18000d2e7:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
-   18000d2ef:	fs rex
-   18000d2f1:	rex
-   18000d2f2:	rex jae 0x18000d369
-   18000d2f5:	fs rex
-   18000d2f7:	rex
-   18000d2f8:	rex.WRB
-   18000d2f9:	rex.RB
-   18000d2fa:	rex.B
-   18000d2fb:	pop    %r15
-   18000d2fd:	rex.WX pop %rax
-   18000d2ff:	pop    %rdx
-   18000d300:	add    %al,(%rax)
-   18000d302:	leave
-   18000d303:	add    (%rdi),%edi
-   18000d305:	imul   $0x646f6324,0x3f(%rax,%rax,2),%esp
-   18000d30d:	movsxd %gs:0x74(%rsi),%esi
-   18000d311:	rex
-   18000d312:	rex.R
-   18000d313:	rex.R push %rbp
-   18000d315:	pop    %rdi
-   18000d316:	(bad)
-   18000d31c:	gs je  0x18000d35f
-   18000d31f:	rex
-   18000d320:	rex jae 0x18000d397
-   18000d323:	fs rex
-   18000d325:	rex xor 0x30(%rsi),%dl
-   18000d329:	insb   (%dx),%es:(%rdi)
-   18000d32a:	outsl  %ds:(%rsi),(%dx)
-   18000d32b:	movsxd 0x6c(%rcx),%esp
-   18000d32e:	rex xor %gs:0x41(%rax),%al
-   18000d333:	add    %cl,0x53(%rbp)
-   18000d336:	push   %rsi
-   18000d337:	rex.XB push %r8
-   18000d339:	xor    %esi,(%rax,%rsi,1)
-   18000d33c:	cs fs insb (%dx),%es:(%rdi)
-   18000d33f:	insb   (%dx),%es:(%rdi)
-   18000d340:	add    %al,(%rax)
-   18000d342:	add    %al,(%rax)
-   18000d344:	pop    %rdi
-   18000d345:	pop    %rdi
-   18000d346:	rex.XB js 0x18000d3c1
-   18000d349:	rex.RX jb 0x18000d3ad
-   18000d34c:	insl   (%dx),%es:(%rdi)
-   18000d34d:	gs rex.W (bad)
-   18000d350:	outsb  %ds:(%rsi),(%dx)
-   18000d351:	fs insb (%dx),%es:(%rdi)
-   18000d353:	gs jb  0x18000d38a
-   18000d356:	add    %al,(%rax)
-   18000d358:	sbb    %al,(%rax)
-   18000d35a:	pop    %rdi
-   18000d35b:	pop    %rdi
-   18000d35c:	push   %rdx
-   18000d35d:	push   %rsp
-   18000d35e:	rex.R jns 0x18000d3cf
-   18000d361:	(bad)
-   18000d362:	insl   (%dx),%es:(%rdi)
-   18000d363:	imul   $0x747361,0x43(%rbx),%esp
-   18000d36a:	and    (%rax),%eax
-   18000d36c:	pop    %rdi
-   18000d36d:	pop    %rdi
-   18000d36e:	jae    0x18000d3e4
-   18000d370:	fs pop %rdi
-   18000d372:	je     0x18000d3d9
-   18000d374:	jb     0x18000d3e3
-   18000d376:	imul   $0x21006574,0x61(%rsi),%ebp
-   18000d37d:	add    %bl,0x5f(%rdi)
-   18000d380:	jae    0x18000d3f6
-   18000d382:	fs pop %rdi
-   18000d384:	gs js  0x18000d3ea
-   18000d387:	gs jo  0x18000d3fe
-   18000d38a:	imul   $0x706f635f,0x6e(%rdi),%ebp
-   18000d391:	jns    0x18000d393
-   18000d393:	add    %ah,(%rdx)
-   18000d395:	add    %bl,0x5f(%rdi)
-   18000d398:	jae    0x18000d40e
-   18000d39a:	fs pop %rdi
-   18000d39c:	gs js  0x18000d402
-   18000d39f:	gs jo  0x18000d416
-   18000d3a2:	imul   $0x7365645f,0x6e(%rdi),%ebp
-   18000d3a9:	je     0x18000d41d
-   18000d3ab:	outsl  %ds:(%rsi),(%dx)
-   18000d3ac:	jns    0x18000d3ae
-   18000d3ae:	(bad)
-   18000d3af:	add    %bl,0x5f(%rdi)
-   18000d3b2:	jae    0x18000d428
-   18000d3b4:	fs pop %rdi
-   18000d3b6:	je     0x18000d431
-   18000d3b8:	jo     0x18000d41f
-   18000d3ba:	pop    %rdi
-   18000d3bb:	imul   $0x616e5f6f,0x66(%rsi),%ebp
-   18000d3c2:	insl   (%dx),%es:(%rdi)
-   18000d3c3:	add    %al,%gs:(%rax)
-   18000d3c6:	add    %eax,(%rax)
-   18000d3c8:	pop    %rdi
-   18000d3c9:	rex.XB js 0x18000d444
-   18000d3cc:	push   %rsp
-   18000d3cd:	push   $0x45776f72
-   18000d3d2:	js     0x18000d437
-   18000d3d4:	gs jo  0x18000d44b
-   18000d3d7:	imul   $0x3c0000,0x6e(%rdi),%ebp
-   18000d3de:	insl   (%dx),%es:(%rdi)
-   18000d3df:	gs insl (%dx),%es:(%rdi)
-   18000d3e1:	movsxd 0x79(%rax),%esi
-   18000d3e4:	add    %al,(%rax)
-   18000d3e6:	cmp    $0x6d656d00,%eax
-   18000d3eb:	insl   (%dx),%es:(%rdi)
-   18000d3ec:	outsl  %ds:(%rsi),(%dx)
-   18000d3ed:	jbe    0x18000d454
-   18000d3ef:	add    %bh,(%rsi)
-   18000d3f1:	add    %ch,0x65(%rbp)
-   18000d3f4:	insl   (%dx),%es:(%rdi)
-   18000d3f5:	jae    0x18000d45c
-   18000d3f7:	je     0x18000d3f9
-   18000d3f9:	add    %bl,(%rbx)
-   18000d3fb:	add    %bl,0x5f(%rdi)
-   18000d3fe:	movsxd 0x72(%rbp),%esi
-   18000d401:	jb     0x18000d468
-   18000d403:	outsb  %ds:(%rsi),(%dx)
-   18000d404:	je     0x18000d465
-   18000d406:	gs js  0x18000d46c
-   18000d409:	gs jo  0x18000d480
-   18000d40c:	imul   $0x5f001c00,0x6e(%rdi),%ebp
-   18000d413:	pop    %rdi
-   18000d414:	movsxd 0x72(%rbp),%esi
-   18000d417:	jb     0x18000d47e
-   18000d419:	outsb  %ds:(%rsi),(%dx)
-   18000d41a:	je     0x18000d47b
-   18000d41c:	gs js  0x18000d482
-   18000d41f:	gs jo  0x18000d496
-   18000d422:	imul   $0x6e6f635f,0x6e(%rdi),%ebp
-   18000d429:	je     0x18000d490
-   18000d42b:	js     0x18000d4a1
-   18000d42d:	add    %cl,(%rax)
-   18000d42f:	add    %bl,0x5f(%rdi)
-   18000d432:	rex.XB pop %r15
-   18000d434:	jae    0x18000d4a6
-   18000d436:	movsxd %gs:0x66(%rcx),%ebp
-   18000d43a:	imul   $0x646e6168,0x5f(%rbx),%esp
-   18000d441:	insb   (%dx),%es:(%rdi)
-   18000d442:	gs jb  0x18000d445
-   18000d445:	add    %ah,0x735f5f00(%rip)        # 0x1f360334b
-   18000d44b:	je     0x18000d4b1
-   18000d44d:	pop    %rdi
-   18000d44e:	je     0x18000d4c9
-   18000d450:	jo     0x18000d4b7
-   18000d452:	pop    %rdi
-   18000d453:	imul   $0x65645f6f,0x66(%rsi),%ebp
-   18000d45a:	jae    0x18000d4d0
-   18000d45c:	jb     0x18000d4cd
-   18000d45e:	jns    0x18000d4bf
-   18000d460:	insb   (%dx),%es:(%rdi)
-   18000d461:	imul   $0x43560000,0x74(%rbx),%esi
-   18000d468:	push   %rdx
-   18000d469:	push   %rbp
-   18000d46a:	rex.WRX push %rsp
-   18000d46c:	rex.WB
-   18000d46d:	rex.WRB
-   18000d46e:	xor    %r14d,(%r8,%rsi,1)
-   18000d472:	pop    %rdi
-   18000d473:	xor    %ebp,(%rsi)
-   18000d475:	fs insb (%dx),%es:(%rdi)
-   18000d477:	insb   (%dx),%es:(%rdi)
-   18000d478:	add    %al,(%rax)
-   18000d47a:	push   %rsi
-   18000d47b:	rex.XB push %r10
-   18000d47d:	push   %rbp
-   18000d47e:	rex.WRX push %rsp
-   18000d480:	rex.WB
-   18000d481:	rex.WRB
-   18000d482:	xor    %r14d,(%r8,%rsi,1)
-   18000d486:	cs fs insb (%dx),%es:(%rdi)
-   18000d489:	insb   (%dx),%es:(%rdi)
-   18000d48a:	add    %al,(%rax)
-   18000d48c:	cmp    %eax,(%rax)
-   18000d48e:	pop    %rdi
-   18000d48f:	imul   $0x64696c61,0x76(%rsi),%ebp
-   18000d496:	pop    %rdi
-   18000d497:	jo     0x18000d4fa
-   18000d499:	jb     0x18000d4fc
-   18000d49b:	insl   (%dx),%es:(%rdi)
-   18000d49c:	gs je  0x18000d504
-   18000d49f:	jb     0x18000d500
-   18000d4a1:	outsb  %ds:(%rsi),(%dx)
-   18000d4a2:	outsl  %ds:(%rsi),(%dx)
-   18000d4a3:	imul   $0x6f6e5f6f,0x66(%rsi),%ebp
-   18000d4aa:	jb     0x18000d511
-   18000d4ac:	je     0x18000d523
-   18000d4ae:	jb     0x18000d51e
-   18000d4b0:	add    %al,(%rax)
-   18000d4b2:	cmp    %eax,(%rax)
-   18000d4b4:	pop    %rdi
-   18000d4b5:	addr32 gs je 0x18000d518
-   18000d4b9:	jae    0x18000d52f
-   18000d4bb:	jb     0x18000d522
-   18000d4bd:	(bad)
-   18000d4be:	insl   (%dx),%es:(%rdi)
-   18000d4bf:	pop    %rdi
-   18000d4c0:	(bad)
-   18000d4c5:	jb     0x18000d526
-   18000d4c7:	jo     0x18000d538
-   18000d4c9:	imul   $0x737265,0x74(%rsi),%ebp
-   18000d4d0:	je     0x18000d4d2
-   18000d4d2:	movsxd 0x73(%rdi,%rbp,2),%bp
-   18000d4d7:	add    %al,%gs:(%rax)
-   18000d4da:	ja     0x18000d4dc
-   18000d4dc:	data16 data16 insb (%dx),%es:(%rdi)
-   18000d4df:	jne    0x18000d554
-   18000d4e1:	push   $0x780000
-   18000d4e6:	data16 addr32 gs je 0x18000d54e
-   18000d4eb:	add    %bh,0x0(%rcx)
-   18000d4ee:	data16 addr32 gs je 0x18000d563
-   18000d4f3:	outsl  %ds:(%rsi),(%dx)
-   18000d4f4:	jae    0x18000d4f6
-   18000d4f6:	jg     0x18000d4f8
-   18000d4f8:	data16 jo 0x18000d570
-   18000d4fb:	je     0x18000d560
-   18000d4fd:	add    %al,0x65726600(%rbx)
-   18000d503:	(bad)
-   18000d504:	add    %cl,%fs:0x65736600(%rax)
-   18000d50b:	je     0x18000d57d
-   18000d50d:	outsl  %ds:(%rsi),(%dx)
-   18000d50e:	jae    0x18000d510
-   18000d510:	(bad)
-   18000d511:	add    %bl,0x66(%rdi)
-   18000d514:	jae    0x18000d57b
-   18000d516:	imul   $0x34,%gs:0x36(%rcx),%ebp
-   18000d51b:	add    %cl,0x72776600(%rdx)
-   18000d521:	imul   $0x73009800,0x0(%rbp,%riz,2),%esi
-   18000d529:	gs je  0x18000d5a2
-   18000d52c:	(bad)
-   18000d531:	add    %dh,0x6e(%rbp)
-   18000d534:	addr32 gs je 0x18000d59b
-   18000d538:	add    %al,(%rax)
-   18000d53a:	(bad)
-   18000d53b:	add    %bl,0x6c(%rdi)
-   18000d53e:	outsl  %ds:(%rsi),(%dx)
-   18000d53f:	movsxd 0x5f(%rbx),%ebp
-   18000d542:	imul   $0x2400,0x0(%rbp,%riz,2),%bp
-   18000d549:	add    %bl,0x75(%rdi)
-   18000d54c:	outsb  %ds:(%rsi),(%dx)
-   18000d54d:	insb   (%dx),%es:(%rdi)
-   18000d54e:	outsl  %ds:(%rsi),(%dx)
-   18000d54f:	movsxd 0x5f(%rbx),%ebp
-   18000d552:	imul   $0x1600,0x0(%rbp,%riz,2),%bp
-   18000d559:	add    %esi,0x71(%rbx)
-   18000d55c:	jb     0x18000d5d2
-   18000d55e:	add    %al,(%rax)
-   18000d560:	add    %dh,0x72(%ebp,%eiz,2)
-   18000d565:	insl   (%dx),%es:(%rdi)
-   18000d566:	imul   $0x8006574,0x61(%rsi),%ebp
-   18000d56d:	add    %bl,0x63(%rdi)
-   18000d570:	(bad)
-   18000d571:	insb   (%dx),%es:(%rdi)
-   18000d572:	insb   (%dx),%es:(%rdi)
-   18000d573:	outsb  %ds:(%rsi),(%dx)
-   18000d574:	gs ja  0x18000d5df
-   18000d577:	add    %bl,(%rcx)
-   18000d579:	add    %ch,0x61(%rbp)
-   18000d57c:	insb   (%dx),%es:(%rdi)
-   18000d57d:	insb   (%dx),%es:(%rdi)
-   18000d57e:	outsl  %ds:(%rsi),(%dx)
-   18000d57f:	movsxd (%rax),%eax
-   18000d581:	add    %dh,(%rsi)
-   18000d583:	add    %bl,0x69(%rdi)
-   18000d586:	outsb  %ds:(%rsi),(%dx)
-   18000d587:	imul   $0x37006d72,0x65(%rsp,%rsi,2),%esi
-   18000d58f:	add    %bl,0x69(%rdi)
-   18000d592:	outsb  %ds:(%rsi),(%dx)
-   18000d593:	imul   $0x655f6d72,0x65(%rsp,%rsi,2),%esi
-   18000d59b:	add    %bh,(%rdi)
-   18000d59d:	add    %bl,0x73(%rdi)
-   18000d5a0:	gs push $0x6c69665f
-   18000d5a6:	je     0x18000d60d
-   18000d5a8:	jb     0x18000d609
-   18000d5aa:	fs insb (%dx),%es:(%rdi)
-   18000d5ac:	insb   (%dx),%es:(%rdi)
-   18000d5ad:	add    %bl,(%rax)
-   18000d5af:	add    %bl,0x63(%rdi)
-   18000d5b2:	outsl  %ds:(%rsi),(%dx)
-   18000d5b3:	outsb  %ds:(%rsi),(%dx)
-   18000d5b4:	imul   $0x6572,0x75(%rdi),%sp
-   18000d5ba:	pop    %rdi
-   18000d5bb:	outsb  %ds:(%rsi),(%dx)
-   18000d5bc:	(bad)
-   18000d5bd:	jb     0x18000d631
-   18000d5bf:	outsl  %ds:(%rsi),(%dx)
-   18000d5c0:	ja     0x18000d621
-   18000d5c2:	(bad)
-   18000d5c3:	jb     0x18000d62c
-   18000d5c5:	jbe    0x18000d5c7
-   18000d5c7:	add    %dh,(%rbx)
-   18000d5c9:	add    %bl,0x69(%rdi)
-   18000d5cc:	outsb  %ds:(%rsi),(%dx)
-   18000d5cd:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
-   18000d5d5:	pop    %rdi
-   18000d5d6:	outsb  %ds:(%rsi),(%dx)
-   18000d5d7:	(bad)
-   18000d5d8:	jb     0x18000d64c
-   18000d5da:	outsl  %ds:(%rsi),(%dx)
-   18000d5db:	ja     0x18000d63c
-   18000d5dd:	outsb  %gs:(%rsi),(%dx)
-   18000d5df:	jbe    0x18000d64a
-   18000d5e1:	jb     0x18000d652
+   18000d202:	rex jae 0x18000d279
+   18000d205:	fs rex
+   18000d207:	rex push %rcx
+   18000d209:	rex.RB
+   18000d20a:	rex.B
+   18000d20b:	rex.B
+   18000d20c:	rex.B
+   18000d20d:	rex.RB
+   18000d20e:	push   %r14
+   18000d210:	xor    %dh,(%rcx)
+   18000d212:	rex
+   18000d213:	rex.WRX
+   18000d214:	rex pop %rdx
+   18000d216:	add    %al,(%rax)
+   18000d218:	push   $0x6c663f03
+   18000d21d:	jne    0x18000d292
+   18000d21f:	push   $0x62243f40
+   18000d224:	(bad)
+   18000d225:	jae    0x18000d290
+   18000d227:	movsxd 0x6f(%rdi),%ebx
+   18000d22a:	jae    0x18000d2a0
+   18000d22c:	jb     0x18000d293
+   18000d22e:	(bad)
+   18000d22f:	insl   (%dx),%es:(%rdi)
+   18000d230:	rex
+   18000d231:	rex.R push %rbp
+   18000d233:	(bad)
+   18000d234:	and    $0x63,%al
+   18000d236:	push   $0x745f7261
+   18000d23b:	jb     0x18000d29e
+   18000d23d:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d245:	fs rex
+   18000d247:	rex
+   18000d248:	rex jae 0x18000d2bf
+   18000d24b:	fs rex
+   18000d24d:	rex push %rcx
+   18000d24f:	rex.RB
+   18000d250:	rex.B
+   18000d251:	rex.B
+   18000d252:	rex.B
+   18000d253:	rex.RB
+   18000d254:	push   %r14
+   18000d256:	xor    %esi,(%rdx)
+   18000d258:	rex pop %rax
+   18000d25a:	pop    %rdx
+   18000d25b:	add    %dl,(%rbx)
+   18000d25d:	add    %bh,(%rdi)
+   18000d25f:	(bad)
+   18000d260:	xor    %bh,(%rdi)
+   18000d262:	and    $0x62,%al
+   18000d264:	(bad)
+   18000d265:	jae    0x18000d2d0
+   18000d267:	movsxd 0x69(%rdi),%ebx
+   18000d26a:	outsl  %ds:(%rsi),(%dx)
+   18000d26b:	jae    0x18000d2e1
+   18000d26d:	jb     0x18000d2d4
+   18000d26f:	(bad)
+   18000d270:	insl   (%dx),%es:(%rdi)
+   18000d271:	rex
+   18000d272:	rex.R push %rbp
+   18000d274:	(bad)
+   18000d275:	and    $0x63,%al
+   18000d277:	push   $0x745f7261
+   18000d27c:	jb     0x18000d2df
+   18000d27e:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d286:	fs rex
+   18000d288:	rex
+   18000d289:	rex jae 0x18000d300
+   18000d28c:	fs rex
+   18000d28e:	rex push %rcx
+   18000d290:	rex.RB
+   18000d291:	rex.B
+   18000d292:	rex.B
+   18000d293:	rex push %rax
+   18000d295:	rex.RB
+   18000d296:	push   %r14
+   18000d298:	(bad)
+   18000d299:	and    $0x62,%al
+   18000d29b:	(bad)
+   18000d29c:	jae    0x18000d307
+   18000d29e:	movsxd 0x73(%rdi),%ebx
+   18000d2a1:	je     0x18000d315
+   18000d2a3:	gs (bad)
+   18000d2a5:	insl   (%dx),%es:(%rdi)
+   18000d2a6:	(bad)
+   18000d2ab:	push   %rbp
+   18000d2ac:	(bad)
+   18000d2ad:	and    $0x63,%al
+   18000d2af:	push   $0x745f7261
+   18000d2b4:	jb     0x18000d317
+   18000d2b6:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d2be:	fs rex
+   18000d2c0:	rex
+   18000d2c1:	rex xor %eax,0x40(%rax)
+   18000d2c5:	pop    %rdx
+   18000d2c6:	add    %al,(%rax)
+   18000d2c8:	addb   $0x3f,(%rax)
+   18000d2cb:	(bad)
+   18000d2cc:	xor    %edi,(%rdi)
+   18000d2ce:	and    $0x62,%al
+   18000d2d0:	(bad)
+   18000d2d1:	jae    0x18000d33c
+   18000d2d3:	movsxd 0x69(%rdi),%ebx
+   18000d2d6:	outsl  %ds:(%rsi),(%dx)
+   18000d2d7:	jae    0x18000d34d
+   18000d2d9:	jb     0x18000d340
+   18000d2db:	(bad)
+   18000d2dc:	insl   (%dx),%es:(%rdi)
+   18000d2dd:	rex
+   18000d2de:	rex.R push %rbp
+   18000d2e0:	(bad)
+   18000d2e1:	and    $0x63,%al
+   18000d2e3:	push   $0x745f7261
+   18000d2e8:	jb     0x18000d34b
+   18000d2ea:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d2f2:	fs rex
+   18000d2f4:	rex
+   18000d2f5:	rex jae 0x18000d36c
+   18000d2f8:	fs rex
+   18000d2fa:	rex push %rbp
+   18000d2fc:	rex.RB
+   18000d2fd:	rex.B
+   18000d2fe:	rex.B
+   18000d2ff:	rex pop %rax
+   18000d301:	pop    %rdx
+   18000d302:	add    %al,(%rax)
+   18000d304:	stos   %eax,%es:(%rdi)
+   18000d305:	add    %edi,(%rdi)
+   18000d307:	pop    %rdi
+   18000d308:	rex.RX imul $0x73406e65,0x70(%rdi),%r13d
+   18000d310:	je     0x18000d376
+   18000d312:	rex
+   18000d313:	rex pop %rcx
+   18000d315:	push   %r8
+   18000d317:	rex.RB
+   18000d318:	push   %r13
+   18000d31a:	pop    %rdi
+   18000d31b:	imul   $0x40406675,0x62(%rdi),%ebp
+   18000d322:	push   %rax
+   18000d323:	rex.RB
+   18000d324:	rex.X
+   18000d325:	rex.R
+   18000d326:	rex.W
+   18000d327:	rex.W
+   18000d328:	rex pop %rdx
+   18000d32a:	add    %al,(%rax)
+   18000d32c:	(bad)
+   18000d32d:	add    $0x3f,%al
+   18000d32f:	jae    0x18000d399
+   18000d331:	outsl  %ds:(%rsi),(%dx)
+   18000d332:	ja     0x18000d3a1
+   18000d334:	(bad)
+   18000d335:	outsb  %ds:(%rsi),(%dx)
+   18000d336:	jns    0x18000d39b
+   18000d338:	rex (bad)
+   18000d33a:	and    $0x62,%al
+   18000d33c:	(bad)
+   18000d33d:	jae    0x18000d3a8
+   18000d33f:	movsxd 0x73(%rdi),%ebx
+   18000d342:	je     0x18000d3b6
+   18000d344:	gs (bad)
+   18000d346:	insl   (%dx),%es:(%rdi)
+   18000d347:	(bad)
+   18000d34c:	push   %rbp
+   18000d34d:	(bad)
+   18000d34e:	and    $0x63,%al
+   18000d350:	push   $0x745f7261
+   18000d355:	jb     0x18000d3b8
+   18000d357:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
+   18000d35f:	fs rex
+   18000d361:	rex
+   18000d362:	rex jae 0x18000d3d9
+   18000d365:	fs rex
+   18000d367:	rex
+   18000d368:	rex.WRB
+   18000d369:	rex.RB
+   18000d36a:	rex.B
+   18000d36b:	pop    %r15
+   18000d36d:	rex.WX pop %rax
+   18000d36f:	pop    %rdx
+   18000d370:	add    %al,(%rax)
+   18000d372:	leave
+   18000d373:	add    (%rdi),%edi
+   18000d375:	imul   $0x646f6324,0x3f(%rax,%rax,2),%esp
+   18000d37d:	movsxd %gs:0x74(%rsi),%esi
+   18000d381:	rex
+   18000d382:	rex.R
+   18000d383:	rex.R push %rbp
+   18000d385:	pop    %rdi
+   18000d386:	(bad)
+   18000d38c:	gs je  0x18000d3cf
+   18000d38f:	rex
+   18000d390:	rex jae 0x18000d407
+   18000d393:	fs rex
+   18000d395:	rex xor 0x30(%rsi),%dl
+   18000d399:	insb   (%dx),%es:(%rdi)
+   18000d39a:	outsl  %ds:(%rsi),(%dx)
+   18000d39b:	movsxd 0x6c(%rcx),%esp
+   18000d39e:	rex xor %gs:0x41(%rax),%al
+   18000d3a3:	add    %cl,0x53(%rbp)
+   18000d3a6:	push   %rsi
+   18000d3a7:	rex.XB push %r8
+   18000d3a9:	xor    %esi,(%rax,%rsi,1)
+   18000d3ac:	cs fs insb (%dx),%es:(%rdi)
+   18000d3af:	insb   (%dx),%es:(%rdi)
+   18000d3b0:	add    %al,(%rax)
+   18000d3b2:	add    %al,(%rax)
+   18000d3b4:	pop    %rdi
+   18000d3b5:	pop    %rdi
+   18000d3b6:	rex.XB js 0x18000d431
+   18000d3b9:	rex.RX jb 0x18000d41d
+   18000d3bc:	insl   (%dx),%es:(%rdi)
+   18000d3bd:	gs rex.W (bad)
+   18000d3c0:	outsb  %ds:(%rsi),(%dx)
+   18000d3c1:	fs insb (%dx),%es:(%rdi)
+   18000d3c3:	gs jb  0x18000d3fa
+   18000d3c6:	add    %al,(%rax)
+   18000d3c8:	sbb    %al,(%rax)
+   18000d3ca:	pop    %rdi
+   18000d3cb:	pop    %rdi
+   18000d3cc:	push   %rdx
+   18000d3cd:	push   %rsp
+   18000d3ce:	rex.R jns 0x18000d43f
+   18000d3d1:	(bad)
+   18000d3d2:	insl   (%dx),%es:(%rdi)
+   18000d3d3:	imul   $0x747361,0x43(%rbx),%esp
+   18000d3da:	and    (%rax),%eax
+   18000d3dc:	pop    %rdi
+   18000d3dd:	pop    %rdi
+   18000d3de:	jae    0x18000d454
+   18000d3e0:	fs pop %rdi
+   18000d3e2:	je     0x18000d449
+   18000d3e4:	jb     0x18000d453
+   18000d3e6:	imul   $0x21006574,0x61(%rsi),%ebp
+   18000d3ed:	add    %bl,0x5f(%rdi)
+   18000d3f0:	jae    0x18000d466
+   18000d3f2:	fs pop %rdi
+   18000d3f4:	gs js  0x18000d45a
+   18000d3f7:	gs jo  0x18000d46e
+   18000d3fa:	imul   $0x706f635f,0x6e(%rdi),%ebp
+   18000d401:	jns    0x18000d403
+   18000d403:	add    %ah,(%rdx)
+   18000d405:	add    %bl,0x5f(%rdi)
+   18000d408:	jae    0x18000d47e
+   18000d40a:	fs pop %rdi
+   18000d40c:	gs js  0x18000d472
+   18000d40f:	gs jo  0x18000d486
+   18000d412:	imul   $0x7365645f,0x6e(%rdi),%ebp
+   18000d419:	je     0x18000d48d
+   18000d41b:	outsl  %ds:(%rsi),(%dx)
+   18000d41c:	jns    0x18000d41e
+   18000d41e:	(bad)
+   18000d41f:	add    %bl,0x5f(%rdi)
+   18000d422:	jae    0x18000d498
+   18000d424:	fs pop %rdi
+   18000d426:	je     0x18000d4a1
+   18000d428:	jo     0x18000d48f
+   18000d42a:	pop    %rdi
+   18000d42b:	imul   $0x616e5f6f,0x66(%rsi),%ebp
+   18000d432:	insl   (%dx),%es:(%rdi)
+   18000d433:	add    %al,%gs:(%rax)
+   18000d436:	add    %eax,(%rax)
+   18000d438:	pop    %rdi
+   18000d439:	rex.XB js 0x18000d4b4
+   18000d43c:	push   %rsp
+   18000d43d:	push   $0x45776f72
+   18000d442:	js     0x18000d4a7
+   18000d444:	gs jo  0x18000d4bb
+   18000d447:	imul   $0x3c0000,0x6e(%rdi),%ebp
+   18000d44e:	insl   (%dx),%es:(%rdi)
+   18000d44f:	gs insl (%dx),%es:(%rdi)
+   18000d451:	movsxd 0x79(%rax),%esi
+   18000d454:	add    %al,(%rax)
+   18000d456:	cmp    $0x6d656d00,%eax
+   18000d45b:	insl   (%dx),%es:(%rdi)
+   18000d45c:	outsl  %ds:(%rsi),(%dx)
+   18000d45d:	jbe    0x18000d4c4
+   18000d45f:	add    %bh,(%rsi)
+   18000d461:	add    %ch,0x65(%rbp)
+   18000d464:	insl   (%dx),%es:(%rdi)
+   18000d465:	jae    0x18000d4cc
+   18000d467:	je     0x18000d469
+   18000d469:	add    %bl,(%rbx)
+   18000d46b:	add    %bl,0x5f(%rdi)
+   18000d46e:	movsxd 0x72(%rbp),%esi
+   18000d471:	jb     0x18000d4d8
+   18000d473:	outsb  %ds:(%rsi),(%dx)
+   18000d474:	je     0x18000d4d5
+   18000d476:	gs js  0x18000d4dc
+   18000d479:	gs jo  0x18000d4f0
+   18000d47c:	imul   $0x5f001c00,0x6e(%rdi),%ebp
+   18000d483:	pop    %rdi
+   18000d484:	movsxd 0x72(%rbp),%esi
+   18000d487:	jb     0x18000d4ee
+   18000d489:	outsb  %ds:(%rsi),(%dx)
+   18000d48a:	je     0x18000d4eb
+   18000d48c:	gs js  0x18000d4f2
+   18000d48f:	gs jo  0x18000d506
+   18000d492:	imul   $0x6e6f635f,0x6e(%rdi),%ebp
+   18000d499:	je     0x18000d500
+   18000d49b:	js     0x18000d511
+   18000d49d:	add    %cl,(%rax)
+   18000d49f:	add    %bl,0x5f(%rdi)
+   18000d4a2:	rex.XB pop %r15
+   18000d4a4:	jae    0x18000d516
+   18000d4a6:	movsxd %gs:0x66(%rcx),%ebp
+   18000d4aa:	imul   $0x646e6168,0x5f(%rbx),%esp
+   18000d4b1:	insb   (%dx),%es:(%rdi)
+   18000d4b2:	gs jb  0x18000d4b5
+   18000d4b5:	add    %ah,0x735f5f00(%rip)        # 0x1f36033bb
+   18000d4bb:	je     0x18000d521
+   18000d4bd:	pop    %rdi
+   18000d4be:	je     0x18000d539
+   18000d4c0:	jo     0x18000d527
+   18000d4c2:	pop    %rdi
+   18000d4c3:	imul   $0x65645f6f,0x66(%rsi),%ebp
+   18000d4ca:	jae    0x18000d540
+   18000d4cc:	jb     0x18000d53d
+   18000d4ce:	jns    0x18000d52f
+   18000d4d0:	insb   (%dx),%es:(%rdi)
+   18000d4d1:	imul   $0x43560000,0x74(%rbx),%esi
+   18000d4d8:	push   %rdx
+   18000d4d9:	push   %rbp
+   18000d4da:	rex.WRX push %rsp
+   18000d4dc:	rex.WB
+   18000d4dd:	rex.WRB
+   18000d4de:	xor    %r14d,(%r8,%rsi,1)
+   18000d4e2:	pop    %rdi
+   18000d4e3:	xor    %ebp,(%rsi)
+   18000d4e5:	fs insb (%dx),%es:(%rdi)
+   18000d4e7:	insb   (%dx),%es:(%rdi)
+   18000d4e8:	add    %al,(%rax)
+   18000d4ea:	push   %rsi
+   18000d4eb:	rex.XB push %r10
+   18000d4ed:	push   %rbp
+   18000d4ee:	rex.WRX push %rsp
+   18000d4f0:	rex.WB
+   18000d4f1:	rex.WRB
+   18000d4f2:	xor    %r14d,(%r8,%rsi,1)
+   18000d4f6:	cs fs insb (%dx),%es:(%rdi)
+   18000d4f9:	insb   (%dx),%es:(%rdi)
+   18000d4fa:	add    %al,(%rax)
+   18000d4fc:	cmp    %eax,(%rax)
+   18000d4fe:	pop    %rdi
+   18000d4ff:	imul   $0x64696c61,0x76(%rsi),%ebp
+   18000d506:	pop    %rdi
+   18000d507:	jo     0x18000d56a
+   18000d509:	jb     0x18000d56c
+   18000d50b:	insl   (%dx),%es:(%rdi)
+   18000d50c:	gs je  0x18000d574
+   18000d50f:	jb     0x18000d570
+   18000d511:	outsb  %ds:(%rsi),(%dx)
+   18000d512:	outsl  %ds:(%rsi),(%dx)
+   18000d513:	imul   $0x6f6e5f6f,0x66(%rsi),%ebp
+   18000d51a:	jb     0x18000d581
+   18000d51c:	je     0x18000d593
+   18000d51e:	jb     0x18000d58e
+   18000d520:	add    %al,(%rax)
+   18000d522:	cmp    %eax,(%rax)
+   18000d524:	pop    %rdi
+   18000d525:	addr32 gs je 0x18000d588
+   18000d529:	jae    0x18000d59f
+   18000d52b:	jb     0x18000d592
+   18000d52d:	(bad)
+   18000d52e:	insl   (%dx),%es:(%rdi)
+   18000d52f:	pop    %rdi
+   18000d530:	(bad)
+   18000d535:	jb     0x18000d596
+   18000d537:	jo     0x18000d5a8
+   18000d539:	imul   $0x737265,0x74(%rsi),%ebp
+   18000d540:	je     0x18000d542
+   18000d542:	movsxd 0x73(%rdi,%rbp,2),%bp
+   18000d547:	add    %al,%gs:(%rax)
+   18000d54a:	ja     0x18000d54c
+   18000d54c:	data16 data16 insb (%dx),%es:(%rdi)
+   18000d54f:	jne    0x18000d5c4
+   18000d551:	push   $0x780000
+   18000d556:	data16 addr32 gs je 0x18000d5be
+   18000d55b:	add    %bh,0x0(%rcx)
+   18000d55e:	data16 addr32 gs je 0x18000d5d3
+   18000d563:	outsl  %ds:(%rsi),(%dx)
+   18000d564:	jae    0x18000d566
+   18000d566:	jg     0x18000d568
+   18000d568:	data16 jo 0x18000d5e0
+   18000d56b:	je     0x18000d5d0
+   18000d56d:	add    %al,0x65726600(%rbx)
+   18000d573:	(bad)
+   18000d574:	add    %cl,%fs:0x65736600(%rax)
+   18000d57b:	je     0x18000d5ed
+   18000d57d:	outsl  %ds:(%rsi),(%dx)
+   18000d57e:	jae    0x18000d580
+   18000d580:	(bad)
+   18000d581:	add    %bl,0x66(%rdi)
+   18000d584:	jae    0x18000d5eb
+   18000d586:	imul   $0x34,%gs:0x36(%rcx),%ebp
+   18000d58b:	add    %cl,0x72776600(%rdx)
+   18000d591:	imul   $0x73009800,0x0(%rbp,%riz,2),%esi
+   18000d599:	gs je  0x18000d612
+   18000d59c:	(bad)
+   18000d5a1:	add    %dh,0x6e(%rbp)
+   18000d5a4:	addr32 gs je 0x18000d60b
+   18000d5a8:	add    %al,(%rax)
+   18000d5aa:	(bad)
+   18000d5ab:	add    %bl,0x6c(%rdi)
+   18000d5ae:	outsl  %ds:(%rsi),(%dx)
+   18000d5af:	movsxd 0x5f(%rbx),%ebp
+   18000d5b2:	imul   $0x2400,0x0(%rbp,%riz,2),%bp
+   18000d5b9:	add    %bl,0x75(%rdi)
+   18000d5bc:	outsb  %ds:(%rsi),(%dx)
+   18000d5bd:	insb   (%dx),%es:(%rdi)
+   18000d5be:	outsl  %ds:(%rsi),(%dx)
+   18000d5bf:	movsxd 0x5f(%rbx),%ebp
+   18000d5c2:	imul   $0x1600,0x0(%rbp,%riz,2),%bp
+   18000d5c9:	add    %esi,0x71(%rbx)
+   18000d5cc:	jb     0x18000d642
+   18000d5ce:	add    %al,(%rax)
+   18000d5d0:	add    %dh,0x72(%ebp,%eiz,2)
+   18000d5d5:	insl   (%dx),%es:(%rdi)
+   18000d5d6:	imul   $0x8006574,0x61(%rsi),%ebp
+   18000d5dd:	add    %bl,0x63(%rdi)
+   18000d5e0:	(bad)
+   18000d5e1:	insb   (%dx),%es:(%rdi)
+   18000d5e2:	insb   (%dx),%es:(%rdi)
    18000d5e3:	outsb  %ds:(%rsi),(%dx)
-   18000d5e4:	insl   (%dx),%es:(%rdi)
-   18000d5e5:	outsb  %gs:(%rsi),(%dx)
-   18000d5e7:	je     0x18000d5e9
-   18000d5e9:	add    %dh,(%rax,%rax,1)
-   18000d5ec:	pop    %rdi
-   18000d5ed:	imul   $0x6c616974,0x69(%rsi),%ebp
-   18000d5f4:	imul   $0x656e6f5f,0x65(%rdx),%edi
-   18000d5fb:	js     0x18000d666
-   18000d5fd:	je     0x18000d65e
-   18000d5ff:	je     0x18000d662
-   18000d601:	(bad)
-   18000d602:	insb   (%dx),%es:(%rdi)
-   18000d603:	add    %al,%gs:(%rax)
-   18000d606:	cmp    $0x0,%al
-   18000d608:	pop    %rdi
-   18000d609:	jb     0x18000d670
-   18000d60b:	imul   $0x6f5f7265,0x74(%ebx),%esi
-   18000d613:	outsb  %ds:(%rsi),(%dx)
-   18000d614:	gs js  0x18000d680
-   18000d617:	je     0x18000d678
-   18000d619:	data16 jne 0x18000d68a
-   18000d61c:	movsxd 0x6f(%rcx,%rbp,2),%esi
-   18000d620:	outsb  %ds:(%rsi),(%dx)
-   18000d621:	add    %ah,(%rdx)
-   18000d623:	add    %bl,0x65(%rdi)
-   18000d626:	js     0x18000d68d
-   18000d628:	movsxd 0x74(%rbp),%esi
-   18000d62b:	gs pop %rdi
-   18000d62d:	outsl  %ds:(%rsi),(%dx)
-   18000d62e:	outsb  %ds:(%rsi),(%dx)
-   18000d62f:	gs js  0x18000d69b
-   18000d632:	je     0x18000d693
-   18000d634:	je     0x18000d697
-   18000d636:	(bad)
-   18000d637:	insb   (%dx),%es:(%rdi)
-   18000d638:	add    %bl,%gs:(%rsi)
-   18000d63b:	add    %bl,0x63(%rdi)
-   18000d63e:	jb     0x18000d6b4
-   18000d640:	pop    %rdi
-   18000d641:	(bad)
-   18000d642:	je     0x18000d6a9
-   18000d644:	js     0x18000d6af
-   18000d646:	je     0x18000d648
-   18000d648:	(bad)
-   18000d649:	add    %bl,0x63(%rdi)
-   18000d64c:	gs js  0x18000d6b8
-   18000d64f:	je     0x18000d651
-   18000d651:	add    %bl,(%rax)
-   18000d653:	add    %ah,0x72(%rsi)
-   18000d656:	gs add %al,%gs:(%rax)
-   18000d65a:	(bad)
-   18000d65b:	jo     0x18000d6c6
-   18000d65d:	sub    $0x772d736d,%eax
-   18000d662:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   18000d669:	jb     0x18000d6e0
-   18000d66b:	outsb  %ds:(%rsi),(%dx)
-   18000d66c:	je     0x18000d6d7
-   18000d66e:	insl   (%dx),%es:(%rdi)
-   18000d66f:	gs sub $0x312d316c,%eax
-   18000d675:	sub    $0x6c642e30,%eax
-   18000d67a:	insb   (%dx),%es:(%rdi)
-   18000d67b:	add    %ah,0x70(%rcx)
-   18000d67e:	imul   $0x632d6e69,0x772d736d(%rip),%ebp        # 0x1f72e49f5
-   18000d688:	jb     0x18000d6fe
-   18000d68a:	sub    $0x69647473,%eax
-   18000d68f:	outsl  %ds:(%rsi),(%dx)
-   18000d690:	sub    $0x312d316c,%eax
-   18000d695:	sub    $0x6c642e30,%eax
-   18000d69a:	insb   (%dx),%es:(%rdi)
-   18000d69b:	add    %ah,0x70(%rcx)
-   18000d69e:	imul   $0x632d6e69,0x772d736d(%rip),%ebp        # 0x1f72e4a15
-   18000d6a8:	jb     0x18000d71e
-   18000d6aa:	sub    $0x656c6966,%eax
-   18000d6af:	jae    0x18000d72a
-   18000d6b1:	jae    0x18000d727
-   18000d6b3:	gs insl (%dx),%es:(%rdi)
-   18000d6b5:	sub    $0x312d316c,%eax
-   18000d6ba:	sub    $0x6c642e30,%eax
-   18000d6bf:	insb   (%dx),%es:(%rdi)
-   18000d6c0:	add    %al,(%rax)
-   18000d6c2:	(bad)
-   18000d6c3:	jo     0x18000d72e
-   18000d6c5:	sub    $0x772d736d,%eax
-   18000d6ca:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   18000d6d1:	insl   (%dx),%es:(%rdi)
-   18000d6d2:	(bad)
-   18000d6d3:	je     0x18000d73d
-   18000d6d5:	sub    $0x312d316c,%eax
-   18000d6da:	sub    $0x6c642e30,%eax
-   18000d6df:	insb   (%dx),%es:(%rdi)
-   18000d6e0:	add    %al,(%rax)
-   18000d6e2:	(bad)
-   18000d6e3:	jo     0x18000d74e
-   18000d6e5:	sub    $0x772d736d,%eax
-   18000d6ea:	imul   $0x2d747263,0x2d(%rsi),%ebp
-   18000d6f1:	push   $0x2d706165
-   18000d6f6:	insb   (%dx),%es:(%rdi)
-   18000d6f7:	xor    %ebp,0x2e302d31(%rip)        # 0x1ae31042e
-   18000d6fd:	fs insb (%dx),%es:(%rdi)
-   18000d6ff:	insb   (%dx),%es:(%rdi)
-   18000d700:	add    %al,(%rax)
-   18000d702:	mov    (%rbx),%al
-   18000d704:	rex.WB outsb %ds:(%rsi),(%dx)
-   18000d706:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
-   18000d70e:	push   %rbx
-   18000d70f:	imul   $0x64616548,0x74(%rbx),%r14
-   18000d717:	add    %dh,%ch
-   18000d719:	add    $0x52,%al
-   18000d71b:	je     0x18000d789
-   18000d71d:	rex.XB (bad)
-   18000d71f:	jo     0x18000d795
-   18000d721:	jne    0x18000d795
-   18000d723:	rex.XB outsl %gs:(%rsi),(%dx)
-   18000d726:	outsb  %ds:(%rsi),(%dx)
-   18000d727:	je     0x18000d78e
-   18000d729:	js     0x18000d79f
-   18000d72b:	add    %bh,%ch
-   18000d72d:	add    $0x52,%al
-   18000d72f:	je     0x18000d79d
-   18000d731:	rex.WR outsl %ds:(%rsi),(%dx)
-   18000d733:	outsl  %ds:(%rsi),(%dx)
-   18000d734:	imul   $0x46,0x70(%rbp),%esi
-   18000d738:	jne    0x18000d7a8
-   18000d73a:	movsxd 0x6f(%rcx,%rbp,2),%esi
-   18000d73e:	outsb  %ds:(%rsi),(%dx)
-   18000d73f:	rex.RB outsb %ds:(%rsi),(%dx)
-   18000d741:	je     0x18000d7b5
-   18000d743:	jns    0x18000d745
-   18000d745:	add    %al,0x566c7452(,%rax,1)
-   18000d74c:	imul   $0x556c6175,0x74(%rdx),%esi
-   18000d753:	outsb  %ds:(%rsi),(%dx)
-   18000d754:	ja     0x18000d7bf
-   18000d756:	outsb  %ds:(%rsi),(%dx)
-   18000d757:	add    %al,%fs:(%rax)
-   18000d75a:	out    %al,$0x5
-   18000d75c:	push   %rbp
-   18000d75d:	outsb  %ds:(%rsi),(%dx)
-   18000d75e:	push   $0x6c646e61
-   18000d763:	gs fs rex.RB js 0x18000d7cb
-   18000d768:	gs jo  0x18000d7df
-   18000d76b:	imul   $0x746c6946,0x6e(%rdi),%ebp
-   18000d772:	gs jb  0x18000d775
-   18000d775:	add    %ah,0x55746553(%rbp,%rax,1)
-   18000d77c:	outsb  %ds:(%rsi),(%dx)
-   18000d77d:	push   $0x6c646e61
-   18000d782:	gs fs rex.RB js 0x18000d7ea
-   18000d787:	gs jo  0x18000d7fe
-   18000d78a:	imul   $0x746c6946,0x6e(%rdi),%ebp
-   18000d791:	gs jb  0x18000d794
-   18000d794:	xor    (%rdx),%al
-   18000d796:	rex.RXB
-   18000d797:	gs je  0x18000d7dd
-   18000d79a:	jne    0x18000d80e
-   18000d79c:	jb     0x18000d803
-   18000d79e:	outsb  %ds:(%rsi),(%dx)
-   18000d79f:	je     0x18000d7f1
-   18000d7a1:	jb     0x18000d812
-   18000d7a3:	movsxd 0x73(%rbp),%esp
-   18000d7a6:	jae    0x18000d7a8
-   18000d7a8:	(bad)
-   18000d7a9:	add    $0x6d726554,%eax
-   18000d7ae:	imul   $0x72506574,0x61(%rsi),%ebp
-   18000d7b5:	outsl  %ds:(%rsi),(%dx)
-   18000d7b6:	movsxd 0x73(%rbp),%esp
-   18000d7b9:	jae    0x18000d7bb
-   18000d7bb:	add    %ch,0x50734903(%rax)
-   18000d7c1:	jb     0x18000d832
-   18000d7c3:	movsxd 0x73(%rbp),%esp
-   18000d7c6:	jae    0x18000d837
-   18000d7c8:	jb     0x18000d810
-   18000d7ca:	gs (bad)
-   18000d7cc:	je     0x18000d843
-   18000d7ce:	jb     0x18000d835
-   18000d7d0:	push   %rax
-   18000d7d1:	jb     0x18000d838
-   18000d7d3:	jae    0x18000d83a
-   18000d7d5:	outsb  %ds:(%rsi),(%dx)
-   18000d7d6:	je     0x18000d7d8
-   18000d7d8:	jo     0x18000d7de
-   18000d7da:	push   %rcx
-   18000d7db:	jne    0x18000d842
-   18000d7dd:	jb     0x18000d858
-   18000d7df:	push   %rax
-   18000d7e0:	gs jb  0x18000d849
-   18000d7e3:	outsl  %ds:(%rsi),(%dx)
-   18000d7e4:	jb     0x18000d853
-   18000d7e6:	(bad)
-   18000d7e7:	outsb  %ds:(%rsi),(%dx)
-   18000d7e8:	movsxd 0x43(%rbp),%esp
-   18000d7eb:	outsl  %ds:(%rsi),(%dx)
-   18000d7ec:	jne    0x18000d85c
-   18000d7ee:	je     0x18000d855
-   18000d7f0:	jb     0x18000d7f2
-   18000d7f2:	xor    (%rdx),%eax
-   18000d7f4:	rex.RXB
-   18000d7f5:	gs je  0x18000d83b
-   18000d7f8:	jne    0x18000d86c
-   18000d7fa:	jb     0x18000d861
-   18000d7fc:	outsb  %ds:(%rsi),(%dx)
-   18000d7fd:	je     0x18000d84f
-   18000d7ff:	jb     0x18000d870
-   18000d801:	movsxd 0x73(%rbp),%esp
-   18000d804:	jae    0x18000d84f
-   18000d806:	add    %dh,%fs:(%rdi)
-   18000d809:	add    0x65(%rdi),%al
-   18000d80c:	je     0x18000d851
-   18000d80e:	jne    0x18000d882
-   18000d810:	jb     0x18000d877
-   18000d812:	outsb  %ds:(%rsi),(%dx)
-   18000d813:	je     0x18000d869
-   18000d815:	push   $0x64616572
-   18000d81a:	rex.WB
-   18000d81b:	add    %al,%fs:(%rax)
-   18000d81e:	or     (%rbx),%al
-   18000d820:	rex.RXB
-   18000d821:	gs je  0x18000d877
-   18000d824:	jns    0x18000d899
-   18000d826:	je     0x18000d88d
-   18000d828:	insl   (%dx),%es:(%rdi)
-   18000d829:	push   %rsp
-   18000d82a:	imul   $0x69467341,0x65(%rbp),%ebp
-   18000d831:	insb   (%dx),%es:(%rdi)
-   18000d832:	gs push %rsp
-   18000d834:	imul   $0x44013400,0x65(%rbp),%ebp
-   18000d83b:	imul   $0x54656c62,0x61(%rbx),%esi
-   18000d842:	push   $0x64616572
-   18000d847:	imul   $0x43797261,0x72(%rdx),%r12
-   18000d84f:	(bad)
-   18000d850:	insb   (%dx),%es:(%rdi)
-   18000d851:	insb   (%dx),%es:(%rdi)
-   18000d852:	jae    0x18000d854
-   18000d854:	movabs 0x6775626544734903,%al
-   18000d85d:	addr32 gs jb 0x18000d8b1
-   18000d861:	jb     0x18000d8c8
-   18000d863:	jae    0x18000d8ca
-   18000d865:	outsb  %ds:(%rsi),(%dx)
-   18000d866:	je     0x18000d868
-   18000d868:	rex.WXB
-   18000d869:	rex.RB push %r10
-   18000d86b:	rex.WRX
-   18000d86c:	rex.RB
-   18000d86d:	xor    (%rdx),%r14
-   18000d870:	cs fs insb (%dx),%es:(%rdi)
-   18000d873:	insb   (%dx),%es:(%rdi)
+   18000d5e4:	gs ja  0x18000d64f
+   18000d5e7:	add    %bl,(%rcx)
+   18000d5e9:	add    %ch,0x61(%rbp)
+   18000d5ec:	insb   (%dx),%es:(%rdi)
+   18000d5ed:	insb   (%dx),%es:(%rdi)
+   18000d5ee:	outsl  %ds:(%rsi),(%dx)
+   18000d5ef:	movsxd (%rax),%eax
+   18000d5f1:	add    %dh,(%rsi)
+   18000d5f3:	add    %bl,0x69(%rdi)
+   18000d5f6:	outsb  %ds:(%rsi),(%dx)
+   18000d5f7:	imul   $0x37006d72,0x65(%rsp,%rsi,2),%esi
+   18000d5ff:	add    %bl,0x69(%rdi)
+   18000d602:	outsb  %ds:(%rsi),(%dx)
+   18000d603:	imul   $0x655f6d72,0x65(%rsp,%rsi,2),%esi
+   18000d60b:	add    %bh,(%rdi)
+   18000d60d:	add    %bl,0x73(%rdi)
+   18000d610:	gs push $0x6c69665f
+   18000d616:	je     0x18000d67d
+   18000d618:	jb     0x18000d679
+   18000d61a:	fs insb (%dx),%es:(%rdi)
+   18000d61c:	insb   (%dx),%es:(%rdi)
+   18000d61d:	add    %bl,(%rax)
+   18000d61f:	add    %bl,0x63(%rdi)
+   18000d622:	outsl  %ds:(%rsi),(%dx)
+   18000d623:	outsb  %ds:(%rsi),(%dx)
+   18000d624:	imul   $0x6572,0x75(%rdi),%sp
+   18000d62a:	pop    %rdi
+   18000d62b:	outsb  %ds:(%rsi),(%dx)
+   18000d62c:	(bad)
+   18000d62d:	jb     0x18000d6a1
+   18000d62f:	outsl  %ds:(%rsi),(%dx)
+   18000d630:	ja     0x18000d691
+   18000d632:	(bad)
+   18000d633:	jb     0x18000d69c
+   18000d635:	jbe    0x18000d637
+   18000d637:	add    %dh,(%rbx)
+   18000d639:	add    %bl,0x69(%rdi)
+   18000d63c:	outsb  %ds:(%rsi),(%dx)
+   18000d63d:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
+   18000d645:	pop    %rdi
+   18000d646:	outsb  %ds:(%rsi),(%dx)
+   18000d647:	(bad)
+   18000d648:	jb     0x18000d6bc
+   18000d64a:	outsl  %ds:(%rsi),(%dx)
+   18000d64b:	ja     0x18000d6ac
+   18000d64d:	outsb  %gs:(%rsi),(%dx)
+   18000d64f:	jbe    0x18000d6ba
+   18000d651:	jb     0x18000d6c2
+   18000d653:	outsb  %ds:(%rsi),(%dx)
+   18000d654:	insl   (%dx),%es:(%rdi)
+   18000d655:	outsb  %gs:(%rsi),(%dx)
+   18000d657:	je     0x18000d659
+   18000d659:	add    %dh,(%rax,%rax,1)
+   18000d65c:	pop    %rdi
+   18000d65d:	imul   $0x6c616974,0x69(%rsi),%ebp
+   18000d664:	imul   $0x656e6f5f,0x65(%rdx),%edi
+   18000d66b:	js     0x18000d6d6
+   18000d66d:	je     0x18000d6ce
+   18000d66f:	je     0x18000d6d2
+   18000d671:	(bad)
+   18000d672:	insb   (%dx),%es:(%rdi)
+   18000d673:	add    %al,%gs:(%rax)
+   18000d676:	cmp    $0x0,%al
+   18000d678:	pop    %rdi
+   18000d679:	jb     0x18000d6e0
+   18000d67b:	imul   $0x6f5f7265,0x74(%ebx),%esi
+   18000d683:	outsb  %ds:(%rsi),(%dx)
+   18000d684:	gs js  0x18000d6f0
+   18000d687:	je     0x18000d6e8
+   18000d689:	data16 jne 0x18000d6fa
+   18000d68c:	movsxd 0x6f(%rcx,%rbp,2),%esi
+   18000d690:	outsb  %ds:(%rsi),(%dx)
+   18000d691:	add    %ah,(%rdx)
+   18000d693:	add    %bl,0x65(%rdi)
+   18000d696:	js     0x18000d6fd
+   18000d698:	movsxd 0x74(%rbp),%esi
+   18000d69b:	gs pop %rdi
+   18000d69d:	outsl  %ds:(%rsi),(%dx)
+   18000d69e:	outsb  %ds:(%rsi),(%dx)
+   18000d69f:	gs js  0x18000d70b
+   18000d6a2:	je     0x18000d703
+   18000d6a4:	je     0x18000d707
+   18000d6a6:	(bad)
+   18000d6a7:	insb   (%dx),%es:(%rdi)
+   18000d6a8:	add    %bl,%gs:(%rsi)
+   18000d6ab:	add    %bl,0x63(%rdi)
+   18000d6ae:	jb     0x18000d724
+   18000d6b0:	pop    %rdi
+   18000d6b1:	(bad)
+   18000d6b2:	je     0x18000d719
+   18000d6b4:	js     0x18000d71f
+   18000d6b6:	je     0x18000d6b8
+   18000d6b8:	(bad)
+   18000d6b9:	add    %bl,0x63(%rdi)
+   18000d6bc:	gs js  0x18000d728
+   18000d6bf:	je     0x18000d6c1
+   18000d6c1:	add    %bl,(%rax)
+   18000d6c3:	add    %ah,0x72(%rsi)
+   18000d6c6:	gs add %al,%gs:(%rax)
+   18000d6ca:	(bad)
+   18000d6cb:	jo     0x18000d736
+   18000d6cd:	sub    $0x772d736d,%eax
+   18000d6d2:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   18000d6d9:	jb     0x18000d750
+   18000d6db:	outsb  %ds:(%rsi),(%dx)
+   18000d6dc:	je     0x18000d747
+   18000d6de:	insl   (%dx),%es:(%rdi)
+   18000d6df:	gs sub $0x312d316c,%eax
+   18000d6e5:	sub    $0x6c642e30,%eax
+   18000d6ea:	insb   (%dx),%es:(%rdi)
+   18000d6eb:	add    %ah,0x70(%rcx)
+   18000d6ee:	imul   $0x632d6e69,0x772d736d(%rip),%ebp        # 0x1f72e4a65
+   18000d6f8:	jb     0x18000d76e
+   18000d6fa:	sub    $0x69647473,%eax
+   18000d6ff:	outsl  %ds:(%rsi),(%dx)
+   18000d700:	sub    $0x312d316c,%eax
+   18000d705:	sub    $0x6c642e30,%eax
+   18000d70a:	insb   (%dx),%es:(%rdi)
+   18000d70b:	add    %ah,0x70(%rcx)
+   18000d70e:	imul   $0x632d6e69,0x772d736d(%rip),%ebp        # 0x1f72e4a85
+   18000d718:	jb     0x18000d78e
+   18000d71a:	sub    $0x656c6966,%eax
+   18000d71f:	jae    0x18000d79a
+   18000d721:	jae    0x18000d797
+   18000d723:	gs insl (%dx),%es:(%rdi)
+   18000d725:	sub    $0x312d316c,%eax
+   18000d72a:	sub    $0x6c642e30,%eax
+   18000d72f:	insb   (%dx),%es:(%rdi)
+   18000d730:	add    %al,(%rax)
+   18000d732:	(bad)
+   18000d733:	jo     0x18000d79e
+   18000d735:	sub    $0x772d736d,%eax
+   18000d73a:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   18000d741:	insl   (%dx),%es:(%rdi)
+   18000d742:	(bad)
+   18000d743:	je     0x18000d7ad
+   18000d745:	sub    $0x312d316c,%eax
+   18000d74a:	sub    $0x6c642e30,%eax
+   18000d74f:	insb   (%dx),%es:(%rdi)
+   18000d750:	add    %al,(%rax)
+   18000d752:	(bad)
+   18000d753:	jo     0x18000d7be
+   18000d755:	sub    $0x772d736d,%eax
+   18000d75a:	imul   $0x2d747263,0x2d(%rsi),%ebp
+   18000d761:	push   $0x2d706165
+   18000d766:	insb   (%dx),%es:(%rdi)
+   18000d767:	xor    %ebp,0x2e302d31(%rip)        # 0x1ae31049e
+   18000d76d:	fs insb (%dx),%es:(%rdi)
+   18000d76f:	insb   (%dx),%es:(%rdi)
+   18000d770:	add    %al,(%rax)
+   18000d772:	mov    (%rbx),%al
+   18000d774:	rex.WB outsb %ds:(%rsi),(%dx)
+   18000d776:	imul   $0x657a696c,0x61(%rcx,%rbp,2),%esi
+   18000d77e:	push   %rbx
+   18000d77f:	imul   $0x64616548,0x74(%rbx),%r14
+   18000d787:	add    %dh,%ch
+   18000d789:	add    $0x52,%al
+   18000d78b:	je     0x18000d7f9
+   18000d78d:	rex.XB (bad)
+   18000d78f:	jo     0x18000d805
+   18000d791:	jne    0x18000d805
+   18000d793:	rex.XB outsl %gs:(%rsi),(%dx)
+   18000d796:	outsb  %ds:(%rsi),(%dx)
+   18000d797:	je     0x18000d7fe
+   18000d799:	js     0x18000d80f
+   18000d79b:	add    %bh,%ch
+   18000d79d:	add    $0x52,%al
+   18000d79f:	je     0x18000d80d
+   18000d7a1:	rex.WR outsl %ds:(%rsi),(%dx)
+   18000d7a3:	outsl  %ds:(%rsi),(%dx)
+   18000d7a4:	imul   $0x46,0x70(%rbp),%esi
+   18000d7a8:	jne    0x18000d818
+   18000d7aa:	movsxd 0x6f(%rcx,%rbp,2),%esi
+   18000d7ae:	outsb  %ds:(%rsi),(%dx)
+   18000d7af:	rex.RB outsb %ds:(%rsi),(%dx)
+   18000d7b1:	je     0x18000d825
+   18000d7b3:	jns    0x18000d7b5
+   18000d7b5:	add    %al,0x566c7452(,%rax,1)
+   18000d7bc:	imul   $0x556c6175,0x74(%rdx),%esi
+   18000d7c3:	outsb  %ds:(%rsi),(%dx)
+   18000d7c4:	ja     0x18000d82f
+   18000d7c6:	outsb  %ds:(%rsi),(%dx)
+   18000d7c7:	add    %al,%fs:(%rax)
+   18000d7ca:	out    %al,$0x5
+   18000d7cc:	push   %rbp
+   18000d7cd:	outsb  %ds:(%rsi),(%dx)
+   18000d7ce:	push   $0x6c646e61
+   18000d7d3:	gs fs rex.RB js 0x18000d83b
+   18000d7d8:	gs jo  0x18000d84f
+   18000d7db:	imul   $0x746c6946,0x6e(%rdi),%ebp
+   18000d7e2:	gs jb  0x18000d7e5
+   18000d7e5:	add    %ah,0x55746553(%rbp,%rax,1)
+   18000d7ec:	outsb  %ds:(%rsi),(%dx)
+   18000d7ed:	push   $0x6c646e61
+   18000d7f2:	gs fs rex.RB js 0x18000d85a
+   18000d7f7:	gs jo  0x18000d86e
+   18000d7fa:	imul   $0x746c6946,0x6e(%rdi),%ebp
+   18000d801:	gs jb  0x18000d804
+   18000d804:	xor    (%rdx),%al
+   18000d806:	rex.RXB
+   18000d807:	gs je  0x18000d84d
+   18000d80a:	jne    0x18000d87e
+   18000d80c:	jb     0x18000d873
+   18000d80e:	outsb  %ds:(%rsi),(%dx)
+   18000d80f:	je     0x18000d861
+   18000d811:	jb     0x18000d882
+   18000d813:	movsxd 0x73(%rbp),%esp
+   18000d816:	jae    0x18000d818
+   18000d818:	(bad)
+   18000d819:	add    $0x6d726554,%eax
+   18000d81e:	imul   $0x72506574,0x61(%rsi),%ebp
+   18000d825:	outsl  %ds:(%rsi),(%dx)
+   18000d826:	movsxd 0x73(%rbp),%esp
+   18000d829:	jae    0x18000d82b
+   18000d82b:	add    %ch,0x50734903(%rax)
+   18000d831:	jb     0x18000d8a2
+   18000d833:	movsxd 0x73(%rbp),%esp
+   18000d836:	jae    0x18000d8a7
+   18000d838:	jb     0x18000d880
+   18000d83a:	gs (bad)
+   18000d83c:	je     0x18000d8b3
+   18000d83e:	jb     0x18000d8a5
+   18000d840:	push   %rax
+   18000d841:	jb     0x18000d8a8
+   18000d843:	jae    0x18000d8aa
+   18000d845:	outsb  %ds:(%rsi),(%dx)
+   18000d846:	je     0x18000d848
+   18000d848:	jo     0x18000d84e
+   18000d84a:	push   %rcx
+   18000d84b:	jne    0x18000d8b2
+   18000d84d:	jb     0x18000d8c8
+   18000d84f:	push   %rax
+   18000d850:	gs jb  0x18000d8b9
+   18000d853:	outsl  %ds:(%rsi),(%dx)
+   18000d854:	jb     0x18000d8c3
+   18000d856:	(bad)
+   18000d857:	outsb  %ds:(%rsi),(%dx)
+   18000d858:	movsxd 0x43(%rbp),%esp
+   18000d85b:	outsl  %ds:(%rsi),(%dx)
+   18000d85c:	jne    0x18000d8cc
+   18000d85e:	je     0x18000d8c5
+   18000d860:	jb     0x18000d862
+   18000d862:	xor    (%rdx),%eax
+   18000d864:	rex.RXB
+   18000d865:	gs je  0x18000d8ab
+   18000d868:	jne    0x18000d8dc
+   18000d86a:	jb     0x18000d8d1
+   18000d86c:	outsb  %ds:(%rsi),(%dx)
+   18000d86d:	je     0x18000d8bf
+   18000d86f:	jb     0x18000d8e0
+   18000d871:	movsxd 0x73(%rbp),%esp
+   18000d874:	jae    0x18000d8bf
+   18000d876:	add    %dh,%fs:(%rdi)
+   18000d879:	add    0x65(%rdi),%al
+   18000d87c:	je     0x18000d8c1
+   18000d87e:	jne    0x18000d8f2
+   18000d880:	jb     0x18000d8e7
+   18000d882:	outsb  %ds:(%rsi),(%dx)
+   18000d883:	je     0x18000d8d9
+   18000d885:	push   $0x64616572
+   18000d88a:	rex.WB
+   18000d88b:	add    %al,%fs:(%rax)
+   18000d88e:	or     (%rbx),%al
+   18000d890:	rex.RXB
+   18000d891:	gs je  0x18000d8e7
+   18000d894:	jns    0x18000d909
+   18000d896:	je     0x18000d8fd
+   18000d898:	insl   (%dx),%es:(%rdi)
+   18000d899:	push   %rsp
+   18000d89a:	imul   $0x69467341,0x65(%rbp),%ebp
+   18000d8a1:	insb   (%dx),%es:(%rdi)
+   18000d8a2:	gs push %rsp
+   18000d8a4:	imul   $0x44013400,0x65(%rbp),%ebp
+   18000d8ab:	imul   $0x54656c62,0x61(%rbx),%esi
+   18000d8b2:	push   $0x64616572
+   18000d8b7:	imul   $0x43797261,0x72(%rdx),%r12
+   18000d8bf:	(bad)
+   18000d8c0:	insb   (%dx),%es:(%rdi)
+   18000d8c1:	insb   (%dx),%es:(%rdi)
+   18000d8c2:	jae    0x18000d8c4
+   18000d8c4:	movabs 0x6775626544734903,%al
+   18000d8cd:	addr32 gs jb 0x18000d921
+   18000d8d1:	jb     0x18000d938
+   18000d8d3:	jae    0x18000d93a
+   18000d8d5:	outsb  %ds:(%rsi),(%dx)
+   18000d8d6:	je     0x18000d8d8
+   18000d8d8:	rex.WXB
+   18000d8d9:	rex.RB push %r10
+   18000d8db:	rex.WRX
+   18000d8dc:	rex.RB
+   18000d8dd:	xor    (%rdx),%r14
+   18000d8e0:	cs fs insb (%dx),%es:(%rdi)
+   18000d8e3:	insb   (%dx),%es:(%rdi)
 	...
 
 Disassembly of section .data:
 
 000000018000e000 <.data>:
    18000e000:	int    $0x5d
    18000e002:	and    %dl,%dl
@@ -18182,152 +18491,157 @@
    18000e029:	clc
    18000e02a:	add    %al,(%rax)
    18000e02c:	add    %al,(%rax)
    18000e02e:	add    %al,(%rax)
    18000e030:	add    %eax,(%rax)
 	...
    18000e03e:	add    %al,(%rax)
-   18000e040:	test   $0x99,%al
-   18000e042:	add    %al,0x1(%rax)
+   18000e040:	enter  $0x99,$0x80
+   18000e044:	add    %eax,(%rax)
 	...
+   18000e04e:	add    %al,(%rax)
    18000e050:	cs (bad)
    18000e052:	push   %r14
    18000e054:	push   %rbx
    18000e055:	imul   $0x6f74656c,0x67(%rsi),%ebp
    18000e05c:	outsb  %ds:(%rsi),(%dx)
    18000e05d:	rex
    18000e05e:	outsl  %gs:(%esi),(%dx)
    18000e061:	fs gs rex
    18000e064:	rex add %al,(%rax)
-   18000e067:	add    %ch,0x1800099(%rax)
+   18000e067:	add    %cl,%al
+   18000e069:	cltd
+   18000e06a:	add    %al,0x1(%rax)
 	...
-   18000e075:	add    %al,(%rax)
-   18000e077:	add    %ch,(%rsi)
-   18000e079:	(bad)
+   18000e078:	cs (bad)
    18000e07a:	push   %r14
    18000e07c:	push   %rsi
    18000e07d:	imul   $0x656c6261,0x77(%rbp),%esp
    18000e084:	jae    0x18000e0d7
    18000e086:	rex.RB
    18000e087:	rex.WRB push %r8
    18000e089:	jb     0x18000e0fa
    18000e08b:	js     0x18000e106
    18000e08d:	imul   $0x40797261,0x72(%rdx),%r12
    18000e095:	outsl  %gs:(%esi),(%dx)
    18000e098:	fs gs rex
    18000e09b:	rex add %al,(%rax)
    18000e09e:	add    %al,(%rax)
-   18000e0a0:	test   $0x99,%al
-   18000e0a2:	add    %al,0x1(%rax)
+   18000e0a0:	enter  $0x99,$0x80
+   18000e0a4:	add    %eax,(%rax)
 	...
+   18000e0ae:	add    %al,(%rax)
    18000e0b0:	cs (bad)
    18000e0b2:	push   %r14
    18000e0b4:	(bad)
    18000e0b9:	jb     0x18000e12d
    18000e0bb:	(bad)
    18000e0bc:	jns    0x18000e11d
    18000e0be:	outsb  %ds:(%rsi),(%dx)
    18000e0bf:	gs ja  0x18000e121
    18000e0c2:	insb   (%dx),%es:(%rdi)
    18000e0c3:	outsb  %gs:(%rsi),(%dx)
    18000e0c5:	addr32 je 0x18000e130
    18000e0c8:	rex jae 0x18000e13f
    18000e0cb:	fs rex
    18000e0cd:	rex add %al,(%rax)
-   18000e0d0:	test   $0x99,%al
-   18000e0d2:	add    %al,0x1(%rax)
+   18000e0d0:	enter  $0x99,$0x80
+   18000e0d4:	add    %eax,(%rax)
 	...
+   18000e0de:	add    %al,(%rax)
    18000e0e0:	cs (bad)
    18000e0e2:	push   %r14
    18000e0e4:	(bad)
    18000e0e9:	insb   (%dx),%es:(%rdi)
    18000e0ea:	insb   (%dx),%es:(%rdi)
    18000e0eb:	outsl  %ds:(%rsi),(%dx)
    18000e0ec:	movsxd 0x73(%rax),%eax
    18000e0ef:	je     0x18000e155
    18000e0f1:	rex
    18000e0f2:	rex add %al,(%rax)
    18000e0f5:	add    %al,(%rax)
-   18000e0f7:	add    %ch,0x1800099(%rax)
+   18000e0f7:	add    %cl,%al
+   18000e0f9:	cltd
+   18000e0fa:	add    %al,0x1(%rax)
 	...
-   18000e105:	add    %al,(%rax)
-   18000e107:	add    %ch,(%rsi)
-   18000e109:	(bad)
+   18000e108:	cs (bad)
    18000e10a:	push   %r14
    18000e10c:	gs js  0x18000e172
    18000e10f:	gs jo  0x18000e186
    18000e112:	imul   $0x64747340,0x6e(%rdi),%ebp
    18000e119:	rex
    18000e11a:	rex add %al,(%rax)
    18000e11d:	add    %al,(%rax)
-   18000e11f:	add    %ch,0x1800099(%rax)
+   18000e11f:	add    %cl,%al
+   18000e121:	cltd
+   18000e122:	add    %al,0x1(%rax)
 	...
-   18000e12d:	add    %al,(%rax)
-   18000e12f:	add    %ch,(%rsi)
-   18000e131:	(bad)
+   18000e130:	cs (bad)
    18000e132:	push   %r14
    18000e134:	jb     0x18000e1ab
    18000e136:	outsb  %ds:(%rsi),(%dx)
    18000e137:	je     0x18000e1a2
    18000e139:	insl   (%dx),%es:(%rdi)
    18000e13a:	gs pop %rdi
    18000e13c:	gs jb  0x18000e1b1
    18000e13f:	outsl  %ds:(%rsi),(%dx)
    18000e140:	jb     0x18000e182
    18000e142:	jae    0x18000e1b8
    18000e144:	fs rex
-   18000e146:	add    %bpl,0x1800099(%rax)
+   18000e146:	rex add %cl,%al
+   18000e149:	cltd
+   18000e14a:	add    %al,0x1(%rax)
 	...
-   18000e155:	add    %al,(%rax)
-   18000e157:	add    %ch,(%rsi)
-   18000e159:	(bad)
+   18000e158:	cs (bad)
    18000e15a:	push   %r14
    18000e15c:	(bad)
    18000e161:	(bad)
    18000e162:	jae    0x18000e1d8
    18000e164:	rex jae 0x18000e1db
    18000e167:	fs rex
    18000e169:	rex add %al,(%rax)
    18000e16c:	add    %al,(%rax)
    18000e16e:	add    %al,(%rax)
-   18000e170:	test   $0x99,%al
-   18000e172:	add    %al,0x1(%rax)
+   18000e170:	enter  $0x99,$0x80
+   18000e174:	add    %eax,(%rax)
 	...
+   18000e17e:	add    %al,(%rax)
    18000e180:	cs (bad)
    18000e182:	push   %r14
    18000e184:	rex.WRXB jo 0x18000e1ec
    18000e187:	outsb  %ds:(%rsi),(%dx)
    18000e188:	rex.RXB
    18000e189:	outsl  %gs:(%rsi),(%dx)
    18000e18b:	fs gs rex.RB js 0x18000e1f3
    18000e190:	gs jo  0x18000e207
    18000e193:	imul   $0x6f656740,0x6e(%rdi),%ebp
    18000e19a:	fs gs rex
    18000e19d:	rex add %al,(%rax)
-   18000e1a0:	test   $0x99,%al
-   18000e1a2:	add    %al,0x1(%rax)
+   18000e1a0:	enter  $0x99,$0x80
+   18000e1a4:	add    %eax,(%rax)
 	...
+   18000e1ae:	add    %al,(%rax)
    18000e1b0:	cs (bad)
    18000e1b2:	push   %r14
    18000e1b4:	rex.B je 0x18000e22b
    18000e1b7:	jb     0x18000e222
    18000e1b9:	(bad)
    18000e1be:	(bad)
    18000e1bf:	jae    0x18000e226
    18000e1c1:	rex
    18000e1c2:	outsl  %gs:(%esi),(%dx)
    18000e1c5:	fs gs rex
    18000e1c8:	rex add %al,(%rax)
    18000e1cb:	add    %al,(%rax)
    18000e1cd:	add    %al,(%rax)
-   18000e1cf:	add    %ch,0x1800099(%rax)
+   18000e1cf:	add    %cl,%al
+   18000e1d1:	cltd
+   18000e1d2:	add    %al,0x1(%rax)
 	...
-   18000e1dd:	add    %al,(%rax)
-   18000e1df:	add    %ch,(%rsi)
-   18000e1e1:	(bad)
+   18000e1e0:	cs (bad)
    18000e1e2:	push   %r14
    18000e1e4:	(bad)
    18000e1e5:	and    $0x56,%al
    18000e1e7:	(bad)
    18000e1e8:	jb     0x18000e253
    18000e1ea:	(bad)
    18000e1eb:	(bad)
@@ -18353,17 +18667,18 @@
    18000e220:	rex
    18000e221:	outsl  %gs:(%esi),(%dx)
    18000e224:	fs gs rex
    18000e227:	rex add %al,(%rax)
    18000e22a:	add    %al,(%rax)
    18000e22c:	add    %al,(%rax)
    18000e22e:	add    %al,(%rax)
-   18000e230:	test   $0x99,%al
-   18000e232:	add    %al,0x1(%rax)
+   18000e230:	enter  $0x99,$0x80
+   18000e234:	add    %eax,(%rax)
 	...
+   18000e23e:	add    %al,(%rax)
    18000e240:	cs (bad)
    18000e242:	push   %r14
    18000e244:	(bad)
    18000e245:	and    $0x6f,%al
    18000e247:	jo     0x18000e2bd
    18000e249:	imul   $0x56406c61,0x6e(%rdi),%ebp
    18000e250:	(bad)
@@ -18374,31 +18689,31 @@
    18000e25e:	outsl  %gs:(%rsi),(%dx)
    18000e260:	fs gs rex
    18000e263:	rex
    18000e264:	rex (bad)
    18000e266:	(bad)
    18000e26b:	add    %al,(%rax)
    18000e26d:	add    %al,(%rax)
-   18000e26f:	add    %ch,0x1800099(%rax)
+   18000e26f:	add    %cl,%al
+   18000e271:	cltd
+   18000e272:	add    %al,0x1(%rax)
 	...
-   18000e27d:	add    %al,(%rax)
-   18000e27f:	add    %ch,(%rsi)
-   18000e281:	(bad)
+   18000e280:	cs (bad)
    18000e282:	push   %r14
    18000e284:	imul   $0x40797261,0x72(%rdx),%r12
    18000e28c:	outsl  %gs:(%esi),(%dx)
    18000e28f:	fs gs rex
    18000e292:	rex add %al,(%rax)
 	...
    18000e29d:	add    %al,(%rax)
-   18000e29f:	add    %ch,0x1800099(%rax)
+   18000e29f:	add    %cl,%al
+   18000e2a1:	cltd
+   18000e2a2:	add    %al,0x1(%rax)
 	...
-   18000e2ad:	add    %al,(%rax)
-   18000e2af:	add    %ch,(%rsi)
-   18000e2b1:	(bad)
+   18000e2b0:	cs (bad)
    18000e2b2:	push   %r14
    18000e2b4:	(bad)
    18000e2b5:	and    $0x62,%al
    18000e2b7:	(bad)
    18000e2b8:	jae    0x18000e323
    18000e2ba:	movsxd 0x66(%rdi),%ebx
    18000e2bd:	imul   $0x44406675,0x62(%rbp,%riz,2),%ebp
@@ -18410,19 +18725,19 @@
    18000e2d0:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
    18000e2d8:	fs rex
    18000e2da:	rex
    18000e2db:	rex jae 0x18000e352
    18000e2de:	fs rex
    18000e2e0:	rex add %al,(%rax)
 	...
-   18000e2ef:	add    %ch,0x1800099(%rax)
+   18000e2ef:	add    %cl,%al
+   18000e2f1:	cltd
+   18000e2f2:	add    %al,0x1(%rax)
 	...
-   18000e2fd:	add    %al,(%rax)
-   18000e2ff:	add    %ch,(%rsi)
-   18000e301:	(bad)
+   18000e300:	cs (bad)
    18000e302:	push   %r14
    18000e304:	(bad)
    18000e305:	and    $0x62,%al
    18000e307:	(bad)
    18000e308:	jae    0x18000e373
    18000e30a:	movsxd 0x73(%rdi),%ebx
    18000e30d:	je     0x18000e381
@@ -18438,19 +18753,19 @@
    18000e32a:	fs rex
    18000e32c:	rex
    18000e32d:	rex jae 0x18000e3a4
    18000e330:	fs rex
    18000e332:	rex add %al,(%rax)
 	...
    18000e33d:	add    %al,(%rax)
-   18000e33f:	add    %ch,0x1800099(%rax)
+   18000e33f:	add    %cl,%al
+   18000e341:	cltd
+   18000e342:	add    %al,0x1(%rax)
 	...
-   18000e34d:	add    %al,(%rax)
-   18000e34f:	add    %ch,(%rsi)
-   18000e351:	(bad)
+   18000e350:	cs (bad)
    18000e352:	push   %r14
    18000e354:	(bad)
    18000e355:	and    $0x62,%al
    18000e357:	(bad)
    18000e358:	jae    0x18000e3c3
    18000e35a:	movsxd 0x66(%rdi),%ebx
    18000e35d:	jae    0x18000e3d3
@@ -18466,19 +18781,19 @@
    18000e370:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
    18000e378:	fs rex
    18000e37a:	rex
    18000e37b:	rex jae 0x18000e3f2
    18000e37e:	fs rex
    18000e380:	rex add %al,(%rax)
 	...
-   18000e38f:	add    %ch,0x1800099(%rax)
+   18000e38f:	add    %cl,%al
+   18000e391:	cltd
+   18000e392:	add    %al,0x1(%rax)
 	...
-   18000e39d:	add    %al,(%rax)
-   18000e39f:	add    %ch,(%rsi)
-   18000e3a1:	(bad)
+   18000e3a0:	cs (bad)
    18000e3a2:	push   %r14
    18000e3a4:	(bad)
    18000e3a5:	and    $0x62,%al
    18000e3a7:	(bad)
    18000e3a8:	jae    0x18000e413
    18000e3aa:	movsxd 0x69(%rdi),%ebx
    18000e3ad:	outsl  %ds:(%rsi),(%dx)
@@ -18495,17 +18810,18 @@
    18000e3c1:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
    18000e3c9:	fs rex
    18000e3cb:	rex
    18000e3cc:	rex jae 0x18000e443
    18000e3cf:	fs rex
    18000e3d1:	rex add %al,(%rax)
 	...
-   18000e3e0:	test   $0x99,%al
-   18000e3e2:	add    %al,0x1(%rax)
+   18000e3e0:	enter  $0x99,$0x80
+   18000e3e4:	add    %eax,(%rax)
 	...
+   18000e3ee:	add    %al,(%rax)
    18000e3f0:	cs (bad)
    18000e3f2:	push   %r14
    18000e3f4:	(bad)
    18000e3f5:	and    $0x62,%al
    18000e3f7:	(bad)
    18000e3f8:	jae    0x18000e463
    18000e3fa:	movsxd 0x69(%rdi),%ebx
@@ -18523,19 +18839,19 @@
    18000e418:	fs rex
    18000e41a:	rex
    18000e41b:	rex jae 0x18000e492
    18000e41e:	fs rex
    18000e420:	rex add %al,(%rax)
    18000e423:	add    %al,(%rax)
    18000e425:	add    %al,(%rax)
-   18000e427:	add    %ch,0x1800099(%rax)
+   18000e427:	add    %cl,%al
+   18000e429:	cltd
+   18000e42a:	add    %al,0x1(%rax)
 	...
-   18000e435:	add    %al,(%rax)
-   18000e437:	add    %ch,(%rsi)
-   18000e439:	(bad)
+   18000e438:	cs (bad)
    18000e43a:	push   %r14
    18000e43c:	(bad)
    18000e43d:	and    $0x62,%al
    18000e43f:	(bad)
    18000e440:	jae    0x18000e4ab
    18000e442:	movsxd 0x69(%rdi),%ebx
    18000e445:	outsl  %ds:(%rsi),(%dx)
@@ -18547,47 +18863,48 @@
    18000e452:	jb     0x18000e4b5
    18000e454:	imul   $0x74734044,0x40(%rbx,%rsi,2),%esi
    18000e45c:	fs rex
    18000e45e:	rex
    18000e45f:	rex jae 0x18000e4d6
    18000e462:	fs rex
    18000e464:	rex add %al,(%rax)
-   18000e467:	add    %ch,0x1800099(%rax)
+   18000e467:	add    %cl,%al
+   18000e469:	cltd
+   18000e46a:	add    %al,0x1(%rax)
 	...
-   18000e475:	add    %al,(%rax)
-   18000e477:	add    %ch,(%rsi)
-   18000e479:	(bad)
+   18000e478:	cs (bad)
    18000e47a:	push   %r14
    18000e47c:	imul   $0x7361625f,0x73(%rdi),%ebp
    18000e483:	gs rex jae 0x18000e4fb
    18000e487:	fs rex
    18000e489:	rex add %al,(%rax)
    18000e48c:	add    %al,(%rax)
    18000e48e:	add    %al,(%rax)
-   18000e490:	test   $0x99,%al
-   18000e492:	add    %al,0x1(%rax)
+   18000e490:	enter  $0x99,$0x80
+   18000e494:	add    %eax,(%rax)
 	...
+   18000e49e:	add    %al,(%rax)
    18000e4a0:	cs (bad)
    18000e4a2:	push   %r14
    18000e4a4:	(bad)
    18000e4a5:	and    $0x5f,%al
    18000e4a7:	rex.WB outsl %ds:(%rsi),(%dx)
    18000e4a9:	jae    0x18000e50d
    18000e4ab:	rex
    18000e4ac:	rex.W
    18000e4ad:	rex jae 0x18000e524
    18000e4b0:	fs rex
    18000e4b2:	rex add %al,(%rax)
 	...
    18000e4bd:	add    %al,(%rax)
-   18000e4bf:	add    %ch,0x1800099(%rax)
+   18000e4bf:	add    %cl,%al
+   18000e4c1:	cltd
+   18000e4c2:	add    %al,0x1(%rax)
 	...
-   18000e4cd:	add    %al,(%rax)
-   18000e4cf:	add    %ch,(%rsi)
-   18000e4d1:	(bad)
+   18000e4d0:	cs (bad)
    18000e4d2:	push   %r14
    18000e4d4:	(bad)
    18000e4d5:	and    $0x62,%al
    18000e4d7:	(bad)
    18000e4d8:	jae    0x18000e543
    18000e4da:	movsxd 0x6f(%rdi),%ebx
    18000e4dd:	jae    0x18000e553
@@ -18604,37 +18921,37 @@
    18000e4f8:	fs rex
    18000e4fa:	rex
    18000e4fb:	rex jae 0x18000e572
    18000e4fe:	fs rex
    18000e500:	rex add %al,(%rax)
    18000e503:	add    %al,(%rax)
    18000e505:	add    %al,(%rax)
-   18000e507:	add    %ch,0x1800099(%rax)
+   18000e507:	add    %cl,%al
+   18000e509:	cltd
+   18000e50a:	add    %al,0x1(%rax)
 	...
-   18000e515:	add    %al,(%rax)
-   18000e517:	add    %ch,(%rsi)
-   18000e519:	(bad)
+   18000e518:	cs (bad)
    18000e51a:	push   %r14
    18000e51c:	pop    %rdi
    18000e51d:	push   %rdx
    18000e51e:	gs pop %di
    18000e521:	movsxd 0x75(%rdi),%ebp
    18000e524:	outsb  %ds:(%rsi),(%dx)
    18000e525:	je     0x18000e586
    18000e527:	(bad)
    18000e529:	jae    0x18000e590
    18000e52b:	rex jae 0x18000e5a2
    18000e52e:	fs rex
    18000e530:	rex add %al,(%rax)
 	...
-   18000e53f:	add    %ch,0x1800099(%rax)
+   18000e53f:	add    %cl,%al
+   18000e541:	cltd
+   18000e542:	add    %al,0x1(%rax)
 	...
-   18000e54d:	add    %al,(%rax)
-   18000e54f:	add    %ch,(%rsi)
-   18000e551:	(bad)
+   18000e550:	cs (bad)
    18000e552:	push   %r14
    18000e554:	(bad)
    18000e555:	and    $0x52,%al
    18000e557:	gs (bad)
    18000e559:	rex.WRXB outsb %fs:(%rsi),(%dx)
    18000e55c:	insb   (%dx),%es:(%rdi)
    18000e55d:	jns    0x18000e5a0
@@ -18659,17 +18976,18 @@
    18000e590:	rex
    18000e591:	outsl  %gs:(%esi),(%dx)
    18000e594:	fs gs rex
    18000e597:	rex add %al,(%rax)
    18000e59a:	add    %al,(%rax)
    18000e59c:	add    %al,(%rax)
    18000e59e:	add    %al,(%rax)
-   18000e5a0:	test   $0x99,%al
-   18000e5a2:	add    %al,0x1(%rax)
+   18000e5a0:	enter  $0x99,$0x80
+   18000e5a4:	add    %eax,(%rax)
 	...
+   18000e5ae:	add    %al,(%rax)
    18000e5b0:	cs (bad)
    18000e5b2:	push   %r14
    18000e5b4:	(bad)
    18000e5b5:	and    $0x5f,%al
    18000e5b7:	push   %rdx
    18000e5b8:	gs pop %di
    18000e5bb:	movsxd 0x75(%rdi),%ebp
@@ -18705,17 +19023,18 @@
    18000e5ff:	outsl  %gs:(%esi),(%dx)
    18000e602:	fs gs rex
    18000e605:	rex
    18000e606:	rex jae 0x18000e67d
    18000e609:	fs rex
    18000e60b:	rex add %al,(%rax)
    18000e60e:	add    %al,(%rax)
-   18000e610:	test   $0x99,%al
-   18000e612:	add    %al,0x1(%rax)
+   18000e610:	enter  $0x99,$0x80
+   18000e614:	add    %eax,(%rax)
 	...
+   18000e61e:	add    %al,(%rax)
    18000e620:	cs (bad)
    18000e622:	push   %r14
    18000e624:	je     0x18000e69f
    18000e626:	jo     0x18000e68d
    18000e628:	pop    %rdi
    18000e629:	imul   $0x40406f,0x66(%rsi),%ebp
 	...
@@ -18745,90 +19064,90 @@
    18000f033:	add    %bl,0x14(%rcx)
    18000f036:	add    %al,(%rax)
    18000f038:	lods   %ds:(%rsi),%al
    18000f039:	scas   %es:(%rdi),%eax
    18000f03a:	add    %al,(%rax)
    18000f03c:	(bad)
    18000f03d:	adc    $0x0,%al
-   18000f03f:	add    %al,-0xbffffec(%rbx)
-   18000f045:	mov    $0x0,%bl
+   18000f03f:	add    %al,0x68000014(%rbx)
+   18000f045:	mov    $0x0,%ah
    18000f047:	add    %dl,-0x3affffec(%rax)
-   18000f04d:	adc    $0xb1d80000,%eax
+   18000f04d:	adc    $0xb24c0000,%eax
    18000f052:	add    %al,(%rax)
    18000f054:	rclb   0x18480000(%rip)        # 0x19848f05a
    18000f05a:	add    %al,(%rax)
-   18000f05c:	or     $0xb3,%al
-   18000f05e:	add    %al,(%rax)
-   18000f060:	push   %rax
-   18000f061:	sbb    %al,(%rax)
+   18000f05c:	xorb   $0x0,0x18500000(%rbx)
    18000f063:	add    %cl,%al
    18000f065:	sbb    (%rax),%al
-   18000f067:	add    %cl,(%rbx,%rsi,4)
-   18000f06a:	add    %al,(%rax)
-   18000f06c:	rcrb   (%rdx)
-   18000f06e:	add    %al,(%rax)
-   18000f070:	add    (%rbx),%bl
-   18000f072:	add    %al,(%rax)
-   18000f074:	push   %rax
+   18000f067:	add    %al,-0x2fffff4d(%rax)
+   18000f06d:	sbb    (%rax),%al
+   18000f06f:	add    %al,(%rdx)
+   18000f071:	sbb    (%rax),%eax
+   18000f073:	add    %al,%ah
    18000f075:	mov    $0x0,%dl
    18000f077:	add    %al,(%rdx)
    18000f079:	sbb    (%rax),%eax
    18000f07b:	add    %ch,(%rdx)
    18000f07d:	sbb    $0x0,%al
-   18000f07f:	add    %ah,-0x4e(%rax)
-   18000f082:	add    %al,(%rax)
-   18000f084:	sub    (%rax,%rax,1),%bl
+   18000f07f:	add    %dl,%ah
+   18000f081:	mov    $0x0,%dl
+   18000f083:	add    %ch,(%rdx)
+   18000f085:	sbb    $0x0,%al
    18000f087:	add    %dh,(%rax)
    18000f089:	sbb    $0x0,%al
-   18000f08b:	add    %bh,0x0(%rdx,%rsi,4)
+   18000f08b:	add    %dh,%al
+   18000f08d:	mov    $0x0,%dl
    18000f08f:	add    %dh,(%rax)
    18000f091:	sbb    $0x0,%al
    18000f093:	add    %dh,(%rsi)
    18000f095:	sbb    $0x0,%al
-   18000f097:	add    %cl,0x1c400000(%rdx,%rsi,4)
+   18000f097:	add    %al,(%rax)
+   18000f099:	mov    $0x0,%bl
+   18000f09b:	add    %al,0x1c(%rax)
    18000f09e:	add    %al,(%rax)
    18000f0a0:	jns    0x18000f0bf
    18000f0a2:	add    %al,(%rax)
-   18000f0a4:	mov    $0x800000b3,%esp
-   18000f0a9:	sbb    $0x1eb80000,%eax
-   18000f0ae:	add    %al,(%rax)
-   18000f0b0:	test   %dh,0x1ec00000(%rbx)
+   18000f0a4:	xor    %dh,0x1d8000(%rax,%rax,1)
+   18000f0ab:	add    %bh,-0x7ffffe2(%rax)
+   18000f0b1:	mov    $0x0,%bl
+   18000f0b3:	add    %al,%al
+   18000f0b5:	(bad)
    18000f0b6:	add    %al,(%rax)
    18000f0b8:	jg     0x18000f0da
    18000f0ba:	add    %al,(%rax)
    18000f0bc:	adc    $0xae,%al
    18000f0be:	add    %al,(%rax)
    18000f0c0:	andb   $0x0,(%rax)
    18000f0c3:	add    %bh,%ch
    18000f0c5:	and    (%rax),%al
-   18000f0c7:	add    %ch,0xb2(%rax)
-   18000f0cd:	and    (%rax),%eax
-   18000f0cf:	add    %dl,0x25(%rdi)
-   18000f0d2:	add    %al,(%rax)
-   18000f0d4:	push   $0x600000b1
+   18000f0c7:	add    %bl,(%rbx,%rsi,4)
+   18000f0ca:	add    %al,(%rax)
+   18000f0cc:	add    %ah,(%rbx)
+   18000f0ce:	add    %al,(%rax)
+   18000f0d0:	push   %rdi
+   18000f0d1:	and    $0xb1dc0000,%eax
+   18000f0d6:	add    %al,(%rax)
+   18000f0d8:	(bad)
    18000f0d9:	and    $0x25a50000,%eax
    18000f0de:	add    %al,(%rax)
-   18000f0e0:	push   %rax
+   18000f0e0:	(bad)
    18000f0e1:	mov    $0x0,%bl
    18000f0e3:	add    %ah,0x6f000025(%rbp)
    18000f0e9:	es add %al,(%rax)
-   18000f0ec:	pop    %rax
+   18000f0ec:	int3
    18000f0ed:	mov    $0x0,%bl
    18000f0ef:	add    %ch,0x26(%rdi)
    18000f0f2:	add    %al,(%rax)
    18000f0f4:	ja     0x18000f11c
    18000f0f6:	add    %al,(%rax)
-   18000f0f8:	je     0x18000f0ad
-   18000f0fa:	add    %al,(%rax)
-   18000f0fc:	andb   $0x0,(%rsi)
-   18000f0ff:	add    %cl,0x27(%rdi)
+   18000f0f8:	call   0x10000f1b0
+   18000f0fd:	es add %al,(%rax)
+   18000f100:	rex.WRXB (bad)
    18000f102:	add    %al,(%rax)
-   18000f104:	movsb  %ds:(%rsi),%es:(%rdi)
-   18000f105:	mov    $0x0,%cl
-   18000f107:	add    %dl,0x27(%rax)
+   18000f104:	sbb    %dh,0x27500000(%rdx)
    18000f10a:	add    %al,(%rax)
    18000f10c:	jl     0x18000f136
    18000f10e:	add    %al,(%rax)
    18000f110:	movsb  %ds:(%rsi),%es:(%rdi)
    18000f111:	stos   %eax,%es:(%rdi)
    18000f112:	add    %al,(%rax)
    18000f114:	subb   $0x0,(%rax)
@@ -18932,27 +19251,25 @@
    18000f223:	add    %ch,%ah
    18000f225:	lods   %ds:(%rsi),%eax
    18000f226:	add    %al,(%rax)
    18000f228:	add    %dh,(%rdx)
    18000f22a:	add    %al,(%rax)
    18000f22c:	and    $0x32,%al
    18000f22e:	add    %al,(%rax)
-   18000f230:	adc    $0xb2,%al
-   18000f232:	add    %al,(%rax)
-   18000f234:	xor    %dh,(%rdx)
+   18000f230:	mov    %dh,0x32300000(%rdx)
    18000f236:	add    %al,(%rax)
    18000f238:	pop    %rdi
    18000f239:	xor    (%rax),%al
    18000f23b:	add    %bh,0x32600000(%rdx,%rbp,4)
    18000f242:	add    %al,(%rax)
    18000f244:	popf
    18000f245:	xor    (%rax),%al
-   18000f247:	add    %ch,(%rdx,%rsi,4)
-   18000f24a:	add    %al,(%rax)
-   18000f24c:	movabs 0x8000003305000032,%al
+   18000f247:	add    %ah,-0x5fffff4e(%rax)
+   18000f24d:	xor    (%rax),%al
+   18000f24f:	add    %al,-0x7fffffcd(%rip)        # 0x10000f288
    18000f255:	stos   %al,%es:(%rdi)
    18000f256:	add    %al,(%rax)
    18000f258:	and    %dh,(%rbx)
    18000f25a:	add    %al,(%rax)
    18000f25c:	(bad)
    18000f25d:	xor    (%rax),%eax
    18000f25f:	add    %ch,0x600000aa(%rax)
@@ -18977,18 +19294,16 @@
    18000f294:	(bad)
    18000f295:	xor    $0x0,%al
    18000f297:	add    %cl,(%rcx)
    18000f299:	xor    $0xad9c0000,%eax
    18000f29e:	add    %al,(%rax)
    18000f2a0:	adc    %dh,0x35c10000(%rip)        # 0x1b5c1f2a6
    18000f2a6:	add    %al,(%rax)
-   18000f2a8:	push   %rsp
-   18000f2a9:	mov    $0x0,%cl
-   18000f2ab:	add    %dl,%al
-   18000f2ad:	xor    $0x36ad0000,%eax
+   18000f2a8:	enter  $0xb1,$0x0
+   18000f2ac:	shlb   0x36ad0000(%rip)        # 0x1b6adf2b2
    18000f2b2:	add    %al,(%rax)
    18000f2b4:	test   $0xaa,%al
    18000f2b6:	add    %al,(%rax)
    18000f2b8:	lock ss add %al,(%rax)
    18000f2bc:	and    $0x64000037,%eax
    18000f2c1:	scas   %es:(%rdi),%eax
    18000f2c2:	add    %al,(%rax)
@@ -19007,15 +19322,15 @@
    18000f2e0:	fdivs  (%rdi)
    18000f2e2:	add    %al,(%rax)
    18000f2e4:	pushf
    18000f2e5:	scas   %es:(%rdi),%eax
    18000f2e6:	add    %al,(%rax)
    18000f2e8:	and    %bh,(%rax)
    18000f2ea:	add    %al,(%rax)
-   18000f2ec:	mov    $0x1c000038,%ebp
+   18000f2ec:	mov    $0x90000038,%ebp
    18000f2f1:	mov    $0x0,%cl
    18000f2f3:	add    %dh,%al
    18000f2f5:	cmp    %al,(%rax)
    18000f2f7:	add    %dl,(%rax)
    18000f2f9:	cmp    %eax,(%rax)
    18000f2fb:	add    %dh,0x39100000(%rdx,%rbp,4)
    18000f302:	add    %al,(%rax)
@@ -19092,449 +19407,509 @@
    18000f3be:	add    %al,(%rax)
    18000f3c0:	and    %bh,(%rdi)
    18000f3c2:	add    %al,(%rax)
    18000f3c4:	push   %rbx
    18000f3c5:	add    %r8b,(%r8)
    18000f3c8:	and    %ch,0x45900000(%rbp)
    18000f3ce:	add    %al,(%rax)
-   18000f3d0:	(bad)
+   18000f3d0:	xlat   %ds:(%rbx)
    18000f3d1:	add    %r8b,(%r8)
    18000f3d4:	test   $0xaa,%al
    18000f3d6:	add    %al,(%rax)
    18000f3d8:	loopne 0x18000f41f
    18000f3da:	add    %al,(%rax)
-   18000f3dc:	jno    0x18000f424
-   18000f3de:	add    %al,(%rax)
-   18000f3e0:	xorb   $0x0,0x46710000(%rax)
-   18000f3e7:	add    %dl,%cl
-   18000f3e9:	rex.RX add %r8b,(%rax)
-   18000f3ec:	nop
-   18000f3ed:	mov    $0x0,%al
-   18000f3ef:	add    %dl,%cl
-   18000f3f1:	rex.RX add %r8b,(%rax)
-   18000f3f4:	loop   0x18000f43c
-   18000f3f6:	add    %al,(%rax)
-   18000f3f8:	test   $0xb0,%al
-   18000f3fa:	add    %al,(%rax)
-   18000f3fc:	lock rex.RX add %r8b,(%rax)
-   18000f400:	xor    0x0(%rdi),%eax
-   18000f403:	add    %bh,0x47400000(%rdx,%rbp,4)
-   18000f40a:	add    %al,(%rax)
-   18000f40c:	jg     0x18000f455
-   18000f40e:	add    %al,(%rax)
-   18000f410:	mov    $0x800000aa,%esp
-   18000f415:	rex.RXB add %r8b,(%r8)
-   18000f418:	ret
-   18000f419:	rex.RXB add %r8b,(%r8)
-   18000f41c:	mov    $0xe00000aa,%esp
+   18000f3dc:	rex.W
+   18000f3dd:	rex.RX add %r8b,(%rax)
+   18000f3e0:	xorb   $0x0,0x46480000(%rax)
+   18000f3e7:	add    %cl,(%rcx)
+   18000f3e9:	rex.RXB add %r8b,(%r8)
+   18000f3ec:	mov    %?,0x47090000(%rax)
+   18000f3f2:	add    %al,(%rax)
+   18000f3f4:	pop    %rdi
+   18000f3f5:	rex.RXB add %r8b,(%r8)
+   18000f3f8:	movabs 0x640000475f0000b0,%al
+   18000f401:	rex.RXB add %r8b,(%r8)
+   18000f404:	mov    $0xb0,%ah
+   18000f406:	add    %al,(%rax)
+   18000f408:	rex.RXB add %r8b,%fs:(%r8)
+   18000f40c:	insl   (%dx),%es:(%rdi)
+   18000f40d:	rex.RXB add %r8b,(%r8)
+   18000f410:	(bad)
+   18000f411:	mov    $0x0,%al
+   18000f413:	add    %dh,0x47(%rax)
+   18000f416:	add    %al,(%rax)
+   18000f418:	mov    $0x47,%bl
+   18000f41a:	add    %al,(%rax)
+   18000f41c:	mov    $0xc00000aa,%esp
    18000f421:	rex.RXB add %r8b,(%r8)
-   18000f424:	sub    $0xc8000048,%eax
-   18000f429:	lods   %ds:(%rsi),%al
-   18000f42a:	add    %al,(%rax)
-   18000f42c:	sub    $0xb8000048,%eax
-   18000f431:	rex.WXB add %al,(%r8)
-   18000f434:	(bad)
-   18000f435:	lods   %ds:(%rsi),%al
-   18000f436:	add    %al,(%rax)
-   18000f438:	mov    $0xc200004b,%eax
-   18000f43d:	rex.WXB add %al,(%r8)
-   18000f440:	adc    %ch,0x4bd00000(%rbp)
-   18000f446:	add    %al,(%rax)
-   18000f448:	lahf
-   18000f449:	rex.WRB add %r8b,(%r8)
-   18000f44c:	mov    $0xa00000b0,%eax
-   18000f451:	rex.WRB add %r8b,(%r8)
-   18000f454:	test   %cl,0x0(%rsi)
-   18000f457:	add    %dh,-0x55(%rax)
-   18000f45a:	add    %al,(%rax)
-   18000f45c:	nop
-   18000f45d:	rex.WRX add %r8b,(%rax)
-   18000f460:	movabs %al,0xb00000aabc00004e
-   18000f469:	rex.WRX add %r8b,(%rax)
-   18000f46c:	add    %cl,0x0(%rdi)
-   18000f46f:	add    %ch,0x200000aa(%rax)
-   18000f475:	rex.WRXB add %r8b,(%r8)
-   18000f478:	orb    $0x0,0x0(%rdi)
-   18000f47c:	and    $0xae,%al
+   18000f424:	incl   0x0(%rdi)
+   18000f427:	add    %bh,0x48000000(%rdx,%rbp,4)
+   18000f42e:	add    %al,(%rax)
+   18000f430:	rex.XB
+   18000f431:	rex.W add %al,(%rax)
+   18000f434:	mov    $0x600000aa,%esp
+   18000f439:	rex.W add %al,(%rax)
+   18000f43c:	lods   %ds:(%rsi),%eax
+   18000f43d:	rex.W add %al,(%rax)
+   18000f440:	enter  $0xac,$0x0
+   18000f444:	lods   %ds:(%rsi),%eax
+   18000f445:	rex.W add %al,(%rax)
+   18000f448:	ds rex.WR add %r8b,(%rax)
+   18000f44c:	(bad)
+   18000f44d:	lods   %ds:(%rsi),%al
+   18000f44e:	add    %al,(%rax)
+   18000f450:	ds rex.WR add %r8b,(%rax)
+   18000f454:	rex.W
+   18000f455:	rex.WR add %r8b,(%rax)
+   18000f458:	adc    %ch,0x4c500000(%rbp)
+   18000f45e:	add    %al,(%rax)
+   18000f460:	repz rex.WRX add %r8b,(%rax)
+   18000f464:	sub    $0xb1,%al
+   18000f466:	add    %al,(%rax)
+   18000f468:	add    %cl,0x0(%rdi)
+   18000f46b:	add    %dl,%dl
+   18000f46d:	push   %rax
+   18000f46e:	add    %al,(%rax)
+   18000f470:	(bad)
+   18000f471:	mov    $0x0,%al
+   18000f473:	add    %ah,%al
+   18000f475:	push   %rax
+   18000f476:	add    %al,(%rax)
+   18000f478:	(bad)
+   18000f479:	push   %rcx
+   18000f47a:	add    %al,(%rax)
+   18000f47c:	jo     0x18000f429
    18000f47e:	add    %al,(%rax)
-   18000f480:	orb    $0x0,0x0(%rdi)
-   18000f484:	movabs %al,0xa20000ae38000050
-   18000f48d:	push   %rax
+   18000f480:	rclb   0x0(%rcx)
+   18000f483:	add    %ah,%ch
+   18000f485:	push   %rcx
+   18000f486:	add    %al,(%rax)
+   18000f488:	mov    $0xf00000aa,%esp
+   18000f48d:	push   %rcx
    18000f48e:	add    %al,(%rax)
-   18000f490:	rclb   $0x0,0x0(%rax)
-   18000f494:	rex.WR scas %es:(%rdi),%al
+   18000f490:	rex push %rdx
+   18000f492:	add    %al,(%rax)
+   18000f494:	test   $0xaa,%al
    18000f496:	add    %al,(%rax)
-   18000f498:	rclb   $0x0,0x0(%rax)
-   18000f49c:	movabs %al,0xb00000aaa8000051
-   18000f4a5:	push   %rcx
-   18000f4a6:	add    %al,(%rax)
-   18000f4a8:	iret
-   18000f4a9:	push   %rcx
+   18000f498:	(bad)
+   18000f499:	push   %rdx
+   18000f49a:	add    %al,(%rax)
+   18000f49c:	rclb   $0x0,0x0(%rdx)
+   18000f4a0:	and    $0xae,%al
+   18000f4a2:	add    %al,(%rax)
+   18000f4a4:	rclb   $0x0,0x0(%rdx)
+   18000f4a8:	loop   0x18000f4fd
    18000f4aa:	add    %al,(%rax)
-   18000f4ac:	sub    %dh,0x52100000(%rax)
+   18000f4ac:	cmp    %ch,0x53e20000(%rsi)
    18000f4b2:	add    %al,(%rax)
-   18000f4b4:	cs push %rbx
-   18000f4b6:	add    %al,(%rax)
-   18000f4b8:	pushf
-   18000f4b9:	lods   %ds:(%rsi),%eax
+   18000f4b4:	add    %dl,0x0(%rax,%rax,1)
+   18000f4b8:	rex.WR scas %es:(%rdi),%al
    18000f4ba:	add    %al,(%rax)
-   18000f4bc:	xor    %dl,0x0(%rbx)
-   18000f4bf:	add    %bh,%bl
-   18000f4c1:	push   %rbx
+   18000f4bc:	add    %dl,0x0(%rax,%rax,1)
+   18000f4c0:	loop   0x18000f516
    18000f4c2:	add    %al,(%rax)
-   18000f4c4:	adc    %dh,0x54000000(%rcx)
+   18000f4c4:	test   $0xaa,%al
+   18000f4c6:	add    %al,(%rax)
+   18000f4c8:	lock push %rsp
    18000f4ca:	add    %al,(%rax)
-   18000f4cc:	lret   $0x54
-   18000f4cf:	add    %dl,(%rax)
-   18000f4d1:	scas   %es:(%rdi),%eax
-   18000f4d2:	add    %al,(%rax)
-   18000f4d4:	rclb   0x0(%rax,%rax,1)
-   18000f4d8:	movsl  %ds:(%rsi),%es:(%rdi)
+   18000f4cc:	andnps (%rax),%xmm0
+   18000f4cf:	add    %ch,(%rax)
+   18000f4d1:	mov    $0x0,%al
+   18000f4d3:	add    %dl,0x55(%rax)
+   18000f4d6:	add    %al,(%rax)
+   18000f4d8:	int3
    18000f4d9:	push   %rbp
    18000f4da:	add    %al,(%rax)
-   18000f4dc:	and    $0xaf,%al
+   18000f4dc:	adc    $0xae,%al
    18000f4de:	add    %al,(%rax)
-   18000f4e0:	mov    $0x55,%al
-   18000f4e2:	add    %al,(%rax)
-   18000f4e4:	out    %al,(%dx)
-   18000f4e5:	push   %rbp
-   18000f4e6:	add    %al,(%rax)
-   18000f4e8:	xor    $0xaf,%al
-   18000f4ea:	add    %al,(%rax)
-   18000f4ec:	out    %al,(%dx)
-   18000f4ed:	push   %rbp
-   18000f4ee:	add    %al,(%rax)
-   18000f4f0:	adcl   $0x0,0x0(%rsi)
-   18000f4f4:	rex scas %es:(%rdi),%eax
-   18000f4f6:	add    %al,(%rax)
-   18000f4f8:	adcl   $0x0,0x0(%rsi)
-   18000f4fc:	mov    %ss,0x0(%rsi)
-   18000f4ff:	add    %dl,0x0(%rdi,%rbp,4)
-   18000f503:	add    %dl,0x21000056(%rax)
-   18000f509:	push   %rdi
+   18000f4e0:	rclb   0x0(%rbp)
+   18000f4e3:	add    %ch,-0x7fffffaa(%rax)
+   18000f4e9:	mov    $0x0,%cl
+   18000f4eb:	add    %dh,0x7a000056(%rax)
+   18000f4f1:	push   %rdi
+   18000f4f2:	add    %al,(%rax)
+   18000f4f4:	adc    %ch,0x57800000(%rdi)
+   18000f4fa:	add    %al,(%rax)
+   18000f4fc:	push   %rbp
+   18000f4fd:	pop    %rax
+   18000f4fe:	add    %al,(%rax)
+   18000f500:	and    $0xaf,%al
+   18000f502:	add    %al,(%rax)
+   18000f504:	(bad)
+   18000f505:	pop    %rax
+   18000f506:	add    %al,(%rax)
+   18000f508:	sahf
+   18000f509:	pop    %rax
    18000f50a:	add    %al,(%rax)
-   18000f50c:	adc    %ch,0x57300000(%rbx)
+   18000f50c:	xor    $0xaf,%al
+   18000f50e:	add    %al,(%rax)
+   18000f510:	sahf
+   18000f511:	pop    %rax
    18000f512:	add    %al,(%rax)
-   18000f514:	out    %eax,(%dx)
-   18000f515:	push   $0xffffffffac140000
+   18000f514:	xor    0x0(%rcx),%ebx
+   18000f517:	add    %al,-0x51(%rax)
    18000f51a:	add    %al,(%rax)
-   18000f51c:	lock push $0x69380000
+   18000f51c:	xor    0x0(%rcx),%ebx
+   18000f51f:	add    %bh,(%rcx,%rbx,2)
    18000f522:	add    %al,(%rax)
-   18000f524:	subb   $0x0,0x69400000(%rdx)
-   18000f52b:	add    %bl,-0x7fffff97(%rcx)
-   18000f531:	stos   %al,%es:(%rdi)
+   18000f524:	push   %rsp
+   18000f525:	scas   %es:(%rdi),%eax
+   18000f526:	add    %al,(%rax)
+   18000f528:	rex pop %rcx
+   18000f52a:	add    %al,(%rax)
+   18000f52c:	rcrl   0x0(%rcx)
+   18000f52f:	add    %dl,(%rax)
+   18000f531:	stos   %eax,%es:(%rdi)
    18000f532:	add    %al,(%rax)
-   18000f534:	movabs 0x8400006c4b000069,%al
-   18000f53d:	scas   %es:(%rdi),%al
+   18000f534:	loopne 0x18000f58f
+   18000f536:	add    %al,(%rax)
+   18000f538:	scas   %es:(%rdi),%eax
+   18000f539:	imul   $0x0,(%rax),%eax
+   18000f53c:	adc    $0xac,%al
    18000f53e:	add    %al,(%rax)
-   18000f540:	push   %rax
-   18000f541:	insb   (%dx),%es:(%rdi)
+   18000f540:	mov    $0x6b,%al
    18000f542:	add    %al,(%rax)
-   18000f544:	subl   $0xffffff80,0x0(%rax,%rax,1)
-   18000f549:	stos   %al,%es:(%rdi)
-   18000f54a:	add    %al,(%rax)
-   18000f54c:	subl   $0xffffff9d,0x0(%rax,%rax,1)
-   18000f551:	insb   (%dx),%es:(%rdi)
+   18000f544:	clc
+   18000f545:	imul   $0x0,(%rax),%eax
+   18000f548:	subb   $0x0,0x6c000000(%rdx)
+   18000f54f:	add    %bl,0x6c(%rcx)
    18000f552:	add    %al,(%rax)
-   18000f554:	pop    %rsp
-   18000f555:	scas   %es:(%rdi),%al
-   18000f556:	add    %al,(%rax)
-   18000f558:	popf
-   18000f559:	insb   (%dx),%es:(%rdi)
-   18000f55a:	add    %al,(%rax)
-   18000f55c:	mov    $0x6c,%ch
+   18000f554:	subb   $0x0,0x6c600000(%rdx)
+   18000f55b:	add    %cl,(%rbx)
+   18000f55d:	outsl  %ds:(%rsi),(%dx)
    18000f55e:	add    %al,(%rax)
-   18000f560:	jo     0x18000f510
-   18000f562:	add    %al,(%rax)
-   18000f564:	lock insb (%dx),%es:(%rdi)
+   18000f560:	test   %ch,0x6f100000(%rsi)
    18000f566:	add    %al,(%rax)
-   18000f568:	rex.XB insl (%dx),%es:(%rdi)
+   18000f568:	rex.XB outsl %ds:(%rsi),(%dx)
    18000f56a:	add    %al,(%rax)
-   18000f56c:	mov    $0x430000ae,%eax
-   18000f571:	insl   (%dx),%es:(%rdi)
-   18000f572:	add    %al,(%rax)
-   18000f574:	push   %rdx
-   18000f575:	outsb  %ds:(%rsi),(%dx)
+   18000f56c:	subb   $0x0,0x6f430000(%rdx)
+   18000f573:	add    %bl,0x6f(%rbp)
    18000f576:	add    %al,(%rax)
-   18000f578:	enter  $0xae,$0x0
-   18000f57c:	push   %rdx
-   18000f57d:	outsb  %ds:(%rsi),(%dx)
+   18000f578:	pop    %rsp
+   18000f579:	scas   %es:(%rdi),%al
+   18000f57a:	add    %al,(%rax)
+   18000f57c:	pop    %rbp
+   18000f57d:	outsl  %ds:(%rsi),(%dx)
    18000f57e:	add    %al,(%rax)
-   18000f580:	push   %rdi
-   18000f581:	outsb  %ds:(%rsi),(%dx)
+   18000f580:	jne    0x18000f5f1
    18000f582:	add    %al,(%rax)
-   18000f584:	loopne 0x18000f534
+   18000f584:	jo     0x18000f534
    18000f586:	add    %al,(%rax)
-   18000f588:	(bad)
-   18000f589:	outsb  %ds:(%rsi),(%dx)
+   18000f588:	mov    $0x6f,%al
    18000f58a:	add    %al,(%rax)
-   18000f58c:	xor    $0x6f,%al
-   18000f58e:	add    %al,(%rax)
-   18000f590:	clc
-   18000f591:	scas   %es:(%rdi),%al
-   18000f592:	add    %al,(%rax)
-   18000f594:	pushf
-   18000f595:	outsl  %ds:(%rsi),(%dx)
-   18000f596:	add    %al,(%rax)
-   18000f598:	(bad)
-   18000f599:	outsl  %ds:(%rsi),(%dx)
-   18000f59a:	add    %al,(%rax)
-   18000f59c:	subb   $0x0,0x6fec0000(%rdx)
-   18000f5a3:	add    %dl,0x70(%rdi)
-   18000f5a6:	add    %al,(%rax)
-   18000f5a8:	and    $0xb4,%al
+   18000f58c:	add    0x0(%rax),%esi
+   18000f58f:	add    %bh,0x30000ae(%rax)
+   18000f595:	jo     0x18000f597
+   18000f597:	add    %dl,(%rdx)
+   18000f599:	jno    0x18000f59b
+   18000f59b:	add    %cl,%al
+   18000f59d:	scas   %es:(%rdi),%al
+   18000f59e:	add    %al,(%rax)
+   18000f5a0:	adc    0x0(%rcx),%dh
+   18000f5a3:	add    %dl,(%rdi)
+   18000f5a5:	jno    0x18000f5a7
+   18000f5a7:	add    %ah,%al
+   18000f5a9:	scas   %es:(%rdi),%al
    18000f5aa:	add    %al,(%rax)
-   18000f5ac:	pop    %rax
-   18000f5ad:	jo     0x18000f5af
-   18000f5af:	add    %bh,0x4c000070(%rcx)
-   18000f5b5:	mov    $0x0,%ah
-   18000f5b7:	add    %bh,0x70f80000(%rax,%rsi,2)
-   18000f5be:	add    %al,(%rax)
-   18000f5c0:	subb   $0x0,0x71080000(%rdx)
-   18000f5c7:	add    %dh,(%rbx)
-   18000f5c9:	jno    0x18000f5cb
-   18000f5cb:	add    %al,0x340000aa(%rax)
-   18000f5d1:	jno    0x18000f5d3
-   18000f5d3:	add    %dl,0x71(%rcx)
+   18000f5ac:	and    %dh,0x0(%rcx)
+   18000f5af:	add    %dh,%ah
+   18000f5b1:	jno    0x18000f5b3
+   18000f5b3:	add    %bh,%al
+   18000f5b5:	scas   %es:(%rdi),%al
+   18000f5b6:	add    %al,(%rax)
+   18000f5b8:	pop    %rsp
+   18000f5b9:	jb     0x18000f5bb
+   18000f5bb:	add    %dl,-0x55800000(%rdx,%rsi,2)
+   18000f5c2:	add    %al,(%rax)
+   18000f5c4:	lods   %ds:(%rsi),%al
+   18000f5c5:	jb     0x18000f5c7
+   18000f5c7:	add    %dl,(%rdi)
+   18000f5c9:	jae    0x18000f5cb
+   18000f5cb:	add    %bl,0x180000b4(%rax)
+   18000f5d1:	jae    0x18000f5d3
+   18000f5d3:	add    %bh,0x73(%rcx)
    18000f5d6:	add    %al,(%rax)
-   18000f5d8:	mov    $0x540000aa,%esp
-   18000f5dd:	jno    0x18000f5df
-   18000f5df:	add    %ch,-0x7bffff8f(%rdi)
-   18000f5e5:	mov    $0x0,%ah
-   18000f5e7:	add    %dh,0x2f000071(%rax)
-   18000f5ed:	jb     0x18000f5ef
-   18000f5ef:	add    %cl,0x72400000(%rsp,%rsi,4)
-   18000f5f6:	add    %al,(%rax)
-   18000f5f8:	pop    %rsi
-   18000f5f9:	jb     0x18000f5fb
-   18000f5fb:	add    %ch,0x7c0000b4(%rax)
-   18000f601:	jb     0x18000f603
-   18000f603:	add    %cl,%ah
-   18000f605:	jb     0x18000f607
-   18000f607:	add    %bh,0x72cc0000(%rdx,%rbp,4)
+   18000f5d8:	shlb   $0x0,0x737c00(%rax,%rax,1)
+   18000f5e0:	mov    $0x80000073,%eax
+   18000f5e5:	stos   %al,%es:(%rdi)
+   18000f5e6:	add    %al,(%rax)
+   18000f5e8:	enter  $0x73,$0x0
+   18000f5ec:	repz jae 0x18000f5ef
+   18000f5ef:	add    %al,-0xbffff56(%rax)
+   18000f5f5:	jae    0x18000f5f7
+   18000f5f7:	add    %dl,(%rcx)
+   18000f5f9:	je     0x18000f5fb
+   18000f5fb:	add    %bh,0x74140000(%rdx,%rbp,4)
+   18000f602:	add    %al,(%rax)
+   18000f604:	outsl  %ds:(%rsi),(%dx)
+   18000f605:	je     0x18000f607
+   18000f607:	add    %bh,%al
+   18000f609:	mov    $0x0,%ah
+   18000f60b:	add    %dh,0x74(%rax)
    18000f60e:	add    %al,(%rax)
-   18000f610:	loop   0x18000f685
-   18000f612:	add    %al,(%rax)
-   18000f614:	lods   %ds:(%rsi),%al
-   18000f615:	mov    $0x0,%ah
-   18000f617:	add    %ah,%ah
-   18000f619:	jae    0x18000f61b
-   18000f61b:	add    %ch,0x74(%rax)
-   18000f61e:	add    %al,(%rax)
-   18000f620:	call   0x1e800f6d9
-   18000f625:	je     0x18000f627
-   18000f627:	add    %bl,0x3c000075(%rcx)
-   18000f62d:	mov    $0x0,%ch
-   18000f62f:	add    %bl,0x75d90000(%rbp,%rsi,2)
-   18000f636:	add    %al,(%rax)
-   18000f638:	adc    $0xae,%al
-   18000f63a:	add    %al,(%rax)
-   18000f63c:	fdivl  0x0(%rbp)
-   18000f63f:	add    %dl,-0x43ffff8a(%rip)        # 0x13c00f6bb
-   18000f645:	stos   %al,%es:(%rdi)
-   18000f646:	add    %al,(%rax)
-   18000f648:	sbb    %dh,0x0(%rsi)
-   18000f64b:	add    %cl,0x0(%rsi,%rsi,2)
-   18000f64f:	add    %bh,0x764c0000(%rdx,%rbp,4)
-   18000f656:	add    %al,(%rax)
-   18000f658:	(bad)
-   18000f659:	jbe    0x18000f65b
-   18000f65b:	add    %bh,0x76640000(%rdx,%rbp,4)
-   18000f662:	add    %al,(%rax)
-   18000f664:	mov    %?,0x0(%rsi)
-   18000f667:	add    %bh,0x768c0000(%rdx,%rbp,4)
+   18000f610:	out    %eax,(%dx)
+   18000f611:	je     0x18000f613
+   18000f613:	add    %al,(%rax)
+   18000f615:	mov    $0x0,%ch
+   18000f617:	add    %al,(%rax)
+   18000f619:	jne    0x18000f61b
+   18000f61b:	add    %bl,(%rsi)
+   18000f61d:	jne    0x18000f61f
+   18000f61f:	add    %bl,(%rax)
+   18000f621:	mov    $0x0,%ch
+   18000f623:	add    %bh,0x758c0000(,%rsi,2)
+   18000f62a:	add    %al,(%rax)
+   18000f62c:	mov    $0x8c0000aa,%esp
+   18000f631:	jne    0x18000f633
+   18000f633:	add    %ah,0x1c000076(%rdx)
+   18000f639:	mov    $0x0,%ch
+   18000f63b:	add    %ah,0x77280000(%rsi,%rsi,2)
+   18000f642:	add    %al,(%rax)
+   18000f644:	pop    %rax
+   18000f645:	mov    $0x0,%ch
+   18000f647:	add    %ch,(%rax)
+   18000f649:	ja     0x18000f64b
+   18000f64b:	add    %bl,0x78(%rcx)
+   18000f64e:	add    %al,(%rax)
+   18000f650:	lods   %ds:(%rsi),%al
+   18000f651:	mov    $0x0,%ch
+   18000f653:	add    %bl,0x0(%rax,%rdi,2)
+   18000f657:	add    %bl,0x14000078(%rcx)
+   18000f65d:	scas   %es:(%rdi),%al
+   18000f65e:	add    %al,(%rax)
+   18000f660:	pushf
+   18000f661:	js     0x18000f663
+   18000f663:	add    %dl,%ch
+   18000f665:	js     0x18000f667
+   18000f667:	add    %bh,0x78d80000(%rdx,%rbp,4)
    18000f66e:	add    %al,(%rax)
-   18000f670:	movabs 0xa40000aabc000076,%eax
-   18000f679:	jbe    0x18000f67b
-   18000f67b:	add    %al,(%rdi,%rsi,2)
-   18000f67e:	add    %al,(%rax)
-   18000f680:	pushf
-   18000f681:	lods   %ds:(%rsi),%eax
-   18000f682:	add    %al,(%rax)
-   18000f684:	add    $0x77,%al
+   18000f670:	or     $0x79,%al
+   18000f672:	add    %al,(%rax)
+   18000f674:	mov    $0xc0000aa,%esp
+   18000f679:	jns    0x18000f67b
+   18000f67b:	add    %ah,(%rcx)
+   18000f67d:	jns    0x18000f67f
+   18000f67f:	add    %bh,0x79240000(%rdx,%rbp,4)
    18000f686:	add    %al,(%rax)
-   18000f688:	xor    $0x77,%al
-   18000f68a:	add    %al,(%rax)
-   18000f68c:	mov    $0x340000aa,%esp
-   18000f691:	ja     0x18000f693
-   18000f693:	add    %cl,0x77(%rax)
-   18000f696:	add    %al,(%rax)
-   18000f698:	mov    $0x480000aa,%esp
-   18000f69d:	ja     0x18000f69f
-   18000f69f:	add    %dl,-0x7fffff89(%rcx)
-   18000f6a5:	stos   %al,%es:(%rdi)
-   18000f6a6:	add    %al,(%rax)
-   18000f6a8:	xchg   %eax,%esp
-   18000f6a9:	ja     0x18000f6ab
-   18000f6ab:	add    %bl,(%rdi)
-   18000f6ad:	js     0x18000f6af
-   18000f6af:	add    %al,0x200000aa(%rax)
-   18000f6b5:	js     0x18000f6b7
-   18000f6b7:	add    %bh,0x6c000078(%rax)
-   18000f6bd:	mov    $0x0,%ch
-   18000f6bf:	add    %bh,-0x23ffff88(%rax)
-   18000f6c5:	js     0x18000f6c7
-   18000f6c7:	add    %al,-0x23ffff56(%rax)
-   18000f6cd:	js     0x18000f6cf
-   18000f6cf:	add    %al,-0x7fffff87(%rip)        # 0x10000f74e
-   18000f6d5:	stos   %al,%es:(%rdi)
-   18000f6d6:	add    %al,(%rax)
-   18000f6d8:	or     %bh,0x0(%rcx)
-   18000f6db:	add    %al,0x79(%rdx)
+   18000f688:	rex.WR jns 0x18000f68b
+   18000f68b:	add    %bh,0x794c0000(%rdx,%rbp,4)
+   18000f692:	add    %al,(%rax)
+   18000f694:	(bad)
+   18000f695:	jns    0x18000f697
+   18000f697:	add    %bh,0x79640000(%rdx,%rbp,4)
+   18000f69e:	add    %al,(%rax)
+   18000f6a0:	(bad)
+   18000f6a1:	jns    0x18000f6a3
+   18000f6a3:	add    %bl,0x79c40000(%rbp,%rbp,4)
+   18000f6aa:	add    %al,(%rax)
+   18000f6ac:	hlt
+   18000f6ad:	jns    0x18000f6af
+   18000f6af:	add    %bh,0x79f40000(%rdx,%rbp,4)
+   18000f6b6:	add    %al,(%rax)
+   18000f6b8:	or     %bh,0x0(%rdx)
+   18000f6bb:	add    %bh,0x7a080000(%rdx,%rbp,4)
+   18000f6c2:	add    %al,(%rax)
+   18000f6c4:	push   %rcx
+   18000f6c5:	jp     0x18000f6c7
+   18000f6c7:	add    %al,0x540000aa(%rax)
+   18000f6cd:	jp     0x18000f6cf
+   18000f6cf:	add    %bl,%bh
+   18000f6d1:	jp     0x18000f6d3
+   18000f6d3:	add    %al,-0x1fffff56(%rax)
+   18000f6d9:	jp     0x18000f6db
+   18000f6db:	add    %bh,0x7b(%rax)
    18000f6de:	add    %al,(%rax)
-   18000f6e0:	subb   $0x0,0x79440000(%rdx)
-   18000f6e7:	add    %bl,0x79(%rbx)
-   18000f6ea:	add    %al,(%rax)
-   18000f6ec:	mov    $0x800000aa,%esp
-   18000f6f1:	jns    0x18000f6f3
-   18000f6f3:	add    %ah,-0x4bffff87(%rax)
-   18000f6f9:	stos   %al,%es:(%rdi)
-   18000f6fa:	add    %al,(%rax)
-   18000f6fc:	test   $0x79,%al
-   18000f6fe:	add    %al,(%rax)
-   18000f700:	fdivrl 0x0(%rcx)
-   18000f703:	add    %al,-0x23ffff56(%rax)
-   18000f709:	jns    0x18000f70b
-   18000f70b:	add    %ch,-0x6bffff86(%rsi)
-   18000f711:	mov    $0x0,%ch
-   18000f713:	add    %dh,0x2100007a(%rax)
-   18000f719:	jnp    0x18000f71b
-   18000f71b:	add    %bl,0x7b240000(%rbp,%rsi,4)
+   18000f6e0:	fdivl  0x7b780000(%rbp)
+   18000f6e6:	add    %al,(%rax)
+   18000f6e8:	pushf
+   18000f6e9:	jnp    0x18000f6eb
+   18000f6eb:	add    %al,-0x63ffff56(%rax)
+   18000f6f1:	jnp    0x18000f6f3
+   18000f6f3:	add    %al,%ch
+   18000f6f5:	jnp    0x18000f6f7
+   18000f6f7:	add    %al,-0x37ffff56(%rax)
+   18000f6fd:	jnp    0x18000f6ff
+   18000f6ff:	add    %al,(%rdx)
+   18000f701:	jl     0x18000f703
+   18000f703:	add    %al,0x40000aa(%rax)
+   18000f709:	jl     0x18000f70b
+   18000f70b:	add    %bl,(%rbx)
+   18000f70d:	jl     0x18000f70f
+   18000f70f:	add    %bh,0x7c400000(%rdx,%rbp,4)
+   18000f716:	add    %al,(%rax)
+   18000f718:	(bad)
+   18000f719:	jl     0x18000f71b
+   18000f71b:	add    %dh,0x7c680000(%rdx,%rbp,4)
    18000f722:	add    %al,(%rax)
-   18000f724:	sarb   0x0(%rbx)
-   18000f727:	add    %ch,-0x2fffff4b(%rax)
-   18000f72d:	jnp    0x18000f72f
-   18000f72f:	add    %dh,%bl
-   18000f731:	jnp    0x18000f733
-   18000f733:	add    %bh,0x7c040000(%rdx,%rbp,4)
+   18000f724:	pushf
+   18000f725:	jl     0x18000f727
+   18000f727:	add    %al,-0x63ffff56(%rax)
+   18000f72d:	jl     0x18000f72f
+   18000f72f:	add    %ch,0x7d(%rsi)
+   18000f732:	add    %al,(%rax)
+   18000f734:	add    $0xb6,%al
+   18000f736:	add    %al,(%rax)
+   18000f738:	jo     0x18000f7b7
    18000f73a:	add    %al,(%rax)
-   18000f73c:	(bad)
-   18000f73d:	jl     0x18000f73f
-   18000f73f:	add    %bh,0x7c300000(%rdx,%rbp,4)
+   18000f73c:	loope  0x18000f7bb
+   18000f73e:	add    %al,(%rax)
+   18000f740:	or     $0xb6,%al
+   18000f742:	add    %al,(%rax)
+   18000f744:	in     $0x7d,%al
    18000f746:	add    %al,(%rax)
-   18000f748:	jnp    0x18000f7c7
-   18000f74a:	add    %al,(%rax)
-   18000f74c:	mov    $0xb5,%ah
-   18000f74e:	add    %al,(%rax)
-   18000f750:	jl     0x18000f7cf
-   18000f752:	add    %al,(%rax)
-   18000f754:	mov    $0xa800007d,%eax
-   18000f759:	stos   %al,%es:(%rdi)
-   18000f75a:	add    %al,(%rax)
-   18000f75c:	mov    $0xf400007d,%eax
-   18000f761:	jge    0x18000f763
-   18000f763:	add    %ch,-0xbffff56(%rax)
-   18000f769:	jge    0x18000f76b
-   18000f76b:	add    %dl,-0x3bffff81(%rbp)
-   18000f771:	mov    $0x0,%ch
-   18000f773:	add    %dh,-0x80(%rax)
+   18000f748:	nop
+   18000f749:	jle    0x18000f74b
+   18000f74b:	add    %bl,(%rax)
+   18000f74d:	mov    $0x0,%dh
+   18000f74f:	add    %dl,-0x4cffff82(%rax)
+   18000f755:	jle    0x18000f757
+   18000f757:	add    %bh,0x7ec40000(%rdx,%rbp,4)
+   18000f75e:	add    %al,(%rax)
+   18000f760:	fistpll 0x0(%rsi)
+   18000f763:	add    %bh,0x7ef00000(%rdx,%rbp,4)
+   18000f76a:	add    %al,(%rax)
+   18000f76c:	cmp    -0x49dc0000(%rax),%eax
+   18000f772:	add    %al,(%rax)
+   18000f774:	cmp    $0x80,%al
    18000f776:	add    %al,(%rax)
-   18000f778:	jb     0x18000f6fa
+   18000f778:	js     0x18000f6fa
    18000f77a:	add    %al,(%rax)
-   18000f77c:	fdivs  -0x7f700000(%rbp)
+   18000f77c:	test   $0xaa,%al
+   18000f77e:	add    %al,(%rax)
+   18000f780:	js     0x18000f702
    18000f782:	add    %al,(%rax)
-   18000f784:	xchg   %eax,%esi
-   18000f785:	addb   $0x0,(%rax)
-   18000f788:	loopne 0x18000f73f
+   18000f784:	mov    $0x80,%ah
+   18000f786:	add    %al,(%rax)
+   18000f788:	test   $0xaa,%al
    18000f78a:	add    %al,(%rax)
-   18000f78c:	movabs 0x78000080bd000080,%al
-   18000f795:	stos   %al,%es:(%rdi)
+   18000f78c:	mov    $0x80,%ah
+   18000f78e:	add    %al,(%rax)
+   18000f790:	push   %rbp
+   18000f791:	(bad)
+   18000f792:	add    %al,(%rax)
+   18000f794:	xor    $0xb6,%al
    18000f796:	add    %al,(%rax)
-   18000f798:	loopne 0x18000f71a
-   18000f79a:	add    %al,(%rax)
-   18000f79c:	sbb    -0x526c0000(%rcx),%eax
-   18000f7a2:	add    %al,(%rax)
-   18000f7a4:	and    %al,-0x7ec90000(%rcx)
-   18000f7aa:	add    %al,(%rax)
-   18000f7ac:	xchg   %eax,%esp
-   18000f7ad:	lods   %ds:(%rsi),%eax
-   18000f7ae:	add    %al,(%rax)
-   18000f7b0:	rex addl $0x816800,(%rax)
-   18000f7b7:	add    %dl,-0x7e900000(%rbp,%rbp,4)
-   18000f7be:	add    %al,(%rax)
-   18000f7c0:	cwtl
-   18000f7c1:	addl   $0xad9400,(%rax)
-   18000f7c7:	add    %ah,-0x2fffff7f(%rax)
-   18000f7cd:	addl   $0xad9400,(%rax)
-   18000f7d3:	add    %dl,%al
-   18000f7d5:	addl   $0x820000,(%rax)
-   18000f7db:	add    %dl,-0x7df00000(%rbp,%rbp,4)
-   18000f7e2:	add    %al,(%rax)
-   18000f7e4:	cmp    %eax,-0x55880000(%rdx)
+   18000f798:	xor    %al,-0x7cce0000(%rbx)
+   18000f79e:	add    %al,(%rax)
+   18000f7a0:	rex.W mov $0x0,%sil
+   18000f7a3:	add    %dl,-0x7d(%rax)
+   18000f7a6:	add    %al,(%rax)
+   18000f7a8:	push   %rsi
+   18000f7a9:	addl   $0x0,(%rax)
+   18000f7ac:	push   %rax
+   18000f7ad:	mov    $0x0,%dh
+   18000f7af:	add    %ah,-0x7d(%rax)
+   18000f7b2:	add    %al,(%rax)
+   18000f7b4:	jge    0x18000f739
+   18000f7b6:	add    %al,(%rax)
+   18000f7b8:	js     0x18000f764
+   18000f7ba:	add    %al,(%rax)
+   18000f7bc:	movabs 0x94000083db000083,%al
+   18000f7c5:	lods   %ds:(%rsi),%eax
+   18000f7c6:	add    %al,(%rax)
+   18000f7c8:	loopne 0x18000f74d
+   18000f7ca:	add    %al,(%rax)
+   18000f7cc:	testl  $0x84000000,-0x526c0000(%rbx)
+   18000f7d6:	add    %al,(%rax)
+   18000f7d8:	sub    %al,0xad9400(%rax,%rax,1)
+   18000f7df:	add    %dh,(%rax)
+   18000f7e1:	test   %al,(%rax)
+   18000f7e3:	add    %bl,-0x7c(%rax)
+   18000f7e6:	add    %al,(%rax)
+   18000f7e8:	xchg   %eax,%esp
+   18000f7e9:	lods   %ds:(%rsi),%eax
    18000f7ea:	add    %al,(%rax)
-   18000f7ec:	rex (bad)
-   18000f7ee:	add    %al,(%rax)
-   18000f7f0:	(bad)
-   18000f7f1:	(bad)
-   18000f7f2:	add    %al,(%rax)
-   18000f7f4:	js     0x18000f7a0
+   18000f7ec:	(bad)
+   18000f7ed:	test   %al,(%rax)
+   18000f7ef:	add    %dl,-0x6bffff7c(%rax)
+   18000f7f5:	lods   %ds:(%rsi),%eax
    18000f7f6:	add    %al,(%rax)
-   18000f7f8:	adc    %al,-0x7cc00000(%rbx)
-   18000f7fe:	add    %al,(%rax)
-   18000f800:	xchg   %eax,%esp
-   18000f801:	lods   %ds:(%rsi),%eax
-   18000f802:	add    %al,(%rax)
-   18000f804:	rex addl $0x0,(%rax)
-   18000f808:	pop    %rbp
-   18000f809:	addl   $0x0,(%rax)
-   18000f80c:	js     0x18000f7b8
+   18000f7f8:	nop
+   18000f7f9:	test   %al,(%rax)
+   18000f7fb:	add    %al,%al
+   18000f7fd:	test   %al,(%rax)
+   18000f7ff:	add    %dl,-0x7b300000(%rbp,%rbp,4)
+   18000f806:	add    %al,(%rax)
+   18000f808:	stc
+   18000f809:	test   %al,(%rax)
+   18000f80b:	add    %bh,-0x56(%rax)
    18000f80e:	add    %al,(%rax)
-   18000f810:	rolb   -0x7bfe0000(%rbx)
+   18000f810:	add    %al,-0x7ae00000(%rbp)
    18000f816:	add    %al,(%rax)
-   18000f818:	xchg   %eax,%esp
-   18000f819:	lods   %ds:(%rsi),%eax
+   18000f818:	js     0x18000f7c4
    18000f81a:	add    %al,(%rax)
-   18000f81c:	adc    %al,0x843000(%rax,%rax,1)
-   18000f823:	add    %bh,-0x56(%rax)
+   18000f81c:	rolb   -0x7a000000(%rbp)
+   18000f822:	add    %al,(%rax)
+   18000f824:	xchg   %eax,%esp
+   18000f825:	lods   %ds:(%rsi),%eax
    18000f826:	add    %al,(%rax)
-   18000f828:	jo     0x18000f7ae
-   18000f82a:	add    %al,(%rax)
-   18000f82c:	xchg   %eax,%esi
-   18000f82d:	test   %al,(%rax)
-   18000f82f:	add    %bh,-0x56(%rax)
+   18000f828:	add    %al,-0x79e30000(%rsi)
+   18000f82e:	add    %al,(%rax)
+   18000f830:	js     0x18000f7dc
    18000f832:	add    %al,(%rax)
-   18000f834:	rolb   0x84fe00(%rax,%rax,1)
-   18000f83b:	add    %bh,-0x56(%rax)
-   18000f83e:	add    %al,(%rax)
-   18000f840:	insb   (%dx),%es:(%rdi)
-   18000f841:	test   %eax,(%rax)
-   18000f843:	add    %bl,0x78000085(%rax)
-   18000f849:	stos   %al,%es:(%rdi)
+   18000f834:	nop
+   18000f835:	xchg   %al,(%rax)
+   18000f837:	add    %al,%dl
+   18000f839:	xchg   %al,(%rax)
+   18000f83b:	add    %dl,-0x79300000(%rbp,%rbp,4)
+   18000f842:	add    %al,(%rax)
+   18000f844:	in     (%dx),%eax
+   18000f845:	xchg   %al,(%rax)
+   18000f847:	add    %bh,-0x56(%rax)
    18000f84a:	add    %al,(%rax)
-   18000f84c:	cwtl
-   18000f84d:	test   %eax,(%rax)
-   18000f84f:	add    %dh,%bh
-   18000f851:	test   %eax,(%rax)
-   18000f853:	add    %bh,-0x4c(%rax)
+   18000f84c:	xor    %al,-0x78b00000(%rdi)
+   18000f852:	add    %al,(%rax)
+   18000f854:	js     0x18000f800
    18000f856:	add    %al,(%rax)
-   18000f858:	testl  $0xaa780000,-0x79f20000(%rbp)
+   18000f858:	nop
+   18000f859:	xchg   %eax,(%rax)
+   18000f85b:	add    %dh,0x78000087(%rsi)
+   18000f861:	stos   %al,%es:(%rdi)
    18000f862:	add    %al,(%rax)
-   18000f864:	(bad)
-   18000f865:	xchg   %al,(%rax)
-   18000f867:	add    %ah,(%rdi)
-   18000f869:	xchg   %al,(%rax)
+   18000f864:	lock xchg %eax,(%rax)
+   18000f867:	add    %bl,(%rsi)
+   18000f869:	mov    %al,(%rax)
    18000f86b:	add    %bh,-0x56(%rax)
    18000f86e:	add    %al,(%rax)
-   18000f870:	(bad)
-   18000f871:	xchg   %al,(%rax)
-   18000f873:	add    %bh,(%rbx)
-   18000f875:	xchg   %al,(%rax)
-   18000f877:	add    %bh,-0x56(%rax)
+   18000f870:	mov    %cs,-0x77480000(%rax)
+   18000f876:	add    %al,(%rax)
+   18000f878:	js     0x18000f824
    18000f87a:	add    %al,(%rax)
-   18000f87c:	cmp    -0x798f0000(%rsi),%eax
-   18000f882:	add    %al,(%rax)
-   18000f884:	fs mov $0x0,%ch
-   18000f887:	add    %dh,-0x7a(%rcx)
-   18000f88a:	add    %al,(%rax)
-   18000f88c:	mov    %eax,-0x4a740000(%rsi)
+   18000f87c:	mov    $0x17000088,%eax
+   18000f881:	mov    %eax,(%rax)
+   18000f883:	add    %ch,%ah
+   18000f885:	mov    $0x0,%ah
+   18000f887:	add    %dl,(%rdi)
+   18000f889:	mov    %eax,(%rax)
+   18000f88b:	add    %ch,(%rsi)
+   18000f88d:	mov    %eax,(%rax)
+   18000f88f:	add    %bh,-0x56(%rax)
    18000f892:	add    %al,(%rax)
-   18000f894:	mov    %es,-0x79190000(%rsi)
+   18000f894:	cs mov %eax,(%rax)
+   18000f897:	add    %al,-0x77(%rdi)
    18000f89a:	add    %al,(%rax)
-   18000f89c:	.byte 0x80
-   18000f89d:	stos   %al,%es:(%rdi)
+   18000f89c:	js     0x18000f848
+   18000f89e:	add    %al,(%rax)
+   18000f8a0:	rex.RXB mov %r8d,(%r8)
+   18000f8a3:	add    %bl,-0x77(%rbx)
+   18000f8a6:	add    %al,(%rax)
+   18000f8a8:	js     0x18000f854
+   18000f8aa:	add    %al,(%rax)
+   18000f8ac:	pop    %rbx
+   18000f8ad:	mov    %eax,(%rax)
+   18000f8af:	add    %dl,-0x2bffff77(%rcx)
+   18000f8b5:	mov    $0x0,%ch
+   18000f8b7:	add    %dl,-0x56ffff77(%rcx)
+   18000f8bd:	mov    %eax,(%rax)
+   18000f8bf:	add    %bh,%ah
+   18000f8c1:	mov    $0x0,%ch
+   18000f8c3:	add    %ch,-0x75f90000(%rcx,%rcx,4)
+   18000f8ca:	add    %al,(%rax)
+   18000f8cc:	.byte 0x80
+   18000f8cd:	stos   %al,%es:(%rdi)
 	...
 
 Disassembly of section .rsrc:
 
 0000000180010000 <.rsrc>:
 	...
    180010008:	add    $0x0,%al
@@ -19745,23 +20120,26 @@
    180011071:	cmpsl  %es:(%rdi),%ds:(%rsi)
    180011072:	(bad)
    180011073:	cmpsl  %es:(%rdi),%ds:(%rsi)
    180011074:	push   $0x78a770a7
    180011079:	cmpsl  %es:(%rdi),%ds:(%rsi)
    18001107a:	andb   $0x98,-0x586f5878(%rdi)
    180011081:	cmpsl  %es:(%rdi),%ds:(%rsi)
-   180011082:	movabs 0x50a848a840a838a7,%al
+   180011082:	movabs 0x50a848a840a7a8a7,%al
    18001108b:	test   $0x58,%al
-   18001108d:	test   $0xa0,%al
-   18001108f:	test   $0xa9e0a9a8,%eax
-   180011094:	call   0x100ab7942
-   180011099:	stos   %al,%es:(%rdi)
-   18001109a:	mov    %ch,-0x54d754f0(%rdx)
-   1800110a0:	xor    %ch,-0x54bf54c8(%rbx)
-   1800110a6:	add    %al,(%rax)
+   18001108d:	test   $0x60,%al
+   18001108f:	test   $0xc0,%al
+   180011091:	test   $0xa9e8a9c8,%eax
+   180011096:	lock test $0xaa90aa78,%eax
+   18001109c:	cwtl
+   18001109d:	stos   %al,%es:(%rdi)
+   18001109e:	and    %ch,-0x54bf54c8(%rbx)
+   1800110a4:	stos   %rax,%es:(%rdi)
+   1800110a6:	push   %rax
+   1800110a7:	stos   %eax,%es:(%rdi)
    1800110a8:	add    %ah,%al
    1800110aa:	add    %al,(%rax)
    1800110ac:	cmp    $0x0,%al
    1800110ae:	add    %al,(%rax)
    1800110b0:	rex movabs 0xa0f8a0d0a0a0a068,%al
    1800110ba:	and    %ah,-0x5e8f5eb8(%rcx)
    1800110c0:	movabs 0xa0a270a230a1d0a1,%al
```

## Comparing `Geode_Viewables-2.0.2.dist-info/METADATA` & `Geode_Viewables-2.0.3rc1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: Geode-Viewables
-Version: 2.0.2
+Version: 2.0.3rc1
 Summary: Geode module to objects visualization
 Home-page: https://github.com/Geode-solutions/Geode-Viewables
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: geode-common (==25.*,>=25.0.0)
-Requires-Dist: opengeode-core (==14.*,>=14.0.0)
-Requires-Dist: opengeode-geosciences (==7.*,>=7.0.0)
-Requires-Dist: opengeode-io (==6.*,>=6.0.0)
+Requires-Dist: geode-common (==26.*,>=26.0.4)
+Requires-Dist: opengeode-core (==14.*,>=14.3.1)
+Requires-Dist: opengeode-geosciences (==7.*,>=7.0.11)
+Requires-Dist: opengeode-io (==6.*,>=6.0.7)
 
 <h1 align="center">Geode-Viewables<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Utilities to help visualizing OpenGeode objects</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-Viewables_private/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/Geode-Viewables_private/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: Geode-Viewables Version: 2.0.2 Summary: Geode
+Metadata-Version: 2.1 Name: Geode-Viewables Version: 2.0.3rc1 Summary: Geode
 module to objects visualization Home-page: https://github.com/Geode-solutions/
 Geode-Viewables Author: Geode-solutions Author-email: contact@geode-
 solutions.com License: Proprietary Platform: UNKNOWN Description-Content-Type:
-text/markdown Requires-Dist: geode-common (==25.*,>=25.0.0) Requires-Dist:
-opengeode-core (==14.*,>=14.0.0) Requires-Dist: opengeode-geosciences
-(==7.*,>=7.0.0) Requires-Dist: opengeode-io (==6.*,>=6.0.0)
+text/markdown Requires-Dist: geode-common (==26.*,>=26.0.4) Requires-Dist:
+opengeode-core (==14.*,>=14.3.1) Requires-Dist: opengeode-geosciences
+(==7.*,>=7.0.11) Requires-Dist: opengeode-io (==6.*,>=6.0.7)
                 ****** Geode-Viewablesby Geode-solutions ******
            **** Utilities to help visualizing OpenGeode objects ****
                 [Build Status] [Deploy Status] [Version] [PyPI]
              [Windows support] [Ubuntu support] [Red Hat support]
                  [Language] [Semantic-release] [Slack_invite]
```

