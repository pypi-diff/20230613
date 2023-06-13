# Comparing `tmp/starcatalogquery-0.1.5-py3-none-any.whl.zip` & `tmp/starcatalogquery-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 27169 bytes, number of entries: 17
+Zip file size: 27067 bytes, number of entries: 17
 -rw-r--r--  2.0 unx       33 b- defN 23-May-08 07:01 starcatalogquery/__init__.py
 -rw-r--r--  2.0 unx     6048 b- defN 23-May-09 01:27 starcatalogquery/catalog_check.py
 -rw-r--r--  2.0 unx     6716 b- defN 23-May-09 01:26 starcatalogquery/catalog_download.py
 -rw-r--r--  2.0 unx    15124 b- defN 23-May-08 13:32 starcatalogquery/catalog_query.py
--rw-r--r--  2.0 unx    51627 b- defN 23-May-15 03:52 starcatalogquery/classes.py
+-rw-r--r--  2.0 unx    51224 b- defN 23-Jun-13 08:08 starcatalogquery/classes.py
 -rw-r--r--  2.0 unx     3078 b- defN 23-May-12 08:00 starcatalogquery/invariantfeatures.py
 -rw-r--r--  2.0 unx     5624 b- defN 23-May-10 03:48 starcatalogquery/tiles_draw.py
--rw-r--r--  2.0 unx     1937 b- defN 23-May-09 08:46 starcatalogquery/wcs.py
+-rw-r--r--  2.0 unx     1978 b- defN 23-May-30 08:00 starcatalogquery/wcs.py
 -rw-r--r--  2.0 unx        1 b- defN 23-May-11 04:20 starcatalogquery/utils/__init__.py
 -rw-r--r--  2.0 unx      612 b- defN 23-May-09 08:08 starcatalogquery/utils/df2info.py
 -rw-r--r--  2.0 unx     4272 b- defN 23-May-09 08:33 starcatalogquery/utils/starcatalog_statistic.py
 -rw-r--r--  2.0 unx      477 b- defN 23-May-09 08:06 starcatalogquery/utils/try_download.py
--rw-r--r--  2.0 unx     1068 b- defN 23-May-15 09:33 starcatalogquery-0.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    12523 b- defN 23-May-15 09:33 starcatalogquery-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 09:33 starcatalogquery-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-May-15 09:33 starcatalogquery-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1510 b- defN 23-May-15 09:33 starcatalogquery-0.1.5.dist-info/RECORD
-17 files, 110759 bytes uncompressed, 24649 bytes compressed:  77.7%
+-rw-r--r--  2.0 unx     1068 b- defN 23-Jun-13 08:21 starcatalogquery-0.1.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12549 b- defN 23-Jun-13 08:21 starcatalogquery-0.1.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 08:21 starcatalogquery-0.1.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-13 08:21 starcatalogquery-0.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1510 b- defN 23-Jun-13 08:21 starcatalogquery-0.1.6.dist-info/RECORD
+17 files, 110423 bytes uncompressed, 24547 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: starcatalogquery/utils/starcatalog_statistic.py
 Comment: 
 
 Filename: starcatalogquery/utils/try_download.py
 Comment: 
 
-Filename: starcatalogquery-0.1.5.dist-info/LICENSE
+Filename: starcatalogquery-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: starcatalogquery-0.1.5.dist-info/METADATA
+Filename: starcatalogquery-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: starcatalogquery-0.1.5.dist-info/WHEEL
+Filename: starcatalogquery-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: starcatalogquery-0.1.5.dist-info/top_level.txt
+Filename: starcatalogquery-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: starcatalogquery-0.1.5.dist-info/RECORD
+Filename: starcatalogquery-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## starcatalogquery/classes.py

