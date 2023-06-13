# Comparing `tmp/EphemSahabatFalak-0.0.4.tar.gz` & `tmp/EphemSahabatFalak-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EphemSahabatFalak-0.0.4.tar", last modified: Thu Jun  8 12:12:42 2023, max compression
+gzip compressed data, was "EphemSahabatFalak-0.0.5.tar", last modified: Tue Jun 13 03:57:30 2023, max compression
```

## Comparing `EphemSahabatFalak-0.0.4.tar` & `EphemSahabatFalak-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 12:12:42.222628 EphemSahabatFalak-0.0.4/
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 12:12:42.220518 EphemSahabatFalak-0.0.4/EphemSahabatFalak/
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    39538 2023-06-08 11:10:54.000000 EphemSahabatFalak-0.0.4/EphemSahabatFalak/KiraanWaktuSolat.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       44 2023-06-08 11:40:58.000000 EphemSahabatFalak-0.0.4/EphemSahabatFalak/__init__.py
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-08 12:12:42.221826 EphemSahabatFalak-0.0.4/EphemSahabatFalak.egg-info/
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11718 2023-06-08 12:12:42.000000 EphemSahabatFalak-0.0.4/EphemSahabatFalak.egg-info/PKG-INFO
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      290 2023-06-08 12:12:42.000000 EphemSahabatFalak-0.0.4/EphemSahabatFalak.egg-info/SOURCES.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        1 2023-06-08 12:12:42.000000 EphemSahabatFalak-0.0.4/EphemSahabatFalak.egg-info/dependency_links.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       46 2023-06-08 12:12:42.000000 EphemSahabatFalak-0.0.4/EphemSahabatFalak.egg-info/requires.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       18 2023-06-08 12:12:42.000000 EphemSahabatFalak-0.0.4/EphemSahabatFalak.egg-info/top_level.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11718 2023-06-08 12:12:42.222224 EphemSahabatFalak-0.0.4/PKG-INFO
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    11075 2023-06-08 11:28:01.000000 EphemSahabatFalak-0.0.4/README.md
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       38 2023-06-08 12:12:42.222718 EphemSahabatFalak-0.0.4/setup.cfg
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1228 2023-06-08 12:12:36.000000 EphemSahabatFalak-0.0.4/setup.py
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-13 03:57:30.438851 EphemSahabatFalak-0.0.5/
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-13 03:57:30.435486 EphemSahabatFalak-0.0.5/EphemSahabatFalak/
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    51556 2023-06-13 03:48:16.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak/KiraanWaktuSolat.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       53 2023-06-11 17:41:20.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak/__init__.py
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-13 03:57:30.438052 EphemSahabatFalak-0.0.5/EphemSahabatFalak.egg-info/
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    13856 2023-06-13 03:57:30.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak.egg-info/PKG-INFO
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      290 2023-06-13 03:57:30.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak.egg-info/SOURCES.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        1 2023-06-13 03:57:30.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak.egg-info/dependency_links.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       46 2023-06-13 03:57:30.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak.egg-info/requires.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       18 2023-06-13 03:57:30.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak.egg-info/top_level.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    13856 2023-06-13 03:57:30.438485 EphemSahabatFalak-0.0.5/PKG-INFO
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    13213 2023-06-12 05:12:54.000000 EphemSahabatFalak-0.0.5/README.md
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       38 2023-06-13 03:57:30.438937 EphemSahabatFalak-0.0.5/setup.cfg
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1228 2023-06-13 03:57:06.000000 EphemSahabatFalak-0.0.5/setup.py
```

### Comparing `EphemSahabatFalak-0.0.4/EphemSahabatFalak/KiraanWaktuSolat.py` & `EphemSahabatFalak-0.0.5/EphemSahabatFalak/KiraanWaktuSolat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 from skyfield import api, almanac
-from skyfield.api import datetime, wgs84, N, E, load
+from skyfield.api import datetime, wgs84, N, E, load, Angle, Distance
 from pytz import timezone
 import datetime as dt
 from skyfield.searchlib import find_discrete
 import pandas as pd
-from mpmath import degrees, acot,cot,sin, atan2, sqrt, cos, radians
+from mpmath import degrees, acot,cot,sin, atan2, sqrt, cos, radians, atan, acos, tan, asin
 from datetime import timedelta
+from skyfield.framelib import ecliptic_frame
+from skyfield.earthlib import refraction
 
 class Takwim:
     def __init__(self,latitude=5.41144, longitude=100.19672, elevation=40, 
                  year = datetime.now().year, month = datetime.now().month, day =datetime.now().day,
                  hour =datetime.now().hour, minute = datetime.now().minute, second =datetime.now().second,
-                 zone='Asia/Kuala_Lumpur', temperature = 27, pressure = 1010, ephem = 'de440s.bsp'): #set default values
+                 zone='Asia/Kuala_Lumpur', temperature = 27, pressure = None, ephem = 'de440s.bsp'): #set default values
         self.latitude = latitude
         self.longitude = longitude
         self.elevation = elevation
         self.year = year
         self.month = month
         self.day = day
         self.hour = hour
         self.minute = minute
         self.second = second
         self.zone = timezone(zone)
         self.temperature = temperature
-        self.pressure = pressure
+
+        if pressure is None:
+            pressure_0 = 101325
+            c_p = 1004.68506
+            t_0 = 288.16
+            g = 9.80665
+            molar = 0.02896968
+            r_0 = 8.314462618
+
+            pressure = pressure_0*(1-(g*self.elevation)/(c_p *t_0))**(c_p*molar/r_0)
+            self.pressure = pressure/100
         self.ephem = ephem
 
         
         
     def location(self):
         loc = wgs84.latlon(self.latitude*N, self.longitude*E, self.elevation)
         
@@ -43,26 +55,38 @@
             current_time = str(current_time.astimezone(self.zone))[:19] #converts the skylib.time to datetime
             
         elif time_format == 'datetime':
             current_time = current_time.astimezone(self.zone) 
         
         return current_time
     
