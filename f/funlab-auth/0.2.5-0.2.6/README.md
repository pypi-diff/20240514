# Comparing `tmp/funlab_auth-0.2.5-py3-none-any.whl.zip` & `tmp/funlab_auth-0.2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 20748 bytes, number of entries: 18
+Zip file size: 21081 bytes, number of entries: 18
 -rw-r--r--  2.0 fat     1002 b- defN 80-Jan-01 00:00 funlab/auth/__init__.py
 -rw-r--r--  2.0 fat      611 b- defN 80-Jan-01 00:00 funlab/auth/conf/plugin.toml
 -rw-r--r--  2.0 fat     1312 b- defN 80-Jan-01 00:00 funlab/auth/forms.py
 -rw-r--r--  2.0 fat      117 b- defN 80-Jan-01 00:00 funlab/auth/templates/logo.html
--rw-r--r--  2.0 fat     1561 b- defN 80-Jan-01 00:00 funlab/auth/templates/logout.html
--rw-r--r--  2.0 fat     3409 b- defN 80-Jan-01 00:00 funlab/auth/templates/register.html
--rw-r--r--  2.0 fat     5004 b- defN 80-Jan-01 00:00 funlab/auth/templates/resetpass.html
--rw-r--r--  2.0 fat     5809 b- defN 80-Jan-01 00:00 funlab/auth/templates/settings.html
--rw-r--r--  2.0 fat     4645 b- defN 80-Jan-01 00:00 funlab/auth/templates/sign-in-cover.html
--rw-r--r--  2.0 fat     5228 b- defN 80-Jan-01 00:00 funlab/auth/templates/sign-in-illustration.html
--rw-r--r--  2.0 fat     4380 b- defN 80-Jan-01 00:00 funlab/auth/templates/sign-in.html
--rw-r--r--  2.0 fat     4499 b- defN 80-Jan-01 00:00 funlab/auth/user.py
--rw-r--r--  2.0 fat    13403 b- defN 80-Jan-01 00:00 funlab/auth/view.py
--rw-r--r--  2.0 fat       52 b- defN 80-Jan-01 00:00 funlab_auth-0.2.5.dist-info/entry_points.txt
--rw-r--r--  2.0 fat     1095 b- defN 80-Jan-01 00:00 funlab_auth-0.2.5.dist-info/LICENSE
--rw-r--r--  2.0 fat      906 b- defN 80-Jan-01 00:00 funlab_auth-0.2.5.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 funlab_auth-0.2.5.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1548 b- defN 16-Jan-01 00:00 funlab_auth-0.2.5.dist-info/RECORD
-18 files, 54669 bytes uncompressed, 18194 bytes compressed:  66.7%
+-rw-r--r--  2.0 fat     1597 b- defN 80-Jan-01 00:00 funlab/auth/templates/logout.html
+-rw-r--r--  2.0 fat     3475 b- defN 80-Jan-01 00:00 funlab/auth/templates/register.html
+-rw-r--r--  2.0 fat     5099 b- defN 80-Jan-01 00:00 funlab/auth/templates/resetpass.html
+-rw-r--r--  2.0 fat     5969 b- defN 80-Jan-01 00:00 funlab/auth/templates/settings.html
+-rw-r--r--  2.0 fat     4753 b- defN 80-Jan-01 00:00 funlab/auth/templates/sign-in-cover.html
+-rw-r--r--  2.0 fat     5341 b- defN 80-Jan-01 00:00 funlab/auth/templates/sign-in-illustration.html
+-rw-r--r--  2.0 fat     4483 b- defN 80-Jan-01 00:00 funlab/auth/templates/sign-in.html
+-rw-r--r--  2.0 fat     5058 b- defN 80-Jan-01 00:00 funlab/auth/user.py
+-rw-r--r--  2.0 fat    13778 b- defN 80-Jan-01 00:00 funlab/auth/view.py
+-rw-r--r--  2.0 fat       52 b- defN 80-Jan-01 00:00 funlab_auth-0.2.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 fat     1091 b- defN 80-Jan-01 00:00 funlab_auth-0.2.6.dist-info/LICENSE
+-rw-r--r--  2.0 fat      971 b- defN 80-Jan-01 00:00 funlab_auth-0.2.6.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 funlab_auth-0.2.6.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1548 b- defN 16-Jan-01 00:00 funlab_auth-0.2.6.dist-info/RECORD
+18 files, 56345 bytes uncompressed, 18527 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: funlab/auth/user.py
 Comment: 
 
 Filename: funlab/auth/view.py
 Comment: 
 
-Filename: funlab_auth-0.2.5.dist-info/entry_points.txt
+Filename: funlab_auth-0.2.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: funlab_auth-0.2.5.dist-info/LICENSE
+Filename: funlab_auth-0.2.6.dist-info/LICENSE
 Comment: 
 
-Filename: funlab_auth-0.2.5.dist-info/METADATA
+Filename: funlab_auth-0.2.6.dist-info/METADATA
 Comment: 
 
-Filename: funlab_auth-0.2.5.dist-info/WHEEL
+Filename: funlab_auth-0.2.6.dist-info/WHEEL
 Comment: 
 
-Filename: funlab_auth-0.2.5.dist-info/RECORD
+Filename: funlab_auth-0.2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## funlab/auth/templates/logout.html

 * *Ordering differences only*

```diff
@@ -1,36 +1,36 @@
-{% extends "layouts/base-fullscreen.html" %}
-
-{% block title %} Error 403 {% endblock %} 
-
-<!-- Specific Page CSS goes HERE  -->
-{% block stylesheets %}{% endblock stylesheets %}
-
-{% block content %}
-
-    <main>
-        <section class="vh-100 d-flex align-items-center justify-content-center">
-            <div class="container">
-                <div class="row">
-                    <div class="col-12 text-center d-flex align-items-center justify-content-center">
-                        <div>
-                            <h1 class="mt-5">
-                                Logout
-                            </h1>
-                            <div class="empty-action">
-                                <a href="./." class="btn btn-primary">
-                                  <!-- Download SVG icon from http://tabler-icons.io/i/arrow-left -->
-                                  <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M5 12l14 0" /><path d="M5 12l6 6" /><path d="M5 12l6 -6" /></svg>
-                                  Take me home
-                                </a>
-                              </div>
-                        </div>
-                    </div>
-                </div>
-            </div>
-        </section>
-    </main>
-
-{% endblock content %}
-
-<!-- Specific Page JS goes HERE  -->
-{% block javascripts %}{% endblock javascripts %}
+{% extends "layouts/base-fullscreen.html" %}
+
+{% block title %} Error 403 {% endblock %} 
+
+<!-- Specific Page CSS goes HERE  -->
+{% block stylesheets %}{% endblock stylesheets %}
+
+{% block content %}
+
+    <main>
+        <section class="vh-100 d-flex align-items-center justify-content-center">
+            <div class="container">
+                <div class="row">
+                    <div class="col-12 text-center d-flex align-items-center justify-content-center">
+                        <div>
+                            <h1 class="mt-5">
+                                Logout
+                            </h1>
+                            <div class="empty-action">
+                                <a href="./." class="btn btn-primary">
+                                  <!-- Download SVG icon from http://tabler-icons.io/i/arrow-left -->
+                                  <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M5 12l14 0" /><path d="M5 12l6 6" /><path d="M5 12l6 -6" /></svg>
+                                  Take me home
+                                </a>
+                              </div>
+                        </div>
+                    </div>
+                </div>
+            </div>
+        </section>
+    </main>
+
+{% endblock content %}
+
+<!-- Specific Page JS goes HERE  -->
+{% block javascripts %}{% endblock javascripts %}
```

## funlab/auth/templates/register.html

 * *Ordering differences only*

```diff
@@ -1,67 +1,67 @@
-<!--
-* Tabler - Premium and Open Source dashboard template with responsive and high quality UI.
-* @version 1.0.0-beta19
-* @link https://tabler.io
-* Copyright 2018-2023 The Tabler Authors
-* Copyright 2018-2023 codecalm.net Paweł Kuna
-* Licensed under MIT (https://github.com/tabler/tabler/blob/master/LICENSE)
--->
-{% extends "layouts/base-fullscreen.html" %}
-
-{% block title %} Sign IN {% endblock %}
-
-<!-- Specific Page CSS goes HERE  -->
-{% block stylesheets %}{% endblock stylesheets %}
-
-{% block page_header %}{% endblock page_header %}
-
-{% block page_body %}
-<div class="page page-center">
-      <div class="container container-tight py-4">
-        <div class="text-center mb-4">
-          <a href="." class="navbar-brand navbar-brand-autodark"><img src="{{ config.APP_LOGO }}" height="36" alt="{{ config.APP_NAME }}"></a>
-        </div>
-        <form id="register" class="card card-md" action="{{ url_for('auth_bp.register') }}" method="post" autocomplete="off" novalidate>
-          <div class="card-body">
-            <h2 class="card-title text-center mb-4">Create new account</h2>
-            <div class="mb-3">
-              <label class="form-label">User Name</label>
-              {{ form.username(placeholder="User name", class="form-control", type="text") }}
-            </div>
-            <div class="mb-3">
-              <label class="form-label">Email address</label>
-              {{ form.email(placeholder="Email", class="form-control", type="email") }}
-            </div>
-            <div class="mb-3">
-              <label class="form-label">Password</label>
-              <div class="input-group input-group-flat">
-                <!-- <input type="password" class="form-control"  placeholder="Password"  autocomplete="off">-->
-                {{ form.password(placeholder="Password", class="form-control", type="password", autocomplete="off") }}
-                <span class="input-group-text">
-                  <a id="show-password" href="#" class="link-secondary" title="Show password" data-bs-toggle="tooltip"><!-- Download SVG icon from http://tabler-icons.io/i/eye -->
-                    <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M10 12a2 2 0 1 0 4 0a2 2 0 0 0 -4 0" /><path d="M21 12c-2.4 4 -5.4 6 -9 6c-3.6 0 -6.6 -2 -9 -6c2.4 -4 5.4 -6 9 -6c3.6 0 6.6 2 9 6" /></svg>
-                  </a>
-                </span>
-              </div>
-            </div>
-            <div class="mb-3">
-              <label class="form-check">
-                <input type="checkbox" class="form-check-input"/>
-                <span class="form-check-label">Agree the <a href="./terms-of-service.html" tabindex="-1">terms and policy</a>.</span>
-              </label>
-            </div>
-            <div class="form-footer">
-              <button name="register" type="submit" class="btn btn-primary w-100">Create new account</button>
-            </div>
-          </div>
-        </form>
-        <div class="text-center text-muted mt-3">
-          Already have account? <a href="{{ url_for('auth_bp.login') }}" tabindex="-1">Sign in</a>
-        </div>
-      </div>
-</div>
-
-{% endblock page_body %}
-
-<!-- Specific Page JS goes HERE  -->
+<!--
+* Tabler - Premium and Open Source dashboard template with responsive and high quality UI.
+* @version 1.0.0-beta19
+* @link https://tabler.io
+* Copyright 2018-2023 The Tabler Authors
+* Copyright 2018-2023 codecalm.net Paweł Kuna
+* Licensed under MIT (https://github.com/tabler/tabler/blob/master/LICENSE)
+-->
+{% extends "layouts/base-fullscreen.html" %}
+
+{% block title %} Sign IN {% endblock %}
+
+<!-- Specific Page CSS goes HERE  -->
+{% block stylesheets %}{% endblock stylesheets %}
+
+{% block page_header %}{% endblock page_header %}
+
+{% block page_body %}
+<div class="page page-center">
+      <div class="container container-tight py-4">
+        <div class="text-center mb-4">
+          <a href="." class="navbar-brand navbar-brand-autodark"><img src="{{ config.APP_LOGO }}" height="36" alt="{{ config.APP_NAME }}"></a>
+        </div>
+        <form id="register" class="card card-md" action="{{ url_for('auth_bp.register') }}" method="post" autocomplete="off" novalidate>
+          <div class="card-body">
+            <h2 class="card-title text-center mb-4">Create new account</h2>
+            <div class="mb-3">
+              <label class="form-label">User Name</label>
+              {{ form.username(placeholder="User name", class="form-control", type="text") }}
+            </div>
+            <div class="mb-3">
+              <label class="form-label">Email address</label>
+              {{ form.email(placeholder="Email", class="form-control", type="email") }}
+            </div>
+            <div class="mb-3">
+              <label class="form-label">Password</label>
+              <div class="input-group input-group-flat">
+                <!-- <input type="password" class="form-control"  placeholder="Password"  autocomplete="off">-->
+                {{ form.password(placeholder="Password", class="form-control", type="password", autocomplete="off") }}
+                <span class="input-group-text">
+                  <a id="show-password" href="#" class="link-secondary" title="Show password" data-bs-toggle="tooltip"><!-- Download SVG icon from http://tabler-icons.io/i/eye -->
+                    <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"><path stroke="none" d="M0 0h24v24H0z" fill="none"/><path d="M10 12a2 2 0 1 0 4 0a2 2 0 0 0 -4 0" /><path d="M21 12c-2.4 4 -5.4 6 -9 6c-3.6 0 -6.6 -2 -9 -6c2.4 -4 5.4 -6 9 -6c3.6 0 6.6 2 9 6" /></svg>
+                  </a>
+                </span>
+              </div>
+            </div>
+            <div class="mb-3">
+              <label class="form-check">
+                <input type="checkbox" class="form-check-input"/>
+                <span class="form-check-label">Agree the <a href="./terms-of-service.html" tabindex="-1">terms and policy</a>.</span>
+              </label>
+            </div>
+            <div class="form-footer">
+              <button name="register" type="submit" class="btn btn-primary w-100">Create new account</button>
+            </div>
+          </div>
+        </form>
+        <div class="text-center text-muted mt-3">
+          Already have account? <a href="{{ url_for('auth_bp.login') }}" tabindex="-1">Sign in</a>
+        </div>
+      </div>
+</div>
+
+{% endblock page_body %}
+
+<!-- Specific Page JS goes HERE  -->
 {% block javascripts %}{% endblock javascripts %}
```

