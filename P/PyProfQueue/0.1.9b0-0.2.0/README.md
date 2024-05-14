# Comparing `tmp/PyProfQueue-0.1.9b0.tar.gz` & `tmp/PyProfQueue-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyProfQueue-0.1.9b0.tar", last modified: Tue Apr 16 13:59:54 2024, max compression
+gzip compressed data, was "PyProfQueue-0.2.0.tar", last modified: Tue May 14 15:11:31 2024, max compression
```

## Comparing `PyProfQueue-0.1.9b0.tar` & `PyProfQueue-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 13:59:54.295280 PyProfQueue-0.1.9b0/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5781 2024-04-16 13:59:54.295280 PyProfQueue-0.1.9b0/PKG-INFO
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 13:59:54.295280 PyProfQueue-0.1.9b0/PyProfQueue/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      330 2024-04-09 11:17:32.000000 PyProfQueue-0.1.9b0/PyProfQueue/__init__.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 13:59:54.295280 PyProfQueue-0.1.9b0/PyProfQueue/data/
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1382 2024-04-12 11:54:50.000000 PyProfQueue-0.1.9b0/PyProfQueue/data/likwid_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      886 2024-04-16 13:56:13.000000 PyProfQueue-0.1.9b0/PyProfQueue/data/prometheus_commands.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5627 2024-04-16 09:23:45.000000 PyProfQueue-0.1.9b0/PyProfQueue/data/read_prometheus.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    39168 2024-04-16 13:24:36.000000 PyProfQueue-0.1.9b0/PyProfQueue/script.py
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2367 2024-04-09 10:03:39.000000 PyProfQueue-0.1.9b0/PyProfQueue/submission.py
-drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-04-16 13:59:54.295280 PyProfQueue-0.1.9b0/PyProfQueue.egg-info/
--rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)     5781 2024-04-16 13:59:54.000000 PyProfQueue-0.1.9b0/PyProfQueue.egg-info/PKG-INFO
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      393 2024-04-16 13:59:54.000000 PyProfQueue-0.1.9b0/PyProfQueue.egg-info/SOURCES.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-04-16 13:59:54.000000 PyProfQueue-0.1.9b0/PyProfQueue.egg-info/dependency_links.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       48 2024-04-16 13:59:54.000000 PyProfQueue-0.1.9b0/PyProfQueue.egg-info/requires.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-04-16 13:59:54.000000 PyProfQueue-0.1.9b0/PyProfQueue.egg-info/top_level.txt
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5079 2024-04-16 10:31:11.000000 PyProfQueue-0.1.9b0/ReadMe.md
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-04-16 13:59:54.295280 PyProfQueue-0.1.9b0/setup.cfg
--rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1198 2024-04-16 13:59:49.000000 PyProfQueue-0.1.9b0/setup.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    19803 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/PKG-INFO
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/PyProfQueue/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      350 2024-05-07 13:36:25.000000 PyProfQueue-0.2.0/PyProfQueue/__init__.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    12690 2024-05-07 13:55:56.000000 PyProfQueue-0.2.0/PyProfQueue/plot.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/PyProfQueue/profilers/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       47 2024-05-14 13:24:22.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/__init__.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2340 2024-05-14 14:28:05.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/_template_profiler.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/PyProfQueue/profilers/data/
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      235 2024-05-14 13:59:27.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/data/_template_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1390 2024-05-14 13:39:52.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/data/likwid_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      880 2024-05-14 13:39:52.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/data/prometheus_commands.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     5629 2024-04-24 08:36:01.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/data/read_prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     3343 2024-05-14 14:33:04.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/likwid.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     3744 2024-05-14 14:28:08.000000 PyProfQueue-0.2.0/PyProfQueue/profilers/prometheus.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    38688 2024-05-14 15:10:36.000000 PyProfQueue-0.2.0/PyProfQueue/script.py
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     2126 2024-05-09 14:25:46.000000 PyProfQueue-0.2.0/PyProfQueue/submission.py
+drwxrwxr-x   0 marcuskeil  (1000) marcuskeil  (1000)        0 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/PyProfQueue.egg-info/
+-rw-r--r--   0 marcuskeil  (1000) marcuskeil  (1000)    19803 2024-05-14 15:11:31.000000 PyProfQueue-0.2.0/PyProfQueue.egg-info/PKG-INFO
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)      639 2024-05-14 15:11:31.000000 PyProfQueue-0.2.0/PyProfQueue.egg-info/SOURCES.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)        1 2024-05-14 15:11:31.000000 PyProfQueue-0.2.0/PyProfQueue.egg-info/dependency_links.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       56 2024-05-14 15:11:31.000000 PyProfQueue-0.2.0/PyProfQueue.egg-info/requires.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       12 2024-05-14 15:11:31.000000 PyProfQueue-0.2.0/PyProfQueue.egg-info/top_level.txt
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)    19079 2024-05-14 14:43:03.000000 PyProfQueue-0.2.0/ReadMe.md
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)       38 2024-05-14 15:11:31.446160 PyProfQueue-0.2.0/setup.cfg
+-rw-rw-r--   0 marcuskeil  (1000) marcuskeil  (1000)     1355 2024-05-14 14:30:49.000000 PyProfQueue-0.2.0/setup.py
```

### Comparing `PyProfQueue-0.1.9b0/PyProfQueue/data/likwid_commands.txt` & `PyProfQueue-0.2.0/PyProfQueue/profilers/data/likwid_commands.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,9 +14,10 @@
 echo 'Scalar MByte/s' >> ${LIK_OUTPUT}
 likwid-bench -t load -W N:8GB:${THREAD_COUNT} | grep 'MByte/s:' >> ${LIK_OUTPUT}
 echo 'SSE MByte/s' >> ${LIK_OUTPUT}
 likwid-bench -t load_sse -W N:8GB:${THREAD_COUNT} | grep 'MByte/s:' >> ${LIK_OUTPUT}
 echo 'AVX MByte/s' >> ${LIK_OUTPUT}
 likwid-bench -t load_avx -W N:8GB:${THREAD_COUNT} | grep 'MByte/s:' >> ${LIK_OUTPUT}
 # *=*
