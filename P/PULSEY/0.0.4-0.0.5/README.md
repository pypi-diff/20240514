# Comparing `tmp/PULSEY-0.0.4.tar.gz` & `tmp/pulsey-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PULSEY-0.0.4.tar", last modified: Fri Feb 16 20:15:41 2024, max compression
+gzip compressed data, was "pulsey-0.0.5.tar", last modified: Tue May 14 19:39:23 2024, max compression
```

## Comparing `PULSEY-0.0.4.tar` & `pulsey-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 aayala     (501) staff       (20)        0 2024-02-16 20:15:41.007382 PULSEY-0.0.4/
--rw-r--r--   0 aayala     (501) staff       (20)      490 2024-02-16 20:15:41.007135 PULSEY-0.0.4/PKG-INFO
-drwxr-xr-x   0 aayala     (501) staff       (20)        0 2024-02-16 20:15:41.005896 PULSEY-0.0.4/PULSEY/
--rw-r--r--   0 aayala     (501) staff       (20)    15452 2024-02-16 20:06:45.000000 PULSEY-0.0.4/PULSEY/PULSEY.py
--rw-r--r--   0 aayala     (501) staff       (20)       21 2024-01-24 17:51:01.000000 PULSEY-0.0.4/PULSEY/__init__.py
-drwxr-xr-x   0 aayala     (501) staff       (20)        0 2024-02-16 20:15:41.006927 PULSEY-0.0.4/PULSEY.egg-info/
--rw-r--r--   0 aayala     (501) staff       (20)      490 2024-02-16 20:15:41.000000 PULSEY-0.0.4/PULSEY.egg-info/PKG-INFO
--rw-r--r--   0 aayala     (501) staff       (20)      180 2024-02-16 20:15:41.000000 PULSEY-0.0.4/PULSEY.egg-info/SOURCES.txt
--rw-r--r--   0 aayala     (501) staff       (20)        1 2024-02-16 20:15:41.000000 PULSEY-0.0.4/PULSEY.egg-info/dependency_links.txt
--rw-r--r--   0 aayala     (501) staff       (20)        7 2024-02-16 20:15:41.000000 PULSEY-0.0.4/PULSEY.egg-info/top_level.txt
--rw-r--r--   0 aayala     (501) staff       (20)        9 2023-06-21 18:06:32.000000 PULSEY-0.0.4/README.md
--rw-r--r--   0 aayala     (501) staff       (20)      572 2024-02-16 20:15:26.000000 PULSEY-0.0.4/pyproject.toml
--rw-r--r--   0 aayala     (501) staff       (20)       38 2024-02-16 20:15:41.007433 PULSEY-0.0.4/setup.cfg
+drwxr-xr-x   0 aayala     (501) staff       (20)        0 2024-05-14 19:39:23.248553 pulsey-0.0.5/
+-rw-r--r--   0 aayala     (501) staff       (20)      490 2024-05-14 19:39:23.248387 pulsey-0.0.5/PKG-INFO
+drwxr-xr-x   0 aayala     (501) staff       (20)        0 2024-05-14 19:39:23.247473 pulsey-0.0.5/PULSEY/
+-rw-r--r--   0 aayala     (501) staff       (20)    16197 2024-05-14 19:38:01.000000 pulsey-0.0.5/PULSEY/PULSEY.py
+-rw-r--r--   0 aayala     (501) staff       (20)       21 2024-01-24 17:51:01.000000 pulsey-0.0.5/PULSEY/__init__.py
+drwxr-xr-x   0 aayala     (501) staff       (20)        0 2024-05-14 19:39:23.248221 pulsey-0.0.5/PULSEY.egg-info/
+-rw-r--r--   0 aayala     (501) staff       (20)      490 2024-05-14 19:39:23.000000 pulsey-0.0.5/PULSEY.egg-info/PKG-INFO
+-rw-r--r--   0 aayala     (501) staff       (20)      180 2024-05-14 19:39:23.000000 pulsey-0.0.5/PULSEY.egg-info/SOURCES.txt
+-rw-r--r--   0 aayala     (501) staff       (20)        1 2024-05-14 19:39:23.000000 pulsey-0.0.5/PULSEY.egg-info/dependency_links.txt
+-rw-r--r--   0 aayala     (501) staff       (20)        7 2024-05-14 19:39:23.000000 pulsey-0.0.5/PULSEY.egg-info/top_level.txt
+-rw-r--r--   0 aayala     (501) staff       (20)        9 2023-06-21 18:06:32.000000 pulsey-0.0.5/README.md
+-rw-r--r--   0 aayala     (501) staff       (20)      572 2024-05-14 19:37:14.000000 pulsey-0.0.5/pyproject.toml
+-rw-r--r--   0 aayala     (501) staff       (20)       38 2024-05-14 19:39:23.248588 pulsey-0.0.5/setup.cfg
```

### Comparing `PULSEY-0.0.4/PULSEY/PULSEY.py` & `pulsey-0.0.5/PULSEY/PULSEY.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,36 +7,29 @@
 utilizes these static maps to create a periodically pulsating stellar source by summing various spherical harmonic magnitude values
 over time.  
 """
 
 ### IMPORT PACKAGES ###
 import sys
 import os
-# sys.path.insert(0, '/Users/aayala/GitHub/starry')
 import starry
 starry.config.lazy = False
 starry.config.quiet = True
 
 import numpy as np
 import math as m
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import matplotlib.animation as animation
 from IPython.display import HTML
-import lightkurve as lk
 from tqdm import tqdm
-# import lmfit
 from PIL import Image
 import warnings
-#import healpy
-
-##Get/Set naming conventions
 
 ### Calculate position in CoeffArray of given L,M index
-
 #Function to determine postition of desire spherical harmonic mode coefficient in L-M array
 def lmIndex(l, m):
     return l*(l+1) + m
 
 #Function to calculate coefficients to construct standing wave pulsation from combining +/- m-modes
 def _LxMx(t, m, frequency=1,amp=1, phase0=0):
     """Construct pulsation coefficients of a single l-m spherical harmonic mode