```diff
@@ -55,15 +55,15 @@
         stars_num,mag,description = starcatalog_info(sc_name)
         dict_values = dir_to,dir_size,file_num,validity,sc_name,'{:d} deg'.format(tile_size),'raw',stars_num,mag,description
         dict_keys = 'tiles_path','sc_size','tiles_num','validity','sc_name','tile_size','_mode','stars_num','mag','description'
         info = dict(zip(dict_keys, dict_values))
 
         return StarCatalogRaw(info)  
 
-    def load(_mode,sc_name,tile_size,dir_from=None,**kwargs):
+    def load(_mode,sc_name,tile_size,dir_from=None):
         """
         Load the star catalog files from the local database.
 
         Usage:
             >>> from starcatalogquery import StarCatalog
             >>> # load the raw star catalog GAIADR3
             >>> dir_from_raw = '/Volumes/TOSHIBA/starcatalog/raw/gaiadr3/res2/'
@@ -71,44 +71,33 @@
             >>>
             >>> # load the reduced star catalog GAIADR3
             >>> dir_from_reduced = '/Volumes/TOSHIBA/starcatalog/reduced/gaiadr3/res2/'
             >>> gaiadr3_reduced = StarCatalog.load('reduced','gaiadr3',2,dir_from_reduced)
             >>>
             >>> # load the simplified star catalog GAIADR3
             >>> dir_from_simplified = '/Volumes/TOSHIBA/starcatalog/simplified/gaiadr3/res2/mag8.0/epoch2023.0/'
-            >>> kwargs = {'mag_cutoff':8,'epoch':2023.0}
-            >>> gaiadr3_simplified = StarCatalog.load('simplified','gaiadr3',2,dir_from_simplified,**kwargs)
-
+            >>> gaiadr3_simplified = StarCatalog.load('simplified','gaiadr3',2,dir_from_simplified)
         Inputs:
              _mode -> [str] Types of star catalogs, including 'raw', 'reduced', 'simplified', where
                 'raw' represents the original star catalog, which contains all information about the star
                 'reduced' represents the reduced star catalog, which contains the position, proper motion, apparent magnitude, epoch of the star
                 'simplified' represents the minimalist star catalog, which only includes the position and apparent magnitude of stars at a specific epoch
             sc_name -> [str] Name of the starcatalog. Available starcatalogs include 'hygv3', 'gsc12', 'gsc242', 'gaiadr3', '2mass', 'ucac5', 'usnob', etc.
             tile_size -> [int] Size of the tile in [deg]
             dir_from -> [str,optional,default=None] The loading path of the star catalog files. If None, the path is automatically assigned to a suitable directory by default.
-            kwargs -> [dict] Keyword arguments, only used for simplified star catalog, such as {'mag_cutoff':8,'epoch':2023.0}
-
         Outputs:
             Instance of class StarCatalog
         """
         if _mode == 'raw':
             starcatalog = StarCatalogRaw.load(sc_name,tile_size,dir_from)
         elif _mode == 'reduced':
             starcatalog = StarCatalogReduced.load(sc_name,tile_size,dir_from)
         elif _mode == 'simplified':    
-            if 'mag_cutoff' in kwargs: 
-                mag_cutoff = kwargs['mag_cutoff']
-            else:     
-                raise Exception("'mag_cutoff' should be specified by a **dictionary for simplified starcatalog.")                
-            if 'epoch' in kwargs: 
-                epoch = kwargs['epoch']
-            else:    
-                raise Exception("'epoch' should be specified by a **dictionary for simplified starcatalog.")
-            starcatalog = StarCatalogSimplified.load(sc_name,tile_size,mag_cutoff,epoch,dir_from)
+        mag_cutoff,epoch = np.array(dir_from.split('mag')[1][:-1].split('/epoch'),dtype=float) 
+        starcatalog = StarCatalogSimplified.load(sc_name,tile_size,mag_cutoff,epoch,dir_from)
 
         return starcatalog 
 
     def read_h5_indices(infile):
         """
         Read in h5-formatted star catalog file, which records the center pointing of each sky area, the pixel coordinates of the stars, the triangle invariants and the asterism indices.
 
@@ -501,42 +490,42 @@
         df = df[flag]
         df['epoch'] = t_pm
         df.reset_index(drop=True,inplace=True)   
 
         info = df2info(self.sc_name,center,df,max_control_points) 
         return Stars(info)
 
-    def _search_draw(self,kwargs):
+    def _search_draw(self,search_area):
         """
         Visualize the scope of the search area and the coverage of the corresponding tiles.
 
         Usage:
             >>> from starcatalogquery import StarCatalogRaw
             >>> dir_from_raw = '/Volumes/TOSHIBA/starcatalog/raw/gaiadr3/res2/'
             >>> gaiadr3_raw = StarCatalogRaw.load('raw','gaiadr3',2,dir_from_raw)
-            >>> kwargs = {'cone':[20,30,10]}
-            >>> stars = gaiadr3_raw._search_draw(kwargs)
+            >>> cone_area = {'cone':[20,30,10]}
+            >>> stars = gaiadr3_raw._search_draw(cone_area)
 
         Inputs:
-            kwargs -> [dict] Keyword arguments, which defines the scope of the search area, such as {'cone':[20,30,10]} or {'box':[20,30,30,40]}, where
+            search_area -> [dict] The scope of the search area, such as {'cone':[20,30,10]} or {'box':[20,30,30,40]}, where
             for {'box':[ra_min,dec_min,ra_max,dec_max]}:
                 ra_min -> [float] Left border of RA in [deg].
                 dec_min -> [float] Lower border of DEC in [deg].
                 ra_max -> [float] Right border of RA in [deg].
                 dec_max -> [float] Upper border of DEC in [deg].
             for {'cone':[ra_c,dec_c,radius]}:
                 ra_c -> [float] RA, in [deg].
                 dec_c -> [float] DEC, in [deg].
                 radius -> [float] Angular radius of the cap, in [deg].  
 
         Outputs:
             An image that shows the scope of the search area and the coverage of the corresponding tiles.          
         """
         tile_size = int(self.tile_size.split()[0]) 
-        search_draw(tile_size,kwargs)       
+        search_draw(tile_size,search_area)       
 
 class StarCatalogReduced(object):
     """
     Class StarCatalogReduced
 
     Attributes:
         - tiles_path: Path of the starcatalog tile files. 
@@ -610,14 +599,16 @@
             >>> from starcatalogquery import StarCatalogReduced
             >>> # load the reduced star catalog GAIADR3
             >>> dir_from_reduced = '/Volumes/TOSHIBA/starcatalog/reduced/gaiadr3/res2/'
             >>> gaiadr3_reduced = StarCatalogReduced.load('reduced','gaiadr3',2,dir_from_reduced)
             >>> gaiadr3_simplified = gaiadr3_reduced.simplify()
 
         Inputs:
+            mag_threshold -> [float] Apparent magnitude limit of the detector  
+            t_pm -> [float] The epoch when the search was performed
             dir_simplified -> [str,optional,default=None] The path of the simplified star catalog files to store. If None, the path is automatically assigned to a suitable directory by default.
 
         Outputs:
             Instance of class StarCatalogSimplified      
         """
         info = self.info.copy()
         tile_size = int(self.tile_size.split(' ')[0])
@@ -725,43 +716,43 @@
             Instance of class Stars
         """
         width = int(self.tile_size.split()[0])
         df = search_cone_magpm(center,radius,self.tiles_path,self.sc_name,width,self._mode,mag_threshold,t_pm)
         info = df2info(self.sc_name,center,df,max_control_points) 
         return Stars(info)
 
-    def _search_draw(self,kwargs):
+    def _search_draw(self,search_area):
         """
         Visualize the scope of the search area and the coverage of the corresponding tiles.
 
         Usage:
             >>> from starcatalogquery import StarCatalogReduced
             >>> # load the reduced star catalog GAIADR3
             >>> dir_from_reduced = '/Volumes/TOSHIBA/starcatalog/reduced/gaiadr3/res2/'
             >>> gaiadr3_reduced = StarCatalogReduced.load('reduced','gaiadr3',2,dir_from_reduced)
-            >>> kwargs = {'cone':[20,30,10]}
-            >>> stars = gaiadr3_reduced._search_draw(kwargs)
+            >>> cone_area = {'cone':[20,30,10]}
+            >>> stars = gaiadr3_reduced._search_draw(cone_area)
 
         Inputs:
-            kwargs -> [dict] Keyword arguments, which defines the scope of the search area, such as {'cone':[20,30,10]} or {'box':[20,30,30,40]}, where
+            search_area -> [dict] The scope of the search area, such as {'cone':[20,30,10]} or {'box':[20,30,30,40]}, where
             for {'box':[ra_min,dec_min,ra_max,dec_max]}:
                 ra_min -> [float] Left border of RA in [deg].
                 dec_min -> [float] Lower border of DEC in [deg].
                 ra_max -> [float] Right border of RA in [deg].
                 dec_max -> [float] Upper border of DEC in [deg].
             for {'cone':[ra_c,dec_c,radius]}:
                 ra_c -> [float] RA, in [deg].
                 dec_c -> [float] DEC, in [deg].
                 radius -> [float] Angular radius of the cap, in [deg].  
 
         Outputs:
             An image that shows the scope of the search area and the coverage of the corresponding tiles.          
         """
         width = int(self.tile_size.split()[0]) 
-        search_draw(width,kwargs)   
+        search_draw(width,search_area)   
 
 class StarCatalogSimplified(object):
     """
     Class StarCatalogSimplified
 
     Attributes:
         - tiles_path: Path of the starcatalog tile files. 
@@ -878,43 +869,43 @@
             Instance of class Stars
         """
         width = int(self.tile_size.split()[0])
         df = search_cone(center,radius,self.tiles_path,self.sc_name,width,self._mode)
         info = df2info(self.sc_name,center,df,max_control_points) 
         return Stars(info)
 
-    def _search_draw(self,kwargs):
+    def _search_draw(self,search_area):
         """
         Visualize the scope of the search area and the coverage of the corresponding tiles.
 
         Usage:
             >>> from starcatalogquery import StarCatalogSimplified
             >>> # load the simplified star catalog GAIADR3
             >>> dir_from_simplified = '/Volumes/TOSHIBA/starcatalog/simplified/gaiadr3/res2/'
             >>> gaiadr3_simplified = StarCatalogReduced.load('simplified','gaiadr3',2,dir_from_simplified)
-            >>> kwargs = {'cone':[20,30,10]}
-            >>> stars = gaiadr3_simplified._search_draw(kwargs)
+            >>> cone_area = {'cone':[20,30,10]}
+            >>> stars = gaiadr3_simplified._search_draw(cone_area)
 
         Inputs:
-            kwargs -> [dict] Keyword arguments, which defines the scope of the search area, such as {'cone':[20,30,10]} or {'box':[20,30,30,40]}, where
+            search_area -> [dict] The scope of the search area, such as {'cone':[20,30,10]} or {'box':[20,30,30,40]}, where
             for {'box':[ra_min,dec_min,ra_max,dec_max]}:
                 ra_min -> [float] Left border of RA in [deg].
                 dec_min -> [float] Lower border of DEC in [deg].
                 ra_max -> [float] Right border of RA in [deg].
                 dec_max -> [float] Upper border of DEC in [deg].
             for {'cone':[ra_c,dec_c,radius]}:
                 ra_c -> [float] RA, in [deg].
                 dec_c -> [float] DEC, in [deg].
                 radius -> [float] Angular radius of the cap, in [deg].  
 
         Outputs:
             An image that shows the scope of the search area and the coverage of the corresponding tiles.          
         """
         width = int(self.tile_size.split()[0]) 
-        search_draw(width,kwargs)   
+        search_draw(width,search_area)   
 
     def h5_incices(self,fov,pixel_width,max_control_points=60):
         """
         Generate a h5-formatted star catalog file, which records the center pointing of each sky area, the pixel coordinates of the stars, the triangle invariants and the asterism indices.
 
         Usage:
             >>> from starcatalogquery import StarCatalogSimplified
@@ -1019,20 +1010,21 @@
         Inputs:
             pixel_width -> [float] Pixel width in [deg]
 
         Outputs:
             Instance of class Stars       
         """
         # Define WCS transformation and convert the celestial coordinates to pixel coordinates
-        x,y = xy_catalog(self.center,self.radec,pixel_width)
+        x,y,wcs = xy_catalog(self.center,self.radec,pixel_width)
 
         df = self.info['df']
         df['pixelx'],df['pixely'] = x,y
         xy = np.stack([x,y]).T
         self.xy = self.info['xy'] = xy
+        self.wcs = self.info['wcs'] = wcs
         return self
 
     def invariantfeatures(self):
         """
         1. Calculate the unique invariants (L2/L1,L1/L0), where L2 >= L1 >= L0 are the three sides of the triangle composed of stars.
         2. Construct the 2D Tree from the the unique invariants.
         3. Record an array of the indices of stars that correspond to each invariant.
```

