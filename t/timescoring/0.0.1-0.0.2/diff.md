# Comparing `tmp/timescoring-0.0.1.tar.gz` & `tmp/timescoring-0.0.2.tar.gz`

## Comparing `timescoring-0.0.1.tar` & `timescoring-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 timescoring-0.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timescoring-0.0.1/src/timescoring/__init__.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 timescoring-0.0.1/src/timescoring/annotations.py
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 timescoring-0.0.1/src/timescoring/scoring.py
--rw-r--r--   0        0        0     6819 2020-02-02 00:00:00.000000 timescoring-0.0.1/src/timescoring/visualization.py
--rw-r--r--   0        0        0    12382 2020-02-02 00:00:00.000000 timescoring-0.0.1/tests/test.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 timescoring-0.0.1/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 timescoring-0.0.1/LICENSE
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 timescoring-0.0.1/README.md
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 timescoring-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 timescoring-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 timescoring-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 timescoring-0.0.2/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 timescoring-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 timescoring-0.0.2/src/timescoring/__init__.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 timescoring-0.0.2/src/timescoring/annotations.py
+-rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 timescoring-0.0.2/src/timescoring/scoring.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 timescoring-0.0.2/src/timescoring/visualization.py
+-rw-r--r--   0        0        0    12973 2020-02-02 00:00:00.000000 timescoring-0.0.2/tests/test.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 timescoring-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 timescoring-0.0.2/README.md
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 timescoring-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6192 2020-02-02 00:00:00.000000 timescoring-0.0.2/PKG-INFO
```

### Comparing `timescoring-0.0.1/src/timescoring/annotations.py` & `timescoring-0.0.2/src/timescoring/annotations.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,61 +6,62 @@
 
 from dataclasses import dataclass
 from typing import List, Tuple
 
 import numpy as np
 from nptyping import Bool, NDArray, Shape
 
+
 @dataclass(frozen=True)
 class Annotation:
     """Class to store annotations both as a binary mask and as a list of events.
-    
+
     Instances can be initiated either from a a binary mask or from a list of events,
     the other data representation will be automatically generated. The class properties
     are immutable to guarantee consistency between both data types.
     """
     events: List[Tuple[int, int]]
     mask: NDArray[Shape["Size"], Bool]
-    fs : int
-    
-    def __init__(self, data, fs : int, numSamples : int = None):
+    fs: int
+
+    def __init__(self, data, fs: int, numSamples: int = None):
         """Initialize an annotation instance.
-        - Annotation(mask, fs) :
+        - Annotation(mask, fs):
         This can either be done by providing a binary vector where positive labels are
         indicated by True.
-        
+
         - Annotation(events, fs, numSamples)
         Or by provding a list of (start, stop) tuples for each event. Start and stop
         times are expected in seconds.
-        
-        The annotation class contains two immutable fields : mask and events.
+
+        The annotation class contains two immutable fields: mask and events.
 
         Args:
             data (List[Tuple[int, int]] OR NDArray[Bool]): _description_
             fs (int): Sampling frequency in Hertz of the annotations.
-            numSamples (int, optional): Is required when initalizing by providing a 
+            numSamples (int, optional): Is required when initalizing by providing a
                 list of (start, stop) tuples. It indicates the number of annotation
                 samples in the annotation binary mask. It should be left to None if
                 a binary mask is provided. Defaults to None.
 
         Raises:
             TypeError: Raises a TypeError if input does not meet one of the expected
                 data types.
         """
         object.__setattr__(self, 'fs', fs)  # Write to frozen object
         # Annotation(events, fs, numSamples)
         # Init by providing a list of start, stop tuples for each event
         if numSamples is not None:
             # Build binary mask associated with list of events
-            mask = np.zeros((numSamples,), dtype=np.bool_)
+            mask = np.zeros((numSamples, ), dtype=np.bool_)
             for event in data:
-                mask[round(event[0]*fs):round(event[1]*fs)] = True
+                mask[round(event[0] * fs):round(event[1] * fs)] = True
             object.__setattr__(self, 'events', data)  # Write to frozen object
             object.__setattr__(self, 'mask', mask)  # Write to frozen object
-        
+
         # Annotation(mask, fs)
         # Init provided by a binary mask with True labels during event
         elif numSamples is None:
             events = list()
             tmpEnd = []
             # Find transitions
             start_i = np.where(np.diff(np.array(data, dtype=int)) == 1)[0]
@@ -68,25 +69,25 @@
 
             # No transitions and first sample is positive -> event is duration of file
             if len(start_i) == 0 and data[0]:
                 events.append((0, len(data) / fs))
             else:
                 # Edge effect - First sample is an event
                 if data[0]:
-                    events.append((0, (end_i[0]+1) / fs))
+                    events.append((0, (end_i[0] + 1) / fs))
                     end_i = np.delete(end_i, 0)
                 # Edge effect - Last event runs until end of file
                 if data[-1]:
                     if len(start_i):