+sleep 1
 echo 'Program Performance' >> ${LIK_OUTPUT}
 grep -e 'MFLOP/s STAT' -e 'Operational intensity STAT' ${WORKING_DIR}/job_output_setup.txt >> ${LIK_OUTPUT}
```

### Comparing `PyProfQueue-0.1.9b0/PyProfQueue/data/prometheus_commands.txt` & `PyProfQueue-0.2.0/PyProfQueue/profilers/data/prometheus_commands.txt`

 * *Files 25% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # *=*
 ${PROMETHEUS_SOFTWARE}/prometheus/prometheus --config.file=${PROMETHEUS_SOFTWARE}/prometheus/prometheus.yml --storage.tsdb.path=${PROMETHEUS_RUNNING_DIR}/data > /dev/null 2>&1 &
 export PROMETHEUS_PID=$!
 ${PROMETHEUS_SOFTWARE}/node_exporter/node_exporter > /dev/null 2>&1 &
 export NODE_PID=$!
 # *=*
 export START_TIME=$(date +%s)
-sleep 15
+sleep 10
 # *=*
-sleep 15
+sleep 10
 export END_TIME=$(date +%s)
 export DURATION=$((${END_TIME} - ${START_TIME}))
-export START=$(date -d @${START_TIME} -u +"%Y-%m-%d %H:%M:%S")
-export END=$(date -d @${END_TIME} -u +"%Y-%m-%d %H:%M:%S")
+export START=$(date -d @${START_TIME} +"%Y-%m-%d %H:%M:%S")
+export END=$(date -d @${END_TIME} +"%Y-%m-%d %H:%M:%S")
 ${PROMETHEUS_PYTHON} ${PROFILE_SCRAPE}/read_prometheus.py -o "${PROMETHEUS_RUNNING_DIR}" -s "${START}" -e "${END}" -i "${PROMETHEUS_IP}"
 # *=*
 sleep 1
 kill -TERM ${NODE_PID}
 kill -TERM ${PROMETHEUS_PID}
 # *=*
 echo 'Run time: '$((${DURATION}/60/60))':'$((${DURATION}/60%60 ))':'$((${DURATION}%60))
```

