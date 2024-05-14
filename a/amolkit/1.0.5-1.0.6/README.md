# Comparing `tmp/amolkit-1.0.5.tar.gz` & `tmp/amolkit-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amolkit-1.0.5.tar", last modified: Mon Apr 15 21:49:28 2024, max compression
+gzip compressed data, was "amolkit-1.0.6.tar", last modified: Tue May 14 21:12:12 2024, max compression
```

## Comparing `amolkit-1.0.5.tar` & `amolkit-1.0.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-04-15 21:49:28.318029 amolkit-1.0.5/
--rw-r--r--   0 anmol     (1000) anmol     (1000)     1498 2023-06-06 15:10:15.000000 amolkit-1.0.5/LICENSE
--rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-04-15 21:49:28.318029 amolkit-1.0.5/PKG-INFO
--rw-r--r--   0 anmol     (1000) anmol     (1000)       56 2023-06-06 15:10:15.000000 amolkit-1.0.5/README.md
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-04-15 21:49:28.318029 amolkit-1.0.5/amolkit/
--rw-r--r--   0 anmol     (1000) anmol     (1000)    32064 2023-08-07 19:56:30.000000 amolkit-1.0.5/amolkit/EleInfo.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)        0 2023-06-06 15:27:54.000000 amolkit-1.0.5/amolkit/__init__.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    12188 2023-08-19 01:44:09.000000 amolkit-1.0.5/amolkit/amolsystem.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3406 2024-04-03 21:23:50.000000 amolkit-1.0.5/amolkit/atom.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     9095 2024-04-03 21:28:54.000000 amolkit-1.0.5/amolkit/genic.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3309 2023-08-10 06:31:01.000000 amolkit-1.0.5/amolkit/getEleInfo.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     2620 2024-04-06 23:08:42.000000 amolkit-1.0.5/amolkit/gethybridstate.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3032 2024-04-03 21:28:42.000000 amolkit-1.0.5/amolkit/getring.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)      313 2023-08-10 20:56:51.000000 amolkit-1.0.5/amolkit/misc.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    23176 2024-04-15 21:29:07.000000 amolkit-1.0.5/amolkit/molecule.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     8261 2023-08-10 20:42:44.000000 amolkit-1.0.5/amolkit/moltransform.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     8967 2023-08-19 01:39:50.000000 amolkit-1.0.5/amolkit/parameter.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    21118 2023-08-16 19:41:35.000000 amolkit-1.0.5/amolkit/psf.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3254 2023-08-16 19:17:38.000000 amolkit-1.0.5/amolkit/stringmanip.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    17660 2023-08-19 01:57:53.000000 amolkit-1.0.5/amolkit/topology.py
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-04-15 21:49:28.318029 amolkit-1.0.5/amolkit.egg-info/
--rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-04-15 21:49:28.000000 amolkit-1.0.5/amolkit.egg-info/PKG-INFO
--rw-r--r--   0 anmol     (1000) anmol     (1000)      480 2024-04-15 21:49:28.000000 amolkit-1.0.5/amolkit.egg-info/SOURCES.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2024-04-15 21:49:28.000000 amolkit-1.0.5/amolkit.egg-info/dependency_links.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2023-06-06 15:29:08.000000 amolkit-1.0.5/amolkit.egg-info/not-zip-safe
--rw-r--r--   0 anmol     (1000) anmol     (1000)        8 2024-04-15 21:49:28.000000 amolkit-1.0.5/amolkit.egg-info/top_level.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)       38 2024-04-15 21:49:28.318029 amolkit-1.0.5/setup.cfg
--rw-r--r--   0 anmol     (1000) anmol     (1000)      902 2024-04-15 21:43:38.000000 amolkit-1.0.5/setup.py
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-14 21:12:12.980649 amolkit-1.0.6/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     1498 2023-06-06 15:10:15.000000 amolkit-1.0.6/LICENSE
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-05-14 21:12:12.980649 amolkit-1.0.6/PKG-INFO
+-rw-r--r--   0 anmol     (1000) anmol     (1000)       56 2023-06-06 15:10:15.000000 amolkit-1.0.6/README.md
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-14 21:12:12.980649 amolkit-1.0.6/amolkit/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    32064 2023-08-07 19:56:30.000000 amolkit-1.0.6/amolkit/EleInfo.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        0 2023-06-06 15:27:54.000000 amolkit-1.0.6/amolkit/__init__.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    12188 2023-08-19 01:44:09.000000 amolkit-1.0.6/amolkit/amolsystem.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3948 2024-05-06 05:25:28.000000 amolkit-1.0.6/amolkit/atom.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     9095 2024-04-03 21:28:54.000000 amolkit-1.0.6/amolkit/genic.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     2713 2024-05-14 21:06:09.000000 amolkit-1.0.6/amolkit/getEleInfo.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     2620 2024-04-06 23:08:42.000000 amolkit-1.0.6/amolkit/gethybridstate.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3032 2024-04-03 21:28:42.000000 amolkit-1.0.6/amolkit/getring.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      313 2023-08-10 20:56:51.000000 amolkit-1.0.6/amolkit/misc.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    23122 2024-05-14 21:04:52.000000 amolkit-1.0.6/amolkit/molecule.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    24779 2024-05-14 21:01:09.000000 amolkit-1.0.6/amolkit/molecule2.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     8261 2023-08-10 20:42:44.000000 amolkit-1.0.6/amolkit/moltransform.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     8967 2023-08-19 01:39:50.000000 amolkit-1.0.6/amolkit/parameter.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    21118 2023-08-16 19:41:35.000000 amolkit-1.0.6/amolkit/psf.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3248 2024-05-14 21:01:31.000000 amolkit-1.0.6/amolkit/stringmanip.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    17639 2024-05-14 21:01:44.000000 amolkit-1.0.6/amolkit/topology.py
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-14 21:12:12.980649 amolkit-1.0.6/amolkit.egg-info/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-05-14 21:12:12.000000 amolkit-1.0.6/amolkit.egg-info/PKG-INFO
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      501 2024-05-14 21:12:12.000000 amolkit-1.0.6/amolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2024-05-14 21:12:12.000000 amolkit-1.0.6/amolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2023-06-06 15:29:08.000000 amolkit-1.0.6/amolkit.egg-info/not-zip-safe
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        8 2024-05-14 21:12:12.000000 amolkit-1.0.6/amolkit.egg-info/top_level.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)       38 2024-05-14 21:12:12.980649 amolkit-1.0.6/setup.cfg
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      902 2024-05-14 21:10:22.000000 amolkit-1.0.6/setup.py
```

### Comparing `amolkit-1.0.5/LICENSE` & `amolkit-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.5/amolkit/EleInfo.py` & `amolkit-1.0.6/amolkit/EleInfo.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.5/amolkit/amolsystem.py` & `amolkit-1.0.6/amolkit/amolsystem.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.5/amolkit/genic.py` & `amolkit-1.0.6/amolkit/genic.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.5/amolkit/gethybridstate.py` & `amolkit-1.0.6/amolkit/gethybridstate.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.5/amolkit/getring.py` & `amolkit-1.0.6/amolkit/getring.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.5/amolkit/molecule.py` & `amolkit-1.0.6/amolkit/molecule.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                 self.atomtfac_byIdx[ind] = tfac
                 segn = line[indexdict['segn'][0]:indexdict['segn'][1]].strip()
                 self.atomsegn_byIdx[ind] = segn 
                 ele = line[indexdict['ele'][0]:indexdict['ele'][1]].strip()
                 if ele:
                     self.atomele_byIdx[ind] = ele
                 else:
-                    self.atomele_byIdx[ind] = gei.atomsymbol_by_anyatomname(aname,bio)
+                    self.atomele_byIdx[ind] = gei.atomsymbol_by_atomname(aname,bio)
                 charge = line[indexdict['charge'][0]:indexdict['charge'][1]].strip()
                 if charge: 
                     self.atomcharge_byIdx[ind] = float(charge)
 
         # For single residue with all names different, populate the atomindex_byId
         allnames = list(map(lambda x:x.upper(), self.atomname_byIdx.values())) 
         if len(allnames) ==  len(list(set(allnames))):
@@ -203,15 +203,15 @@
                 else:
                     resid = int(line[indexdict['resid'][0]:indexdict['resid'][1]].strip())
                     self.atomresid_byIdx[ind] = resid 
                 resn = line[indexdict['resn'][0]:indexdict['resn'][1]].strip()
                 self.atomresn_byIdx[ind] = resn 
                 aname = line[indexdict['aname'][0]:indexdict['aname'][1]].strip()
                 self.atomname_byIdx[ind] = aname 
-                self.atomele_byIdx[ind] = gei.atomsymbol_by_anyatomname(aname,bio)
+                self.atomele_byIdx[ind] = gei.atomsymbol_by_atomname(aname,bio)
                 x=round(float(line[indexdict['x'][0]:indexdict['x'][1]].strip()),7)
                 y=round(float(line[indexdict['y'][0]:indexdict['y'][1]].strip()),7)
                 z=round(float(line[indexdict['z'][0]:indexdict['z'][1]].strip()),7)
                 self.atomcoord_byIdx[ind] = [x,y,z]
                 segn = line[indexdict['segn'][0]:indexdict['segn'][1]].strip()
                 self.atomsegn_byIdx[ind] = segn 
                 tfac = float(line[indexdict['tfac'][0]:indexdict['tfac'][1]].strip())