-    def sun_altitude(self, t = None, angle_format = 'skylib', temperature = None, pressure = None):
+    def sun_altitude(self, t = None, angle_format = 'skylib', temperature = None, pressure = None, topo = 'topo'):
         eph = api.load(self.ephem)
         earth, sun = eph['earth'], eph['sun']
         current_topo = earth + self.location()
         if t is None :
             t = self.current_time()
         if temperature is None and pressure is None:
             s_al= current_topo.at(t).observe(sun).apparent().altaz(temperature_C = self.temperature, pressure_mbar = self.pressure)   
         else:
             s_al= current_topo.at(t).observe(sun).apparent().altaz(temperature_C = temperature, pressure_mbar = pressure)
         sun_altitude = s_al[0]
         
+        if topo =='geo' or topo == 'geocentric':
+            topo_vector = self.location().at(self.current_time()).xyz.km
+            radius_at_topo = Distance(km =topo_vector).length().km
+            center_of_earth = Takwim()
+            center_of_earth.latitude = self.latitude
+            center_of_earth.longitude = self.longitude
+            center_of_earth.elevation = -radius_at_topo*1000 #Set observer at the center of the Earth using the x,y,z vector magnitude. 
+            center_of_earth = earth + center_of_earth.location()
+            center_of_earth.pressure = 0
+
+            sun_altitude = center_of_earth.at(t).observe(sun).apparent().altaz(temperature_C = 0, pressure_mbar = 0)[0]
+
         if angle_format != 'skylib' and angle_format != 'degree':
             sun_altitude = sun_altitude.dstr(format=u'{0}{1}°{2:02}′{3:02}.{4:0{5}}″')
         
         elif angle_format == 'degree':
             sun_altitude = sun_altitude.degrees
             
         return sun_altitude
@@ -81,38 +105,63 @@
             sun_azimuth = sun_azimuth.dstr(format=u'{0}{1}°{2:02}′{3:02}.{4:0{5}}″')
         
         elif angle_format == 'degree':
             sun_azimuth = sun_azimuth.degrees
         
         return sun_azimuth
     
-    def sun_distance(self, t = None):
+    def sun_distance(self, t = None, topo = 'topo', unit = 'km'):
         eph = api.load(self.ephem)
         earth, sun = eph['earth'], eph['sun']
         current_topo = earth + self.location()
         if t is None:
             t = self.current_time()
        
-        sun_distance = current_topo.at(t).observe(sun).apparent().altaz(temperature_C = self.temperature, pressure_mbar = self.pressure)   
-        return sun_distance[2]
+        sun_distance = current_topo.at(t).observe(sun).apparent().altaz(temperature_C = self.temperature, pressure_mbar = self.pressure)  
+        if topo == 'topo' or topo== 'topocentric':
+            if unit == 'km' or unit == 'KM':
+                sun_distance = current_topo.at(t).observe(sun).apparent().altaz(temperature_C = self.temperature, pressure_mbar = self.pressure)[2].km
+            else:
+                sun_distance = current_topo.at(t).observe(sun).apparent().altaz(temperature_C = self.temperature, pressure_mbar = self.pressure)[2]
+            return sun_distance
+        else:
+            if unit == 'km' or unit == 'KM':
+                sun_distance = earth.at(t).observe(sun).apparent().distance().km
+            else:
+                sun_distance = earth.at(t).observe(sun).apparent().distance()
+            return sun_distance 
+
     
-    def moon_altitude(self, t = None, angle_format = 'skylib', temperature = None, pressure = None):
+    def moon_altitude(self, t = None, angle_format = 'skylib', temperature = None, pressure = None, topo = 'topo'):
         eph = api.load(self.ephem)
         earth, moon = eph['earth'], eph['moon']
         current_topo = earth + self.location()
+        
         if t is None:
             t = self.current_time()
        
         if temperature is None and pressure is None:
             m_al = current_topo.at(t).observe(moon).apparent().altaz(temperature_C = self.temperature, pressure_mbar = self.pressure)   
         else:
             m_al = current_topo.at(t).observe(moon).apparent().altaz(temperature_C = temperature, pressure_mbar = pressure)   
         
         
         moon_altitude = m_al[0]
+
+        if topo =='geo' or topo == 'geocentric':
+            topo_vector = self.location().at(self.current_time()).xyz.km
+            radius_at_topo = Distance(km =topo_vector).length().km
+            center_of_earth = Takwim()
+            center_of_earth.latitude = self.latitude
+            center_of_earth.longitude = self.longitude
+            center_of_earth.elevation = -radius_at_topo*1000 #Set observer at the center of the Earth using the x,y,z vector magnitude. 
+            center_of_earth = earth + center_of_earth.location()
+            center_of_earth.pressure = 0
+
+            moon_altitude = center_of_earth.at(t).observe(moon).apparent().altaz(temperature_C = 0, pressure_mbar = 0)[0]
         
         if angle_format != 'skylib' and angle_format != 'degree':
             moon_altitude = moon_altitude.dstr(format=u'{0}{1}°{2:02}′{3:02}.{4:0{5}}″')
         
         elif angle_format == 'degree':
             moon_altitude = moon_altitude.degrees
         
@@ -132,73 +181,140 @@
             moon_azimuth = moon_azimuth.dstr(format=u'{0}{1}°{2:02}′{3:02}.{4:0{5}}″')
 
         elif angle_format == 'degree':
             moon_azimuth = moon_azimuth.degrees
             
         return moon_azimuth
     
-    def moon_distance(self, t = None):
+    def moon_distance(self, t = None, topo = 'topo', unit = 'km'):
         eph = api.load(self.ephem)
         earth, moon = eph['earth'], eph['moon']
         current_topo = earth + self.location()
         if t is None:
             t = self.current_time()
        