### Comparing `PyProfQueue-0.1.9b0/PyProfQueue/data/read_prometheus.py` & `PyProfQueue-0.2.0/PyProfQueue/profilers/data/read_prometheus.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     cpu_usage_dict = prometheus_scrape(connection=api,
                                        command='100 - irate(node_cpu_seconds_total{mode="idle"}[1m])*100',
                                        begin=start_time, end=end_time,
                                        given_name='CPU Usage:', name_convention='cpu')
     Full_df = pandas_merge(dictionary=cpu_usage_dict)
 
     cpu_iowait_dict = prometheus_scrape(connection=api,
-                                        command='irate(node_cpu_seconds_total{mode="idle"}[1m])*100',
+                                        command='irate(node_cpu_seconds_total{mode="iowait"}[1m])*100',
                                         begin=start_time, end=end_time,
                                         given_name='CPU IO Wait:', name_convention='cpu')
     Full_df = pandas_merge(dictionary=cpu_iowait_dict, dataframe=Full_df)
 
     memory_dict = prometheus_scrape(connection=api,
                                     command='(node_memory_MemTotal_bytes-node_memory_MemAvailable_bytes)/(1000000000)',
                                     begin=start_time, end=end_time,
```

### Comparing `PyProfQueue-0.1.9b0/PyProfQueue/script.py` & `PyProfQueue-0.2.0/PyProfQueue/script.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,79 @@
 # Built in Modules
-from importlib import resources as impresources
+import importlib
 import itertools
 import sys
 # Local package imports
-from . import data
+
+# from . import profilers
 
 
 class Script:
     """
-        Bash class to read existing bash scripts, pull out the options and create new file to be submitted so the
-        work in the script gets profiled.
+    Class to read existing bash scripts, pull out the options and create an object that contains all the
+    queue options, bash options, and desired profiling methods to be injected
 
-        Parameters to initiate
-        ----------
-        queue_system : str
-            str of the queue system to be used. [sbatch, torque]
-        work_script : str
-            str of the path and name of the original bash script to be profiled
-        read_queue_system : str = None
-            str of the queue system that the work_script was written for, if not specified it is assumed
-            it is the same as queue_system. [sbatch, torque]
-        queue_options : dict = None
-            dictionary of options to be passed to the queue system.
-        likwid : bool = False
-            bool determining if likwid should be used to measure the performance such that a roofline
-            model can be plotted
-        likwid_req: list = None
-            list of the required lines that need to be added to a bash script in order to allow likwid
-            to be used. For example, lines that load the likwid module if modules is being used on the
-            system.
-        prometheus : bool = False
-            bool determining if prometheus should be used to measure the metrics of the node on which
-            the script is being run.
-        prometheus_req: list = None
-            list of the required lines that need to be added to a bash script in order to allow prometheus
-            to be used. In order to run prometheus this list will need at least one entry:
-                'export PROMETHEUS_SOFTWARE=<path to the Prometheus software to be used>'
-            with an optional entry to change the python executable to use by declaring:
-                'export PROMETHEUS_PYTHON=<path to the Python version to be used to scrape the prometheus database>'
-            any additional entries will be added, but are at users discretion
+    Parameters to initiate
+    ----------
+    queue_system : str
+        str of the queue system to be used. [sbatch, torque]
+    work_script : str
+        str of the path and name of the original bash script to be profiled
+    read_queue_system : str = None
+        str of the queue system that the work_script was written for, if not specified it is assumed
+        it is the same as queue_system. [sbatch, torque]
+    queue_options : dict = None
+        dictionary of options to be passed to the queue system.
+    profiling : dict = None
+        dictionary where keys are the name of the profiler to use, and the values are dictionaries containing
+        "requirements" or other optional commands depending on the profiler being used.
 
-        Notes
-        -----
-        The Script class is intended to manage the components necessary in order to take an existing bash script,
-        extract any options for a queue system it has, add any desired options, and initiate the information needed
-        for prometheus and likwid to perform their metric collections. This object can then be passed on to the
-        submit() function in order to create the profiling bash script and submit it to the queue that it is
-        designed to be submitted to.
+    Notes
+    -----
+    The Script class is intended to manage the components necessary in order to take an existing bash script,
+    extract any options for a queue system it has, add any desired options, and initiate the information needed
+    for prometheus and likwid to perform their metric collections. This object can then be passed on to the
+    submit() function in order to create the profiling bash script and submit it to the queue that it is
+    designed to be submitted to.
 
-        Adding new queue systems
-        -----
-        To add a new queue system, go to the sections marked Queue System specifics {1}, {2}, {3} and {4} in order to
-        follow the instructions there
+    Adding new queue systems
+    -----
+    To add a new queue system, go to the sections marked Queue System specifics {1}, {2}, {3} and {4} in order to
+    follow the instructions there
 
-        Examples
-        -------- # As of now this example doesn't apply to this class.
-        #>>> from PyProfQueue.script import Script
-        #>>> ProfileScript = Script(queue_system='slurm',
-                                    work_script='./example.sh',
-                                    read_queue_system='slurm',
-                                    likwid=True,
-                                    likwid_req=['module load oneAPI_comp',
-                                                'module load likwid'],
-                                    prometheus=True,
-                                    prometheus_req=['export PROMETHEUS_SOFTWARE=~/Software/prometheus'],
-                                    queue_options={'user': 'user_name'})
+    Examples
+    -------- # As of now this example doesn't apply to this class.
+    #>>> from PyProfQueue.script import Script
+    #>>> ProfileScript = Script(queue_system='slurm',
+                                work_script='./example.sh',
+                                read_queue_system='slurm',
+                                likwid=True,
+                                likwid_req=['module load oneAPI_comp',
+                                            'module load likwid'],
+                                prometheus=True,
+                                prometheus_req=['export PROMETHEUS_SOFTWARE=~/Software/prometheus'],
+                                queue_options={'user': 'user_name'})
     """
     def __init__(self, queue_system: str,
                  work_script: str,
                  read_queue_system: str = None,
                  queue_options: dict = None,
-                 likwid: bool = False, likwid_req: list = None,
-                 prometheus: bool = False, prometheus_ip: str = None, prometheus_req: list = None):
+                 profiling: dict = None
+                 ):
         if True:  # If statement added to allow for the collapse of the initiation of variables
             self.queue_system = queue_system
             self.work_script = work_script
             self.tmp_work_script = None
             self.tmp_profile_script = None
             self.works = None
             self.work_dir = None
