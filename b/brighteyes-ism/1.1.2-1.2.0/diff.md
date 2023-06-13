# Comparing `tmp/brighteyes-ism-1.1.2.tar.gz` & `tmp/brighteyes-ism-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brighteyes-ism-1.1.2.tar", last modified: Thu May 25 16:23:15 2023, max compression
+gzip compressed data, was "brighteyes-ism-1.2.0.tar", last modified: Tue Jun 13 17:54:16 2023, max compression
```

## Comparing `brighteyes-ism-1.1.2.tar` & `brighteyes-ism-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.888029 brighteyes-ism-1.1.2/
--rw-rw-rw-   0        0        0    35823 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     4246 2023-05-25 16:23:15.888029 brighteyes-ism-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3383 2023-05-23 10:37:26.000000 brighteyes-ism-1.1.2/README.md
--rw-rw-rw-   0        0        0     1006 2023-05-25 15:29:32.000000 brighteyes-ism-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0     1658 2023-05-25 16:23:15.896037 brighteyes-ism-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0       72 2023-02-06 17:07:56.000000 brighteyes-ism-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.762390 brighteyes-ism-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.781341 brighteyes-ism-1.1.2/src/brighteyes_ism/
--rw-rw-rw-   0        0        0      123 2023-02-06 17:07:56.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.857111 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/
--rw-rw-rw-   0        0        0     7276 2023-04-21 10:40:17.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/APR_lib.py
--rw-rw-rw-   0        0        0    15991 2023-04-07 08:56:11.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/Deconv_lib.py
--rw-rw-rw-   0        0        0     9410 2023-04-07 12:04:30.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/FRC_lib.py
--rw-rw-rw-   0        0        0    11458 2023-05-18 16:44:26.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/FocusISM_lib.py
--rw-rw-rw-   0        0        0    16427 2023-05-23 17:49:33.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/Tools_lib.py
--rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.865122 brighteyes-ism-1.1.2/src/brighteyes_ism/dataio/
--rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/dataio/__init__.py
--rw-rw-rw-   0        0        0     5852 2023-04-06 15:11:23.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/dataio/mcs.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.887061 brighteyes-ism-1.1.2/src/brighteyes_ism/simulation/
--rw-rw-rw-   0        0        0    19397 2023-05-25 15:44:43.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/simulation/PSF_sim.py
--rw-rw-rw-   0        0        0     5701 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/simulation/Tubulin_sim.py
--rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.1.2/src/brighteyes_ism/simulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 16:23:15.806274 brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/
--rw-rw-rw-   0        0        0     4246 2023-05-25 16:23:15.000000 brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-05-25 16:23:15.000000 brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 16:23:15.000000 brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-05-25 16:23:15.000000 brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-25 16:23:15.000000 brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.856156 brighteyes-ism-1.2.0/
+-rw-rw-rw-   0        0        0    35823 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4246 2023-06-13 17:54:16.856156 brighteyes-ism-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3383 2023-05-23 10:37:26.000000 brighteyes-ism-1.2.0/README.md
+-rw-rw-rw-   0        0        0     1006 2023-06-09 19:13:34.000000 brighteyes-ism-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1658 2023-06-13 17:54:16.857158 brighteyes-ism-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       72 2023-02-06 17:07:56.000000 brighteyes-ism-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.833188 brighteyes-ism-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.839172 brighteyes-ism-1.2.0/src/brighteyes_ism/
+-rw-rw-rw-   0        0        0      123 2023-02-06 17:07:56.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.851141 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/
+-rw-rw-rw-   0        0        0     7231 2023-06-12 09:19:15.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/APR_lib.py
+-rw-rw-rw-   0        0        0    16108 2023-06-12 10:11:08.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/Deconv_lib.py
+-rw-rw-rw-   0        0        0     9410 2023-04-07 12:04:30.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/FRC_lib.py
+-rw-rw-rw-   0        0        0    11499 2023-05-31 13:30:30.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/FocusISM_lib.py
+-rw-rw-rw-   0        0        0    10496 2023-06-12 09:58:17.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/Graph_lib.py
+-rw-rw-rw-   0        0        0     6848 2023-06-10 15:14:36.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/Tools_lib.py
+-rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.852137 brighteyes-ism-1.2.0/src/brighteyes_ism/dataio/
+-rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/dataio/__init__.py
+-rw-rw-rw-   0        0        0     5852 2023-04-06 15:11:23.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/dataio/mcs.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.855168 brighteyes-ism-1.2.0/src/brighteyes_ism/simulation/
+-rw-rw-rw-   0        0        0    21695 2023-06-13 17:51:50.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/simulation/PSF_sim.py
+-rw-rw-rw-   0        0        0     5701 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/simulation/Tubulin_sim.py
+-rw-rw-rw-   0        0        0        0 2023-01-24 14:06:21.000000 brighteyes-ism-1.2.0/src/brighteyes_ism/simulation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:54:16.844184 brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/
+-rw-rw-rw-   0        0        0     4246 2023-06-13 17:54:16.000000 brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2023-06-13 17:54:16.000000 brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:54:16.000000 brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-06-13 17:54:16.000000 brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-13 17:54:16.000000 brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/top_level.txt
```

### Comparing `brighteyes-ism-1.1.2/LICENSE` & `brighteyes-ism-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.1.2/PKG-INFO` & `brighteyes-ism-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brighteyes-ism
-Version: 1.1.2
+Version: 1.2.0
 Summary: A toolbox for analysing and simulating ISM images
 Home-page: https://github.com/VicidominiLab/brighteyes-ism
 Author: Alessandro Zunino
 Author-email: Alessandro Zunino <alessandro.zunino@iit.it>
 Project-URL: Homepage, https://github.com/VicidominiLab/brighteyes-ism
 Project-URL: Documentation, https://brighteyes-ism.readthedocs.io
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `brighteyes-ism-1.1.2/README.md` & `brighteyes-ism-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.1.2/pyproject.toml` & `brighteyes-ism-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "scikit-image>=0.19.2", "scikit-learn", "numpy", "scipy", "matplotlib", "joblib", "poppy", 	"PyCustomFocus", "h5py", "statsmodels", "tqdm", "matplotlib-scalebar"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "brighteyes-ism"
-version = "1.1.2"
+version = "1.2.0"
 authors = [
   { name="Alessandro Zunino", email="alessandro.zunino@iit.it" },
 ]
 description = "A toolbox for analysing and simulating ISM images"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
```