-        moon_distance = current_topo.at(t).observe(moon).apparent().altaz(temperature_C = self.temperature, pressure_mbar = self.pressure)   
-        return moon_distance[2]
+        if topo == 'topo' or topo== 'topocentric':
+            if unit == 'km' or unit == 'KM':
+                moon_distance = current_topo.at(t).observe(moon).apparent().altaz(temperature_C = self.temperature, pressure_mbar = self.pressure).km
+            else:
+                moon_distance = current_topo.at(t).observe(moon).apparent().altaz(temperature_C = self.temperature, pressure_mbar = self.pressure)
+            return moon_distance[2]
+        else:
+            if unit == 'km' or unit == 'KM':
+                moon_distance = earth.at(t).observe(moon).apparent().distance().km
+            else:
+                moon_distance = earth.at(t).observe(moon).apparent().distance()
+            return moon_distance
+
+        
+    def moon_illumination(self, t = None, topo = 'topo'):
+        eph = api.load(self.ephem)
+        earth, moon, sun = eph['earth'], eph['moon'], eph['sun']
+        current_topo = earth + self.location()
+
+        if t is None:
+            t = self.current_time()
+        if topo == 'geo' or topo == 'geocentric':
+            illumination = earth.at(t).observe(moon).apparent().fraction_illuminated(sun)
+
+        else:
+            illumination = current_topo.at(t).observe(moon).apparent().fraction_illuminated(sun)
+
+        moon_illumination = illumination * 100
+        return moon_illumination
+    
+    def daz(self):
+        moon_az = self.moon_azimuth(angle_format='degree')
+        sun_az = self.sun_azimuth(angle_format='degree')
+
+        return abs(moon_az-sun_az)
+    
+    def arcv(self):
+        moon_alt = self.moon_altitude(topo='geo', angle_format='degree')
+        sun_alt = self.sun_altitude(topo = 'geo', pressure=0, angle_format='degree')
+
+        return abs(moon_alt-sun_alt)
     
     def __iteration_moonset(self, t):
         
         current_moon_altitude = self.moon_altitude(t, pressure = 0).degrees
             
         return current_moon_altitude < -0.8333 #ensure that pressure is set to zero (airless) or it will calculate refracted altitude
 
     __iteration_moonset.step_days = 1/86400
     
     #For moonset/moonrise, syuruk and maghrib, if altitude is customised, ensure that pressure is zero to remove refraction
     #Refracted altitude are taken from Meuss Astronomical Algorithm, p105-107
     def moon_set(self, time_format = 'default'):
+        eph = api.load(self.ephem)
+        moon = eph['moon']
         now = self.current_time().astimezone(self.zone)
         midnight = now.replace(hour = 0, minute = 0, second = 0, microsecond = 0)
         next_midnight = midnight + dt.timedelta(days =1)
         ts = load.timescale()
         t0 = ts.from_datetime(midnight)
         t1 = ts.from_datetime(next_midnight)
-        
-        moon_setting, y = find_discrete(t0, t1, self.__iteration_moonset)
-        moon_rise_set = list(zip(moon_setting,y))
+        surface = Takwim()
+        surface.latitude = self.latitude
+        surface.longitude = self.longitude
+        surface.elevation = 0
+        topo_vector = surface.location().at(self.current_time()).xyz.km
+        radius_at_topo = Distance(km =topo_vector).length().km
+        sun_radius = 695508 #km
+        sun_apparent_radius = degrees(asin(sun_radius/self.sun_distance()))
+        horizon_depression = degrees(acos(radius_at_topo/(radius_at_topo+ self.elevation/1000)))
+        r = 0.016667 / tan((-(horizon_depression+sun_apparent_radius) + 7.31 / (-(horizon_depression+sun_apparent_radius) + 4.4)) * 0.017453292519943296)
+        d = r * (0.28 * self.pressure / (self.temperature + 273.0))    
+
+        f = almanac.risings_and_settings(eph, moon, surface.location(), horizon_degrees= -(d+horizon_depression))
+        moon_sett, nilai = almanac.find_discrete(t0, t1, f)
+        moon_rise_set = list(zip(moon_sett,nilai))
         try:
             for x in moon_rise_set:
-                if x[1] == 1:
+                if x[1] == 0:
                     moon_set_time = x[0].astimezone(self.zone) 
         
             if time_format == 'datetime':
                 moon_set_time = moon_set_time.astimezone(self.zone)
 
             elif time_format == 'string':
                 moon_set_time = str(moon_set_time.astimezone(self.zone))[11:19]
 
             else:
                 moon_set_time = ts.from_datetime(moon_set_time)
         except:
                 return "Moon does not set on " + str(self.day) +"-" + str(self.month) + "-" + str(self.year)
         return moon_set_time
     def moon_rise(self, time_format = 'default'):
+        eph = api.load(self.ephem)
+        moon = eph['moon']
         now = self.current_time().astimezone(self.zone)
         midnight = now.replace(hour = 0, minute = 0, second = 0, microsecond = 0)
         next_midnight = midnight + dt.timedelta(days =1)
         ts = load.timescale()
         t0 = ts.from_datetime(midnight)
         t1 = ts.from_datetime(next_midnight)
-        
-        moon_setting, y = find_discrete(t0, t1, self.__iteration_moonset)
-        moon_rise_set = list(zip(moon_setting,y))
+        surface = Takwim()
+        surface.latitude = self.latitude
+        surface.longitude = self.longitude
+        surface.elevation = 0
+        topo_vector = surface.location().at(self.current_time()).xyz.km
+        radius_at_topo = Distance(km =topo_vector).length().km
+        sun_radius = 695508 #km
+        sun_apparent_radius = degrees(asin(sun_radius/self.sun_distance()))
+        horizon_depression = degrees(acos(radius_at_topo/(radius_at_topo+ self.elevation/1000)))
+        r = 0.016667 / tan((-(horizon_depression+sun_apparent_radius) + 7.31 / (-(horizon_depression+sun_apparent_radius) + 4.4)) * 0.017453292519943296)
+        d = r * (0.28 * self.pressure / (self.temperature + 273.0))    
+
+        f = almanac.risings_and_settings(eph, moon, surface.location(), horizon_degrees= -(d+horizon_depression))
+        moon_sett, nilai = almanac.find_discrete(t0, t1, f)
+        moon_rise_set = list(zip(moon_sett,nilai))
         try:
             for x in moon_rise_set:
-                if x[1] == 0:
+                if x[1] == 1:
                     moon_set_time = x[0].astimezone(self.zone) 
         
             if time_format == 'datetime':
                 moon_set_time = moon_set_time.astimezone(self.zone)
 
             elif time_format == 'string':
                 moon_set_time = str(moon_set_time.astimezone(self.zone))[11:19]
@@ -233,14 +349,81 @@
 
         if angle_format != 'skylib':
             elongation_moon_sun = elongation_moon_sun.dstr(format=u'{0}{1}°{2:02}′{3:02}.{4:0{5}}″')
 
 
         return elongation_moon_sun
     
