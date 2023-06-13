# Comparing `tmp/EzGM-1.6.6.1.tar.gz` & `tmp/EzGM-1.6.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EzGM-1.6.6.1.tar", last modified: Thu Mar  9 12:54:41 2023, max compression
+gzip compressed data, was "EzGM-1.6.6.2.tar", last modified: Tue Jun 13 08:43:19 2023, max compression
```

## Comparing `EzGM-1.6.6.1.tar` & `EzGM-1.6.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 12:54:41.785944 EzGM-1.6.6.1/
-drwxrwxrwx   0        0        0        0 2023-03-09 12:54:41.770434 EzGM-1.6.6.1/EzGM/
--rw-rw-rw-   0        0        0      105 2022-10-20 15:03:59.000000 EzGM-1.6.6.1/EzGM/__init__.py
--rw-rw-rw-   0        0        0   180434 2023-02-14 11:29:47.000000 EzGM-1.6.6.1/EzGM/selection.py
--rw-rw-rw-   0        0        0    20201 2023-02-19 11:07:04.000000 EzGM-1.6.6.1/EzGM/signal.py
--rw-rw-rw-   0        0        0    54668 2023-02-25 20:44:42.000000 EzGM-1.6.6.1/EzGM/utility.py
--rw-rw-rw-   0        0        0    22955 2022-11-17 11:50:02.000000 EzGM-1.6.6.1/EzGM/webdriverdownloader.py
-drwxrwxrwx   0        0        0        0 2023-03-09 12:54:41.785944 EzGM-1.6.6.1/EzGM.egg-info/
--rw-rw-rw-   0        0        0     6801 2023-03-09 12:54:41.000000 EzGM-1.6.6.1/EzGM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-03-09 12:54:41.000000 EzGM-1.6.6.1/EzGM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 12:54:41.000000 EzGM-1.6.6.1/EzGM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-03-09 12:54:41.000000 EzGM-1.6.6.1/EzGM.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-09 12:54:41.000000 EzGM-1.6.6.1/EzGM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2022-10-20 15:03:59.000000 EzGM-1.6.6.1/LICENSE
--rw-rw-rw-   0        0        0     6801 2023-03-09 12:54:41.785944 EzGM-1.6.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     6174 2023-03-09 12:54:15.000000 EzGM-1.6.6.1/README.md
--rw-rw-rw-   0        0        0      108 2022-10-20 15:03:59.000000 EzGM-1.6.6.1/pyproject.toml
--rw-rw-rw-   0        0        0      893 2023-03-09 12:54:41.785944 EzGM-1.6.6.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 08:43:19.911844 EzGM-1.6.6.2/
+drwxrwxrwx   0        0        0        0 2023-06-13 08:43:19.889760 EzGM-1.6.6.2/EzGM/
+-rw-rw-rw-   0        0        0      105 2022-10-20 15:03:59.000000 EzGM-1.6.6.2/EzGM/__init__.py
+-rw-rw-rw-   0        0        0   180770 2023-06-01 20:34:44.000000 EzGM-1.6.6.2/EzGM/selection.py
+-rw-rw-rw-   0        0        0    22786 2023-06-01 17:18:21.000000 EzGM-1.6.6.2/EzGM/signal.py
+-rw-rw-rw-   0        0        0    55844 2023-06-01 17:20:06.000000 EzGM-1.6.6.2/EzGM/utility.py
+-rw-rw-rw-   0        0        0    26111 2023-06-01 20:23:19.000000 EzGM-1.6.6.2/EzGM/webdriverdownloader.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:43:19.910848 EzGM-1.6.6.2/EzGM.egg-info/
+-rw-rw-rw-   0        0        0     6801 2023-06-13 08:43:19.000000 EzGM-1.6.6.2/EzGM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-06-13 08:43:19.000000 EzGM-1.6.6.2/EzGM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 08:43:19.000000 EzGM-1.6.6.2/EzGM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-06-13 08:43:19.000000 EzGM-1.6.6.2/EzGM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-13 08:43:19.000000 EzGM-1.6.6.2/EzGM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2022-10-20 15:03:59.000000 EzGM-1.6.6.2/LICENSE
+-rw-rw-rw-   0        0        0     6801 2023-06-13 08:43:19.911844 EzGM-1.6.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6174 2023-03-09 12:54:15.000000 EzGM-1.6.6.2/README.md
+-rw-rw-rw-   0        0        0      108 2022-10-20 15:03:59.000000 EzGM-1.6.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0      893 2023-06-13 08:43:19.913845 EzGM-1.6.6.2/setup.cfg
```

### Comparing `EzGM-1.6.6.1/EzGM/selection.py` & `EzGM-1.6.6.2/EzGM/selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,15 +388,15 @@
                 # H1 component
                 save_signal(os.path.join(self.outdir, gmr_file1), inp_acc1, self.rec_scale[i], dts[i])
                 h1s.write(gmr_file1 + '\n')
 
             # Time steps
             np.savetxt(os.path.join(self.outdir, 'GMR_dts.txt'), dts, fmt='%.5f')
             # Scale factors
