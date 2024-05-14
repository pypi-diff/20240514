# Comparing `tmp/funlab_sched-0.3.0-py3-none-any.whl.zip` & `tmp/funlab_sched-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 9514 bytes, number of entries: 12
+Zip file size: 9615 bytes, number of entries: 12
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 funlab/sched/__init__.py
 -rw-r--r--  2.0 fat      446 b- defN 80-Jan-01 00:00 funlab/sched/conf/plugin.toml
 -rw-r--r--  2.0 fat      308 b- defN 80-Jan-01 00:00 funlab/sched/conf/task.toml
--rw-r--r--  2.0 fat     8815 b- defN 80-Jan-01 00:00 funlab/sched/service.py
+-rw-r--r--  2.0 fat     9171 b- defN 80-Jan-01 00:00 funlab/sched/service.py
 -rw-r--r--  2.0 fat     4864 b- defN 80-Jan-01 00:00 funlab/sched/task.py
 -rw-r--r--  2.0 fat     2302 b- defN 80-Jan-01 00:00 funlab/sched/templates/args_dialog.html
--rw-r--r--  2.0 fat     2322 b- defN 80-Jan-01 00:00 funlab/sched/templates/tasks.html
--rw-r--r--  2.0 fat       64 b- defN 80-Jan-01 00:00 funlab_sched-0.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 fat     1095 b- defN 80-Jan-01 00:00 funlab_sched-0.3.0.dist-info/LICENSE
--rw-r--r--  2.0 fat      704 b- defN 80-Jan-01 00:00 funlab_sched-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 funlab_sched-0.3.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1002 b- defN 16-Jan-01 00:00 funlab_sched-0.3.0.dist-info/RECORD
-12 files, 22010 bytes uncompressed, 7816 bytes compressed:  64.5%
+-rw-r--r--  2.0 fat     2383 b- defN 80-Jan-01 00:00 funlab/sched/templates/tasks.html
+-rw-r--r--  2.0 fat       64 b- defN 80-Jan-01 00:00 funlab_sched-0.3.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 fat     1091 b- defN 80-Jan-01 00:00 funlab_sched-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 fat      727 b- defN 80-Jan-01 00:00 funlab_sched-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 funlab_sched-0.3.1.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1002 b- defN 16-Jan-01 00:00 funlab_sched-0.3.1.dist-info/RECORD
+12 files, 22446 bytes uncompressed, 7917 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: funlab/sched/templates/args_dialog.html
 Comment: 
 
 Filename: funlab/sched/templates/tasks.html
 Comment: 
 
-Filename: funlab_sched-0.3.0.dist-info/entry_points.txt
+Filename: funlab_sched-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: funlab_sched-0.3.0.dist-info/LICENSE
+Filename: funlab_sched-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: funlab_sched-0.3.0.dist-info/METADATA
+Filename: funlab_sched-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: funlab_sched-0.3.0.dist-info/WHEEL
+Filename: funlab_sched-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: funlab_sched-0.3.0.dist-info/RECORD
+Filename: funlab_sched-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## funlab/sched/service.py