-            self.likwid = likwid
-            self.likwid_file = None
-            self.likwid_initEndSplit = None
-            self.likwid_req = None
-            self.prometheus = prometheus
-            self.prometheus_ip = prometheus_ip
-            self.prometheus_file = None
-            self.prometheus_initEndSplit = None
+            self.profiling = profiling
+            self.at_execute = False  # boolean to see if a profiler is already used at the execution line.
             self.read_queue_system = read_queue_system
 
-        if self.likwid:
-            self.add_likwid(likwid_req)
-        if self.prometheus:
-            self.add_prometheus(prometheus_req)
-
         if bool(queue_options):
             self.obj_options = self.Options(queue_options)
         else:
             self.obj_options = self.Options()
 
         # Queue System specifics {1}
         '''
@@ -110,15 +86,15 @@
                 self.submission = '<terminal command to submit scripts>'
                 job_name = '<Variable to give Job Name>'
                 job_id = '<Variable to give Job ID>'
         
         - Second, add a case to 'match self.read_queue_system' with the format of:
             case '<queue name>'
                 self.read_option_start = '<Format of how to read queue options>'
-                options = self.option_pass()
+                options, self.works = self.read_script()
                 self.obj_options.<OBJ Option function name for this queue>_options(options)
                 self.outputvariable_convert(job_directory)
         
         Template 1:
         =====
         case '<queue_name>':
             self.option_start = ''
@@ -127,15 +103,15 @@
         =====
         Template 2:
         =====
         case '<queue_name>':
             self.read_option_start = ''
             read_job_name = '${}'
             read_job_id = '${}'
-            options = self.option_pass()
+            options, self.works = self.read_script()
             self.obj_options.<queue_name>_options(options)
             self.outputvariable_convert(job_name, job_id, read_job_name, read_job_id)
         =====
         -----
         '''
         # ==========================
         match self.queue_system:
@@ -151,20 +127,20 @@
 
             case _:
                 exit('No queue system chosen')
 
         match self.read_queue_system:
             case 'slurm':
                 self.read_option_start = '#SBATCH '
-                options = self.option_pass()
+                options, self.works = self.read_script()
                 self.obj_options.slurm_options(options)
                 self.outputvariable_convert()
             case 'torque':
                 self.read_option_start = '#PBS '
-                options = self.option_pass()
+                options, self.works = self.read_script()
                 self.obj_options.torque_options(options)
                 self.outputvariable_convert()
             case None:
                 if self.queue_system is None:
                     if self.obj_options.workdir is None:
                         self.obj_options.workdir = './'
                 elif queue_options is None:
@@ -174,51 +150,89 @@
 
             case _:
                 exit('Provided queue system, {}, is not supported in the initialisation '
                      '"match self.read_queue_system"'.format(self.read_queue_system))
         # ==========================
         self.obj_options.remove_empty_options()
 
-    def add_likwid(self, likwid_req):
-        self.likwid = True
-        self.likwid_file = impresources.files(data) / "likwid_commands.txt"
-        self.likwid_initEndSplit = -1
-        self.likwid_req = likwid_req
-
-    def add_prometheus(self, prometheus_req: list, prometheus_ip: str = None):
-        contains_ps = False
-        contains_pp = False
-        if prometheus_ip is not None:
-            self.prometheus_ip = prometheus_ip
-        if prometheus_req is not None:
-            for req in prometheus_req:
-                if 'PROMETHEUS_SOFTWARE' in req:
-                    contains_ps = True
-                    continue
-                if 'PROMETHEUS_PYTHON' in req:
-                    contains_pp = True
-                    continue
-                else:
-                    prometheus_req += ['export PROMETHEUS_PYTHON={}'.format(sys.executable)]
-                    contains_pp = True
-                    continue
+    def initialise_profiling(self, profiler, profilefile):
+        """
+        initialse_profiling is used to call the define_initialise() function of the different profilers
+        Parameters
+
+        ----------
+        profiler: str
+            name of the profiler to be used, must match the .py file name located in PyProfQueue.profilers
+                Currently supports: ["likwid", "prometheus"]
+        profilefile: io.TextIOWrapper
+            open profile file with write permissions.
+
+        Returns None
+        -------
+
+        """
+        if self.profiling[profiler] is None:
+            exit(f"Each profiling type, has to have a value that is not None. Profiling {profiler} "
+                 f"had a value of None")
         else:
-            prometheus_req = []
-        if not contains_pp:
-            prometheus_req += ['export PROMETHEUS_PYTHON={}'.format(sys.executable)]
-        if not contains_ps and self.prometheus_ip is None:
-            exit('When requesting prometheus profiling, prometheus_req must include "export PROMETHEUS_SOFTWARE=".')
-        self.prometheus = True
-        self.prometheus_file = impresources.files(data) / "prometheus_commands.txt"
-        self.prometheus_initEndSplit = -1
-        self.prometheus_req = prometheus_req
-
-    def option_pass(self):
-        options, self.works = self.read_script()
-        return options
+            module = ".profilers."+profiler
+            current_prof = importlib.import_module(module, package="PyProfQueue")
+            current_prof.define_initialise(profilefile=profilefile,
+                                           profilerdict=self.profiling[profiler])
+
+    def run_work_profiling(self, profiler, profilefile, bash_options):
+        """
+        run_work_profiling is used to call the define_run() function of the different profilers. This function makes
+        it so that the user specified bash script is executed using the chosen profiler. This can only occur once,
+        listing multiple profilers that rely on this functions will cause an error.
+
+        Parameters
+        ----------
+        profiler: str
+            name of the profiler to be used, must match the .py file name located in PyProfQueue.profilers
+            Currently supports: ["likwid", "prometheus"]
+        profilefile: io.TextIOWrapper
+            open profile file with write permissions.
+        bash_options: list
+            List of bash options to pass to the user defined bash script.
+
+        Returns None
+        -------
+
+        """
+        module = ".profilers."+profiler
+        current_prof = importlib.import_module(module, package="PyProfQueue")
+        if hasattr(current_prof, "define_run"):
+            if not self.at_execute:
+                current_prof.define_run(profilefile=profilefile,
+                                        bash_options=bash_options,
+                                        tmp_work_script=self.tmp_work_script)
+                self.at_execute = True
+            else:
+                exit(f"Multiple at execution profilers were defined. Failed when adding profiler {profiler}")
+
+    def end_profiling(self, profiler, profilefile):
+        """
+        end_profiling is used to call the define_end() function of the different profilers.
+
+        Parameters
+        ----------
+        profiler: str
+            name of the profiler to be used, must match the .py file name located in PyProfQueue.profilers
+                Currently supports: ["likwid", "prometheus"]
+        profilefile: io.TextIOWrapper
+            pen profile file with write permissions.
+
+        Returns
+        -------
+
+        """
+        module = ".profilers."+profiler
+        current_prof = importlib.import_module(module, package="PyProfQueue")
+        current_prof.define_end(profilefile=profilefile)
 
     # Queue System specifics {2}
     '''
     -----
     To add a new queue system, this section needs two things. First, a new case has to be created which handles a 
     file using the new queue system being read in, which then needs a nested case to translate the output variable
     to all other queue system formats to handle a file being written out. Second, the nested case of all older 
@@ -295,14 +309,21 @@
         self.obj_options.output = self.obj_options.output.replace(job_directory, <'<special format>' or job_directory>)
         working_dir = self.obj_options.output[:-4]
     =====
     -----
     '''
     # ==========================
     def outputvariable_convert(self):
+        """
+        outputvariable_convert converts the variables in a script that are queue specific for output files.
+
+        Returns None
+        -------
+
+        """
         match self.read_queue_system:
             case 'slurm':
                 match self.queue_system:
                     case 'slurm':
                         if self.obj_options.workdir is not None:
                             self.work_dir = self.obj_options.workdir\
                                 .replace('%x', '${SLURM_JOB_NAME}')\
@@ -363,31 +384,57 @@
                         else:
                             self.work_dir = self.obj_options.output[:-4]
                     case _:
                         exit('queue_system was unknown when translating from no queue '
                              'system to {}'.format(self.queue_system))
             case _:
                 exit('read_queue_system was unknown with value: {}'.format(self.read_queue_system))
+        return
     # ==========================
+
     class Options:
+        """
+        Class to read existing bash scripts, pull out the options and create an object that contains all the
+        queue options, bash options, and desired profiling methods to be injected
+
+        Parameters to initiate
+        ----------
+        queue_options: dict
+            dictionary containing all the queue options to be used. These will overwrite queue options inside the
+            user defined bash script.
+        """
         def __init__(self, queue_options: dict = None):
             self.user = None
             self.nodes = None
             self.cores = None
             self.tasks = None
             self.time = None
             self.partition = None
             self.account = None
             self.subname = None
             self.output = None
             self.workdir = None
             if queue_options is not None:
                 self.pass_options(queue_options)
 
-        def pass_options(self, stated_options):
+        def pass_options(self, stated_options: dict):
+            """
+            pass_options takes a dictionary containing all the queue options to be used. These will overwrite queue
+            options in the user defined bash script.
+
+            Parameters
+            ----------
+            stated_options: dict
+                dictionary containing all the queue options to be used. These will overwrite queue options inside the
+                user defined bash script.
+
+            Returns None
+            -------
+
+            """
             for key, value in stated_options.items():
                 match key:
                     case 'user':
                         self.user = value
                     case 'nodes':
                         self.nodes = value
                     case 'cores':