## funlab/auth/templates/resetpass.html

 * *Ordering differences only*

```diff
@@ -1,96 +1,96 @@
-{% extends "layouts/base-fullscreen.html" %}
-
-{% block title %} Reset Password {% endblock %}
-
-<!-- Specific Page CSS goes HERE  -->
-{% block stylesheets %}{% endblock stylesheets %}
-
-{% block page_header %}{% endblock page_header %}
-
-{% block page_body %}
-<div class="page page-center">
-    <div class="container container-tight py-4">
-        <div class="text-center mb-4">
-            <a href="." class="navbar-brand navbar-brand-autodark"><img src="{{ config.APP_LOGO }}"
-                    height="36" alt="{{ config.APP_NAME }}"></a>
-        </div>
-        <form class="card card-md" method="post" action="">
-            {{ form.hidden_tag() }}
-            <div class="card-body">
-                <h2 class="h2 text-center mb-4">Reset password</h2>
-                <p>
-                    {% if msg %}
-                    <span class="text-danger">{{ msg | safe }}</span>
-                    {% endif %}
-                </p>
-                <input id="email" name="email" type="hidden" value="{{ current_user.email }}">
-                <!-- Form -->
-                <div class="form-group mb-4">
-                    <label for="old_password">Your Old Password</label>
-                    <div class="input-group">
-                        <span class="input-group-text" id="basic-addon2">
-                            <svg class="icon icon-xs text-gray-600" fill="currentColor" viewBox="0 0 20 20"
-                                xmlns="http://www.w3.org/2000/svg">
-                                <path fill-rule="evenodd"
-                                    d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z"
-                                    clip-rule="evenodd"></path>
-                            </svg>
-                        </span>
-                        {{ form.old_password(class="form-control") }}
-                    </div>
-                </div>
-                <div class="form-group mb-4">
-                    <label for="new_password">New Password</label>
-                    <div class="input-group">
-                        <span class="input-group-text" id="basic-addon2">
-                            <svg class="icon icon-xs text-gray-600" fill="currentColor" viewBox="0 0 20 20"
-                                xmlns="http://www.w3.org/2000/svg">
-                                <path fill-rule="evenodd"
-                                    d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z"
-                                    clip-rule="evenodd"></path>
-                            </svg>
-                        </span>
-                        {{ form.new_password(class="form-control") }}
-                    </div>
-                </div>
-                <div class="form-group mb-4">
-                    <label for="confirm_password">Confirm Password</label>
-                    <div class="input-group">
-                        <span class="input-group-text" id="basic-addon2">
-                            <svg class="icon icon-xs text-gray-600" fill="currentColor" viewBox="0 0 20 20"
-                                xmlns="http://www.w3.org/2000/svg">
-                                <path fill-rule="evenodd"
-                                    d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z"
-                                    clip-rule="evenodd"></path>
-                            </svg>
-                        </span>
-                        {{ form.confirm_password(class="form-control") }}
-                    </div>
-                </div>
-                <!-- End of Form -->
-                <div class="d-grid">
-                    {{form.resetpass(class="btn btn-secondary")}}
-                </div>
-                <div class="form-footer">
-                    <a href="#" class="btn btn-primary w-100">
-                        <!-- Download SVG icon from http://tabler-icons.io/i/mail -->
-                        <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24"
-                            stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round"
-                            stroke-linejoin="round">
-                            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
-                            <path d="M3 7a2 2 0 0 1 2 -2h14a2 2 0 0 1 2 2v10a2 2 0 0 1 -2 2h-14a2 2 0 0 1 -2 -2v-10z" />
-                            <path d="M3 7l9 6l9 -6" />
-                        </svg>
-                        Send me new password
-                    </a>
-                </div>
-            </div>
-        </form>
-        <div class="text-center text-muted mt-3">
-            Forget it, <a href="{{ url_for('auth_bp.login') }}">send me back</a> to the sign in screen.
-        </div>
-    </div>
-</div>
-    {% endblock page_body %}
-<!-- Specific Page JS goes HERE  -->
+{% extends "layouts/base-fullscreen.html" %}
+
+{% block title %} Reset Password {% endblock %}
+
+<!-- Specific Page CSS goes HERE  -->
+{% block stylesheets %}{% endblock stylesheets %}
+
+{% block page_header %}{% endblock page_header %}
+
+{% block page_body %}
+<div class="page page-center">
+    <div class="container container-tight py-4">
+        <div class="text-center mb-4">
+            <a href="." class="navbar-brand navbar-brand-autodark"><img src="{{ config.APP_LOGO }}"
+                    height="36" alt="{{ config.APP_NAME }}"></a>
+        </div>
+        <form class="card card-md" method="post" action="">
+            {{ form.hidden_tag() }}
+            <div class="card-body">
+                <h2 class="h2 text-center mb-4">Reset password</h2>
+                <p>
+                    {% if msg %}
+                    <span class="text-danger">{{ msg | safe }}</span>
+                    {% endif %}
+                </p>
+                <input id="email" name="email" type="hidden" value="{{ current_user.email }}">
+                <!-- Form -->
+                <div class="form-group mb-4">
+                    <label for="old_password">Your Old Password</label>
+                    <div class="input-group">
+                        <span class="input-group-text" id="basic-addon2">
+                            <svg class="icon icon-xs text-gray-600" fill="currentColor" viewBox="0 0 20 20"
+                                xmlns="http://www.w3.org/2000/svg">
+                                <path fill-rule="evenodd"
+                                    d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z"
+                                    clip-rule="evenodd"></path>
+                            </svg>
+                        </span>
+                        {{ form.old_password(class="form-control") }}
+                    </div>
+                </div>
+                <div class="form-group mb-4">
+                    <label for="new_password">New Password</label>
+                    <div class="input-group">
+                        <span class="input-group-text" id="basic-addon2">
+                            <svg class="icon icon-xs text-gray-600" fill="currentColor" viewBox="0 0 20 20"
+                                xmlns="http://www.w3.org/2000/svg">
+                                <path fill-rule="evenodd"
+                                    d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z"
+                                    clip-rule="evenodd"></path>
+                            </svg>
+                        </span>
+                        {{ form.new_password(class="form-control") }}
+                    </div>
+                </div>
+                <div class="form-group mb-4">
+                    <label for="confirm_password">Confirm Password</label>
+                    <div class="input-group">
+                        <span class="input-group-text" id="basic-addon2">
+                            <svg class="icon icon-xs text-gray-600" fill="currentColor" viewBox="0 0 20 20"
+                                xmlns="http://www.w3.org/2000/svg">
+                                <path fill-rule="evenodd"
+                                    d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 0 012-2zm8-2v2H7V7a3 3 0 016 0z"
+                                    clip-rule="evenodd"></path>
+                            </svg>
+                        </span>
+                        {{ form.confirm_password(class="form-control") }}
+                    </div>
+                </div>
+                <!-- End of Form -->
+                <div class="d-grid">
+                    {{form.resetpass(class="btn btn-secondary")}}
+                </div>
+                <div class="form-footer">
+                    <a href="#" class="btn btn-primary w-100">
+                        <!-- Download SVG icon from http://tabler-icons.io/i/mail -->
+                        <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24"
+                            stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round"
+                            stroke-linejoin="round">
+                            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
+                            <path d="M3 7a2 2 0 0 1 2 -2h14a2 2 0 0 1 2 2v10a2 2 0 0 1 -2 2h-14a2 2 0 0 1 -2 -2v-10z" />
+                            <path d="M3 7l9 6l9 -6" />
+                        </svg>
+                        Send me new password
+                    </a>
+                </div>
+            </div>
+        </form>
+        <div class="text-center text-muted mt-3">
+            Forget it, <a href="{{ url_for('auth_bp.login') }}">send me back</a> to the sign in screen.
+        </div>
+    </div>
+</div>
+    {% endblock page_body %}
+<!-- Specific Page JS goes HERE  -->
 {% block javascripts %}{% endblock javascripts %}
```

## funlab/auth/templates/settings.html