-                        tmpEnd = [((start_i[-1]+1) / fs, len(data) / fs)]
+                        tmpEnd = [((start_i[-1] + 1) / fs, len(data) / fs)]
                         start_i = np.delete(start_i, len(start_i) - 1)
                 # Add all events
                 start_i += 1
                 end_i += 1
                 for i in range(len(start_i)):
                     events.append((start_i[i] / fs, end_i[i] / fs))
                 events += tmpEnd  # add potential end edge effect
             object.__setattr__(self, 'events', events)  # Write to frozen object
             object.__setattr__(self, 'mask', np.array(data, dtype=np.bool_))  # Write to frozen object
-            
+
         else:
             raise TypeError
```

### Comparing `timescoring-0.0.1/src/timescoring/scoring.py` & `timescoring-0.0.2/src/timescoring/scoring.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,227 +4,224 @@
 __author__ = "Jonathan Dan, Una Pale"
 __email__ = "jonathan.dan at epfl.ch"
 
 import numpy as np
 
 from .annotations import Annotation
 
+
 class _Scoring:
     """" Base class for different scoring methods. The class provides the common
     attributes and computation of common scores based on these attributes.
     """
-    fs : int
-    numSamples : int
-    
-    refTrue : int
-    tp : int
-    fp : int
-
-    sensitivity : float
-    precision : float
-    f1 : float
-    fpRate : float
-    
+    fs: int
+    numSamples: int
+
+    refTrue: int
+    tp: int
+    fp: int
+
+    sensitivity: float
+    precision: float
+    f1: float
+    fpRate: float
+
     def computeScores(self):
         """ Compute performance metrics."""
         # Sensitivity
         if self.refTrue > 0:
             self.sensitivity = self.tp / self.refTrue
         else:
             self.sensitivity = np.nan  # no ref event
-        
+
         # Precision
         if self.tp + self.fp > 0:
             self.precision = self.tp / (self.tp + self.fp)
         else:
             self.precision = np.nan  # no hyp event
-            
+
         # F1 Score
         if np.isnan(self.sensitivity) or np.isnan(self.precision):
             self.f1 = np.nan
         elif (self.sensitivity + self.precision) == 0:  # No overlap ref & hyp
             self.f1 = 0
         else:
             self.f1 = 2 * self.sensitivity * self.precision / (self.sensitivity + self.precision)
-            
+
         # FP Rate
         self.fpRate = self.fp / (self.numSamples / self.fs / 3600 / 24)  # FP per day
-    
-    
+
+
 class SampleScoring(_Scoring):
     """Calculates performance metrics on the sample by sample basis"""
-    
-    def __init__(self, ref : Annotation, hyp : Annotation, fs : int = 1):
+
+    def __init__(self, ref: Annotation, hyp: Annotation, fs: int = 1):
         """Computes scores on a sample by sample basis.
 
         Args:
             ref (Annotation): Reference annotations (ground-truth)
             hyp (Annotation): Hypotheses annotations (output of a ML pipeline)
             fs (int): Sampling frequency of the labels. Default 1 Hz.
         """
         # Resample Data
-        ref = Annotation(ref.events, fs, round(len(ref.mask)/ref.fs*fs))
-        hyp = Annotation(hyp.events, fs, round(len(hyp.mask)/hyp.fs*fs))
-        
+        ref = Annotation(ref.events, fs, round(len(ref.mask) / ref.fs * fs))
+        hyp = Annotation(hyp.events, fs, round(len(hyp.mask) / hyp.fs * fs))
+
         if len(ref.mask) != len(hyp.mask):
             raise ValueError(("The number of samples in the reference Annotation"
                               " (n={}) must match the number of samples in the "
                               "hypotheses Annotation (n={})").format(len(ref.mask), len(hyp.mask)))
-        
+
         self.tpMask = ref.mask & hyp.mask
         self.fpMask = ~ref.mask & hyp.mask
         self.fnMask = ref.mask & ~hyp.mask
-        
+
         self.fs = fs
         self.numSamples = len(ref.mask)
-        
+
         self.refTrue = np.sum(ref.mask)
-        
+
         self.tp = np.sum(self.tpMask)
         self.fp = np.sum(self.fpMask)
-        
+
         self.computeScores()
-        
-        
+
+
 class EventScoring(_Scoring):
     """Calculates performance metrics on an event basis"""
     class Parameters:
         """Parameters for event scoring"""