@@ -404,21 +451,29 @@
                         self.subname = value
                     case 'workdir':
                         self.workdir = value
                     case 'output':
                         self.output = value
                     case _:
                         exit('Unknown option value in key: {}, with value: {} passed to pass_options'.format(key, value))
+            None
 
         def remove_empty_options(self):
+            """
+            remove_empty_options removes all empty options from the Options object.
+
+            Returns None
+            -------
+            """
             empty_attributes = [a for a in dir(self) if (not a.startswith('__') and
                                                          not callable(getattr(self, a)) and
                                                          getattr(self, a) is None)]
             for attribute in empty_attributes:
                 delattr(self, attribute)
+            return
 
         # Queue System specifics {3}
         '''
         -----
         To add a new queue system, this section needs to have a new function declared.
         This function needs to take self and a dictionary of options. This dictionary will use the queue options
         from the bash script provided as keys, with the values being the declared options in the bash script.
@@ -604,15 +659,29 @@
                         else:
                             self.output = value
                     case _:
                         exit('Unknown option value in key: {}, with value: {} passed to torque_options'.format(key, value))
         # ==========================
 
     def change_options(self, queue_options: dict):
+        """
+        change_options allows users to change the options they specified, after initialising their object.
+
+        Parameters
+        ----------
+        queue_options: dict
+            dictionary containing all the queue options to be used. These will overwrite queue options inside the
+            user defined bash script.
+
+        Returns None
+        -------
+
+        """
         self.obj_options.pass_options(queue_options)
+        return
 
     # Queue System specifics {4}
     '''
     -----
     To add a new queue system one cases need to be added in this section.
     This case needs to have the following format:
         case <queue name>
@@ -711,14 +780,21 @@
                     case 'workdir':
                         return '-d '
                     case 'output':
                         return '-o '
     # ==========================
 
     def read_script(self):
+        """
+        read_script reads the user defined bash script and returns the options as a dictionary, and all the work
+        that is to be run as a list of strings.
+
+        Returns options (dict), work (list[str])
+        -------
+        """
         options = {}
         work = []
         with open(self.work_script, 'r') as script:
             for line in script.readlines():
                 if self.read_option_start in line:
                     if line[line.find("-"):][1:2] == '-':
                         option_end = line.find("-") + line[line.find("-"):].find('=')
@@ -735,159 +811,101 @@
                         option_value = line[option_end:option_value_end]
                     options[option_name] = option_value
                 else:
                     work += [line]
         return options, work
 
     def create_workfile(self):
+        """
+        create_workfile creates the work file based on the user defined bash script by simply removing the options.
+        This is not used, when the work script has no queue options.
+        Returns
+        -------
+
+        """
         with open(self.tmp_work_script, 'w') as workfile:
             workfile.seek(0)
             for line in self.works:
                 workfile.write(line)
         return
 
+
+    def add_options(self, profilefile):
+        """
+        add_options adds the queue options from the Script object to the profile file.
+        Parameters
+        ----------
+        profilefile: io.TextIOWrapper
+            open profile file with write access.
+        Returns None
+        -------
+
+        """
+        to_write = [a for a in dir(self.obj_options) if not a.startswith('__') and
+                    not callable(getattr(self.obj_options, a))]
+        for option in to_write:
+            if option is not None and option != 'workdir':
+                profilefile.write(self.option_start + self.option_converter(option) +
+                                  self.obj_options.__getattribute__(option) + '\n')
+        profilefile.write('\n')
+        return
+
     def create_profilefile(self, tmp_work_script='./tmp_workfile.sh',
                            tmp_profile_script='./tmp_profilefile.sh',
                            bash_options=['']):
+        """
+        create_profilefile uses the attributes of the Script object, and creates the temporary profile file that will
+        be submitted to the queue on behalf of the user.
+
+        Parameters
+        ----------
+        tmp_work_script: str
+            path and name of the temporary work file that should be created. This file is the user defined bash script
+            with any queue options removed.
+        tmp_profile_script: str
+            path and name of the temporary profile file that should be created. This will contain any profiling
+            initialisations, calls and terminations needed to profile the user defined work with the desired profiling
+            software.
+        bash_options: list[str]
+            list of bash options that should be passed to the user defined bash script.
+        Returns None
+        -------
+        """
         if self.read_queue_system is not None:
             self.tmp_work_script = tmp_work_script
             self.create_workfile()
         else:
             self.tmp_work_script = self.work_script
         self.tmp_profile_script = tmp_profile_script