@@ -101,108 +94,110 @@
         Star object with pulsation modes, frequencies, and amplitudes as indicated by user
 
     ### Example
     
     """
 
     #Init function taking freq, amp, etc. to initialize star with features
-    def __init__(self, lmMode, freq, amp, phase, inc=90, lMax = None, fcn = None, osParam = 2, observed = True):
+    def __init__(self, lmMode, freq, amp, phase, inc=90, obl = 0, lMax = None, fcn = None, osParam = 2, observed = True):
         #Insert warning if fcn given and no lMax provided (make sure its large enough)
         #See if we can change complexity (lMax) of map after initialization
         self.lmMode = lmMode
         self.freq = freq
         self.amp = amp
         self.phase = phase
         self.inc = inc
+        self.obl = obl
         self.fcn = fcn
         self.observed = observed
-
-        #Save Y2P from pixel transform as feature of star
+        self.nSignals = len(lmMode)
+        self.unphysical = False
         
-        #Provided lMax means we will transform surface output values SH-maps.  Need to carry along larger transform array.
+        #Provided lMax means we will transform surface output values SH-maps
         if(lMax is None):
             if(len(lmMode) > 0):
                 self.lMax = np.max(self.lmMode)
             else:
                 self.lMax = 0
         else:
             self.lMax = lMax
 
 
-        self.nSignals = len(self.lmMode)
-        self._map = starry.Map(ydeg=self.lMax, amp=1.0, inc = self.inc - 90)
+        self._map = starry.Map(ydeg=self.lMax, amp=1.0, inc = self.inc + 90, obl = self.obl)
         #Look into creating inclination function
 
-        self._computeAmpCoeffs() #Think about renaming
+        #Calculate
+        self._pulsationCorrections()
         #self.computeMapCoeffs()
-        #self._computeFlux()
+        #self.computePulsation([0])
 
         if self.fcn is not None:
             self.setTransFcn(self.fcn, osParam)
             self.lat, self.lon, self.Y2P, self.P2Y, self.Dx, self.Dy = self._map.get_pixel_transforms(oversample=osParam)
 
-    #Transform constructed stellar surface map to new values in accordance with input transform function
-    def setTransFcn(self, fcn):
-        """Set function for transforming surface map pixel magnitudes to desired values
-
-        ### Parameters
-
-        fcn : float (default = 1.0)
-            Equation to transform surface magnitudes to observable values
-        osParam: int (default = 2)
-            Degree to which surface map of star will be granulated to pixels. Higher value equals more pixels
-
-        ### Example
-        
-        """
-
-        #Translate lons/lats due to inclination of star
-        self.fcn = fcn
-        
-        # self.lat = self.lat-self.inc
 
     #Perform coefficient transform to retrieve necessary input amplitude map values in order to receive desired output amplitudes
-    def _computeAmpCoeffs(self):
+    def _pulsationCorrections(self):
         """Compute the amplitude coefficients for converting map values to desired observables
 
         ### Parameters
 
         ### Example
         Add example
         """
         # DESIRED amplitudes set to ampScaleFactor, transform if observed flag is true
         self.ampScaleFactor = np.ones(self.nSignals)
-        self.phaseOffsetArray = np.zeros(self.nSignals)
+        self._phaseOffsetArray = np.zeros(self.nSignals)
 
         #Sample map over arbitrary time to retrieve necessary amplitudes and phase to combine for constructing desired surfacd map
         for i in range(len(self.lmMode)):
-            timeSample = np.arange(0,1,0.25)
+            timeSample = np.arange(0.0,1.0,0.25)
             testFluxArray = np.zeros(len(timeSample))
             for j, t in enumerate(timeSample):
                 self._map.y[1:] = 0.0
                 l = self.lmMode[i][0]
                 m = self.lmMode[i][1]
-                posC,negC = _LxMx(t, m, frequency=1, amp=1.0, phase0=0)
+                posC,negC = _LxMx(t, m, frequency=1.0, amp=1.0, phase0=0)
                 self._map[l,np.abs(m)]  += posC
                 if m != 0:
                     self._map[l,-np.abs(m)] += negC
 
                 testFluxArray[j] = self._map.flux()
 
             #Save amp and phase coefficients for use in map construction
             maxAmp = np.nanmax(testFluxArray)
             maxAmp = maxAmp-1.0
             if self.observed:
                 self.ampScaleFactor[i] = 1.0/maxAmp
                 if(self.ampScaleFactor[i] > 1.0):
                     warnings.warn("WARNING: Producing unphysical amplitude values!")
                     
-            self.phaseOffsetArray[i] = (timeSample[np.argmax(testFluxArray)]-0.25)
+            self._phaseOffsetArray[i] = (timeSample[np.argmax(testFluxArray)]-0.25)
+
+    #Transform constructed stellar surface map to new values in accordance with input transform function
+    def setTransFcn(self, fcn):
+        """Set function for transforming surface map pixel magnitudes to desired values
+
+        ### Parameters
+
+        fcn : float (default = 1.0)
+            Equation to transform surface magnitudes to observable values
+        osParam: int (default = 2)
+            Degree to which surface map of star will be granulated to pixels. Higher value equals more pixels
+
+        ### Example
+        
+        """
+
+        #Translate lons/lats due to inclination of star
+        self.fcn = fcn
+        
+        # self.lat = self.lat-self.inc
+
 
-    #Compute coefficients necessary to construct surface maps for pulsation over given time sample
     #Compute coefficients necessary to construct surface maps for pulsation over given time sample
     def computePulsation(self, time):
         """Construct surface maps for every timestamp in the given time period
 
         ### Parameters
 
         timeArray : array_like (float, 1D)