```diff
@@ -1,214 +1,212 @@
-
-import logging
-import threading
-import time
-from dataclasses import fields
-from datetime import datetime, timedelta
-
-from apscheduler.events import (EVENT_ALL, EVENT_JOB_ADDED, EVENT_JOB_MODIFIED,
-                                EVENT_JOB_REMOVED, EVENT_SCHEDULER_PAUSED,
-                                EVENT_SCHEDULER_RESUMED,
-                                EVENT_SCHEDULER_SHUTDOWN, JobEvent,
-                                JobExecutionEvent, JobSubmissionEvent,
-                                SchedulerEvent)
-from apscheduler.job import Job
-from apscheduler.schedulers.background import BackgroundScheduler
-from flask import render_template, request
-from flask_login import login_required
-from funlab.core.appbase import _FlaskBase
-from funlab.core.plugin import ServicePlugin, load_plugins
-from funlab.core.menu import MenuItem
-from funlab.sched.task import SchedTask
-from funlab.utils import log
-
-mylogger = log.get_logger(__name__, level=logging.INFO)
-
-class SchedService(ServicePlugin):
-    def __init__(self, app:_FlaskBase, trace_job_status=True):
-        super().__init__(app)
-        self._task_lock = threading.Lock()
-        self._scheduler = BackgroundScheduler()
-        self.sched_tasks: dict[str, SchedTask] = {}
-        self._load_config()
-        self._load_tasks()
-        self.start_service()
-        self.register_routes()
-        if trace_job_status:
-            self._scheduler.add_listener(self._listener_all_event, EVENT_ALL)
-        mi = MenuItem(title='Sched Tasks',
-                icon='<svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-calendar-stats" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">\
-                        <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>\
-                        <path d="M11.795 21h-6.795a2 2 0 0 1 -2 -2v-12a2 2 0 0 1 2 -2h12a2 2 0 0 1 2 2v4"></path>\
-                        <path d="M18 14v4h4"></path>\
-                        <path d="M18 18m-4 0a4 4 0 1 0 8 0a4 4 0 1 0 -8 0"></path>\
-                        <path d="M15 3v4"></path>\
-                        <path d="M7 3v4"></path>\
-                        <path d="M3 11h16"></path>\
-                        </svg>',
-                href=f'/{self.name}/tasks', admin_only=True)
-        self.app.append_adminmenu(mi)
-
-    def _load_config(self):
-        self._scheduler.configure(**self.plugin_config.as_dict())
-
-    def _load_tasks(self):
-        """
-        Load the job from the plugin class.
-        """
-        tasks = load_plugins(group="funlab_sched_task")
-        for task in tasks.values():
-            task: SchedTask = task(self)
-            if (next_plan:=task.plan_schedule()):
-                task.task_def.update(next_plan)
-            job: Job = self._scheduler.get_job(task.id)
-            if not job:
-                job = self._scheduler.add_job(**task.task_def)
-                self._align_task_job(None, task, job)
-            else:
-                if task.task_def.get("replace_existing", False):
-                    job.modify(**task.task_def)
-                    pass
-            mylogger.info(f"Sched loaded task {task.id}")
-
-    def _align_task_job(self, old_task, new_task, new_job):
-        if old_task:
-            self.sched_tasks.pop(old_task.id, None)
-        if new_task and new_job:
-            new_task.id = new_job.id
-            setattr(new_task, "job", new_job)
-            self.sched_tasks[new_task.id] = new_task
-
-    def _listener_all_event(self, event):
-        """
-        keep tracing of job execution
-        """
-        # with self._task_lock:
-        time.sleep(1)
-        if isinstance(event, JobSubmissionEvent):
-            event: JobSubmissionEvent = event
-            self.sched_tasks[
-                event.job_id
-            ].last_status = (
-                f'summited:{event.scheduled_run_times[0].strftime("%y-%m-%d %H:%M:%S")}'
-            )
-        elif isinstance(event, JobExecutionEvent):
-            event: JobExecutionEvent = event
-            if event.exception:
-                self.sched_tasks[
-                    event.job_id
-                ].last_status = f'failed:{event.scheduled_run_time.strftime("%y-%m-%d %H:%M:%S")},{event.exception}'
-            else:
-                self.sched_tasks[event.job_id].last_status = (
-                    f'executed:{event.scheduled_run_time.strftime("%y-%m-%d %H:%M:%S")}'
-                    + (f"ret={event.retval}" if event.retval is not None else "")
-                )  # {'status': 'executed', 'time': event.scheduled_run_time, 'retval': event.retval}
-        elif isinstance(event, JobEvent):
-            event: JobEvent = event
-            # if event.code == EVENT_JOB_ADDED:
-            #     self.sched_tasks[event.job_id].last_status = 'added'
-            # elif event.code == EVENT_JOB_REMOVED:
-            #     self.sched_tasks[event.job_id].last_status = 'removed'
-
-        elif isinstance(event, SchedulerEvent):
-            if event.code == EVENT_SCHEDULER_PAUSED:
-                status = "Paused"
-            elif event.code == EVENT_SCHEDULER_RESUMED:
-                status = "Waiting"
-            elif event.code == EVENT_SCHEDULER_SHUTDOWN:
-                status = "Shutdown"
-            else:
-                status = ""
-            if status:
-                for task in self.sched_tasks.values():
-                    task.last_status = status
-
-    def register_routes(self):
-        @self.blueprint.route("/tasks", methods=["GET", "POST"])
-        @login_required
-        def tasks():
-            def run_task(task):
-                task_kwargs = {}
-                for field in fields(task):
-                    if arg_value := request.form.get(field.name, None):
-                        task_kwargs.update({field.name: arg_value})
-                job = self._scheduler.get_job(task_id)
-                if job:
-                    job.modify(
-                        next_run_time=datetime.now() + timedelta(seconds=1),
-                        kwargs=task_kwargs,
-                    )
-                else:
-                    task.task_def.update({"kwargs": task_kwargs})
-                    task.task_def.update(
-                        {"next_run_time": datetime.now() + timedelta(seconds=1)}
-                    )
-                    job = self._scheduler.add_job(**task.task_def)
-                    self._align_task_job(task, task, job)
-
-            if task_id:=request.form.get('id'):
-                run_task(self.sched_tasks[task_id])
-            forms = {}
-            for task in self.sched_tasks.values():
-                form = request.form if (request.form and task.id in request.form) else None
-                if formcls := task.generate_params_formclass():
-                    forms[task.id] = formcls(formdata=form)  # task.form_class(formdata=form)
-            return render_template(
-                "tasks.html", tasks=self.sched_tasks.values(), forms=forms
-            )
-
-    @property
-    def running(self):
-        """Get true whether the scheduler is running."""
-        return self._scheduler.running
-
-    @property
-    def state(self):
-        """Get the state of the scheduler."""
-        return self._scheduler.state
-
-    @property
-    def scheduler(self):
-        return self._scheduler
-
-    @property
-    def task(self):
-        """Get the base scheduler decorator"""
-        return self._scheduler.scheduled_job
-
-    def start_service(self, paused=False):
-        """Start the configured executors and job stores and begin processing scheduled jobs.
-        Args:
-            paused (bool, optional): if True, don't start job processing until resume is called. Defaults to False.
-        """
-        self._scheduler.start(paused=paused)
-
-    def stop_service(self, wait=True):
-        """Shuts down the scheduler, along with its executors and job stores. Does not interrupt any currently running jobs.
-        Args:
-            wait (bool, optional): True to wait until all currently executing jobs have finished. Defaults to True.
-        """
-        self._scheduler.shutdown(wait)
-
-    def restart_service(self, wait=True):
-        self.stop_service(wait=wait)
-        self.start_service()
-
-    def reload_service(self, wait=True):
-        self.stop_service(wait=wait)
-        self._load_config()
-        self._load_tasks()
-        self.start_service()
-
-    def pause(self):
-        """
-        Pause job processing in the scheduler.
-        This will prevent the scheduler from waking up to do job processing until :meth:`resume`
-        is called. It will not however stop any already running job processing.
-        """
-        self._scheduler.pause()
-
-    def resume(self):
-        """
-        Resume job processing in the scheduler.
-        """
-        self._scheduler.resume()
+
+import logging
+import threading
+import time
+from dataclasses import fields
+from datetime import datetime, timedelta
+
+from apscheduler.events import (EVENT_ALL, EVENT_JOB_ADDED, EVENT_JOB_MODIFIED,
+                                EVENT_JOB_REMOVED, EVENT_SCHEDULER_PAUSED,
+                                EVENT_SCHEDULER_RESUMED,
+                                EVENT_SCHEDULER_SHUTDOWN, JobEvent,
+                                JobExecutionEvent, JobSubmissionEvent,
+                                SchedulerEvent)
+from apscheduler.job import Job
+from apscheduler.schedulers.background import BackgroundScheduler
+from flask import render_template, request
+from flask_login import login_required
+from funlab.core.appbase import _FlaskBase
+from funlab.core.plugin import ServicePlugin, load_plugins
+from funlab.core.menu import MenuItem
+from funlab.sched.task import SchedTask
+from funlab.utils import log
+
+class SchedService(ServicePlugin):
+    def __init__(self, app:_FlaskBase, trace_job_status=True):
+        super().__init__(app)
+        self._task_lock = threading.Lock()
+        self._scheduler = BackgroundScheduler()
+        self.sched_tasks: dict[str, SchedTask] = {}
+        self._load_config()
+        self._load_tasks()
+        self.start_service()
+        self.register_routes()
+        if trace_job_status:
+            self._scheduler.add_listener(self._listener_all_event, EVENT_ALL)
+        mi = MenuItem(title='Sched Tasks',
+                icon='<svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-calendar-stats" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">\
+                        <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>\
+                        <path d="M11.795 21h-6.795a2 2 0 0 1 -2 -2v-12a2 2 0 0 1 2 -2h12a2 2 0 0 1 2 2v4"></path>\
+                        <path d="M18 14v4h4"></path>\
+                        <path d="M18 18m-4 0a4 4 0 1 0 8 0a4 4 0 1 0 -8 0"></path>\
+                        <path d="M15 3v4"></path>\
+                        <path d="M7 3v4"></path>\
+                        <path d="M3 11h16"></path>\
+                        </svg>',
+                href=f'/{self.name}/tasks', admin_only=True)
+        self.app.append_adminmenu(mi)
+
+    def _load_config(self):
+        self._scheduler.configure(**self.plugin_config.as_dict())
+
+    def _load_tasks(self):
+        """
+        Load the job from the plugin class.
+        """
+        tasks = load_plugins(group="funlab_sched_task")
+        no_leading_logger=log.get_logger('', fmt=log.LogFmtType.EMPTY, level=logging.INFO)
+        no_leading_logger.info('')  # default plugin loading info without newline, so to let subtask log.info to start from new line
+        for task in tasks.values():
+            self.mylogger.info(f"Loading task {task} ...", end='')
+            task: SchedTask = task(self)
+            if (next_plan:=task.plan_schedule()):
+                task.task_def.update(next_plan)
+            job: Job = self._scheduler.get_job(task.id)
+            if not job:
+                job = self._scheduler.add_job(**task.task_def)
+                self._align_task_job(None, task, job)
+            else:
+                if task.task_def.get("replace_existing", False):
+                    job.modify(**task.task_def)
+            no_leading_logger.info('Done')
+
+
+    def _align_task_job(self, old_task, new_task, new_job):
+        if old_task:
+            self.sched_tasks.pop(old_task.id, None)
+        if new_task and new_job:
+            new_task.id = new_job.id
+            setattr(new_task, "job", new_job)
+            self.sched_tasks[new_task.id] = new_task
+
+    def _listener_all_event(self, event):
+        """
+        keep tracing of job execution
+        """
+        if isinstance(event, JobSubmissionEvent):
+            event: JobSubmissionEvent = event
+            self.sched_tasks[
+                event.job_id
+            ].last_status = (
+                f'summited:{event.scheduled_run_times[0].strftime("%y-%m-%d %H:%M:%S")}'
+            )
+        elif isinstance(event, JobExecutionEvent):
+            event: JobExecutionEvent = event
+            if event.exception:
+                self.sched_tasks[
+                    event.job_id
+                ].last_status = f'failed:{event.scheduled_run_time.strftime("%y-%m-%d %H:%M:%S")},{event.exception}'
+            else:
+                self.sched_tasks[event.job_id].last_status = (
+                    f'executed:{event.scheduled_run_time.strftime("%y-%m-%d %H:%M:%S")}'
+                    + (f"ret={event.retval}" if event.retval is not None else "")
+                )  # {'status': 'executed', 'time': event.scheduled_run_time, 'retval': event.retval}
+        # elif isinstance(event, JobEvent):
+        #     event: JobEvent = event
+        #     if event.code == EVENT_JOB_ADDED:
+        #         self.sched_tasks[event.job_id].last_status = 'added'
+        #     elif event.code == EVENT_JOB_REMOVED:
+        #         self.sched_tasks[event.job_id].last_status = 'removed'
+        elif isinstance(event, SchedulerEvent):
+            if event.code == EVENT_SCHEDULER_PAUSED:
+                status = "Paused"
+            elif event.code == EVENT_SCHEDULER_RESUMED:
+                status = "Waiting"
+            elif event.code == EVENT_SCHEDULER_SHUTDOWN:
+                status = "Shutdown"
+            else:
+                status = ""
+            if status:
+                for task in self.sched_tasks.values():
+                    task.last_status = status
+
+    def register_routes(self):
+        @self.blueprint.route("/tasks", methods=["GET", "POST"])
+        @login_required
+        def tasks():
+            def run_task(task):
+                task_kwargs = {}
+                for field in fields(task):
+                    if arg_value := request.form.get(field.name, None):
+                        task_kwargs.update({field.name: arg_value})
+                job = self._scheduler.get_job(task_id)
+                if job:
+                    job.modify(
+                        next_run_time=datetime.now() + timedelta(seconds=1),
+                        kwargs=task_kwargs,
+                    )
+                else:
+                    task.task_def.update({"kwargs": task_kwargs})
+                    task.task_def.update(
+                        {"next_run_time": datetime.now() + timedelta(seconds=1)}
+                    )
+                    job = self._scheduler.add_job(**task.task_def)
+                    self._align_task_job(task, task, job)
+
+            if task_id:=request.form.get('id'):
+                run_task(self.sched_tasks[task_id])
+            forms = {}
+            for task in self.sched_tasks.values():
+                form = request.form if (request.form and task.id in request.form) else None
+                if formcls := task.generate_params_formclass():
+                    forms[task.id] = formcls(formdata=form)  # task.form_class(formdata=form)
+            return render_template(
+                "tasks.html", tasks=self.sched_tasks.values(), forms=forms
+            )
+
+    @property
+    def running(self):
+        """Get true whether the scheduler is running."""
+        return self._scheduler.running
+
+    @property
+    def state(self):
+        """Get the state of the scheduler."""
+        return self._scheduler.state
+
+    @property
+    def scheduler(self):
+        return self._scheduler
+
+    @property
+    def task(self):
+        """Get the base scheduler decorator"""
+        return self._scheduler.scheduled_job
+
+    def start_service(self, paused=False):
+        """Start the configured executors and job stores and begin processing scheduled jobs.
+        Args:
+            paused (bool, optional): if True, don't start job processing until resume is called. Defaults to False.
+        """
+        self._scheduler.start(paused=paused)
+
+    def stop_service(self, wait=True):
+        """Shuts down the scheduler, along with its executors and job stores. Does not interrupt any currently running jobs.
+        Args:
+            wait (bool, optional): True to wait until all currently executing jobs have finished. Defaults to True.
+        """
+        self._scheduler.shutdown(wait)
+
+    def restart_service(self, wait=True):
+        self.stop_service(wait=wait)
+        self.start_service()
+
+    def reload_service(self, wait=True):
+        self.stop_service(wait=wait)
+        self._load_config()
+        self._load_tasks()
+        self.start_service()
+
+    def pause(self):
+        """
+        Pause job processing in the scheduler.
+        This will prevent the scheduler from waking up to do job processing until :meth:`resume`
+        is called. It will not however stop any already running job processing.
+        """
+        self._scheduler.pause()
+
+    def resume(self):
+        """
+        Resume job processing in the scheduler.
+        """
+        self._scheduler.resume()
```