```diff
@@ -1,160 +1,160 @@
-<!doctype html>
-<!--
-* Tabler - Premium and Open Source dashboard template with responsive and high quality UI.
-* @version 1.0.0-beta20
-* @link https://tabler.io
-* Copyright 2018-2023 The Tabler Authors
-* Copyright 2018-2023 codecalm.net Paweł Kuna
-* Licensed under MIT (https://github.com/tabler/tabler/blob/master/LICENSE)
--->
-{% extends "layouts/base.html" %}
-
-{% block title %}{{ config.TITLE }} - {{ self._TemplateReference__context.name }} {% endblock title %}
-<!-- Specific Page CSS goes HERE  -->
-{% block stylesheets %}
-<style>
-  @import url('https://rsms.me/inter/inter.css');
-
-  :root {
-    --tblr-font-sans-serif: 'Inter Var', -apple-system, BlinkMacSystemFont, San Francisco, Segoe UI, Roboto, Helvetica Neue, sans-serif;
-  }
-
-  body {
-    font-feature-settings: "cv03", "cv04", "cv11";
-  }
-</style>
-{% endblock stylesheets %}
-{% block page_header %}
-<!-- Page header -->
-<div class="container-xl">
-  <div class="row g-2 align-items-center">
-    <div class="col">
-      <h2 class="page-title">
-        Account Settings
-      </h2>
-    </div>
-  </div>
-</div>
-{% endblock page_header %}
-<!-- Page body -->
-{% block page_body %}
-<div class="container-xl">
-  <div class="card">
-    <div class="card-header">
-      <ul class="nav nav-tabs card-header-tabs nav-fill" data-bs-toggle="tabs">
-        <li class="nav-item">
-          <a href="#my-account" class="nav-link active"
-            data-bs-toggle="tab"><!-- Download SVG icon from http://tabler-icons.io/i/home -->
-            <svg xmlns="http://www.w3.org/2000/svg" class="icon me-2" width="24" height="24" viewBox="0 0 24 24"
-              stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
-              <path stroke="none" d="M0 0h24v24H0z" fill="none" />
-              <path d="M8 7a4 4 0 1 0 8 0a4 4 0 0 0 -8 0" />
-              <path d="M6 21v-2a4 4 0 0 1 4 -4h4a4 4 0 0 1 4 4v2" />
-            </svg>
-            My Account</a>
-        </li>
-        <li class="nav-item">
-          <a href="#tabs-activity-7" class="nav-link"
-            data-bs-toggle="tab"><!-- Download SVG icon from http://tabler-icons.io/i/activity -->
-            <svg xmlns="http://www.w3.org/2000/svg" class="icon me-2" width="24" height="24" viewBox="0 0 24 24"
-              stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
-              <path stroke="none" d="M0 0h24v24H0z" fill="none" />
-              <path d="M3 12h4l3 8l4 -16l3 8h4" />
-            </svg>
-            Activity</a>
-        </li>
-      </ul>
-    </div>
-    <div class="card-body">
-      <div class="tab-content">
-        <div class="tab-pane active show" id="my-account">
-          <h2 class="mb-4">My Account</h2>
-          <div class="row align-items-center">
-            <div class="col-auto"><span class="avatar avatar-xl"
-                style="background-image: url({{ current_user.avatar_url|default('static/nobody.svg', true) }})"></span>
-            </div>
-            <div class="col-auto"><a href="#" class="btn">
-                Change avatar
-              </a></div>
-          </div>
-          <h3 class="card-title mt-4">User Name</h3>
-          <div>
-            <div class="row g-2">
-              <div class="col-auto">
-                <input type="text" class="form-control w-auto" value="{{current_user.username}}">
-              </div>
-
-            </div>
-          </div>
-          <h3 class="card-title mt-4">Email</h3>
-          <div>
-            <div class="row g-2">
-              <div class="col-auto">
-                {{current_user.email}}
-              </div>
-            </div>
-          </div>
-          <h3 class="card-title mt-4">Password</h3>
-          <p class="card-subtitle">You can set a permanent password if you don't want to use temporary login codes.
-          </p>
-          <div>
-            <a href="/resetpass" class="btn">
-              Set new password
-            </a>
-          </div>
-          <div class="card-footer bg-transparent mt-3">
-            <div class="btn-list justify-content-end">
-              <a href="#" class="btn">
-                Cancel
-              </a>
-              <a href="#" class="btn btn-primary">
-                Save
-              </a>
-            </div>
-          </div>
-        </div>
-        <div class="tab-pane" id="tabs-activity-7">
-          <h4>Activity tab</h4>
-          <div>Donec ac vitae diam amet vel leo egestas consequat rhoncus in luctus amet, facilisi sit mauris accumsan
-            nibh habitant senectus</div>
-        </div>
-      </div>
-    </div>
-  </div>
-</div>
-
-{% endblock page_body %}
-
-<!-- Specific Page JS goes HERE  -->
-
-{% block javascripts %}
-<script type="text/javascript">
-  document.addEventListener("DOMContentLoaded", function () {
-    // Show last tab
-    var lastTabElement = document.querySelector("#broker_accounts li:first-child a");
-    var lastTab = new bootstrap.Tab(lastTabElement);
-    lastTab.show();
-  });
-  $(".nav-tabs").on("click", "a", function (e) {
-    e.preventDefault();
-    if (!$(this).hasClass('new_broker')) {
-      $(this).tab('show');
-    }
-  })
-    .on("click", "span", function () {
-      var anchor = $(this).siblings('a');
-      $(anchor.attr('href')).remove();
-      $(this).parent().remove();
-      $(".nav-tabs li").children('a').first().click();
-    });
-
-  $('.add-contact').click(function (e) {
-    e.preventDefault();
-    var id = $(".nav-tabs").children().length; //think about it ;)
-    var tabId = 'contact_' + id;
-    $(this).closest('li').before('<li><a href="#contact_' + id + '">New Tab</a> <span> x </span></li>');
-    $('.tab-content').append('<div class="tab-pane" id="' + tabId + '">Contact Form: New Contact ' + id + '</div>');
-    $('.nav-tabs li:nth-child(' + id + ') a').click();
-  });
-</script>
+<!doctype html>
+<!--
+* Tabler - Premium and Open Source dashboard template with responsive and high quality UI.
+* @version 1.0.0-beta20
+* @link https://tabler.io
+* Copyright 2018-2023 The Tabler Authors
+* Copyright 2018-2023 codecalm.net Paweł Kuna
+* Licensed under MIT (https://github.com/tabler/tabler/blob/master/LICENSE)
+-->
+{% extends "layouts/base.html" %}
+
+{% block title %}{{ config.TITLE }} - {{ self._TemplateReference__context.name }} {% endblock title %}
+<!-- Specific Page CSS goes HERE  -->
+{% block stylesheets %}
+<style>
+  @import url('https://rsms.me/inter/inter.css');
+
+  :root {
+    --tblr-font-sans-serif: 'Inter Var', -apple-system, BlinkMacSystemFont, San Francisco, Segoe UI, Roboto, Helvetica Neue, sans-serif;
+  }
+
+  body {
+    font-feature-settings: "cv03", "cv04", "cv11";
+  }
+</style>
+{% endblock stylesheets %}
+{% block page_header %}
+<!-- Page header -->
+<div class="container-xl">
+  <div class="row g-2 align-items-center">
+    <div class="col">
+      <h2 class="page-title">
+        Account Settings
+      </h2>
+    </div>
+  </div>
+</div>
+{% endblock page_header %}
+<!-- Page body -->
+{% block page_body %}
+<div class="container-xl">
+  <div class="card">
+    <div class="card-header">
+      <ul class="nav nav-tabs card-header-tabs nav-fill" data-bs-toggle="tabs">
+        <li class="nav-item">
+          <a href="#my-account" class="nav-link active"
+            data-bs-toggle="tab"><!-- Download SVG icon from http://tabler-icons.io/i/home -->
+            <svg xmlns="http://www.w3.org/2000/svg" class="icon me-2" width="24" height="24" viewBox="0 0 24 24"
+              stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
+              <path stroke="none" d="M0 0h24v24H0z" fill="none" />
+              <path d="M8 7a4 4 0 1 0 8 0a4 4 0 0 0 -8 0" />
+              <path d="M6 21v-2a4 4 0 0 1 4 -4h4a4 4 0 0 1 4 4v2" />
+            </svg>
+            My Account</a>
+        </li>
+        <li class="nav-item">
+          <a href="#tabs-activity-7" class="nav-link"
+            data-bs-toggle="tab"><!-- Download SVG icon from http://tabler-icons.io/i/activity -->
+            <svg xmlns="http://www.w3.org/2000/svg" class="icon me-2" width="24" height="24" viewBox="0 0 24 24"
+              stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
+              <path stroke="none" d="M0 0h24v24H0z" fill="none" />
+              <path d="M3 12h4l3 8l4 -16l3 8h4" />
+            </svg>
+            Activity</a>
+        </li>
+      </ul>
+    </div>
+    <div class="card-body">
+      <div class="tab-content">
+        <div class="tab-pane active show" id="my-account">
+          <h2 class="mb-4">My Account</h2>
+          <div class="row align-items-center">
+            <div class="col-auto"><span class="avatar avatar-xl"
+                style="background-image: url({{ current_user.avatar_url|default('/static/nobody.svg', true) }})"></span>
+            </div>
+            <div class="col-auto"><a href="#" class="btn">
+                Change avatar
+              </a></div>
+          </div>
+          <h3 class="card-title mt-4">User Name</h3>
+          <div>
+            <div class="row g-2">
+              <div class="col-auto">
+                <input type="text" class="form-control w-auto" value="{{current_user.username}}">
+              </div>
+
+            </div>
+          </div>
+          <h3 class="card-title mt-4">Email</h3>
+          <div>
+            <div class="row g-2">
+              <div class="col-auto">
+                {{current_user.email}}
+              </div>
+            </div>
+          </div>
+          <h3 class="card-title mt-4">Password</h3>
+          <p class="card-subtitle">You can set a permanent password if you don't want to use temporary login codes.
+          </p>
+          <div>
+            <a href="/resetpass" class="btn">
+              Set new password
+            </a>
+          </div>
+          <div class="card-footer bg-transparent mt-3">
+            <div class="btn-list justify-content-end">
+              <a href="#" class="btn">
+                Cancel
+              </a>
+              <a href="#" class="btn btn-primary">
+                Save
+              </a>
+            </div>
+          </div>
+        </div>
+        <div class="tab-pane" id="tabs-activity-7">
+          <h4>Activity tab</h4>
+          <div>Donec ac vitae diam amet vel leo egestas consequat rhoncus in luctus amet, facilisi sit mauris accumsan
+            nibh habitant senectus</div>
+        </div>
+      </div>
+    </div>
+  </div>
+</div>
+
+{% endblock page_body %}
+
+<!-- Specific Page JS goes HERE  -->
+
+{% block javascripts %}
+<script type="text/javascript">
+  document.addEventListener("DOMContentLoaded", function () {
+    // Show last tab
+    var lastTabElement = document.querySelector("#broker_accounts li:first-child a");
+    var lastTab = new bootstrap.Tab(lastTabElement);
+    lastTab.show();
+  });
+  $(".nav-tabs").on("click", "a", function (e) {
+    e.preventDefault();
+    if (!$(this).hasClass('new_broker')) {
+      $(this).tab('show');
+    }
+  })
+    .on("click", "span", function () {
+      var anchor = $(this).siblings('a');
+      $(anchor.attr('href')).remove();
+      $(this).parent().remove();
+      $(".nav-tabs li").children('a').first().click();
+    });
+
+  $('.add-contact').click(function (e) {
+    e.preventDefault();
+    var id = $(".nav-tabs").children().length; //think about it ;)
+    var tabId = 'contact_' + id;
+    $(this).closest('li').before('<li><a href="#contact_' + id + '">New Tab</a> <span> x </span></li>');
+    $('.tab-content').append('<div class="tab-pane" id="' + tabId + '">Contact Form: New Contact ' + id + '</div>');
+    $('.nav-tabs li:nth-child(' + id + ') a').click();
+  });
+</script>
 {% endblock javascripts %}
```

