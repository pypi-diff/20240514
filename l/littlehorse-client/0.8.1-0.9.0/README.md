# Comparing `tmp/littlehorse_client-0.8.1.tar.gz` & `tmp/littlehorse_client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "littlehorse_client-0.8.1.tar", max compression
+gzip compressed data, was "littlehorse_client-0.9.0.tar", max compression
```

## Comparing `littlehorse_client-0.8.1.tar` & `littlehorse_client-0.9.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      860 2024-03-26 09:04:31.832931 littlehorse_client-0.8.1/README.md
--rw-r--r--   0        0        0      648 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/__init__.py
--rw-r--r--   0        0        0     5262 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/auth.py
--rw-r--r--   0        0        0    13731 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/config.py
--rw-r--r--   0        0        0      868 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/exceptions.py
--rw-r--r--   0        0        0     4627 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/acls_pb2.py
--rw-r--r--   0        0        0     5121 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/acls_pb2.pyi
--rw-r--r--   0        0        0     3031 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/common_enums_pb2.py
--rw-r--r--   0        0        0     3194 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/common_enums_pb2.pyi
--rw-r--r--   0        0        0     6656 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/common_wfspec_pb2.py
--rw-r--r--   0        0        0     8613 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/common_wfspec_pb2.pyi
--rw-r--r--   0        0        0     2583 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/external_event_pb2.py
--rw-r--r--   0        0        0     2248 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/external_event_pb2.pyi
--rw-r--r--   0        0        0     7014 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/node_run_pb2.py
--rw-r--r--   0        0        0     9762 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/node_run_pb2.pyi
--rw-r--r--   0        0        0     5304 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/object_id_pb2.py
--rw-r--r--   0        0        0     6398 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/object_id_pb2.pyi
--rw-r--r--   0        0        0    34382 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/service_pb2.py
--rw-r--r--   0        0        0    40658 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/service_pb2.pyi
--rw-r--r--   0        0        0    93203 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/service_pb2_grpc.py
--rw-r--r--   0        0        0     1687 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/task_def_pb2.py
--rw-r--r--   0        0        0     1151 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/task_def_pb2.pyi
--rw-r--r--   0        0        0     4867 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/task_run_pb2.py
--rw-r--r--   0        0        0     6233 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/task_run_pb2.pyi
--rw-r--r--   0        0        0     7136 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/user_tasks_pb2.py
--rw-r--r--   0        0        0     8973 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/user_tasks_pb2.pyi
--rw-r--r--   0        0        0     2120 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/variable_pb2.py
--rw-r--r--   0        0        0     1807 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/variable_pb2.pyi
--rw-r--r--   0        0        0     6480 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/wf_run_pb2.py
--rw-r--r--   0        0        0     9647 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/wf_run_pb2.pyi
--rw-r--r--   0        0        0    14866 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/wf_spec_pb2.py
--rw-r--r--   0        0        0    20689 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/wf_spec_pb2.pyi
--rw-r--r--   0        0        0     2150 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/workflow_event_pb2.py
--rw-r--r--   0        0        0     1643 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/model/workflow_event_pb2.pyi
--rw-r--r--   0        0        0     5539 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/utils.py
--rw-r--r--   0        0        0    22629 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/worker.py
--rw-r--r--   0        0        0    65683 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/littlehorse/workflow.py
--rw-r--r--   0        0        0     1343 2024-03-26 09:04:31.836931 littlehorse_client-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1940 1970-01-01 00:00:00.000000 littlehorse_client-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      860 2024-05-14 20:00:04.504316 littlehorse_client-0.9.0/README.md
+-rw-r--r--   0        0        0      648 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/__init__.py
+-rw-r--r--   0        0        0     5262 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/auth.py
+-rw-r--r--   0        0        0    13731 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/config.py
+-rw-r--r--   0        0        0      868 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/exceptions.py
+-rw-r--r--   0        0        0     4676 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/acls_pb2.py
+-rw-r--r--   0        0        0     5206 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/acls_pb2.pyi
+-rw-r--r--   0        0        0     3031 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/common_enums_pb2.py
+-rw-r--r--   0        0        0     3194 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/common_enums_pb2.pyi
+-rw-r--r--   0        0        0     6656 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/common_wfspec_pb2.py
+-rw-r--r--   0        0        0     8613 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/common_wfspec_pb2.pyi
+-rw-r--r--   0        0        0     2583 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/external_event_pb2.py
+-rw-r--r--   0        0        0     2248 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/external_event_pb2.pyi
+-rw-r--r--   0        0        0     7014 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/node_run_pb2.py
+-rw-r--r--   0        0        0     9762 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/node_run_pb2.pyi
+-rw-r--r--   0        0        0     5304 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/object_id_pb2.py
+-rw-r--r--   0        0        0     6398 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/object_id_pb2.pyi
+-rw-r--r--   0        0        0    36601 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/service_pb2.py
+-rw-r--r--   0        0        0    43385 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/service_pb2.pyi
+-rw-r--r--   0        0        0    96335 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/service_pb2_grpc.py
+-rw-r--r--   0        0        0     1687 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/task_def_pb2.py
+-rw-r--r--   0        0        0     1151 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/task_def_pb2.pyi
+-rw-r--r--   0        0        0     4867 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/task_run_pb2.py
+-rw-r--r--   0        0        0     6233 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/task_run_pb2.pyi
+-rw-r--r--   0        0        0     7136 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/user_tasks_pb2.py
+-rw-r--r--   0        0        0     8973 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/user_tasks_pb2.pyi
+-rw-r--r--   0        0        0     2120 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/variable_pb2.py
+-rw-r--r--   0        0        0     1807 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/variable_pb2.pyi
+-rw-r--r--   0        0        0     6480 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/wf_run_pb2.py
+-rw-r--r--   0        0        0     9647 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/wf_run_pb2.pyi
+-rw-r--r--   0        0        0    14804 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/wf_spec_pb2.py
+-rw-r--r--   0        0        0    20694 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/wf_spec_pb2.pyi
+-rw-r--r--   0        0        0     2150 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/workflow_event_pb2.py
+-rw-r--r--   0        0        0     1643 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/model/workflow_event_pb2.pyi
+-rw-r--r--   0        0        0     5539 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/utils.py
+-rw-r--r--   0        0        0    22629 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/worker.py
+-rw-r--r--   0        0        0    69098 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/littlehorse/workflow.py
+-rw-r--r--   0        0        0     1343 2024-05-14 20:00:04.508316 littlehorse_client-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1940 1970-01-01 00:00:00.000000 littlehorse_client-0.9.0/PKG-INFO
```

### Comparing `littlehorse_client-0.8.1/README.md` & `littlehorse_client-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/__init__.py` & `littlehorse_client-0.9.0/littlehorse/__init__.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/auth.py` & `littlehorse_client-0.9.0/littlehorse/auth.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/config.py` & `littlehorse_client-0.9.0/littlehorse/config.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/exceptions.py` & `littlehorse_client-0.9.0/littlehorse/exceptions.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/acls_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/acls_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 import littlehorse.model.object_id_pb2 as object__id__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nacls.proto\x12\x0blittlehorse\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0fobject_id.proto\"\xa2\x02\n\tPrincipal\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.littlehorse.PrincipalId\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x0fper_tenant_acls\x18\x03 \x03(\x0b\x32).littlehorse.Principal.PerTenantAclsEntry\x12,\n\x0bglobal_acls\x18\x04 \x01(\x0b\x32\x17.littlehorse.ServerACLs\x1aM\n\x12PerTenantAclsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ServerACLs:\x02\x38\x01\"[\n\x06Tenant\x12!\n\x02id\x18\x01 \x01(\x0b\x32\x15.littlehorse.TenantId\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"2\n\nServerACLs\x12$\n\x04\x61\x63ls\x18\x01 \x03(\x0b\x32\x16.littlehorse.ServerACL\"\x9e\x01\n\tServerACL\x12+\n\tresources\x18\x01 \x03(\x0e\x32\x18.littlehorse.ACLResource\x12/\n\x0f\x61llowed_actions\x18\x02 \x03(\x0e\x32\x16.littlehorse.ACLAction\x12\x0e\n\x04name\x18\x03 \x01(\tH\x00\x12\x10\n\x06prefix\x18\x04 \x01(\tH\x00\x42\x11\n\x0fresource_filter\"\xff\x01\n\x13PutPrincipalRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12L\n\x0fper_tenant_acls\x18\x02 \x03(\x0b\x32\x33.littlehorse.PutPrincipalRequest.PerTenantAclsEntry\x12,\n\x0bglobal_acls\x18\x03 \x01(\x0b\x32\x17.littlehorse.ServerACLs\x12\x11\n\toverwrite\x18\x05 \x01(\x08\x1aM\n\x12PerTenantAclsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ServerACLs:\x02\x38\x01\"$\n\x16\x44\x65letePrincipalRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x1e\n\x10PutTenantRequest\x12\n\n\x02id\x18\x01 \x01(\t*\x92\x01\n\x0b\x41\x43LResource\x12\x10\n\x0c\x41\x43L_WORKFLOW\x10\x00\x12\x0c\n\x08\x41\x43L_TASK\x10\x01\x12\x16\n\x12\x41\x43L_EXTERNAL_EVENT\x10\x02\x12\x11\n\rACL_USER_TASK\x10\x03\x12\x11\n\rACL_PRINCIPAL\x10\x04\x12\x0e\n\nACL_TENANT\x10\x05\x12\x15\n\x11\x41\x43L_ALL_RESOURCES\x10\x06*C\n\tACLAction\x12\x08\n\x04READ\x10\x00\x12\x07\n\x03RUN\x10\x01\x12\x12\n\x0eWRITE_METADATA\x10\x02\x12\x0f\n\x0b\x41LL_ACTIONS\x10\x03\x42G\n\x1fio.littlehorse.sdk.common.protoP\x01Z\x07.;model\xaa\x02\x18LittleHorse.Common.Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nacls.proto\x12\x0blittlehorse\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x0fobject_id.proto\"\xa2\x02\n\tPrincipal\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.littlehorse.PrincipalId\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x42\n\x0fper_tenant_acls\x18\x03 \x03(\x0b\x32).littlehorse.Principal.PerTenantAclsEntry\x12,\n\x0bglobal_acls\x18\x04 \x01(\x0b\x32\x17.littlehorse.ServerACLs\x1aM\n\x12PerTenantAclsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ServerACLs:\x02\x38\x01\"[\n\x06Tenant\x12!\n\x02id\x18\x01 \x01(\x0b\x32\x15.littlehorse.TenantId\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"2\n\nServerACLs\x12$\n\x04\x61\x63ls\x18\x01 \x03(\x0b\x32\x16.littlehorse.ServerACL\"\x9e\x01\n\tServerACL\x12+\n\tresources\x18\x01 \x03(\x0e\x32\x18.littlehorse.ACLResource\x12/\n\x0f\x61llowed_actions\x18\x02 \x03(\x0e\x32\x16.littlehorse.ACLAction\x12\x0e\n\x04name\x18\x03 \x01(\tH\x00\x12\x10\n\x06prefix\x18\x04 \x01(\tH\x00\x42\x11\n\x0fresource_filter\"\xff\x01\n\x13PutPrincipalRequest\x12\n\n\x02id\x18\x01 \x01(\t\x12L\n\x0fper_tenant_acls\x18\x02 \x03(\x0b\x32\x33.littlehorse.PutPrincipalRequest.PerTenantAclsEntry\x12,\n\x0bglobal_acls\x18\x03 \x01(\x0b\x32\x17.littlehorse.ServerACLs\x12\x11\n\toverwrite\x18\x05 \x01(\x08\x1aM\n\x12PerTenantAclsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ServerACLs:\x02\x38\x01\"$\n\x16\x44\x65letePrincipalRequest\x12\n\n\x02id\x18\x01 \x01(\t\"\x1e\n\x10PutTenantRequest\x12\n\n\x02id\x18\x01 \x01(\t*\xad\x01\n\x0b\x41\x43LResource\x12\x10\n\x0c\x41\x43L_WORKFLOW\x10\x00\x12\x0c\n\x08\x41\x43L_TASK\x10\x01\x12\x16\n\x12\x41\x43L_EXTERNAL_EVENT\x10\x02\x12\x11\n\rACL_USER_TASK\x10\x03\x12\x11\n\rACL_PRINCIPAL\x10\x04\x12\x0e\n\nACL_TENANT\x10\x05\x12\x15\n\x11\x41\x43L_ALL_RESOURCES\x10\x06\x12\x19\n\x15\x41\x43L_TASK_WORKER_GROUP\x10\x07*C\n\tACLAction\x12\x08\n\x04READ\x10\x00\x12\x07\n\x03RUN\x10\x01\x12\x12\n\x0eWRITE_METADATA\x10\x02\x12\x0f\n\x0b\x41LL_ACTIONS\x10\x03\x42G\n\x1fio.littlehorse.sdk.common.protoP\x01Z\x07.;model\xaa\x02\x18LittleHorse.Common.Protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'acls_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\037io.littlehorse.sdk.common.protoP\001Z\007.;model\252\002\030LittleHorse.Common.Proto'
   _PRINCIPAL_PERTENANTACLSENTRY._options = None
   _PRINCIPAL_PERTENANTACLSENTRY._serialized_options = b'8\001'
   _PUTPRINCIPALREQUEST_PERTENANTACLSENTRY._options = None
   _PUTPRINCIPALREQUEST_PERTENANTACLSENTRY._serialized_options = b'8\001'
   _globals['_ACLRESOURCE']._serialized_start=1005
-  _globals['_ACLRESOURCE']._serialized_end=1151
-  _globals['_ACLACTION']._serialized_start=1153
-  _globals['_ACLACTION']._serialized_end=1220
+  _globals['_ACLRESOURCE']._serialized_end=1178
+  _globals['_ACLACTION']._serialized_start=1180
+  _globals['_ACLACTION']._serialized_end=1247
   _globals['_PRINCIPAL']._serialized_start=78
   _globals['_PRINCIPAL']._serialized_end=368
   _globals['_PRINCIPAL_PERTENANTACLSENTRY']._serialized_start=291
   _globals['_PRINCIPAL_PERTENANTACLSENTRY']._serialized_end=368
   _globals['_TENANT']._serialized_start=370
   _globals['_TENANT']._serialized_end=461
   _globals['_SERVERACLS']._serialized_start=463
```

### Comparing `littlehorse_client-0.8.1/littlehorse/model/acls_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/acls_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,30 @@
     ACL_WORKFLOW: _ClassVar[ACLResource]
     ACL_TASK: _ClassVar[ACLResource]
     ACL_EXTERNAL_EVENT: _ClassVar[ACLResource]
     ACL_USER_TASK: _ClassVar[ACLResource]
     ACL_PRINCIPAL: _ClassVar[ACLResource]
     ACL_TENANT: _ClassVar[ACLResource]
     ACL_ALL_RESOURCES: _ClassVar[ACLResource]
+    ACL_TASK_WORKER_GROUP: _ClassVar[ACLResource]
 
 class ACLAction(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
     READ: _ClassVar[ACLAction]
     RUN: _ClassVar[ACLAction]
     WRITE_METADATA: _ClassVar[ACLAction]
     ALL_ACTIONS: _ClassVar[ACLAction]
 ACL_WORKFLOW: ACLResource
 ACL_TASK: ACLResource
 ACL_EXTERNAL_EVENT: ACLResource
 ACL_USER_TASK: ACLResource
 ACL_PRINCIPAL: ACLResource
 ACL_TENANT: ACLResource
 ACL_ALL_RESOURCES: ACLResource
+ACL_TASK_WORKER_GROUP: ACLResource
 READ: ACLAction
 RUN: ACLAction
 WRITE_METADATA: ACLAction
 ALL_ACTIONS: ACLAction
 
 class Principal(_message.Message):
     __slots__ = ["id", "created_at", "per_tenant_acls", "global_acls"]
```

### Comparing `littlehorse_client-0.8.1/littlehorse/model/common_enums_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/common_enums_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/common_enums_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/common_enums_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/common_wfspec_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/common_wfspec_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/common_wfspec_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/common_wfspec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/external_event_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/external_event_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/external_event_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/external_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/node_run_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/node_run_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/node_run_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/node_run_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/object_id_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/object_id_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/object_id_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/object_id_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/service_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,29 +24,31 @@
 import littlehorse.model.user_tasks_pb2 as user__tasks__pb2
 import littlehorse.model.wf_spec_pb2 as wf__spec__pb2
 import littlehorse.model.task_def_pb2 as task__def__pb2
 import littlehorse.model.acls_pb2 as acls__pb2
 import littlehorse.model.workflow_event_pb2 as workflow__event__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rservice.proto\x12\x0blittlehorse\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x13\x63ommon_wfspec.proto\x1a\x12\x63ommon_enums.proto\x1a\x0fobject_id.proto\x1a\x0evariable.proto\x1a\x14\x65xternal_event.proto\x1a\x0cwf_run.proto\x1a\x0enode_run.proto\x1a\x0etask_run.proto\x1a\x10user_tasks.proto\x1a\rwf_spec.proto\x1a\x0etask_def.proto\x1a\nacls.proto\x1a\x14workflow_event.proto\"+\n\x1bGetLatestUserTaskDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xd3\x03\n\x10PutWfSpecRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x44\n\x0cthread_specs\x18\x05 \x03(\x0b\x32..littlehorse.PutWfSpecRequest.ThreadSpecsEntry\x12\x1e\n\x16\x65ntrypoint_thread_name\x18\x06 \x01(\t\x12\x43\n\x10retention_policy\x18\x08 \x01(\x0b\x32$.littlehorse.WorkflowRetentionPolicyH\x00\x88\x01\x01\x12\x46\n\x0eparent_wf_spec\x18\t \x01(\x0b\x32).littlehorse.WfSpec.ParentWfSpecReferenceH\x01\x88\x01\x01\x12\x37\n\x0f\x61llowed_updates\x18\n \x01(\x0e\x32\x1e.littlehorse.AllowedUpdateType\x1aK\n\x10ThreadSpecsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ThreadSpec:\x02\x38\x01\x42\x13\n\x11_retention_policyB\x11\n\x0f_parent_wf_specJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05\"O\n\x11PutTaskDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\ninput_vars\x18\x02 \x03(\x0b\x32\x18.littlehorse.VariableDef\"S\n\x1aPutWorkflowEventDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\'\n\x04type\x18\x02 \x01(\x0e\x32\x19.littlehorse.VariableType\"{\n\x15PutUserTaskDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x06\x66ields\x18\x02 \x03(\x0b\x32\x1a.littlehorse.UserTaskField\x12\x18\n\x0b\x64\x65scription\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_description\"o\n\x1aPutExternalEventDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x43\n\x10retention_policy\x18\x02 \x01(\x0b\x32).littlehorse.ExternalEventRetentionPolicy\"\xc3\x02\n\x17PutExternalEventRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12>\n\x15\x65xternal_event_def_id\x18\x02 \x01(\x0b\x32\x1f.littlehorse.ExternalEventDefId\x12\x11\n\x04guid\x18\x03 \x01(\tH\x00\x88\x01\x01\x12+\n\x07\x63ontent\x18\x05 \x01(\x0b\x32\x1a.littlehorse.VariableValue\x12\x1e\n\x11thread_run_number\x18\x06 \x01(\x05H\x01\x88\x01\x01\x12\x1e\n\x11node_run_position\x18\x07 \x01(\x05H\x02\x88\x01\x01\x42\x07\n\x05_guidB\x14\n\x12_thread_run_numberB\x14\n\x12_node_run_positionJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"F\n\x1a\x44\x65leteExternalEventRequest\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.littlehorse.ExternalEventId\"6\n\x12\x44\x65leteWfRunRequest\x12 \n\x02id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\":\n\x14\x44\x65leteTaskDefRequest\x12\"\n\x02id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\"B\n\x18\x44\x65leteUserTaskDefRequest\x12&\n\x02id\x18\x01 \x01(\x0b\x32\x1a.littlehorse.UserTaskDefId\"8\n\x13\x44\x65leteWfSpecRequest\x12!\n\x02id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\"L\n\x1d\x44\x65leteExternalEventDefRequest\x12+\n\x02id\x18\x01 \x01(\x0b\x32\x1f.littlehorse.ExternalEventDefId\"\xe3\x02\n\x0cRunWfRequest\x12\x14\n\x0cwf_spec_name\x18\x01 \x01(\t\x12\x1a\n\rmajor_version\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\x15\n\x08revision\x18\x03 \x01(\x05H\x01\x88\x01\x01\x12;\n\tvariables\x18\x04 \x03(\x0b\x32(.littlehorse.RunWfRequest.VariablesEntry\x12\x0f\n\x02id\x18\x05 \x01(\tH\x02\x88\x01\x01\x12\x33\n\x10parent_wf_run_id\x18\x06 \x01(\x0b\x32\x14.littlehorse.WfRunIdH\x03\x88\x01\x01\x1aL\n\x0eVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.littlehorse.VariableValue:\x02\x38\x01\x42\x10\n\x0e_major_versionB\x0b\n\t_revisionB\x05\n\x03_idB\x13\n\x11_parent_wf_run_id\"L\n\rVariableMatch\x12\x10\n\x08var_name\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.littlehorse.VariableValue\"\xbd\x01\n\x19\x41waitWorkflowEventRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x36\n\revent_def_ids\x18\x02 \x03(\x0b\x32\x1f.littlehorse.WorkflowEventDefId\x12?\n\x19workflow_events_to_ignore\x18\x03 \x03(\x0b\x32\x1c.littlehorse.WorkflowEventId\"\xdf\x03\n\x12SearchWfRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x14\n\x0cwf_spec_name\x18\x03 \x01(\t\x12\"\n\x15wf_spec_major_version\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x1d\n\x10wf_spec_revision\x18\x05 \x01(\x05H\x03\x88\x01\x01\x12*\n\x06status\x18\x06 \x01(\x0e\x32\x15.littlehorse.LHStatusH\x04\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x05\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x34\n\x10variable_filters\x18\t \x03(\x0b\x32\x1a.littlehorse.VariableMatchB\x0b\n\t_bookmarkB\x08\n\x06_limitB\x18\n\x16_wf_spec_major_versionB\x13\n\x11_wf_spec_revisionB\t\n\x07_statusB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"X\n\x0bWfRunIdList\x12%\n\x07results\x18\x01 \x03(\x0b\x32\x14.littlehorse.WfRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xbc\x02\n\x14SearchTaskRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x15\n\rtask_def_name\x18\x03 \x01(\t\x12,\n\x06status\x18\x04 \x01(\x0e\x32\x17.littlehorse.TaskStatusH\x02\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x04\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_statusB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"\\\n\rTaskRunIdList\x12\'\n\x07results\x18\x01 \x03(\x0b\x32\x16.littlehorse.TaskRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xf1\x03\n\x14SearchNodeRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x02\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12=\n\tnode_type\x18\x05 \x01(\x0e\x32*.littlehorse.SearchNodeRunRequest.NodeType\x12%\n\x06status\x18\x06 \x01(\x0e\x32\x15.littlehorse.LHStatus\"\x9c\x01\n\x08NodeType\x12\x08\n\x04TASK\x10\x00\x12\x12\n\x0e\x45XTERNAL_EVENT\x10\x01\x12\x0e\n\nENTRYPOINT\x10\x02\x12\x08\n\x04\x45XIT\x10\x03\x12\x10\n\x0cSTART_THREAD\x10\x04\x12\x10\n\x0cWAIT_THREADS\x10\x05\x12\t\n\x05SLEEP\x10\x06\x12\r\n\tUSER_TASK\x10\x07\x12\x1a\n\x16START_MULTIPLE_THREADS\x10\x08\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"\\\n\rNodeRunIdList\x12\'\n\x07results\x18\x01 \x03(\x0b\x32\x16.littlehorse.NodeRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xb2\x03\n\x18SearchUserTaskRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x33\n\x06status\x18\x03 \x01(\x0e\x32\x1e.littlehorse.UserTaskRunStatusH\x02\x88\x01\x01\x12\x1f\n\x12user_task_def_name\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x14\n\x07user_id\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x17\n\nuser_group\x18\x06 \x01(\tH\x05\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x07\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_statusB\x15\n\x13_user_task_def_nameB\n\n\x08_user_idB\r\n\x0b_user_groupB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"d\n\x11UserTaskRunIdList\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.UserTaskRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x9e\x02\n\x15SearchVariableRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12)\n\x05value\x18\x03 \x01(\x0b\x32\x1a.littlehorse.VariableValue\x12\"\n\x15wf_spec_major_version\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x1d\n\x10wf_spec_revision\x18\x05 \x01(\x05H\x03\x88\x01\x01\x12\x10\n\x08var_name\x18\x06 \x01(\t\x12\x14\n\x0cwf_spec_name\x18\x07 \x01(\tB\x0b\n\t_bookmarkB\x08\n\x06_limitB\x18\n\x16_wf_spec_major_versionB\x13\n\x11_wf_spec_revision\"^\n\x0eVariableIdList\x12(\n\x07results\x18\x01 \x03(\x0b\x32\x17.littlehorse.VariableId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"x\n\x14SearchTaskDefRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x13\n\x06prefix\x18\x03 \x01(\tH\x02\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_prefix\"\\\n\rTaskDefIdList\x12\'\n\x07results\x18\x01 \x03(\x0b\x32\x16.littlehorse.TaskDefId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x98\x01\n\x18SearchUserTaskDefRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x02\x88\x01\x01\x12\x10\n\x06prefix\x18\x03 \x01(\tH\x00\x12\x0e\n\x04name\x18\x04 \x01(\tH\x00\x42\x18\n\x16user_task_def_criteriaB\x0b\n\t_bookmarkB\x08\n\x06_limit\"d\n\x11UserTaskDefIdList\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.UserTaskDefId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xa6\x01\n\x13SearchWfSpecRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x02\x88\x01\x01\x12\x0e\n\x04name\x18\x03 \x01(\tH\x00\x12\x10\n\x06prefix\x18\x04 \x01(\tH\x00\x12\x17\n\rtask_def_name\x18\x05 \x01(\tH\x00\x42\x12\n\x10wf_spec_criteriaB\x0b\n\t_bookmarkB\x08\n\x06_limit\"Z\n\x0cWfSpecIdList\x12&\n\x07results\x18\x01 \x03(\x0b\x32\x15.littlehorse.WfSpecId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x81\x01\n\x1dSearchExternalEventDefRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x13\n\x06prefix\x18\x03 \x01(\tH\x02\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_prefix\"n\n\x16\x45xternalEventDefIdList\x12\x30\n\x07results\x18\x01 \x03(\x0b\x32\x1f.littlehorse.ExternalEventDefId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x80\x03\n\x1aSearchExternalEventRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x02\x88\x01\x01\x12)\n\twf_run_id\x18\x03 \x01(\x0b\x32\x14.littlehorse.WfRunIdH\x00\x12u\n\"external_event_def_name_and_status\x18\x04 \x01(\x0b\x32G.littlehorse.SearchExternalEventRequest.ByExtEvtDefNameAndStatusRequestH\x00\x1aj\n\x1f\x42yExtEvtDefNameAndStatusRequest\x12\x1f\n\x17\x65xternal_event_def_name\x18\x01 \x01(\t\x12\x17\n\nis_claimed\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\r\n\x0b_is_claimedB\x12\n\x10\x65xt_evt_criteriaB\x0b\n\t_bookmarkB\x08\n\x06_limit\"h\n\x13\x45xternalEventIdList\x12-\n\x07results\x18\x01 \x03(\x0b\x32\x1c.littlehorse.ExternalEventId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\">\n\x13ListNodeRunsRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"4\n\x0bNodeRunList\x12%\n\x07results\x18\x01 \x03(\x0b\x32\x14.littlehorse.NodeRun\"?\n\x14ListVariablesRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"6\n\x0cVariableList\x12&\n\x07results\x18\x01 \x03(\x0b\x32\x15.littlehorse.Variable\"D\n\x19ListExternalEventsRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"@\n\x11\x45xternalEventList\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.ExternalEvent\"w\n\x19RegisterTaskWorkerRequest\x12\x16\n\x0etask_worker_id\x18\x01 \x01(\t\x12+\n\x0btask_def_id\x18\x02 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x15\n\rlistener_name\x18\x03 \x01(\t\"s\n\x1aTaskWorkerHeartBeatRequest\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12+\n\x0btask_def_id\x18\x02 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x15\n\rlistener_name\x18\x03 \x01(\t\"\x81\x01\n\x1aRegisterTaskWorkerResponse\x12+\n\nyour_hosts\x18\x01 \x03(\x0b\x32\x17.littlehorse.LHHostInfo\x12\x1f\n\x12is_cluster_healthy\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\x15\n\x13_is_cluster_healthy\"(\n\nLHHostInfo\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x8b\x01\n\x0fPollTaskRequest\x12+\n\x0btask_def_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x11\n\tclient_id\x18\x02 \x01(\t\x12 \n\x13task_worker_version\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x16\n\x14_task_worker_version\"\x8c\x02\n\rScheduledTask\x12+\n\x0btask_run_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskRunId\x12+\n\x0btask_def_id\x18\x02 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x16\n\x0e\x61ttempt_number\x18\x03 \x01(\x05\x12-\n\tvariables\x18\x04 \x03(\x0b\x32\x1a.littlehorse.VarNameAndVal\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06source\x18\x06 \x01(\x0b\x32\x1a.littlehorse.TaskRunSource\"N\n\x10PollTaskResponse\x12/\n\x06result\x18\x01 \x01(\x0b\x32\x1a.littlehorse.ScheduledTaskH\x00\x88\x01\x01\x42\t\n\x07_result\"\x81\x03\n\rReportTaskRun\x12+\n\x0btask_run_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskRunId\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x06status\x18\x03 \x01(\x0e\x32\x17.littlehorse.TaskStatus\x12\x33\n\nlog_output\x18\x05 \x01(\x0b\x32\x1a.littlehorse.VariableValueH\x01\x88\x01\x01\x12\x16\n\x0e\x61ttempt_number\x18\x06 \x01(\x05\x12,\n\x06output\x18\x04 \x01(\x0b\x32\x1a.littlehorse.VariableValueH\x00\x12)\n\x05\x65rror\x18\x07 \x01(\x0b\x32\x18.littlehorse.LHTaskErrorH\x00\x12\x31\n\texception\x18\x08 \x01(\x0b\x32\x1c.littlehorse.LHTaskExceptionH\x00\x42\x08\n\x06resultB\r\n\x0b_log_output\"V\n\x10StopWfRunRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x19\n\x11thread_run_number\x18\x02 \x01(\x05\"X\n\x12ResumeWfRunRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x19\n\x11thread_run_number\x18\x02 \x01(\x05\"\xb3\x01\n\x1aTaskDefMetricsQueryRequest\x12\x30\n\x0cwindow_start\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x0bwindow_type\x18\x02 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x1a\n\rtask_def_name\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x10\n\x0e_task_def_name\"\xca\x01\n\x16ListTaskMetricsRequest\x12+\n\x0btask_def_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x35\n\x11last_window_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\rwindow_length\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x13\n\x0bnum_windows\x18\x04 \x01(\x05\"G\n\x17ListTaskMetricsResponse\x12,\n\x07results\x18\x01 \x03(\x0b\x32\x1b.littlehorse.TaskDefMetrics\"\xb1\x01\n\x19WfSpecMetricsQueryRequest\x12)\n\nwf_spec_id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x30\n\x0cwindow_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\rwindow_length\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\"\xc6\x01\n\x14ListWfMetricsRequest\x12)\n\nwf_spec_id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x35\n\x11last_window_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\rwindow_length\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x13\n\x0bnum_windows\x18\x04 \x01(\x05\"D\n\x15ListWfMetricsResponse\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.WfSpecMetrics\"\xfb\x02\n\x0eTaskDefMetrics\x12+\n\x0btask_def_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x30\n\x0cwindow_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x04type\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x1d\n\x15schedule_to_start_max\x18\x04 \x01(\x03\x12\x1d\n\x15schedule_to_start_avg\x18\x05 \x01(\x03\x12\x1d\n\x15start_to_complete_max\x18\x06 \x01(\x03\x12\x1d\n\x15start_to_complete_avg\x18\x07 \x01(\x03\x12\x17\n\x0ftotal_completed\x18\x08 \x01(\x03\x12\x15\n\rtotal_errored\x18\t \x01(\x03\x12\x15\n\rtotal_started\x18\n \x01(\x03\x12\x17\n\x0ftotal_scheduled\x18\x0b \x01(\x03\"\xa1\x02\n\rWfSpecMetrics\x12)\n\nwf_spec_id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x30\n\x0cwindow_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x04type\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x15\n\rtotal_started\x18\x04 \x01(\x03\x12\x17\n\x0ftotal_completed\x18\x05 \x01(\x03\x12\x15\n\rtotal_errored\x18\x06 \x01(\x03\x12\x1d\n\x15start_to_complete_max\x18\x07 \x01(\x03\x12\x1d\n\x15start_to_complete_avg\x18\x08 \x01(\x03\"A\n\x16ListUserTaskRunRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"<\n\x0fUserTaskRunList\x12)\n\x07results\x18\x01 \x03(\x0b\x32\x18.littlehorse.UserTaskRun\">\n\x13ListTaskRunsRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"4\n\x0bTaskRunList\x12%\n\x07results\x18\x01 \x03(\x0b\x32\x14.littlehorse.TaskRun\"z\n\x14MigrateWfSpecRequest\x12*\n\x0bold_wf_spec\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x36\n\tmigration\x18\x02 \x01(\x0b\x32#.littlehorse.WfSpecVersionMigration\"T\n\x16GetLatestWfSpecRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1a\n\rmajor_version\x18\x02 \x01(\x05H\x00\x88\x01\x01\x42\x10\n\x0e_major_version\"\x9c\x01\n\x15ServerVersionResponse\x12\x15\n\rmajor_version\x18\x01 \x01(\x05\x12\x15\n\rminor_version\x18\x02 \x01(\x05\x12\x15\n\rpatch_version\x18\x03 \x01(\x05\x12#\n\x16pre_release_identifier\x18\x04 \x01(\tH\x00\x88\x01\x01\x42\x19\n\x17_pre_release_identifier*P\n\x11\x41llowedUpdateType\x12\x0f\n\x0b\x41LL_UPDATES\x10\x00\x12\x1a\n\x16MINOR_REVISION_UPDATES\x10\x01\x12\x0e\n\nNO_UPDATES\x10\x02\x32\xa1$\n\x0bLittleHorse\x12\x44\n\nPutTaskDef\x12\x1e.littlehorse.PutTaskDefRequest\x1a\x14.littlehorse.TaskDef\"\x00\x12<\n\nGetTaskDef\x12\x16.littlehorse.TaskDefId\x1a\x14.littlehorse.TaskDef\"\x00\x12_\n\x13PutExternalEventDef\x12\'.littlehorse.PutExternalEventDefRequest\x1a\x1d.littlehorse.ExternalEventDef\"\x00\x12W\n\x13GetExternalEventDef\x12\x1f.littlehorse.ExternalEventDefId\x1a\x1d.littlehorse.ExternalEventDef\"\x00\x12_\n\x13PutWorkflowEventDef\x12\'.littlehorse.PutWorkflowEventDefRequest\x1a\x1d.littlehorse.WorkflowEventDef\"\x00\x12\x41\n\tPutWfSpec\x12\x1d.littlehorse.PutWfSpecRequest\x1a\x13.littlehorse.WfSpec\"\x00\x12\x39\n\tGetWfSpec\x12\x15.littlehorse.WfSpecId\x1a\x13.littlehorse.WfSpec\"\x00\x12M\n\x0fGetLatestWfSpec\x12#.littlehorse.GetLatestWfSpecRequest\x1a\x13.littlehorse.WfSpec\"\x00\x12I\n\rMigrateWfSpec\x12!.littlehorse.MigrateWfSpecRequest\x1a\x13.littlehorse.WfSpec\"\x00\x12P\n\x0ePutUserTaskDef\x12\".littlehorse.PutUserTaskDefRequest\x1a\x18.littlehorse.UserTaskDef\"\x00\x12H\n\x0eGetUserTaskDef\x12\x1a.littlehorse.UserTaskDefId\x1a\x18.littlehorse.UserTaskDef\"\x00\x12\\\n\x14GetLatestUserTaskDef\x12(.littlehorse.GetLatestUserTaskDefRequest\x1a\x18.littlehorse.UserTaskDef\"\x00\x12\x38\n\x05RunWf\x12\x19.littlehorse.RunWfRequest\x1a\x12.littlehorse.WfRun\"\x00\x12\x36\n\x08GetWfRun\x12\x14.littlehorse.WfRunId\x1a\x12.littlehorse.WfRun\"\x00\x12H\n\x0eGetUserTaskRun\x12\x1a.littlehorse.UserTaskRunId\x1a\x18.littlehorse.UserTaskRun\"\x00\x12T\n\x11\x41ssignUserTaskRun\x12%.littlehorse.AssignUserTaskRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x13\x43ompleteUserTaskRun\x12\'.littlehorse.CompleteUserTaskRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x11\x43\x61ncelUserTaskRun\x12%.littlehorse.CancelUserTaskRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12W\n\x10ListUserTaskRuns\x12#.littlehorse.ListUserTaskRunRequest\x1a\x1c.littlehorse.UserTaskRunList\"\x00\x12<\n\nGetNodeRun\x12\x16.littlehorse.NodeRunId\x1a\x14.littlehorse.NodeRun\"\x00\x12L\n\x0cListNodeRuns\x12 .littlehorse.ListNodeRunsRequest\x1a\x18.littlehorse.NodeRunList\"\x00\x12<\n\nGetTaskRun\x12\x16.littlehorse.TaskRunId\x1a\x14.littlehorse.TaskRun\"\x00\x12L\n\x0cListTaskRuns\x12 .littlehorse.ListTaskRunsRequest\x1a\x18.littlehorse.TaskRunList\"\x00\x12?\n\x0bGetVariable\x12\x17.littlehorse.VariableId\x1a\x15.littlehorse.Variable\"\x00\x12O\n\rListVariables\x12!.littlehorse.ListVariablesRequest\x1a\x19.littlehorse.VariableList\"\x00\x12V\n\x10PutExternalEvent\x12$.littlehorse.PutExternalEventRequest\x1a\x1a.littlehorse.ExternalEvent\"\x00\x12N\n\x10GetExternalEvent\x12\x1c.littlehorse.ExternalEventId\x1a\x1a.littlehorse.ExternalEvent\"\x00\x12Z\n\x12\x41waitWorkflowEvent\x12&.littlehorse.AwaitWorkflowEventRequest\x1a\x1a.littlehorse.WorkflowEvent\"\x00\x12^\n\x12ListExternalEvents\x12&.littlehorse.ListExternalEventsRequest\x1a\x1e.littlehorse.ExternalEventList\"\x00\x12J\n\x0bSearchWfRun\x12\x1f.littlehorse.SearchWfRunRequest\x1a\x18.littlehorse.WfRunIdList\"\x00\x12P\n\rSearchNodeRun\x12!.littlehorse.SearchNodeRunRequest\x1a\x1a.littlehorse.NodeRunIdList\"\x00\x12P\n\rSearchTaskRun\x12!.littlehorse.SearchTaskRunRequest\x1a\x1a.littlehorse.TaskRunIdList\"\x00\x12\\\n\x11SearchUserTaskRun\x12%.littlehorse.SearchUserTaskRunRequest\x1a\x1e.littlehorse.UserTaskRunIdList\"\x00\x12S\n\x0eSearchVariable\x12\".littlehorse.SearchVariableRequest\x1a\x1b.littlehorse.VariableIdList\"\x00\x12\x62\n\x13SearchExternalEvent\x12\'.littlehorse.SearchExternalEventRequest\x1a .littlehorse.ExternalEventIdList\"\x00\x12P\n\rSearchTaskDef\x12!.littlehorse.SearchTaskDefRequest\x1a\x1a.littlehorse.TaskDefIdList\"\x00\x12\\\n\x11SearchUserTaskDef\x12%.littlehorse.SearchUserTaskDefRequest\x1a\x1e.littlehorse.UserTaskDefIdList\"\x00\x12M\n\x0cSearchWfSpec\x12 .littlehorse.SearchWfSpecRequest\x1a\x19.littlehorse.WfSpecIdList\"\x00\x12k\n\x16SearchExternalEventDef\x12*.littlehorse.SearchExternalEventDefRequest\x1a#.littlehorse.ExternalEventDefIdList\"\x00\x12g\n\x12RegisterTaskWorker\x12&.littlehorse.RegisterTaskWorkerRequest\x1a\'.littlehorse.RegisterTaskWorkerResponse\"\x00\x12M\n\x08PollTask\x12\x1c.littlehorse.PollTaskRequest\x1a\x1d.littlehorse.PollTaskResponse\"\x00(\x01\x30\x01\x12\x42\n\nReportTask\x12\x1a.littlehorse.ReportTaskRun\x1a\x16.google.protobuf.Empty\"\x00\x12\x44\n\tStopWfRun\x12\x1d.littlehorse.StopWfRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0bResumeWfRun\x12\x1f.littlehorse.ResumeWfRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0b\x44\x65leteWfRun\x12\x1f.littlehorse.DeleteWfRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\rDeleteTaskDef\x12!.littlehorse.DeleteTaskDefRequest\x1a\x16.google.protobuf.Empty\"\x00\x12J\n\x0c\x44\x65leteWfSpec\x12 .littlehorse.DeleteWfSpecRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x11\x44\x65leteUserTaskDef\x12%.littlehorse.DeleteUserTaskDefRequest\x1a\x16.google.protobuf.Empty\"\x00\x12^\n\x16\x44\x65leteExternalEventDef\x12*.littlehorse.DeleteExternalEventDefRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x61\n\x17GetTaskDefMetricsWindow\x12\'.littlehorse.TaskDefMetricsQueryRequest\x1a\x1b.littlehorse.TaskDefMetrics\"\x00\x12^\n\x16GetWfSpecMetricsWindow\x12&.littlehorse.WfSpecMetricsQueryRequest\x1a\x1a.littlehorse.WfSpecMetrics\"\x00\x12\x61\n\x12ListTaskDefMetrics\x12#.littlehorse.ListTaskMetricsRequest\x1a$.littlehorse.ListTaskMetricsResponse\"\x00\x12\\\n\x11ListWfSpecMetrics\x12!.littlehorse.ListWfMetricsRequest\x1a\".littlehorse.ListWfMetricsResponse\"\x00\x12\x41\n\tPutTenant\x12\x1d.littlehorse.PutTenantRequest\x1a\x13.littlehorse.Tenant\"\x00\x12J\n\x0cPutPrincipal\x12 .littlehorse.PutPrincipalRequest\x1a\x16.littlehorse.Principal\"\x00\x12:\n\x06Whoami\x12\x16.google.protobuf.Empty\x1a\x16.littlehorse.Principal\"\x00\x12P\n\x10GetServerVersion\x12\x16.google.protobuf.Empty\x1a\".littlehorse.ServerVersionResponse\"\x00\x42G\n\x1fio.littlehorse.sdk.common.protoP\x01Z\x07.;model\xaa\x02\x18LittleHorse.Common.Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rservice.proto\x12\x0blittlehorse\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x13\x63ommon_wfspec.proto\x1a\x12\x63ommon_enums.proto\x1a\x0fobject_id.proto\x1a\x0evariable.proto\x1a\x14\x65xternal_event.proto\x1a\x0cwf_run.proto\x1a\x0enode_run.proto\x1a\x0etask_run.proto\x1a\x10user_tasks.proto\x1a\rwf_spec.proto\x1a\x0etask_def.proto\x1a\nacls.proto\x1a\x14workflow_event.proto\"+\n\x1bGetLatestUserTaskDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xd3\x03\n\x10PutWfSpecRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x44\n\x0cthread_specs\x18\x05 \x03(\x0b\x32..littlehorse.PutWfSpecRequest.ThreadSpecsEntry\x12\x1e\n\x16\x65ntrypoint_thread_name\x18\x06 \x01(\t\x12\x43\n\x10retention_policy\x18\x08 \x01(\x0b\x32$.littlehorse.WorkflowRetentionPolicyH\x00\x88\x01\x01\x12\x46\n\x0eparent_wf_spec\x18\t \x01(\x0b\x32).littlehorse.WfSpec.ParentWfSpecReferenceH\x01\x88\x01\x01\x12\x37\n\x0f\x61llowed_updates\x18\n \x01(\x0e\x32\x1e.littlehorse.AllowedUpdateType\x1aK\n\x10ThreadSpecsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ThreadSpec:\x02\x38\x01\x42\x13\n\x11_retention_policyB\x11\n\x0f_parent_wf_specJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05\"O\n\x11PutTaskDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\ninput_vars\x18\x02 \x03(\x0b\x32\x18.littlehorse.VariableDef\"S\n\x1aPutWorkflowEventDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\'\n\x04type\x18\x02 \x01(\x0e\x32\x19.littlehorse.VariableType\"{\n\x15PutUserTaskDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12*\n\x06\x66ields\x18\x02 \x03(\x0b\x32\x1a.littlehorse.UserTaskField\x12\x18\n\x0b\x64\x65scription\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_description\"o\n\x1aPutExternalEventDefRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x43\n\x10retention_policy\x18\x02 \x01(\x0b\x32).littlehorse.ExternalEventRetentionPolicy\"\xc3\x02\n\x17PutExternalEventRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12>\n\x15\x65xternal_event_def_id\x18\x02 \x01(\x0b\x32\x1f.littlehorse.ExternalEventDefId\x12\x11\n\x04guid\x18\x03 \x01(\tH\x00\x88\x01\x01\x12+\n\x07\x63ontent\x18\x05 \x01(\x0b\x32\x1a.littlehorse.VariableValue\x12\x1e\n\x11thread_run_number\x18\x06 \x01(\x05H\x01\x88\x01\x01\x12\x1e\n\x11node_run_position\x18\x07 \x01(\x05H\x02\x88\x01\x01\x42\x07\n\x05_guidB\x14\n\x12_thread_run_numberB\x14\n\x12_node_run_positionJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"F\n\x1a\x44\x65leteExternalEventRequest\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.littlehorse.ExternalEventId\"6\n\x12\x44\x65leteWfRunRequest\x12 \n\x02id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\":\n\x14\x44\x65leteTaskDefRequest\x12\"\n\x02id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\"B\n\x18\x44\x65leteUserTaskDefRequest\x12&\n\x02id\x18\x01 \x01(\x0b\x32\x1a.littlehorse.UserTaskDefId\"8\n\x13\x44\x65leteWfSpecRequest\x12!\n\x02id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\"L\n\x1d\x44\x65leteExternalEventDefRequest\x12+\n\x02id\x18\x01 \x01(\x0b\x32\x1f.littlehorse.ExternalEventDefId\"\xe3\x02\n\x0cRunWfRequest\x12\x14\n\x0cwf_spec_name\x18\x01 \x01(\t\x12\x1a\n\rmajor_version\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\x15\n\x08revision\x18\x03 \x01(\x05H\x01\x88\x01\x01\x12;\n\tvariables\x18\x04 \x03(\x0b\x32(.littlehorse.RunWfRequest.VariablesEntry\x12\x0f\n\x02id\x18\x05 \x01(\tH\x02\x88\x01\x01\x12\x33\n\x10parent_wf_run_id\x18\x06 \x01(\x0b\x32\x14.littlehorse.WfRunIdH\x03\x88\x01\x01\x1aL\n\x0eVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.littlehorse.VariableValue:\x02\x38\x01\x42\x10\n\x0e_major_versionB\x0b\n\t_revisionB\x05\n\x03_idB\x13\n\x11_parent_wf_run_id\"L\n\rVariableMatch\x12\x10\n\x08var_name\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.littlehorse.VariableValue\"\xbd\x01\n\x19\x41waitWorkflowEventRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x36\n\revent_def_ids\x18\x02 \x03(\x0b\x32\x1f.littlehorse.WorkflowEventDefId\x12?\n\x19workflow_events_to_ignore\x18\x03 \x03(\x0b\x32\x1c.littlehorse.WorkflowEventId\"\xdf\x03\n\x12SearchWfRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x14\n\x0cwf_spec_name\x18\x03 \x01(\t\x12\"\n\x15wf_spec_major_version\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x1d\n\x10wf_spec_revision\x18\x05 \x01(\x05H\x03\x88\x01\x01\x12*\n\x06status\x18\x06 \x01(\x0e\x32\x15.littlehorse.LHStatusH\x04\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x05\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x34\n\x10variable_filters\x18\t \x03(\x0b\x32\x1a.littlehorse.VariableMatchB\x0b\n\t_bookmarkB\x08\n\x06_limitB\x18\n\x16_wf_spec_major_versionB\x13\n\x11_wf_spec_revisionB\t\n\x07_statusB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"X\n\x0bWfRunIdList\x12%\n\x07results\x18\x01 \x03(\x0b\x32\x14.littlehorse.WfRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xbc\x02\n\x14SearchTaskRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x15\n\rtask_def_name\x18\x03 \x01(\t\x12,\n\x06status\x18\x04 \x01(\x0e\x32\x17.littlehorse.TaskStatusH\x02\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x04\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_statusB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"\\\n\rTaskRunIdList\x12\'\n\x07results\x18\x01 \x03(\x0b\x32\x16.littlehorse.TaskRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xf1\x03\n\x14SearchNodeRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x02\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x03\x88\x01\x01\x12=\n\tnode_type\x18\x05 \x01(\x0e\x32*.littlehorse.SearchNodeRunRequest.NodeType\x12%\n\x06status\x18\x06 \x01(\x0e\x32\x15.littlehorse.LHStatus\"\x9c\x01\n\x08NodeType\x12\x08\n\x04TASK\x10\x00\x12\x12\n\x0e\x45XTERNAL_EVENT\x10\x01\x12\x0e\n\nENTRYPOINT\x10\x02\x12\x08\n\x04\x45XIT\x10\x03\x12\x10\n\x0cSTART_THREAD\x10\x04\x12\x10\n\x0cWAIT_THREADS\x10\x05\x12\t\n\x05SLEEP\x10\x06\x12\r\n\tUSER_TASK\x10\x07\x12\x1a\n\x16START_MULTIPLE_THREADS\x10\x08\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"\\\n\rNodeRunIdList\x12\'\n\x07results\x18\x01 \x03(\x0b\x32\x16.littlehorse.NodeRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xb2\x03\n\x18SearchUserTaskRunRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x33\n\x06status\x18\x03 \x01(\x0e\x32\x1e.littlehorse.UserTaskRunStatusH\x02\x88\x01\x01\x12\x1f\n\x12user_task_def_name\x18\x04 \x01(\tH\x03\x88\x01\x01\x12\x14\n\x07user_id\x18\x05 \x01(\tH\x04\x88\x01\x01\x12\x17\n\nuser_group\x18\x06 \x01(\tH\x05\x88\x01\x01\x12\x37\n\x0e\x65\x61rliest_start\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x06\x88\x01\x01\x12\x35\n\x0clatest_start\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x07\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_statusB\x15\n\x13_user_task_def_nameB\n\n\x08_user_idB\r\n\x0b_user_groupB\x11\n\x0f_earliest_startB\x0f\n\r_latest_start\"d\n\x11UserTaskRunIdList\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.UserTaskRunId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x9e\x02\n\x15SearchVariableRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12)\n\x05value\x18\x03 \x01(\x0b\x32\x1a.littlehorse.VariableValue\x12\"\n\x15wf_spec_major_version\x18\x04 \x01(\x05H\x02\x88\x01\x01\x12\x1d\n\x10wf_spec_revision\x18\x05 \x01(\x05H\x03\x88\x01\x01\x12\x10\n\x08var_name\x18\x06 \x01(\t\x12\x14\n\x0cwf_spec_name\x18\x07 \x01(\tB\x0b\n\t_bookmarkB\x08\n\x06_limitB\x18\n\x16_wf_spec_major_versionB\x13\n\x11_wf_spec_revision\"^\n\x0eVariableIdList\x12(\n\x07results\x18\x01 \x03(\x0b\x32\x17.littlehorse.VariableId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"x\n\x14SearchTaskDefRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x13\n\x06prefix\x18\x03 \x01(\tH\x02\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_prefix\"\\\n\rTaskDefIdList\x12\'\n\x07results\x18\x01 \x03(\x0b\x32\x16.littlehorse.TaskDefId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x98\x01\n\x18SearchUserTaskDefRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x02\x88\x01\x01\x12\x10\n\x06prefix\x18\x03 \x01(\tH\x00\x12\x0e\n\x04name\x18\x04 \x01(\tH\x00\x42\x18\n\x16user_task_def_criteriaB\x0b\n\t_bookmarkB\x08\n\x06_limit\"d\n\x11UserTaskDefIdList\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.UserTaskDefId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xa6\x01\n\x13SearchWfSpecRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x02\x88\x01\x01\x12\x0e\n\x04name\x18\x03 \x01(\tH\x00\x12\x10\n\x06prefix\x18\x04 \x01(\tH\x00\x12\x17\n\rtask_def_name\x18\x05 \x01(\tH\x00\x42\x12\n\x10wf_spec_criteriaB\x0b\n\t_bookmarkB\x08\n\x06_limit\"Z\n\x0cWfSpecIdList\x12&\n\x07results\x18\x01 \x03(\x0b\x32\x15.littlehorse.WfSpecId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x81\x01\n\x1dSearchExternalEventDefRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x01\x88\x01\x01\x12\x13\n\x06prefix\x18\x03 \x01(\tH\x02\x88\x01\x01\x42\x0b\n\t_bookmarkB\x08\n\x06_limitB\t\n\x07_prefix\"n\n\x16\x45xternalEventDefIdList\x12\x30\n\x07results\x18\x01 \x03(\x0b\x32\x1f.littlehorse.ExternalEventDefId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"W\n\x13SearchTenantRequest\x12\x12\n\x05limit\x18\x01 \x01(\x05H\x00\x88\x01\x01\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x01\x88\x01\x01\x42\x08\n\x06_limitB\x0b\n\t_bookmark\"Z\n\x0cTenantIdList\x12&\n\x07results\x18\x01 \x03(\x0b\x32\x15.littlehorse.TenantId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\x80\x03\n\x1aSearchExternalEventRequest\x12\x15\n\x08\x62ookmark\x18\x01 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x02 \x01(\x05H\x02\x88\x01\x01\x12)\n\twf_run_id\x18\x03 \x01(\x0b\x32\x14.littlehorse.WfRunIdH\x00\x12u\n\"external_event_def_name_and_status\x18\x04 \x01(\x0b\x32G.littlehorse.SearchExternalEventRequest.ByExtEvtDefNameAndStatusRequestH\x00\x1aj\n\x1f\x42yExtEvtDefNameAndStatusRequest\x12\x1f\n\x17\x65xternal_event_def_name\x18\x01 \x01(\t\x12\x17\n\nis_claimed\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\r\n\x0b_is_claimedB\x12\n\x10\x65xt_evt_criteriaB\x0b\n\t_bookmarkB\x08\n\x06_limit\"h\n\x13\x45xternalEventIdList\x12-\n\x07results\x18\x01 \x03(\x0b\x32\x1c.littlehorse.ExternalEventId\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"\xb6\x01\n\x13ListNodeRunsRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x1e\n\x11thread_run_number\x18\x02 \x01(\x05H\x00\x88\x01\x01\x12\x15\n\x08\x62ookmark\x18\x03 \x01(\x0cH\x01\x88\x01\x01\x12\x12\n\x05limit\x18\x04 \x01(\x05H\x02\x88\x01\x01\x42\x14\n\x12_thread_run_numberB\x0b\n\t_bookmarkB\x08\n\x06_limit\"X\n\x0bNodeRunList\x12%\n\x07results\x18\x01 \x03(\x0b\x32\x14.littlehorse.NodeRun\x12\x15\n\x08\x62ookmark\x18\x02 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_bookmark\"?\n\x14ListVariablesRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"6\n\x0cVariableList\x12&\n\x07results\x18\x01 \x03(\x0b\x32\x15.littlehorse.Variable\"D\n\x19ListExternalEventsRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"@\n\x11\x45xternalEventList\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.ExternalEvent\"w\n\x19RegisterTaskWorkerRequest\x12\x16\n\x0etask_worker_id\x18\x01 \x01(\t\x12+\n\x0btask_def_id\x18\x02 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x15\n\rlistener_name\x18\x03 \x01(\t\"s\n\x1aTaskWorkerHeartBeatRequest\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12+\n\x0btask_def_id\x18\x02 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x15\n\rlistener_name\x18\x03 \x01(\t\"\x81\x01\n\x1aRegisterTaskWorkerResponse\x12+\n\nyour_hosts\x18\x01 \x03(\x0b\x32\x17.littlehorse.LHHostInfo\x12\x1f\n\x12is_cluster_healthy\x18\x02 \x01(\x08H\x00\x88\x01\x01\x42\x15\n\x13_is_cluster_healthy\"(\n\nLHHostInfo\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x8b\x01\n\x0fPollTaskRequest\x12+\n\x0btask_def_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x11\n\tclient_id\x18\x02 \x01(\t\x12 \n\x13task_worker_version\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x16\n\x14_task_worker_version\"\x8c\x02\n\rScheduledTask\x12+\n\x0btask_run_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskRunId\x12+\n\x0btask_def_id\x18\x02 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x16\n\x0e\x61ttempt_number\x18\x03 \x01(\x05\x12-\n\tvariables\x18\x04 \x03(\x0b\x32\x1a.littlehorse.VarNameAndVal\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06source\x18\x06 \x01(\x0b\x32\x1a.littlehorse.TaskRunSource\"N\n\x10PollTaskResponse\x12/\n\x06result\x18\x01 \x01(\x0b\x32\x1a.littlehorse.ScheduledTaskH\x00\x88\x01\x01\x42\t\n\x07_result\"\x81\x03\n\rReportTaskRun\x12+\n\x0btask_run_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskRunId\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x06status\x18\x03 \x01(\x0e\x32\x17.littlehorse.TaskStatus\x12\x33\n\nlog_output\x18\x05 \x01(\x0b\x32\x1a.littlehorse.VariableValueH\x01\x88\x01\x01\x12\x16\n\x0e\x61ttempt_number\x18\x06 \x01(\x05\x12,\n\x06output\x18\x04 \x01(\x0b\x32\x1a.littlehorse.VariableValueH\x00\x12)\n\x05\x65rror\x18\x07 \x01(\x0b\x32\x18.littlehorse.LHTaskErrorH\x00\x12\x31\n\texception\x18\x08 \x01(\x0b\x32\x1c.littlehorse.LHTaskExceptionH\x00\x42\x08\n\x06resultB\r\n\x0b_log_output\"V\n\x10StopWfRunRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x19\n\x11thread_run_number\x18\x02 \x01(\x05\"X\n\x12ResumeWfRunRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\x12\x19\n\x11thread_run_number\x18\x02 \x01(\x05\"\xb3\x01\n\x1aTaskDefMetricsQueryRequest\x12\x30\n\x0cwindow_start\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x0bwindow_type\x18\x02 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x1a\n\rtask_def_name\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x10\n\x0e_task_def_name\"\xca\x01\n\x16ListTaskMetricsRequest\x12+\n\x0btask_def_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x35\n\x11last_window_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\rwindow_length\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x13\n\x0bnum_windows\x18\x04 \x01(\x05\"G\n\x17ListTaskMetricsResponse\x12,\n\x07results\x18\x01 \x03(\x0b\x32\x1b.littlehorse.TaskDefMetrics\"\xb1\x01\n\x19WfSpecMetricsQueryRequest\x12)\n\nwf_spec_id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x30\n\x0cwindow_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\rwindow_length\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\"\xc6\x01\n\x14ListWfMetricsRequest\x12)\n\nwf_spec_id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x35\n\x11last_window_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\rwindow_length\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x13\n\x0bnum_windows\x18\x04 \x01(\x05\"D\n\x15ListWfMetricsResponse\x12+\n\x07results\x18\x01 \x03(\x0b\x32\x1a.littlehorse.WfSpecMetrics\"\xfb\x02\n\x0eTaskDefMetrics\x12+\n\x0btask_def_id\x18\x01 \x01(\x0b\x32\x16.littlehorse.TaskDefId\x12\x30\n\x0cwindow_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x04type\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x1d\n\x15schedule_to_start_max\x18\x04 \x01(\x03\x12\x1d\n\x15schedule_to_start_avg\x18\x05 \x01(\x03\x12\x1d\n\x15start_to_complete_max\x18\x06 \x01(\x03\x12\x1d\n\x15start_to_complete_avg\x18\x07 \x01(\x03\x12\x17\n\x0ftotal_completed\x18\x08 \x01(\x03\x12\x15\n\rtotal_errored\x18\t \x01(\x03\x12\x15\n\rtotal_started\x18\n \x01(\x03\x12\x17\n\x0ftotal_scheduled\x18\x0b \x01(\x03\"\xa1\x02\n\rWfSpecMetrics\x12)\n\nwf_spec_id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x30\n\x0cwindow_start\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x04type\x18\x03 \x01(\x0e\x32 .littlehorse.MetricsWindowLength\x12\x15\n\rtotal_started\x18\x04 \x01(\x03\x12\x17\n\x0ftotal_completed\x18\x05 \x01(\x03\x12\x15\n\rtotal_errored\x18\x06 \x01(\x03\x12\x1d\n\x15start_to_complete_max\x18\x07 \x01(\x03\x12\x1d\n\x15start_to_complete_avg\x18\x08 \x01(\x03\"A\n\x16ListUserTaskRunRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"<\n\x0fUserTaskRunList\x12)\n\x07results\x18\x01 \x03(\x0b\x32\x18.littlehorse.UserTaskRun\"\x8a\x01\n\x12TaskWorkerMetadata\x12\x16\n\x0etask_worker_id\x18\x01 \x01(\t\x12\x34\n\x10latest_heartbeat\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x05hosts\x18\x03 \x03(\x0b\x32\x17.littlehorse.LHHostInfo\"\x87\x02\n\x0fTaskWorkerGroup\x12*\n\x02id\x18\x01 \x01(\x0b\x32\x1e.littlehorse.TaskWorkerGroupId\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\x0ctask_workers\x18\x03 \x03(\x0b\x32-.littlehorse.TaskWorkerGroup.TaskWorkersEntry\x1aS\n\x10TaskWorkersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.littlehorse.TaskWorkerMetadata:\x02\x38\x01\">\n\x13ListTaskRunsRequest\x12\'\n\twf_run_id\x18\x01 \x01(\x0b\x32\x14.littlehorse.WfRunId\"4\n\x0bTaskRunList\x12%\n\x07results\x18\x01 \x03(\x0b\x32\x14.littlehorse.TaskRun\"z\n\x14MigrateWfSpecRequest\x12*\n\x0bold_wf_spec\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12\x36\n\tmigration\x18\x02 \x01(\x0b\x32#.littlehorse.WfSpecVersionMigration\"T\n\x16GetLatestWfSpecRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1a\n\rmajor_version\x18\x02 \x01(\x05H\x00\x88\x01\x01\x42\x10\n\x0e_major_version\"\x9c\x01\n\x15ServerVersionResponse\x12\x15\n\rmajor_version\x18\x01 \x01(\x05\x12\x15\n\rminor_version\x18\x02 \x01(\x05\x12\x15\n\rpatch_version\x18\x03 \x01(\x05\x12#\n\x16pre_release_identifier\x18\x04 \x01(\tH\x00\x88\x01\x01\x42\x19\n\x17_pre_release_identifier*P\n\x11\x41llowedUpdateType\x12\x0f\n\x0b\x41LL_UPDATES\x10\x00\x12\x1a\n\x16MINOR_REVISION_UPDATES\x10\x01\x12\x0e\n\nNO_UPDATES\x10\x02\x32\xbe%\n\x0bLittleHorse\x12\x44\n\nPutTaskDef\x12\x1e.littlehorse.PutTaskDefRequest\x1a\x14.littlehorse.TaskDef\"\x00\x12<\n\nGetTaskDef\x12\x16.littlehorse.TaskDefId\x1a\x14.littlehorse.TaskDef\"\x00\x12L\n\x12GetTaskWorkerGroup\x12\x16.littlehorse.TaskDefId\x1a\x1c.littlehorse.TaskWorkerGroup\"\x00\x12_\n\x13PutExternalEventDef\x12\'.littlehorse.PutExternalEventDefRequest\x1a\x1d.littlehorse.ExternalEventDef\"\x00\x12W\n\x13GetExternalEventDef\x12\x1f.littlehorse.ExternalEventDefId\x1a\x1d.littlehorse.ExternalEventDef\"\x00\x12_\n\x13PutWorkflowEventDef\x12\'.littlehorse.PutWorkflowEventDefRequest\x1a\x1d.littlehorse.WorkflowEventDef\"\x00\x12\x41\n\tPutWfSpec\x12\x1d.littlehorse.PutWfSpecRequest\x1a\x13.littlehorse.WfSpec\"\x00\x12\x39\n\tGetWfSpec\x12\x15.littlehorse.WfSpecId\x1a\x13.littlehorse.WfSpec\"\x00\x12M\n\x0fGetLatestWfSpec\x12#.littlehorse.GetLatestWfSpecRequest\x1a\x13.littlehorse.WfSpec\"\x00\x12I\n\rMigrateWfSpec\x12!.littlehorse.MigrateWfSpecRequest\x1a\x13.littlehorse.WfSpec\"\x00\x12P\n\x0ePutUserTaskDef\x12\".littlehorse.PutUserTaskDefRequest\x1a\x18.littlehorse.UserTaskDef\"\x00\x12H\n\x0eGetUserTaskDef\x12\x1a.littlehorse.UserTaskDefId\x1a\x18.littlehorse.UserTaskDef\"\x00\x12\\\n\x14GetLatestUserTaskDef\x12(.littlehorse.GetLatestUserTaskDefRequest\x1a\x18.littlehorse.UserTaskDef\"\x00\x12\x38\n\x05RunWf\x12\x19.littlehorse.RunWfRequest\x1a\x12.littlehorse.WfRun\"\x00\x12\x36\n\x08GetWfRun\x12\x14.littlehorse.WfRunId\x1a\x12.littlehorse.WfRun\"\x00\x12H\n\x0eGetUserTaskRun\x12\x1a.littlehorse.UserTaskRunId\x1a\x18.littlehorse.UserTaskRun\"\x00\x12T\n\x11\x41ssignUserTaskRun\x12%.littlehorse.AssignUserTaskRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12X\n\x13\x43ompleteUserTaskRun\x12\'.littlehorse.CompleteUserTaskRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x11\x43\x61ncelUserTaskRun\x12%.littlehorse.CancelUserTaskRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12W\n\x10ListUserTaskRuns\x12#.littlehorse.ListUserTaskRunRequest\x1a\x1c.littlehorse.UserTaskRunList\"\x00\x12<\n\nGetNodeRun\x12\x16.littlehorse.NodeRunId\x1a\x14.littlehorse.NodeRun\"\x00\x12L\n\x0cListNodeRuns\x12 .littlehorse.ListNodeRunsRequest\x1a\x18.littlehorse.NodeRunList\"\x00\x12<\n\nGetTaskRun\x12\x16.littlehorse.TaskRunId\x1a\x14.littlehorse.TaskRun\"\x00\x12L\n\x0cListTaskRuns\x12 .littlehorse.ListTaskRunsRequest\x1a\x18.littlehorse.TaskRunList\"\x00\x12?\n\x0bGetVariable\x12\x17.littlehorse.VariableId\x1a\x15.littlehorse.Variable\"\x00\x12O\n\rListVariables\x12!.littlehorse.ListVariablesRequest\x1a\x19.littlehorse.VariableList\"\x00\x12V\n\x10PutExternalEvent\x12$.littlehorse.PutExternalEventRequest\x1a\x1a.littlehorse.ExternalEvent\"\x00\x12N\n\x10GetExternalEvent\x12\x1c.littlehorse.ExternalEventId\x1a\x1a.littlehorse.ExternalEvent\"\x00\x12Z\n\x12\x41waitWorkflowEvent\x12&.littlehorse.AwaitWorkflowEventRequest\x1a\x1a.littlehorse.WorkflowEvent\"\x00\x12^\n\x12ListExternalEvents\x12&.littlehorse.ListExternalEventsRequest\x1a\x1e.littlehorse.ExternalEventList\"\x00\x12J\n\x0bSearchWfRun\x12\x1f.littlehorse.SearchWfRunRequest\x1a\x18.littlehorse.WfRunIdList\"\x00\x12P\n\rSearchNodeRun\x12!.littlehorse.SearchNodeRunRequest\x1a\x1a.littlehorse.NodeRunIdList\"\x00\x12P\n\rSearchTaskRun\x12!.littlehorse.SearchTaskRunRequest\x1a\x1a.littlehorse.TaskRunIdList\"\x00\x12\\\n\x11SearchUserTaskRun\x12%.littlehorse.SearchUserTaskRunRequest\x1a\x1e.littlehorse.UserTaskRunIdList\"\x00\x12S\n\x0eSearchVariable\x12\".littlehorse.SearchVariableRequest\x1a\x1b.littlehorse.VariableIdList\"\x00\x12\x62\n\x13SearchExternalEvent\x12\'.littlehorse.SearchExternalEventRequest\x1a .littlehorse.ExternalEventIdList\"\x00\x12P\n\rSearchTaskDef\x12!.littlehorse.SearchTaskDefRequest\x1a\x1a.littlehorse.TaskDefIdList\"\x00\x12\\\n\x11SearchUserTaskDef\x12%.littlehorse.SearchUserTaskDefRequest\x1a\x1e.littlehorse.UserTaskDefIdList\"\x00\x12M\n\x0cSearchWfSpec\x12 .littlehorse.SearchWfSpecRequest\x1a\x19.littlehorse.WfSpecIdList\"\x00\x12k\n\x16SearchExternalEventDef\x12*.littlehorse.SearchExternalEventDefRequest\x1a#.littlehorse.ExternalEventDefIdList\"\x00\x12M\n\x0cSearchTenant\x12 .littlehorse.SearchTenantRequest\x1a\x19.littlehorse.TenantIdList\"\x00\x12g\n\x12RegisterTaskWorker\x12&.littlehorse.RegisterTaskWorkerRequest\x1a\'.littlehorse.RegisterTaskWorkerResponse\"\x00\x12M\n\x08PollTask\x12\x1c.littlehorse.PollTaskRequest\x1a\x1d.littlehorse.PollTaskResponse\"\x00(\x01\x30\x01\x12\x42\n\nReportTask\x12\x1a.littlehorse.ReportTaskRun\x1a\x16.google.protobuf.Empty\"\x00\x12\x44\n\tStopWfRun\x12\x1d.littlehorse.StopWfRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0bResumeWfRun\x12\x1f.littlehorse.ResumeWfRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12H\n\x0b\x44\x65leteWfRun\x12\x1f.littlehorse.DeleteWfRunRequest\x1a\x16.google.protobuf.Empty\"\x00\x12L\n\rDeleteTaskDef\x12!.littlehorse.DeleteTaskDefRequest\x1a\x16.google.protobuf.Empty\"\x00\x12J\n\x0c\x44\x65leteWfSpec\x12 .littlehorse.DeleteWfSpecRequest\x1a\x16.google.protobuf.Empty\"\x00\x12T\n\x11\x44\x65leteUserTaskDef\x12%.littlehorse.DeleteUserTaskDefRequest\x1a\x16.google.protobuf.Empty\"\x00\x12^\n\x16\x44\x65leteExternalEventDef\x12*.littlehorse.DeleteExternalEventDefRequest\x1a\x16.google.protobuf.Empty\"\x00\x12\x61\n\x17GetTaskDefMetricsWindow\x12\'.littlehorse.TaskDefMetricsQueryRequest\x1a\x1b.littlehorse.TaskDefMetrics\"\x00\x12^\n\x16GetWfSpecMetricsWindow\x12&.littlehorse.WfSpecMetricsQueryRequest\x1a\x1a.littlehorse.WfSpecMetrics\"\x00\x12\x61\n\x12ListTaskDefMetrics\x12#.littlehorse.ListTaskMetricsRequest\x1a$.littlehorse.ListTaskMetricsResponse\"\x00\x12\\\n\x11ListWfSpecMetrics\x12!.littlehorse.ListWfMetricsRequest\x1a\".littlehorse.ListWfMetricsResponse\"\x00\x12\x41\n\tPutTenant\x12\x1d.littlehorse.PutTenantRequest\x1a\x13.littlehorse.Tenant\"\x00\x12J\n\x0cPutPrincipal\x12 .littlehorse.PutPrincipalRequest\x1a\x16.littlehorse.Principal\"\x00\x12:\n\x06Whoami\x12\x16.google.protobuf.Empty\x1a\x16.littlehorse.Principal\"\x00\x12P\n\x10GetServerVersion\x12\x16.google.protobuf.Empty\x1a\".littlehorse.ServerVersionResponse\"\x00\x42G\n\x1fio.littlehorse.sdk.common.protoP\x01Z\x07.;model\xaa\x02\x18LittleHorse.Common.Protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\037io.littlehorse.sdk.common.protoP\001Z\007.;model\252\002\030LittleHorse.Common.Proto'
   _PUTWFSPECREQUEST_THREADSPECSENTRY._options = None
   _PUTWFSPECREQUEST_THREADSPECSENTRY._serialized_options = b'8\001'
   _RUNWFREQUEST_VARIABLESENTRY._options = None
   _RUNWFREQUEST_VARIABLESENTRY._serialized_options = b'8\001'
-  _globals['_ALLOWEDUPDATETYPE']._serialized_start=10603
-  _globals['_ALLOWEDUPDATETYPE']._serialized_end=10683
+  _TASKWORKERGROUP_TASKWORKERSENTRY._options = None
+  _TASKWORKERGROUP_TASKWORKERSENTRY._serialized_options = b'8\001'
+  _globals['_ALLOWEDUPDATETYPE']._serialized_start=11348
+  _globals['_ALLOWEDUPDATETYPE']._serialized_end=11428
   _globals['_GETLATESTUSERTASKDEFREQUEST']._serialized_start=317
   _globals['_GETLATESTUSERTASKDEFREQUEST']._serialized_end=360
   _globals['_PUTWFSPECREQUEST']._serialized_start=363
   _globals['_PUTWFSPECREQUEST']._serialized_end=830
   _globals['_PUTWFSPECREQUEST_THREADSPECSENTRY']._serialized_start=697
   _globals['_PUTWFSPECREQUEST_THREADSPECSENTRY']._serialized_end=772
   _globals['_PUTTASKDEFREQUEST']._serialized_start=832
@@ -113,78 +115,88 @@
   _globals['_SEARCHWFSPECREQUEST']._serialized_end=5725
   _globals['_WFSPECIDLIST']._serialized_start=5727
   _globals['_WFSPECIDLIST']._serialized_end=5817
   _globals['_SEARCHEXTERNALEVENTDEFREQUEST']._serialized_start=5820
   _globals['_SEARCHEXTERNALEVENTDEFREQUEST']._serialized_end=5949
   _globals['_EXTERNALEVENTDEFIDLIST']._serialized_start=5951
   _globals['_EXTERNALEVENTDEFIDLIST']._serialized_end=6061
-  _globals['_SEARCHEXTERNALEVENTREQUEST']._serialized_start=6064
-  _globals['_SEARCHEXTERNALEVENTREQUEST']._serialized_end=6448
-  _globals['_SEARCHEXTERNALEVENTREQUEST_BYEXTEVTDEFNAMEANDSTATUSREQUEST']._serialized_start=6299
-  _globals['_SEARCHEXTERNALEVENTREQUEST_BYEXTEVTDEFNAMEANDSTATUSREQUEST']._serialized_end=6405
-  _globals['_EXTERNALEVENTIDLIST']._serialized_start=6450
-  _globals['_EXTERNALEVENTIDLIST']._serialized_end=6554
-  _globals['_LISTNODERUNSREQUEST']._serialized_start=6556
-  _globals['_LISTNODERUNSREQUEST']._serialized_end=6618
-  _globals['_NODERUNLIST']._serialized_start=6620
-  _globals['_NODERUNLIST']._serialized_end=6672
-  _globals['_LISTVARIABLESREQUEST']._serialized_start=6674
-  _globals['_LISTVARIABLESREQUEST']._serialized_end=6737
-  _globals['_VARIABLELIST']._serialized_start=6739
-  _globals['_VARIABLELIST']._serialized_end=6793
-  _globals['_LISTEXTERNALEVENTSREQUEST']._serialized_start=6795
-  _globals['_LISTEXTERNALEVENTSREQUEST']._serialized_end=6863
-  _globals['_EXTERNALEVENTLIST']._serialized_start=6865
-  _globals['_EXTERNALEVENTLIST']._serialized_end=6929
-  _globals['_REGISTERTASKWORKERREQUEST']._serialized_start=6931
-  _globals['_REGISTERTASKWORKERREQUEST']._serialized_end=7050
-  _globals['_TASKWORKERHEARTBEATREQUEST']._serialized_start=7052
-  _globals['_TASKWORKERHEARTBEATREQUEST']._serialized_end=7167
-  _globals['_REGISTERTASKWORKERRESPONSE']._serialized_start=7170
-  _globals['_REGISTERTASKWORKERRESPONSE']._serialized_end=7299
-  _globals['_LHHOSTINFO']._serialized_start=7301
-  _globals['_LHHOSTINFO']._serialized_end=7341
-  _globals['_POLLTASKREQUEST']._serialized_start=7344
-  _globals['_POLLTASKREQUEST']._serialized_end=7483
-  _globals['_SCHEDULEDTASK']._serialized_start=7486
-  _globals['_SCHEDULEDTASK']._serialized_end=7754
-  _globals['_POLLTASKRESPONSE']._serialized_start=7756
-  _globals['_POLLTASKRESPONSE']._serialized_end=7834
-  _globals['_REPORTTASKRUN']._serialized_start=7837
-  _globals['_REPORTTASKRUN']._serialized_end=8222
-  _globals['_STOPWFRUNREQUEST']._serialized_start=8224
-  _globals['_STOPWFRUNREQUEST']._serialized_end=8310
-  _globals['_RESUMEWFRUNREQUEST']._serialized_start=8312
-  _globals['_RESUMEWFRUNREQUEST']._serialized_end=8400
-  _globals['_TASKDEFMETRICSQUERYREQUEST']._serialized_start=8403
-  _globals['_TASKDEFMETRICSQUERYREQUEST']._serialized_end=8582
-  _globals['_LISTTASKMETRICSREQUEST']._serialized_start=8585
-  _globals['_LISTTASKMETRICSREQUEST']._serialized_end=8787
-  _globals['_LISTTASKMETRICSRESPONSE']._serialized_start=8789
-  _globals['_LISTTASKMETRICSRESPONSE']._serialized_end=8860
-  _globals['_WFSPECMETRICSQUERYREQUEST']._serialized_start=8863
-  _globals['_WFSPECMETRICSQUERYREQUEST']._serialized_end=9040
-  _globals['_LISTWFMETRICSREQUEST']._serialized_start=9043
-  _globals['_LISTWFMETRICSREQUEST']._serialized_end=9241
-  _globals['_LISTWFMETRICSRESPONSE']._serialized_start=9243
-  _globals['_LISTWFMETRICSRESPONSE']._serialized_end=9311
-  _globals['_TASKDEFMETRICS']._serialized_start=9314
-  _globals['_TASKDEFMETRICS']._serialized_end=9693
-  _globals['_WFSPECMETRICS']._serialized_start=9696
-  _globals['_WFSPECMETRICS']._serialized_end=9985
-  _globals['_LISTUSERTASKRUNREQUEST']._serialized_start=9987
-  _globals['_LISTUSERTASKRUNREQUEST']._serialized_end=10052
-  _globals['_USERTASKRUNLIST']._serialized_start=10054
-  _globals['_USERTASKRUNLIST']._serialized_end=10114
-  _globals['_LISTTASKRUNSREQUEST']._serialized_start=10116
-  _globals['_LISTTASKRUNSREQUEST']._serialized_end=10178
-  _globals['_TASKRUNLIST']._serialized_start=10180
-  _globals['_TASKRUNLIST']._serialized_end=10232
-  _globals['_MIGRATEWFSPECREQUEST']._serialized_start=10234
-  _globals['_MIGRATEWFSPECREQUEST']._serialized_end=10356
-  _globals['_GETLATESTWFSPECREQUEST']._serialized_start=10358
-  _globals['_GETLATESTWFSPECREQUEST']._serialized_end=10442
-  _globals['_SERVERVERSIONRESPONSE']._serialized_start=10445
-  _globals['_SERVERVERSIONRESPONSE']._serialized_end=10601
-  _globals['_LITTLEHORSE']._serialized_start=10686
-  _globals['_LITTLEHORSE']._serialized_end=15327
+  _globals['_SEARCHTENANTREQUEST']._serialized_start=6063
+  _globals['_SEARCHTENANTREQUEST']._serialized_end=6150
+  _globals['_TENANTIDLIST']._serialized_start=6152
+  _globals['_TENANTIDLIST']._serialized_end=6242
+  _globals['_SEARCHEXTERNALEVENTREQUEST']._serialized_start=6245
+  _globals['_SEARCHEXTERNALEVENTREQUEST']._serialized_end=6629
+  _globals['_SEARCHEXTERNALEVENTREQUEST_BYEXTEVTDEFNAMEANDSTATUSREQUEST']._serialized_start=6480
+  _globals['_SEARCHEXTERNALEVENTREQUEST_BYEXTEVTDEFNAMEANDSTATUSREQUEST']._serialized_end=6586
+  _globals['_EXTERNALEVENTIDLIST']._serialized_start=6631
+  _globals['_EXTERNALEVENTIDLIST']._serialized_end=6735
+  _globals['_LISTNODERUNSREQUEST']._serialized_start=6738
+  _globals['_LISTNODERUNSREQUEST']._serialized_end=6920
+  _globals['_NODERUNLIST']._serialized_start=6922
+  _globals['_NODERUNLIST']._serialized_end=7010
+  _globals['_LISTVARIABLESREQUEST']._serialized_start=7012
+  _globals['_LISTVARIABLESREQUEST']._serialized_end=7075
+  _globals['_VARIABLELIST']._serialized_start=7077
+  _globals['_VARIABLELIST']._serialized_end=7131
+  _globals['_LISTEXTERNALEVENTSREQUEST']._serialized_start=7133
+  _globals['_LISTEXTERNALEVENTSREQUEST']._serialized_end=7201
+  _globals['_EXTERNALEVENTLIST']._serialized_start=7203
+  _globals['_EXTERNALEVENTLIST']._serialized_end=7267
+  _globals['_REGISTERTASKWORKERREQUEST']._serialized_start=7269
+  _globals['_REGISTERTASKWORKERREQUEST']._serialized_end=7388
+  _globals['_TASKWORKERHEARTBEATREQUEST']._serialized_start=7390
+  _globals['_TASKWORKERHEARTBEATREQUEST']._serialized_end=7505
+  _globals['_REGISTERTASKWORKERRESPONSE']._serialized_start=7508
+  _globals['_REGISTERTASKWORKERRESPONSE']._serialized_end=7637
+  _globals['_LHHOSTINFO']._serialized_start=7639
+  _globals['_LHHOSTINFO']._serialized_end=7679
+  _globals['_POLLTASKREQUEST']._serialized_start=7682
+  _globals['_POLLTASKREQUEST']._serialized_end=7821
+  _globals['_SCHEDULEDTASK']._serialized_start=7824
+  _globals['_SCHEDULEDTASK']._serialized_end=8092
+  _globals['_POLLTASKRESPONSE']._serialized_start=8094
+  _globals['_POLLTASKRESPONSE']._serialized_end=8172
+  _globals['_REPORTTASKRUN']._serialized_start=8175
+  _globals['_REPORTTASKRUN']._serialized_end=8560
+  _globals['_STOPWFRUNREQUEST']._serialized_start=8562
+  _globals['_STOPWFRUNREQUEST']._serialized_end=8648
+  _globals['_RESUMEWFRUNREQUEST']._serialized_start=8650
+  _globals['_RESUMEWFRUNREQUEST']._serialized_end=8738
+  _globals['_TASKDEFMETRICSQUERYREQUEST']._serialized_start=8741
+  _globals['_TASKDEFMETRICSQUERYREQUEST']._serialized_end=8920
+  _globals['_LISTTASKMETRICSREQUEST']._serialized_start=8923
+  _globals['_LISTTASKMETRICSREQUEST']._serialized_end=9125
+  _globals['_LISTTASKMETRICSRESPONSE']._serialized_start=9127
+  _globals['_LISTTASKMETRICSRESPONSE']._serialized_end=9198
+  _globals['_WFSPECMETRICSQUERYREQUEST']._serialized_start=9201
+  _globals['_WFSPECMETRICSQUERYREQUEST']._serialized_end=9378
+  _globals['_LISTWFMETRICSREQUEST']._serialized_start=9381
+  _globals['_LISTWFMETRICSREQUEST']._serialized_end=9579
+  _globals['_LISTWFMETRICSRESPONSE']._serialized_start=9581
+  _globals['_LISTWFMETRICSRESPONSE']._serialized_end=9649
+  _globals['_TASKDEFMETRICS']._serialized_start=9652
+  _globals['_TASKDEFMETRICS']._serialized_end=10031
+  _globals['_WFSPECMETRICS']._serialized_start=10034
+  _globals['_WFSPECMETRICS']._serialized_end=10323
+  _globals['_LISTUSERTASKRUNREQUEST']._serialized_start=10325
+  _globals['_LISTUSERTASKRUNREQUEST']._serialized_end=10390
+  _globals['_USERTASKRUNLIST']._serialized_start=10392
+  _globals['_USERTASKRUNLIST']._serialized_end=10452
+  _globals['_TASKWORKERMETADATA']._serialized_start=10455
+  _globals['_TASKWORKERMETADATA']._serialized_end=10593
+  _globals['_TASKWORKERGROUP']._serialized_start=10596
+  _globals['_TASKWORKERGROUP']._serialized_end=10859
+  _globals['_TASKWORKERGROUP_TASKWORKERSENTRY']._serialized_start=10776
+  _globals['_TASKWORKERGROUP_TASKWORKERSENTRY']._serialized_end=10859
+  _globals['_LISTTASKRUNSREQUEST']._serialized_start=10861
+  _globals['_LISTTASKRUNSREQUEST']._serialized_end=10923
+  _globals['_TASKRUNLIST']._serialized_start=10925
+  _globals['_TASKRUNLIST']._serialized_end=10977
+  _globals['_MIGRATEWFSPECREQUEST']._serialized_start=10979
+  _globals['_MIGRATEWFSPECREQUEST']._serialized_end=11101
+  _globals['_GETLATESTWFSPECREQUEST']._serialized_start=11103
+  _globals['_GETLATESTWFSPECREQUEST']._serialized_end=11187
+  _globals['_SERVERVERSIONRESPONSE']._serialized_start=11190
+  _globals['_SERVERVERSIONRESPONSE']._serialized_end=11346
+  _globals['_LITTLEHORSE']._serialized_start=11431
+  _globals['_LITTLEHORSE']._serialized_end=16229
 # @@protoc_insertion_point(module_scope)
```

### Comparing `littlehorse_client-0.8.1/littlehorse/model/service_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/service_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -412,14 +412,30 @@
     __slots__ = ["results", "bookmark"]
     RESULTS_FIELD_NUMBER: _ClassVar[int]
     BOOKMARK_FIELD_NUMBER: _ClassVar[int]
     results: _containers.RepeatedCompositeFieldContainer[_object_id_pb2.ExternalEventDefId]
     bookmark: bytes
     def __init__(self, results: _Optional[_Iterable[_Union[_object_id_pb2.ExternalEventDefId, _Mapping]]] = ..., bookmark: _Optional[bytes] = ...) -> None: ...
 
+class SearchTenantRequest(_message.Message):
+    __slots__ = ["limit", "bookmark"]
+    LIMIT_FIELD_NUMBER: _ClassVar[int]
+    BOOKMARK_FIELD_NUMBER: _ClassVar[int]
+    limit: int
+    bookmark: bytes
+    def __init__(self, limit: _Optional[int] = ..., bookmark: _Optional[bytes] = ...) -> None: ...
+
+class TenantIdList(_message.Message):
+    __slots__ = ["results", "bookmark"]
+    RESULTS_FIELD_NUMBER: _ClassVar[int]
+    BOOKMARK_FIELD_NUMBER: _ClassVar[int]
+    results: _containers.RepeatedCompositeFieldContainer[_object_id_pb2.TenantId]
+    bookmark: bytes
+    def __init__(self, results: _Optional[_Iterable[_Union[_object_id_pb2.TenantId, _Mapping]]] = ..., bookmark: _Optional[bytes] = ...) -> None: ...
+
 class SearchExternalEventRequest(_message.Message):
     __slots__ = ["bookmark", "limit", "wf_run_id", "external_event_def_name_and_status"]
     class ByExtEvtDefNameAndStatusRequest(_message.Message):
         __slots__ = ["external_event_def_name", "is_claimed"]
         EXTERNAL_EVENT_DEF_NAME_FIELD_NUMBER: _ClassVar[int]
         IS_CLAIMED_FIELD_NUMBER: _ClassVar[int]
         external_event_def_name: str
@@ -440,24 +456,32 @@
     RESULTS_FIELD_NUMBER: _ClassVar[int]
     BOOKMARK_FIELD_NUMBER: _ClassVar[int]
     results: _containers.RepeatedCompositeFieldContainer[_object_id_pb2.ExternalEventId]
     bookmark: bytes
     def __init__(self, results: _Optional[_Iterable[_Union[_object_id_pb2.ExternalEventId, _Mapping]]] = ..., bookmark: _Optional[bytes] = ...) -> None: ...
 
 class ListNodeRunsRequest(_message.Message):
-    __slots__ = ["wf_run_id"]
+    __slots__ = ["wf_run_id", "thread_run_number", "bookmark", "limit"]
     WF_RUN_ID_FIELD_NUMBER: _ClassVar[int]
+    THREAD_RUN_NUMBER_FIELD_NUMBER: _ClassVar[int]
+    BOOKMARK_FIELD_NUMBER: _ClassVar[int]
+    LIMIT_FIELD_NUMBER: _ClassVar[int]
     wf_run_id: _object_id_pb2.WfRunId
-    def __init__(self, wf_run_id: _Optional[_Union[_object_id_pb2.WfRunId, _Mapping]] = ...) -> None: ...
+    thread_run_number: int
+    bookmark: bytes
+    limit: int
+    def __init__(self, wf_run_id: _Optional[_Union[_object_id_pb2.WfRunId, _Mapping]] = ..., thread_run_number: _Optional[int] = ..., bookmark: _Optional[bytes] = ..., limit: _Optional[int] = ...) -> None: ...
 
 class NodeRunList(_message.Message):
-    __slots__ = ["results"]
+    __slots__ = ["results", "bookmark"]
     RESULTS_FIELD_NUMBER: _ClassVar[int]
+    BOOKMARK_FIELD_NUMBER: _ClassVar[int]
     results: _containers.RepeatedCompositeFieldContainer[_node_run_pb2.NodeRun]
-    def __init__(self, results: _Optional[_Iterable[_Union[_node_run_pb2.NodeRun, _Mapping]]] = ...) -> None: ...
+    bookmark: bytes
+    def __init__(self, results: _Optional[_Iterable[_Union[_node_run_pb2.NodeRun, _Mapping]]] = ..., bookmark: _Optional[bytes] = ...) -> None: ...
 
 class ListVariablesRequest(_message.Message):
     __slots__ = ["wf_run_id"]
     WF_RUN_ID_FIELD_NUMBER: _ClassVar[int]
     wf_run_id: _object_id_pb2.WfRunId
     def __init__(self, wf_run_id: _Optional[_Union[_object_id_pb2.WfRunId, _Mapping]] = ...) -> None: ...
 
@@ -693,14 +717,41 @@
 
 class UserTaskRunList(_message.Message):
     __slots__ = ["results"]
     RESULTS_FIELD_NUMBER: _ClassVar[int]
     results: _containers.RepeatedCompositeFieldContainer[_user_tasks_pb2.UserTaskRun]
     def __init__(self, results: _Optional[_Iterable[_Union[_user_tasks_pb2.UserTaskRun, _Mapping]]] = ...) -> None: ...
 
+class TaskWorkerMetadata(_message.Message):
+    __slots__ = ["task_worker_id", "latest_heartbeat", "hosts"]
+    TASK_WORKER_ID_FIELD_NUMBER: _ClassVar[int]
+    LATEST_HEARTBEAT_FIELD_NUMBER: _ClassVar[int]
+    HOSTS_FIELD_NUMBER: _ClassVar[int]
+    task_worker_id: str
+    latest_heartbeat: _timestamp_pb2.Timestamp
+    hosts: _containers.RepeatedCompositeFieldContainer[LHHostInfo]
+    def __init__(self, task_worker_id: _Optional[str] = ..., latest_heartbeat: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., hosts: _Optional[_Iterable[_Union[LHHostInfo, _Mapping]]] = ...) -> None: ...
+
+class TaskWorkerGroup(_message.Message):
+    __slots__ = ["id", "created_at", "task_workers"]
+    class TaskWorkersEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: TaskWorkerMetadata
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[TaskWorkerMetadata, _Mapping]] = ...) -> None: ...
+    ID_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    TASK_WORKERS_FIELD_NUMBER: _ClassVar[int]
+    id: _object_id_pb2.TaskWorkerGroupId
+    created_at: _timestamp_pb2.Timestamp
+    task_workers: _containers.MessageMap[str, TaskWorkerMetadata]
+    def __init__(self, id: _Optional[_Union[_object_id_pb2.TaskWorkerGroupId, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., task_workers: _Optional[_Mapping[str, TaskWorkerMetadata]] = ...) -> None: ...
+
 class ListTaskRunsRequest(_message.Message):
     __slots__ = ["wf_run_id"]
     WF_RUN_ID_FIELD_NUMBER: _ClassVar[int]
     wf_run_id: _object_id_pb2.WfRunId
     def __init__(self, wf_run_id: _Optional[_Union[_object_id_pb2.WfRunId, _Mapping]] = ...) -> None: ...
 
 class TaskRunList(_message.Message):
```

### Comparing `littlehorse_client-0.8.1/littlehorse/model/service_pb2_grpc.py` & `littlehorse_client-0.9.0/littlehorse/model/service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,19 @@
                 response_deserializer=task__def__pb2.TaskDef.FromString,
                 )
         self.GetTaskDef = channel.unary_unary(
                 '/littlehorse.LittleHorse/GetTaskDef',
                 request_serializer=object__id__pb2.TaskDefId.SerializeToString,
                 response_deserializer=task__def__pb2.TaskDef.FromString,
                 )
+        self.GetTaskWorkerGroup = channel.unary_unary(
+                '/littlehorse.LittleHorse/GetTaskWorkerGroup',
+                request_serializer=object__id__pb2.TaskDefId.SerializeToString,
+                response_deserializer=service__pb2.TaskWorkerGroup.FromString,
+                )
         self.PutExternalEventDef = channel.unary_unary(
                 '/littlehorse.LittleHorse/PutExternalEventDef',
                 request_serializer=service__pb2.PutExternalEventDefRequest.SerializeToString,
                 response_deserializer=external__event__pb2.ExternalEventDef.FromString,
                 )
         self.GetExternalEventDef = channel.unary_unary(
                 '/littlehorse.LittleHorse/GetExternalEventDef',
@@ -217,14 +222,19 @@
                 response_deserializer=service__pb2.WfSpecIdList.FromString,
                 )
         self.SearchExternalEventDef = channel.unary_unary(
                 '/littlehorse.LittleHorse/SearchExternalEventDef',
                 request_serializer=service__pb2.SearchExternalEventDefRequest.SerializeToString,
                 response_deserializer=service__pb2.ExternalEventDefIdList.FromString,
                 )
+        self.SearchTenant = channel.unary_unary(
+                '/littlehorse.LittleHorse/SearchTenant',
+                request_serializer=service__pb2.SearchTenantRequest.SerializeToString,
+                response_deserializer=service__pb2.TenantIdList.FromString,
+                )
         self.RegisterTaskWorker = channel.unary_unary(
                 '/littlehorse.LittleHorse/RegisterTaskWorker',
                 request_serializer=service__pb2.RegisterTaskWorkerRequest.SerializeToString,
                 response_deserializer=service__pb2.RegisterTaskWorkerResponse.FromString,
                 )
         self.PollTask = channel.stream_stream(
                 '/littlehorse.LittleHorse/PollTask',
@@ -326,14 +336,21 @@
     def GetTaskDef(self, request, context):
         """Gets a TaskDef.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetTaskWorkerGroup(self, request, context):
+        """Gets the registered task worker group associated with a specific TaskDef.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def PutExternalEventDef(self, request, context):
         """Creates an ExternalEventDef.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -369,15 +386,16 @@
         """Returns the latest WfSpec with a specified name (and optionally a specified Major Version).
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def MigrateWfSpec(self, request, context):
-        """EXPERIMENTAL: Migrates all WfRun's from one version of a WfSpec onto a newer version of the
+        """
+        EXPERIMENTAL: Migrates all WfRun's from one version of a WfSpec onto a newer version of the
         same WfSpec. This is useful for long-running WfRun's (eg. a 60-day marketing campaign) where
         you must update WfRun's that are in the RUNNING state rather than allowing them to run to
         completion.
 
         As of 0.7.2, this feature is only partially implemented.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
@@ -612,15 +630,22 @@
         """Search for WfSpec's.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SearchExternalEventDef(self, request, context):
-        """Search for ExteranlEventDef's.
+        """Search for ExternalEventDef's.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def SearchTenant(self, request, context):
+        """Search for all available TenantIds for current Principal
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def RegisterTaskWorker(self, request, context):
         """Used by the Task Worker to:
@@ -762,14 +787,19 @@
                     response_serializer=task__def__pb2.TaskDef.SerializeToString,
             ),
             'GetTaskDef': grpc.unary_unary_rpc_method_handler(
                     servicer.GetTaskDef,
                     request_deserializer=object__id__pb2.TaskDefId.FromString,
                     response_serializer=task__def__pb2.TaskDef.SerializeToString,
             ),
+            'GetTaskWorkerGroup': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetTaskWorkerGroup,
+                    request_deserializer=object__id__pb2.TaskDefId.FromString,
+                    response_serializer=service__pb2.TaskWorkerGroup.SerializeToString,
+            ),
             'PutExternalEventDef': grpc.unary_unary_rpc_method_handler(
                     servicer.PutExternalEventDef,
                     request_deserializer=service__pb2.PutExternalEventDefRequest.FromString,
                     response_serializer=external__event__pb2.ExternalEventDef.SerializeToString,
             ),
             'GetExternalEventDef': grpc.unary_unary_rpc_method_handler(
                     servicer.GetExternalEventDef,
@@ -947,14 +977,19 @@
                     response_serializer=service__pb2.WfSpecIdList.SerializeToString,
             ),
             'SearchExternalEventDef': grpc.unary_unary_rpc_method_handler(
                     servicer.SearchExternalEventDef,
                     request_deserializer=service__pb2.SearchExternalEventDefRequest.FromString,
                     response_serializer=service__pb2.ExternalEventDefIdList.SerializeToString,
             ),
+            'SearchTenant': grpc.unary_unary_rpc_method_handler(
+                    servicer.SearchTenant,
+                    request_deserializer=service__pb2.SearchTenantRequest.FromString,
+                    response_serializer=service__pb2.TenantIdList.SerializeToString,
+            ),
             'RegisterTaskWorker': grpc.unary_unary_rpc_method_handler(
                     servicer.RegisterTaskWorker,
                     request_deserializer=service__pb2.RegisterTaskWorkerRequest.FromString,
                     response_serializer=service__pb2.RegisterTaskWorkerResponse.SerializeToString,
             ),
             'PollTask': grpc.stream_stream_rpc_method_handler(
                     servicer.PollTask,
@@ -1082,14 +1117,31 @@
         return grpc.experimental.unary_unary(request, target, '/littlehorse.LittleHorse/GetTaskDef',
             object__id__pb2.TaskDefId.SerializeToString,
             task__def__pb2.TaskDef.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetTaskWorkerGroup(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/littlehorse.LittleHorse/GetTaskWorkerGroup',
+            object__id__pb2.TaskDefId.SerializeToString,
+            service__pb2.TaskWorkerGroup.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def PutExternalEventDef(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -1711,14 +1763,31 @@
         return grpc.experimental.unary_unary(request, target, '/littlehorse.LittleHorse/SearchExternalEventDef',
             service__pb2.SearchExternalEventDefRequest.SerializeToString,
             service__pb2.ExternalEventDefIdList.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def SearchTenant(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/littlehorse.LittleHorse/SearchTenant',
+            service__pb2.SearchTenantRequest.SerializeToString,
+            service__pb2.TenantIdList.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def RegisterTaskWorker(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `littlehorse_client-0.8.1/littlehorse/model/task_def_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/task_def_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/task_def_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/task_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/task_run_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/task_run_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/task_run_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/task_run_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/user_tasks_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/user_tasks_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/user_tasks_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/user_tasks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/variable_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/variable_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/variable_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/variable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/wf_run_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/wf_run_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/wf_run_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/wf_run_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/wf_spec_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/wf_spec_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 import littlehorse.model.common_enums_pb2 as common__enums__pb2
 import littlehorse.model.common_wfspec_pb2 as common__wfspec__pb2
 import littlehorse.model.object_id_pb2 as object__id__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rwf_spec.proto\x12\x0blittlehorse\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x12\x63ommon_enums.proto\x1a\x13\x63ommon_wfspec.proto\x1a\x0fobject_id.proto\"\xb4\x05\n\x06WfSpec\x12!\n\x02id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x10\x66rozen_variables\x18\x03 \x03(\x0b\x32\x19.littlehorse.ThreadVarDef\x12+\n\x06status\x18\x04 \x01(\x0e\x32\x1b.littlehorse.MetadataStatus\x12:\n\x0cthread_specs\x18\x05 \x03(\x0b\x32$.littlehorse.WfSpec.ThreadSpecsEntry\x12\x1e\n\x16\x65ntrypoint_thread_name\x18\x06 \x01(\t\x12\x43\n\x10retention_policy\x18\x07 \x01(\x0b\x32$.littlehorse.WorkflowRetentionPolicyH\x00\x88\x01\x01\x12;\n\tmigration\x18\x08 \x01(\x0b\x32#.littlehorse.WfSpecVersionMigrationH\x01\x88\x01\x01\x12\x46\n\x0eparent_wf_spec\x18\t \x01(\x0b\x32).littlehorse.WfSpec.ParentWfSpecReferenceH\x02\x88\x01\x01\x1aK\n\x10ThreadSpecsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ThreadSpec:\x02\x38\x01\x1aL\n\x15ParentWfSpecReference\x12\x14\n\x0cwf_spec_name\x18\x01 \x01(\t\x12\x1d\n\x15wf_spec_major_version\x18\x02 \x01(\x05\x42\x13\n\x11_retention_policyB\x0c\n\n_migrationB\x11\n\x0f_parent_wf_spec\"Q\n\x17WorkflowRetentionPolicy\x12&\n\x1cseconds_after_wf_termination\x18\x01 \x01(\x03H\x00\x42\x0e\n\x0cwf_gc_policy\"N\n\tJsonIndex\x12\x12\n\nfield_path\x18\x01 \x01(\t\x12-\n\nfield_type\x18\x02 \x01(\x0e\x32\x19.littlehorse.VariableType\"B\n\x15SearchableVariableDef\x12)\n\x07var_def\x18\x01 \x01(\x0b\x32\x18.littlehorse.VariableDef\"\xca\x01\n\x0cThreadVarDef\x12)\n\x07var_def\x18\x01 \x01(\x0b\x32\x18.littlehorse.VariableDef\x12\x10\n\x08required\x18\x02 \x01(\x08\x12\x12\n\nsearchable\x18\x03 \x01(\x08\x12,\n\x0cjson_indexes\x18\x04 \x03(\x0b\x32\x16.littlehorse.JsonIndex\x12;\n\x0c\x61\x63\x63\x65ss_level\x18\x05 \x01(\x0e\x32%.littlehorse.WfRunVariableAccessLevel\"\xbd\x02\n\nThreadSpec\x12\x31\n\x05nodes\x18\x01 \x03(\x0b\x32\".littlehorse.ThreadSpec.NodesEntry\x12\x30\n\rvariable_defs\x18\x02 \x03(\x0b\x32\x19.littlehorse.ThreadVarDef\x12\x31\n\x0einterrupt_defs\x18\x03 \x03(\x0b\x32\x19.littlehorse.InterruptDef\x12\x41\n\x10retention_policy\x18\x04 \x01(\x0b\x32\".littlehorse.ThreadRetentionPolicyH\x00\x88\x01\x01\x1a?\n\nNodesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12 \n\x05value\x18\x02 \x01(\x0b\x32\x11.littlehorse.Node:\x02\x38\x01\x42\x13\n\x11_retention_policy\"W\n\x15ThreadRetentionPolicy\x12*\n seconds_after_thread_termination\x18\x01 \x01(\x03H\x00\x42\x12\n\x10thread_gc_policy\"i\n\x0cInterruptDef\x12>\n\x15\x65xternal_event_def_id\x18\x01 \x01(\x0b\x32\x1f.littlehorse.ExternalEventDefId\x12\x19\n\x11handler_spec_name\x18\x02 \x01(\t\"\xbe\x01\n\x0fStartThreadNode\x12\x18\n\x10thread_spec_name\x18\x01 \x01(\t\x12>\n\tvariables\x18\x02 \x03(\x0b\x32+.littlehorse.StartThreadNode.VariablesEntry\x1aQ\n\x0eVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment:\x02\x38\x01\"\x83\x02\n\x18StartMultipleThreadsNode\x12\x18\n\x10thread_spec_name\x18\x01 \x01(\t\x12G\n\tvariables\x18\x02 \x03(\x0b\x32\x34.littlehorse.StartMultipleThreadsNode.VariablesEntry\x12\x31\n\x08iterable\x18\x03 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment\x1aQ\n\x0eVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment:\x02\x38\x01\"\xf0\x01\n\x11\x46\x61ilureHandlerDef\x12\x19\n\x11handler_spec_name\x18\x02 \x01(\t\x12\x1a\n\x10specific_failure\x18\x01 \x01(\tH\x00\x12K\n\x13\x61ny_failure_of_type\x18\x03 \x01(\x0e\x32,.littlehorse.FailureHandlerDef.LHFailureTypeH\x00\"C\n\rLHFailureType\x12\x16\n\x12\x46\x41ILURE_TYPE_ERROR\x10\x00\x12\x1a\n\x16\x46\x41ILURE_TYPE_EXCEPTION\x10\x01\x42\x12\n\x10\x66\x61ilure_to_catch\"\x92\x03\n\x12WaitForThreadsNode\x12\x43\n\x07threads\x18\x01 \x01(\x0b\x32\x30.littlehorse.WaitForThreadsNode.ThreadsToWaitForH\x00\x12\x36\n\x0bthread_list\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x00\x12\x43\n\x1bper_thread_failure_handlers\x18\x03 \x03(\x0b\x32\x1e.littlehorse.FailureHandlerDef\x1aM\n\x0fThreadToWaitFor\x12:\n\x11thread_run_number\x18\x01 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment\x1aT\n\x10ThreadsToWaitFor\x12@\n\x07threads\x18\x01 \x03(\x0b\x32/.littlehorse.WaitForThreadsNode.ThreadToWaitForB\x15\n\x13threads_to_wait_for\"\x8d\x01\n\x11\x45xternalEventNode\x12>\n\x15\x65xternal_event_def_id\x18\x01 \x01(\x0b\x32\x1f.littlehorse.ExternalEventDefId\x12\x38\n\x0ftimeout_seconds\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment\"\x10\n\x0e\x45ntrypointNode\"M\n\x08\x45xitNode\x12\x31\n\x0b\x66\x61ilure_def\x18\x01 \x01(\x0b\x32\x17.littlehorse.FailureDefH\x00\x88\x01\x01\x42\x0e\n\x0c_failure_def\"v\n\nFailureDef\x12\x14\n\x0c\x66\x61ilure_name\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x00\x88\x01\x01\x42\n\n\x08_content\"\x9c\x05\n\x04Node\x12)\n\x0eoutgoing_edges\x18\x01 \x03(\x0b\x32\x11.littlehorse.Edge\x12\x38\n\x10\x66\x61ilure_handlers\x18\x04 \x03(\x0b\x32\x1e.littlehorse.FailureHandlerDef\x12\x31\n\nentrypoint\x18\x05 \x01(\x0b\x32\x1b.littlehorse.EntrypointNodeH\x00\x12%\n\x04\x65xit\x18\x06 \x01(\x0b\x32\x15.littlehorse.ExitNodeH\x00\x12%\n\x04task\x18\x07 \x01(\x0b\x32\x15.littlehorse.TaskNodeH\x00\x12\x38\n\x0e\x65xternal_event\x18\x08 \x01(\x0b\x32\x1e.littlehorse.ExternalEventNodeH\x00\x12\x34\n\x0cstart_thread\x18\t \x01(\x0b\x32\x1c.littlehorse.StartThreadNodeH\x00\x12;\n\x10wait_for_threads\x18\n \x01(\x0b\x32\x1f.littlehorse.WaitForThreadsNodeH\x00\x12#\n\x03nop\x18\x0b \x01(\x0b\x32\x14.littlehorse.NopNodeH\x00\x12\'\n\x05sleep\x18\x0c \x01(\x0b\x32\x16.littlehorse.SleepNodeH\x00\x12.\n\tuser_task\x18\r \x01(\x0b\x32\x19.littlehorse.UserTaskNodeH\x00\x12G\n\x16start_multiple_threads\x18\x0f \x01(\x0b\x32%.littlehorse.StartMultipleThreadsNodeH\x00\x12\x32\n\x0bthrow_event\x18\x10 \x01(\x0b\x32\x1b.littlehorse.ThrowEventNodeH\x00\x42\x06\n\x04node\"y\n\x0eThrowEventNode\x12\x35\n\x0c\x65vent_def_id\x18\x01 \x01(\x0b\x32\x1f.littlehorse.WorkflowEventDefId\x12\x30\n\x07\x63ontent\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment\"\xe2\x02\n\x0cUserTaskNode\x12\x1a\n\x12user_task_def_name\x18\x01 \x01(\t\x12\x38\n\nuser_group\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x00\x88\x01\x01\x12\x35\n\x07user_id\x18\x03 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x01\x88\x01\x01\x12-\n\x07\x61\x63tions\x18\x04 \x03(\x0b\x32\x1c.littlehorse.UTActionTrigger\x12\"\n\x15user_task_def_version\x18\x05 \x01(\x05H\x02\x88\x01\x01\x12\x33\n\x05notes\x18\x06 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x03\x88\x01\x01\x42\r\n\x0b_user_groupB\n\n\x08_user_idB\x18\n\x16_user_task_def_versionB\x08\n\x06_notes\"\x9b\x01\n\rEdgeCondition\x12+\n\ncomparator\x18\x01 \x01(\x0e\x32\x17.littlehorse.Comparator\x12-\n\x04left\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment\x12.\n\x05right\x18\x03 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment\"\x9b\x01\n\x04\x45\x64ge\x12\x16\n\x0esink_node_name\x18\x01 \x01(\t\x12\x32\n\tcondition\x18\x02 \x01(\x0b\x32\x1a.littlehorse.EdgeConditionH\x00\x88\x01\x01\x12\x39\n\x12variable_mutations\x18\x03 \x03(\x0b\x32\x1d.littlehorse.VariableMutationB\x0c\n\n_condition\"\t\n\x07NopNode\"\xbe\x01\n\tSleepNode\x12\x36\n\x0braw_seconds\x18\x01 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x00\x12\x34\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x00\x12\x33\n\x08iso_date\x18\x03 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x00\x42\x0e\n\x0csleep_length\"\x87\x02\n\x16WfSpecVersionMigration\x12\x19\n\x11new_major_version\x18\x01 \x01(\x05\x12\x14\n\x0cnew_revision\x18\x02 \x01(\x05\x12]\n\x16thread_spec_migrations\x18\x03 \x03(\x0b\x32=.littlehorse.WfSpecVersionMigration.ThreadSpecMigrationsEntry\x1a]\n\x19ThreadSpecMigrationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .littlehorse.ThreadSpecMigration:\x02\x38\x01\"\xd5\x01\n\x13ThreadSpecMigration\x12\x1c\n\x14new_thread_spec_name\x18\x01 \x01(\t\x12M\n\x0fnode_migrations\x18\x02 \x03(\x0b\x32\x34.littlehorse.ThreadSpecMigration.NodeMigrationsEntry\x1aQ\n\x13NodeMigrationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.littlehorse.NodeMigration:\x02\x38\x01\"&\n\rNodeMigration\x12\x15\n\rnew_node_name\x18\x01 \x01(\t*N\n\x18WfRunVariableAccessLevel\x12\x0e\n\nPUBLIC_VAR\x10\x00\x12\x0f\n\x0bPRIVATE_VAR\x10\x01\x12\x11\n\rINHERITED_VAR\x10\x02\x42G\n\x1fio.littlehorse.sdk.common.protoP\x01Z\x07.;model\xaa\x02\x18LittleHorse.Common.Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rwf_spec.proto\x12\x0blittlehorse\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x12\x63ommon_enums.proto\x1a\x13\x63ommon_wfspec.proto\x1a\x0fobject_id.proto\"\xb4\x05\n\x06WfSpec\x12!\n\x02id\x18\x01 \x01(\x0b\x32\x15.littlehorse.WfSpecId\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x10\x66rozen_variables\x18\x03 \x03(\x0b\x32\x19.littlehorse.ThreadVarDef\x12+\n\x06status\x18\x04 \x01(\x0e\x32\x1b.littlehorse.MetadataStatus\x12:\n\x0cthread_specs\x18\x05 \x03(\x0b\x32$.littlehorse.WfSpec.ThreadSpecsEntry\x12\x1e\n\x16\x65ntrypoint_thread_name\x18\x06 \x01(\t\x12\x43\n\x10retention_policy\x18\x07 \x01(\x0b\x32$.littlehorse.WorkflowRetentionPolicyH\x00\x88\x01\x01\x12;\n\tmigration\x18\x08 \x01(\x0b\x32#.littlehorse.WfSpecVersionMigrationH\x01\x88\x01\x01\x12\x46\n\x0eparent_wf_spec\x18\t \x01(\x0b\x32).littlehorse.WfSpec.ParentWfSpecReferenceH\x02\x88\x01\x01\x1aK\n\x10ThreadSpecsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.littlehorse.ThreadSpec:\x02\x38\x01\x1aL\n\x15ParentWfSpecReference\x12\x14\n\x0cwf_spec_name\x18\x01 \x01(\t\x12\x1d\n\x15wf_spec_major_version\x18\x02 \x01(\x05\x42\x13\n\x11_retention_policyB\x0c\n\n_migrationB\x11\n\x0f_parent_wf_spec\"Q\n\x17WorkflowRetentionPolicy\x12&\n\x1cseconds_after_wf_termination\x18\x01 \x01(\x03H\x00\x42\x0e\n\x0cwf_gc_policy\"N\n\tJsonIndex\x12\x12\n\nfield_path\x18\x01 \x01(\t\x12-\n\nfield_type\x18\x02 \x01(\x0e\x32\x19.littlehorse.VariableType\"\xca\x01\n\x0cThreadVarDef\x12)\n\x07var_def\x18\x01 \x01(\x0b\x32\x18.littlehorse.VariableDef\x12\x10\n\x08required\x18\x02 \x01(\x08\x12\x12\n\nsearchable\x18\x03 \x01(\x08\x12,\n\x0cjson_indexes\x18\x04 \x03(\x0b\x32\x16.littlehorse.JsonIndex\x12;\n\x0c\x61\x63\x63\x65ss_level\x18\x05 \x01(\x0e\x32%.littlehorse.WfRunVariableAccessLevel\"\xbd\x02\n\nThreadSpec\x12\x31\n\x05nodes\x18\x01 \x03(\x0b\x32\".littlehorse.ThreadSpec.NodesEntry\x12\x30\n\rvariable_defs\x18\x02 \x03(\x0b\x32\x19.littlehorse.ThreadVarDef\x12\x31\n\x0einterrupt_defs\x18\x03 \x03(\x0b\x32\x19.littlehorse.InterruptDef\x12\x41\n\x10retention_policy\x18\x04 \x01(\x0b\x32\".littlehorse.ThreadRetentionPolicyH\x00\x88\x01\x01\x1a?\n\nNodesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12 \n\x05value\x18\x02 \x01(\x0b\x32\x11.littlehorse.Node:\x02\x38\x01\x42\x13\n\x11_retention_policy\"W\n\x15ThreadRetentionPolicy\x12*\n seconds_after_thread_termination\x18\x01 \x01(\x03H\x00\x42\x12\n\x10thread_gc_policy\"i\n\x0cInterruptDef\x12>\n\x15\x65xternal_event_def_id\x18\x01 \x01(\x0b\x32\x1f.littlehorse.ExternalEventDefId\x12\x19\n\x11handler_spec_name\x18\x02 \x01(\t\"\xbe\x01\n\x0fStartThreadNode\x12\x18\n\x10thread_spec_name\x18\x01 \x01(\t\x12>\n\tvariables\x18\x02 \x03(\x0b\x32+.littlehorse.StartThreadNode.VariablesEntry\x1aQ\n\x0eVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment:\x02\x38\x01\"\x83\x02\n\x18StartMultipleThreadsNode\x12\x18\n\x10thread_spec_name\x18\x01 \x01(\t\x12G\n\tvariables\x18\x02 \x03(\x0b\x32\x34.littlehorse.StartMultipleThreadsNode.VariablesEntry\x12\x31\n\x08iterable\x18\x03 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment\x1aQ\n\x0eVariablesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12.\n\x05value\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment:\x02\x38\x01\"\xf0\x01\n\x11\x46\x61ilureHandlerDef\x12\x19\n\x11handler_spec_name\x18\x02 \x01(\t\x12\x1a\n\x10specific_failure\x18\x01 \x01(\tH\x00\x12K\n\x13\x61ny_failure_of_type\x18\x03 \x01(\x0e\x32,.littlehorse.FailureHandlerDef.LHFailureTypeH\x00\"C\n\rLHFailureType\x12\x16\n\x12\x46\x41ILURE_TYPE_ERROR\x10\x00\x12\x1a\n\x16\x46\x41ILURE_TYPE_EXCEPTION\x10\x01\x42\x12\n\x10\x66\x61ilure_to_catch\"\x92\x03\n\x12WaitForThreadsNode\x12\x43\n\x07threads\x18\x01 \x01(\x0b\x32\x30.littlehorse.WaitForThreadsNode.ThreadsToWaitForH\x00\x12\x36\n\x0bthread_list\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x00\x12\x43\n\x1bper_thread_failure_handlers\x18\x03 \x03(\x0b\x32\x1e.littlehorse.FailureHandlerDef\x1aM\n\x0fThreadToWaitFor\x12:\n\x11thread_run_number\x18\x01 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment\x1aT\n\x10ThreadsToWaitFor\x12@\n\x07threads\x18\x01 \x03(\x0b\x32/.littlehorse.WaitForThreadsNode.ThreadToWaitForB\x15\n\x13threads_to_wait_for\"\x8d\x01\n\x11\x45xternalEventNode\x12>\n\x15\x65xternal_event_def_id\x18\x01 \x01(\x0b\x32\x1f.littlehorse.ExternalEventDefId\x12\x38\n\x0ftimeout_seconds\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment\"\x10\n\x0e\x45ntrypointNode\"M\n\x08\x45xitNode\x12\x31\n\x0b\x66\x61ilure_def\x18\x01 \x01(\x0b\x32\x17.littlehorse.FailureDefH\x00\x88\x01\x01\x42\x0e\n\x0c_failure_def\"v\n\nFailureDef\x12\x14\n\x0c\x66\x61ilure_name\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x00\x88\x01\x01\x42\n\n\x08_content\"\x9c\x05\n\x04Node\x12)\n\x0eoutgoing_edges\x18\x01 \x03(\x0b\x32\x11.littlehorse.Edge\x12\x38\n\x10\x66\x61ilure_handlers\x18\x04 \x03(\x0b\x32\x1e.littlehorse.FailureHandlerDef\x12\x31\n\nentrypoint\x18\x05 \x01(\x0b\x32\x1b.littlehorse.EntrypointNodeH\x00\x12%\n\x04\x65xit\x18\x06 \x01(\x0b\x32\x15.littlehorse.ExitNodeH\x00\x12%\n\x04task\x18\x07 \x01(\x0b\x32\x15.littlehorse.TaskNodeH\x00\x12\x38\n\x0e\x65xternal_event\x18\x08 \x01(\x0b\x32\x1e.littlehorse.ExternalEventNodeH\x00\x12\x34\n\x0cstart_thread\x18\t \x01(\x0b\x32\x1c.littlehorse.StartThreadNodeH\x00\x12;\n\x10wait_for_threads\x18\n \x01(\x0b\x32\x1f.littlehorse.WaitForThreadsNodeH\x00\x12#\n\x03nop\x18\x0b \x01(\x0b\x32\x14.littlehorse.NopNodeH\x00\x12\'\n\x05sleep\x18\x0c \x01(\x0b\x32\x16.littlehorse.SleepNodeH\x00\x12.\n\tuser_task\x18\r \x01(\x0b\x32\x19.littlehorse.UserTaskNodeH\x00\x12G\n\x16start_multiple_threads\x18\x0f \x01(\x0b\x32%.littlehorse.StartMultipleThreadsNodeH\x00\x12\x32\n\x0bthrow_event\x18\x10 \x01(\x0b\x32\x1b.littlehorse.ThrowEventNodeH\x00\x42\x06\n\x04node\"y\n\x0eThrowEventNode\x12\x35\n\x0c\x65vent_def_id\x18\x01 \x01(\x0b\x32\x1f.littlehorse.WorkflowEventDefId\x12\x30\n\x07\x63ontent\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment\"\xd3\x03\n\x0cUserTaskNode\x12\x1a\n\x12user_task_def_name\x18\x01 \x01(\t\x12\x38\n\nuser_group\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x00\x88\x01\x01\x12\x35\n\x07user_id\x18\x03 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x01\x88\x01\x01\x12-\n\x07\x61\x63tions\x18\x04 \x03(\x0b\x32\x1c.littlehorse.UTActionTrigger\x12\"\n\x15user_task_def_version\x18\x05 \x01(\x05H\x02\x88\x01\x01\x12\x33\n\x05notes\x18\x06 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x03\x88\x01\x01\x12L\n\x1eon_cancellation_exception_name\x18\x07 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x04\x88\x01\x01\x42\r\n\x0b_user_groupB\n\n\x08_user_idB\x18\n\x16_user_task_def_versionB\x08\n\x06_notesB!\n\x1f_on_cancellation_exception_name\"\x9b\x01\n\rEdgeCondition\x12+\n\ncomparator\x18\x01 \x01(\x0e\x32\x17.littlehorse.Comparator\x12-\n\x04left\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment\x12.\n\x05right\x18\x03 \x01(\x0b\x32\x1f.littlehorse.VariableAssignment\"\x9b\x01\n\x04\x45\x64ge\x12\x16\n\x0esink_node_name\x18\x01 \x01(\t\x12\x32\n\tcondition\x18\x02 \x01(\x0b\x32\x1a.littlehorse.EdgeConditionH\x00\x88\x01\x01\x12\x39\n\x12variable_mutations\x18\x03 \x03(\x0b\x32\x1d.littlehorse.VariableMutationB\x0c\n\n_condition\"\t\n\x07NopNode\"\xbe\x01\n\tSleepNode\x12\x36\n\x0braw_seconds\x18\x01 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x00\x12\x34\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x00\x12\x33\n\x08iso_date\x18\x03 \x01(\x0b\x32\x1f.littlehorse.VariableAssignmentH\x00\x42\x0e\n\x0csleep_length\"\x87\x02\n\x16WfSpecVersionMigration\x12\x19\n\x11new_major_version\x18\x01 \x01(\x05\x12\x14\n\x0cnew_revision\x18\x02 \x01(\x05\x12]\n\x16thread_spec_migrations\x18\x03 \x03(\x0b\x32=.littlehorse.WfSpecVersionMigration.ThreadSpecMigrationsEntry\x1a]\n\x19ThreadSpecMigrationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .littlehorse.ThreadSpecMigration:\x02\x38\x01\"\xd5\x01\n\x13ThreadSpecMigration\x12\x1c\n\x14new_thread_spec_name\x18\x01 \x01(\t\x12M\n\x0fnode_migrations\x18\x02 \x03(\x0b\x32\x34.littlehorse.ThreadSpecMigration.NodeMigrationsEntry\x1aQ\n\x13NodeMigrationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x1a.littlehorse.NodeMigration:\x02\x38\x01\"&\n\rNodeMigration\x12\x15\n\rnew_node_name\x18\x01 \x01(\t*N\n\x18WfRunVariableAccessLevel\x12\x0e\n\nPUBLIC_VAR\x10\x00\x12\x0f\n\x0bPRIVATE_VAR\x10\x01\x12\x11\n\rINHERITED_VAR\x10\x02\x42G\n\x1fio.littlehorse.sdk.common.protoP\x01Z\x07.;model\xaa\x02\x18LittleHorse.Common.Protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'wf_spec_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -34,82 +34,80 @@
   _STARTTHREADNODE_VARIABLESENTRY._serialized_options = b'8\001'
   _STARTMULTIPLETHREADSNODE_VARIABLESENTRY._options = None
   _STARTMULTIPLETHREADSNODE_VARIABLESENTRY._serialized_options = b'8\001'
   _WFSPECVERSIONMIGRATION_THREADSPECMIGRATIONSENTRY._options = None
   _WFSPECVERSIONMIGRATION_THREADSPECMIGRATIONSENTRY._serialized_options = b'8\001'
   _THREADSPECMIGRATION_NODEMIGRATIONSENTRY._options = None
   _THREADSPECMIGRATION_NODEMIGRATIONSENTRY._serialized_options = b'8\001'
-  _globals['_WFRUNVARIABLEACCESSLEVEL']._serialized_start=5425
-  _globals['_WFRUNVARIABLEACCESSLEVEL']._serialized_end=5503
+  _globals['_WFRUNVARIABLEACCESSLEVEL']._serialized_start=5470
+  _globals['_WFRUNVARIABLEACCESSLEVEL']._serialized_end=5548
   _globals['_WFSPEC']._serialized_start=122
   _globals['_WFSPEC']._serialized_end=814
   _globals['_WFSPEC_THREADSPECSENTRY']._serialized_start=607
   _globals['_WFSPEC_THREADSPECSENTRY']._serialized_end=682
   _globals['_WFSPEC_PARENTWFSPECREFERENCE']._serialized_start=684
   _globals['_WFSPEC_PARENTWFSPECREFERENCE']._serialized_end=760
   _globals['_WORKFLOWRETENTIONPOLICY']._serialized_start=816
   _globals['_WORKFLOWRETENTIONPOLICY']._serialized_end=897
   _globals['_JSONINDEX']._serialized_start=899
   _globals['_JSONINDEX']._serialized_end=977
-  _globals['_SEARCHABLEVARIABLEDEF']._serialized_start=979
-  _globals['_SEARCHABLEVARIABLEDEF']._serialized_end=1045
-  _globals['_THREADVARDEF']._serialized_start=1048
-  _globals['_THREADVARDEF']._serialized_end=1250
-  _globals['_THREADSPEC']._serialized_start=1253
-  _globals['_THREADSPEC']._serialized_end=1570
-  _globals['_THREADSPEC_NODESENTRY']._serialized_start=1486
-  _globals['_THREADSPEC_NODESENTRY']._serialized_end=1549
-  _globals['_THREADRETENTIONPOLICY']._serialized_start=1572
-  _globals['_THREADRETENTIONPOLICY']._serialized_end=1659
-  _globals['_INTERRUPTDEF']._serialized_start=1661
-  _globals['_INTERRUPTDEF']._serialized_end=1766
-  _globals['_STARTTHREADNODE']._serialized_start=1769
-  _globals['_STARTTHREADNODE']._serialized_end=1959
-  _globals['_STARTTHREADNODE_VARIABLESENTRY']._serialized_start=1878
-  _globals['_STARTTHREADNODE_VARIABLESENTRY']._serialized_end=1959
-  _globals['_STARTMULTIPLETHREADSNODE']._serialized_start=1962
-  _globals['_STARTMULTIPLETHREADSNODE']._serialized_end=2221
-  _globals['_STARTMULTIPLETHREADSNODE_VARIABLESENTRY']._serialized_start=1878
-  _globals['_STARTMULTIPLETHREADSNODE_VARIABLESENTRY']._serialized_end=1959
-  _globals['_FAILUREHANDLERDEF']._serialized_start=2224
-  _globals['_FAILUREHANDLERDEF']._serialized_end=2464
-  _globals['_FAILUREHANDLERDEF_LHFAILURETYPE']._serialized_start=2377
-  _globals['_FAILUREHANDLERDEF_LHFAILURETYPE']._serialized_end=2444
-  _globals['_WAITFORTHREADSNODE']._serialized_start=2467
-  _globals['_WAITFORTHREADSNODE']._serialized_end=2869
-  _globals['_WAITFORTHREADSNODE_THREADTOWAITFOR']._serialized_start=2683
-  _globals['_WAITFORTHREADSNODE_THREADTOWAITFOR']._serialized_end=2760
-  _globals['_WAITFORTHREADSNODE_THREADSTOWAITFOR']._serialized_start=2762
-  _globals['_WAITFORTHREADSNODE_THREADSTOWAITFOR']._serialized_end=2846
-  _globals['_EXTERNALEVENTNODE']._serialized_start=2872
-  _globals['_EXTERNALEVENTNODE']._serialized_end=3013
-  _globals['_ENTRYPOINTNODE']._serialized_start=3015
-  _globals['_ENTRYPOINTNODE']._serialized_end=3031
-  _globals['_EXITNODE']._serialized_start=3033
-  _globals['_EXITNODE']._serialized_end=3110
-  _globals['_FAILUREDEF']._serialized_start=3112
-  _globals['_FAILUREDEF']._serialized_end=3230
-  _globals['_NODE']._serialized_start=3233
-  _globals['_NODE']._serialized_end=3901
-  _globals['_THROWEVENTNODE']._serialized_start=3903
-  _globals['_THROWEVENTNODE']._serialized_end=4024
-  _globals['_USERTASKNODE']._serialized_start=4027
-  _globals['_USERTASKNODE']._serialized_end=4381
-  _globals['_EDGECONDITION']._serialized_start=4384
-  _globals['_EDGECONDITION']._serialized_end=4539
-  _globals['_EDGE']._serialized_start=4542
-  _globals['_EDGE']._serialized_end=4697
-  _globals['_NOPNODE']._serialized_start=4699
-  _globals['_NOPNODE']._serialized_end=4708
-  _globals['_SLEEPNODE']._serialized_start=4711
-  _globals['_SLEEPNODE']._serialized_end=4901
-  _globals['_WFSPECVERSIONMIGRATION']._serialized_start=4904
-  _globals['_WFSPECVERSIONMIGRATION']._serialized_end=5167
-  _globals['_WFSPECVERSIONMIGRATION_THREADSPECMIGRATIONSENTRY']._serialized_start=5074
-  _globals['_WFSPECVERSIONMIGRATION_THREADSPECMIGRATIONSENTRY']._serialized_end=5167
-  _globals['_THREADSPECMIGRATION']._serialized_start=5170
-  _globals['_THREADSPECMIGRATION']._serialized_end=5383
-  _globals['_THREADSPECMIGRATION_NODEMIGRATIONSENTRY']._serialized_start=5302
-  _globals['_THREADSPECMIGRATION_NODEMIGRATIONSENTRY']._serialized_end=5383
-  _globals['_NODEMIGRATION']._serialized_start=5385
-  _globals['_NODEMIGRATION']._serialized_end=5423
+  _globals['_THREADVARDEF']._serialized_start=980
+  _globals['_THREADVARDEF']._serialized_end=1182
+  _globals['_THREADSPEC']._serialized_start=1185
+  _globals['_THREADSPEC']._serialized_end=1502
+  _globals['_THREADSPEC_NODESENTRY']._serialized_start=1418
+  _globals['_THREADSPEC_NODESENTRY']._serialized_end=1481
+  _globals['_THREADRETENTIONPOLICY']._serialized_start=1504
+  _globals['_THREADRETENTIONPOLICY']._serialized_end=1591
+  _globals['_INTERRUPTDEF']._serialized_start=1593
+  _globals['_INTERRUPTDEF']._serialized_end=1698
+  _globals['_STARTTHREADNODE']._serialized_start=1701
+  _globals['_STARTTHREADNODE']._serialized_end=1891
+  _globals['_STARTTHREADNODE_VARIABLESENTRY']._serialized_start=1810
+  _globals['_STARTTHREADNODE_VARIABLESENTRY']._serialized_end=1891
+  _globals['_STARTMULTIPLETHREADSNODE']._serialized_start=1894
+  _globals['_STARTMULTIPLETHREADSNODE']._serialized_end=2153
+  _globals['_STARTMULTIPLETHREADSNODE_VARIABLESENTRY']._serialized_start=1810
+  _globals['_STARTMULTIPLETHREADSNODE_VARIABLESENTRY']._serialized_end=1891
+  _globals['_FAILUREHANDLERDEF']._serialized_start=2156
+  _globals['_FAILUREHANDLERDEF']._serialized_end=2396
+  _globals['_FAILUREHANDLERDEF_LHFAILURETYPE']._serialized_start=2309
+  _globals['_FAILUREHANDLERDEF_LHFAILURETYPE']._serialized_end=2376
+  _globals['_WAITFORTHREADSNODE']._serialized_start=2399
+  _globals['_WAITFORTHREADSNODE']._serialized_end=2801
+  _globals['_WAITFORTHREADSNODE_THREADTOWAITFOR']._serialized_start=2615
+  _globals['_WAITFORTHREADSNODE_THREADTOWAITFOR']._serialized_end=2692
+  _globals['_WAITFORTHREADSNODE_THREADSTOWAITFOR']._serialized_start=2694
+  _globals['_WAITFORTHREADSNODE_THREADSTOWAITFOR']._serialized_end=2778
+  _globals['_EXTERNALEVENTNODE']._serialized_start=2804
+  _globals['_EXTERNALEVENTNODE']._serialized_end=2945
+  _globals['_ENTRYPOINTNODE']._serialized_start=2947
+  _globals['_ENTRYPOINTNODE']._serialized_end=2963
+  _globals['_EXITNODE']._serialized_start=2965
+  _globals['_EXITNODE']._serialized_end=3042
+  _globals['_FAILUREDEF']._serialized_start=3044
+  _globals['_FAILUREDEF']._serialized_end=3162
+  _globals['_NODE']._serialized_start=3165
+  _globals['_NODE']._serialized_end=3833
+  _globals['_THROWEVENTNODE']._serialized_start=3835
+  _globals['_THROWEVENTNODE']._serialized_end=3956
+  _globals['_USERTASKNODE']._serialized_start=3959
+  _globals['_USERTASKNODE']._serialized_end=4426
+  _globals['_EDGECONDITION']._serialized_start=4429
+  _globals['_EDGECONDITION']._serialized_end=4584
+  _globals['_EDGE']._serialized_start=4587
+  _globals['_EDGE']._serialized_end=4742
+  _globals['_NOPNODE']._serialized_start=4744
+  _globals['_NOPNODE']._serialized_end=4753
+  _globals['_SLEEPNODE']._serialized_start=4756
+  _globals['_SLEEPNODE']._serialized_end=4946
+  _globals['_WFSPECVERSIONMIGRATION']._serialized_start=4949
+  _globals['_WFSPECVERSIONMIGRATION']._serialized_end=5212
+  _globals['_WFSPECVERSIONMIGRATION_THREADSPECMIGRATIONSENTRY']._serialized_start=5119
+  _globals['_WFSPECVERSIONMIGRATION_THREADSPECMIGRATIONSENTRY']._serialized_end=5212
+  _globals['_THREADSPECMIGRATION']._serialized_start=5215
+  _globals['_THREADSPECMIGRATION']._serialized_end=5428
+  _globals['_THREADSPECMIGRATION_NODEMIGRATIONSENTRY']._serialized_start=5347
+  _globals['_THREADSPECMIGRATION_NODEMIGRATIONSENTRY']._serialized_end=5428
+  _globals['_NODEMIGRATION']._serialized_start=5430
+  _globals['_NODEMIGRATION']._serialized_end=5468
 # @@protoc_insertion_point(module_scope)
```

### Comparing `littlehorse_client-0.8.1/littlehorse/model/wf_spec_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/wf_spec_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -65,20 +65,14 @@
     __slots__ = ["field_path", "field_type"]
     FIELD_PATH_FIELD_NUMBER: _ClassVar[int]
     FIELD_TYPE_FIELD_NUMBER: _ClassVar[int]
     field_path: str
     field_type: _common_enums_pb2.VariableType
     def __init__(self, field_path: _Optional[str] = ..., field_type: _Optional[_Union[_common_enums_pb2.VariableType, str]] = ...) -> None: ...
 
-class SearchableVariableDef(_message.Message):
-    __slots__ = ["var_def"]
-    VAR_DEF_FIELD_NUMBER: _ClassVar[int]
-    var_def: _common_wfspec_pb2.VariableDef
-    def __init__(self, var_def: _Optional[_Union[_common_wfspec_pb2.VariableDef, _Mapping]] = ...) -> None: ...
-
 class ThreadVarDef(_message.Message):
     __slots__ = ["var_def", "required", "searchable", "json_indexes", "access_level"]
     VAR_DEF_FIELD_NUMBER: _ClassVar[int]
     REQUIRED_FIELD_NUMBER: _ClassVar[int]
     SEARCHABLE_FIELD_NUMBER: _ClassVar[int]
     JSON_INDEXES_FIELD_NUMBER: _ClassVar[int]
     ACCESS_LEVEL_FIELD_NUMBER: _ClassVar[int]
@@ -253,28 +247,30 @@
     EVENT_DEF_ID_FIELD_NUMBER: _ClassVar[int]
     CONTENT_FIELD_NUMBER: _ClassVar[int]
     event_def_id: _object_id_pb2.WorkflowEventDefId
     content: _common_wfspec_pb2.VariableAssignment
     def __init__(self, event_def_id: _Optional[_Union[_object_id_pb2.WorkflowEventDefId, _Mapping]] = ..., content: _Optional[_Union[_common_wfspec_pb2.VariableAssignment, _Mapping]] = ...) -> None: ...
 
 class UserTaskNode(_message.Message):
-    __slots__ = ["user_task_def_name", "user_group", "user_id", "actions", "user_task_def_version", "notes"]
+    __slots__ = ["user_task_def_name", "user_group", "user_id", "actions", "user_task_def_version", "notes", "on_cancellation_exception_name"]
     USER_TASK_DEF_NAME_FIELD_NUMBER: _ClassVar[int]
     USER_GROUP_FIELD_NUMBER: _ClassVar[int]
     USER_ID_FIELD_NUMBER: _ClassVar[int]
     ACTIONS_FIELD_NUMBER: _ClassVar[int]
     USER_TASK_DEF_VERSION_FIELD_NUMBER: _ClassVar[int]
     NOTES_FIELD_NUMBER: _ClassVar[int]
+    ON_CANCELLATION_EXCEPTION_NAME_FIELD_NUMBER: _ClassVar[int]
     user_task_def_name: str
     user_group: _common_wfspec_pb2.VariableAssignment
     user_id: _common_wfspec_pb2.VariableAssignment
     actions: _containers.RepeatedCompositeFieldContainer[_common_wfspec_pb2.UTActionTrigger]
     user_task_def_version: int
     notes: _common_wfspec_pb2.VariableAssignment
-    def __init__(self, user_task_def_name: _Optional[str] = ..., user_group: _Optional[_Union[_common_wfspec_pb2.VariableAssignment, _Mapping]] = ..., user_id: _Optional[_Union[_common_wfspec_pb2.VariableAssignment, _Mapping]] = ..., actions: _Optional[_Iterable[_Union[_common_wfspec_pb2.UTActionTrigger, _Mapping]]] = ..., user_task_def_version: _Optional[int] = ..., notes: _Optional[_Union[_common_wfspec_pb2.VariableAssignment, _Mapping]] = ...) -> None: ...
+    on_cancellation_exception_name: _common_wfspec_pb2.VariableAssignment
+    def __init__(self, user_task_def_name: _Optional[str] = ..., user_group: _Optional[_Union[_common_wfspec_pb2.VariableAssignment, _Mapping]] = ..., user_id: _Optional[_Union[_common_wfspec_pb2.VariableAssignment, _Mapping]] = ..., actions: _Optional[_Iterable[_Union[_common_wfspec_pb2.UTActionTrigger, _Mapping]]] = ..., user_task_def_version: _Optional[int] = ..., notes: _Optional[_Union[_common_wfspec_pb2.VariableAssignment, _Mapping]] = ..., on_cancellation_exception_name: _Optional[_Union[_common_wfspec_pb2.VariableAssignment, _Mapping]] = ...) -> None: ...
 
 class EdgeCondition(_message.Message):
     __slots__ = ["comparator", "left", "right"]
     COMPARATOR_FIELD_NUMBER: _ClassVar[int]
     LEFT_FIELD_NUMBER: _ClassVar[int]
     RIGHT_FIELD_NUMBER: _ClassVar[int]
     comparator: _common_wfspec_pb2.Comparator
```

### Comparing `littlehorse_client-0.8.1/littlehorse/model/workflow_event_pb2.py` & `littlehorse_client-0.9.0/littlehorse/model/workflow_event_pb2.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/model/workflow_event_pb2.pyi` & `littlehorse_client-0.9.0/littlehorse/model/workflow_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/utils.py` & `littlehorse_client-0.9.0/littlehorse/utils.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/worker.py` & `littlehorse_client-0.9.0/littlehorse/worker.py`

 * *Files identical despite different names*

### Comparing `littlehorse_client-0.8.1/littlehorse/workflow.py` & `littlehorse_client-0.9.0/littlehorse/workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -664,36 +664,73 @@
     def __init__(
         self,
         node_name: str,
         thread: "WorkflowThread",
         user_task_def_name: str,
         user_id: Optional[Union[str, WfRunVariable]] = None,
         user_group: Optional[Union[str, WfRunVariable]] = None,
+        notes: Optional[Union[str, WfRunVariable, LHFormatString]] = None,
+        on_cancellation_exception_name: Optional[Union[str, WfRunVariable]] = None,
     ) -> None:
         super().__init__(node_name)
         self._thread = thread
         self._node_name = node_name
         self._user_task_def_name = user_task_def_name
         self._user_group = user_group
         self._user_id = user_id
+        self._notes = notes
+        self._on_cancellation_exception_name = on_cancellation_exception_name
 
     def with_notes(
         self, notes: Union[str, WfRunVariable, LHFormatString]
     ) -> "UserTaskOutput":
         node = self._thread._last_node()
         if node.name != self._node_name:
             raise ValueError("tried to mutate stale UserTaskOutput!")
 
         ug = to_variable_assignment(self._user_group) if self._user_group else None
         ui = to_variable_assignment(self._user_id) if self._user_id else None
+        if self._on_cancellation_exception_name:
+            exception_name = to_variable_assignment(
+                self._on_cancellation_exception_name
+            )
+        else:
+            exception_name = None
+
         ut_node = UserTaskNode(
             user_task_def_name=self._user_task_def_name,
             user_group=ug,
             user_id=ui,
             notes=to_variable_assignment(notes),
+            on_cancellation_exception_name=exception_name,
+        )
+        self._notes = notes
+
+        node.sub_node = ut_node
+        return self
+
+    def with_on_cancellation_exception(
+        self, exception_name: Union[str, WfRunVariable]
+    ) -> "UserTaskOutput":
+        node = self._thread._last_node()
+        if node.name != self._node_name:
+            raise ValueError("tried to mutate stale UserTaskOutput!")
+
+        ug = to_variable_assignment(self._user_group) if self._user_group else None
+        ui = to_variable_assignment(self._user_id) if self._user_id else None
+        if self._notes:
+            notes = to_variable_assignment(self._notes)
+        else:
+            notes = None
+        ut_node = UserTaskNode(
+            user_task_def_name=self._user_task_def_name,
+            user_group=ug,
+            user_id=ui,
+            notes=notes,
+            on_cancellation_exception_name=to_variable_assignment(exception_name),
         )
 
         node.sub_node = ut_node
         return self
 
 
 class WorkflowThread:
@@ -1276,14 +1313,15 @@
             raise ValueError("Cannot release node to group if user_group is None")
         if ut_node.user_id is None:
             raise ValueError("Cannot release node to group if user_id is none")
 
         trigger: UTActionTrigger = UTActionTrigger(
             reassign=UTActionTrigger.UTAReassign(user_group=ut_node.user_group),
             delay_seconds=to_variable_assignment(deadline_seconds),
+            hook=UTActionTrigger.UTHook.ON_TASK_ASSIGNED,
         )
         ut_node.actions.append(trigger)
 
     def schedule_reminder_task(
         self,
         user_task: UserTaskOutput,
         delay_in_seconds: Union[int, WfRunVariable],
@@ -1635,14 +1673,62 @@
 
     def _collect_variable_mutations(self) -> list[VariableMutation]:
         variables_from_if_block = []
         while len(self._variable_mutations) > 0:
             variables_from_if_block.append(self._variable_mutations.popleft())
         return variables_from_if_block
 
+    def cancel_user_task_run_after(
+        self, user_task: UserTaskOutput, delay_in_seconds: Union[int, WfRunVariable]
+    ) -> None:
+        """
+        Cancels a User Task Run if it exceeds a specified deadline.
+        Args:
+            user_task: reference to the UserTaskNode that will be canceled after the deadline.
+            delay_in_seconds: delay time after which the User Task Run should be canceled.
+        """
+        self._check_if_active()
+        self._schedule_user_task_cancellation_after(
+            user_task, delay_in_seconds, UTActionTrigger.UTHook.ON_ARRIVAL
+        )
+
+    def cancel_user_task_run_after_assignment(
+        self, user_task: UserTaskOutput, delay_in_seconds: Union[int, WfRunVariable]
+    ) -> None:
+        """
+        Cancels a User Task Run if it exceeds a specified deadline after it is assigned.
+        Args:
+            user_task: reference to the UserTaskNode that will be canceled after the deadline.
+            delay_in_seconds: delay time after which the User Task Run should be canceled.
+        """
+        self._check_if_active()
+        self._schedule_user_task_cancellation_after(
+            user_task, delay_in_seconds, UTActionTrigger.UTHook.ON_TASK_ASSIGNED
+        )
+
+    def _schedule_user_task_cancellation_after(
+        self,
+        user_task: UserTaskOutput,
+        delay_in_seconds: Union[int, WfRunVariable],
+        hook: UTActionTrigger.UTHook,
+    ) -> None:
+        if self._last_node().name != user_task.node_name:
+            raise ValueError("Tried to reassign stale user task node!")
+
+        cancel = UTActionTrigger.UTACancel()
+
+        ut_node: UserTaskNode = typing.cast(UserTaskNode, self._last_node().sub_node)
+        ut_node.actions.append(
+            UTActionTrigger(
+                cancel=cancel,
+                delay_seconds=to_variable_assignment(delay_in_seconds),
+                hook=hook,
+            )
+        )
+
 
 ThreadInitializer = Callable[[WorkflowThread], None]
 
 
 class Workflow:
     def __init__(
         self,
```

### Comparing `littlehorse_client-0.8.1/pyproject.toml` & `littlehorse_client-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "littlehorse-client"
-version = "0.8.1"
+version = "0.9.0"
 description = "LittleHorse is a high-performance microservice orchestration engine that allows developers to build scalable, maintainable, and observable applications"
 authors = [ "LittleHorse Engineering <engineering@littlehorse.io>",]
 readme = "README.md"
 license = "SSPL-1.0"
 homepage = "https://littlehorse.dev"
 repository = "https://github.com/littlehorse-enterprises/littlehorse"
 documentation = "https://littlehorse.dev/docs/Overview"
```

### Comparing `littlehorse_client-0.8.1/PKG-INFO` & `littlehorse_client-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: littlehorse-client
-Version: 0.8.1
+Version: 0.9.0
 Summary: LittleHorse is a high-performance microservice orchestration engine that allows developers to build scalable, maintainable, and observable applications
 Home-page: https://littlehorse.dev
 License: SSPL-1.0
 Keywords: littlehorse
 Author: LittleHorse Engineering
 Author-email: engineering@littlehorse.io
 Requires-Python: >=3.9,<3.13
```