## funlab/sched/templates/tasks.html

 * *Ordering differences only*

```diff
@@ -1,61 +1,61 @@
-{% extends "layouts/base.html" %}
-{% block page_header %}
-<div class="container-xl">
-    <div class="row g-2 align-items-center">
-        <div class="col">
-            <h2 class="page-title">
-                Defined Tasks
-            </h2>
-        </div>
-    </div>
-</div>
-{% endblock page_header %}
-
-{% block page_body %}
-<div class="container-xl">
-    <div class="row row-deck row-cards">
-        <div class="col-12">
-            <div class="card card-sm">
-                <div class="card-header">
-                </div>
-                <div class="card-body">
-                    <table class="table table-centered mb-0 rounded">
-                        <thead>
-                            <tr>
-                                <th>Id</th>
-                                <th>Last Status</th>
-                                <th>Next Run</th>
-                                <!-- <th>Func</th> -->
-                                <th>Trigger</th>
-                                <!-- <th>Misfire Grace Time</th> -->
-                                <th>Max Instances</th>
-                            </tr>
-                        </thead>
-                        <tbody>
-                            <!-- Item -->
-                            {% for task in tasks %}
-                            <tr>
-                                <td><a href="#" data-bs-toggle="modal"
-                                        data-bs-target="#{{task.id}}_args-form">{{task.name}}</a></td>
-                                <td style="width:25%;word-break:break-word">{{task.last_status}}</td>
-                                <td>{{task.next_run_time}}</td>
-                                <!-- <td>{{task.func_ref}}</td> -->
-                                <td style="width:25%;word-break:break-word">{{task.trigger}}</td>
-                                <!-- <td>{{task.misfire_grace_time}}</td> -->
-                                <td>{{task.max_instances}}</td>
-                            </tr>
-                            {% endfor %}
-                            <!-- End of Item -->
-                        </tbody>
-                    </table>
-                </div>
-            </div>
-        </div>
-    </div>
-</dev>
-{% endblock page_body %}
-
-{% block modal_dialog %}
-{% include 'args_dialog.html' %}
-{% endblock modal_dialog %}
-
+{% extends "layouts/base.html" %}
+{% block page_header %}
+<div class="container-xl">
+    <div class="row g-2 align-items-center">
+        <div class="col">
+            <h2 class="page-title">
+                Defined Tasks
+            </h2>
+        </div>
+    </div>
+</div>
+{% endblock page_header %}
+
+{% block page_body %}
+<div class="container-xl">
+    <div class="row row-deck row-cards">
+        <div class="col-12">
+            <div class="card card-sm">
+                <div class="card-header">
+                </div>
+                <div class="card-body">
+                    <table class="table table-centered mb-0 rounded">
+                        <thead>
+                            <tr>
+                                <th>Id</th>
+                                <th>Last Status</th>
+                                <th>Next Run</th>
+                                <!-- <th>Func</th> -->
+                                <th>Trigger</th>
+                                <!-- <th>Misfire Grace Time</th> -->
+                                <th>Max Instances</th>
+                            </tr>
+                        </thead>
+                        <tbody>
+                            <!-- Item -->
+                            {% for task in tasks %}
+                            <tr>
+                                <td><a href="#" data-bs-toggle="modal"
+                                        data-bs-target="#{{task.id}}_args-form">{{task.name}}</a></td>
+                                <td style="width:25%;word-break:break-word">{{task.last_status}}</td>
+                                <td>{{task.next_run_time}}</td>
+                                <!-- <td>{{task.func_ref}}</td> -->
+                                <td style="width:25%;word-break:break-word">{{task.trigger}}</td>
+                                <!-- <td>{{task.misfire_grace_time}}</td> -->
+                                <td>{{task.max_instances}}</td>
+                            </tr>
+                            {% endfor %}
+                            <!-- End of Item -->
+                        </tbody>
+                    </table>
+                </div>
+            </div>
+        </div>
+    </div>
+</dev>
+{% endblock page_body %}
+
+{% block modal_dialog %}
+{% include 'args_dialog.html' %}
+{% endblock modal_dialog %}
+
```