## funlab/auth/templates/sign-in-cover.html

 * *Ordering differences only*

```diff
@@ -1,109 +1,109 @@
-<!--
-* Tabler - Premium and Open Source dashboard template with responsive and high quality UI.
-* @version 1.0.0-beta19
-* @link https://tabler.io
-* Copyright 2018-2023 The Tabler Authors
-* Copyright 2018-2023 codecalm.net Paweł Kuna
-* Licensed under MIT (https://github.com/tabler/tabler/blob/master/LICENSE)
--->
-
-{% extends "layouts/base-fullscreen.html" %}
-
-{% block title %} Sign IN {% endblock %}
-
-<!-- Specific Page CSS goes HERE  -->
-{% block stylesheets %}{% endblock stylesheets %}
-
-{% block page_header %}{% endblock page_header %}
-
-{% block page_body %}
-<div class="row g-0 flex-fill">
-  <div class="col-12 col-lg-6 col-xl-4 border-top-wide border-primary d-flex flex-column justify-content-center">
-    <div class="container container-tight my-5 px-lg-5">
-      {% with config=config %}
-      {% include 'logo.html' %}
-      {% endwith %}
-      <h2 class="h2 text-center mb-4">Login to {{ config.APP_NAME }}</h2>
-      <!-- Flash Messages -->
-      <div class="text-left">
-        {% with messages = get_flashed_messages(with_categories=true) %}
-        {% if messages %}
-        <div class="alert-container">
-          {% for category, message in messages %}
-          <div class="alert alert-{{ category }} fade show" role="alert">
-            {{ message }}
-            <!-- <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button> -->
-          </div>
-          {% endfor %}
-        </div>
-        {% endif %}
-        {% endwith %}
-      </div>
-      <form id="login" action="{{ url_for('auth_bp.login') }}" method="post" autocomplete="off" novalidate>
-        {{ form.hidden_tag() }}
-        <div class="mb-3">
-          <label class="form-label">Email</label>
-          {{ form.email(placeholder="Email", class="form-control") }}
-        </div>
-        <div class="mb-2">
-          <label class="form-label">
-            Password
-            <span class="form-label-description">
-              <a href="{{ url_for('auth_bp.resetpass') }}">I forgot password</a>
-            </span>
-          </label>
-          <div class="input-group input-group-flat">
-            {{ form.password(placeholder="Password", class="form-control", type="password") }}
-            <span class="input-group-text">
-              <a href="#" id="show-password" class="link-secondary" title="Show password"
-                data-bs-toggle="tooltip"><!-- Download SVG icon from http://tabler-icons.io/i/eye -->
-                <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24"
-                  stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round"
-                          stroke-linejoin="round">
-                  <path stroke="none" d="M0 0h24v24H0z" fill="none" />
-                  <path d="M10 12a2 2 0 1 0 4 0a2 2 0 0 0 -4 0" />
-                  <path d="M21 12c-2.4 4 -5.4 6 -9 6c-3.6 0 -6.6 -2 -9 -6c2.4 -4 5.4 -6 9 -6c3.6 0 6.6 2 9 6" />
-                </svg>
-              </a>
-            </span>
-          </div>
-        </div>
-        <div class="mb-2">
-          <label class="form-check">
-            <input type="checkbox" class="form-check-input" />
-            {{ form.rememberme(class="form-check-input", type="checkbox", checked=True) }}
-            <span class="form-check-label">Remember me on this device</span>
-          </label>
-        </div>
-        <div class="form-footer">
-          <button name="login" type="submit" class="btn btn-primary w-100">Sign in</button>
-        </div>
-      </form>
-
-      <div class="hr-text">or</div>
-      <div class="card-body">
-        {% for oauth_name, provider in oauths_info.items() %}
-        <div class="row mb-3">
-          <a class="btn w-100" href="{{ url_for('auth_bp.oauth_login', oauth_name=oauth_name) }}">
-            <img class="icon text-{{provider}}" width="24" height="24" alt="{{provider}} Login"
-              src="{{ url_for('root_bp.static', filename='brands/' + provider + '.svg') }}">
-            Login with {{provider.capitalize()}} by {{oauth_name}}
-          </a>
-        </div>
-        {% endfor %}
-      </div>
-      <div class="text-center text-muted mt-3">
-        Don't have account yet? <a href="{{ url_for('auth_bp.register') }}" tabindex="-1">Sign up</a>
-      </div>
-    </div>
-  </div>
-  <div class="col-12 col-lg-6 col-xl-8 d-none d-lg-block">
-    <!-- Photo -->
-    <div class="bg-cover h-100 min-vh-100"
-      style="background-image: url(/static/photos/finances-us-dollars-and-bitcoins-currency-money-4.jpg)"></div>
-  </div>
-</div>
-{% endblock page_body %}
-
-<!-- Specific Page JS goes HERE  -->
+<!--
+* Tabler - Premium and Open Source dashboard template with responsive and high quality UI.
+* @version 1.0.0-beta19
+* @link https://tabler.io
+* Copyright 2018-2023 The Tabler Authors
+* Copyright 2018-2023 codecalm.net Paweł Kuna
+* Licensed under MIT (https://github.com/tabler/tabler/blob/master/LICENSE)
+-->
+
+{% extends "layouts/base-fullscreen.html" %}
+
+{% block title %} Sign IN {% endblock %}
+
+<!-- Specific Page CSS goes HERE  -->
+{% block stylesheets %}{% endblock stylesheets %}
+
+{% block page_header %}{% endblock page_header %}
+
+{% block page_body %}
+<div class="row g-0 flex-fill">
+  <div class="col-12 col-lg-6 col-xl-4 border-top-wide border-primary d-flex flex-column justify-content-center">
+    <div class="container container-tight my-5 px-lg-5">
+      {% with config=config %}
+      {% include 'logo.html' %}
+      {% endwith %}
+      <h2 class="h2 text-center mb-4">Login to {{ config.APP_NAME }}</h2>
+      <!-- Flash Messages -->
+      <div class="text-left">
+        {% with messages = get_flashed_messages(with_categories=true) %}
+        {% if messages %}
+        <div class="alert-container">
+          {% for category, message in messages %}
+          <div class="alert alert-{{ category }} fade show" role="alert">
+            {{ message }}
+            <!-- <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button> -->
+          </div>
+          {% endfor %}
+        </div>
+        {% endif %}
+        {% endwith %}
+      </div>
+      <form id="login" action="{{ url_for('auth_bp.login') }}" method="post" autocomplete="off" novalidate>
+        {{ form.hidden_tag() }}
+        <div class="mb-3">
+          <label class="form-label">Email</label>
+          {{ form.email(placeholder="Email", class="form-control") }}
+        </div>
+        <div class="mb-2">
+          <label class="form-label">
+            Password
+            <span class="form-label-description">
+              <a href="{{ url_for('auth_bp.resetpass') }}">I forgot password</a>
+            </span>
+          </label>
+          <div class="input-group input-group-flat">
+            {{ form.password(placeholder="Password", class="form-control", type="password") }}
+            <span class="input-group-text">
+              <a href="#" id="show-password" class="link-secondary" title="Show password"
+                data-bs-toggle="tooltip"><!-- Download SVG icon from http://tabler-icons.io/i/eye -->
+                <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24"
+                  stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round"
+                          stroke-linejoin="round">
+                  <path stroke="none" d="M0 0h24v24H0z" fill="none" />
+                  <path d="M10 12a2 2 0 1 0 4 0a2 2 0 0 0 -4 0" />
+                  <path d="M21 12c-2.4 4 -5.4 6 -9 6c-3.6 0 -6.6 -2 -9 -6c2.4 -4 5.4 -6 9 -6c3.6 0 6.6 2 9 6" />
+                </svg>
+              </a>
+            </span>
+          </div>
+        </div>
+        <div class="mb-2">
+          <label class="form-check">
+            <input type="checkbox" class="form-check-input" />
+            {{ form.rememberme(class="form-check-input", type="checkbox", checked=True) }}
+            <span class="form-check-label">Remember me on this device</span>
+          </label>
+        </div>
+        <div class="form-footer">
+          <button name="login" type="submit" class="btn btn-primary w-100">Sign in</button>
+        </div>
+      </form>
+
+      <div class="hr-text">or</div>
+      <div class="card-body">
+        {% for oauth_name, provider in oauths_info.items() %}
+        <div class="row mb-3">
+          <a class="btn w-100" href="{{ url_for('auth_bp.oauth_login', oauth_name=oauth_name) }}">
+            <img class="icon text-{{provider}}" width="24" height="24" alt="{{provider}} Login"
+              src="{{ url_for('root_bp.static', filename='brands/' + provider + '.svg') }}">
+            Login with {{provider.capitalize()}} by {{oauth_name}}
+          </a>
+        </div>
+        {% endfor %}
+      </div>
+      <div class="text-center text-muted mt-3">
+        Don't have account yet? <a href="{{ url_for('auth_bp.register') }}" tabindex="-1">Sign up</a>
+      </div>
+    </div>
+  </div>
+  <div class="col-12 col-lg-6 col-xl-8 d-none d-lg-block">
+    <!-- Photo -->
+    <div class="bg-cover h-100 min-vh-100"
+      style="background-image: url(/static/photos/finances-us-dollars-and-bitcoins-currency-money-4.jpg)"></div>
+  </div>
+</div>
+{% endblock page_body %}
+
+<!-- Specific Page JS goes HERE  -->
 {% block javascripts %}{% endblock javascripts %}
```

## funlab/auth/templates/sign-in-illustration.html

 * *Ordering differences only*