## starcatalogquery/wcs.py

```diff
@@ -48,14 +48,15 @@
     Inputs:
         fp_radec -> [list or tuple of int] Fiducial point(center pointing) of the camera in form of [Ra,Dec] in [deg]
         radec -> [2d array of float] Celestial coordinates of stars in format of [[Ra0,Dec0],..,[Ran,Decn]] in [deg]
         pixel_width -> [float] Pixel width in [deg]
 
     Outputs:
         x -> [array of float] x components of the star pixel coordinates       
-        y -> [array of float] y components of the star pixel coordinates    
+        y -> [array of float] y components of the star pixel coordinates   
+        wcs -> Instance of class WCS 
     """
     wcs = wcs_trans(pixel_width,fp_radec)
     radec = SkyCoord(radec, unit='deg')
     x,y = np.array(wcs.world_to_pixel(radec))
 
-    return x,y   
+    return x,y,wcs
```

## Comparing `starcatalogquery-0.1.5.dist-info/LICENSE` & `starcatalogquery-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `starcatalogquery-0.1.5.dist-info/METADATA` & `starcatalogquery-0.1.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: starcatalogquery
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package to establish an offline star catalog query database
 Home-page: https://github.com/lcx366/STARQUERY
 Author: Chunxiao Li
 Author-email: lcx366@126.com
 License: MIT
 Keywords: StarCatalog
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scipy
 Requires-Dist: pyshtools
 Requires-Dist: astropy (>=4.3.1)
 Requires-Dist: pandas