@@ -238,15 +238,15 @@
             if i == 1: continue # Second line is comment
             if len(field) >= 4:
                 ind += 1
                 srlno = int(istart) + ind
                 self.atomserial_byIdx[ind] = srlno
                 self.atomname_byIdx[ind] = field[0]
                 self.atomcoord_byIdx[ind] = list(map(lambda x:round(float(x),7), field[1:4]))
-                self.atomele_byIdx[ind] = gei.atomsymbol_by_anyatomname(field[0],bio)
+                self.atomele_byIdx[ind] = gei.atomsymbol_by_atomname(field[0],bio)
 
         # sanity check
         if self.nmolatoms != ind:
             raise ValueError("Found %d coordinates in %r but should be %d coordinates." % (self.nmolatoms, filename, ind))
 
         allnames = list(map(lambda x:x.upper(), self.atomname_byIdx.values())) 
         if len(allnames) ==  len(list(set(allnames))):
@@ -273,15 +273,15 @@
            coord = coordinates[:,i]
            delta[i] = coord - coord.reshape((len(coord),1))
     
         dist = delta[0]**2 + delta[1]**2 + delta[2]**2 + 10. * np.identity(len(coordinates))
     
         radius = []
         for el in elementnames:
-            radius.append(gei.covrad_by_atomsymbol(el)) 
+            radius.append(gei.covrad_by_atomname(el)) 
         radius = np.array(radius, dtype='float32')
     
         radcov = (radius + radius.reshape((len(radius),1)))*2
         bonded = np.array(np.where(dist - radcov<0.)).transpose()
         distmat = np.sqrt(dist[bonded[:,0],bonded[:,1]])
         
         # amolkit indices for molecules starts from 1
@@ -328,29 +328,29 @@
     if not isinstance(atomnames,list) and not isinstance(atomcoords,list):
         raise ValueError ("Provide list of atomnames and list of coords")
     if len(atomnames) != len(atomcoords):
         raise IndexError ("Length of atomnames and coords are not same.")
     
     resname = "RESN"; resid = 1; segname = "SEGN"
     if 'resname' in kwargs:
-       resname = resname if resname else "RESN"
+       resname = kwargs["resname"] 
     if 'resid' in kwargs:
-       resid = resid if resid else 1
+       resid = kwargs["resid"]
     if 'segname' in kwargs:
-       segname = segname if segname else "SEGN"
+       segname = kwargs["segname"]
 
     mol = Molecule()
     mol.nmolatoms = len(atomnames) 
     
     for i in range(len(atomnames)): 
         ind = i + 1
         mol.atomname_byIdx[ind] = atomnames[i]
         mol.atomcoord_byIdx[ind] = atomcoords[i] 
         mol.atomserial_byIdx[ind]= ind 
-        mol.atomele_byIdx[ind]   = gei.atomsymbol_by_anyatomname(atomnames[i]) 
+        mol.atomele_byIdx[ind]   = gei.atomsymbol_by_atomname(atomnames[i]) 
         mol.atomresn_byIdx[ind]  = resname
         mol.atomresid_byIdx[ind] = resid
         mol.atomsegn_byIdx[ind]  = segname 
     return mol
 
 def coordline(molecule,ind,serialnum=None,resid=None):
     '''
@@ -531,19 +531,19 @@
         self.topology = topology()
         self.topology.loadCharmmTopology(resname,resitopfile)
 
     def genRDMolTop(self):
         self.mol=Chem.RWMol()
         atid={}
         idat={}
-        atomicnumber_by_anyatomname
+        atomicnumber_by_atomname
         for i, aname in topology.atomname_byIdx.items():
             if aname[0]=="D" or aname[0:2] =="LP": continue
-            atomicnumber = gei.atomicnumber_by_anyatomname(aname) 
-            atomsymbol = gei.atomsymbol_by_anyatomname(aname) 
+            atomicnumber = gei.atomicnumber_by_atomname(aname) 
+            atomsymbol = gei.atomsymbol_by_atomname(aname) 
             idx = m.AddAtom(Chem.Atom(atomicnumber))
             atid.update({atomsymbol:idx})
             idat.update({idx:atomsymbol})
         for bond in self.bonds:
             self.mol.AddBond(atid[bond[0]], atid[bond[1]],Chem.BondType.SINGLE)
         try:
             Chem.SanitizeMol(self.mol)
```

### Comparing `amolkit-1.0.5/amolkit/moltransform.py` & `amolkit-1.0.6/amolkit/moltransform.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.5/amolkit/parameter.py` & `amolkit-1.0.6/amolkit/parameter.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.5/amolkit/psf.py` & `amolkit-1.0.6/amolkit/psf.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.5/amolkit/stringmanip.py` & `amolkit-1.0.6/amolkit/stringmanip.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
             end = i 
             break
 
     atomname=tmpatomname[start:end]
     return (atomname)
 
 def renumber(prevname,bio=True):
-    #atomsymbol=atomsymbol_by_anyatomname(atomname,bio)
-    #atomname=list(map(lambda x:gei.atomsymbol_by_anyatomname(x[0:4].strip(),bio),prevname))
+    #atomsymbol=atomsymbol_by_atomname(atomname,bio)
+    #atomname=list(map(lambda x:gei.atomsymbol_by_atomname(x[0:4].strip(),bio),prevname))
     atomname=list(map(lambda x:x[0:4].strip(),prevname))
     collect={}
     newname=[None]*len(atomname)
     for i,a in enumerate(atomname):
         if a not in collect.keys():
             collect[a]=[i]
         else:
```

### Comparing `amolkit-1.0.5/amolkit/topology.py` & `amolkit-1.0.6/amolkit/topology.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     def readCharmmTopology(resname,resitopfile,bio=True):
         '''
         Load the features of the residue based on topology file.
     
         Note::
         field[1] is atomname
         field[2] is atomtype
