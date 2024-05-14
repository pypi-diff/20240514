# Comparing `tmp/cae_cli-0.2.8.tar.gz` & `tmp/cae_cli-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.2.8.tar", last modified: Thu May  9 22:46:51 2024, max compression
+gzip compressed data, was "cae_cli-0.2.9.tar", last modified: Tue May 14 19:33:47 2024, max compression
```

## Comparing `cae_cli-0.2.8.tar` & `cae_cli-0.2.9.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 22:46:51.605070 cae_cli-0.2.8/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.8/LICENSE
--rw-rw-rw-   0        0        0      415 2024-05-09 22:46:51.604071 cae_cli-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 22:46:51.473104 cae_cli-0.2.8/cae/
--rw-rw-rw-   0        0        0     9506 2024-05-09 22:42:15.000000 cae_cli-0.2.8/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.8/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.8/cae/__init__.py
--rw-rw-rw-   0        0        0    10247 2024-05-09 22:46:38.000000 cae_cli-0.2.8/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-09 22:46:51.588497 cae_cli-0.2.8/cae/templates/
--rw-rw-rw-   0        0        0     1170 2024-05-09 02:44:28.000000 cae_cli-0.2.8/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.8/cae/templates/entity.txt
--rw-rw-rw-   0        0        0      770 2024-05-09 02:30:03.000000 cae_cli-0.2.8/cae/templates/entityFactory.txt
--rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.8/cae/templates/entityImplementation.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.8/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      794 2024-05-09 02:03:37.000000 cae_cli-0.2.8/cae/templates/implementation_ruc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.8/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.2.8/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.8/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1945 2024-05-09 22:31:57.000000 cae_cli-0.2.8/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.8/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-09 02:30:03.000000 cae_cli-0.2.8/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.8/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.8/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.8/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      236 2024-05-09 02:34:53.000000 cae_cli-0.2.8/cae/templates/use_case_ruc.txt
--rw-rw-rw-   0        0        0      408 2024-05-09 02:34:53.000000 cae_cli-0.2.8/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 22:46:51.603069 cae_cli-0.2.8/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      415 2024-05-09 22:46:51.000000 cae_cli-0.2.8/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      797 2024-05-09 22:46:51.000000 cae_cli-0.2.8/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 22:46:51.000000 cae_cli-0.2.8/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-09 22:46:51.000000 cae_cli-0.2.8/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-09 22:46:51.000000 cae_cli-0.2.8/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 22:46:51.605070 cae_cli-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      610 2024-05-09 22:46:38.000000 cae_cli-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-14 19:33:47.586631 cae_cli-0.2.9/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      415 2024-05-14 19:33:47.585625 cae_cli-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-14 19:33:47.445127 cae_cli-0.2.9/cae/
+-rw-rw-rw-   0        0        0     9506 2024-05-09 22:42:15.000000 cae_cli-0.2.9/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.9/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.9/cae/__init__.py
+-rw-rw-rw-   0        0        0    10247 2024-05-09 22:46:38.000000 cae_cli-0.2.9/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-14 19:33:47.561928 cae_cli-0.2.9/cae/templates/
+-rw-rw-rw-   0        0        0     1000 2024-05-14 19:33:43.000000 cae_cli-0.2.9/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.9/cae/templates/dependency_wrapper.txt
+-rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.9/cae/templates/entity.txt
+-rw-rw-rw-   0        0        0      770 2024-05-09 02:30:03.000000 cae_cli-0.2.9/cae/templates/entityFactory.txt
+-rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.9/cae/templates/entityImplementation.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.9/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      794 2024-05-09 02:03:37.000000 cae_cli-0.2.9/cae/templates/implementation_ruc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.9/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1737 2024-05-14 19:27:43.000000 cae_cli-0.2.9/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.9/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1945 2024-05-09 22:31:57.000000 cae_cli-0.2.9/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.9/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-09 02:30:03.000000 cae_cli-0.2.9/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.9/cae/templates/use_case_factory.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.9/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.9/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.9/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      236 2024-05-09 02:34:53.000000 cae_cli-0.2.9/cae/templates/use_case_ruc.txt
+-rw-rw-rw-   0        0        0      408 2024-05-09 02:34:53.000000 cae_cli-0.2.9/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-14 19:33:47.584624 cae_cli-0.2.9/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-05-14 19:33:47.000000 cae_cli-0.2.9/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      869 2024-05-14 19:33:47.000000 cae_cli-0.2.9/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-14 19:33:47.000000 cae_cli-0.2.9/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-14 19:33:47.000000 cae_cli-0.2.9/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-14 19:33:47.000000 cae_cli-0.2.9/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-14 19:33:47.586631 cae_cli-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      610 2024-05-14 19:33:43.000000 cae_cli-0.2.9/setup.py
```

### Comparing `cae_cli-0.2.8/LICENSE` & `cae_cli-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.8/README.md` & `cae_cli-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.8/cae/ArchFlowJavaWeb.py` & `cae_cli-0.2.9/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.8/cae/db.json` & `cae_cli-0.2.9/cae/db.json`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.8/cae/templates/assembler.txt` & `cae_cli-0.2.9/cae/templates/assembler.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,22 +7,14 @@
 import lombok.NoArgsConstructor;
 
 @NoArgsConstructor(access = AccessLevel.PRIVATE)
 public class <pc>args[0]</pc>UseCaseAssembler implements UseCaseAssembler<<pc>args[0]</pc>UseCase>{
 
     public static final <pc>args[0]</pc>UseCaseAssembler SINGLETON_ASSEMBLER = new <pc>args[0]</pc>UseCaseAssembler();
 
-    public static final <pc>args[0]</pc>UseCase V1;
-
-    static {
-        V1 = <pc>args[0]</pc>UseCaseAssembler.initializeV1();
-    }
-
-    private static <pc>args[0]</pc>UseCase initializeV1(){
-        return new <pc>args[0]</pc>UseCaseImplementation();
-    }
+    public static final <pc>args[0]</pc>UseCase V1 = new <pc>args[0]</pc>UseCaseImplementation();
 
     @Override
     public <pc>args[0]</pc>UseCase getDefaultAssembledInstance(){
         return V1;
     }
 }
```