### Comparing `brighteyes-ism-1.1.2/setup.cfg` & `brighteyes-ism-1.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 7269 6768 7465 7965 732d 6973   = brighteyes-is
-00000020: 6d0d 0a76 6572 7369 6f6e 203d 2031 2e31  m..version = 1.1
-00000030: 2e32 0d0a 6175 7468 6f72 203d 2041 6c65  .2..author = Ale
+00000020: 6d0d 0a76 6572 7369 6f6e 203d 2031 2e32  m..version = 1.2
+00000030: 2e30 0d0a 6175 7468 6f72 203d 2041 6c65  .0..author = Ale
 00000040: 7373 616e 6472 6f20 5a75 6e69 6e6f 0d0a  ssandro Zunino..
 00000050: 6175 7468 6f72 5f65 6d61 696c 203d 2061  author_email = a
 00000060: 6c65 7373 616e 6472 6f2e 7a75 6e69 6e6f  lessandro.zunino
 00000070: 4069 6974 2e69 740d 0a75 726c 203d 2068  @iit.it..url = h
 00000080: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 00000090: 6d2f 5669 6369 646f 6d69 6e69 4c61 622f  m/VicidominiLab/
 000000a0: 6272 6967 6874 6579 6573 2d69 736d 0d0a  brighteyes-ism..