## Comparing `funlab_sched-0.3.0.dist-info/LICENSE` & `funlab_sched-0.3.1.dist-info/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023-2024 Sunny Lin(013)
+Copyright (c) 2023- Sunny Lin(013)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `funlab_sched-0.3.0.dist-info/METADATA` & `funlab_sched-0.3.1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: funlab-sched
-Version: 0.3.0
-Summary: 
+Version: 0.3.1
+Summary: A funlab-flaskr service plugin provide task scheduling, using APScheduler.
 Author: sunny
 Author-email: 013.lin@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: apscheduler (>=3.10.1,<4.0.0)
 Requires-Dist: flask-wtf (>=1.2.1,<2.0.0)
 Requires-Dist: funlab-flaskr (>=0.3.1,<0.4.0)
 Description-Content-Type: text/markdown
 
 # A funlab-flaskr plugin provide tasks scheduling using APScheculer
```

## Comparing `funlab_sched-0.3.0.dist-info/RECORD` & `funlab_sched-0.3.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 funlab/sched/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funlab/sched/conf/plugin.toml,sha256=wEySCFZ8KGUWDw5iexY0uml6168eKJ01URTvJyNJ7AI,446
 funlab/sched/conf/task.toml,sha256=ELlsMS9RUCZCfRE2F5_9jjSkKMz393gfFc4ujaTUYno,308