### Comparing `cae_cli-0.2.8/cae/templates/entityFactory.txt` & `cae_cli-0.2.9/cae/templates/entityFactory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.8/cae/templates/implementation_cuc.txt` & `cae_cli-0.2.9/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.8/cae/templates/implementation_ruc.txt` & `cae_cli-0.2.9/cae/templates/implementation_ruc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.8/cae/templates/implementation_suc.txt` & `cae_cli-0.2.9/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.8/cae/templates/pom-adapters.txt` & `cae_cli-0.2.9/cae/templates/pom-adapters.txt`

 * *Files 1% similar despite different names*

#### Comparing `cae_cli-0.2.8/cae/templates/pom-adapters.txt` & `cae_cli-0.2.9/cae/templates/pom-adapters.txt`

```diff
@@ -44,11 +44,11 @@
         <kc>args[1]-core</kc>
       </artifactId>
       <version>1.0-SNAPSHOT</version>
     </dependency>
     <dependency>
       <groupId>ch.qos.logback</groupId>
       <artifactId>logback-classic</artifactId>
-      <version>1.4.7</version>
+      <version>1.4.12</version>
     </dependency>
   </dependencies>
 </project>
```

### Comparing `cae_cli-0.2.8/cae/templates/pom-assemblers.txt` & `cae_cli-0.2.9/cae/templates/pom-assemblers.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.8/cae/templates/pom-core.txt` & `cae_cli-0.2.9/cae/templates/pom-core.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.8/cae/templates/use_case.txt` & `cae_cli-0.2.9/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.8/cae/templates/use_case_implementation.txt` & `cae_cli-0.2.9/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.8/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.2.9/cae_cli.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 README.md
 setup.py
 cae/ArchFlowJavaWeb.py
 cae/Run.py
 cae/__init__.py
 cae/db.json
 cae/templates/assembler.txt
+cae/templates/dependency_wrapper.txt
 cae/templates/entity.txt
 cae/templates/entityFactory.txt
 cae/templates/entityImplementation.txt
 cae/templates/implementation_cuc.txt
 cae/templates/implementation_ruc.txt
 cae/templates/implementation_suc.txt
 cae/templates/pom-adapters.txt
 cae/templates/pom-assemblers.txt
 cae/templates/pom-core.txt
 cae/templates/use_case.txt
 cae/templates/use_case_cuc.txt
+cae/templates/use_case_factory.txt
 cae/templates/use_case_implementation.txt
 cae/templates/use_case_input.txt
 cae/templates/use_case_output.txt
 cae/templates/use_case_ruc.txt
 cae/templates/use_case_suc.txt
 cae_cli.egg-info/PKG-INFO
 cae_cli.egg-info/SOURCES.txt
```

### Comparing `cae_cli-0.2.8/setup.py` & `cae_cli-0.2.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.2.8',
+    version='0.2.9',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
```