-            np.savetxt(os.path.join(self.outdir, 'GMR_sf_used'), np.array([self.rec_scale]).T, fmt='%1.5f')
+            np.savetxt(os.path.join(self.outdir, 'GMR_sf_used.txt'), np.array([self.rec_scale]).T, fmt='%1.5f')
             # Close the files
             h1s.close()
             if self.selection == 2:
                 h2s.close()
 
         if obj == 1:
             # save some info as pickle obj
@@ -455,14 +455,19 @@
         plt.rc('font', size=SMALL_SIZE)  # controls default text sizes
         plt.rc('axes', titlesize=SMALL_SIZE)  # fontsize of the axes title
         plt.rc('axes', labelsize=BIG_SIZE)  # fontsize of the x and y labels
         plt.rc('xtick', labelsize=SMALL_SIZE)  # fontsize of the tick labels
         plt.rc('ytick', labelsize=SMALL_SIZE)  # fontsize of the tick labels
         plt.rc('legend', fontsize=MEDIUM_SIZE)  # legend fontsize
         plt.rc('figure', titlesize=BIGGER_SIZE)  # fontsize of the figure title
+        plt.rc('font', **{'family': 'serif', 'serif': ['Times New Roman']})
+        plt.rcParams['mathtext.it']= 'Times New Roman:italic'
+        plt.rcParams['mathtext.cal']= 'Times New Roman:italic'
+        plt.rcParams['mathtext.default'] = 'regular'
+        plt.rcParams["mathtext.fontset"] ='custom'
         plt.ioff()
 
         if type(self).__name__ == 'conditional_spectrum':
 
             # xticks and yticks to use for plotting
             xticks = [self.T[0]]
             for x in [0.01, 0.1, 0.2, 0.5, 1, 2, 4, 7, 10]:
@@ -904,15 +909,15 @@
                     options.set_preference('browser.download.useDownloadDir', True)
                     options.set_preference('browser.helperApps.neverAsk.saveToDisk', 'application/zip')
                     driver = webdriver.Firefox(executable_path=driver_path[1], options=options)
 
                 # Running on personal computer (PC) using chrome
                 elif browser == 'chrome':
                     gdd = ChromeDriverDownloader()
-                    driver_path = gdd.download_and_install()
+                    driver_path = gdd.download_and_install(version = 'compatible')
                     ChromeOptions = webdriver.ChromeOptions()
                     prefs = {"download.default_directory": download_dir}
                     ChromeOptions.add_experimental_option("prefs", prefs)
                     ChromeOptions.headless = True
                     driver = webdriver.Chrome(executable_path=driver_path[1], options=ChromeOptions)
 
                 print('Webdriver is obtained successfully.')
```

### Comparing `EzGM-1.6.6.1/EzGM/signal.py` & `EzGM-1.6.6.2/EzGM/signal.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Signal processing toolbox
 """
 
 # Import python libraries
 import numpy as np
 import numpy.matlib
-from scipy.signal import butter, lfilter, windows
-from scipy.integrate import cumtrapz
+from scipy.signal import butter, windows, find_peaks, filtfilt
+from scipy.integrate import cumtrapz, trapz
 from scipy.fft import fft, fftfreq, fftshift
 
 
 def baseline_correction(values, dt, polynomial_type):
     """
     Details
     -------
@@ -23,24 +23,24 @@
     References
     ----------
     Kramer, Steven L. 1996. Geotechnical Earthquake Engineering. Prentice Hall.
         
     Parameters
     ----------
     values: numpy.array
-        signal values.
+        Input signal values.
     dt: float          
-        sampling interval.
+        Sampling interval.
     polynomial_type: str
-        type of baseline correction 'Constant', 'Linear', 'Quadratic', 'Cubic'.
+        Type of baseline correction 'Constant', 'Linear', 'Quadratic', 'Cubic'.
         
     Returns
     -------
     values_corrected: numpy.array
-        corrected values
+        Corrected signal values
     """
 
     if polynomial_type == 'Constant':
         n = 0
     elif polynomial_type == 'Linear':
         n = 1
     elif polynomial_type == 'Quadratic':
@@ -52,63 +52,67 @@
     P = np.polyfit(t, values, n)  # Best fit line of values
     po_va = np.polyval(P, t)  # Matrix of best fit line
     values_corrected = values - po_va  # Baseline corrected values
 
     return values_corrected
 
 
-def butterworth_filter(values, dt, cut_off=25, filter_order=4, filter_type='lowpass', alpha_window=0.05):
+def butterworth_filter(values, dt, cut_off=(0.1, 25), filter_order=4, filter_type='bandpass', alpha_window=0.0):
     """
     Details
     -------