@@ -220,28 +215,34 @@
         coeffArray = np.zeros((len(time),len(self._map.y)))
         coeffArray[:,0] = 1.0
         for i,t in enumerate(time):
             for j in range(self.nSignals):
                     l = self.lmMode[j][0]
                     m = self.lmMode[j][1]
                     posC,negC = _LxMx(t, m, frequency=self.freq[j],amp=self.amp[j]*self.ampScaleFactor[j], 
-                                        phase0=self.phase[j]+self.phaseOffsetArray[j])
+                                        phase0=self.phase[j]+self._phaseOffsetArray[j])
                     
                     #print(posC)
 
                     coeffArray[i,lmIndex(l, np.abs(m))] += posC
                     if m != 0:
                         coeffArray[i,lmIndex(l,-np.abs(m))] += negC
 
             if self.fcn is not None:
                 p = self.Y2P.dot(coeffArray[i,:])
                 newP = self.fcn(p)
                 coeffArray[i,:] = self.P2Y.dot(newP)
 
         return coeffArray
+    
+    def show(self, time=0, cmap="seismic_r", **kwargs):
+        coeffArray = self.computePulsation(time)
+        self._map.y[:] = coeffArray
+        self._map.show(grid = False, cmap=cmap, **kwargs)
+
 
     #Calculate flux of surface map pulsation over given time sample (time Array given HERE)
     def computeFlux(self, time, binaryIndicator=False):
         """Compute output flux of star object over input time array and save as feature of star
 
         ### Parameters
 
@@ -256,18 +257,21 @@
 
         fluxArray : array_like (float, 1D)
             Integrated disc flux values of star at each value of timeArray 
 
         ### Example
         
         """