+Requires-Dist: h5py
 Requires-Dist: colorama
 Requires-Dist: healpy
 Requires-Dist: cartopy
 Requires-Dist: wget
 
 # Welcome to the STARQUERY package
 
@@ -171,18 +171,18 @@
 ```
 
 ### Visualization
 
 Visualize the scope of the search area and the coverage of the corresponding catalog tiles.
 
 ```python
->>> kwargs_box = {'box':[5,15,35,45]} # {'box':[ra_min,dec_min,ra_max,dec_max]}
->>> kwargs_cone = {'cone':[20,30,15]} # {'cone':[ra_c,dec_c,radius]}
->>> gaiadr3_simplified._search_draw(kwargs_box)
->>> gaiadr3_simplified._search_draw(kwargs_cone)
+>>> box_area = {'box':[5,15,35,45]} # {'box':[ra_min,dec_min,ra_max,dec_max]}
+>>> cone_area = {'cone':[20,30,15]} # {'cone':[ra_c,dec_c,radius]}
+>>> gaiadr3_simplified._search_draw(box_area)
+>>> gaiadr3_simplified._search_draw(cone_area)
 >>> # ._search_draw is also available for gaiadr3_raw and gaiadr3_reduced
 ```
 
 <p align="middle">
   <img src="readme_figs/box.png" width="500" />
 </p>
 
@@ -244,20 +244,23 @@
 #### Load the simplified star catalog
 
 ```python
 >>> from starcatalogquery import StarCatalog
 >>> sc_name = 'hygv3' # Name of the star catalog
 >>> tile_size = 5 # Size of the tile in [deg]
 >>> dir_from_simplified = '/Volumes/TOSHIBA/starcatalogs/raw/hygv3/res5/mag8.0/epoch2023.0/' # Path of the starcatalog