```diff
@@ -1,114 +1,114 @@
-<!--
-* Tabler - Premium and Open Source dashboard template with responsive and high quality UI.
-* @version 1.0.0-beta19
-* @link https://tabler.io
-* Copyright 2018-2023 The Tabler Authors
-* Copyright 2018-2023 codecalm.net Paweł Kuna
-* Licensed under MIT (https://github.com/tabler/tabler/blob/master/LICENSE)
--->
-
-{% extends "layouts/base-fullscreen.html" %}
-
-{% block title %} Sign IN {% endblock %}
-
-<!-- Specific Page CSS goes HERE  -->
-{% block stylesheets %}{% endblock stylesheets %}
-
-{% block page_header %}{% endblock page_header %}
-
-{% block page_body %}
-<div class="page page-center">
-  <div class="container container-normal py-4">
-    <div class="row align-items-center g-4">
-      <div class="col-lg">
-        <div class="container-tight">
-          {% with config=config %}
-          {% include 'logo.html' %}
-          {% endwith %}
-          <div class="card card-md">
-            <div class="card-body">
-              <h2 class="h2 text-center mb-4">Login to {{ config.APP_NAME }}</h2>
-              <!-- Flash Messages -->
-              <div class="text-left">
-                {% with messages = get_flashed_messages(with_categories=true) %}
-                {% if messages %}
-                <div class="alert-container">
-                  {% for category, message in messages %}
-                  <div class="alert alert-{{ category }} fade show" role="alert">
-                    {{ message }}
-                    <!-- <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button> -->
-                  </div>
-                  {% endfor %}
-                </div>
-                {% endif %}
-                {% endwith %}
-              </div>
-              <form id="login" action="{{ url_for('auth_bp.login') }}" method="post" autocomplete="off" novalidate>
-                {{ form.hidden_tag() }}
-                <div class="mb-3">
-                  <label class="form-label">Email</label>
-                  {{ form.email(placeholder="Email", class="form-control") }}
-                </div>
-                <div class="mb-2">
-                  <label class="form-label">
-                    Password
-                    <span class="form-label-description">
-                      <a href="{{ url_for('auth_bp.resetpass') }}">I forgot password</a>
-                    </span>
-                  </label>
-                  <div class="input-group input-group-flat">
-                    {{ form.password(placeholder="Password", class="form-control", type="password") }}
-                    <span class="input-group-text">
-                      <a href="#" id="show-password" class="link-secondary" title="Show password"
-                        data-bs-toggle="tooltip"><!-- Download SVG icon from http://tabler-icons.io/i/eye -->
-                        <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24"
-                          stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round"
-                          stroke-linejoin="round">
-                          <path stroke="none" d="M0 0h24v24H0z" fill="none" />
-                          <path d="M10 12a2 2 0 1 0 4 0a2 2 0 0 0 -4 0" />
-                          <path d="M21 12c-2.4 4 -5.4 6 -9 6c-3.6 0 -6.6 -2 -9 -6c2.4 -4 5.4 -6 9 -6c3.6 0 6.6 2 9 6" />
-                        </svg>
-                      </a>
-                    </span>
-                  </div>
-                </div>
-                <div class="mb-2">
-                  <label class="form-check">
-                    <input type="checkbox" class="form-check-input" />
-                    {{ form.rememberme(class="form-check-input", type="checkbox", checked=True) }}
-                    <span class="form-check-label">Remember me on this device</span>
-                  </label>
-                </div>
-                <div class="form-footer">
-                  <button name="login" type="submit" class="btn btn-primary w-100">Sign in</button>
-                </div>
-              </form>
-            </div>
-            <div class="hr-text">or</div>
-            <div class="card-body">
-              {% for oauth_name, provider in oauths_info.items() %}
-              <div class="row mb-3">
-                <a class="btn w-100" href="{{ url_for('auth_bp.oauth_login', oauth_name=oauth_name) }}">
-                  <img class="icon text-{{provider}}" width="24" height="24" alt="{{provider}} Login"
-                    src="{{ url_for('root_bp.static', filename='brands/' + provider + '.svg') }}">
-                  Login with {{provider.capitalize()}} by {{oauth_name}}
-                </a>
-              </div>
-              {% endfor %}
-            </div>
-          </div>
-          <div class="text-center text-muted mt-3">
-            Don't have account yet? <a href="{{ url_for('auth_bp.register') }}" tabindex="-1">Sign up</a>
-          </div>
-        </div>
-      </div>
-      <div class="col-lg d-none d-lg-block">
-        <img src="/static/illustrations/undraw_sign_in_e6hj.svg" height="300" class="d-block mx-auto" alt="">
-      </div>
-    </div>
-  </div>
-</div>
-{% endblock page_body %}
-
-<!-- Specific Page JS goes HERE  -->
+<!--
+* Tabler - Premium and Open Source dashboard template with responsive and high quality UI.
+* @version 1.0.0-beta19
+* @link https://tabler.io
+* Copyright 2018-2023 The Tabler Authors
+* Copyright 2018-2023 codecalm.net Paweł Kuna
+* Licensed under MIT (https://github.com/tabler/tabler/blob/master/LICENSE)
+-->
+
+{% extends "layouts/base-fullscreen.html" %}
+
+{% block title %} Sign IN {% endblock %}
+
+<!-- Specific Page CSS goes HERE  -->
+{% block stylesheets %}{% endblock stylesheets %}
+
+{% block page_header %}{% endblock page_header %}
+
+{% block page_body %}
+<div class="page page-center">
+  <div class="container container-normal py-4">
+    <div class="row align-items-center g-4">
+      <div class="col-lg">
+        <div class="container-tight">
+          {% with config=config %}
+          {% include 'logo.html' %}
+          {% endwith %}
+          <div class="card card-md">
+            <div class="card-body">
+              <h2 class="h2 text-center mb-4">Login to {{ config.APP_NAME }}</h2>
+              <!-- Flash Messages -->
+              <div class="text-left">
+                {% with messages = get_flashed_messages(with_categories=true) %}
+                {% if messages %}
+                <div class="alert-container">
+                  {% for category, message in messages %}
+                  <div class="alert alert-{{ category }} fade show" role="alert">
+                    {{ message }}
+                    <!-- <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button> -->
+                  </div>
+                  {% endfor %}
+                </div>
+                {% endif %}
+                {% endwith %}
+              </div>
+              <form id="login" action="{{ url_for('auth_bp.login') }}" method="post" autocomplete="off" novalidate>
+                {{ form.hidden_tag() }}
+                <div class="mb-3">
+                  <label class="form-label">Email</label>
+                  {{ form.email(placeholder="Email", class="form-control") }}
+                </div>
+                <div class="mb-2">
+                  <label class="form-label">
+                    Password
+                    <span class="form-label-description">
+                      <a href="{{ url_for('auth_bp.resetpass') }}">I forgot password</a>
+                    </span>
+                  </label>
+                  <div class="input-group input-group-flat">
+                    {{ form.password(placeholder="Password", class="form-control", type="password") }}
+                    <span class="input-group-text">
+                      <a href="#" id="show-password" class="link-secondary" title="Show password"
+                        data-bs-toggle="tooltip"><!-- Download SVG icon from http://tabler-icons.io/i/eye -->
+                        <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24"
+                          stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round"
+                          stroke-linejoin="round">
+                          <path stroke="none" d="M0 0h24v24H0z" fill="none" />
+                          <path d="M10 12a2 2 0 1 0 4 0a2 2 0 0 0 -4 0" />
+                          <path d="M21 12c-2.4 4 -5.4 6 -9 6c-3.6 0 -6.6 -2 -9 -6c2.4 -4 5.4 -6 9 -6c3.6 0 6.6 2 9 6" />
+                        </svg>
+                      </a>
+                    </span>
+                  </div>
+                </div>
+                <div class="mb-2">
+                  <label class="form-check">
+                    <input type="checkbox" class="form-check-input" />
+                    {{ form.rememberme(class="form-check-input", type="checkbox", checked=True) }}
+                    <span class="form-check-label">Remember me on this device</span>
+                  </label>
+                </div>
+                <div class="form-footer">
+                  <button name="login" type="submit" class="btn btn-primary w-100">Sign in</button>
+                </div>
+              </form>
+            </div>
+            <div class="hr-text">or</div>
+            <div class="card-body">
+              {% for oauth_name, provider in oauths_info.items() %}
+              <div class="row mb-3">
+                <a class="btn w-100" href="{{ url_for('auth_bp.oauth_login', oauth_name=oauth_name) }}">
+                  <img class="icon text-{{provider}}" width="24" height="24" alt="{{provider}} Login"
+                    src="{{ url_for('root_bp.static', filename='brands/' + provider + '.svg') }}">
+                  Login with {{provider.capitalize()}} by {{oauth_name}}
+                </a>
+              </div>
+              {% endfor %}
+            </div>
+          </div>
+          <div class="text-center text-muted mt-3">
+            Don't have account yet? <a href="{{ url_for('auth_bp.register') }}" tabindex="-1">Sign up</a>
+          </div>
+        </div>
+      </div>
+      <div class="col-lg d-none d-lg-block">
+        <img src="/static/illustrations/undraw_sign_in_e6hj.svg" height="300" class="d-block mx-auto" alt="">
+      </div>
+    </div>
+  </div>
+</div>
+{% endblock page_body %}
+
+<!-- Specific Page JS goes HERE  -->
 {% block javascripts %}{% endblock javascripts %}
```

## funlab/auth/templates/sign-in.html

 * *Ordering differences only*