-        if bio is True then utilize gei.atomicmass_by_anyatomname upon atomtype
+        if bio is True then utilize gei.atomicmass_by_atomname upon atomtype
         to get atomicmass or symbol. This way I am not limited to predefined atomtypes in EleInfo.
     
-        atommass_byId[field[1]] = gei.atomicmass_by_anyatomname(field[2],bio)
-        atomele_byId[field[1]] = gei.atomsymbol_by_anyatomname(field[2],bio)
+        atommass_byId[field[1]] = gei.atomicmass_by_atomname(field[2],bio)
+        atomele_byId[field[1]] = gei.atomsymbol_by_atomname(field[2],bio)
     
         But if it false, then I should ideally get atomicmass by atomtype
         and in case an atomtype is missing, I should allow user to supply new atomtype and its correspondence.
     
         # Give some thought if bio is False. In that case, atomtype = MAG will not be converted to Mg
         # Thus it would not find Mg
         '''
@@ -111,18 +111,18 @@
                     continue
                 elif ftype == "ATOM" and len(fieldup) > 3: 
                     nat = nat + 1
                     topology['atomindex_byId'][fieldup[1]] = nat
                     topology['atomname_byIdx'][nat] = fieldup[1]    # Atomname stored as in str
                     topology['atomtype_byId'][fieldup[1]] = fieldup[2]  # Atomtype capitalized before storing
                     topology['atomcharge_byId'][fieldup[1]] = float(field[3])
-                    # Using atomicmass_by_anyatomname, but supplying atomtype
-                    # Because atomicmass_by_anyatomtype does a fixed conversion
-                    topology['atommass_byId'][fieldup[1]] = gei.atomicmass_by_anyatomname(field[2],bio)
-                    topology['atomele_byId'][fieldup[1]] = gei.atomsymbol_by_anyatomname(field[2],bio)
+                    # Using atomicmass_by_atomname, but supplying atomtype
+                    # Because atomicmass_by_atomtype does a fixed conversion
+                    topology['atommass_byId'][fieldup[1]] = gei.atomicmass_by_atomname(field[2],bio)
+                    topology['atomele_byId'][fieldup[1]] = gei.atomsymbol_by_atomname(field[2],bio)
                     topology['atomcharges'].append(float(field[3]))
                     topology['atompenalty_byId'][fieldup[1]],_ = getPenaltyfromString(comment)
     
                     if topology['atomnames'] and fieldup[1] in topology['atomnames']:
                         raise ValueError("Topology contains repeated atomname %s. Unable to load."%(field[1]))
                     else:
                         topology['atomnames'].append(fieldup[1])
```

### Comparing `amolkit-1.0.5/setup.py` & `amolkit-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
      with open("README.md","r") as f:
           long_description=f.read()
 except:
      long_description=""
      pass
 
 setup(name='amolkit', 
-      version='1.0.5', 
+      version='1.0.6', 
       description='Library for extracting molecule information', 
       long_description=long_description,
       url='https://github.com/anmolecule/amolkit', 
       author='Anmol Kumar', 
       author_email='anmolecule@gmail.com', 
       license='BSD 3-Clause "New" or "Revised" License',
       packages=find_packages(),
```