-funlab/sched/service.py,sha256=J78-0vaCtvsdA5vCbeah5Wkd5iqQuQUHbDWmNb9tIq8,8815
+funlab/sched/service.py,sha256=hBUD6Dmw3DvYCPKE02ky8sNHRjiNeKnj9mDhD5JJnxk,9171
 funlab/sched/task.py,sha256=-IgQ_rOthLEbZkNiIJotPIQ2s9RomzebG2TersdPBYo,4864
 funlab/sched/templates/args_dialog.html,sha256=OsGjbzdtAA2R6unuBxfvLERP03Bf51z9j9gtP6tNphQ,2302
-funlab/sched/templates/tasks.html,sha256=fOlPX3-gqwo97vv_N91aXt5VVzlxETefZkiwjJGevf0,2322
-funlab_sched-0.3.0.dist-info/entry_points.txt,sha256=gLwkuvZnCAY-q3VVxJM74wRpSmDEiIaXhbSvAcTxfxg,64
-funlab_sched-0.3.0.dist-info/LICENSE,sha256=1S4A7HXlZTwTjb5TDP5LCY_0yBdx_c4GmIW_hJ2WqPk,1095
-funlab_sched-0.3.0.dist-info/METADATA,sha256=PAkCFaif17IcKTNrOGmm7paJCiffLkdcQVCwMELzYvw,704
-funlab_sched-0.3.0.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-funlab_sched-0.3.0.dist-info/RECORD,,
+funlab/sched/templates/tasks.html,sha256=AVObfUOUrI45eex5fgpd0_U2qL7o3WRWR3IaEQmHJgk,2383
+funlab_sched-0.3.1.dist-info/entry_points.txt,sha256=gLwkuvZnCAY-q3VVxJM74wRpSmDEiIaXhbSvAcTxfxg,64
+funlab_sched-0.3.1.dist-info/LICENSE,sha256=zVP1MdO-7OQCUwUz2kFKV4tD8u2ju_WGztpQ3fObdO8,1091
+funlab_sched-0.3.1.dist-info/METADATA,sha256=JwcgFOHPHePApLl_1seQxyGikKJgVJmBxCRGLEUoPsw,727
+funlab_sched-0.3.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+funlab_sched-0.3.1.dist-info/RECORD,,
```