```diff
@@ -1,104 +1,104 @@
-<!--
-* Tabler - Premium and Open Source dashboard template with responsive and high quality UI.
-* @version 1.0.0-beta19
-* @link https://tabler.io
-* Copyright 2018-2023 The Tabler Authors
-* Copyright 2018-2023 codecalm.net Paweł Kuna
-* Licensed under MIT (https://github.com/tabler/tabler/blob/master/LICENSE)
--->
-
-{% extends "layouts/base-fullscreen.html" %}
-
-{% block title %} Sign IN {% endblock %}
-
-<!-- Specific Page CSS goes HERE  -->
-{% block stylesheets %}{% endblock stylesheets %}
-
-{% block page_header %}{% endblock page_header %}
-
-{% block page_body %}
-<div class="page page-center">
-  <div class="container container-tight py-4">
-    {% with config=config %}
-    {% include 'logo.html' %}
-    {% endwith %}
-    <div class="card card-md">
-      <div class="card-body">
-        <h2 class="h2 text-center mb-4">Login to {{ config.APP_NAME }}</h2>
-        <!-- Flash Messages -->
-        <div class="text-left">
-          {% with messages = get_flashed_messages(with_categories=true) %}
-          {% if messages %}
-          <div class="alert-container">
-            {% for category, message in messages %}
-            <div class="alert alert-{{ category }} fade show" role="alert">
-              {{ message }}
-              <!-- <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button> -->
-            </div>
-            {% endfor %}
-          </div>
-          {% endif %}
-          {% endwith %}
-        </div>
-        <form id="login" action="{{ url_for('auth_bp.login') }}" method="post" autocomplete="off" novalidate>
-          {{ form.hidden_tag() }}
-          <div class="mb-3">
-            <label class="form-label">Email</label>
-            {{ form.email(placeholder="Email", class="form-control") }}
-          </div>
-          <div class="mb-2">
-            <label class="form-label">
-              Password
-              <span class="form-label-description">
-                <a href="{{ url_for('auth_bp.resetpass') }}">I forgot password</a>
-              </span>
-            </label>
-            <div class="input-group input-group-flat">
-              {{ form.password(placeholder="Password", class="form-control", type="password") }}
-              <span class="input-group-text">
-                <a href="#" id="show-password" class="link-secondary" title="Show password"
-                  data-bs-toggle="tooltip"><!-- Download SVG icon from http://tabler-icons.io/i/eye -->
-                  <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24"
-                    stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
-                    <path stroke="none" d="M0 0h24v24H0z" fill="none" />
-                    <path d="M10 12a2 2 0 1 0 4 0a2 2 0 0 0 -4 0" />
-                    <path d="M21 12c-2.4 4 -5.4 6 -9 6c-3.6 0 -6.6 -2 -9 -6c2.4 -4 5.4 -6 9 -6c3.6 0 6.6 2 9 6" />
-                  </svg>
-                </a>
-              </span>
-            </div>
-          </div>
-          <div class="mb-2">
-            <label class="form-check">
-              <input type="checkbox" class="form-check-input" />
-              {{ form.rememberme(class="form-check-input", type="checkbox", checked=True) }}
-              <span class="form-check-label">Remember me on this device</span>
-            </label>
-          </div>
-          <div class="form-footer">
-            <button name="login" type="submit" class="btn btn-primary w-100">Sign in</button>
-          </div>
-        </form>
-      </div>
-      {% if oauths_info %}
-      <div class="hr-text">or</div>
-      <div class="card-body">
-        {% for oauth_name, provider in oauths_info.items() %}
-        <div class="row mb-3">
-          <a class="btn w-100" href="{{ url_for('auth_bp.oauth_login', oauth_name=oauth_name) }}">
-            <img class="icon text-{{provider}}" width="24" height="24" alt="{{provider}} Login"
-              src="{{ url_for('root_bp.static', filename='brands/' + provider + '.svg') }}">
-            Login with {{provider.capitalize()}} by {{oauth_name}}
-          </a>
-        </div>
-        {% endfor %}
-      </div>
-      {% endif %}
-    </div>
-    <div class="text-center text-muted mt-3">
-      Don't have account yet? <a href="{{ url_for('auth_bp.register') }}" tabindex="-1">Sign up</a>
-    </div>
-  </div>
-</div>
-
+<!--
+* Tabler - Premium and Open Source dashboard template with responsive and high quality UI.
+* @version 1.0.0-beta19
+* @link https://tabler.io
+* Copyright 2018-2023 The Tabler Authors
+* Copyright 2018-2023 codecalm.net Paweł Kuna
+* Licensed under MIT (https://github.com/tabler/tabler/blob/master/LICENSE)
+-->
+
+{% extends "layouts/base-fullscreen.html" %}
+
+{% block title %} Sign IN {% endblock %}
+
+<!-- Specific Page CSS goes HERE  -->
+{% block stylesheets %}{% endblock stylesheets %}
+
+{% block page_header %}{% endblock page_header %}
+
+{% block page_body %}
+<div class="page page-center">
+  <div class="container container-tight py-4">
+    {% with config=config %}
+    {% include 'logo.html' %}
+    {% endwith %}
+    <div class="card card-md">
+      <div class="card-body">
+        <h2 class="h2 text-center mb-4">Login to {{ config.APP_NAME }}</h2>
+        <!-- Flash Messages -->
+        <div class="text-left">
+          {% with messages = get_flashed_messages(with_categories=true) %}
+          {% if messages %}
+          <div class="alert-container">
+            {% for category, message in messages %}
+            <div class="alert alert-{{ category }} fade show" role="alert">
+              {{ message }}
+              <!-- <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button> -->
+            </div>
+            {% endfor %}
+          </div>
+          {% endif %}
+          {% endwith %}
+        </div>
+        <form id="login" action="{{ url_for('auth_bp.login') }}" method="post" autocomplete="off" novalidate>
+          {{ form.hidden_tag() }}
+          <div class="mb-3">
+            <label class="form-label">Email</label>
+            {{ form.email(placeholder="Email", class="form-control") }}
+          </div>
+          <div class="mb-2">
+            <label class="form-label">
+              Password
+              <span class="form-label-description">
+                <a href="{{ url_for('auth_bp.resetpass') }}">I forgot password</a>
+              </span>
+            </label>
+            <div class="input-group input-group-flat">
+              {{ form.password(placeholder="Password", class="form-control", type="password") }}
+              <span class="input-group-text">
+                <a href="#" id="show-password" class="link-secondary" title="Show password"
+                  data-bs-toggle="tooltip"><!-- Download SVG icon from http://tabler-icons.io/i/eye -->
+                  <svg xmlns="http://www.w3.org/2000/svg" class="icon" width="24" height="24" viewBox="0 0 24 24"
+                    stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">
+                    <path stroke="none" d="M0 0h24v24H0z" fill="none" />
+                    <path d="M10 12a2 2 0 1 0 4 0a2 2 0 0 0 -4 0" />
+                    <path d="M21 12c-2.4 4 -5.4 6 -9 6c-3.6 0 -6.6 -2 -9 -6c2.4 -4 5.4 -6 9 -6c3.6 0 6.6 2 9 6" />
+                  </svg>
+                </a>
+              </span>
+            </div>
+          </div>
+          <div class="mb-2">
+            <label class="form-check">
+              <input type="checkbox" class="form-check-input" />
+              {{ form.rememberme(class="form-check-input", type="checkbox", checked=True) }}
+              <span class="form-check-label">Remember me on this device</span>
+            </label>
+          </div>
+          <div class="form-footer">
+            <button name="login" type="submit" class="btn btn-primary w-100">Sign in</button>
+          </div>
+        </form>
+      </div>
+      {% if oauths_info %}
+      <div class="hr-text">or</div>
+      <div class="card-body">
+        {% for oauth_name, provider in oauths_info.items() %}
+        <div class="row mb-3">
+          <a class="btn w-100" href="{{ url_for('auth_bp.oauth_login', oauth_name=oauth_name) }}">
+            <img class="icon text-{{provider}}" width="24" height="24" alt="{{provider}} Login"
+              src="{{ url_for('root_bp.static', filename='brands/' + provider + '.svg') }}">
+            Login with {{provider.capitalize()}} by {{oauth_name}}
+          </a>
+        </div>
+        {% endfor %}
+      </div>
+      {% endif %}
+    </div>
+    <div class="text-center text-muted mt-3">
+      Don't have account yet? <a href="{{ url_for('auth_bp.register') }}" tabindex="-1">Sign up</a>
+    </div>
+  </div>
+</div>
+
 {% endblock page_body %}
```

## funlab/auth/user.py

```diff
@@ -1,38 +1,49 @@
 from __future__ import annotations
 
 import base64
 from dataclasses import dataclass, field
 
 import bcrypt
+import enum
 from sqlalchemy import Boolean, Column, Integer, String, UniqueConstraint
 from sqlalchemy import or_, select
+from sqlalchemy import Enum as SQLEnum
 from sqlalchemy.orm import Session
+from sqlalchemy.ext.hybrid import hybrid_property
 
 # all of application's entity, use same registry to declarate
-from funlab.flaskr.app import APP_ENTITIES_REGISTRY as entities_registry
+# from funlab.flaskr.app import APP_ENTITIES_REGISTRY as entities_registry
+from funlab.core.appbase import APP_ENTITIES_REGISTRY as entities_registry
 
 def load_user(id_email, sa_session:Session)->UserEntity:
     stmt = select(UserEntity).where(or_(UserEntity.id == id_email
                                         , UserEntity.email == id_email, ))
     return sa_session.execute(stmt).scalar()
 
 def save_user(user:UserEntity, sa_session:Session):
     sa_session.merge(user)
     sa_session.commit()
 
+class RoleEnum(enum.Enum):
+    GUEST = 'GUEST'
+    USER = 'USER'
+    MANAGER = 'MANAGER'
+    SUPERVISOR = 'SUPERVISOR'
+
 @dataclass
 class User:
     id:int = field(init=False)
     email:str  # this what we use to login, not username
     username:str  # just a name
     password:str
     avatar_url:str
     state:str # = field(init=False)
     is_admin:bool =  field(init=False)
+    # role: RoleEnum = field(init=False)
     role: str = field(init=False)
 
     def __post_init__(self):
         self.is_admin = False
         if getattr(self, 'password', None) is None:
             self.password = 'account+is+from+external+authentication+provider!!!'
         self.hash_pass()
@@ -102,22 +113,27 @@
     username: str = field(metadata={'sa': Column(String, nullable=False)})
     email: str = field(metadata={'sa': Column(String, nullable=False, unique=True, index=True)})
     password: str = field(metadata={'sa': Column(String, nullable=False)})
     avatar_url:str = field(metadata={'sa': Column(String)})
     state:str = field(metadata={'sa': Column(String)})
     is_admin:bool = field(init=False, metadata={'sa': Column(Boolean)})
     role: str = field(init=False, metadata={'sa': Column(String)})
+    # role: RoleEnum = field(init=False, metadata={'sa': Column(SQLEnum(RoleEnum))})  # Use the Enum for the role column
 
     __mapper_args__ = {
         "polymorphic_identity": "user",
         "polymorphic_on": "role",
     }
 
     __table_args__ = (UniqueConstraint('email', name='_user_email_uc'),)
 
+    @hybrid_property
+    def is_active(self):
+        return self.state=='active'
+
     def merge_userdata(self, oauth_user:OAuthUser):
         updated=False
         for attr in vars(oauth_user):
             if attr in oauth_user.external_attrs:
                 if hasattr(self, attr) and getattr(self, attr)!=getattr(oauth_user, attr):
                     setattr(self, attr, getattr(oauth_user, attr))  # user update google
                     updated=True
```

## funlab/auth/view.py