+    def moon_phase(self,t=None, topo = 'topo'):
+        eph = api.load(self.ephem)
+        earth, moon, sun = eph['earth'], eph['moon'], eph['sun']
+        current_topo = earth + self.location()
+
+        if t is None:
+            t = self.current_time()
+
+        if topo == 'geo' or topo == 'geocentric':
+            e = earth.at(t)
+            s = e.observe(sun).apparent()
+            m = e.observe(moon).apparent()
+
+        else: 
+            e = current_topo.at(t)
+            s = e.observe(sun).apparent()
+            m = e.observe(moon).apparent()
+
+        _, slon, _ = s.frame_latlon(ecliptic_frame) #returns ecliptic latitude, longitude and distance, from the ecliptic reference frame
+        _, mlon, _ = m.frame_latlon(ecliptic_frame)
+        phase = (mlon.degrees - slon.degrees) % 360.0
+
+        return phase
+
+
+    def lunar_crescent_width (self,t=None, topo = 'topo',angle_format = 'skylib', method = 'modern'):
+        eph = api.load(self.ephem)
+        earth, moon, sun = eph['earth'], eph['moon'], eph['sun']
+        current_topo = earth + self.location()
+        radius_of_the_Moon = 1738.1 #at equator. In reality, this should be the radius of the moon along the thickest part of the crescent
+
+        if t is None:
+            t = self.current_time()
+
+        m = moon.at(t)
+        s = m.observe(sun).apparent()
+        if topo == 'geo' or topo == 'geocentric':
+            earth_moon_distance = earth.at(t).observe(moon).apparent().distance().km #center of earth - center of moon distance
+            e = m.observe(earth).apparent() #vector from the center of the moon, to the center of the earth
+        
+        else:
+            earth_moon_distance = current_topo.at(t).observe(moon).apparent().distance().km # topo - center of moon distance
+            e = m.observe(current_topo).apparent() #vector from center of the moon, to topo
+
+        elon_earth_sun = e.separation_from(s) #elongation of the earth-sun, as seen from the center of the moon. Not to be confused with phase angle
+        first_term = atan(radius_of_the_Moon/earth_moon_distance) #returns the angle of the semi-diameter of the moon
+        second_term = atan((radius_of_the_Moon*cos(elon_earth_sun.radians))/earth_moon_distance) #returns the (negative) angle of the semi-ellipse between the inner terminator and center of the moon
+
+        crescent_width = Angle(radians = (first_term + second_term)) # in radians
+
+        if method == 'bruin' or method == 'Bruin':
+            length_crescent_km = 1738.1*(1-cos(self.elongation_moon_sun(topo = topo).radians)) #length of crescent width, in km
+            crescent_width = Angle(degrees = degrees(length_crescent_km/earth_moon_distance)) #in radians
+
+        if angle_format != 'skylib':
+            crescent_width = crescent_width.dstr(format=u'{0}{1}°{2:02}′{3:02}.{4:0{5}}″')
+        
+        return crescent_width
+    
+    def lag_time(self):
+        sun_set = self.waktu_maghrib()
+        moon_set = self.moon_set()
+
+        lag_time = str(dt.timedelta(moon_set-sun_set))[2:7]
+
+        return lag_time
+    
     
     def waktu_zawal(self, time_format = 'default'):
         eph = api.load(self.ephem)
         earth, sun = eph['earth'], eph['sun']
         ts = load.timescale()
         
         transit_Sun = almanac.meridian_transits(eph, sun, self.location())
@@ -395,27 +578,37 @@
     
     __iteration_waktu_syuruk.step_days = 1/86400
     
     def waktu_syuruk(self, altitude = 'default', time_format = 'default'):
         eph = api.load(self.ephem)
         earth, sun = eph['earth'], eph['sun']
         ts = load.timescale()
-        current_topo = earth + self.location()
         now = self.current_time().astimezone(self.zone)
         midnight = now.replace(hour = 0, minute = 0, second = 0, microsecond = 0)
         next_midnight = midnight + dt.timedelta(days =1)
         t0 = ts.from_datetime(midnight)
         t1 = ts.from_datetime(next_midnight)
         self.altitude_syuruk = altitude
         
         if altitude == 'default':
-            twilight_default = almanac.dark_twilight_day(eph, self.location())
-            t2, event = almanac.find_discrete(t0, t1, twilight_default)
-            sunrise_refraction_accounted = t2[event==4]
-            syuruk = sunrise_refraction_accounted[0].astimezone(self.zone)
+            surface = Takwim()
+            surface.latitude = self.latitude
+            surface.longitude = self.longitude
+            surface.elevation = 0
+            topo_vector = surface.location().at(self.current_time()).xyz.km
+            radius_at_topo = Distance(km =topo_vector).length().km
+            sun_radius = 695508 #km
+            sun_apparent_radius = degrees(asin(sun_radius/self.sun_distance()))
+            horizon_depression = degrees(acos(radius_at_topo/(radius_at_topo+ self.elevation/1000)))
+            r = 0.016667 / tan((-(horizon_depression+sun_apparent_radius) + 7.31 / (-(horizon_depression+sun_apparent_radius) + 4.4)) * 0.017453292519943296)
+            d = r * (0.28 * self.pressure / (self.temperature + 273.0))    
+
+            f = almanac.risings_and_settings(eph, sun, surface.location(), horizon_degrees= -(d+horizon_depression))
+            syur, nilai = almanac.find_discrete(t0, t1, f)
+            syuruk = syur[0].astimezone(self.zone)
             
         elif altitude <= 0 and altitude >= -4:
             #legacy edition uses while loop
             """twilight_default = almanac.dark_twilight_day(eph, self.location())
             self.temperature = 0
             self.pressure = 0
             t2, event = almanac.find_discrete(t0, t1, twilight_default)
@@ -483,27 +676,48 @@
     
     __iteration_waktu_maghrib.step_days = 1/86400
     
     def waktu_maghrib(self, altitude = 'default', time_format = 'default'):
         eph = api.load(self.ephem)
         earth, sun = eph['earth'], eph['sun']
         ts = load.timescale()
-        current_topo = earth + self.location()
         now = self.current_time().astimezone(self.zone)
         midnight = now.replace(hour = 0, minute = 0, second = 0, microsecond = 0)
         next_midnight = midnight + dt.timedelta(days =1)
         t0 = ts.from_datetime(midnight)
         t1 = ts.from_datetime(next_midnight)
-        self.altitude_maghrib = altitude
+        
         
         if altitude == 'default':
+            ts = load.timescale()
             twilight_default = almanac.dark_twilight_day(eph, self.location())
             t2, event = almanac.find_discrete(t0, t1, twilight_default)
             sunset_refraction_accounted = t2[event==3]
-            maghrib = sunset_refraction_accounted[1].astimezone(self.zone)
+            maghrib_time = sunset_refraction_accounted[1].astimezone(self.zone)
+            now = maghrib_time - timedelta(minutes=10) #begins iteration 10 minutes before default sunset
+            end = maghrib_time + timedelta(minutes=28) #ends iteration 28 minutes after default sunset
+
+            t0 = ts.from_datetime(now)
+            t1 = ts.from_datetime(end)
+
+            surface = Takwim()
+            surface.latitude = self.latitude
+            surface.longitude = self.longitude
+            surface.elevation = 0
+            topo_vector = surface.location().at(self.current_time()).xyz.km
+            radius_at_topo = Distance(km =topo_vector).length().km
+            sun_radius = 695508 #km
+            sun_apparent_radius = degrees(asin(sun_radius/self.sun_distance()))
+            horizon_depression = degrees(acos(radius_at_topo/(radius_at_topo+ self.elevation/1000)))
+            r = 0.016667 / tan((-(horizon_depression+sun_apparent_radius) + 7.31 / (-(horizon_depression+sun_apparent_radius) + 4.4)) * 0.017453292519943296)
+            d = r * (0.28 * self.pressure / (self.temperature + 273.0))    
+
+            f = almanac.risings_and_settings(eph, sun, surface.location(), horizon_degrees= -(d+horizon_depression))
+            magh, nilai = almanac.find_discrete(t0, t1, f)
+            maghrib = magh[0].astimezone(self.zone)
             
         elif altitude <= 0 and altitude >= -4:
             #legacy version using while loop
             """twilight_default = almanac.dark_twilight_day(eph, self.location())
             self.temperature = 0
             self.pressure = 0
             t2, event = almanac.find_discrete(t0, t1, twilight_default)