+
+        if not hasattr(time, '__iter__'):
+                time = [time]
+
         coeffArray = self.computePulsation(time)
         fluxArray = np.zeros(len(time))
 
-
         if binaryIndicator == True:
             for i,t in enumerate(time):
                 self.sys.primary.map.y[1:] = coeffArray[i][1:]
                 fluxArray[i] = self.sys.flux(t)
 
         else:
             for i in range(len(time)):
@@ -275,15 +279,15 @@
                 fluxArray[i] = self._map.flux()
         
         return fluxArray
     
     #Internal starry dummy object
     
     #Construct binary system model using stellar pulsation source as primary and black source as secondary
-    def setBinarySystem(self, r1, m1, r2, m2, sbRatio, period, t0):
+    def setBinarySystem(self, r1, m1, r2, m2, sbRatio, period, t0, inc=90):
         """Inserts star within binary system with given paramater inputs
 
         ### Parameters
 
         r1 : float
             Radius of primary star
 
@@ -304,123 +308,146 @@
 
         ### Example
         
         """
 
         pri = starry.Primary(self._map, r=r1, m=m1, prot=np.inf)
             #starry.Primary(starry.Map(ydeg=primary.ydeg, inc=primary.inc, amp=amp1), r=r1, m=m1, prot=np.inf)
-        sec = starry.Secondary(starry.Map(ydeg=0, inc=0, amp=sbRatio), r=r2, m=m2, porb=period, prot=np.inf, t0=t0, inc=90)
+        sec = starry.Secondary(starry.Map(ydeg=0, inc=0, amp=sbRatio), r=r2, m=m2, porb=period, prot=np.inf, t0=t0, inc=inc)
 
         self.sys = starry.System(pri, sec)
 
+        # compute flux once to try to prime everything
+        _ = self.sys.flux(0)
 
 
-    #Function for computing flux map for SPECIFIC time instance and outputs map
-    # def setTime(self, time, binaryFlag):
-    #     """Construct surface map at specific time isntance and associate time value as a feature of star
-
-    #     ### Parameters
-
-    #     time : float
-    #         Time value last associated with given star object
-
-    #     binaryFlag : boolean (deafault = False)
-    #         Flag indicating whether star is in binary system
-        
-        
-    #     ### Returns
-
-    #     ### Example
-    #     Returns the desired output
-    #     """
-
-    #     _ = self.getFlux([time], binaryIndicator=binaryFlag)
-    #     #self.time = time
-
-    #Visualize should take a time parameter
-    def visualizeStar(self):
+    def visualizeStar(self, time):
         """Construct animated gif visualizing star's pulsation over specific time period
 
         ### Parameters
         
         ### Returns
 
         ### Example
         
         """
+
+        # Have user give start and end time, throw Nyquist warningaz7
+        if not hasattr(time, '__iter__'):
+                time = [time]
+        
+        for i,t in enumerate(time[:-1]):
+            for f in self.freq:
+                if (time[i+1]-time[i]) > 1.0/f :
+                    warnings.warn("WARNING: One or more periods skipped between timestamp frames")
+                    break
+
+
+
         fig = plt.figure(figsize=(5,5))
         ax = fig.add_subplot(1,1,1)
         ax.axis('off')
 
 #         norm = np.linalg.norm(fluxArray)
 #         normFluxArray = fluxArray/norm
         # print(np.min(normFluxArray))
         # print(np.max(normFluxArray))
         #vRange = np.nanmax(np.abs(self.coeffArray.flatten() - 1/np.pi))
         #vmid = 1.0/np.pi
 
+        
+
         # Render the surface values first
         rendered = []
-        for coeffs in tqdm(self.coeffArray[:,:]):
+        coeffArray = self.computePulsation(time)
+        
+        for coeffs in tqdm(coeffArray):
             self._map.y[:] = coeffs
             rendered.append(self._map.render())
 
         # Find most extreme surface brightness excursions for color bar
         vRange = np.nanmax(np.abs(np.array(rendered).flatten() - 1/np.pi))
         vmid = 1.0/np.pi
 
         # Plot individual frames for animation
         imList = []
         for render in rendered:
-            im = ax.imshow(render, cmap="seismic_r", animated=True, vmin = vmid-vRange, vmax = vmid+vRange)
+            im = ax.imshow(render, cmap="seismic_r", animated=True, vmin = vmid-vRange, vmax = vmid+vRange, origin = "lower")
             imList.append([im])
 
-        anim = animation.ArtistAnimation(fig, imList, interval = 50, blit=True)
-        writergif = animation.PillowWriter(fps=30)
-        anim.save('Pulsation.gif',writer=writergif)
-        display(HTML(anim.to_html5_video()))
+        anim = animation.ArtistAnimation(fig, imList, interval=50, blit=True)
+        # writergif = animation.PillowWriter(fps=30)
+        # gif = anim.save('Pulsation.gif',writer=writergif)
+        display(HTML(anim.to_jshtml()))
+        plt.close(fig)
+
+        # video = anim.to_html5_video() 
+        # # embedding for the video 
+        # html = display.HTML(video) 
+        # # draw the animation 
+        # display(html)
+        # #plt.show()
 
-    def visualizeBinary(self):
+    def visualizeBinary(self, time):
         fig = plt.figure(figsize=(5,5))
         ax = fig.add_subplot(1,1,1)
         ax.axis('off')
 
+        if not hasattr(time, '__iter__'):
+                time = [time]
+
+        coeffArray = self.computePulsation(time)
+
         rendered = []
-        for coeffs in tqdm(self.coeffArray[:,:]):
+        for coeffs in tqdm(coeffArray[:,:]):
             self._map.y[:] = coeffs
             rendered.append(self._map.render())
 
         # Find most extreme surface brightness excursions for color bar
         vRange = np.nanmax(np.abs(np.array(rendered).flatten() - 1/np.pi))
         vmid = 1.0/np.pi
         fileNames = []
         
-        for i in range(len(self.time)):
-            fileLength = int(np.ceil(np.log10(len(self.time))))
-            self.sys.primary.map.y[:] = self.coeffArray[i,:]
+        for i in range(len(time)):
+            fileLength = int(np.ceil(np.log10(len(time))))
+            self.sys.primary.map.y[:] = coeffArray[i,:]
             fileNames.append(f"./BinaryImages/{i:0{fileLength}}.png")
-            self.sys.show(t=self.time[i], figsize=(5, 5), cmap="seismic_r", file=fileNames[i])
+            self.sys.show(t=time[i], figsize=(5, 5), cmap="seismic_r", file=fileNames[i])
 
         
         frames = [Image.open(fileName).convert("RGBA") for fileName in fileNames]
         newFrames = []
 
         for frame in frames:
             newFrame = Image.new("RGBA", frames[0].size, "WHITE")
             newFrame.paste(frame,(0,0), frame)
             newFrame.convert('RGB')
             newFrames.append(newFrame)
 
         newFrames[0].save("Binary.gif", format="GIF", append_images=newFrames, save_all=True, duration = 50, loop=0)
 
+        anim = animation.ArtistAnimation(fig, newFrames, interval=50, blit=True)
+        display(HTML(anim.to_jshtml()))
+
         # anim = animation.ArtistAnimation(fig, frames, interval = 50, blit=True)
         # writergif = animation.PillowWriter(fps=30)
         # anim.save('Pulsation.gif',writer=writergif)
         # display(HTML(anim.to_html5_video()))
 
+    
+    def plot(self,var1,var2):
+        plt.figure(figsize=(10, 5))
+        plt.plot(var1, var2, lw=2, alpha = 1)
+        plt.scatter(var1, var2, color = 'black', alpha = 0.25, s = 10)
+        plt.title("Integrated Flux over Time of Random Pulsation")
+        #plt.xlim(0,1)
+        plt.xlabel("Time [s]", fontsize=20)
+        plt.ylabel("Flux [normalized]", fontsize=20)
+        plt.show()
+
 
 
 ### OLD STUFF (MAYBE DELETE) ###
 """
 
 # Loop to create true flux array using newly determined phase offset values
 for i,time in enumerate(timeArray):
```

### Comparing `PULSEY-0.0.4/pyproject.toml` & `pulsey-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PULSEY"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Andrew Ayala", email="andrew.ayala.2018@gmail.com" },
 ]
 description = "Stellar Pulsation Package"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