```diff
@@ -1,235 +1,239 @@
-
-from authlib.integrations.flask_client import OAuth
-from flask import (flash, redirect, render_template, request,
-                    session, url_for)
-from flask_login import current_user, login_required, login_user, logout_user
-from funlab.flaskr.app import FunlabFlask
-
-from funlab.flaskr.menu import MenuDivider, MenuItem
-from funlab.flaskr.plugin import SecurityPlugin
-from funlab.core import config
-
-from .forms import AddUserForm, LoginForm, ResetPassForm
-from .user import OAuthUser, UserEntity, load_user, save_user, entities_registry
-import copy
-
-class AuthView(SecurityPlugin):
-    def __init__(self, app:FunlabFlask):
-        super().__init__(app, url_prefix="")
-        oauth = OAuth(app)
-        oauth_configs:config.Config = self.plugin_config
-        self.oauths:dict[str:dict] = {}
-        default_userinfo_keys = {'email':'email', 'username':'username', 'avatar_url':'avatar_url'}
-        try:
-            for oauth_name in oauth_configs.keys(): #  oauth_names:
-                oauth_cfg = oauth_configs.get(oauth_name)
-                provider = oauth_cfg.pop('provider')
-                userinfo_key_mapping =  copy.copy(default_userinfo_keys)
-                userinfo_key_mapping.update(oauth_cfg.pop('userinfo_key_mapping', {}))
-                oauth_register = oauth.register(name=oauth_name, **oauth_cfg)
-                self.oauths.update({oauth_name: {'provider':provider, 'register':oauth_register, 'userinfo_key_mapping':userinfo_key_mapping}})
-        except Exception as e:
-            msg = f'{oauth_name} OAuth register fail, please check config:{oauth_cfg}'
-            raise e from Exception(msg)
-        self.oauth_name_inuse:str = None
-        self.app.add_usermenu([MenuItem(title='Settings',
-                            icon='<svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-settings" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">\
-                                    <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>\
-                                    <path d="M10.325 4.317c.426 -1.756 2.924 -1.756 3.35 0a1.724 1.724 0 0 0 2.573 1.066c1.543 -.94 3.31 .826 2.37 2.37a1.724 1.724 0 0 0 1.065 2.572c1.756 .426 1.756 2.924 0 3.35a1.724 1.724 0 0 0 -1.066 2.573c.94 1.543 -.826 3.31 -2.37 2.37a1.724 1.724 0 0 0 -2.572 1.065c-.426 1.756 -2.924 1.756 -3.35 0a1.724 1.724 0 0 0 -2.573 -1.066c-1.543 .94 -3.31 -.826 -2.37 -2.37a1.724 1.724 0 0 0 -1.065 -2.572c-1.756 -.426 -1.756 -2.924 0 -3.35a1.724 1.724 0 0 0 1.066 -2.573c-.94 -1.543 .826 -3.31 2.37 -2.37c1 .608 2.296 .07 2.572 -1.065z"></path>\
-                                    <path d="M9 12a3 3 0 1 0 6 0a3 3 0 0 0 -6 0"></path>\
-                                    </svg>',
-                            href=f'/settings'),
-                            MenuDivider(),
-                            MenuItem(title='Logout',
-                                icon='<svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-logout" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">\
-                                        <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>\
-                                        <path d="M14 8v-2a2 2 0 0 0 -2 -2h-7a2 2 0 0 0 -2 2v12a2 2 0 0 0 2 2h7a2 2 0 0 0 2 -2v-2"></path>\
-                                        <path d="M9 12h12l-3 -3"></path>\
-                                        <path d="M18 15l3 -3"></path>\
-                                        </svg>',
-                                href=f'/logout'),
-                            ])
-
-        self.register_routes()
-        self.register_login_handler()
-
-    @property
-    def entities_registry(self):
-        """ FunlabFlask use to table creation by sqlalchemy in __init__ for application initiation """
-        return entities_registry
-
-    @property
-    def oauths_info(self):
-        return { oauth_name:value.get('provider') for (oauth_name, value) in self.oauths.items()}
-
-    def get_oauth_register(self, oauth_name:str=None):
-        if oauth_name is None:
-            oauth_name = self.oauth_name_inuse
-        return self.oauths.get(oauth_name).get('register')
-
-    def get_userinfo_field_value(self, userinfo, fieldname):
-        return userinfo[self.oauths.get(self.oauth_name_inuse).get('userinfo_key_mapping')[fieldname]]
-
-    def register_routes(self):
-        @self.blueprint.route('/login', defaults={'style': None}, methods=['GET', 'POST'])
-        @self.blueprint.route('/login/', defaults={'style': None}, methods=['GET', 'POST'])
-        @self.blueprint.route('/login/<style>', methods=['GET', 'POST'])
-        def login(style):
-            login_form = LoginForm(request.form)
-            if 'login' in request.form:
-                email = request.form['email']
-                password = request.form['password']
-                rememberme = request.form['rememberme']
-                # Locate user
-                sa_session = self.app.dbmgr.get_db_session()
-                user = load_user(email, sa_session)
-                if user and user.verify_pass(password):
-                    login_user(user, remember=(rememberme=='y'))
-                    return redirect(url_for('root_bp.home'))
-                elif not user:
-                    flash('User email not exist. Please check.', "warning")
-                elif user.verify_pass('account+is+from+external+authentication+provider!!!'):
-                    flash('Your account is from external authentication provider, please login with proper provider below.', "info")
-                else:
-                    flash("Incorrect password. Please try again.", "warning")
-                return render_template('/sign-in.html', form=login_form, oauths_info=self.oauths_info)
-            elif current_user and current_user.is_authenticated:
-                return redirect(url_for('root_bp.home'))
-            else:
-                style = '-'+style if style else ''
-                return render_template(f'/sign-in{style}.html', form=login_form, oauths_info=self.oauths_info)
-
-        @self.blueprint.route('/oauth_login/<oauth_name>')
-        def oauth_login(oauth_name):
-            redirect_uri = url_for(f'{self.bp_name}.authorize', oauth_name=oauth_name, _external=True)
-            return self.get_oauth_register(oauth_name).authorize_redirect(redirect_uri)
-
-        @self.blueprint.route('/authorize/<oauth_name>')
-        def authorize(oauth_name):
-            try:
-                token = self.get_oauth_register(oauth_name).authorize_access_token()
-                if token is None:
-                    msg = 'Access denied: reason={0} error={1}'.format(
-                        request.args['error_reason'],
-                        request.args['error_description']
-                    )
-                    flash(f'{msg}', category='danger')
-                    return render_template('sign-in.html', form=LoginForm(), oauths_info=self.oauths_info)
-            except Exception as e:
-                flash(f'Exception:{str(e)}', category='danger')
-                return render_template('sign-in.html', form=LoginForm(), oauths_info=self.oauths_info)
-            try:
-                self.oauth_name_inuse = oauth_name
-                userinfo = self.get_oauth_register(oauth_name).userinfo()
-                oauth_user = OAuthUser(email=self.get_userinfo_field_value(userinfo, 'email'),
-                                       username=self.get_userinfo_field_value(userinfo, 'username'),
-                                       avatar_url=self.get_userinfo_field_value(userinfo, 'avatar_url'),
-                                       password=None,  state='active')
-                sa_session = self.app.dbmgr.get_db_session()
-                if (user:=load_user(oauth_user.email, sa_session)):
-                    if user.merge_userdata(oauth_user):
-                        save_user(user, sa_session)
-                else:
-                    save_user(oauth_user.to_userentity(), sa_session)
-                    user=load_user(oauth_user.email, sa_session)
-                login_user(user)
-                return redirect(url_for('root_bp.home'))
-            except Exception as e:
-                self.oauth_name_inuse = None
-                flash(f'Get userinfo from OAuth provider failed. Exception:{e}', category='danger')
-                return render_template('sign-in.html', form=LoginForm(), oauths_info=self.oauths_info)
-
-        @self.blueprint.route('/logout')
-        @login_required
-        def logout():
-            logout_user()
-            return redirect(url_for('root_bp.index'))
-
-        @self.blueprint.route('/register', methods=['GET', 'POST'])
-        def register():
-            create_account_form = AddUserForm(request.form)
-            if 'register' in request.form:
-                username = request.form['username']
-                email = request.form['email']
-                password = request.form['password']
-                sa_session = self.app.dbmgr.get_db_session()
-                user = load_user(email, sa_session)
-                if user:
-                    flash('Email already registered. Check it and register again.', category='warning')
-                    return render_template('/register.html', form=create_account_form)
-                else:
-                    user = UserEntity(username=username, email=email, password=password, avatar_url='', state='active')
-                    sa_session = self.app.dbmgr.get_db_session()
-                    sa_session.add(user)
-                    sa_session.commit()
-                    logout_user()
-                    flash("Account is created successfully. Please login.", category='success')
-                    return render_template('sign-in.html', form=LoginForm(), oauths_info=self.oauths_info)
-            else:
-                return render_template('/register.html', form=create_account_form)
-
-        @self.blueprint.route('/resetpass', methods=['GET', 'POST'])
-        def resetpass():
-            resetpass_form = ResetPassForm(request.form)
-            if 'resetpass' in request.form:
-                old_password = request.form['old_password']
-                email = request.form['email']
-                new_password = request.form['new_password']
-                confirm_password = request.form['confirm_password']
-                if new_password != confirm_password:
-                    flash('New password not consistancy. Please re-enter.', category='warning')
-                    return render_template('/resetpass.html', form=resetpass_form)
-                sa_session = self.app.dbmgr.get_db_session()
-                user = load_user(email, sa_session)
-                if user and (user.verify_pass(old_password) or user.verify_pass('account+is+from+external+authentication+provider!!!')):
-                    # sa_session = current_app.dbmgr.get_db_session()
-                    user.password = new_password
-                    user.hash_pass()
-                    save_user(user, sa_session)
-                    # sa_session.merge(user)
-                    # sa_session.commit()
-                    flash('Password reset successfully. Please login again.', category='success')
-                    return render_template('/sign-in.html', form=LoginForm(), oauths_info=self.oauths_info)
-                elif user is not None:
-                    flash('Wrong password! Please check.', category='danger')
-                    return render_template('/resetpass.html', form=resetpass_form)
-                elif user is None:
-                    flash('User email not exist. Please check.', "warning")
-                    return render_template('/resetpass.html', form=resetpass_form)
-            else:
-                return render_template('/resetpass.html', form=resetpass_form)
-
-        @self.blueprint.route('/settings')
-        @login_required
-        def settings():
-            return render_template('settings.html')
-
-    def register_login_handler(self):
-        @self.login_manager.unauthorized_handler
-        def unauthorized_handler():
-            return render_template('error-403.html'), 403
-
-        @self.login_manager.user_loader
-        def user_loader(id):
-            return load_user(id, self.app.dbmgr.get_db_session())
-
-        @self.login_manager.request_loader
-        def request_loader(request):
-            sa_session = self.app.dbmgr.get_db_session()
-            if 'user_id' in session:
-                return load_user(session['user_id'], sa_session)
-            elif self.oauth_name_inuse and (oauth_register:=self.get_oauth_register()):
-                if (token:=request.headers.get('Authorization')):
-                    oauth_register.token = token
-                elif (token:=request.args.get('google_token')):
-                    oauth_register.token = token
-
-                if oauth_register.token:
-                    try:
-                        userinfo = oauth_register.userinfo()
-                        user = load_user(self.get_userinfo_field_value(userinfo, 'email'), sa_session)
-                        return user
-                    except Exception as e:
-                        raise Exception("Oauth request_loader for oauth_register.userinfo() failed! Check") from e
-            return None
-
+
+import copy
+from authlib.integrations.flask_client import OAuth
+from flask import (flash, redirect, render_template, request,
+                    session, url_for)
+from flask_login import current_user, login_required, login_user, logout_user
+
+
+from funlab.core.menu import MenuDivider, MenuItem
+from funlab.core.plugin import SecurityPlugin
+from funlab.core.config import Config
+
+from .forms import AddUserForm, LoginForm, ResetPassForm
+from .user import OAuthUser, UserEntity, load_user, save_user, entities_registry
+from funlab.core.appbase import _FlaskBase
+
+class AuthView(SecurityPlugin):
+    def __init__(self, app:_FlaskBase):
+        super().__init__(app, url_prefix="")
+        oauth = OAuth(app)
+        oauth_configs:Config = self.plugin_config
+        self.oauths:dict[str:dict] = {}
+        default_userinfo_keys = {'email':'email', 'username':'username', 'avatar_url':'avatar_url'}
+        try:
+            for oauth_name in oauth_configs.keys(): #  oauth_names:
+                oauth_cfg = oauth_configs.get(oauth_name)
+                provider = oauth_cfg.pop('provider')
+                userinfo_key_mapping =  copy.copy(default_userinfo_keys)
+                userinfo_key_mapping.update(oauth_cfg.pop('userinfo_key_mapping', {}))
+                oauth_register = oauth.register(name=oauth_name, **oauth_cfg)
+                self.oauths.update({oauth_name: {'provider':provider, 'register':oauth_register, 'userinfo_key_mapping':userinfo_key_mapping}})
+        except Exception as e:
+            msg = f'{oauth_name} OAuth register fail, please check config:{oauth_cfg}'
+            raise e from Exception(msg)
+        self.oauth_name_inuse:str = None
+        self.app.append_usermenu([MenuItem(title='Settings',
+                            icon='<svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-settings" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">\
+                                    <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>\
+                                    <path d="M10.325 4.317c.426 -1.756 2.924 -1.756 3.35 0a1.724 1.724 0 0 0 2.573 1.066c1.543 -.94 3.31 .826 2.37 2.37a1.724 1.724 0 0 0 1.065 2.572c1.756 .426 1.756 2.924 0 3.35a1.724 1.724 0 0 0 -1.066 2.573c.94 1.543 -.826 3.31 -2.37 2.37a1.724 1.724 0 0 0 -2.572 1.065c-.426 1.756 -2.924 1.756 -3.35 0a1.724 1.724 0 0 0 -2.573 -1.066c-1.543 .94 -3.31 -.826 -2.37 -2.37a1.724 1.724 0 0 0 -1.065 -2.572c-1.756 -.426 -1.756 -2.924 0 -3.35a1.724 1.724 0 0 0 1.066 -2.573c-.94 -1.543 .826 -3.31 2.37 -2.37c1 .608 2.296 .07 2.572 -1.065z"></path>\
+                                    <path d="M9 12a3 3 0 1 0 6 0a3 3 0 0 0 -6 0"></path>\
+                                    </svg>',
+                            href=f'/settings'),
+                            MenuDivider(),
+                            MenuItem(title='Logout',
+                                icon='<svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-logout" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round">\
+                                        <path stroke="none" d="M0 0h24v24H0z" fill="none"></path>\
+                                        <path d="M14 8v-2a2 2 0 0 0 -2 -2h-7a2 2 0 0 0 -2 2v12a2 2 0 0 0 2 2h7a2 2 0 0 0 2 -2v-2"></path>\
+                                        <path d="M9 12h12l-3 -3"></path>\
+                                        <path d="M18 15l3 -3"></path>\
+                                        </svg>',
+                                href=f'/logout'),
+                            ])
+
+        self.register_routes()
+        self.register_login_handler()
+
+    @property
+    def entities_registry(self):
+        """ FunlabFlask use to table creation by sqlalchemy in __init__ for application initiation """
+        return entities_registry
+
+    @property
+    def oauths_info(self):
+        return { oauth_name:value.get('provider') for (oauth_name, value) in self.oauths.items()}
+
+    def get_oauth_register(self, oauth_name:str=None):
+        if oauth_name is None:
+            oauth_name = self.oauth_name_inuse
+        return self.oauths.get(oauth_name).get('register')
+
+    def get_userinfo_field_value(self, userinfo, fieldname):
+        return userinfo[self.oauths.get(self.oauth_name_inuse).get('userinfo_key_mapping')[fieldname]]
+
+    def register_routes(self):
+        @self.blueprint.route('/login', defaults={'style': None}, methods=['GET', 'POST'])
+        @self.blueprint.route('/login/', defaults={'style': None}, methods=['GET', 'POST'])
+        @self.blueprint.route('/login/<style>', methods=['GET', 'POST'])
+        def login(style):
+            login_form = LoginForm(request.form)
+            if 'login' in request.form:
+                email = request.form['email']
+                password = request.form['password']
+                rememberme = request.form['rememberme']
+                # Locate user
+                sa_session = self.app.dbmgr.get_db_session()
+                user = load_user(email, sa_session)
+                if user: # and user.verify_pass(password):
+                    login_user(user, remember=(rememberme=='y'))
+                    return redirect(url_for('root_bp.home'))
+                elif not user:
+                    flash('User email not exist. Please check.', "warning")
+                elif user.verify_pass('account+is+from+external+authentication+provider!!!'):
+                    flash('Your account is from external authentication provider, please login with proper provider below.', "info")
+                else:
+                    flash("Incorrect password. Please try again.", "warning")
+                return render_template('/sign-in.html', form=login_form, oauths_info=self.oauths_info)
+            elif current_user and current_user.is_authenticated:
+                return redirect(url_for('root_bp.home'))
+            else:
+                style = '-'+style if style else ''
+                return render_template(f'/sign-in{style}.html', form=login_form, oauths_info=self.oauths_info)
+
+        @self.blueprint.route('/oauth_login/<oauth_name>')
+        def oauth_login(oauth_name):
+            redirect_uri = url_for(f'{self.bp_name}.authorize', oauth_name=oauth_name, _external=True)
+            return self.get_oauth_register(oauth_name).authorize_redirect(redirect_uri)
+
+        @self.blueprint.route('/authorize/<oauth_name>')
+        def authorize(oauth_name):
+            try:
+                token = self.get_oauth_register(oauth_name).authorize_access_token()
+                if token is None:
+                    msg = 'Access denied: reason={0} error={1}'.format(
+                        request.args['error_reason'],
+                        request.args['error_description']
+                    )
+                    flash(f'{msg}', category='danger')
+                    return render_template('sign-in.html', form=LoginForm(), oauths_info=self.oauths_info)
+            except Exception as e:
+                flash(f'Exception:{str(e)}', category='danger')
+                return render_template('sign-in.html', form=LoginForm(), oauths_info=self.oauths_info)
+            try:
+                self.oauth_name_inuse = oauth_name
+                userinfo = self.get_oauth_register(oauth_name).userinfo()
+                oauth_user = OAuthUser(email=self.get_userinfo_field_value(userinfo, 'email'),
+                                       username=self.get_userinfo_field_value(userinfo, 'username'),
+                                       avatar_url=self.get_userinfo_field_value(userinfo, 'avatar_url'),
+                                       password=None,  state='active')
+                sa_session = self.app.dbmgr.get_db_session()
+                if (user:=load_user(oauth_user.email, sa_session)):
+                    if user.merge_userdata(oauth_user):
+                        save_user(user, sa_session)
+                else:
+                    save_user(oauth_user.to_userentity(), sa_session)
+                    user=load_user(oauth_user.email, sa_session)
+                session['oauth_token'] = token
+                login_user(user)
+                return redirect(url_for('root_bp.home'))
+            except Exception as e:
+                self.oauth_name_inuse = None
+                flash(f'Get userinfo from OAuth provider failed. Exception:{e}', category='danger')
+                return render_template('sign-in.html', form=LoginForm(), oauths_info=self.oauths_info)
+
+        @self.blueprint.route('/logout')
+        @login_required
+        def logout():
+            logout_user()
+            session.pop('oauth_token', None)
+            session.pop('user_id', None)
+            return redirect(url_for('root_bp.index'))
+
+        @self.blueprint.route('/register', methods=['GET', 'POST'])
+        def register():
+            create_account_form = AddUserForm(request.form)
+            if 'register' in request.form:
+                username = request.form['username']
+                email = request.form['email']
+                password = request.form['password']
+                sa_session = self.app.dbmgr.get_db_session()
+                user = load_user(email, sa_session)
+                if user:
+                    flash('Email already registered. Check it and register again.', category='warning')
+                    return render_template('/register.html', form=create_account_form)
+                else:
+                    user = UserEntity(username=username, email=email, password=password, avatar_url='', state='active')
+                    sa_session = self.app.dbmgr.get_db_session()
+                    sa_session.add(user)
+                    sa_session.commit()
+                    logout_user()
+                    flash("Account is created successfully. Please login.", category='success')
+                    return render_template('sign-in.html', form=LoginForm(), oauths_info=self.oauths_info)
+            else:
+                return render_template('/register.html', form=create_account_form)
+
+        @self.blueprint.route('/resetpass', methods=['GET', 'POST'])
+        def resetpass():
+            resetpass_form = ResetPassForm(request.form)
+            if 'resetpass' in request.form:
+                old_password = request.form['old_password']
+                email = request.form['email']
+                new_password = request.form['new_password']
+                confirm_password = request.form['confirm_password']
+                if new_password != confirm_password:
+                    flash('New password not consistancy. Please re-enter.', category='warning')
+                    return render_template('/resetpass.html', form=resetpass_form)
+                sa_session = self.app.dbmgr.get_db_session()
+                user = load_user(email, sa_session)
+                if user and (user.verify_pass(old_password) or user.verify_pass('account+is+from+external+authentication+provider!!!')):
+                    # sa_session = current_app.dbmgr.get_db_session()
+                    user.password = new_password
+                    user.hash_pass()
+                    save_user(user, sa_session)
+                    # sa_session.merge(user)
+                    # sa_session.commit()
+                    flash('Password reset successfully. Please login again.', category='success')
+                    return render_template('/sign-in.html', form=LoginForm(), oauths_info=self.oauths_info)
+                elif user is not None:
+                    flash('Wrong password! Please check.', category='danger')
+                    return render_template('/resetpass.html', form=resetpass_form)
+                elif user is None:
+                    flash('User email not exist. Please check.', "warning")
+                    return render_template('/resetpass.html', form=resetpass_form)
+            else:
+                return render_template('/resetpass.html', form=resetpass_form)
+
+        @self.blueprint.route('/settings')
+        @login_required
+        def settings():
+            return render_template('settings.html')
+
+    def register_login_handler(self):
+        @self.login_manager.unauthorized_handler
+        def unauthorized_handler():
+            return render_template('error-403.html'), 403
+
+        @self.login_manager.user_loader
+        def user_loader(id):
+            return load_user(id, self.app.dbmgr.get_db_session())
+
+        @self.login_manager.request_loader
+        def request_loader(request):
+            sa_session = self.app.dbmgr.get_db_session()
+            if 'user_id' in session:
+                return load_user(session['user_id'], sa_session)
+            elif self.oauth_name_inuse and (oauth_register:=self.get_oauth_register()):
+                if (token:=request.headers.get('Authorization')):
+                    oauth_register.token = token
+                elif (token:=request.args.get('google_token')):
+                    oauth_register.token = token
+
+                if oauth_register.token:
+                    try:
+                        userinfo = oauth_register.userinfo()
+                        user = load_user(self.get_userinfo_field_value(userinfo, 'email'), sa_session)
+                        return user
+                    except Exception as e:
+                        raise Exception("Oauth request_loader for oauth_register.userinfo() failed! Check") from e
+            return None
+
```

## Comparing `funlab_auth-0.2.5.dist-info/LICENSE` & `funlab_auth-0.2.6.dist-info/LICENSE`

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

## Comparing `funlab_auth-0.2.5.dist-info/METADATA` & `funlab_auth-0.2.6.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: funlab-auth
-Version: 0.2.5
+Version: 0.2.6
 Summary: A funlab-flaskr plugin provide authentication mechenism.
+Home-page: https://github.com/python-poetry/poetry
 License: MIT
 Author: SunnyLin
 Author-email: 013.lin@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: authlib (>=1.3.0,<2.0.0)
 Requires-Dist: bcrypt (>=4.1.2,<5.0.0)
 Requires-Dist: flask-wtf (>=1.2.1,<2.0.0)
-Requires-Dist: funlab-flaskr (>=0.2.3,<0.3.0)
+Requires-Dist: funlab-flaskr (>=0.3.7,<0.4.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Repository, https://github.com/python-poetry/poetry
 Description-Content-Type: text/markdown
 
 # A funlab-flaskr plugin provide authentication mechenism
 
 ## Installation
 
 pip install funlab-auth
```

