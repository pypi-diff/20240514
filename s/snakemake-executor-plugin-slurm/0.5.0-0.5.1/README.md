# Comparing `tmp/snakemake_executor_plugin_slurm-0.5.0.tar.gz` & `tmp/snakemake_executor_plugin_slurm-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_executor_plugin_slurm-0.5.0.tar", max compression
+gzip compressed data, was "snakemake_executor_plugin_slurm-0.5.1.tar", max compression
```

## Comparing `snakemake_executor_plugin_slurm-0.5.0.tar` & `snakemake_executor_plugin_slurm-0.5.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2024-05-07 18:57:25.612998 snakemake_executor_plugin_slurm-0.5.0/LICENSE
--rw-r--r--   0        0        0      319 2024-05-07 18:57:25.612998 snakemake_executor_plugin_slurm-0.5.0/README.md
--rw-r--r--   0        0        0     1151 2024-05-07 18:57:25.612998 snakemake_executor_plugin_slurm-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    20257 2024-05-07 18:57:25.612998 snakemake_executor_plugin_slurm-0.5.0/snakemake_executor_plugin_slurm/__init__.py
--rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 snakemake_executor_plugin_slurm-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-14 14:50:30.856810 snakemake_executor_plugin_slurm-0.5.1/LICENSE
+-rw-r--r--   0        0        0      319 2024-05-14 14:50:30.856810 snakemake_executor_plugin_slurm-0.5.1/README.md
+-rw-r--r--   0        0        0     1151 2024-05-14 14:50:30.856810 snakemake_executor_plugin_slurm-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    20551 2024-05-14 14:50:30.856810 snakemake_executor_plugin_slurm-0.5.1/snakemake_executor_plugin_slurm/__init__.py
+-rw-r--r--   0        0        0     1380 1970-01-01 00:00:00.000000 snakemake_executor_plugin_slurm-0.5.1/PKG-INFO
```

### Comparing `snakemake_executor_plugin_slurm-0.5.0/LICENSE` & `snakemake_executor_plugin_slurm-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_slurm-0.5.0/pyproject.toml` & `snakemake_executor_plugin_slurm-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-executor-plugin-slurm"
-version = "0.5.0"
+version = "0.5.1"
 description = "A Snakemake executor plugin for submitting jobs to a SLURM cluster."
 authors = [
     "Christian Meesters <meesters@uni-mainz.de>",
     "David Lähnemann <david.laehnemann@dkfz-heidelberg.de>",
     "Johannes Koester <johannes.koester@uni-due.de>",
 ]
 readme = "README.md"
```

### Comparing `snakemake_executor_plugin_slurm-0.5.0/snakemake_executor_plugin_slurm/__init__.py` & `snakemake_executor_plugin_slurm-0.5.1/snakemake_executor_plugin_slurm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
 
         active_jobs_ids = {job_info.external_jobid for job_info in active_jobs}
         active_jobs_seen_by_sacct = set()
         missing_sacct_status = set()
 
         # We use this sacct syntax for argument 'starttime' to keep it compatible
         # with slurm < 20.11
-        sacct_starttime = f"{datetime.now() - timedelta(days=2):%Y-%m-%dT%H:00}"
+        sacct_starttime = f"{datetime.now() - timedelta(days = 2):%Y-%m-%dT%H:00}"
         # previously we had
         # f"--starttime now-2days --endtime now --name {self.run_uuid}"
         # in line 218 - once v20.11 is definitively not in use any more,
         # the more readable version ought to be re-adapted
 
         # this code is inspired by the snakemake profile:
         # https://github.com/Snakemake-Profiles/slurm
@@ -289,15 +289,17 @@
                     # so we assume it is finished
                     self.report_job_success(j)
                     any_finished = True
                     active_jobs_seen_by_sacct.remove(j.external_jobid)
                 elif status in fail_stati:
                     msg = (
                         f"SLURM-job '{j.external_jobid}' failed, SLURM status is: "
-                        f"'{status}'"
+                        # message ends with '. ', because it is proceeded
+                        # with a new sentence
+                        f"'{status}'. "
                     )
                     self.report_job_error(j, msg=msg, aux_logs=[j.aux["slurm_logfile"]])
                     active_jobs_seen_by_sacct.remove(j.external_jobid)
                 else:  # still running?
                     yield j
 
             if not any_finished:
@@ -369,15 +371,15 @@
         returns a default account, if applicable
         else raises an error - implicetly.
         """
         if job.resources.get("slurm_account"):
             # here, we check whether the given or guessed account is valid
             # if not, a WorkflowError is raised
             self.test_account(job.resources.slurm_account)
-            return f" -A {job.resources.slurm_account}"
+            return f" -A '{job.resources.slurm_account}'"
         else:
             if self._fallback_account_arg is None:
                 self.logger.warning("No SLURM account given, trying to guess.")
                 account = self.get_account()
                 if account:
                     self.logger.warning(f"Guessed SLURM account: {account}")
                     self._fallback_account_arg = f" -A {account}"
@@ -436,15 +438,17 @@
             )
         except subprocess.CalledProcessError as e:
             raise WorkflowError(
                 f"Unable to test the validity of the given or guessed SLURM account "
                 f"'{account}' with sacctmgr: {e.stderr}"
             )
 
-        accounts = accounts.split()
+        # The set() has been introduced during review to eliminate
+        # duplicates. They are not harmful, but disturbing to read.
+        accounts = set(_.strip() for _ in accounts.split("\n") if _)
 
         if account not in accounts:
             raise WorkflowError(
                 f"The given account {account} appears to be invalid. Available "
                 f"accounts:\n{', '.join(accounts)}"
             )
```

### Comparing `snakemake_executor_plugin_slurm-0.5.0/PKG-INFO` & `snakemake_executor_plugin_slurm-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-executor-plugin-slurm
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Snakemake executor plugin for submitting jobs to a SLURM cluster.
 Home-page: https://github.com/snakemake/snakemake-executor-plugin-slurm
 License: MIT
 Keywords: snakemake,plugin,executor,cluster,slurm
 Author: Christian Meesters
 Author-email: meesters@uni-mainz.de
 Requires-Python: >=3.11,<4.0
```