@@ -516,20 +730,18 @@
                 y0 = self.sun_altitude(t0)
                 
                 if y0.degrees <= altitude:
                     maghrib = now
                     break
                 now += timedelta(seconds=1)
                 maghrib = now"""
-                
+            self.altitude_maghrib = altitude    
             #starts iteration
             ts = load.timescale()
             twilight_default = almanac.dark_twilight_day(eph, self.location())
-            self.temperature = 0
-            self.pressure = 0
             t2, event = almanac.find_discrete(t0, t1, twilight_default)
             sunset_refraction_accounted = t2[event==3]
             maghrib_time = sunset_refraction_accounted[1].astimezone(self.zone)
             now = maghrib_time - timedelta(minutes=10) #begins iteration 10 minutes before default sunset
             end = maghrib_time + timedelta(minutes=28) #ends iteration 28 minutes after default sunset
 
             t0 = ts.from_datetime(now)
@@ -571,16 +783,14 @@
     
     __iteration_waktu_isya.step_days = 1/86400
     
     def waktu_isyak(self, altitude = 'default', time_format = 'default'):
         eph = api.load(self.ephem)
         earth, sun = eph['earth'], eph['sun']
         ts = load.timescale()
-        current_topo = earth + self.location()
-        sun_altitude = current_topo.at(self.current_time()).observe(sun).apparent().altaz(temperature_C = self.temperature, pressure_mbar = self.pressure)
         now = self.current_time().astimezone(self.zone)
         midnight = now.replace(hour = 0, minute = 0, second = 0, microsecond = 0)
         next_midnight = midnight + dt.timedelta(days =1)
         t0 = ts.from_datetime(midnight)
         t1 = ts.from_datetime(next_midnight)
         self.altitude_isya = altitude
         
@@ -759,15 +969,20 @@
 
     def efemeris_hilal(self, topo = 'topo'):
         alt_bulan_list = []
         alt_mat = []
         azm_mat = []
         azm_bul = []
         elon_bulanMat = []
+        illumination_bulan = []
+        lebar_sabit = []
+        az_diff = []
         tarikh = []
+        arc_vision = []
+        lag_time_list = []
         min_in_day = 1/1440
 
         for i in range (60):
             delta_time = self.waktu_maghrib(time_format= 'default') - (59-i)*min_in_day
             hour = int(str(delta_time.astimezone(self.zone))[11:13])
             minute = int(str(delta_time.astimezone(self.zone))[14:16])
 
@@ -795,14 +1010,34 @@
             azimut_matahari = self.sun_azimuth(angle_format= 'string')
             azm_mat.append(azimut_matahari)
 
             #elongasi bulan matahari
             elongasi_bulan_matahari = self.elongation_moon_sun(angle_format='string', topo = topo)
             elon_bulanMat.append(elongasi_bulan_matahari)
 
+            #iluminasi bulan
+            illumination = self.moon_illumination(topo= topo)
+            illumination_bulan.append(illumination)
+
+            #lebar sabit
+            sabit = self.lunar_crescent_width(topo=topo, angle_format='string')
+            lebar_sabit.append(sabit)
+
+            #Azimuth Difference
+            daz = self.daz()
+            az_diff.append(daz)
+
+            #Arc of Vision
+            arcv = self.arcv()
+            arc_vision.append(arcv)
+
+            #Lag time
+            lagtime = self.lag_time()
+            lag_time_list.append(lagtime)
+
         for i in range (1,60):
             delta_time = self.waktu_maghrib(time_format= 'default') + i*min_in_day
             hour = int(str(delta_time.astimezone(self.zone))[11:13])
             minute = int(str(delta_time.astimezone(self.zone))[14:16])
 
             self.hour = hour
             self.minute = minute
@@ -828,17 +1063,37 @@
             azimut_matahari = self.sun_azimuth(angle_format= 'string')
             azm_mat.append(azimut_matahari)
 
             #elongasi bulan matahari
             elongasi_bulan_matahari = self.elongation_moon_sun(angle_format='string', topo = topo)
             elon_bulanMat.append(elongasi_bulan_matahari)
 
-        ephem_bulan = pd.DataFrame(list(zip(elon_bulanMat,alt_bulan_list, azm_bul, alt_mat, azm_mat)), 
+            #iluminasi bulan
+            illumination = self.moon_illumination(topo= topo)
+            illumination_bulan.append(illumination)
+
+            #lebar sabit
+            sabit = self.lunar_crescent_width(topo=topo, angle_format='string')
+            lebar_sabit.append(sabit)
+
+            #Azimuth Difference
+            daz = self.daz()
+            az_diff.append(daz)
+
+            #Arc of Vision
+            arcv = self.arcv()
+            arc_vision.append(arcv)
+
+            #Lag time
+            lagtime = self.lag_time()
+            lag_time_list.append(lagtime)
+            
+        ephem_bulan = pd.DataFrame(list(zip(elon_bulanMat,alt_bulan_list, azm_bul, alt_mat, azm_mat, illumination_bulan, lebar_sabit, az_diff, arc_vision, lag_time_list)), 
                            index=tarikh, 
-                           columns=["Elongasi","Alt Bulan", "Az Bulan", "Alt Matahari", "Az Matahari"])
+                           columns=["Elongasi","Alt Bulan", "Az Bulan", "Alt Matahari", "Az Matahari", "Illuminasi bulan", "Lebar Hilal(%)", "DAZ", "ARCV", "Lag time"])
 
         return ephem_bulan
     
     def __round_up(self, waktu):
         rounded_up_waktu = str((waktu + dt.timedelta(minutes=1.0)).replace(second= 0))[11:16]
         
         return rounded_up_waktu
@@ -960,8 +1215,7 @@
 
         
         takwim_bulanan = pd.DataFrame(list(zip(bayang_kiblat_mula, bayang_kiblat_tamat, subuh, syuruk, zohor, asar, maghrib, isyak)), index = tarikh, columns=["Bayang mula", "Bayang tamat", "Subuh", "Syuruk", "Zohor", "Asar", "Maghrib", "Isyak"])
 
         return takwim_bulanan
 
 
-
```

### Comparing `EphemSahabatFalak-0.0.4/EphemSahabatFalak.egg-info/PKG-INFO` & `EphemSahabatFalak-0.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,19 @@
-Metadata-Version: 2.1
-Name: EphemSahabatFalak
-Version: 0.0.4
-Summary: Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak
-Home-page: UNKNOWN
-Author: cartcosine (izzatzubir)
-Author-email: <cart.cosine.0x@icloud.com>
-License: UNKNOWN
-Keywords: python,falak,solat,hilal,waktu,matahari,bulan
-Platform: UNKNOWN
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
-
 # Falak_py
 
 <p>EphemSahabatFalak ialah sebuah file python yang mengandungi sebuah python Class iaitu Takwim() yang mempunyai pelbagai method. </p>
 <p> Program ini menggunakan data ephemeris dari JPL Horizon (NASA) iaitu de440s. Pengguna boleh untuk mengubah kepada ephemeris lain </p>
 <p> Program ini menggunapakai pakej Skyfield </p>
+<p> Pengguna boleh melihat contoh dalam directory /EphemSahabatFalak/Contoh </p>
+<p> Antara data yang boleh dijana dengan mudah ialah takwim solat bulanan di kawasan pilihan, jadual hilal bagi cerapan, azimut kiblat.</p>
+<p> Pengguna boleh melihat contoh dalam directory /EphemSahabatFalak/Contoh </p>
 <p> Program ini dihasilkan oleh Izzat Zubir, dengan sokongan dari keluarga, beserta maklum balas dari Dr. Abdul Halim Abdul Aziz, Panel Pakar Falak JAKIM </p>
 
 
+
 <h1> Parameter </h1>
 <p> Terdapat 13 parameter yang boleh diubah:</p>
 <p> nilai dalam kurungan ialah nilai 'default' </p>
 <p>1. latitud (5.41144) </p>
 <p>2. longitud (100.19672) --> latitud dan longitud Pusat Falak Sheikh Tahir</p>
 <p>3. elevation (40) --> dalam unit meter</p>
 <p>4. year (tahun semasa)</p>
@@ -124,17 +109,19 @@
 <p> time_format = 'datetime' -> format waktu subuh dalam python datetime </p>
 <p> time_format = 'string' -> format waktu subuh dalam string (hh:mm:ss) </p>
 <p> time_format = 'default' -> format waktu subuh dalam skyfield.Time </p>
 <hr>
 
 ## Efemeris matahari dan bulan
 
-<h3>moon_altitude(t = current_time, angle_format = 'skylib', temperature = None, pressure = None)</h3>
+<h3>moon_altitude(t = current_time, angle_format = 'skylib',topo = 'topo', temperature = None, pressure = None)</h3>
   <p> Metod ini memberikan altitud bulan pada waktu yang ditetapkan </p>
   <p> Suhu dan Tekanan adalah berdasarkan tetapan yang dibuat </p>
+  <p> Parameter topo boleh dipilih antara topo(centric) dan geo(centric). Nilai default ialah topo</p>
+  <p> Altitud pada tetapan geocentric ialah altitud dari ufuk, yang berkongsi zenith yang sama dengan pemerhati di permukaan. Rujuk Yallop 1998</p>
  <h4>angle_format</h4>
  <p> angle_format = 'skylib' -> format sudut dalam skylib.Angle.radians
  <p> angle_format = 'degree' -> format sudut dalam skylib.Angle.degrees
  <p> angle_format = 'string' -> format sudut dalam string, darjah° minit' saat"
 
 <hr>
 <h3>moon_azimuth(t = None, angle_format = 'skylib')</h3>
@@ -144,17 +131,19 @@
  <p> angle_format = 'skylib' -> format sudut dalam skylib.Angle.radians
  <p> angle_format = 'degree' -> format sudut dalam skylib.Angle.degrees
  <p> angle_format = 'string' -> format sudut dalam string, darjah° minit' saat"
 <hr>
 <h3>moon_distance(t = None, angle_format = 'skylib')</h3>
   <p> Metod ini memberikan jarak bulan dalam unit au </p>
   <hr>
-<h3>sun_altitude(t = current_time, angle_format = 'skylib', temperature = None, pressure = None)</h3>
+<h3>sun_altitude(t = current_time, angle_format = 'skylib', topo='topo' temperature = None, pressure = None)</h3>
   <p> Metod ini memberikan altitud matahari pada waktu yang ditetapkan </p>
   <p> Suhu dan Tekanan adalah berdasarkan tetapan yang dibuat </p>
+  <p> Parameter topo boleh dipilih antara topo(centric) dan geo(centric). Nilai default ialah topo</p>
+  <p> Altitud pada tetapan geocentric ialah altitud dari ufuk, yang berkongsi zenith yang sama dengan pemerhati di permukaan. Rujuk Yallop 1998</p>
  <h4>angle_format</h4>
  <p> angle_format = 'skylib' -> format sudut dalam skylib.Angle.radians
  <p> angle_format = 'degree' -> format sudut dalam skylib.Angle.degrees
  <p> angle_format = 'string' -> format sudut dalam string, darjah° minit' saat"
 
 <hr>
 <h3>sun_azimuth(t = None, angle_format = 'skylib')</h3>
@@ -187,14 +176,39 @@
 <p> Jika tiada waktu terbit, maka ia akan memberikan "Moon does not rise on tarikh semasa"</p>
 <h4>time_format</h4>
 <p> time_format = 'datetime' -> format waktu subuh dalam python datetime </p>
 <p> time_format = 'string' -> format waktu subuh dalam string (hh:mm:ss) </p>
 <p> time_format = 'default' -> format waktu subuh dalam skyfield.Time </p>
 <hr>
 
+<h3>moon_phase(topo = 'topo')</h3>
+<p> Metod ini memberikan fasa bulan</p>
+<p> Fasa bulan dihitung berdasarkan longitud ekliptik bulan</p>
+<p> Nilai 0 ialah ketika bulan baru (new moon)</p>
+<p> Nilai 180 ialah ketika bulan purnama</p>
+<p> Parameter topo boleh dipilih antara 'topo' (default) bagi toposentrik dan 'geo' bagi geosentrik</p>
+<hr>
+
+<h3>lunar_crescent_width(topo = 'topo',angle_format = 'skylib', method = 'modern')</h3>
+<p> Metod ini memberikan sudut bagi ketebalan cahaya bulan</p>
+<p> Ketika bulan purnama, nilai ini akan bersamaan dengan saiz sudut bulan (~32') </p>
+<p> Parameter method boleh dipilih antara 'modern' atau 'Bruin'</p>
+<p> Hitungan Bruin boleh dirujuk pada Bruin (1977). Hitungan beliau menggunakan andaian bulan 2-dimensi </p>
+<p> Hitungan moden dirujuk kepada Segura: https://www.researchgate.net/publication/343219170_Moon%27s_crescent_width </p>
+
+<h3>moon_illumination(topo = 'topo')</h3>
+<p> Metod ini memberikan peratusan bulan yang disinari matahari, dari perspektif Bumi</p>
+<p> Parameter topo boleh dipilih antara 'topo' (default) bagi toposentrik dan 'geo' bagi geosentrik</p>
+
+<h3>daz()<h3>
+<p> Metod ini memberikan perbezaan azimut antara bulan dan matahari </p>
+
+<h3>arcv()<h3>
+<p>Metod ini memberikan perbezaan altitud geocentrik antara Bulan dan Matahari</p>
+
 <h3>azimut_kiblat()</h3>
   <p> Metod ini memberikan azimut kiblat bagi kawasan yang ditetapkan (berdasarkan latitud dan longitud) </p>
   <p> unit azimut kiblat ialah dalam skyfield.Angle.degrees </p>
   <p> latitud dan longitud kaabah yang ditetapkan ialah 21.422487 Utara dan 39.826206 Timur. </p>
   <p> jejari Bumi yang digunakan ialah 6371000 meter </p>
   <p> formula yang digunakan ialah berdasarkan https://www.omnicalculator.com/other/azimuth</p>
   <hr>
@@ -221,9 +235,7 @@
   <h4>tetapan altitud dan saat</h4>
   <p> Tetapan altitud subuh hingga isyak boleh dirujuk pada method waktu solat masing-masing </p>
   <p> Tetapan saat ialah bagi memilih sama ada mahu bundarkan kepada minit bawah (syuruk dan bayang tamat) atau minit atas (selainnya).</p>
   <p> Tetapan asal bagi saat ialah bundarkan, namun jika mahu nilai saat, ubah kepada saat = 'ya' </p>
   
   
   
-
-
```

### Comparing `EphemSahabatFalak-0.0.4/PKG-INFO` & `EphemSahabatFalak-0.0.5/EphemSahabatFalak.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EphemSahabatFalak
-Version: 0.0.4
+Version: 0.0.5
 Summary: Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak
 Home-page: UNKNOWN
 Author: cartcosine (izzatzubir)
 Author-email: <cart.cosine.0x@icloud.com>
 License: UNKNOWN
 Keywords: python,falak,solat,hilal,waktu,matahari,bulan
 Platform: UNKNOWN
@@ -18,17 +18,21 @@
 
 
 # Falak_py
 
 <p>EphemSahabatFalak ialah sebuah file python yang mengandungi sebuah python Class iaitu Takwim() yang mempunyai pelbagai method. </p>
 <p> Program ini menggunakan data ephemeris dari JPL Horizon (NASA) iaitu de440s. Pengguna boleh untuk mengubah kepada ephemeris lain </p>
 <p> Program ini menggunapakai pakej Skyfield </p>
+<p> Pengguna boleh melihat contoh dalam directory /EphemSahabatFalak/Contoh </p>
+<p> Antara data yang boleh dijana dengan mudah ialah takwim solat bulanan di kawasan pilihan, jadual hilal bagi cerapan, azimut kiblat.</p>
+<p> Pengguna boleh melihat contoh dalam directory /EphemSahabatFalak/Contoh </p>
 <p> Program ini dihasilkan oleh Izzat Zubir, dengan sokongan dari keluarga, beserta maklum balas dari Dr. Abdul Halim Abdul Aziz, Panel Pakar Falak JAKIM </p>
 
 
+
 <h1> Parameter </h1>
 <p> Terdapat 13 parameter yang boleh diubah:</p>
 <p> nilai dalam kurungan ialah nilai 'default' </p>
 <p>1. latitud (5.41144) </p>
 <p>2. longitud (100.19672) --> latitud dan longitud Pusat Falak Sheikh Tahir</p>
 <p>3. elevation (40) --> dalam unit meter</p>
 <p>4. year (tahun semasa)</p>
@@ -124,17 +128,19 @@
 <p> time_format = 'datetime' -> format waktu subuh dalam python datetime </p>
 <p> time_format = 'string' -> format waktu subuh dalam string (hh:mm:ss) </p>
 <p> time_format = 'default' -> format waktu subuh dalam skyfield.Time </p>
 <hr>
 
 ## Efemeris matahari dan bulan
 
-<h3>moon_altitude(t = current_time, angle_format = 'skylib', temperature = None, pressure = None)</h3>
+<h3>moon_altitude(t = current_time, angle_format = 'skylib',topo = 'topo', temperature = None, pressure = None)</h3>
   <p> Metod ini memberikan altitud bulan pada waktu yang ditetapkan </p>
   <p> Suhu dan Tekanan adalah berdasarkan tetapan yang dibuat </p>
+  <p> Parameter topo boleh dipilih antara topo(centric) dan geo(centric). Nilai default ialah topo</p>
+  <p> Altitud pada tetapan geocentric ialah altitud dari ufuk, yang berkongsi zenith yang sama dengan pemerhati di permukaan. Rujuk Yallop 1998</p>
  <h4>angle_format</h4>
  <p> angle_format = 'skylib' -> format sudut dalam skylib.Angle.radians
  <p> angle_format = 'degree' -> format sudut dalam skylib.Angle.degrees
  <p> angle_format = 'string' -> format sudut dalam string, darjah° minit' saat"
 
 <hr>
 <h3>moon_azimuth(t = None, angle_format = 'skylib')</h3>
@@ -144,17 +150,19 @@
  <p> angle_format = 'skylib' -> format sudut dalam skylib.Angle.radians
  <p> angle_format = 'degree' -> format sudut dalam skylib.Angle.degrees
  <p> angle_format = 'string' -> format sudut dalam string, darjah° minit' saat"
 <hr>
 <h3>moon_distance(t = None, angle_format = 'skylib')</h3>
   <p> Metod ini memberikan jarak bulan dalam unit au </p>
   <hr>
-<h3>sun_altitude(t = current_time, angle_format = 'skylib', temperature = None, pressure = None)</h3>
+<h3>sun_altitude(t = current_time, angle_format = 'skylib', topo='topo' temperature = None, pressure = None)</h3>
   <p> Metod ini memberikan altitud matahari pada waktu yang ditetapkan </p>
   <p> Suhu dan Tekanan adalah berdasarkan tetapan yang dibuat </p>
+  <p> Parameter topo boleh dipilih antara topo(centric) dan geo(centric). Nilai default ialah topo</p>
+  <p> Altitud pada tetapan geocentric ialah altitud dari ufuk, yang berkongsi zenith yang sama dengan pemerhati di permukaan. Rujuk Yallop 1998</p>
  <h4>angle_format</h4>
  <p> angle_format = 'skylib' -> format sudut dalam skylib.Angle.radians
  <p> angle_format = 'degree' -> format sudut dalam skylib.Angle.degrees
  <p> angle_format = 'string' -> format sudut dalam string, darjah° minit' saat"
 
 <hr>
 <h3>sun_azimuth(t = None, angle_format = 'skylib')</h3>
@@ -187,14 +195,39 @@
 <p> Jika tiada waktu terbit, maka ia akan memberikan "Moon does not rise on tarikh semasa"</p>
 <h4>time_format</h4>
 <p> time_format = 'datetime' -> format waktu subuh dalam python datetime </p>
 <p> time_format = 'string' -> format waktu subuh dalam string (hh:mm:ss) </p>
 <p> time_format = 'default' -> format waktu subuh dalam skyfield.Time </p>
 <hr>
 
+<h3>moon_phase(topo = 'topo')</h3>
+<p> Metod ini memberikan fasa bulan</p>
+<p> Fasa bulan dihitung berdasarkan longitud ekliptik bulan</p>
+<p> Nilai 0 ialah ketika bulan baru (new moon)</p>
+<p> Nilai 180 ialah ketika bulan purnama</p>
+<p> Parameter topo boleh dipilih antara 'topo' (default) bagi toposentrik dan 'geo' bagi geosentrik</p>
+<hr>
+
+<h3>lunar_crescent_width(topo = 'topo',angle_format = 'skylib', method = 'modern')</h3>
+<p> Metod ini memberikan sudut bagi ketebalan cahaya bulan</p>
+<p> Ketika bulan purnama, nilai ini akan bersamaan dengan saiz sudut bulan (~32') </p>
+<p> Parameter method boleh dipilih antara 'modern' atau 'Bruin'</p>
+<p> Hitungan Bruin boleh dirujuk pada Bruin (1977). Hitungan beliau menggunakan andaian bulan 2-dimensi </p>
+<p> Hitungan moden dirujuk kepada Segura: https://www.researchgate.net/publication/343219170_Moon%27s_crescent_width </p>
+
+<h3>moon_illumination(topo = 'topo')</h3>
+<p> Metod ini memberikan peratusan bulan yang disinari matahari, dari perspektif Bumi</p>
+<p> Parameter topo boleh dipilih antara 'topo' (default) bagi toposentrik dan 'geo' bagi geosentrik</p>
+
+<h3>daz()<h3>
+<p> Metod ini memberikan perbezaan azimut antara bulan dan matahari </p>
+
+<h3>arcv()<h3>
+<p>Metod ini memberikan perbezaan altitud geocentrik antara Bulan dan Matahari</p>
+
 <h3>azimut_kiblat()</h3>
   <p> Metod ini memberikan azimut kiblat bagi kawasan yang ditetapkan (berdasarkan latitud dan longitud) </p>
   <p> unit azimut kiblat ialah dalam skyfield.Angle.degrees </p>
   <p> latitud dan longitud kaabah yang ditetapkan ialah 21.422487 Utara dan 39.826206 Timur. </p>
   <p> jejari Bumi yang digunakan ialah 6371000 meter </p>
   <p> formula yang digunakan ialah berdasarkan https://www.omnicalculator.com/other/azimuth</p>
   <hr>
```

### Comparing `EphemSahabatFalak-0.0.4/setup.py` & `EphemSahabatFalak-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak'
 LONG_DESCRIPTION = 'Sebuah pakej python yang menggunakan ephemeris dari JPL Horizon bagi menghasilkan hitungan falak'
 
 # Setting up
 setup(
     name="EphemSahabatFalak",
     version=VERSION,
```