->>> kwargs = {'mag_cutoff':8,'epoch':2023.0}
->>> hygv3_raw = StarCatalog.load('simplified',sc_name,tile_size,dir_from_simplified,**kwargs)
+>>> hygv3_raw = StarCatalog.load('simplified',sc_name,tile_size,dir_from_simplified)
 ```
 
 ## Change log
 
+- **0.1.6 — May 13, 2023**
+  
+  - Delete the kwargs in `StarCatalog.load` for loading the simplified star catalog.
+
 - **0.1.5 — May 13, 2023**
   
   - Add method `.invariantfeatures()` to class `Stars`, which calculates the triangle invariants and constructs a 2D Tree; and records the asterism indices for each triangle.
 
 - **0.1.0 — May 10,  2023**
   
   - The ***starcatalogquery*** package was released.
```

## Comparing `starcatalogquery-0.1.5.dist-info/RECORD` & `starcatalogquery-0.1.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 starcatalogquery/__init__.py,sha256=F5XhiD_gjaRsVVK_KfSD9ZkmgQnoNiJQqIMoMsceHRY,33
 starcatalogquery/catalog_check.py,sha256=r6B-MtO3bq3NVRHkyq0xnZxBvTRf8Epmn-thBD53gHo,6048
 starcatalogquery/catalog_download.py,sha256=gDFjQEtwKX56Sdwv7L53YIZKLrLy_3CtbvE3tfyxrvQ,6716
 starcatalogquery/catalog_query.py,sha256=kBY8F25jt_WiLLY_SNJWseHCx0XWVti-b7ToL17csV4,15124