-        
-        def __init__(self, toleranceStart : float = 30,
-                     toleranceEnd : float = 60,
-                     minOverlap : float = 0,
-                     maxEventDuration : float = 5*60,
-                     minDurationBetweenEvents : float = 90):
+
+        def __init__(self, toleranceStart: float = 30,
+                     toleranceEnd: float = 60,
+                     minOverlap: float = 0,
+                     maxEventDuration: float = 5 * 60,
+                     minDurationBetweenEvents: float = 90):
             """Parameters for event scoring
 
             Args:
-                toleranceStart (float): Allow some tolerance on the start of an event 
+                toleranceStart (float): Allow some tolerance on the start of an event
                     without counting a false detection. Defaults to 30  # [seconds].
-                toleranceEnd (float): Allow some tolerance on the end of an event 
+                toleranceEnd (float): Allow some tolerance on the end of an event
                     without counting a false detection. Defaults to 60  # [seconds].
-                minOverlap (float): Minimum relative overlap between ref and hyp for 
+                minOverlap (float): Minimum relative overlap between ref and hyp for
                     a detection. Defaults to 0 which corresponds to any overlap  # [relative].
-                maxEventDuration (float): Automatically split events longer than a 
+                maxEventDuration (float): Automatically split events longer than a
                     given duration. Defaults to 5*60  # [seconds].
                 minDurationBetweenEvents (float): Automatically merge events that are
                     separated by less than the given duration. Defaults to 90 # [seconds].
-            """   
+            """
             self.toleranceStart = toleranceStart
             self.toleranceEnd = toleranceEnd
             self.minOverlap = minOverlap
             self.maxEventDuration = maxEventDuration
             self.minDurationBetweenEvents = minDurationBetweenEvents
 
-    
-    def __init__(self, ref : Annotation, hyp : Annotation, param : Parameters = Parameters()):
+    def __init__(self, ref: Annotation, hyp: Annotation, param: Parameters = Parameters()):
         """Computes a scoring on an event basis.
 
         Args:
             ref (Annotation): Reference annotations (ground-truth)
             hyp (Annotation): Hypotheses annotations (output of a ML pipeline)
             param(EventScoring.Parameters, optional):  Parameters for event scoring.
                 Defaults to default values.
         """
         # Resample data
         fs = 10  # Operate at a time precision of 10 Hz
-        ref = Annotation(ref.events, fs, round(len(ref.mask)/ref.fs*fs))
-        hyp = Annotation(hyp.events, fs, round(len(hyp.mask)/hyp.fs*fs))
-        
+        ref = Annotation(ref.events, fs, round(len(ref.mask) / ref.fs * fs))
+        hyp = Annotation(hyp.events, fs, round(len(hyp.mask) / hyp.fs * fs))
+
         # Merge events separated by less than param.minDurationBetweenEvents
         ref = EventScoring._mergeNeighbouringEvents(ref, param.minDurationBetweenEvents)
         hyp = EventScoring._mergeNeighbouringEvents(hyp, param.minDurationBetweenEvents)
-        
+
         # Split long events to param.maxEventDuration
         ref = EventScoring._splitLongEvents(ref, param.maxEventDuration)
         hyp = EventScoring._splitLongEvents(hyp, param.maxEventDuration)
-        
+
         self.fs = ref.fs
         self.numSamples = len(ref.mask)
-        
+
         self.refTrue = len(ref.events)
-        
+
         # Count True detections
         self.tp = 0
         self.tpMask = np.zeros_like(ref.mask)
         extendedRef = EventScoring._extendEvents(ref, param.toleranceStart, param.toleranceEnd)
         for event in extendedRef.events:
-            if (np.sum(hyp.mask[round(event[0]*hyp.fs):round(event[1]*hyp.fs)])/hyp.fs)/(event[1]-event[0]) > param.minOverlap + 1e-6:
-                self.tp +=1
-                self.tpMask[round(event[0]*ref.fs):round(event[1]*ref.fs)] = 1
-                
+            relativeOverlap = (np.sum(hyp.mask[round(event[0] * hyp.fs):round(event[1] * hyp.fs)]) / hyp.fs
+                               ) / (event[1] - event[0])
+            if relativeOverlap > param.minOverlap + 1e-6:
+                self.tp += 1
+                self.tpMask[round(event[0] * ref.fs):round(event[1] * ref.fs)] = 1
+
         # Count False detections
         self.fp = 0
-        extendedDetections = EventScoring._extendEvents(Annotation(self.tpMask, ref.fs), param.toleranceStart, param.toleranceEnd)
         for event in hyp.events:
-            if np.any(~self.tpMask[round(event[0]*ref.fs):round(event[1]*ref.fs)]):
-                self.fp +=1
-        
+            if np.any(~self.tpMask[round(event[0] * ref.fs):round(event[1] * ref.fs)]):
+                self.fp += 1
+
         self.computeScores()
-        
-        
-    def _splitLongEvents(events : Annotation, maxEventDuration : float) -> Annotation:
+
+    def _splitLongEvents(events: Annotation, maxEventDuration: float) -> Annotation:
         """Split events longer than maxEventDuration in shorter events.
         Args:
             events (Annotation): Annotation object containing events to split
             maxEventDuration (float): maximum duration of an event [seconds]
 
         Returns:
             Annotation: Returns a new Annotation instance with all events split to
                 a maximum duration of maxEventDuration.
         """
-        
+
         shorterEvents = events.events.copy()
-        
+
         for i, event in enumerate(shorterEvents):
             if event[1] - event[0] > maxEventDuration:
                 shorterEvents[i] = (event[0], event[0] + maxEventDuration)
                 shorterEvents.insert(i + 1, (event[0] + maxEventDuration, event[1]))
-                
+
         return Annotation(shorterEvents, events.fs, len(events.mask))
-    
-    
-    def _mergeNeighbouringEvents(events : Annotation, minDurationBetweenEvents : float) -> Annotation:
+
+    def _mergeNeighbouringEvents(events: Annotation, minDurationBetweenEvents: float) -> Annotation:
         """Merge events separated by less than longer than minDurationBetweenEvents.
         Args:
             events (Annotation): Annotation object containing events to split
             minDurationBetweenEvents (float): minimum duration between events [seconds]
 
         Returns:
             Annotation: Returns a new Annotation instance with events separated by less than
                 minDurationBetweenEvents merged as one event.
         """
-        
+
         mergedEvents = events.events.copy()
-        
+
         i = 1
         while i < len(mergedEvents):
             event = mergedEvents[i]
-            if  event[0] - mergedEvents[i-1][1] < minDurationBetweenEvents:
-                mergedEvents[i-1] = (mergedEvents[i-1][0], event[1])
+            if event[0] - mergedEvents[i - 1][1] < minDurationBetweenEvents:
+                mergedEvents[i - 1] = (mergedEvents[i - 1][0], event[1])
                 del mergedEvents[i]
                 i -= 1
             i += 1
-                
+
         return Annotation(mergedEvents, events.fs, len(events.mask))
-    
-    
-    def _extendEvents(events : Annotation, before : float, after : float) -> Annotation:
+
+    def _extendEvents(events: Annotation, before: float, after: float) -> Annotation:
         """Extend duration of all events in an Annotation object.
 
         Args:
             events (Annotation): Annotation object containing events to extend
             before (float): Time to extend before each event [seconds]
             after (float):  Time to extend after each event [seconds]
 
         Returns:
             Annotation: Returns a new Annotation instance with all events extended
         """
-        
+
         extendedEvents = events.events.copy()
         fileDuration = len(events.mask) / events.fs
-        
+
         for i, event in enumerate(extendedEvents):
             extendedEvents[i] = (max(0, event[0] - before), (min(fileDuration, event[1] + after)))
-            
+
         return Annotation(extendedEvents, events.fs, len(events.mask))
-
```

### Comparing `timescoring-0.0.1/src/timescoring/visualization.py` & `timescoring-0.0.2/src/timescoring/visualization.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,180 +1,189 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
 from .annotations import Annotation
 from . import scoring
 
-def plotSampleScoring(ref : Annotation, hyp : Annotation, fs : int = 1) -> plt.figure:
+
+def plotSampleScoring(ref: Annotation, hyp: Annotation, fs: int = 1) -> plt.figure:
     """Build an overview plot showing the outcome of sample scoring.
 
     Args:
-        ref (Annotation): Reference annotations (ground-truth)
+        ref (Annotation): Reference annotations (ground - truth)
         hyp (Annotation): Hypotheses annotations (output of a ML pipeline)
         fs (int): Sampling frequency of the labels. Default 1 Hz.
 
     Returns:
         plt.figure: Output matplotlib figure
     """
-    
+
     score = scoring.SampleScoring(ref, hyp, fs)
-    time = np.arange(len(ref.mask)) / fs
+    time = np.arange(len(score.tpMask)) / fs
+    # Resample Data
+    ref = Annotation(ref.events, fs, round(len(ref.mask) / ref.fs * fs))
+    hyp = Annotation(hyp.events, fs, round(len(hyp.mask) / hyp.fs * fs))
 
     fig = plt.figure(figsize=(16, 3))
-    
+
     # Plot background shading
-    plt.fill_between(time, 0, 1, where=score.tpMask, 
+    plt.fill_between(time, 0, 1, where=score.tpMask,
                      alpha=0.2, color='tab:green',
                      transform=plt.gca().get_xaxis_transform())
-    plt.fill_between(time, 0, 1, where=score.fnMask, 
+    plt.fill_between(time, 0, 1, where=score.fnMask,
                      alpha=0.2, color='tab:purple',
                      transform=plt.gca().get_xaxis_transform())
     plt.fill_between(time, 0, 1, where=score.fpMask,
                      alpha=0.2, color='tab:red',
                      transform=plt.gca().get_xaxis_transform())
-    
+
     # Plot Labels
-    plt.plot(time, ref.mask*0.4 + 0.6, 'k')
-    plt.plot(time, hyp.mask*0.4 + 0.1, 'k')
-    
+    plt.plot(time, ref.mask * 0.4 + 0.6, 'k')
+    plt.plot(time, hyp.mask * 0.4 + 0.1, 'k')
+
     # Plot Colored dots for detections
     lineFn, = plt.plot(time[score.fnMask], score.fnMask[score.fnMask], 'o', color='tab:purple')
     lineTp, = plt.plot(time[score.tpMask], score.tpMask[score.tpMask], 'o', color='tab:green')
-    plt.plot(time[score.tpMask], score.tpMask[score.tpMask]*0.5, 'o', color='tab:green')
-    lineFp, = plt.plot(time[score.fpMask], score.fpMask[score.fpMask]*0.5, 'o', color='tab:red')
-        
-    # Text  
+    plt.plot(time[score.tpMask], score.tpMask[score.tpMask] * 0.5, 'o', color='tab:green')
+    lineFp, = plt.plot(time[score.fpMask], score.fpMask[score.fpMask] * 0.5, 'o', color='tab:red')
+
+    # Text
     plt.title('Sample based Scoring')
 
     plt.yticks([0.3, 0.8], ['HYP', 'REF'])
     _scale_time_xaxis(fig)
-    
+
     _buildLegend(lineTp, lineFn, lineFp, score, fig)
-        
+
     return fig
 
 
-def plotEventScoring(ref : Annotation, hyp : Annotation, param : scoring.EventScoring.Parameters = scoring.EventScoring.Parameters()) -> plt.figure:
+def plotEventScoring(ref: Annotation, hyp: Annotation,
+                     param: scoring.EventScoring.Parameters = scoring.EventScoring.Parameters()) -> plt.figure:
     """Build an overview plot showing the outcome of event scoring.
 
     Args:
-        ref (Annotation): Reference annotations (ground-truth)
+        ref (Annotation): Reference annotations (ground - truth)
         hyp (Annotation): Hypotheses annotations (output of a ML pipeline)
         param(EventScoring.Parameters, optional):  Parameters for event scoring.
             Defaults to default values.
 
     Returns:
         plt.figure: Output matplotlib figure
     """
     def _plotEvent(x, y, color):
-            plt.axvspan(x[0], x[1], alpha=0.2, color=color)
-            if x[1] - x[0] > 0:
-                plt.plot(x, y, color=color, linewidth=5, solid_capstyle='butt')
-            else:
-                plt.scatter(x[0], y[0], color=color)
-    
-    
+        plt.axvspan(x[0], x[1], alpha=0.2, color=color)
+        if x[1] - x[0] > 0:
+            plt.plot(x, y, color=color, linewidth=5, solid_capstyle='butt')
+        else:
+            plt.scatter(x[0], y[0], color=color)
+
     score = scoring.EventScoring(ref, hyp, param)
     time = np.arange(len(ref.mask)) / ref.fs
 
     fig = plt.figure(figsize=(16, 3))
-    
+
     # Plot Labels
-    plt.plot(time, ref.mask*0.4 + 0.6, 'k')
-    plt.plot(time, hyp.mask*0.4 + 0.1, 'k')
-    
+    plt.plot(time, ref.mask * 0.4 + 0.6, 'k')
+    plt.plot(time, hyp.mask * 0.4 + 0.1, 'k')
+
     # Initialize lines for legend
     lineTp, = plt.plot([], [], color='tab:green', linewidth=5)
     lineFn, = plt.plot([], [], color='tab:purple', linewidth=5)
     lineFp, = plt.plot([], [], color='tab:red', linewidth=5)
-    
+
     # Plot REF TP & FN
     for event in ref.events:
         # TP
-        if np.any(score.tpMask[round(event[0]*score.fs):round(event[1]*score.fs)]):
-            _plotEvent([event[0], event[1]-(1/ref.fs)], [1, 1], 'tab:green')
-            score.tpMask[round(event[0]*score.fs):round(event[1]*score.fs)] = 1
+        if np.any(score.tpMask[round(event[0] * score.fs):round(event[1] * score.fs)]):
+            _plotEvent([event[0], event[1] - (1 / ref.fs)], [1, 1], 'tab:green')
+            score.tpMask[round(event[0] * score.fs):round(event[1] * score.fs)] = 1
         else:
-            _plotEvent([event[0], event[1]-(1/ref.fs)], [1, 1], 'tab:purple')
-    
-    # Plot HYP TP & FP 
+            _plotEvent([event[0], event[1] - (1 / ref.fs)], [1, 1], 'tab:purple')
+
+    # Plot HYP TP & FP
     for event in hyp.events:
         # FP
-        if np.all(~score.tpMask[round(event[0]*score.fs):round(event[1]*score.fs)]):
-            _plotEvent([event[0], event[1]-(1/ref.fs)], [0.5, 0.5], 'tab:red')
+        if np.all(~score.tpMask[round(event[0] * score.fs):round(event[1] * score.fs)]):
+            _plotEvent([event[0], event[1] - (1 / ref.fs)], [0.5, 0.5], 'tab:red')
         # TP
-        elif np.all(score.tpMask[round(event[0]*score.fs):round(event[1]*score.fs)]):
-            plt.plot([event[0], event[1]-(1/ref.fs)], [0.5, 0.5], color='tab:green', linewidth=5, solid_capstyle='butt', linestyle='solid')
+        elif np.all(score.tpMask[round(event[0] * score.fs):round(event[1] * score.fs)]):
+            plt.plot([event[0], event[1] - (1 / ref.fs)], [0.5, 0.5],
+                     color='tab:green', linewidth=5, solid_capstyle='butt', linestyle='solid')
         # Mix TP, FP
         else:
-            _plotEvent([event[0], event[1]-(1/ref.fs)], [0.5, 0.5], 'tab:red')
-            plt.plot([event[0], event[1]-(1/ref.fs)], [0.5, 0.5], color='tab:green', linewidth=5, solid_capstyle='butt', linestyle=(0, (2, 2)))
+            _plotEvent([event[0], event[1] - (1 / ref.fs)], [0.5, 0.5], 'tab:red')
+            plt.plot([event[0], event[1] - (1 / ref.fs)], [0.5, 0.5],
+                     color='tab:green', linewidth=5, solid_capstyle='butt', linestyle=(0, (2, 2)))
 
-    # Text  
+    # Text
     plt.title('Event Scoring')
 
     plt.yticks([0.3, 0.8], ['HYP', 'REF'])
     _scale_time_xaxis(fig)
-    
+
     _buildLegend(lineTp, lineFn, lineFp, score, fig)
-        
+
     return fig
 
 
-def _scale_time_xaxis(fig : plt.figure):
+def _scale_time_xaxis(fig: plt.figure):
     """Scale x axis of a figure where initial values are in seconds.