-    This function performs infinite impulse response (IIR) filtering.
+    This function performs acausal or two-pass (forward and reverse) infinite impulse response (IIR) filtering.
+    The acausal filter is preferable to a causal filter (one pass) as it does not cause phase shift, in other words it is a zero-phase filter.
     It uses butterworth digital and analog filter design.
-    Before performing the filtering, it applies tukey window on the signal, and adds zero pads with signal length
-    to the start and end.
     
     References
     ----------
-    Kramer, Steven L. 1996. Geotechnical Earthquake Engineering, Prentice Hall.
-        
+    Boore, D. M., and S. Akkar (2003). Effect of causal and acausal filters on
+    elastic and inelastic response spectra, Earthquake Eng. Struct. Dyn. 32, 1729–1748.
+    Boore, D. M. (2005). On Pads and Filters: Processing Strong-Motion Data. 
+    Bulletin of the Seismological Society of America, 95(2), 745–750. 
+    doi: 10.1785/0120040160
+
     Parameters
     ----------
     values: numpy.array
         Input signal.
     dt: float
-        time-step.
-    cut_off: float, tuple, list, optional (The default is 25)
+        Sampling interval.
+    cut_off: float, tuple, list, numpy.array, optional (The default is (0.1, 25)
         Cut off frequencies for the filter (Hz).
         For lowpass and highpass filters this parameters is a float e.g. 25 or 0.1
         For bandpass or bandstop filters this parameter is a tuple or list e.g. (0.1, 25)
     filter_type: str, optional (The default is 'lowpass')
         The type of filter {'lowpass', 'highpass', 'bandpass', 'bandstop'}.
     filter_order: int, optional (The default is 4)
         Order of the Butterworth filter.
-    alpha_window: float, optional (The default is 0.05)
+    alpha_window: float, optional (The default is 0.0)
         Shape parameter of the Tukey window
 
     Returns
     -------
     values_filtered: numpy.array
-        Filtered signal.
+        Filtered signal values.
     """
 
     if isinstance(cut_off, list) or isinstance(cut_off, tuple):
         cut_off = np.array(cut_off)
-    L = len(values)  # Signal length
+
     sampling_rate = 1.0 / dt  # Sampling rate
     nyq_freq = sampling_rate * 0.5  # Nyquist frequency
-    w = windows.tukey(L, alpha_window)  # This is the window
-    values_filtered = w * values  # Apply the tapered cosine window
-    values_filtered = np.append(np.append(np.zeros(L), values_filtered), np.zeros(L))  # Add zero pads to start and end
     wn = cut_off / nyq_freq  # The critical frequency or frequencies. For lowpass and highpass filters,
+    Lpad = round(len(values) /2)  # Half of signal length
+    w = windows.tukey(len(values), alpha_window)  # This is the window
+    values = w * values  # Apply the tapered cosine window
+    values = np.append(np.append(np.zeros(Lpad), values), np.zeros(Lpad))  # Add zero pads to start and end
     # Wn is a scalar; for bandpass and bandstop filters, Wn is a length-2 sequence.
     b, a = butter(filter_order, wn, filter_type)  # Numerator (b) and denominator (a) polynomials of the IIR filter.
-    values_filtered = lfilter(b, a, values_filtered)  # Filter data along one-dimension with an IIR or FIR filter.
-    values_filtered = values_filtered[L:2 * L]  # removing extra zeros
+    values = filtfilt(b, a, values)  # Filtering data with an IIR or FIR filter.
+    values_filtered = values[Lpad: -Lpad]  # removing extra zeros
 
     return values_filtered
 
 
 def sdof_ltha(Ag, dt, T, xi, m=1):
     """
     Details
@@ -255,17 +259,17 @@
         PSv: numpy.array
             Elastic pseudo-velocity response spectrum [m/s].
         Sd: numpy.array
             Elastic relative displacement response spectrum [m].
         Sv: numpy.array
             Elastic relative velocity response spectrum [m/s].
         Sa_r: numpy.array
-            Elastic relative accleration response spectrum [m/s2].
+            Elastic relative acceleration response spectrum [m/s2].
         Sa_a: numpy.array
-            Elastic absolute accleration response spectrum [m/s2].
+            Elastic absolute acceleration response spectrum [m/s2].
         Ei_r: numpy.array
             Relative input energy spectrum for elastic system [N.m].
         Ei_a: numpy.array
             Absolute input energy spectrum for elastic system [N.m].
         Periods: numpy.array 
             Periods where spectral values are calculated [sec].
         FAS: numpy.array 
@@ -293,15 +297,15 @@
             Significant duration between 5% and 75% of energy release (from Aint).
         t_5_95: list    
             Significant duration time vector between 5% and 95% of energy release (from Aint).
         D_5_95: float
             Significant duration between 5% and 95% of energy release (from Aint).
         t_bracketed: list 
             Bracketed duration time vector (acc>0.05g).
-            Not applicable, in case of low intensity records, thus, equal to '-1.
+            Not applicable, in case of low intensity records, thus, equal to -1.
         D_bracketed: float
             Bracketed duration (acc>0.05g)
         t_uniform: list 
             Uniform duration time vector (acc>0.05g)
             Not applicable, in case of low intensity records, thus, equal to -1.
         D_uniform: float 
             Uniform duration (acc>0.05g)
@@ -317,23 +321,28 @@
             Root mean square root of displacement [m].
         Ic: float
             Characteristic intensity.
             End time might which is used herein, is not always a good choice.
         ASI: float   
             Acceleration spectrum intensity [m/s].
             Requires T to be defined between (0.1-0.5 sec), otherwise not applicable, and equal to -1.
-        MASI: float [m]
-            Modified acceleration spectrum intensity.
+        MASI: float 
+            Modified acceleration spectrum intensity [m].
             Requires T to be defined between (0.1-2.5 sec), otherwise not applicable, and equal to -1.
-        VSI: float [m]
-            Velocity spectrum intensity.
+        VSI: float
+            Velocity spectrum intensity [m].
+            Requires T to be defined between (0.1-2.5 sec), otherwise not applicable, and equal to -1.
+        VSI: float
+            Velocity spectrum intensity [m].
             Requires T to be defined between (0.1-2.5 sec), otherwise not applicable, and equal to -1.
     """
     # TODO: there are bunch of other IMs which can be computed. Add them here.
 
+    g = 9.81
+
     if isinstance(T, (int, float)):
         T = np.array([T])
     if isinstance(T, list):
         T = np.array(T)
     elif isinstance(T, numpy.ndarray):
         T = T
 
@@ -343,15 +352,15 @@
 
     # GET SPECTRAL VALUES
     # Get the length of acceleration history array
     n1 = max(Ag.shape)
     # Get the length of period array
     n2 = max(T.shape)
     # Create the time array
-    t = np.linspace(0, (n1 - 1) * dt, n1)
+    t = dt * np.arange(0, n1, 1)
     # Get ground velocity and displacement through integration
     Vg = cumtrapz(Ag, t, initial=0)
     Dg = cumtrapz(Vg, t, initial=0)
     # Mass (kg)
     m = 1
     # Carry out linear time history analyses for SDOF system
     u, v, ac, ac_tot = sdof_ltha(Ag, dt, T, xi, m)
@@ -369,15 +378,15 @@
 
     # GET PEAK GROUND ACCELERATION, VELOCITY AND DISPLACEMENT
     param['PGA'] = np.max(np.abs(Ag))
     param['PGV'] = np.max(np.abs(Vg))
     param['PGD'] = np.max(np.abs(Dg))
 
     # GET ARIAS INTENSITY
-    Aint = np.cumsum(Ag ** 2) * np.pi * dt / (2 * 9.81)
+    Aint = np.cumsum(Ag ** 2) * np.pi * dt / (2 * g)
     param['Arias'] = Aint[-1]
     temp = np.zeros((len(Aint), 2))
     temp[:, 0] = t
     temp[:, 1] = Aint
     param['Aint'] = temp
 
     # GET HOUSNER INTENSITY
@@ -402,28 +411,28 @@
     t1 = round(timed[0], 3)
     t2 = round(timed[-1], 3)
     param['t_5_95'] = [t1, t2]
     param['D_5_95'] = round(t2 - t1, 3)
 
     # BRACKETED DURATION (0.05g)
     try:
-        mask = np.abs(Ag) >= 0.05 * 9.81
+        mask = np.abs(Ag) >= 0.05 * g
         # mask = np.abs(Ag) >= 0.05 * np.max(np.abs(Ag))
         indices = np.where(mask)[0]
         t1 = round(t[indices[0]], 3)
         t2 = round(t[indices[-1]], 3)
         param['t_bracketed'] = [t1, t2]
         param['D_bracketed'] = round(t2 - t1, 3)
     except:  # in case of ground motions with low intensities
         param['t_bracketed'] = -1
         param['D_bracketed'] = 0
 
     # UNIFORM DURATION (0.05g)
     try:
-        mask = np.abs(Ag) >= 0.05 * 9.81
+        mask = np.abs(Ag) >= 0.05 * g
         # mask = np.abs(Ag) >= 0.05 * np.max(np.abs(Ag))
         indices = np.where(mask)[0]
         t_treshold = t[indices]
         param['t_uniform'] = [t_treshold]
         temp = np.round(np.diff(t_treshold), 8)
         param['D_uniform'] = round(np.sum(temp[temp == dt]), 3)
     except:  # in case of ground motions with low intensities
@@ -496,37 +505,29 @@
     References
     ---------- 
     Boore, D. M. (2006). Orientation-Independent Measures of Ground Motion. 
     Bulletin of the Seismological Society of America, 96(4A), 1502–1511.
     Boore, D. M. (2010). Orientation-Independent, Nongeometric-Mean Measures 
     of Seismic Intensity from Two Horizontal Components of Motion. 
     Bulletin of the Seismological Society of America, 100(4), 1830–1835.
-    
-    Notes
-    -----
-    * Linear Acceleration Method: Gamma = 1/2, Beta = 1/6
-    * Average Acceleration Method: Gamma = 1/2, Beta = 1/4
-    * Average acceleration method is unconditionally stable,
-      whereas linear acceleration method is stable only if dt/Tn <= 0.55
-      Linear acceleration method is preferable due to its accuracy.
         
     Parameters
     ----------
-    Ag1 : numpy.array    
-        Acceleration values of 1st horizontal ground motion component.
-    Ag2 : numpy.array    
-        Acceleration values of 2nd horizontal ground motion component.
-    dt: float
-        Time step [sec].
-    T:  float, numpy.array
-        Considered period array e.g. 0 sec, 0.1 sec ... 4 sec.
-    xi: float
-        Damping ratio, e.g. 0.05 for 5%.
-    xx: int, list
-        Percentile to calculate, e.g. 50 for RotD50.
+    Ag1: numpy.array    
+         Acceleration values of 1st horizontal ground motion component.
+    Ag2: numpy.array    
+         Acceleration values of 2nd horizontal ground motion component.
+    dt:  float
+         Time step [sec].
+    T:   float, numpy.array
+         Considered period array e.g. 0 sec, 0.1 sec ... 4 sec.
+    xi:  float
+         Damping ratio, e.g. 0.05 for 5%.
+    xx:  int, list
+         Percentile to calculate, e.g. 50 for RotD50.
         
     Returns
     -------
     Sa_RotDxx: numpy.array 
         RotDxx Spectra.
     """
 
@@ -567,7 +568,89 @@
     if isinstance(xx, list):
         Sa_RotDxx = [np.percentile(Rot_Acc, value, axis=0) for value in xx]
     else:
         Sa_RotDxx = np.percentile(Rot_Acc, xx, axis=0)
     Periods = T
 
     return Periods, Sa_RotDxx
+
+def get_fiv3(Ag, dt, T, alpha = 0.7, beta = 0.85):
+    """
+    Details
+    -------
+    This function computes the filtered incremental velocity for a ground motion
+
+    References
+    ----------
+    Dávalos H, Miranda E. Filtered incremental velocity: A novel approach in intensity measures for seismic collapse estimation. 
+    Earthquake Engineering & Structural Dynamics 2019; 48(12): 1384-1405. DOI: 10.1002/eqe.3205.
+
+    Parameters
+    ----------
+    Ag: numpy.array    
+        Acceleration values.
+    dt: float
+        Time step [sec]
+    T:  float, numpy.array.
+        Considered period array e.g. 0 sec, 0.1 sec ... 4 sec.
+    alpha : float
+        Period factor, by default 0.7
+    beta : float
+        Cut-off frequency factor, by default 0.85
+
+    Returns
+    ----------
+    fiv3: numpy.array 
+        filtered incremental velocity, FIV3 as per Eq. (3) of Davalos and Miranda (2019)
+    """
+    
+    if isinstance(T, (int, float)):
+        T = np.array([T])
+    if isinstance(T, list):
+        T = np.array(T)
+    elif isinstance(T, numpy.ndarray):
+        T = T
+
+    T = T[T != 0]  # do not use T = zero for response spectrum calculations
+
+    # Time series of the signal
+    t = dt * np.arange(0, len(Ag), 1)
+
+    # FIV3 array
+    fiv3 = []
+
+    # apply a 2nd order Butterworth low pass filter to the ground motion
+    for tn in T:
+        wn = beta / tn / (0.5 / dt)
+        b, a = butter(2, wn, 'lowpass')
+        ugf = filtfilt(b, a, Ag)
+
+        # filtered incremental velocity (FIV)
+        ugf_pc = np.zeros(
+            (np.sum(t < t[-1] - alpha * tn), int(np.floor(alpha * tn / dt))))
+        for i in range(int(np.floor(alpha * tn / dt))):
+            ugf_pc[:, i] = ugf[np.where(t < t[-1] - alpha * tn)[0] + i]
+
+        fiv = dt * trapz(ugf_pc, axis=1)
+
+        # Find the peaks and troughs of the FIV array
+        pks_ind, _ = find_peaks(fiv)
+        trs_ind, _ = find_peaks(-fiv)
+
+        # Sort the values
+        pks_srt = np.sort(fiv[pks_ind])
+        trs_srt = np.sort(fiv[trs_ind])
+
+        # Get the peaks
+        pks = pks_srt[-3:]
+        trs = trs_srt[0:3]
+
+        # Compute the FIV3
+        fiv3_tmp = np.max([np.sum(pks), np.sum(trs)])
+
+        # Append the computed FIV3
+        fiv3.append(fiv3_tmp)
+    
+    # Convert list to an array
+    fiv3 = np.array(fiv3)
+
+    return fiv3
```

### Comparing `EzGM-1.6.6.1/EzGM/utility.py` & `EzGM-1.6.6.2/EzGM/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,20 @@
         flag to show figure (1 or 0)
 
     Returns
     -------
     None.
     """
 
+    plt.rc('font', **{'family': 'serif', 'serif': ['Times New Roman']})
+    plt.rcParams['mathtext.it']= 'Times New Roman:italic'
+    plt.rcParams['mathtext.cal']= 'Times New Roman:italic'
+    plt.rcParams['mathtext.default'] = 'regular'
+    plt.rcParams["mathtext.fontset"] ='custom'
+
     # Initialise some lists
     lat = []
     lon = []
     im = []
     iml_data = []
     poe_data = []
     id_no = []
@@ -81,15 +87,15 @@
 
             # Get the column headers (but they have a 'poe-' string in them to strip out)
             iml = list(df.columns.values)[3:]  # List of headers
             iml = [float(i[4:]) for i in iml]  # Strip out the actual IM values
             f = open(''.join([path_hazard_results, '/', file]), "r")
             temp1 = f.readline().split(',')
             temp2 = list(filter(None, temp1))
-            inv_t = float(temp2[5].replace(" investigation_time=", ""))
+            inv_t = float(list(filter(lambda x: 'investigation_time=' in x, temp2))[0].replace(" investigation_time=", ""))
             f.close()
 
             # For each of the sites investigated
             for site in np.arange(len(df)):
 
                 # Append each site's info to the output array
                 lat.append([df.lat[site]][0])
@@ -174,30 +180,36 @@
         flag to show figure (1 or 0)
 
     Returns
     -------
     None.
     """
 
+    plt.rc('font', **{'family': 'serif', 'serif': ['Times New Roman']})
+    plt.rcParams['mathtext.it']= 'Times New Roman:italic'
+    plt.rcParams['mathtext.cal']= 'Times New Roman:italic'
+    plt.rcParams['mathtext.default'] = 'regular'
+    plt.rcParams["mathtext.fontset"] ='custom'
+
     # lets add the plotting options to make everything clearer
     cmap = cm.get_cmap('jet')  # Get desired colormap
 
     for file in os.listdir(path_disagg_results):
         if file.startswith(filename) and 'Mag_Dist_Eps' not in file:
             # Load the dataframe
             df = pd.read_csv(''.join([path_disagg_results, '/', file]), skiprows=1)
             poes = np.unique(df['poe']).tolist()
             poes.sort(reverse=True)
             # Get some salient values
             f = open(''.join([path_disagg_results, '/', file]), "r")
             ff = f.readline().split(',')
-            lon = float(ff[-2].replace(" lon=", ""))
-            lat = float(ff[-1].replace(" lat=", "").replace("\"\n", ""))
+            lon = float(list(filter(lambda x: 'lon=' in x, ff))[0].replace(" lon=", ""))
+            lat = float(list(filter(lambda x: 'lat=' in x, ff))[0].replace(" lat=", "").replace("\"\n", ""))
+            inv_t = float(list(filter(lambda x: 'investigation_time=' in x, ff))[0].replace(" investigation_time=", ""))
             ims = np.unique(df['imt'])
-            inv_t = float(ff[7].replace(" investigation_time=", ""))
             for imt in ims:
                 M, R = [], []
                 hz_cont = []
                 Tr = []
                 modeLst, meanLst = [], []
                 for poe in poes:
                     Tr.append(round(-inv_t / np.log(1 - poe)))
@@ -316,14 +328,20 @@
         flag to show figure (1 or 0)
 
     Returns
     -------
     None.
     """
 
+    plt.rc('font', **{'family': 'serif', 'serif': ['Times New Roman']})
+    plt.rcParams['mathtext.it']= 'Times New Roman:italic'
+    plt.rcParams['mathtext.cal']= 'Times New Roman:italic'
+    plt.rcParams['mathtext.default'] = 'regular'
+    plt.rcParams["mathtext.fontset"] ='custom'
+
     # lets add the plotting options to make everything clearer
     cmap = cm.get_cmap('jet')  # Get desired colormap
 
     mags = []
     dists = []
 
     for file in os.listdir(path_disagg_results):
@@ -331,18 +349,18 @@
             # Load the dataframe
             df = pd.read_csv(''.join([path_disagg_results, '/', file]), skiprows=1)
             poes = np.unique(df['poe']).tolist()
             poes.sort(reverse=True)
             # Get some salient values
             f = open(''.join([path_disagg_results, '/', file]), "r")
             ff = f.readline().split(',')
-            lon = float(ff[-2].replace(" lon=", ""))
-            lat = float(ff[-1].replace(" lat=", "").replace("\"\n", ""))
+            lon = float(list(filter(lambda x: 'lon=' in x, ff))[0].replace(" lon=", ""))
+            lat = float(list(filter(lambda x: 'lat=' in x, ff))[0].replace(" lat=", "").replace("\"\n", ""))
+            inv_t = float(list(filter(lambda x: 'investigation_time=' in x, ff))[0].replace(" investigation_time=", ""))
             ims = np.unique(df['imt'])
-            inv_t = float(ff[8].replace(" investigation_time=", ""))
             for imt in ims:
                 modeLst, meanLst = [], []
                 Tr = []
                 hz_cont = []
                 M, R, eps = [], [], []
                 for poe in poes:
                     Tr.append(round(-inv_t / np.log(1 - poe)))
```

### Comparing `EzGM-1.6.6.1/EzGM/webdriverdownloader.py` & `EzGM-1.6.6.2/EzGM/webdriverdownloader.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Modified by Volkan Ozsarac on 21/04/2022
 """
 
 # Import python libraries
 import abc
 import logging
 import os
+import re
 from pathlib import Path
 import platform
 import shutil
 import stat
 import tarfile
 from urllib.parse import urlparse, urlsplit
 import zipfile
@@ -350,25 +351,38 @@
 
 
 class ChromeDriverDownloader(WebDriverDownloaderBase):
     """Class for downloading the Google Chrome WebDriver.
     """
 
     chrome_driver_base_url = 'https://www.googleapis.com/storage/v1/b/chromedriver'
+    chrome_driver_base_url2 = 'https://chromedriver.storage.googleapis.com/LATEST_RELEASE_'
 
     def _get_latest_version_number(self):
         resp = requests.get(self.chrome_driver_base_url + '/o/LATEST_RELEASE')
         if resp.status_code != 200:
             error_message = "Error, unable to get version number for latest release, got code: {0}".format(
                 resp.status_code)
             logger.error(error_message)
             raise RuntimeError(error_message)
         latest_release = requests.get(resp.json()['mediaLink'])
         return latest_release.text
 
+    def _get_chrome_compatible_version_number(self):
+        version = get_chrome_version()
+        version = '.'.join(version.split('.')[:-1])
+        resp = requests.get(self.chrome_driver_base_url2 + version)
+        if resp.status_code != 200:
+            error_message = "Error, unable to get version number for the chrome compatible release, got code: {0}".format(
+                resp.status_code)
+            logger.error(error_message)
+            raise RuntimeError(error_message)
+
+        return resp.text       
+
     def get_driver_filename(self, os_name=None):
         """
         Method for getting the filename of the web driver binary.
 
         :param os_name: Name of the OS to download the web driver binary for, as a str.  If not specified, we will use
                         platform.system() to get the OS.
         :returns: The filename of the web driver binary.
@@ -380,15 +394,15 @@
         else:
             return "chromedriver"
 
     def get_download_path(self, version="latest"):
         if version == "latest":
             ver = self._get_latest_version_number()
         else:
-            ver = version
+            ver = self._get_chrome_compatible_version_number()
         return os.path.join(self.download_root, "chrome", ver)
 
     def get_download_url(self, version="latest", os_name=None, bitness=None):
         """
         Method for getting the download URL for the Google Chome driver binary.
 
         :param version: String representing the version of the web driver binary to download.  For example, "2.39".
@@ -398,14 +412,16 @@
                         platform.system() to get the OS.
         :param bitness: Bitness of the web driver binary to download, as a str e.g. "32", "64".  If not specified, we
                         will try to guess the bitness by using util.get_architecture_bitness().
         :returns: The download URL for the Google Chrome driver binary.
         """
         if version == "latest":
             version = self._get_latest_version_number()
+        elif version == 'compatible':
+            version = self._get_chrome_compatible_version_number()
 
         if os_name is None:
             os_name = platform.system()
             if os_name == "Darwin":
                 os_name = "mac"
             elif os_name == "Windows":
                 os_name = "win"
@@ -437,7 +453,72 @@
 
      https://docs.python.org/3/library/platform.html#cross-platform
 
     :return: The bitness of the underlying architecture, as a str i.e. "32" or "64"
     """
     # TODO: Try using py-cpuinfo https://pypi.org/project/py-cpuinfo/
     return "64" if sys.maxsize > 2 ** 32 else "32"
+
+
+def extract_version_registry(output):
+    try:
+        google_version = ''
+        for letter in output[output.rindex('DisplayVersion    REG_SZ') + 24:]:
+            if letter != '\n':
+                google_version += letter
+            else:
+                break
+        return(google_version.strip())
+    except TypeError:
+        return
+
+def extract_version_folder():
+    # Check if the Chrome folder exists in the x32 or x64 Program Files folders.
+    for i in range(2):
+        path = 'C:\\Program Files' + (' (x86)' if i else '') +'\\Google\\Chrome\\Application'
+        if os.path.isdir(path):
+            paths = [f.path for f in os.scandir(path) if f.is_dir()]
+            for path in paths:
+                filename = os.path.basename(path)
+                pattern = '\d+\.\d+\.\d+\.\d+'
+                match = re.search(pattern, filename)
+                if match and match.group():
+                    # Found a Chrome version.
+                    return match.group(0)
+
+    return None
+
+def get_chrome_version():
+    #
+    # Programmatically detect the version of the Chrome web browser installed on the PC.
+    # Compatible with Windows, Mac, Linux.
+    # Written in Python.
+    # Uses native OS detection. Does not require Selenium nor the Chrome web driver.
+    #
+    version = None
+    install_path = None
+
+    try:
+        os_name = sys.platform.lower()
+        if os_name == "linux" or os_name == "linux2":
+            # linux
+            install_path = "/usr/bin/google-chrome"
+        elif os_name == "darwin":
+            # OS X
+            install_path = "/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome"
+        elif os_name == "win32":
+            # Windows...
+            try:
+                # Try registry key.
+                stream = os.popen('reg query "HKLM\\SOFTWARE\\Wow6432Node\\Microsoft\\Windows\\CurrentVersion\\Uninstall\\Google Chrome"')
+                output = stream.read()
+                version = extract_version_registry(output)
+            except Exception as ex:
+                # Try folder path.
+                version = extract_version_folder()
+    except Exception as ex:
+        print(ex)
+
+    version = os.popen(f"{install_path} --version").read().strip('Google Chrome ').strip() if install_path else version
+
+    return version
+
```

### Comparing `EzGM-1.6.6.1/EzGM.egg-info/PKG-INFO` & `EzGM-1.6.6.2/EzGM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EzGM
-Version: 1.6.6.1
+Version: 1.6.6.2
 Summary: Toolbox for ground motion record selection and processing
 Home-page: https://github.com/volkanozsarac/EzGM
 Author: Volkan Ozsarac
 Author-email: volkan.ozsarac@iusspavia.it
 Project-URL: Bug Tracker, https://github.com/volkanozsarac/EzGM/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `EzGM-1.6.6.1/LICENSE` & `EzGM-1.6.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `EzGM-1.6.6.1/PKG-INFO` & `EzGM-1.6.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EzGM
-Version: 1.6.6.1
+Version: 1.6.6.2
 Summary: Toolbox for ground motion record selection and processing
 Home-page: https://github.com/volkanozsarac/EzGM
 Author: Volkan Ozsarac
 Author-email: volkan.ozsarac@iusspavia.it
 Project-URL: Bug Tracker, https://github.com/volkanozsarac/EzGM/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `EzGM-1.6.6.1/README.md` & `EzGM-1.6.6.2/README.md`

 * *Files identical despite different names*

### Comparing `EzGM-1.6.6.1/setup.cfg` & `EzGM-1.6.6.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2045 7a47 4d0d 0a76 6572 7369 6f6e   = EzGM..version
-00000020: 203d 2031 2e36 2e36 2e31 0d0a 6175 7468   = 1.6.6.1..auth
+00000020: 203d 2031 2e36 2e36 2e32 0d0a 6175 7468   = 1.6.6.2..auth
 00000030: 6f72 203d 2056 6f6c 6b61 6e20 4f7a 7361  or = Volkan Ozsa
 00000040: 7261 630d 0a61 7574 686f 725f 656d 6169  rac..author_emai
 00000050: 6c20 3d20 766f 6c6b 616e 2e6f 7a73 6172  l = volkan.ozsar
 00000060: 6163 4069 7573 7370 6176 6961 2e69 740d  ac@iusspavia.it.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2054  .description = T
 00000080: 6f6f 6c62 6f78 2066 6f72 2067 726f 756e  oolbox for groun
 00000090: 6420 6d6f 7469 6f6e 2072 6563 6f72 6420  d motion record
```