-starcatalogquery/classes.py,sha256=qaM0Zuakq-sQhgibZJTmgAlcO1fsNh0woT5vfVAmZbg,51627
+starcatalogquery/classes.py,sha256=aGhea-2WLIXy0Rsme7RPiaA2HUCQqzUrO7DEI2MCZ_s,51224
 starcatalogquery/invariantfeatures.py,sha256=iJG2K3R4BcbAqkX0I-P0nQYR4Xeo2UpPaQuEqx4CP58,3078
 starcatalogquery/tiles_draw.py,sha256=zsL2lOnfOrb-fWXDSSmdGwdfYWNIL08D84Kvk8Lvc0E,5624
-starcatalogquery/wcs.py,sha256=SMhSDUNat1755eyzwY9A56DZzDBqhz2XVVMBx8SYFQw,1937
+starcatalogquery/wcs.py,sha256=gtHOyg7Y51Icc3uAfA_uX3YznXqYbhtSKwVDcO1gIcg,1978
 starcatalogquery/utils/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 starcatalogquery/utils/df2info.py,sha256=_eQENb_DxX5Q5EGxbanJuo9nQKBm-A6Tz8pEsLFinxI,612
 starcatalogquery/utils/starcatalog_statistic.py,sha256=xnyKAJFuduuXo3dKkO0B1YoeTlvu-j-BtNtgrRMvZIY,4272
 starcatalogquery/utils/try_download.py,sha256=cTfNaevU_ELwKP3R9SpYQsiGtEvoBETnsi__EdkLSVE,477
-starcatalogquery-0.1.5.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
-starcatalogquery-0.1.5.dist-info/METADATA,sha256=DoVB0R1Ke0OKd4joKqTjnjYnYMaOxUp4nSiM6XkL6bs,12523
-starcatalogquery-0.1.5.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-starcatalogquery-0.1.5.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
-starcatalogquery-0.1.5.dist-info/RECORD,,
+starcatalogquery-0.1.6.dist-info/LICENSE,sha256=1mo8gGwn9nEfzoruoWYAD1ttN40DofMYGQNef1rsytY,1068
+starcatalogquery-0.1.6.dist-info/METADATA,sha256=eTSY6DhDnFIqutVUMHg6oqOF-5pG_DmTR7gYckP0voc,12549
+starcatalogquery-0.1.6.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+starcatalogquery-0.1.6.dist-info/top_level.txt,sha256=xZmWsZTK993L9eaiWI9PM0exXZiKw-64leh_79J2M9U,17
+starcatalogquery-0.1.6.dist-info/RECORD,,
```