```

### Comparing `brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/APR_lib.py` & `brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/APR_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -245,20 +245,17 @@
     result_ism_pc : np.ndarray
         Reassigned ISM dataset (Nx x Ny x Nch).
 
     '''
     
     sz = dset.shape    
     result_ism_pc = np.empty( sz )
-    
-    if mode == 'fourier':
-    
-        for i in range( sz[-1] ):
-            offset  = fourier_shift(np.fft.fftn(dset[:,:,i]), (shift_vec[i,:]))
-            result_ism_pc[:,:,i]  = np.real( np.fft.ifftn(offset) )
-        return result_ism_pc
-        
-    elif mode == 'interp':
-        
-        for i in range( sz[-1] ):
-            result_ism_pc[:,:,i]  = shift( dset[:,:,i], shift_vec[i,:] )
-        return result_ism_pc
+
+    for i in range(sz[-1]):
+        if mode == 'fourier':
+            offset = fourier_shift(np.fft.fftn(dset[:, :, i]), (shift_vec[i, :]))
+            result_ism_pc[:, :, i] = np.real( np.fft.ifftn(offset) )
+        elif mode == 'interp':
+            result_ism_pc[:, :, i] = shift( dset[:, :, i], shift_vec[i,:] )
+
+    result_ism_pc[result_ism_pc < 0] = 0
+    return result_ism_pc
```

### Comparing `brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/Deconv_lib.py` & `brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/Deconv_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from scipy.linalg import toeplitz
 from scipy.linalg import inv
 from scipy.ndimage import laplace
 from scipy.signal import convolve
+from tqdm import tqdm
 
 from . import FRC_lib as FRC
 from . import APR_lib as APR
 
 def gauss2d(X, Y, mux, muy, sigma):
     """
     2D radially symmetric Gaussian function
@@ -304,23 +305,25 @@
         bkg = np.zeros(i.shape)
     
     if pad is not None:
         h = PadDataset(h, pad)
         i = PadDataset(i, pad)
         
     N = i.shape[-1]
-    
+
     if epsilon is None:
        epsilon = np.finfo(float).eps
     
     h = h/np.sum(h) #PSF normalization
     hT = np.flip(h, axis=(0,1))
     obj = np.ones( i.shape[0:-1] ) #Initialization
     
     k = 0
+    print('Multi-image deconvolution:')
+    pbar = tqdm(total=max_iter)
     while k < max_iter:
         
         if verbose == True:
             print(k)
         
         tmp = 0        
         
@@ -334,14 +337,15 @@
             
         obj = ( obj * tmp / ( 1 + reg * obj ) ) # * s[n]
 
         if out == 'all':
             obj_all[k] = obj.copy()
             
         k += 1
+        pbar.update(1)
 
     if pad is not None:
         if out == 'last':
             obj = UnpadDataset(obj, pad)
         elif out == 'all':
             for n in range(max_iter):
                 obj_all[n] = UnpadDataset(obj_all[n], pad)
```

### Comparing `brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/FRC_lib.py` & `brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/FRC_lib.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.1.2/src/brighteyes_ism/analysis/FocusISM_lib.py` & `brighteyes-ism-1.2.0/src/brighteyes_ism/analysis/FocusISM_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,16 @@
         sigma_B_bound = 2*sigma_A
     else:
         sigma_B_bound *= sigma_A
         
     threshold = threshold
 
     if parallelize == True:
-        Result = Parallel(n_jobs = N, backend = 'threading')( delayed(pixel_fit_2)( img_reshaped[i,:], sigma_A, sigma_B_bound = sigma_B_bound, threshold = threshold) for i in range(sz[0]*sz[1]) )
+        print('Focus-ISM - parallel:')
+        Result = Parallel(n_jobs = N, backend = 'threading')( delayed(pixel_fit_2)( img_reshaped[i,:], sigma_A, sigma_B_bound = sigma_B_bound, threshold = threshold) for i in trange(sz[0]*sz[1]) )
     else:
         Result =[[]] * (sz[0] * sz[1])
         print('Focus-ISM:')
         for i in trange(sz[0] * sz[1]):
             Result[i] = pixel_fit_2(img_reshaped[i, :], sigma_A, sigma_B_bound = sigma_B_bound, threshold = threshold)
 
     # Reshape
```

### Comparing `brighteyes-ism-1.1.2/src/brighteyes_ism/dataio/mcs.py` & `brighteyes-ism-1.2.0/src/brighteyes_ism/dataio/mcs.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.1.2/src/brighteyes_ism/simulation/PSF_sim.py` & `brighteyes-ism-1.2.0/src/brighteyes_ism/simulation/PSF_sim.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,14 +62,71 @@
         
         phase += A[i] * 1j * norm_coeff * ( radial * angular ) 
         
     return  np.exp( phase )
 
 #%% functions
 
+class GridParameters:
+    """
+    It calculates a z-stack of PSFs for all the elements of the SPAD array detector.
+
+    Attributes
+    ----------
+    N : int
+        Number of detector elements in the array in each dimension (typically 5)
+    Nx : int
+        Number of pixels in each dimension in the simulation array (e.g. 1024)
+    pxpitch : float
+        Pixel pitch of the detector [nm] (real space, typically 75000)
+    pxdim : float
+        Detector element size [nm] (real space, typically 50000)
+    pxsizex : float
+        Pixel size of the simulation space [nm] (typically 1)
+    M : float
+        Total magnification of the optical system (typically 500)
+    Nz : int
+        number of axial planes (typically an odd integer)
+    """
+
+    __slots__ = ['pxsizex', 'pxsizez', 'Nx', 'Ny', 'Nz', 'pxpitch', 'pxdim', 'N', 'M']
+    def __init__(self, pxsizex=40, pxsizez=50, Nx = 100, Ny = 100, Nz = 1, pxpitch = 75e3, pxdim = 50e3, N = 5, M = 450):
+        self.pxsizex = pxsizex  # nm - lateral pixel size of the images
+        self.pxsizez = pxsizez  # nm - distance of the axial planes
+        self.Nx = Nx  # number of samples along the X and Y axis
+        self.Nz = Nz  # number of axial planes
+        self.pxpitch = pxpitch  # nm - spad array pixel pitch (real space)
+        self.pxdim = pxdim  # nm - spad pixel size (real space) 57.3e-3 for cooled spad
+        self.N = N  # number of pixels in the detector in each dimension (5x5 typically)
+        self.M = M  # overall magnification of the system
+
+    @property
+    def rangex(self):
+        return self.Nx * self.pxsizex
+
+    @property
+    def rangez(self):
+        return self.Nz * self.pxsizez
+
+    @property
+    def Nch(self):
+        return self.N**2
+
+    def spad_size(self, mode: str = 'magnified', simPar = None):
+        size = (self.pxpitch * (self.N - 1) + self.pxdim)
+        if simPar is not None:
+            return size / self.M / simPar.airy_unit
+        elif mode == 'magnified':
+            return size / self.M
+        elif mode == 'real':
+            return size
+
+    def copy(self):
+        return cp.copy(self)
+
 class simSettings:
     """
     Optical settings used to calculate the psf 
     Read more at https://pyfocus.readthedocs.io/en/latest/
 
     Attributes
     ----------
@@ -121,48 +178,58 @@
     aberration : str / list
         Returns the list of aberrations by name.
     """
     
     __slots__ = ['na', 'n', 'wl', 'h', 'gamma', 'beta', 'w0', 'I0', 'field', 'mask', 'mask_sampl',
                  'sted_sat', 'sted_pulse', 'sted_tau', 'abe_index', 'abe_ampli']
 
-    def __init__(self, na=1.4, n = 1.5, wl = 485.0, h = 2.8, gamma = 45.0, beta = 90.0,
-                 w0 = 100.0, I0 = 1, field = 'PlaneWave', mask = None,  mask_sampl = 200,
-                 sted_sat = 50, sted_pulse = 1, sted_tau = 3.5,
-                 abe_index = None, abe_ampli = None):
-        
-        self.na = na            # numerical aperture
-        self.n = n              # sample refractive index
-        self.wl = wl            # wavelength [nm]
-        self.h = h              # radius of aperture of the objective lens [mm]
-        self.w0 = w0            # radius of the incident gaussian beam [mm]
-        self.gamma = gamma      # parameter describing the light polarization (amplitude)
-        self.beta = beta        # parameter describing the light polarization (phase)
-        self.I0 = I0            # Intensity of the entrance field
-        self.field = field      # entrance field at the pupil plane
-                                #   'PlaneWave' = Flat field
-                                #   'Gaussian' = Gaussian beam with waist w0
-        self.mask = mask        # phase mask 
-                                #   None = no mask
-                                #   'VP' = vortex phase plate
-                                #   'Zernike' = zernike polynomials
-        self.mask_sampl = mask_sampl   # phase mask sampling
-        self.sted_sat = sted_sat   # STED maximum saturation factor
-        self.sted_pulse = sted_pulse   # STED pulse duration [ns]
-        self.sted_tau = sted_tau   # fluorescence lifetime [ns]
-        self.abe_index = abe_index      # aberration index (int or array)
-        self.abe_ampli = abe_ampli      # aberration amplitude in rad (float or array)
+    def __init__(self, na=1.4, n=1.5, wl=485.0, h=2.8, gamma=45.0, beta=90.0,
+                 w0=100.0, I0=1, field='PlaneWave', mask=None, mask_sampl=200,
+                 sted_sat=50, sted_pulse=1, sted_tau=3.5,
+                 abe_index=None, abe_ampli=None):
+
+        self.na = na  # numerical aperture
+        self.n = n  # sample refractive index
+        self.wl = wl  # wavelength [nm]
+        self.h = h  # radius of aperture of the objective lens [mm]
+        self.w0 = w0  # radius of the incident gaussian beam [mm]
+        self.gamma = gamma  # parameter describing the light polarization (amplitude)
+        self.beta = beta  # parameter describing the light polarization (phase)
+        self.I0 = I0  # Intensity of the entrance field
+        self.field = field  # entrance field at the pupil plane
+        #   'PlaneWave' = Flat field
+        #   'Gaussian' = Gaussian beam with waist w0
+        self.mask = mask  # phase mask
+        #   None = no mask
+        #   'VP' = vortex phase plate
+        #   'Zernike' = zernike polynomials
+        self.mask_sampl = mask_sampl  # phase mask sampling
+        self.sted_sat = sted_sat  # STED maximum saturation factor
+        self.sted_pulse = sted_pulse  # STED pulse duration [ns]
+        self.sted_tau = sted_tau  # fluorescence lifetime [ns]
+        self.abe_index = abe_index  # aberration index (int or array)
+        self.abe_ampli = abe_ampli  # aberration amplitude in rad (float or array)
         
     @property
     def f(self):    # focal length of the objective lens [mm]
         return self.h*self.n/self.na
 
     @property
     def alpha(self):    # semiangular aperture of the objective [rad]
-        return np.arcsin(self.na/self.n)   
+        return np.arcsin(self.na/self.n)
+
+    @property
+    def airy_unit(self):
+        au = 1.22 * self.wl / self.na
+        return au
+
+    @property
+    def depth_of_field(self):
+        dof = 2 * self.n * self.wl / (self.na ** 2)
+        return dof
 
     @property
     def aberration(self):
         
         if self.abe_index is None:
             return 'None'
         
@@ -305,15 +372,15 @@
         
         # Emission PSF
         
         em_PSF = singlePSF(emPar, pxsizex, Nx, z_shift = z_shift)
     
         return ex_PSF, em_PSF
 
-def Pinholes(N, Nx, pxsizex, M, pxpitch, pxdim):
+def Pinholes(gridPar):
     """
     Simulate PSFs with PyFocus
 
     Parameters
     ----------
     N : int
         Number of detector elements in the array in each dimension (typically 5)
@@ -331,36 +398,37 @@
     Returns
     -------
     p : np.array(Nx x Nx x N**2)
         array with the pinholes of each detector element
     
     """
     
-    p = np.zeros((Nx, Nx, N*N))
-    center = Nx//2
-    sizeDet = int( np.round(pxdim / M / pxsizex) )
+    p = np.zeros((gridPar.Nx, gridPar.Nx, gridPar.N**2))
+    center = gridPar.Nx//2
+    sizeDet = int( np.round(gridPar.pxdim / gridPar.M / gridPar.pxsizex) )
     if np.mod(sizeDet, 2) == 0:
         sizeDet -= 1 # let this be odd
     sizeDet = np.max((sizeDet, 1))
-    stepDet = int( np.round(pxpitch / M / pxsizex) )
-    startcoord = int(np.ceil(center - np.floor(N/2) * stepDet - 0.5 * sizeDet))
+    stepDet = int( np.round(gridPar.pxpitch / gridPar.M / gridPar.pxsizex) )
+    startcoord = int(np.ceil(center - np.floor(gridPar.N/2) * stepDet - 0.5 * sizeDet))
 
     i = 0
-    for dy in range(N):
-        for dx in range(N):
+    for dy in range(gridPar.N):
+        for dx in range(gridPar.N):
             ymin = np.max((startcoord+dy*stepDet, 0))
             ymax = np.max((startcoord+dy*stepDet+sizeDet, 0))
             xmin = np.max((startcoord+dx*stepDet, 0))
             xmax = np.max((startcoord+dx*stepDet+sizeDet, 0))
             p[ymin:ymax, xmin:xmax, i] = 1
             i += 1    
 
     return p
 
-def SPAD_PSF_2D(N, Nx, pxpitch, pxdim, pxsizex, M, exPar, emPar, rotParam = None, stedPar = None, z_shift=0, spad = None, return_entrance_field = False):
+def SPAD_PSF_2D(gridPar, exPar, emPar, rotParam = None, stedPar = None, z_shift=0, spad = None,
+                return_entrance_field = False, normalize = True):
     """
     Calculate PSFs for all pixels of the SPAD array by using FFTs
 
     Parameters
     ----------
     N : int
         Number of detector elements in the array in each dimension (typically 5)
@@ -388,14 +456,17 @@
     spad : np.array( N**2 x Nx x Nx)
         Pinholes distribution . If none it is calculated using the input parameters
     return_entrance_field : bool
         Returns the X and Y components of the field at the
         pupil plane in polar coordinates. They have to be
         converted into cartesian coordinate using the
         plot_in_cartesian function
+    normalize : bool
+        If True, all the returned PSFs are divided by the total flux.
+        Default is True.
     
     Returns
     -------
     PSF : np.array(Nx x Nx x N**2)
         array with the overall PSFs for each detector element
     detPSF : np.array(Nx x Nx x N**2)
         array with the detection PSFs for each detector element
@@ -403,31 +474,31 @@
         array with the excitation PSF
     
     """
     
     # Simulate ism psfs
     
     if return_entrance_field == True:
-        exPSF, emPSF, ex_fields, em_fields = PSFs2D(exPar, emPar, pxsizex, Nx, z_shift = z_shift, return_entrance_field = True)
+        exPSF, emPSF, ex_fields, em_fields = PSFs2D(exPar, emPar, gridPar.pxsizex, gridPar.Nx, z_shift = z_shift, return_entrance_field = True)
     else:
-        exPSF, emPSF = PSFs2D(exPar, emPar, pxsizex, Nx, z_shift = z_shift)
+        exPSF, emPSF = PSFs2D(exPar, emPar, gridPar.pxsizex, gridPar.Nx, z_shift = z_shift)
     
     if spad is None:
-        spad = Pinholes(N, Nx, pxsizex, M, pxpitch, pxdim)
+        spad = Pinholes(gridPar)
     
-    detPSF = np.empty( (Nx, Nx, N*N) )
+    detPSF = np.empty( (gridPar.Nx, gridPar.Nx, gridPar.N**2) )
 
-    for i in range(N*N):
+    for i in range(gridPar.N**2):
         detPSF[:,:,i] = sgn.convolve( emPSF, spad[:,:,i], mode ='same' )
 
     # Simulate donut
     
     if type(stedPar) == simSettings:
         stedPar.mask = 'VP'
-        donut = singlePSF(stedPar, pxsizex, Nx, z_shift = z_shift)
+        donut = singlePSF(stedPar, gridPar.pxsizex, gridPar.Nx, z_shift = z_shift)
         donut *= stedPar.sted_sat/np.max(donut)
         stedPSF = np.exp( - donut * stedPar.sted_pulse / stedPar.sted_tau )
         exPSF *= stedPSF
 
     # Rotate and mirror detPSF
 
     if rotParam is None:
@@ -435,31 +506,37 @@
     else:
         detPSFrot = detPSF.copy()
 
         theta = rotParam[1] * 180 / np.pi
         mirror = rotParam[2]
 
         if mirror == -1:
-            detPSFrot = detPSFrot.reshape(Nx, Nx, N, N)
+            detPSFrot = detPSFrot.reshape(gridPar.Nx, gridPar.Nx, gridPar.N, gridPar.N)
             detPSFrot = np.flip(detPSFrot, axis=-1)
-            detPSFrot = detPSFrot.reshape(Nx, Nx, N ** 2)
+            detPSFrot = detPSFrot.reshape(gridPar.Nx, gridPar.Nx, gridPar.N ** 2)
 
         detPSFrot = rotate(detPSFrot, theta, resize=False, center=None, order=None, mode='constant', cval=0,
                            clip=True, preserve_range=False)
 
     # Calculate total PSF
     
     PSF = np.einsum('ijk, ij -> ijk', detPSFrot, exPSF)
-    
+
+    if normalize == True:
+        PSF /= PSF.sum()
+        detPSFrot /= detPSFrot.sum()
+        exPSF /= exPSF.sum()
+
     if return_entrance_field == True:
         return PSF, detPSFrot, exPSF, ex_fields, em_fields
     else:
         return PSF, detPSFrot, exPSF
     
-def SPAD_PSF_3D(N, Nx, pxpitch, pxdim, pxsizex, M, exPar, emPar, Nz, pxsizez, rotParam = None, stedPar = None, spad = None, stack: str = 'symmetrical'):
+def SPAD_PSF_3D(gridPar, exPar, emPar, rotParam = None, stedPar = None, spad = None, stack: str = 'symmetrical',
+                normalize = True):
     """
     It calculates a z-stack of PSFs for all the elements of the SPAD array detector.
 
     Parameters
     ----------
     N : int
         Number of detector elements in the array in each dimension (typically 5)
@@ -490,70 +567,48 @@
     spad : np.array( N**2 x Nx x Nx)
         Pinholes distribution . If none it is calculated using the input parameters
     stack : str
         String that defines the direction along z of the simulation.
         If "symmetrical", the stack is generated at planes around z = 0 both on the negative and positive directions.
         Other possible entries are "positive", and "negative".
         Default: "symmetrical".
+    normalize : bool
+        If True, the returned PSFs are divided by the total flux calculated on the focal plane (z=0).
+        Default is True.
     Returns
     -------
     PSF : np.array(Nz x Nx x Nx x N**2)
         array with the overall PSFs for each detector element
     detPSF : np.array(Nz x Nx x Nx x N**2)
         array with the detection PSFs for each detector element
     exPSF : np.array(Nz x Nx x Nx)
         array with the excitation PSF
     
     """
 
     if stack == "symmetrical":
-        zeta = (np.arange(Nz) - Nz//2) * pxsizez
+        zeta = (np.arange(gridPar.Nz) - gridPar.Nz//2) * gridPar.pxsizez
     elif stack == "positive":
-        zeta = np.arange(Nz) * pxsizez
+        zeta = np.arange(gridPar.Nz) * gridPar.pxsizez
     elif stack == "negative":
-        zeta = -np.arange(Nz) * pxsizez
+        zeta = -np.arange(gridPar.Nz) * gridPar.pxsizez
 
     if spad is None:
-        spad = Pinholes(N, Nx, pxsizex, M, pxpitch, pxdim)
+        spad = Pinholes(gridPar)
     
-    PSF = np.empty( (Nz, Nx, Nx, N*N) )
-    detPSF = np.empty( (Nz, Nx, Nx, N*N) )
-    exPSF = np.empty( (Nz, Nx, Nx) )
+    PSF = np.empty( (gridPar.Nz, gridPar.Nx, gridPar.Nx, gridPar.N**2) )
+    detPSF = np.empty( (gridPar.Nz, gridPar.Nx, gridPar.Nx, gridPar.N**2) )
+    exPSF = np.empty( (gridPar.Nz, gridPar.Nx, gridPar.Nx) )
     
     for i, z in enumerate(zeta):
         print( f'Calculating the PSFs at z = {z} nm')
-        PSF[i, :, :, :], detPSF[i, :, :, :], exPSF[i, :, :] = SPAD_PSF_2D(N, Nx, pxpitch, pxdim, pxsizex, M, exPar, emPar, rotParam = rotParam, stedPar = stedPar, z_shift = z, spad = spad)
-        
-    return PSF, detPSF, exPSF
-
-def Fingerprint(dset, volumetric = False):
-    """
-    Calculate the fingerprint of an ISM dataset.
-    The last dimension has to be the spad array channel.
+        PSF[i, :, :, :], detPSF[i, :, :, :], exPSF[i, :, :] = SPAD_PSF_2D(gridPar, exPar, emPar, rotParam = rotParam,
+                                                                          stedPar = stedPar, z_shift = z, spad = spad,
+                                                                          normalize = False)
+
+    if normalize == True:
+        idx = np.argwhere(zeta == 0).item()
+        focal_flux = PSF[idx, :, :, :].sum()
+        for i, z in enumerate(zeta):
+            PSF[i, :, :, :] /= focal_flux
 
-    Parameters
-    ----------
-    dset : np.array(Nz x Nx x Nx x ... x N*N)
-        ISM dataset
-    volumetric : bool
-        if true, a fingerprint is returned for each axial plane
-    
-    Returns
-    -------
-    Fingerprint : np.array(Nz x N x N)
-        Finger print
-    
-    """
-    
-    N = int( np.sqrt(dset.shape[-1]) )
-    
-    if volumetric == True:
-        Nz = dset.shape[0]
-        f = np.empty( (Nz, N*N) )
-        axis = tuple( range(1, dset.ndim - 1) )
-        f = np.sum( dset, axis = axis )
-        f = f.reshape(Nz, N, N)
-    else:
-        axis = tuple( range(dset.ndim - 1) )
-        f = np.sum( dset, axis = axis )
-        f = f.reshape(N,N)
-    return f
+    return PSF, detPSF, exPSF
```

### Comparing `brighteyes-ism-1.1.2/src/brighteyes_ism/simulation/Tubulin_sim.py` & `brighteyes-ism-1.2.0/src/brighteyes_ism/simulation/Tubulin_sim.py`

 * *Files identical despite different names*

### Comparing `brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/PKG-INFO` & `brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brighteyes-ism
-Version: 1.1.2
+Version: 1.2.0
 Summary: A toolbox for analysing and simulating ISM images
 Home-page: https://github.com/VicidominiLab/brighteyes-ism
 Author: Alessandro Zunino
 Author-email: Alessandro Zunino <alessandro.zunino@iit.it>
 Project-URL: Homepage, https://github.com/VicidominiLab/brighteyes-ism
 Project-URL: Documentation, https://brighteyes-ism.readthedocs.io
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `brighteyes-ism-1.1.2/src/brighteyes_ism.egg-info/SOURCES.txt` & `brighteyes-ism-1.2.0/src/brighteyes_ism.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/brighteyes_ism.egg-info/dependency_links.txt
 src/brighteyes_ism.egg-info/requires.txt
 src/brighteyes_ism.egg-info/top_level.txt
 src/brighteyes_ism/analysis/APR_lib.py
 src/brighteyes_ism/analysis/Deconv_lib.py
 src/brighteyes_ism/analysis/FRC_lib.py
 src/brighteyes_ism/analysis/FocusISM_lib.py
+src/brighteyes_ism/analysis/Graph_lib.py
 src/brighteyes_ism/analysis/Tools_lib.py
 src/brighteyes_ism/analysis/__init__.py
 src/brighteyes_ism/dataio/__init__.py
 src/brighteyes_ism/dataio/mcs.py
 src/brighteyes_ism/simulation/PSF_sim.py
 src/brighteyes_ism/simulation/Tubulin_sim.py
 src/brighteyes_ism/simulation/__init__.py
```