-
         with open(self.tmp_profile_script, 'w') as profilefile:
             profilefile.seek(0)
             profilefile.write('#!/bin/bash\n')
             if self.queue_system is not None:
                 self.add_options(profilefile)
 
             profilefile.write('export WORKING_DIR={}\n'.format(self.work_dir))
             profilefile.write('if [ ! -d  "${WORKING_DIR}" ]; then\n')
             profilefile.write('  mkdir ${WORKING_DIR}\n')
             profilefile.write('fi\n')
             profilefile.write('cd ${WORKING_DIR}\n')
             profilefile.write('\n')
+            if self.profiling is not None:
+                for key in self.profiling.keys():
+                    self.initialise_profiling(key, profilefile)
 
-            if self.likwid:
-                self.init_likwid(profilefile)
+                for key in self.profiling.keys():
+                    self.run_work_profiling(key, profilefile, bash_options)
 
-            if self.prometheus:
-                self.init_prometheus(profilefile)
+                if not self.at_execute:
+                    self.run_work(profilefile, bash_options)
 
-            if self.likwid:
-                self.run_likwid(profilefile, bash_options)
+                for key in self.profiling.keys():
+                    self.end_profiling(key, profilefile)
             else:
                 self.run_work(profilefile, bash_options)
-
-            if self.prometheus:
-                self.end_prometheus(profilefile)
-
-            if self.likwid:
-                self.end_likwid(profilefile)
-
         return
 
-    def add_options(self, profilefile):
-        to_write = [a for a in dir(self.obj_options) if not a.startswith('__') and
-                    not callable(getattr(self.obj_options, a))]
-        for option in to_write:
-            if option is not None and option != 'workdir':
-                profilefile.write(self.option_start + self.option_converter(option) +
-                                  self.obj_options.__getattribute__(option) + '\n')
-        profilefile.write('\n')
-
     def run_work(self, profilefile, bash_options=['']):
         profilefile.write('bash {} {}\n'.format(self.tmp_work_script,
                                                 ' '.join(str(x) for x in bash_options)))
         profilefile.write('\n')
         return
-
-    def init_likwid(self, profilefile):
-        profilefile.write('# Likwid initialisation declarations\n')
-        for i in self.likwid_req:
-            profilefile.write(i)
-            profilefile.write('\n')
-        profilefile.write('\n')
-        profilefile.write('export LIKWID_RUNNING_DIR=${WORKING_DIR}/Likwid\n')
-        with open(self.likwid_file, 'r') as likwid_file:
-            for number, line in enumerate(likwid_file):
-                if line == '# *=*\n':
-                    self.likwid_initEndSplit = number + 1
-                    break
-                profilefile.write(line)
-        profilefile.write('# Likwid initialisation done\n')
-        profilefile.write('\n')
-
-    def run_likwid(self, profilefile, bash_options=['']):
-        profilefile.write('likwid-perfctr -g MEM_DP -f bash {} {}\n'.format(self.tmp_work_script,
-                                                                            ' '.join(str(x) for x in bash_options)))
-        profilefile.write('\n')
-        return
-
-    def end_likwid(self, profilefile):
-        profilefile.write('# Likwid final steps declarations\n')
-        with open(self.likwid_file, 'r') as likwid_file:
-            for line in itertools.islice(likwid_file, self.likwid_initEndSplit, None):
-                profilefile.write(line)
-        profilefile.write('# Likwid final steps done\n')
-        profilefile.write('\n')
-        return
-
-    def init_prometheus(self, profilefile):
-        profilefile.write('# Prometheus initialisation declarations\n')
-        if self.prometheus_ip is None:
-            profilefile.write("export PROMETHEUS_IP=http://localhost:9090\n")
-        else:
-            profilefile.write("export PROMETHEUS_IP={}\n".format(self.prometheus_ip))
-        for i in self.prometheus_req:
-            profilefile.write(i)
-            profilefile.write('\n')
-        profilefile.write('export PROMETHEUS_RUNNING_DIR=${WORKING_DIR}/Prometheus\n')
-        scrape_path = str(impresources.path(data, 'read_prometheus.py'))[:-19]
-        profilefile.write('export PROFILE_SCRAPE={}\n'.format(scrape_path))
-        profilefile.write('\n')
-        final_init_indicator = 2
-        if self.prometheus_ip is None:
-            read_indicators = [0, 1, 2]
-        else:
-            read_indicators = [0, 2]
-        indicator = 0
-        with open(self.prometheus_file, 'r') as prometheus_file:
-            for number, line in enumerate(prometheus_file):
-                if line == '# *=*\n' and indicator >= final_init_indicator:
-                    self.prometheus_initEndSplit = number + 1
-                    break
-                elif line == '# *=*\n':
-                    indicator += 1
-                    continue
-                if indicator in read_indicators:
-                    profilefile.write(line)
-        profilefile.write('# Prometheus initialisation done\n')
-        profilefile.write('\n')
-
-    def end_prometheus(self, profilefile):
-        profilefile.write('# Prometheus final steps declarations\n')
-        if self.prometheus_ip is None:
-            read_indicators = [0, 1, 2]
-        else:
-            read_indicators = [0, 2]
-        indicator = 0
-        with open(self.prometheus_file, 'r') as prometheus_file:
-            for line in itertools.islice(prometheus_file, self.prometheus_initEndSplit, None):
-                if line == '# *=*\n':
-                    indicator += 1
-                    continue
-                if indicator in read_indicators:
-                    profilefile.write(line)
-        profilefile.write('# Prometheus final steps done\n')
-        profilefile.write('\n')
-
-    def existing_init_prometheus(self, profilefile):
-        profilefile.write('# Prometheus initialisation for scraping existing instance')
-        for i in self.prometheus_req:
-            profilefile.write(i)
-            profilefile.write('\n')
-        profilefile.write('export PROMETHEUS_RUNNING_DIR=${WORKING_DIR}/Prometheus\n')
-
-    def existing_end_prometheus(self, profilefile):
-        profilefile.write('# Prometheus final steps for scraping existing instance')
```

### Comparing `PyProfQueue-0.1.9b0/PyProfQueue/submission.py` & `PyProfQueue-0.2.0/PyProfQueue/submission.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,52 +5,45 @@
 from .script import Script
 
 
 def submit(script: Script,
            tmp_work_script: str = './tmp_workfile.sh',
            tmp_profile_script: str = './tmp_profilefile.sh',
            bash_options: list = [''],
-           leave_scripts: bool = False,
-           verbose: bool = False,
+           leave_scripts: bool = True,
            test: bool = False):
     '''
-    Submission
+    Create the temporary profile file and temporary work script in order to submit them to the appropriate queuing
+    system.
+
     Parameters
     ----------
     script : pyprofbash.Script
         pyprofbash.Script created prior to submission.
     tmp_work_script : str = './tmp_workfile.sh'
         Optional Parameter to change the name of the temporary work script which should be the original script
         used to initiate the Script object, but all queue options should have been removed.
     tmp_profile_script : str = './tmp_profilefile.sh'
         Optional Parameter to change the name of the temporary profile script which will be submitted to the queue
     bash_options : list = ['']
         Optional parameter to add additional strings to the end of the call of the original work script in case
         that script has options it needs to have passed to it.
-    leave_scripts : bool = False
+    leave_scripts : bool = True
         If True, leave scripts after submission.
-    verbose : bool =  False
-        If True, steps taken will be printed to stdout.
+    test : bool =  False
+        If True, leaves scripts that are created, but does not submit them. Instead, it prints out the command it would
+        have used if it had submitted them.
     '''
     script.create_profilefile(tmp_work_script, tmp_profile_script, bash_options)