-    
-    The function leaves the xaxis as is if the number of seconds to display is < 5*60
+
+    The function leaves the xaxis as is if the number of seconds to display is < 5 * 60
     If it is larger than 5 minutes, xaxis is formatted as m:s
     If it is larger than 5 hours, xaxis is formatted as h:m:s
-    
+
     Args:
         fig (plt.figure): figure to handle
     """
-    
-    s2m = lambda x, _: f'{int(x/60)}:{int(x%60)}'
-    s2h = lambda x, _: f'{int(x/3600)}:{int((x/60)%60)}:{int(x%60)}'
-    
+
+    def s2m(x, _):
+        return f'{int(x / 60)}:{int(x%60)}'
+
+    def s2h(x, _):
+        return f'{int(x / 3600)}:{int((x / 60)%60)}:{int(x%60)}'
+
     maxTime = fig.gca().get_xlim()[1]
-    if maxTime > 5*60*60:
+    if maxTime > 5 * 60 * 60:
         fig.gca().xaxis.set_major_formatter(s2h)
         fig.gca().set_xlabel('time [h:m:s]')
-    elif maxTime > 5*60:
+    elif maxTime > 5 * 60:
         fig.gca().xaxis.set_major_formatter(s2m)
         fig.gca().set_xlabel('time [m:s]')
     else:
         fig.gca().set_xlabel('time [s]')
-        
-        
+
+
 def _buildLegend(lineTp, lineFn, lineFp, score, fig):
     """Build legend and adjust spacing for scoring text"""
     plt.legend([lineTp, lineFn, lineFp],
-               ['TP : {}'.format(np.sum(score.tp)), 
-                'FN : {}'.format(np.sum(score.refTrue - score.tp)),
-                'FP : {}'.format(np.sum(score.fp))], loc=(1.02, 0.65))
-    
-    textstr = "• Sensitivity : {:.2f}\n".format(score.sensitivity)
-    textstr+= "• Precision   : {:.2f}\n".format(score.precision)
-    textstr+= "• F1-score    : {:.2f}".format(score.f1)
+               ['TP: {}'.format(np.sum(score.tp)),
+                'FN: {}'.format(np.sum(score.refTrue - score.tp)),
+                'FP: {}'.format(np.sum(score.fp))], loc=(1.02, 0.65))
+
+    textstr = "• Sensitivity: {:.2f}\n".format(score.sensitivity)
+    textstr += "• Precision  : {:.2f}\n".format(score.precision)
+    textstr += "• F1 - score   : {:.2f}".format(score.f1)
     fig.text(1.02, 0.05, textstr, fontsize=12, transform=plt.gca().transAxes)
-    
+
     # Adjust spacing
     plt.margins(x=0)  # No margin on X data
     plt.tight_layout()
     fig.subplots_adjust(right=0.86)  # Allow space for scoring text
 
 
 if __name__ == "__main__":
     fs = 1
-    duration = 66*60
-    ref = Annotation([(8*60, 12*60), (30*60, 35*60), (48*60, 50*60)], fs, duration)
-    hyp = Annotation([(8*60, 12*60), (28*60, 32*60), (50.5*60, 51*60), (60*60, 62*60)], fs, duration)
+    duration = 66 * 60
+    ref = Annotation([(8 * 60, 12 * 60), (30 * 60, 35 * 60), (48 * 60, 50 * 60)], fs, duration)
+    hyp = Annotation([(8 * 60, 12 * 60), (28 * 60, 32 * 60), (50.5 * 60, 51 * 60), (60 * 60, 62 * 60)], fs, duration)
 
     fig = plotSampleScoring(ref, hyp)
     param = scoring.EventScoring.Parameters(
-            toleranceStart=30,
-            toleranceEnd=60,   
-            minOverlap=0,
-            maxEventDuration=5*60,
-            minDurationBetweenEvents=90)
+        toleranceStart=30,
+        toleranceEnd=60,
+        minOverlap=0,
+        maxEventDuration=5 * 60,
+        minDurationBetweenEvents=90)
     fig = plotEventScoring(ref, hyp, param)
     plt.show()
```

### Comparing `timescoring-0.0.1/LICENSE` & `timescoring-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timescoring-0.0.1/README.md` & `timescoring-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Library for measuring performance of time series classification
 
+![PyPI](https://img.shields.io/pypi/v/timescoring?style=flat-square)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/esl-epfl/epilepsy_performance_metrics/python-app.yml?label=unittest&style=flat-square)
+
 ## Motivation
 
 For temporal and sequential data (e.g. in biomedical applications), standard performance evaluation metrics, such as sensitivity and specificity, may not always be the most appropriate and can even be misleading. Evaluation metrics must ultimately reflect the needs of users and also be sufficiently sensitive to guide algorithm development.
 
 For example, for epilepsy monitoring, neurologists ask for assesments on the level of seizure episodes (events), rather than duration or sample-by-sample based metrics. Similarly,  another performance measure with a strong practical impact in epilepsy monitoring, is the false alarm rate (FAR), or the number of false positives per hour/day. Clinicians and patients see this measure as more meaningful than some established metrics in the ML community, and are very demanding in terms of performance, requiring it to be as low as possible for potential wearable applications (e.g., less than 1 FP/day). This also necessitates exceptionally high constraints on the required precision (usually much higher than 99\%).
 
 For this reason, here we provide code that measures performance on the level of events and on a sample-by-sample basis.
@@ -56,22 +59,23 @@
 - `precision`
 - `f1` : F1-score
 - `fpRate` : False alarm rate per 24h
 
 ## Example of usage
 
 ```python
-## Loading Annotations ##
+# Loading Annotations #
+
 
 from timescoring.annotations import Annotation
 
 # Annotation objects can be instantiated from a binary mask
 
 fs = 1
-mask = [0,1,1,0,0,0,1,1,1,0]
+mask = [0, 1, 1, 0, 0, 0, 1, 1, 1, 0]
 
 labels = Annotation(mask, fs)
 
 print('Annotation objects contain a representation as a mask and as a list of events:')
 print(labels.mask)
 print(labels.events)
 
@@ -80,37 +84,37 @@
 fs = 1
 numSamples = 10  # In this case the duration of the recording in samples should be provided
 events = [(1, 3), (6, 9)]
 
 labels = Annotation(events, fs, numSamples)
 
 
-## Computing performance score ## 
+# Computing performance score #
 
 from timescoring import scoring
 from timescoring import visualization
 
 fs = 1
-duration = 66*60
-ref = Annotation([(8*60, 12*60), (30*60, 35*60), (48*60, 50*60)], fs, duration)
-hyp = Annotation([(8*60, 12*60), (28*60, 32*60), (50.5*60, 51*60), (60*60, 62*60)], fs, duration)
+duration = 66 * 60
+ref = Annotation([(8 * 60, 12 * 60), (30 * 60, 35 * 60), (48 * 60, 50 * 60)], fs, duration)
+hyp = Annotation([(8 * 60, 12 * 60), (28 * 60, 32 * 60), (50.5 * 60, 51 * 60), (60 * 60, 62 * 60)], fs, duration)
 scores = scoring.SampleScoring(ref, hyp)
 figSamples = visualization.plotSampleScoring(ref, hyp)
 
 # Scores can also be computed per event
 param = scoring.EventScoring.Parameters(
-        toleranceStart=30,
-        toleranceEnd=60,   
-        minOverlap=0,
-        maxEventDuration=5*60,
-        minDurationBetweenEvents=90)
+    toleranceStart=30,
+    toleranceEnd=60,
+    minOverlap=0,
+    maxEventDuration=5 * 60,
+    minDurationBetweenEvents=90)
 scores = scoring.EventScoring(ref, hyp, param)
 figEvents = visualization.plotEventScoring(ref, hyp, param)
 
 print("# Event scoring\n" +
-      "- Sensitivity : {:.2f} \n".format(scores.sensitivity) + 
-      "- Precision   : {:.2f} \n".format(scores.precision) + 
-      "- F1-score    : {:.2f} \n".format(scores.f1) + 
+      "- Sensitivity : {:.2f} \n".format(scores.sensitivity) +
+      "- Precision   : {:.2f} \n".format(scores.precision) +
+      "- F1-score    : {:.2f} \n".format(scores.f1) +
       "- FP/24h      : {:.2f} \n".format(scores.fpRate))
 ```
 
-A presentation explaining these metrics is available [here](https://drive.google.com/file/d/1-k6i2jVpU7bzqnV6zQPUKlfPkO7qaXau/view?usp=sharing).
+A presentation explaining these metrics is available [here](https://drive.google.com/file/d/1-k6i2jVpU7bzqnV6zQPUKlfPkO7qaXau/view?usp=sharing).
```

### Comparing `timescoring-0.0.1/pyproject.toml` & `timescoring-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "timescoring"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jonathan Dan", email="jonathan.dan@epfl.ch" },
   { name="Una Pale", email="una.pale@epfl.ch" },
   { name="PEDESITE" }
 ]
 description = "Library for measuring performance of time series classification"
 readme = "README.md"
```

### Comparing `timescoring-0.0.1/PKG-INFO` & `timescoring-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timescoring
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for measuring performance of time series classification
 Project-URL: Homepage, https://github.com/esl-epfl/epilepsy_performance_metrics
 Project-URL: Bug Tracker, https://github.com/esl-epfl/epilepsy_performance_metrics/issues
 Author: PEDESITE
 Author-email: Jonathan Dan <jonathan.dan@epfl.ch>, Una Pale <una.pale@epfl.ch>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,17 @@
 Requires-Dist: matplotlib>=3.7.1
 Requires-Dist: nptyping>=2.5.0
 Requires-Dist: numpy>=1.24.3
 Description-Content-Type: text/markdown
 
 # Library for measuring performance of time series classification
 
+![PyPI](https://img.shields.io/pypi/v/timescoring?style=flat-square)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/esl-epfl/epilepsy_performance_metrics/python-app.yml?label=unittest&style=flat-square)
+
 ## Motivation
 
 For temporal and sequential data (e.g. in biomedical applications), standard performance evaluation metrics, such as sensitivity and specificity, may not always be the most appropriate and can even be misleading. Evaluation metrics must ultimately reflect the needs of users and also be sufficiently sensitive to guide algorithm development.
 
 For example, for epilepsy monitoring, neurologists ask for assesments on the level of seizure episodes (events), rather than duration or sample-by-sample based metrics. Similarly,  another performance measure with a strong practical impact in epilepsy monitoring, is the false alarm rate (FAR), or the number of false positives per hour/day. Clinicians and patients see this measure as more meaningful than some established metrics in the ML community, and are very demanding in terms of performance, requiring it to be as low as possible for potential wearable applications (e.g., less than 1 FP/day). This also necessitates exceptionally high constraints on the required precision (usually much higher than 99\%).
 
 For this reason, here we provide code that measures performance on the level of events and on a sample-by-sample basis.
@@ -74,22 +77,23 @@
 - `precision`
 - `f1` : F1-score
 - `fpRate` : False alarm rate per 24h
 
 ## Example of usage
 
 ```python
-## Loading Annotations ##
+# Loading Annotations #
+
 
 from timescoring.annotations import Annotation
 
 # Annotation objects can be instantiated from a binary mask
 
 fs = 1
-mask = [0,1,1,0,0,0,1,1,1,0]
+mask = [0, 1, 1, 0, 0, 0, 1, 1, 1, 0]
 
 labels = Annotation(mask, fs)
 
 print('Annotation objects contain a representation as a mask and as a list of events:')
 print(labels.mask)
 print(labels.events)
 
@@ -98,37 +102,37 @@
 fs = 1
 numSamples = 10  # In this case the duration of the recording in samples should be provided
 events = [(1, 3), (6, 9)]
 
 labels = Annotation(events, fs, numSamples)
 
 
-## Computing performance score ## 
+# Computing performance score #
 
 from timescoring import scoring
 from timescoring import visualization
 
 fs = 1
-duration = 66*60
-ref = Annotation([(8*60, 12*60), (30*60, 35*60), (48*60, 50*60)], fs, duration)
-hyp = Annotation([(8*60, 12*60), (28*60, 32*60), (50.5*60, 51*60), (60*60, 62*60)], fs, duration)
+duration = 66 * 60
+ref = Annotation([(8 * 60, 12 * 60), (30 * 60, 35 * 60), (48 * 60, 50 * 60)], fs, duration)
+hyp = Annotation([(8 * 60, 12 * 60), (28 * 60, 32 * 60), (50.5 * 60, 51 * 60), (60 * 60, 62 * 60)], fs, duration)
 scores = scoring.SampleScoring(ref, hyp)
 figSamples = visualization.plotSampleScoring(ref, hyp)
 
 # Scores can also be computed per event
 param = scoring.EventScoring.Parameters(
-        toleranceStart=30,
-        toleranceEnd=60,   
-        minOverlap=0,
-        maxEventDuration=5*60,
-        minDurationBetweenEvents=90)
+    toleranceStart=30,
+    toleranceEnd=60,
+    minOverlap=0,
+    maxEventDuration=5 * 60,
+    minDurationBetweenEvents=90)
 scores = scoring.EventScoring(ref, hyp, param)
 figEvents = visualization.plotEventScoring(ref, hyp, param)
 
 print("# Event scoring\n" +
-      "- Sensitivity : {:.2f} \n".format(scores.sensitivity) + 
-      "- Precision   : {:.2f} \n".format(scores.precision) + 
-      "- F1-score    : {:.2f} \n".format(scores.f1) + 
+      "- Sensitivity : {:.2f} \n".format(scores.sensitivity) +
+      "- Precision   : {:.2f} \n".format(scores.precision) +
+      "- F1-score    : {:.2f} \n".format(scores.f1) +
       "- FP/24h      : {:.2f} \n".format(scores.fpRate))
 ```
 
-A presentation explaining these metrics is available [here](https://drive.google.com/file/d/1-k6i2jVpU7bzqnV6zQPUKlfPkO7qaXau/view?usp=sharing).
+A presentation explaining these metrics is available [here](https://drive.google.com/file/d/1-k6i2jVpU7bzqnV6zQPUKlfPkO7qaXau/view?usp=sharing).
```