-    if verbose or test:
-        if verbose:
-            print('Submitting script to profile using the following command:')
-        if test:
-            print('The following command would be used to submit a job to the queue:')
-            print(' '.join([getattr(script, 'submission'), getattr(script, 'tmp_profile_script')]))
-    if not test:
+    if test:
+        print('The following command would be used to submit a job to the queue:')
+        print(' '.join([getattr(script, 'submission'), getattr(script, 'tmp_profile_script')]))
+    else:
         subprocess.run(' '.join([getattr(script, 'submission'), getattr(script, 'tmp_profile_script')]), shell=True)
         time.sleep(1)
 
-    if verbose or test:
-        print('Submitted script.')
-    if leave_scripts:
-        if verbose or test:
-            print('Leaving scripts after submission.')
+    if leave_scripts or test:
         return
     else:
-        subprocess.run('rm {}'.format(getattr(script, 'tmp_profile_script')), shell=True)
-        subprocess.run('rm {}'.format(getattr(script, 'tmp_work_script')), shell=True)
-        if verbose or test:
-            print('Removed temporary scripts after submission.')
+        subprocess.run(f'rm {tmp_profile_script}', shell=True)
+        subprocess.run(f'rm {tmp_work_script}', shell=True)
         return
```

### Comparing `PyProfQueue-0.1.9b0/setup.py` & `PyProfQueue-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "ReadMe.md").read_text()
 
 setup(
     name='PyProfQueue',
-    version='0.1.9b0',
+    version='0.2.0',
     url='https://github.com/Marcus-Keil/PyProfQueue',
     author='Marcus Keil',
     author_email='marcusk050291@gmail.com',
     license='MIT License',
     packages=['PyProfQueue'],
     package_dir={'PyProfQueue': 'PyProfQueue'},
-    package_data={'PyProfQueue': ['../ReadMe.md', 'data/*.txt', 'data/read_prometheus.py']},
+    package_data={'PyProfQueue': ['../ReadMe.md',
+                                  'profilers/*.py',
+                                  'profilers/data/*.txt',
+                                  'profilers/data/read_prometheus.py']},
     install_requires=[
         'numpy',
         'pytz',
+        'pyarrow',
         'promql_http_api==0.3.3',
         'pandas<=2.2.1',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',
```

