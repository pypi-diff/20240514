# Comparing `tmp/fabric_cf-1.6.2.tar.gz` & `tmp/fabric_cf-1.6.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_cf-1.6.2.tar", last modified: Mon Feb 26 14:42:08 2024, max compression
+gzip compressed data, was "fabric_cf-1.6.2rc0.tar", last modified: Sat Feb 24 02:48:01 2024, max compression
```

## Comparing `fabric_cf-1.6.2.tar` & `fabric_cf-1.6.2rc0.tar`

### file list

```diff
@@ -1,526 +1,526 @@
--rw-r--r--   0        0        0     2035 2023-07-06 14:40:19.903102 fabric_cf-1.6.2/.gitignore
--rw-r--r--   0        0        0      851 2024-02-24 02:42:05.148233 fabric_cf-1.6.2/Dockerfile-auth
--rw-r--r--   0        0        0      771 2024-01-22 16:38:27.605442 fabric_cf-1.6.2/Dockerfile-broker
--rw-r--r--   0        0        0     1041 2024-01-22 16:38:27.606382 fabric_cf-1.6.2/Dockerfile-cf
--rw-r--r--   0        0        0      789 2024-01-22 16:38:27.607632 fabric_cf-1.6.2/Dockerfile-orchestrator
--rw-r--r--   0        0        0     1071 2023-07-06 14:40:19.903692 fabric_cf-1.6.2/LICENSE
--rw-r--r--   0        0        0     2046 2023-07-06 14:40:19.903887 fabric_cf-1.6.2/README.md
--rwxr-xr-x   0        0        0       74 2023-07-06 14:40:19.904024 fabric_cf-1.6.2/authority.sh
--rwxr-xr-x   0        0        0       79 2023-07-06 14:40:19.904125 fabric_cf-1.6.2/broker.sh
--rw-r--r--   0        0        0      947 2023-07-06 14:40:19.904225 fabric_cf-1.6.2/cleanup_old_schema_from_schema_registry.sh
--rw-r--r--   0        0        0     2861 2023-07-06 14:40:19.904409 fabric_cf-1.6.2/docker-compose-kafka.yaml
--rw-r--r--   0        0        0     1560 2023-07-06 14:40:19.904579 fabric_cf-1.6.2/docker-compose-no-ssl-kafka.yaml
--rw-r--r--   0        0        0    10307 2024-01-22 16:38:27.610519 fabric_cf-1.6.2/docker-compose-test.yaml
--rwxr-xr-x   0        0        0       46 2024-01-22 16:38:27.611401 fabric_cf-1.6.2/docker-entrypoint.sh
--rw-r--r--   0        0        0      350 2023-07-06 14:40:19.904923 fabric_cf-1.6.2/env.template
--rw-r--r--   0        0        0     1135 2023-07-06 14:40:19.905192 fabric_cf-1.6.2/env.template.test
--rw-r--r--   0        0        0    16609 2023-07-06 14:40:19.905386 fabric_cf-1.6.2/fabricNo.AnyActorNoPolicy.xml
--rw-r--r--   0        0        0     6343 2023-07-06 14:40:19.905685 fabric_cf-1.6.2/fabric_cf/Design.md
--rw-r--r--   0        0        0       48 2024-02-26 14:42:01.359826 fabric_cf-1.6.2/fabric_cf/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.905895 fabric_cf-1.6.2/fabric_cf/actor/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.905999 fabric_cf-1.6.2/fabric_cf/actor/boot/__init__.py
--rw-r--r--   0        0        0    15904 2024-02-15 17:39:56.133953 fabric_cf-1.6.2/fabric_cf/actor/boot/configuration.py
--rw-r--r--   0        0        0     1268 2023-07-06 14:40:19.906660 fabric_cf-1.6.2/fabric_cf/actor/boot/configuration_exception.py
--rw-r--r--   0        0        0     2509 2023-07-06 14:40:19.907136 fabric_cf-1.6.2/fabric_cf/actor/boot/configuration_loader.py
--rw-r--r--   0        0        0    23003 2023-07-06 14:40:19.907477 fabric_cf-1.6.2/fabric_cf/actor/boot/configuration_processor.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.907709 fabric_cf-1.6.2/fabric_cf/actor/boot/inventory/__init__.py
--rw-r--r--   0        0        0     4969 2023-07-06 14:40:19.907981 fabric_cf-1.6.2/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.908142 fabric_cf-1.6.2/fabric_cf/actor/core/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.908303 fabric_cf-1.6.2/fabric_cf/actor/core/apis/__init__.py
--rw-r--r--   0        0        0     4907 2023-07-06 14:40:19.908566 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_container.py
--rw-r--r--   0        0        0     1530 2023-07-06 14:40:19.908811 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_event.py
--rw-r--r--   0        0        0     2176 2023-07-06 14:40:19.909045 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_identity.py
--rw-r--r--   0        0        0    11057 2024-02-15 17:39:56.134395 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_management_object.py
--rw-r--r--   0        0        0    22153 2024-02-15 17:39:56.135663 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_mixin.py
--rw-r--r--   0        0        0     1918 2023-07-06 14:40:19.910056 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_proxy.py
--rw-r--r--   0        0        0     1323 2023-07-06 14:40:19.910353 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_runnable.py
--rw-r--r--   0        0        0     4749 2024-01-22 16:38:27.617796 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_authority.py
--rw-r--r--   0        0        0     8736 2023-07-06 14:40:19.910801 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_authority_policy.py
--rw-r--r--   0        0        0     3657 2023-07-06 14:40:19.911078 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_authority_proxy.py
--rw-r--r--   0        0        0     3367 2023-07-06 14:40:19.912325 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_authority_reservation.py
--rw-r--r--   0        0        0     6071 2023-07-06 14:40:19.912747 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_base_plugin.py
--rw-r--r--   0        0        0     2290 2023-07-06 14:40:19.913005 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_broker_mixin.py
--rw-r--r--   0        0        0     1492 2023-07-06 14:40:19.913272 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py
--rw-r--r--   0        0        0     3690 2023-07-06 14:40:19.913487 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_broker_proxy.py
--rw-r--r--   0        0        0     4012 2023-07-06 14:40:19.913729 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_broker_reservation.py
--rw-r--r--   0        0        0     2442 2023-07-06 14:40:19.913939 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_callback_proxy.py
--rw-r--r--   0        0        0     9846 2023-07-06 14:40:19.914206 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_client_actor.py
--rw-r--r--   0        0        0     6811 2023-07-06 14:40:19.914611 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_client_actor_management_object.py
--rw-r--r--   0        0        0     2640 2023-07-06 14:40:19.914862 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_client_callback_proxy.py
--rw-r--r--   0        0        0     5802 2023-07-06 14:40:19.915112 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_client_policy.py
--rw-r--r--   0        0        0     7724 2023-07-06 14:40:19.915445 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_client_reservation.py
--rw-r--r--   0        0        0     1936 2023-07-06 14:40:19.915721 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_component.py
--rw-r--r--   0        0        0    10115 2023-07-06 14:40:19.915929 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_concrete_set.py
--rw-r--r--   0        0        0     2729 2023-07-06 14:40:19.916612 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_container_clock.py
--rw-r--r--   0        0        0     3976 2023-07-06 14:40:19.917089 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_container_database.py
--rw-r--r--   0        0        0     3367 2023-07-06 14:40:19.917325 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_controller.py
--rw-r--r--   0        0        0     2855 2023-07-06 14:40:19.917527 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py
--rw-r--r--   0        0        0     2787 2023-07-06 14:40:19.917690 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_controller_policy.py
--rw-r--r--   0        0        0     5713 2023-07-06 14:40:19.917899 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_controller_reservation.py
--rw-r--r--   0        0        0    12064 2024-02-15 17:39:56.136629 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_database.py
--rw-r--r--   0        0        0    11127 2023-07-06 14:40:19.918323 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_delegation.py
--rw-r--r--   0        0        0     1867 2023-07-06 14:40:19.918509 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_event.py
--rw-r--r--   0        0        0     1943 2023-07-06 14:40:19.918929 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_management_object.py
--rw-r--r--   0        0        0    10150 2024-02-15 17:39:56.137005 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_actor.py
--rw-r--r--   0        0        0     2534 2023-07-06 14:40:19.919334 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_authority.py
--rw-r--r--   0        0        0     1452 2023-07-06 14:40:19.919514 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py
--rw-r--r--   0        0        0     6191 2023-07-06 14:40:19.919720 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py
--rw-r--r--   0        0        0     5041 2023-07-06 14:40:19.919903 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_container.py
--rw-r--r--   0        0        0     2486 2023-07-06 14:40:19.920096 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py
--rw-r--r--   0        0        0     5014 2023-07-06 14:40:19.920347 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py
--rw-r--r--   0        0        0    11147 2023-07-06 14:40:19.920532 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_policy.py
--rw-r--r--   0        0        0     2304 2023-07-06 14:40:19.920723 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_proxy.py
--rw-r--r--   0        0        0     2290 2023-07-06 14:40:19.920941 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_proxy_factory.py
--rw-r--r--   0        0        0     1658 2023-07-06 14:40:19.921528 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_query_response_handler.py
--rw-r--r--   0        0        0    14642 2024-02-15 17:39:56.138505 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_reservation_mixin.py
--rw-r--r--   0        0        0     9388 2023-07-06 14:40:19.922320 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_reservation_resources.py
--rw-r--r--   0        0        0     5581 2023-07-06 14:40:19.922552 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_reservation_status.py
--rw-r--r--   0        0        0     8963 2023-07-06 14:40:19.922838 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_resource_control.py
--rw-r--r--   0        0        0     1336 2023-07-06 14:40:19.923076 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_response_handler.py
--rw-r--r--   0        0        0     2246 2023-07-06 14:40:19.923329 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_rpc_request_state.py
--rw-r--r--   0        0        0     5634 2023-07-06 14:40:19.923525 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_server_actor.py
--rw-r--r--   0        0        0     6415 2023-07-06 14:40:19.923729 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_server_policy.py
--rw-r--r--   0        0        0     4846 2023-07-06 14:40:19.923935 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_server_reservation.py
--rw-r--r--   0        0        0    13280 2023-07-06 14:40:19.924255 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_slice.py
--rw-r--r--   0        0        0     3548 2023-07-06 14:40:19.924544 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_substrate.py
--rw-r--r--   0        0        0     2225 2023-07-06 14:40:19.924790 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_substrate_database.py
--rw-r--r--   0        0        0     2943 2023-07-06 14:40:19.925003 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_tick.py
--rw-r--r--   0        0        0     6121 2023-07-06 14:40:19.925195 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_ticker.py
--rw-r--r--   0        0        0     1590 2023-07-06 14:40:19.925375 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_timer_queue.py
--rw-r--r--   0        0        0     1387 2023-07-06 14:40:19.925617 fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_timer_task.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.925835 fabric_cf-1.6.2/fabric_cf/actor/core/common/__init__.py
--rw-r--r--   0        0        0    13545 2024-02-19 14:44:58.093768 fabric_cf-1.6.2/fabric_cf/actor/core/common/constants.py
--rw-r--r--   0        0        0     5894 2024-01-22 16:38:27.622996 fabric_cf-1.6.2/fabric_cf/actor/core/common/event_logger.py
--rw-r--r--   0        0        0     5517 2023-07-06 14:40:19.926617 fabric_cf-1.6.2/fabric_cf/actor/core/common/exceptions.py
--rw-r--r--   0        0        0     6108 2023-07-06 14:40:19.926828 fabric_cf-1.6.2/fabric_cf/actor/core/common/resource_config.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.927014 fabric_cf-1.6.2/fabric_cf/actor/core/container/__init__.py
--rw-r--r--   0        0        0    24564 2024-02-05 19:10:51.724345 fabric_cf-1.6.2/fabric_cf/actor/core/container/container.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.927724 fabric_cf-1.6.2/fabric_cf/actor/core/container/db/__init__.py
--rw-r--r--   0        0        0     8667 2023-07-06 14:40:19.928046 fabric_cf-1.6.2/fabric_cf/actor/core/container/db/container_database.py
--rw-r--r--   0        0        0    22315 2024-02-15 17:39:56.139869 fabric_cf-1.6.2/fabric_cf/actor/core/container/globals.py
--rw-r--r--   0        0        0     9407 2023-12-01 02:09:02.681115 fabric_cf-1.6.2/fabric_cf/actor/core/container/maintenance.py
--rw-r--r--   0        0        0     4284 2024-02-15 17:39:56.140477 fabric_cf-1.6.2/fabric_cf/actor/core/container/message_service.py
--rw-r--r--   0        0        0     1508 2023-07-06 14:40:19.929116 fabric_cf-1.6.2/fabric_cf/actor/core/container/protocol_descriptor.py
--rw-r--r--   0        0        0    13005 2023-07-06 14:40:19.929611 fabric_cf-1.6.2/fabric_cf/actor/core/container/remote_actor_cache.py
--rw-r--r--   0        0        0     7320 2024-02-15 17:39:56.140947 fabric_cf-1.6.2/fabric_cf/actor/core/container/rpc_consumer.py
--rw-r--r--   0        0        0     8437 2024-02-15 17:39:56.141308 fabric_cf-1.6.2/fabric_cf/actor/core/container/rpc_producer.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.930049 fabric_cf-1.6.2/fabric_cf/actor/core/core/__init__.py
--rw-r--r--   0        0        0    36977 2024-02-15 17:39:56.142190 fabric_cf-1.6.2/fabric_cf/actor/core/core/actor.py
--rw-r--r--   0        0        0     1975 2023-07-06 14:40:19.930990 fabric_cf-1.6.2/fabric_cf/actor/core/core/actor_identity.py
--rw-r--r--   0        0        0    15515 2024-01-22 16:38:27.626136 fabric_cf-1.6.2/fabric_cf/actor/core/core/authority.py
--rw-r--r--   0        0        0     4845 2023-07-06 14:40:19.931698 fabric_cf-1.6.2/fabric_cf/actor/core/core/authority_policy.py
--rw-r--r--   0        0        0    20447 2023-07-06 14:40:19.932087 fabric_cf-1.6.2/fabric_cf/actor/core/core/broker.py
--rw-r--r--   0        0        0     5914 2023-07-06 14:40:19.933176 fabric_cf-1.6.2/fabric_cf/actor/core/core/broker_policy.py
--rw-r--r--   0        0        0    20424 2024-01-22 16:38:27.627154 fabric_cf-1.6.2/fabric_cf/actor/core/core/controller.py
--rw-r--r--   0        0        0     8631 2023-07-06 14:40:19.934048 fabric_cf-1.6.2/fabric_cf/actor/core/core/event_processor.py
--rw-r--r--   0        0        0     5467 2023-07-06 14:40:19.934289 fabric_cf-1.6.2/fabric_cf/actor/core/core/inventory_slice_manager.py
--rw-r--r--   0        0        0     6171 2023-07-06 14:40:19.934575 fabric_cf-1.6.2/fabric_cf/actor/core/core/policy.py
--rw-r--r--   0        0        0     2042 2023-07-06 14:40:19.934764 fabric_cf-1.6.2/fabric_cf/actor/core/core/rpc_request_state.py
--rw-r--r--   0        0        0     8688 2023-07-06 14:40:19.934985 fabric_cf-1.6.2/fabric_cf/actor/core/core/ticket.py
--rw-r--r--   0        0        0    16794 2024-01-22 16:38:27.628065 fabric_cf-1.6.2/fabric_cf/actor/core/core/unit.py
--rw-r--r--   0        0        0    13818 2024-01-22 16:38:27.629229 fabric_cf-1.6.2/fabric_cf/actor/core/core/unit_set.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.935644 fabric_cf-1.6.2/fabric_cf/actor/core/delegation/__init__.py
--rw-r--r--   0        0        0    11147 2024-02-15 17:39:56.142971 fabric_cf-1.6.2/fabric_cf/actor/core/delegation/broker_delegation.py
--rw-r--r--   0        0        0     1933 2023-07-06 14:40:19.936411 fabric_cf-1.6.2/fabric_cf/actor/core/delegation/broker_delegation_factory.py
--rw-r--r--   0        0        0    17061 2023-07-06 14:40:19.936650 fabric_cf-1.6.2/fabric_cf/actor/core/delegation/delegation.py
--rw-r--r--   0        0        0     1916 2023-07-06 14:40:19.936853 fabric_cf-1.6.2/fabric_cf/actor/core/delegation/delegation_factory.py
--rw-r--r--   0        0        0     5364 2023-07-06 14:40:19.937100 fabric_cf-1.6.2/fabric_cf/actor/core/delegation/resource_ticket.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.937314 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/__init__.py
--rw-r--r--   0        0        0    32557 2024-02-15 17:39:56.143738 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/authority_reservation.py
--rw-r--r--   0        0        0     3384 2023-07-06 14:40:19.938172 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/broker_query_model_publisher.py
--rw-r--r--   0        0        0    27849 2024-02-15 17:39:56.145093 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/broker_reservation.py
--rw-r--r--   0        0        0     2992 2023-07-06 14:40:19.938929 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/claim_timeout.py
--rw-r--r--   0        0        0     4396 2023-07-06 14:40:19.939229 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/failed_rpc.py
--rw-r--r--   0        0        0     3639 2023-07-06 14:40:19.939436 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/failed_rpc_event.py
--rw-r--r--   0        0        0     2668 2023-07-06 14:40:19.939773 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py
--rw-r--r--   0        0        0     2708 2023-07-06 14:40:19.940197 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_failed_rpc.py
--rw-r--r--   0        0        0     2274 2023-07-06 14:40:19.940545 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_poa_rpc.py
--rw-r--r--   0        0        0     2105 2023-07-06 14:40:19.940998 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_query_rpc.py
--rw-r--r--   0        0        0     2703 2023-07-06 14:40:19.941194 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py
--rw-r--r--   0        0        0     4158 2023-07-06 14:40:19.941400 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_rpc.py
--rw-r--r--   0        0        0    11227 2023-07-06 14:40:19.941668 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_rpc_event.py
--rw-r--r--   0        0        0    67404 2024-02-15 17:39:56.146021 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/kernel.py
--rw-r--r--   0        0        0     3314 2023-07-06 14:40:19.942401 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/kernel_tick.py
--rw-r--r--   0        0        0    58250 2024-02-15 17:39:56.146854 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/kernel_wrapper.py
--rw-r--r--   0        0        0    13520 2024-01-22 16:38:27.632286 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/poa.py
--rw-r--r--   0        0        0     2363 2023-07-06 14:40:19.943408 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/predecessor_state.py
--rw-r--r--   0        0        0     2860 2023-07-06 14:40:19.943609 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/query_timeout.py
--rw-r--r--   0        0        0     1404 2023-07-06 14:40:19.943902 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/request_types.py
--rw-r--r--   0        0        0    24768 2024-02-15 17:39:56.148232 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/reservation.py
--rw-r--r--   0        0        0    92379 2024-02-15 17:39:56.149732 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/reservation_client.py
--rw-r--r--   0        0        0     9994 2023-07-06 14:40:19.945164 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/reservation_server.py
--rw-r--r--   0        0        0     3451 2024-02-15 17:39:56.150884 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/reservation_states.py
--rw-r--r--   0        0        0    21131 2023-07-06 14:40:19.945902 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/resource_set.py
--rw-r--r--   0        0        0     1614 2023-07-06 14:40:19.946143 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/retry_rpc.py
--rw-r--r--   0        0        0     1899 2023-07-06 14:40:19.946405 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/retry_rpc_event.py
--rw-r--r--   0        0        0     4128 2023-07-06 14:40:19.946774 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/rpc_executor.py
--rw-r--r--   0        0        0    32934 2024-02-12 17:21:22.410231 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/rpc_manager.py
--rw-r--r--   0        0        0     1772 2023-07-06 14:40:19.947586 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/rpc_manager_singleton.py
--rw-r--r--   0        0        0     3793 2023-07-06 14:40:19.947812 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/rpc_request.py
--rw-r--r--   0        0        0     1650 2023-07-06 14:40:19.948108 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/rpc_request_type.py
--rw-r--r--   0        0        0     1340 2023-07-06 14:40:19.948369 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/sequence_comparison_codes.py
--rw-r--r--   0        0        0    12284 2023-07-06 14:40:19.948609 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/slice.py
--rw-r--r--   0        0        0    13487 2024-02-15 17:39:56.151880 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/slice_state_machine.py
--rw-r--r--   0        0        0     8319 2023-07-06 14:40:19.949044 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/slice_table.py
--rw-r--r--   0        0        0     6527 2023-07-06 14:40:19.949206 fabric_cf-1.6.2/fabric_cf/actor/core/kernel/tick.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.949376 fabric_cf-1.6.2/fabric_cf/actor/core/manage/__init__.py
--rw-r--r--   0        0        0    41298 2024-02-15 17:39:56.152901 fabric_cf-1.6.2/fabric_cf/actor/core/manage/actor_management_object.py
--rw-r--r--   0        0        0     8431 2023-07-06 14:40:19.950168 fabric_cf-1.6.2/fabric_cf/actor/core/manage/authority_management_object.py
--rw-r--r--   0        0        0     7315 2023-07-06 14:40:19.950425 fabric_cf-1.6.2/fabric_cf/actor/core/manage/broker_management_object.py
--rw-r--r--   0        0        0    29438 2023-07-06 14:40:19.950803 fabric_cf-1.6.2/fabric_cf/actor/core/manage/client_actor_management_object_helper.py
--rw-r--r--   0        0        0     9605 2023-07-06 14:40:19.951070 fabric_cf-1.6.2/fabric_cf/actor/core/manage/container_management_object.py
--rw-r--r--   0        0        0     9165 2023-07-06 14:40:19.951281 fabric_cf-1.6.2/fabric_cf/actor/core/manage/controller_management_object.py
--rw-r--r--   0        0        0    13007 2023-07-06 14:40:19.951532 fabric_cf-1.6.2/fabric_cf/actor/core/manage/converter.py
--rw-r--r--   0        0        0     1624 2023-07-06 14:40:19.951814 fabric_cf-1.6.2/fabric_cf/actor/core/manage/error.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.951987 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/__init__.py
--rw-r--r--   0        0        0    10686 2024-02-15 17:39:56.153449 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_actor.py
--rw-r--r--   0        0        0     3509 2023-07-06 14:40:19.952418 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_authority.py
--rw-r--r--   0        0        0     8200 2023-12-01 02:08:52.565147 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_broker.py
--rw-r--r--   0        0        0     4483 2023-07-06 14:40:19.952942 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_container.py
--rw-r--r--   0        0        0     5462 2023-07-06 14:40:19.953162 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_controller.py
--rw-r--r--   0        0        0     5462 2023-07-06 14:40:19.953389 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py
--rw-r--r--   0        0        0     6960 2023-07-06 14:40:19.953595 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_proxy.py
--rw-r--r--   0        0        0     5730 2023-07-06 14:40:19.953784 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.954011 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/__init__.py
--rw-r--r--   0        0        0    24550 2023-07-06 14:40:19.954465 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py
--rw-r--r--   0        0        0     5715 2023-07-06 14:40:19.954804 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py
--rw-r--r--   0        0        0     5797 2023-07-06 14:40:19.955203 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py
--rw-r--r--   0        0        0    15846 2023-09-15 17:58:20.250112 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py
--rw-r--r--   0        0        0     4008 2023-07-06 14:40:19.955727 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py
--rw-r--r--   0        0        0     8228 2023-07-06 14:40:19.956009 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py
--rw-r--r--   0        0        0     2136 2024-02-15 17:39:56.153820 fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_service.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.956509 fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/__init__.py
--rw-r--r--   0        0        0    12259 2024-02-15 17:39:56.154238 fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_actor.py
--rw-r--r--   0        0        0     3902 2023-07-06 14:40:19.956881 fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_authority.py
--rw-r--r--   0        0        0     8391 2023-07-06 14:40:19.957075 fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_broker.py
--rw-r--r--   0        0        0    10119 2023-07-06 14:40:19.957225 fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_container.py
--rw-r--r--   0        0        0     9646 2023-07-06 14:40:19.957405 fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_controller.py
--rw-r--r--   0        0        0     2954 2023-07-06 14:40:19.957574 fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_proxy.py
--rw-r--r--   0        0        0     8655 2023-07-06 14:40:19.957761 fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_server_actor.py
--rw-r--r--   0        0        0     7217 2023-07-06 14:40:19.958014 fabric_cf-1.6.2/fabric_cf/actor/core/manage/management_object.py
--rw-r--r--   0        0        0     7841 2023-07-06 14:40:19.958239 fabric_cf-1.6.2/fabric_cf/actor/core/manage/management_object_manager.py
--rw-r--r--   0        0        0     4972 2023-07-06 14:40:19.958443 fabric_cf-1.6.2/fabric_cf/actor/core/manage/management_utils.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.958621 fabric_cf-1.6.2/fabric_cf/actor/core/manage/messages/__init__.py
--rw-r--r--   0        0        0     1604 2023-07-06 14:40:19.958823 fabric_cf-1.6.2/fabric_cf/actor/core/manage/messages/client_mng.py
--rw-r--r--   0        0        0     1570 2023-07-06 14:40:19.958990 fabric_cf-1.6.2/fabric_cf/actor/core/manage/messages/event_mng.py
--rw-r--r--   0        0        0     1802 2023-07-06 14:40:19.959148 fabric_cf-1.6.2/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py
--rw-r--r--   0        0        0     1741 2023-07-06 14:40:19.959730 fabric_cf-1.6.2/fabric_cf/actor/core/manage/messages/result_client_mng.py
--rw-r--r--   0        0        0     1554 2023-07-06 14:40:19.960110 fabric_cf-1.6.2/fabric_cf/actor/core/manage/messages/result_event_mng.py
--rw-r--r--   0        0        0     1904 2023-07-06 14:40:19.960406 fabric_cf-1.6.2/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py
--rw-r--r--   0        0        0    15777 2023-07-06 14:40:19.960693 fabric_cf-1.6.2/fabric_cf/actor/core/manage/server_actor_management_object.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.960916 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/__init__.py
--rw-r--r--   0        0        0     7965 2023-07-06 14:40:19.961135 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/base_plugin.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.961310 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/db/__init__.py
--rw-r--r--   0        0        0    38466 2024-02-15 17:39:56.155699 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/db/actor_database.py
--rw-r--r--   0        0        0     2624 2023-07-06 14:40:19.961912 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/db/client_database.py
--rw-r--r--   0        0        0     3792 2023-07-06 14:40:19.962101 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/db/server_actor_database.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.962266 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/handlers/__init__.py
--rw-r--r--   0        0        0    13211 2023-07-06 14:40:19.962490 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py
--rw-r--r--   0        0        0     2955 2023-07-06 14:40:19.962670 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/handlers/config_token.py
--rw-r--r--   0        0        0     2286 2023-07-06 14:40:19.962952 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py
--rw-r--r--   0        0        0     7556 2023-07-06 14:40:19.963150 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/handlers/handler_processor.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.963334 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/substrate/__init__.py
--rw-r--r--   0        0        0     3612 2023-07-06 14:40:19.963647 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/substrate/authority_substrate.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.963874 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/substrate/db/__init__.py
--rw-r--r--   0        0        0     4365 2023-07-06 14:40:19.964116 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py
--rw-r--r--   0        0        0    16974 2023-07-06 14:40:19.964376 fabric_cf-1.6.2/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.964609 fabric_cf-1.6.2/fabric_cf/actor/core/policy/__init__.py
--rw-r--r--   0        0        0    28449 2024-02-19 14:44:58.094716 fabric_cf-1.6.2/fabric_cf/actor/core/policy/authority_calendar_policy.py
--rw-r--r--   0        0        0     8891 2023-07-06 14:40:19.965192 fabric_cf-1.6.2/fabric_cf/actor/core/policy/broker_calendar_policy.py
--rw-r--r--   0        0        0    67508 2024-02-15 17:39:56.157344 fabric_cf-1.6.2/fabric_cf/actor/core/policy/broker_simpler_units_policy.py
--rw-r--r--   0        0        0    19787 2024-02-15 17:39:56.158233 fabric_cf-1.6.2/fabric_cf/actor/core/policy/controller_calendar_policy.py
--rw-r--r--   0        0        0     9815 2023-07-06 14:40:19.966140 fabric_cf-1.6.2/fabric_cf/actor/core/policy/controller_simple_policy.py
--rw-r--r--   0        0        0    10156 2024-01-22 16:38:27.640224 fabric_cf-1.6.2/fabric_cf/actor/core/policy/controller_ticket_review_policy.py
--rw-r--r--   0        0        0     1814 2023-07-06 14:40:19.966667 fabric_cf-1.6.2/fabric_cf/actor/core/policy/fifo_queue.py
--rw-r--r--   0        0        0     2981 2023-07-06 14:40:19.967022 fabric_cf-1.6.2/fabric_cf/actor/core/policy/inventory.py
--rw-r--r--   0        0        0     2785 2023-07-06 14:40:19.967293 fabric_cf-1.6.2/fabric_cf/actor/core/policy/inventory_for_type.py
--rw-r--r--   0        0        0    14503 2023-07-06 14:40:19.967543 fabric_cf-1.6.2/fabric_cf/actor/core/policy/network_node_control.py
--rw-r--r--   0        0        0    30968 2024-02-15 17:39:56.160477 fabric_cf-1.6.2/fabric_cf/actor/core/policy/network_node_inventory.py
--rw-r--r--   0        0        0     5961 2023-12-01 02:09:02.686548 fabric_cf-1.6.2/fabric_cf/actor/core/policy/network_service_control.py
--rw-r--r--   0        0        0    23429 2024-02-19 14:44:58.095454 fabric_cf-1.6.2/fabric_cf/actor/core/policy/network_service_inventory.py
--rw-r--r--   0        0        0     2032 2023-07-06 14:40:19.969184 fabric_cf-1.6.2/fabric_cf/actor/core/policy/queue_wrapper.py
--rw-r--r--   0        0        0     5157 2023-07-06 14:40:19.969467 fabric_cf-1.6.2/fabric_cf/actor/core/policy/resource_control.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.969656 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/__init__.py
--rw-r--r--   0        0        0     1821 2023-07-06 14:40:19.969919 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/actor_location.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.970121 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/__init__.py
--rw-r--r--   0        0        0     8305 2024-01-22 16:38:27.642867 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py
--rw-r--r--   0        0        0     8924 2023-07-06 14:40:19.970530 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py
--rw-r--r--   0        0        0     6744 2023-07-06 14:40:19.970730 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py
--rw-r--r--   0        0        0     4809 2023-07-06 14:40:19.970883 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py
--rw-r--r--   0        0        0     8927 2024-01-22 16:38:27.644032 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/kafka_retun.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.971273 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/services/__init__.py
--rw-r--r--   0        0        0    12672 2024-02-05 19:27:31.143225 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/services/actor_service.py
--rw-r--r--   0        0        0     7627 2023-07-06 14:40:19.971702 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/services/authority_service.py
--rw-r--r--   0        0        0     8288 2023-07-06 14:40:19.971959 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/services/broker_service.py
--rw-r--r--   0        0        0     1380 2023-07-06 14:40:19.972189 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/services/controller_service.py
--rw-r--r--   0        0        0    19239 2024-01-22 16:38:27.645754 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/translate.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.972644 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/local/__init__.py
--rw-r--r--   0        0        0     4948 2023-07-06 14:40:19.972828 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/local/local_authority.py
--rw-r--r--   0        0        0     5754 2023-07-06 14:40:19.973005 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/local/local_broker.py
--rw-r--r--   0        0        0     6924 2023-07-06 14:40:19.973194 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/local/local_proxy.py
--rw-r--r--   0        0        0     2868 2023-07-06 14:40:19.973364 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/local/local_proxy_factory.py
--rw-r--r--   0        0        0     6762 2023-07-06 14:40:19.973574 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/local/local_return.py
--rw-r--r--   0        0        0     8222 2023-07-06 14:40:19.973802 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/proxy.py
--rw-r--r--   0        0        0     3013 2023-07-06 14:40:19.974020 fabric_cf-1.6.2/fabric_cf/actor/core/proxies/proxy_factory.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.974198 fabric_cf-1.6.2/fabric_cf/actor/core/registry/__init__.py
--rw-r--r--   0        0        0     7672 2023-07-06 14:40:19.974361 fabric_cf-1.6.2/fabric_cf/actor/core/registry/actor_registry.py
--rw-r--r--   0        0        0     2177 2023-07-06 14:40:19.974574 fabric_cf-1.6.2/fabric_cf/actor/core/registry/callback_registry.py
--rw-r--r--   0        0        0     4926 2023-07-06 14:40:19.974770 fabric_cf-1.6.2/fabric_cf/actor/core/registry/peer_registry.py
--rw-r--r--   0        0        0     3912 2023-07-06 14:40:19.974918 fabric_cf-1.6.2/fabric_cf/actor/core/registry/proxy_registry.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.975103 fabric_cf-1.6.2/fabric_cf/actor/core/time/__init__.py
--rw-r--r--   0        0        0     7165 2023-07-06 14:40:19.975407 fabric_cf-1.6.2/fabric_cf/actor/core/time/actor_clock.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.975636 fabric_cf-1.6.2/fabric_cf/actor/core/time/calendar/__init__.py
--rw-r--r--   0        0        0     8224 2023-07-06 14:40:19.975920 fabric_cf-1.6.2/fabric_cf/actor/core/time/calendar/authority_calendar.py
--rw-r--r--   0        0        0     1667 2023-07-06 14:40:19.976183 fabric_cf-1.6.2/fabric_cf/actor/core/time/calendar/base_calendar.py
--rw-r--r--   0        0        0    11573 2023-07-06 14:40:19.976431 fabric_cf-1.6.2/fabric_cf/actor/core/time/calendar/broker_calendar.py
--rw-r--r--   0        0        0     9733 2023-07-06 14:40:19.976701 fabric_cf-1.6.2/fabric_cf/actor/core/time/calendar/client_calendar.py
--rw-r--r--   0        0        0     5239 2023-07-06 14:40:19.976932 fabric_cf-1.6.2/fabric_cf/actor/core/time/calendar/controller_calendar.py
--rw-r--r--   0        0        0     2550 2023-07-06 14:40:19.977120 fabric_cf-1.6.2/fabric_cf/actor/core/time/calendar/source_calendar.py
--rw-r--r--   0        0        0    15769 2023-07-06 14:40:19.977531 fabric_cf-1.6.2/fabric_cf/actor/core/time/term.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.977752 fabric_cf-1.6.2/fabric_cf/actor/core/util/__init__.py
--rw-r--r--   0        0        0     2213 2023-07-06 14:40:19.978018 fabric_cf-1.6.2/fabric_cf/actor/core/util/bids.py
--rw-r--r--   0        0        0     2905 2023-07-06 14:40:19.978525 fabric_cf-1.6.2/fabric_cf/actor/core/util/client.py
--rw-r--r--   0        0        0     2063 2023-07-06 14:40:19.978808 fabric_cf-1.6.2/fabric_cf/actor/core/util/graceful_interrupt_handler.py
--rw-r--r--   0        0        0     2163 2023-07-06 14:40:19.979101 fabric_cf-1.6.2/fabric_cf/actor/core/util/id.py
--rw-r--r--   0        0        0     1488 2023-07-06 14:40:19.979278 fabric_cf-1.6.2/fabric_cf/actor/core/util/iterable_queue.py
--rw-r--r--   0        0        0     2263 2023-07-06 14:40:19.979510 fabric_cf-1.6.2/fabric_cf/actor/core/util/kernel_timer.py
--rw-r--r--   0        0        0     3711 2024-01-22 16:38:27.646909 fabric_cf-1.6.2/fabric_cf/actor/core/util/log_helper.py
--rw-r--r--   0        0        0     2238 2023-07-06 14:40:19.979946 fabric_cf-1.6.2/fabric_cf/actor/core/util/notice.py
--rw-r--r--   0        0        0     1999 2023-07-06 14:40:19.980116 fabric_cf-1.6.2/fabric_cf/actor/core/util/reflection_utils.py
--rw-r--r--   0        0        0     8380 2023-07-06 14:40:19.980424 fabric_cf-1.6.2/fabric_cf/actor/core/util/reservation_holdings.py
--rw-r--r--   0        0        0     8864 2023-07-06 14:40:19.980689 fabric_cf-1.6.2/fabric_cf/actor/core/util/reservation_list.py
--rw-r--r--   0        0        0     6700 2023-07-06 14:40:19.980886 fabric_cf-1.6.2/fabric_cf/actor/core/util/reservation_set.py
--rw-r--r--   0        0        0     3144 2023-07-06 14:40:19.981141 fabric_cf-1.6.2/fabric_cf/actor/core/util/reservation_state.py
--rw-r--r--   0        0        0     2250 2023-07-06 14:40:19.981342 fabric_cf-1.6.2/fabric_cf/actor/core/util/resource_type.py
--rw-r--r--   0        0        0     1690 2023-07-06 14:40:19.981517 fabric_cf-1.6.2/fabric_cf/actor/core/util/rpc_exception.py
--rw-r--r--   0        0        0     4440 2024-02-12 19:17:43.249488 fabric_cf-1.6.2/fabric_cf/actor/core/util/update_data.py
--rw-r--r--   0        0        0     4619 2024-01-22 16:38:27.647929 fabric_cf-1.6.2/fabric_cf/actor/core/util/utils.py
--rw-r--r--   0        0        0     8939 2024-02-15 17:39:56.162928 fabric_cf-1.6.2/fabric_cf/actor/db/__init__.py
--rw-r--r--   0        0        0    67567 2024-02-15 17:39:56.163775 fabric_cf-1.6.2/fabric_cf/actor/db/psql_database.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.983496 fabric_cf-1.6.2/fabric_cf/actor/fim/__init__.py
--rw-r--r--   0        0        0     6326 2023-07-06 14:40:19.983705 fabric_cf-1.6.2/fabric_cf/actor/fim/asm_update_thread.py
--rw-r--r--   0        0        0    27908 2024-02-15 17:39:56.164466 fabric_cf-1.6.2/fabric_cf/actor/fim/fim_helper.py
--rw-r--r--   0        0        0        1 2023-07-06 14:40:19.984284 fabric_cf-1.6.2/fabric_cf/actor/fim/plugins/__init__.py
--rw-r--r--   0        0        0        1 2023-07-06 14:40:19.984503 fabric_cf-1.6.2/fabric_cf/actor/fim/plugins/broker/__init__.py
--rw-r--r--   0        0        0    27496 2024-02-15 17:39:56.164888 fabric_cf-1.6.2/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.985039 fabric_cf-1.6.2/fabric_cf/actor/handlers/__init__.py
--rw-r--r--   0        0        0     3015 2023-07-06 14:40:19.985319 fabric_cf-1.6.2/fabric_cf/actor/handlers/handler_base.py
--rw-r--r--   0        0        0    11187 2023-07-06 14:40:19.985524 fabric_cf-1.6.2/fabric_cf/actor/handlers/no_op_handler.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.985687 fabric_cf-1.6.2/fabric_cf/actor/security/__init__.py
--rw-r--r--   0        0        0     4736 2024-01-22 16:38:27.648990 fabric_cf-1.6.2/fabric_cf/actor/security/access_checker.py
--rw-r--r--   0        0        0     3168 2024-01-22 16:38:27.649962 fabric_cf-1.6.2/fabric_cf/actor/security/auth_token.py
--rw-r--r--   0        0        0     1561 2024-01-22 16:38:27.650914 fabric_cf-1.6.2/fabric_cf/actor/security/fabric_token.py
--rw-r--r--   0        0        0     5856 2024-01-22 16:38:27.651975 fabric_cf-1.6.2/fabric_cf/actor/security/pdp_auth.py
--rw-r--r--   0        0        0     4758 2024-01-22 16:38:27.652899 fabric_cf-1.6.2/fabric_cf/actor/security/token_validator.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.986694 fabric_cf-1.6.2/fabric_cf/actor/test/__init__.py
--rw-r--r--   0        0        0    10932 2023-07-06 14:40:19.986896 fabric_cf-1.6.2/fabric_cf/actor/test/base_test_case.py
--rw-r--r--   0        0        0     4679 2023-07-06 14:40:19.987086 fabric_cf-1.6.2/fabric_cf/actor/test/client_callback_helper.py
--rw-r--r--   0        0        0     4639 2023-07-06 14:40:19.987375 fabric_cf-1.6.2/fabric_cf/actor/test/config/config.jenkins.yaml
--rw-r--r--   0        0        0     4305 2023-07-06 14:40:19.987535 fabric_cf-1.6.2/fabric_cf/actor/test/config/config.orchestrator.yaml
--rw-r--r--   0        0        0     4696 2023-07-06 14:40:19.987673 fabric_cf-1.6.2/fabric_cf/actor/test/config/config.test.yaml
--rw-r--r--   0        0        0     5376 2023-07-06 14:40:19.987829 fabric_cf-1.6.2/fabric_cf/actor/test/controller_callback_helper.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.987976 fabric_cf-1.6.2/fabric_cf/actor/test/core/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.988137 fabric_cf-1.6.2/fabric_cf/actor/test/core/container/__init__.py
--rw-r--r--   0        0        0     2815 2023-07-06 14:40:19.988405 fabric_cf-1.6.2/fabric_cf/actor/test/core/container/container_database_test.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.988557 fabric_cf-1.6.2/fabric_cf/actor/test/core/core/__init__.py
--rw-r--r--   0        0        0     4091 2023-07-06 14:40:19.988847 fabric_cf-1.6.2/fabric_cf/actor/test/core/core/unit_test.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.989004 fabric_cf-1.6.2/fabric_cf/actor/test/core/kernel/__init__.py
--rw-r--r--   0        0        0    21480 2023-07-06 14:40:19.989244 fabric_cf-1.6.2/fabric_cf/actor/test/core/kernel/kernel_test.py
--rw-r--r--   0        0        0     3378 2023-07-06 14:40:19.989463 fabric_cf-1.6.2/fabric_cf/actor/test/core/kernel/tick_test.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.989634 fabric_cf-1.6.2/fabric_cf/actor/test/core/plugins/__init__.py
--rw-r--r--   0        0        0     3176 2023-07-06 14:40:19.989812 fabric_cf-1.6.2/fabric_cf/actor/test/core/plugins/actor_database_test.py
--rw-r--r--   0        0        0     4729 2023-07-06 14:40:19.990071 fabric_cf-1.6.2/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py
--rw-r--r--   0        0        0     1963 2023-07-06 14:40:19.990259 fabric_cf-1.6.2/fabric_cf/actor/test/core/plugins/authority_substrate_test.py
--rw-r--r--   0        0        0     3263 2023-07-06 14:40:19.990435 fabric_cf-1.6.2/fabric_cf/actor/test/core/plugins/substrate_database_test.py
--rw-r--r--   0        0        0     2280 2023-07-06 14:40:19.991829 fabric_cf-1.6.2/fabric_cf/actor/test/core/plugins/substrate_test_base.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.992082 fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/__init__.py
--rw-r--r--   0        0        0    21995 2023-07-06 14:40:19.992331 fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py
--rw-r--r--   0        0        0    23678 2023-07-06 14:40:19.992681 fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py
--rw-r--r--   0        0        0     4515 2023-07-06 14:40:19.993078 fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py
--rw-r--r--   0        0        0     1561 2023-07-06 14:40:19.993380 fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py
--rw-r--r--   0        0        0     8437 2023-07-06 14:40:19.993618 fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/controller_test_wrapper.py
--rw-r--r--   0        0        0     7719 2023-07-06 14:40:19.993823 fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py
--rw-r--r--   0        0        0     1586 2023-07-06 14:40:19.993986 fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.994155 fabric_cf-1.6.2/fabric_cf/actor/test/core/time/__init__.py
--rw-r--r--   0        0        0     3786 2023-07-06 14:40:19.994406 fabric_cf-1.6.2/fabric_cf/actor/test/core/time/actor_clock_test.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.994579 fabric_cf-1.6.2/fabric_cf/actor/test/core/time/calendar/__init__.py
--rw-r--r--   0        0        0     4290 2023-07-06 14:40:19.994779 fabric_cf-1.6.2/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py
--rw-r--r--   0        0        0     2225 2023-07-06 14:40:19.995009 fabric_cf-1.6.2/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py
--rw-r--r--   0        0        0    14887 2023-07-06 14:40:19.995232 fabric_cf-1.6.2/fabric_cf/actor/test/core/time/term_test.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.995401 fabric_cf-1.6.2/fabric_cf/actor/test/core/util/__init__.py
--rw-r--r--   0        0        0     8041 2023-07-06 14:40:19.995626 fabric_cf-1.6.2/fabric_cf/actor/test/core/util/reservation_holdings_test.py
--rw-r--r--   0        0        0     5072 2023-07-06 14:40:19.995872 fabric_cf-1.6.2/fabric_cf/actor/test/core/util/reservation_list_test.py
--rw-r--r--   0        0        0     3738 2023-07-06 14:40:19.996064 fabric_cf-1.6.2/fabric_cf/actor/test/dummy_authority_proxy.py
--rw-r--r--   0        0        0     1953 2023-07-06 14:40:19.996233 fabric_cf-1.6.2/fabric_cf/actor/test/dummy_proxy.py
--rw-r--r--   0        0        0     2498 2023-08-29 19:20:39.689504 fabric_cf-1.6.2/fabric_cf/actor/test/fim_test_helper.py
--rw-r--r--   0        0        0       92 2023-07-06 14:40:19.996635 fabric_cf-1.6.2/fabric_cf/actor/test/schema/key.avsc
--rw-r--r--   0        0        0    27389 2023-07-06 14:40:19.996847 fabric_cf-1.6.2/fabric_cf/actor/test/schema/message.avsc
--rw-r--r--   0        0        0     5358 2023-08-29 19:21:00.479457 fabric_cf-1.6.2/fabric_cf/actor/test/test_abqm.py
--rw-r--r--   0        0        0     1892 2023-07-06 14:40:19.997319 fabric_cf-1.6.2/fabric_cf/actor/test/test_actor.py
--rw-r--r--   0        0        0     1249 2023-07-06 14:40:19.997537 fabric_cf-1.6.2/fabric_cf/actor/test/test_exception.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.997709 fabric_cf-1.6.2/fabric_cf/aits/__init__.py
--rw-r--r--   0        0        0     4826 2023-07-06 14:40:19.997962 fabric_cf-1.6.2/fabric_cf/aits/config/config.broker.yaml
--rw-r--r--   0        0        0     4808 2023-07-06 14:40:19.998148 fabric_cf-1.6.2/fabric_cf/aits/config/config.netam.yaml
--rw-r--r--   0        0        0     4414 2023-07-06 14:40:19.998315 fabric_cf-1.6.2/fabric_cf/aits/config/config.orchestrator.yaml
--rw-r--r--   0        0        0     4788 2023-07-06 14:40:19.998464 fabric_cf-1.6.2/fabric_cf/aits/config/config.siteam.yaml
--rw-r--r--   0        0        0    49220 2023-07-06 14:40:19.998792 fabric_cf-1.6.2/fabric_cf/aits/integration_test.py
--rw-r--r--   0        0        0     7393 2023-07-06 14:40:19.999015 fabric_cf-1.6.2/fabric_cf/aits/kafka_processor.py
--rw-r--r--   0        0        0     8633 2023-07-06 14:40:19.999246 fabric_cf-1.6.2/fabric_cf/aits/manage_helper.py
--rw-r--r--   0        0        0     8339 2023-07-06 14:40:19.999482 fabric_cf-1.6.2/fabric_cf/aits/orchestrator_helper.py
--rw-r--r--   0        0        0    16414 2024-01-22 16:38:27.654744 fabric_cf-1.6.2/fabric_cf/authority/Readme.md
--rw-r--r--   0        0        0        0 2023-07-06 14:40:19.999946 fabric_cf-1.6.2/fabric_cf/authority/__init__.py
--rw-r--r--   0        0        0     2164 2023-07-06 14:40:20.000130 fabric_cf-1.6.2/fabric_cf/authority/__main__.py
--rw-r--r--   0        0        0     1503 2024-01-22 16:38:27.655589 fabric_cf-1.6.2/fabric_cf/authority/al2s_handler_config.yml
--rw-r--r--   0        0        0    32973 2023-07-06 14:40:20.000429 fabric_cf-1.6.2/fabric_cf/authority/am-yes.xml
--rw-r--r--   0        0        0     5125 2024-02-15 17:39:56.165295 fabric_cf-1.6.2/fabric_cf/authority/config.al2s.am.yaml
--rw-r--r--   0        0        0     5219 2024-02-15 17:39:56.165586 fabric_cf-1.6.2/fabric_cf/authority/config.net.am.yaml
--rw-r--r--   0        0        0     5589 2024-02-15 17:39:56.165822 fabric_cf-1.6.2/fabric_cf/authority/config.site.am.geni.yaml
--rw-r--r--   0        0        0     5083 2024-02-15 17:39:56.166190 fabric_cf-1.6.2/fabric_cf/authority/config.site.am.yaml
--rw-r--r--   0        0        0     3431 2024-01-22 16:38:27.660843 fabric_cf-1.6.2/fabric_cf/authority/docker-compose.geni.yml
--rw-r--r--   0        0        0     3340 2024-02-24 02:42:52.685976 fabric_cf-1.6.2/fabric_cf/authority/docker-compose.yml
--rw-r--r--   0        0        0     1191 2023-07-06 14:40:20.001777 fabric_cf-1.6.2/fabric_cf/authority/env.template
--rw-r--r--   0        0        0    16080 2023-07-06 14:40:20.001955 fabric_cf-1.6.2/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml
--rw-r--r--   0        0        0     1588 2023-07-06 14:40:20.002362 fabric_cf-1.6.2/fabric_cf/authority/net_handler_config.yml
--rw-r--r--   0        0        0     1523 2023-07-06 14:40:20.002545 fabric_cf-1.6.2/fabric_cf/authority/oess_handler_config.yml
--rw-r--r--   0        0        0     1380 2023-07-06 14:40:20.002705 fabric_cf-1.6.2/fabric_cf/authority/pdp.xml
--rwxr-xr-x   0        0        0     2446 2023-07-06 14:40:20.003053 fabric_cf-1.6.2/fabric_cf/authority/setup.sh
--rw-r--r--   0        0        0        0 2023-07-06 14:40:20.003243 fabric_cf-1.6.2/fabric_cf/authority/test/__init__.py
--rw-r--r--   0        0        0     2463 2023-07-06 14:40:20.003608 fabric_cf-1.6.2/fabric_cf/authority/test/al2s_am.py
--rw-r--r--   0        0        0     2459 2023-07-06 14:40:20.003800 fabric_cf-1.6.2/fabric_cf/authority/test/net_am.py
--rw-r--r--   0        0        0     2456 2023-07-06 14:40:20.004030 fabric_cf-1.6.2/fabric_cf/authority/test/site_am.py
--rw-r--r--   0        0        0     2461 2023-07-06 14:40:20.004325 fabric_cf-1.6.2/fabric_cf/authority/test/site_am_geni.py
--rw-r--r--   0        0        0     4834 2024-02-15 17:39:56.167061 fabric_cf-1.6.2/fabric_cf/authority/test/test-al2sam.yaml
--rw-r--r--   0        0        0     4944 2024-02-15 17:39:56.167727 fabric_cf-1.6.2/fabric_cf/authority/test/test-netam.yaml
--rw-r--r--   0        0        0     5175 2024-02-15 17:39:56.168748 fabric_cf-1.6.2/fabric_cf/authority/test/test.geni.yaml
--rw-r--r--   0        0        0     4761 2024-02-15 17:39:56.169733 fabric_cf-1.6.2/fabric_cf/authority/test/test.yaml
--rw-r--r--   0        0        0     3189 2024-01-22 16:38:27.668968 fabric_cf-1.6.2/fabric_cf/authority/vm_handler_config.yml
--rw-r--r--   0        0        0     1448 2023-07-06 14:40:20.005355 fabric_cf-1.6.2/fabric_cf/authority/vnic_net_handler_config.yml
--rw-r--r--   0        0        0    14262 2023-07-06 14:40:20.005654 fabric_cf-1.6.2/fabric_cf/broker/Readme.md
--rw-r--r--   0        0        0        0 2023-07-06 14:40:20.005739 fabric_cf-1.6.2/fabric_cf/broker/__init__.py
--rw-r--r--   0        0        0     2290 2023-07-06 14:40:20.005953 fabric_cf-1.6.2/fabric_cf/broker/__main__.py
--rw-r--r--   0        0        0    27944 2023-07-06 14:40:20.006218 fabric_cf-1.6.2/fabric_cf/broker/broker-yes.xml
--rw-r--r--   0        0        0     5222 2024-02-15 17:39:56.170241 fabric_cf-1.6.2/fabric_cf/broker/config.broker.yaml
--rw-r--r--   0        0        0        0 2023-07-06 14:40:20.006704 fabric_cf-1.6.2/fabric_cf/broker/core/__init__.py
--rw-r--r--   0        0        0     3314 2023-07-06 14:40:20.006887 fabric_cf-1.6.2/fabric_cf/broker/core/broker_kernel.py
--rw-r--r--   0        0        0     3139 2024-02-24 02:42:45.493292 fabric_cf-1.6.2/fabric_cf/broker/docker-compose.yml
--rw-r--r--   0        0        0     1195 2023-07-06 14:40:20.007248 fabric_cf-1.6.2/fabric_cf/broker/env.template
--rw-r--r--   0        0        0    16080 2023-07-06 14:40:20.007412 fabric_cf-1.6.2/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml
--rw-r--r--   0        0        0     1380 2023-07-06 14:40:20.007566 fabric_cf-1.6.2/fabric_cf/broker/pdp.xml
--rwxr-xr-x   0        0        0     2239 2023-07-06 14:40:20.007731 fabric_cf-1.6.2/fabric_cf/broker/setup.sh
--rw-r--r--   0        0        0        0 2023-07-06 14:40:20.007889 fabric_cf-1.6.2/fabric_cf/broker/test/__init__.py
--rw-r--r--   0        0        0     2507 2023-07-06 14:40:20.008088 fabric_cf-1.6.2/fabric_cf/broker/test/broker.py
--rw-r--r--   0        0        0     5236 2024-02-15 17:39:56.172112 fabric_cf-1.6.2/fabric_cf/broker/test/test.yaml
--rw-r--r--   0        0        0    20305 2023-07-06 14:40:20.008659 fabric_cf-1.6.2/fabric_cf/orchestrator/README.md
--rw-r--r--   0        0        0        0 2023-07-06 14:40:20.008780 fabric_cf-1.6.2/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0        0        0     3355 2023-07-06 14:40:20.008979 fabric_cf-1.6.2/fabric_cf/orchestrator/__main__.py
--rw-r--r--   0        0        0     1757 2023-07-06 14:40:20.009241 fabric_cf-1.6.2/fabric_cf/orchestrator/certs/fullchain.pem
--rw-r--r--   0        0        0     3272 2023-07-06 14:40:20.009402 fabric_cf-1.6.2/fabric_cf/orchestrator/certs/privkey.pem
--rw-r--r--   0        0        0     5088 2024-02-19 14:44:58.098651 fabric_cf-1.6.2/fabric_cf/orchestrator/config.orchestrator.yaml
--rw-r--r--   0        0        0        0 2023-07-06 14:40:20.009701 fabric_cf-1.6.2/fabric_cf/orchestrator/core/__init__.py
--rw-r--r--   0        0        0     3026 2024-02-15 17:39:56.173873 fabric_cf-1.6.2/fabric_cf/orchestrator/core/active_status_checker.py
--rw-r--r--   0        0        0     3247 2023-07-12 19:30:09.758686 fabric_cf-1.6.2/fabric_cf/orchestrator/core/bqm_wrapper.py
--rw-r--r--   0        0        0     1556 2023-07-06 14:40:20.010274 fabric_cf-1.6.2/fabric_cf/orchestrator/core/exceptions.py
--rw-r--r--   0        0        0     1884 2023-07-06 14:40:20.010462 fabric_cf-1.6.2/fabric_cf/orchestrator/core/i_status_update_callback.py
--rw-r--r--   0        0        0    46479 2024-02-19 14:44:58.099723 fabric_cf-1.6.2/fabric_cf/orchestrator/core/orchestrator_handler.py
--rw-r--r--   0        0        0     7423 2023-07-12 19:30:09.758992 fabric_cf-1.6.2/fabric_cf/orchestrator/core/orchestrator_kernel.py
--rw-r--r--   0        0        0    36011 2024-01-22 16:38:27.673275 fabric_cf-1.6.2/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py
--rw-r--r--   0        0        0     3581 2023-07-06 14:40:20.011490 fabric_cf-1.6.2/fabric_cf/orchestrator/core/reservation_converter.py
--rw-r--r--   0        0        0     4880 2023-07-06 14:40:20.011649 fabric_cf-1.6.2/fabric_cf/orchestrator/core/reservation_status_update.py
--rw-r--r--   0        0        0     7876 2023-07-06 14:40:20.011878 fabric_cf-1.6.2/fabric_cf/orchestrator/core/reservation_status_update_thread.py
--rw-r--r--   0        0        0     7219 2023-07-06 14:40:20.012054 fabric_cf-1.6.2/fabric_cf/orchestrator/core/response_builder.py
--rw-r--r--   0        0        0     8722 2023-07-06 14:40:20.012245 fabric_cf-1.6.2/fabric_cf/orchestrator/core/slice_defer_thread.py
--rw-r--r--   0        0        0     1972 2023-07-06 14:40:20.012433 fabric_cf-1.6.2/fabric_cf/orchestrator/core/status_checker.py
--rw-r--r--   0        0        0     1581 2023-07-06 14:40:20.012642 fabric_cf-1.6.2/fabric_cf/orchestrator/core/watch_entry.py
--rw-r--r--   0        0        0     3505 2024-02-24 02:43:00.047016 fabric_cf-1.6.2/fabric_cf/orchestrator/docker-compose.yml
--rw-r--r--   0        0        0     1201 2023-07-06 14:40:20.012989 fabric_cf-1.6.2/fabric_cf/orchestrator/env.template
--rw-r--r--   0        0        0    74275 2024-01-22 16:38:27.676544 fabric_cf-1.6.2/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml
--rw-r--r--   0        0        0     1626 2023-07-06 14:40:20.013737 fabric_cf-1.6.2/fabric_cf/orchestrator/nginx/default.conf
--rw-r--r--   0        0        0    64528 2024-01-22 16:38:27.677758 fabric_cf-1.6.2/fabric_cf/orchestrator/openapi.json
--rw-r--r--   0        0        0    30829 2023-07-06 14:40:20.014329 fabric_cf-1.6.2/fabric_cf/orchestrator/orchestrator-yes.xml
--rw-r--r--   0        0        0     1548 2023-07-06 14:40:20.014528 fabric_cf-1.6.2/fabric_cf/orchestrator/pdp.xml
--rwxr-xr-x   0        0        0     2284 2023-07-06 14:40:20.014684 fabric_cf-1.6.2/fabric_cf/orchestrator/setup.sh
--rw-r--r--   0        0        0      430 2023-07-21 13:05:26.706807 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/__init__.py
--rw-r--r--   0        0        0      392 2023-07-21 13:05:26.712379 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/__main__.py
--rw-r--r--   0        0        0        0 2023-07-21 13:05:26.687107 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/controllers/__init__.py
--rw-r--r--   0        0        0      309 2024-01-22 16:38:27.678841 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/controllers/authorization_controller.py
--rw-r--r--   0        0        0     1948 2024-01-22 16:38:27.680272 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/controllers/poas_controller.py
--rw-r--r--   0        0        0     1249 2023-07-21 14:27:27.362230 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py
--rw-r--r--   0        0        0     7375 2024-01-22 16:38:27.681314 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py
--rw-r--r--   0        0        0     1094 2023-07-21 14:27:53.536237 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py
--rw-r--r--   0        0        0      305 2023-07-21 14:28:03.310778 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/controllers/version_controller.py
--rw-r--r--   0        0        0      631 2023-07-21 13:05:26.686191 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/encoder.py
--rw-r--r--   0        0        0     2849 2024-01-22 16:38:27.682326 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/__init__.py
--rw-r--r--   0        0        0     1889 2023-07-21 13:05:26.681811 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/base_model_.py
--rw-r--r--   0        0        0     3400 2023-07-21 13:05:26.678341 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/poa.py
--rw-r--r--   0        0        0     5315 2023-07-21 13:05:26.685259 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/poa_data.py
--rw-r--r--   0        0        0     2647 2024-01-22 16:38:27.683283 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/poa_post.py
--rw-r--r--   0        0        0     3539 2024-01-22 16:38:27.684009 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/poa_post_data.py
--rw-r--r--   0        0        0     2458 2024-01-22 16:38:27.684893 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/poa_post_data_keys.py
--rw-r--r--   0        0        0     2484 2024-01-22 16:38:27.685792 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     1628 2023-07-21 13:05:26.679846 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/resource.py
--rw-r--r--   0        0        0     3564 2023-07-21 13:05:26.682401 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/resources.py
--rw-r--r--   0        0        0     7311 2023-07-21 13:05:26.678076 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/slice.py
--rw-r--r--   0        0        0     3616 2023-07-21 13:05:26.675485 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/slice_details.py
--rw-r--r--   0        0        0     5251 2023-07-21 13:05:26.683801 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/slices.py
--rw-r--r--   0        0        0     2634 2023-07-21 13:05:26.682083 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/slices_post.py
--rw-r--r--   0        0        0     8995 2023-07-21 13:05:26.685624 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/sliver.py
--rw-r--r--   0        0        0     5301 2023-07-21 13:05:26.683526 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/slivers.py
--rw-r--r--   0        0        0     3896 2023-07-21 13:05:26.684094 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     2464 2023-07-21 13:05:26.678890 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     4929 2023-07-21 13:05:26.681517 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     2870 2023-07-21 13:05:26.680712 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py
--rw-r--r--   0        0        0     1983 2023-07-21 13:05:26.681255 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py
--rw-r--r--   0        0        0     4503 2023-07-21 13:05:26.684376 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     3984 2023-07-21 13:05:26.683221 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py
--rw-r--r--   0        0        0     2512 2023-07-21 13:05:26.675987 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     3879 2023-07-21 13:05:26.682775 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py
--rw-r--r--   0        0        0     2461 2023-07-21 13:05:26.679526 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     3846 2023-07-21 13:05:26.680992 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py
--rw-r--r--   0        0        0     2446 2023-07-21 13:05:26.684653 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     4233 2023-07-21 13:05:26.679207 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     2635 2023-07-21 13:05:26.677106 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     3540 2023-07-21 13:05:26.677698 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/version.py
--rw-r--r--   0        0        0     2536 2023-07-21 13:05:26.677423 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/version_data.py
--rw-r--r--   0        0        0        0 2023-07-21 13:05:26.696979 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/__init__.py
--rw-r--r--   0        0        0     1355 2023-07-21 14:26:34.212959 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py
--rw-r--r--   0        0        0     1997 2023-07-21 13:05:26.696810 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/constants.py
--rw-r--r--   0        0        0     5537 2023-07-21 13:05:26.696497 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/cors_response.py
--rw-r--r--   0        0        0     5471 2024-01-22 16:38:27.686829 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/poas_controller.py
--rw-r--r--   0        0        0     4321 2023-07-21 13:05:26.703189 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/resources_controller.py
--rw-r--r--   0        0        0    15437 2023-07-21 13:05:26.701619 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/slices_controller.py
--rw-r--r--   0        0        0     4642 2023-07-21 13:05:26.702268 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py
--rw-r--r--   0        0        0     2530 2023-07-21 13:05:26.701151 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/utils.py
--rw-r--r--   0        0        0     2632 2023-07-21 13:05:26.702831 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/version_controller.py
--rw-r--r--   0        0        0    46662 2024-01-22 16:38:27.688350 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml
--rw-r--r--   0        0        0      438 2023-07-21 13:05:26.672917 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/test/__init__.py
--rw-r--r--   0        0        0     2531 2023-07-21 13:16:16.850784 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/test/test_poas_controller.py
--rw-r--r--   0        0        0     2094 2023-07-21 13:16:26.523105 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py
--rw-r--r--   0        0        0     5917 2023-07-21 13:16:33.995263 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py
--rw-r--r--   0        0        0     1989 2023-07-21 13:16:44.547066 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py
--rw-r--r--   0        0        0      855 2023-07-21 13:16:53.155233 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py
--rw-r--r--   0        0        0      809 2023-07-21 13:05:26.686486 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/type_util.py
--rw-r--r--   0        0        0     3452 2023-07-21 13:05:26.674386 fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/util.py
--rw-r--r--   0        0        0        0 2023-07-06 14:40:20.026771 fabric_cf-1.6.2/fabric_cf/orchestrator/test/__init__.py
--rw-r--r--   0        0        0     3542 2023-07-06 14:40:20.026956 fabric_cf-1.6.2/fabric_cf/orchestrator/test/orchestrator.py
--rwxr-xr-x   0        0        0       78 2023-07-06 14:40:20.027092 fabric_cf-1.6.2/fabric_cf/orchestrator/test/test.sh
--rw-r--r--   0        0        0     4560 2024-02-15 17:39:56.176013 fabric_cf-1.6.2/fabric_cf/orchestrator/test/test.yaml
--rwxr-xr-x   0        0        0     2900 2023-07-06 14:40:20.027470 fabric_cf-1.6.2/fabric_cf/orchestrator/update_swagger_stub.sh
--rw-r--r--   0        0        0    18177 2023-07-06 14:40:20.027906 fabric_cf-1.6.2/images/am-pod.png
--rw-r--r--   0        0        0    74927 2023-07-06 14:40:20.028627 fabric_cf-1.6.2/images/am.png
--rw-r--r--   0        0        0    18471 2023-07-06 14:40:20.028960 fabric_cf-1.6.2/images/broker-pod.png
--rw-r--r--   0        0        0    73799 2023-07-06 14:40:20.029590 fabric_cf-1.6.2/images/broker.png
--rw-r--r--   0        0        0    90831 2023-07-06 14:40:20.030329 fabric_cf-1.6.2/images/cf.png
--rw-r--r--   0        0        0    19611 2023-07-06 14:40:20.030664 fabric_cf-1.6.2/images/orchestrator-pod.png
--rw-r--r--   0        0        0    78622 2023-07-06 14:40:20.031328 fabric_cf-1.6.2/images/orchestrator.png
--rw-r--r--   0        0        0    14808 2023-07-06 14:40:20.040989 fabric_cf-1.6.2/neo4j/abqm.graphml
--rw-r--r--   0        0        0     1757 2023-07-06 14:40:20.041291 fabric_cf-1.6.2/neo4j/certs/fullchain.pem
--rw-r--r--   0        0        0     3272 2023-07-06 14:40:20.041462 fabric_cf-1.6.2/neo4j/certs/privkey.pem
--rwxr-xr-x   0        0        0       91 2023-07-06 14:40:20.041625 fabric_cf-1.6.2/orchestrator.sh
--rw-r--r--   0        0        0      980 2024-02-15 17:39:56.177452 fabric_cf-1.6.2/psql.upgrade
--rw-r--r--   0        0        0     1317 2024-02-15 17:39:56.178227 fabric_cf-1.6.2/pyproject.toml
--rwxr-xr-x   0        0        0     2594 2023-07-06 14:40:20.042295 fabric_cf-1.6.2/secrets/create-certs.sh
--rw-r--r--   0        0        0    12796 2023-07-06 14:40:20.042623 fabric_cf-1.6.2/tools/audit.py
--rw-r--r--   0        0        0     9897 2024-02-15 17:39:56.179350 fabric_cf-1.6.2/tools/db_cli.py
--rw-r--r--   0        0        0      357 2024-02-15 17:39:56.180113 fabric_cf-1.6.2/tools/install.sh
--rw-r--r--   0        0        0      143 2023-07-06 14:40:20.043220 fabric_cf-1.6.2/tox.ini
--rw-r--r--   0        0        0     3390 1970-01-01 00:00:00.000000 fabric_cf-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     2035 2023-07-06 14:40:19.903102 fabric_cf-1.6.2rc0/.gitignore
+-rw-r--r--   0        0        0      851 2024-02-24 02:42:05.148233 fabric_cf-1.6.2rc0/Dockerfile-auth
+-rw-r--r--   0        0        0      771 2024-01-22 16:38:27.605442 fabric_cf-1.6.2rc0/Dockerfile-broker
+-rw-r--r--   0        0        0     1041 2024-01-22 16:38:27.606382 fabric_cf-1.6.2rc0/Dockerfile-cf
+-rw-r--r--   0        0        0      789 2024-01-22 16:38:27.607632 fabric_cf-1.6.2rc0/Dockerfile-orchestrator
+-rw-r--r--   0        0        0     1071 2023-07-06 14:40:19.903692 fabric_cf-1.6.2rc0/LICENSE
+-rw-r--r--   0        0        0     2046 2023-07-06 14:40:19.903887 fabric_cf-1.6.2rc0/README.md
+-rwxr-xr-x   0        0        0       74 2023-07-06 14:40:19.904024 fabric_cf-1.6.2rc0/authority.sh
+-rwxr-xr-x   0        0        0       79 2023-07-06 14:40:19.904125 fabric_cf-1.6.2rc0/broker.sh
+-rw-r--r--   0        0        0      947 2023-07-06 14:40:19.904225 fabric_cf-1.6.2rc0/cleanup_old_schema_from_schema_registry.sh
+-rw-r--r--   0        0        0     2861 2023-07-06 14:40:19.904409 fabric_cf-1.6.2rc0/docker-compose-kafka.yaml
+-rw-r--r--   0        0        0     1560 2023-07-06 14:40:19.904579 fabric_cf-1.6.2rc0/docker-compose-no-ssl-kafka.yaml
+-rw-r--r--   0        0        0    10307 2024-01-22 16:38:27.610519 fabric_cf-1.6.2rc0/docker-compose-test.yaml
+-rwxr-xr-x   0        0        0       46 2024-01-22 16:38:27.611401 fabric_cf-1.6.2rc0/docker-entrypoint.sh
+-rw-r--r--   0        0        0      350 2023-07-06 14:40:19.904923 fabric_cf-1.6.2rc0/env.template
+-rw-r--r--   0        0        0     1135 2023-07-06 14:40:19.905192 fabric_cf-1.6.2rc0/env.template.test
+-rw-r--r--   0        0        0    16609 2023-07-06 14:40:19.905386 fabric_cf-1.6.2rc0/fabricNo.AnyActorNoPolicy.xml
+-rw-r--r--   0        0        0     6343 2023-07-06 14:40:19.905685 fabric_cf-1.6.2rc0/fabric_cf/Design.md
+-rw-r--r--   0        0        0       51 2024-02-24 02:47:58.223384 fabric_cf-1.6.2rc0/fabric_cf/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.905895 fabric_cf-1.6.2rc0/fabric_cf/actor/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.905999 fabric_cf-1.6.2rc0/fabric_cf/actor/boot/__init__.py
+-rw-r--r--   0        0        0    15904 2024-02-15 17:39:56.133953 fabric_cf-1.6.2rc0/fabric_cf/actor/boot/configuration.py
+-rw-r--r--   0        0        0     1268 2023-07-06 14:40:19.906660 fabric_cf-1.6.2rc0/fabric_cf/actor/boot/configuration_exception.py
+-rw-r--r--   0        0        0     2509 2023-07-06 14:40:19.907136 fabric_cf-1.6.2rc0/fabric_cf/actor/boot/configuration_loader.py
+-rw-r--r--   0        0        0    23003 2023-07-06 14:40:19.907477 fabric_cf-1.6.2rc0/fabric_cf/actor/boot/configuration_processor.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.907709 fabric_cf-1.6.2rc0/fabric_cf/actor/boot/inventory/__init__.py
+-rw-r--r--   0        0        0     4969 2023-07-06 14:40:19.907981 fabric_cf-1.6.2rc0/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.908142 fabric_cf-1.6.2rc0/fabric_cf/actor/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.908303 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/__init__.py
+-rw-r--r--   0        0        0     4907 2023-07-06 14:40:19.908566 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_container.py
+-rw-r--r--   0        0        0     1530 2023-07-06 14:40:19.908811 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_event.py
+-rw-r--r--   0        0        0     2176 2023-07-06 14:40:19.909045 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_identity.py
+-rw-r--r--   0        0        0    11057 2024-02-15 17:39:56.134395 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_management_object.py
+-rw-r--r--   0        0        0    22153 2024-02-15 17:39:56.135663 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_mixin.py
+-rw-r--r--   0        0        0     1918 2023-07-06 14:40:19.910056 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_proxy.py
+-rw-r--r--   0        0        0     1323 2023-07-06 14:40:19.910353 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_runnable.py
+-rw-r--r--   0        0        0     4749 2024-01-22 16:38:27.617796 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_authority.py
+-rw-r--r--   0        0        0     8736 2023-07-06 14:40:19.910801 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_authority_policy.py
+-rw-r--r--   0        0        0     3657 2023-07-06 14:40:19.911078 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_authority_proxy.py
+-rw-r--r--   0        0        0     3367 2023-07-06 14:40:19.912325 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_authority_reservation.py
+-rw-r--r--   0        0        0     6071 2023-07-06 14:40:19.912747 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_base_plugin.py
+-rw-r--r--   0        0        0     2290 2023-07-06 14:40:19.913005 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_broker_mixin.py
+-rw-r--r--   0        0        0     1492 2023-07-06 14:40:19.913272 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py
+-rw-r--r--   0        0        0     3690 2023-07-06 14:40:19.913487 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_broker_proxy.py
+-rw-r--r--   0        0        0     4012 2023-07-06 14:40:19.913729 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_broker_reservation.py
+-rw-r--r--   0        0        0     2442 2023-07-06 14:40:19.913939 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_callback_proxy.py
+-rw-r--r--   0        0        0     9846 2023-07-06 14:40:19.914206 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_client_actor.py
+-rw-r--r--   0        0        0     6811 2023-07-06 14:40:19.914611 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_client_actor_management_object.py
+-rw-r--r--   0        0        0     2640 2023-07-06 14:40:19.914862 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_client_callback_proxy.py
+-rw-r--r--   0        0        0     5802 2023-07-06 14:40:19.915112 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_client_policy.py
+-rw-r--r--   0        0        0     7724 2023-07-06 14:40:19.915445 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_client_reservation.py
+-rw-r--r--   0        0        0     1936 2023-07-06 14:40:19.915721 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_component.py
+-rw-r--r--   0        0        0    10115 2023-07-06 14:40:19.915929 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_concrete_set.py
+-rw-r--r--   0        0        0     2729 2023-07-06 14:40:19.916612 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_container_clock.py
+-rw-r--r--   0        0        0     3976 2023-07-06 14:40:19.917089 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_container_database.py
+-rw-r--r--   0        0        0     3367 2023-07-06 14:40:19.917325 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_controller.py
+-rw-r--r--   0        0        0     2855 2023-07-06 14:40:19.917527 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py
+-rw-r--r--   0        0        0     2787 2023-07-06 14:40:19.917690 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_controller_policy.py
+-rw-r--r--   0        0        0     5713 2023-07-06 14:40:19.917899 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_controller_reservation.py
+-rw-r--r--   0        0        0    12064 2024-02-15 17:39:56.136629 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_database.py
+-rw-r--r--   0        0        0    11127 2023-07-06 14:40:19.918323 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_delegation.py
+-rw-r--r--   0        0        0     1867 2023-07-06 14:40:19.918509 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_event.py
+-rw-r--r--   0        0        0     1943 2023-07-06 14:40:19.918929 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_management_object.py
+-rw-r--r--   0        0        0    10150 2024-02-15 17:39:56.137005 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_actor.py
+-rw-r--r--   0        0        0     2534 2023-07-06 14:40:19.919334 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_authority.py
+-rw-r--r--   0        0        0     1452 2023-07-06 14:40:19.919514 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py
+-rw-r--r--   0        0        0     6191 2023-07-06 14:40:19.919720 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py
+-rw-r--r--   0        0        0     5041 2023-07-06 14:40:19.919903 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_container.py
+-rw-r--r--   0        0        0     2486 2023-07-06 14:40:19.920096 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py
+-rw-r--r--   0        0        0     5014 2023-07-06 14:40:19.920347 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py
+-rw-r--r--   0        0        0    11147 2023-07-06 14:40:19.920532 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_policy.py
+-rw-r--r--   0        0        0     2304 2023-07-06 14:40:19.920723 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_proxy.py
+-rw-r--r--   0        0        0     2290 2023-07-06 14:40:19.920941 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_proxy_factory.py
+-rw-r--r--   0        0        0     1658 2023-07-06 14:40:19.921528 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_query_response_handler.py
+-rw-r--r--   0        0        0    14642 2024-02-15 17:39:56.138505 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_reservation_mixin.py
+-rw-r--r--   0        0        0     9388 2023-07-06 14:40:19.922320 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_reservation_resources.py
+-rw-r--r--   0        0        0     5581 2023-07-06 14:40:19.922552 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_reservation_status.py
+-rw-r--r--   0        0        0     8963 2023-07-06 14:40:19.922838 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_resource_control.py
+-rw-r--r--   0        0        0     1336 2023-07-06 14:40:19.923076 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_response_handler.py
+-rw-r--r--   0        0        0     2246 2023-07-06 14:40:19.923329 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_rpc_request_state.py
+-rw-r--r--   0        0        0     5634 2023-07-06 14:40:19.923525 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_server_actor.py
+-rw-r--r--   0        0        0     6415 2023-07-06 14:40:19.923729 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_server_policy.py
+-rw-r--r--   0        0        0     4846 2023-07-06 14:40:19.923935 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_server_reservation.py
+-rw-r--r--   0        0        0    13280 2023-07-06 14:40:19.924255 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_slice.py
+-rw-r--r--   0        0        0     3548 2023-07-06 14:40:19.924544 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_substrate.py
+-rw-r--r--   0        0        0     2225 2023-07-06 14:40:19.924790 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_substrate_database.py
+-rw-r--r--   0        0        0     2943 2023-07-06 14:40:19.925003 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_tick.py
+-rw-r--r--   0        0        0     6121 2023-07-06 14:40:19.925195 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_ticker.py
+-rw-r--r--   0        0        0     1590 2023-07-06 14:40:19.925375 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_timer_queue.py
+-rw-r--r--   0        0        0     1387 2023-07-06 14:40:19.925617 fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_timer_task.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.925835 fabric_cf-1.6.2rc0/fabric_cf/actor/core/common/__init__.py
+-rw-r--r--   0        0        0    13545 2024-02-19 14:44:58.093768 fabric_cf-1.6.2rc0/fabric_cf/actor/core/common/constants.py
+-rw-r--r--   0        0        0     5894 2024-01-22 16:38:27.622996 fabric_cf-1.6.2rc0/fabric_cf/actor/core/common/event_logger.py
+-rw-r--r--   0        0        0     5517 2023-07-06 14:40:19.926617 fabric_cf-1.6.2rc0/fabric_cf/actor/core/common/exceptions.py
+-rw-r--r--   0        0        0     6108 2023-07-06 14:40:19.926828 fabric_cf-1.6.2rc0/fabric_cf/actor/core/common/resource_config.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.927014 fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/__init__.py
+-rw-r--r--   0        0        0    24564 2024-02-05 19:10:51.724345 fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/container.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.927724 fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/db/__init__.py
+-rw-r--r--   0        0        0     8667 2023-07-06 14:40:19.928046 fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/db/container_database.py
+-rw-r--r--   0        0        0    22315 2024-02-15 17:39:56.139869 fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/globals.py
+-rw-r--r--   0        0        0     9407 2023-12-01 02:09:02.681115 fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/maintenance.py
+-rw-r--r--   0        0        0     4284 2024-02-15 17:39:56.140477 fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/message_service.py
+-rw-r--r--   0        0        0     1508 2023-07-06 14:40:19.929116 fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/protocol_descriptor.py
+-rw-r--r--   0        0        0    13005 2023-07-06 14:40:19.929611 fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/remote_actor_cache.py
+-rw-r--r--   0        0        0     7320 2024-02-15 17:39:56.140947 fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/rpc_consumer.py
+-rw-r--r--   0        0        0     8437 2024-02-15 17:39:56.141308 fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/rpc_producer.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.930049 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/__init__.py
+-rw-r--r--   0        0        0    36977 2024-02-15 17:39:56.142190 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/actor.py
+-rw-r--r--   0        0        0     1975 2023-07-06 14:40:19.930990 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/actor_identity.py
+-rw-r--r--   0        0        0    15515 2024-01-22 16:38:27.626136 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/authority.py
+-rw-r--r--   0        0        0     4845 2023-07-06 14:40:19.931698 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/authority_policy.py
+-rw-r--r--   0        0        0    20447 2023-07-06 14:40:19.932087 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/broker.py
+-rw-r--r--   0        0        0     5914 2023-07-06 14:40:19.933176 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/broker_policy.py
+-rw-r--r--   0        0        0    20424 2024-01-22 16:38:27.627154 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/controller.py
+-rw-r--r--   0        0        0     8631 2023-07-06 14:40:19.934048 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/event_processor.py
+-rw-r--r--   0        0        0     5467 2023-07-06 14:40:19.934289 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/inventory_slice_manager.py
+-rw-r--r--   0        0        0     6171 2023-07-06 14:40:19.934575 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/policy.py
+-rw-r--r--   0        0        0     2042 2023-07-06 14:40:19.934764 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/rpc_request_state.py
+-rw-r--r--   0        0        0     8688 2023-07-06 14:40:19.934985 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/ticket.py
+-rw-r--r--   0        0        0    16794 2024-01-22 16:38:27.628065 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/unit.py
+-rw-r--r--   0        0        0    13818 2024-01-22 16:38:27.629229 fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/unit_set.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.935644 fabric_cf-1.6.2rc0/fabric_cf/actor/core/delegation/__init__.py
+-rw-r--r--   0        0        0    11147 2024-02-15 17:39:56.142971 fabric_cf-1.6.2rc0/fabric_cf/actor/core/delegation/broker_delegation.py
+-rw-r--r--   0        0        0     1933 2023-07-06 14:40:19.936411 fabric_cf-1.6.2rc0/fabric_cf/actor/core/delegation/broker_delegation_factory.py
+-rw-r--r--   0        0        0    17061 2023-07-06 14:40:19.936650 fabric_cf-1.6.2rc0/fabric_cf/actor/core/delegation/delegation.py
+-rw-r--r--   0        0        0     1916 2023-07-06 14:40:19.936853 fabric_cf-1.6.2rc0/fabric_cf/actor/core/delegation/delegation_factory.py
+-rw-r--r--   0        0        0     5364 2023-07-06 14:40:19.937100 fabric_cf-1.6.2rc0/fabric_cf/actor/core/delegation/resource_ticket.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.937314 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/__init__.py
+-rw-r--r--   0        0        0    32557 2024-02-15 17:39:56.143738 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/authority_reservation.py
+-rw-r--r--   0        0        0     3384 2023-07-06 14:40:19.938172 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/broker_query_model_publisher.py
+-rw-r--r--   0        0        0    27849 2024-02-15 17:39:56.145093 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/broker_reservation.py
+-rw-r--r--   0        0        0     2992 2023-07-06 14:40:19.938929 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/claim_timeout.py
+-rw-r--r--   0        0        0     4396 2023-07-06 14:40:19.939229 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/failed_rpc.py
+-rw-r--r--   0        0        0     3639 2023-07-06 14:40:19.939436 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/failed_rpc_event.py
+-rw-r--r--   0        0        0     2668 2023-07-06 14:40:19.939773 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py
+-rw-r--r--   0        0        0     2708 2023-07-06 14:40:19.940197 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_failed_rpc.py
+-rw-r--r--   0        0        0     2274 2023-07-06 14:40:19.940545 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_poa_rpc.py
+-rw-r--r--   0        0        0     2105 2023-07-06 14:40:19.940998 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_query_rpc.py
+-rw-r--r--   0        0        0     2703 2023-07-06 14:40:19.941194 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py
+-rw-r--r--   0        0        0     4158 2023-07-06 14:40:19.941400 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_rpc.py
+-rw-r--r--   0        0        0    11227 2023-07-06 14:40:19.941668 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_rpc_event.py
+-rw-r--r--   0        0        0    67404 2024-02-15 17:39:56.146021 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/kernel.py
+-rw-r--r--   0        0        0     3314 2023-07-06 14:40:19.942401 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/kernel_tick.py
+-rw-r--r--   0        0        0    58250 2024-02-15 17:39:56.146854 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/kernel_wrapper.py
+-rw-r--r--   0        0        0    13520 2024-01-22 16:38:27.632286 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/poa.py
+-rw-r--r--   0        0        0     2363 2023-07-06 14:40:19.943408 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/predecessor_state.py
+-rw-r--r--   0        0        0     2860 2023-07-06 14:40:19.943609 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/query_timeout.py
+-rw-r--r--   0        0        0     1404 2023-07-06 14:40:19.943902 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/request_types.py
+-rw-r--r--   0        0        0    24768 2024-02-15 17:39:56.148232 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/reservation.py
+-rw-r--r--   0        0        0    92379 2024-02-15 17:39:56.149732 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/reservation_client.py
+-rw-r--r--   0        0        0     9994 2023-07-06 14:40:19.945164 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/reservation_server.py
+-rw-r--r--   0        0        0     3451 2024-02-15 17:39:56.150884 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/reservation_states.py
+-rw-r--r--   0        0        0    21131 2023-07-06 14:40:19.945902 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/resource_set.py
+-rw-r--r--   0        0        0     1614 2023-07-06 14:40:19.946143 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/retry_rpc.py
+-rw-r--r--   0        0        0     1899 2023-07-06 14:40:19.946405 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/retry_rpc_event.py
+-rw-r--r--   0        0        0     4128 2023-07-06 14:40:19.946774 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/rpc_executor.py
+-rw-r--r--   0        0        0    32934 2024-02-12 17:21:22.410231 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/rpc_manager.py
+-rw-r--r--   0        0        0     1772 2023-07-06 14:40:19.947586 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/rpc_manager_singleton.py
+-rw-r--r--   0        0        0     3793 2023-07-06 14:40:19.947812 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/rpc_request.py
+-rw-r--r--   0        0        0     1650 2023-07-06 14:40:19.948108 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/rpc_request_type.py
+-rw-r--r--   0        0        0     1340 2023-07-06 14:40:19.948369 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/sequence_comparison_codes.py
+-rw-r--r--   0        0        0    12284 2023-07-06 14:40:19.948609 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/slice.py
+-rw-r--r--   0        0        0    13487 2024-02-15 17:39:56.151880 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/slice_state_machine.py
+-rw-r--r--   0        0        0     8319 2023-07-06 14:40:19.949044 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/slice_table.py
+-rw-r--r--   0        0        0     6527 2023-07-06 14:40:19.949206 fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/tick.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.949376 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/__init__.py
+-rw-r--r--   0        0        0    41298 2024-02-15 17:39:56.152901 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/actor_management_object.py
+-rw-r--r--   0        0        0     8431 2023-07-06 14:40:19.950168 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/authority_management_object.py
+-rw-r--r--   0        0        0     7315 2023-07-06 14:40:19.950425 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/broker_management_object.py
+-rw-r--r--   0        0        0    29438 2023-07-06 14:40:19.950803 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/client_actor_management_object_helper.py
+-rw-r--r--   0        0        0     9605 2023-07-06 14:40:19.951070 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/container_management_object.py
+-rw-r--r--   0        0        0     9165 2023-07-06 14:40:19.951281 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/controller_management_object.py
+-rw-r--r--   0        0        0    13007 2023-07-06 14:40:19.951532 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/converter.py
+-rw-r--r--   0        0        0     1624 2023-07-06 14:40:19.951814 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/error.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.951987 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/__init__.py
+-rw-r--r--   0        0        0    10686 2024-02-15 17:39:56.153449 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_actor.py
+-rw-r--r--   0        0        0     3509 2023-07-06 14:40:19.952418 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_authority.py
+-rw-r--r--   0        0        0     8200 2023-12-01 02:08:52.565147 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     4483 2023-07-06 14:40:19.952942 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_container.py
+-rw-r--r--   0        0        0     5462 2023-07-06 14:40:19.953162 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_controller.py
+-rw-r--r--   0        0        0     5462 2023-07-06 14:40:19.953389 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py
+-rw-r--r--   0        0        0     6960 2023-07-06 14:40:19.953595 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_proxy.py
+-rw-r--r--   0        0        0     5730 2023-07-06 14:40:19.953784 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.954011 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/__init__.py
+-rw-r--r--   0        0        0    24550 2023-07-06 14:40:19.954465 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py
+-rw-r--r--   0        0        0     5715 2023-07-06 14:40:19.954804 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py
+-rw-r--r--   0        0        0     5797 2023-07-06 14:40:19.955203 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py
+-rw-r--r--   0        0        0    15846 2023-09-15 17:58:20.250112 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py
+-rw-r--r--   0        0        0     4008 2023-07-06 14:40:19.955727 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py
+-rw-r--r--   0        0        0     8228 2023-07-06 14:40:19.956009 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py
+-rw-r--r--   0        0        0     2136 2024-02-15 17:39:56.153820 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_service.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.956509 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/__init__.py
+-rw-r--r--   0        0        0    12259 2024-02-15 17:39:56.154238 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_actor.py
+-rw-r--r--   0        0        0     3902 2023-07-06 14:40:19.956881 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_authority.py
+-rw-r--r--   0        0        0     8391 2023-07-06 14:40:19.957075 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_broker.py
+-rw-r--r--   0        0        0    10119 2023-07-06 14:40:19.957225 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_container.py
+-rw-r--r--   0        0        0     9646 2023-07-06 14:40:19.957405 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_controller.py
+-rw-r--r--   0        0        0     2954 2023-07-06 14:40:19.957574 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_proxy.py
+-rw-r--r--   0        0        0     8655 2023-07-06 14:40:19.957761 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_server_actor.py
+-rw-r--r--   0        0        0     7217 2023-07-06 14:40:19.958014 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/management_object.py
+-rw-r--r--   0        0        0     7841 2023-07-06 14:40:19.958239 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/management_object_manager.py
+-rw-r--r--   0        0        0     4972 2023-07-06 14:40:19.958443 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/management_utils.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.958621 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/messages/__init__.py
+-rw-r--r--   0        0        0     1604 2023-07-06 14:40:19.958823 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/messages/client_mng.py
+-rw-r--r--   0        0        0     1570 2023-07-06 14:40:19.958990 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/messages/event_mng.py
+-rw-r--r--   0        0        0     1802 2023-07-06 14:40:19.959148 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py
+-rw-r--r--   0        0        0     1741 2023-07-06 14:40:19.959730 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/messages/result_client_mng.py
+-rw-r--r--   0        0        0     1554 2023-07-06 14:40:19.960110 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/messages/result_event_mng.py
+-rw-r--r--   0        0        0     1904 2023-07-06 14:40:19.960406 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py
+-rw-r--r--   0        0        0    15777 2023-07-06 14:40:19.960693 fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/server_actor_management_object.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.960916 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/__init__.py
+-rw-r--r--   0        0        0     7965 2023-07-06 14:40:19.961135 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/base_plugin.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.961310 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/db/__init__.py
+-rw-r--r--   0        0        0    38466 2024-02-15 17:39:56.155699 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/db/actor_database.py
+-rw-r--r--   0        0        0     2624 2023-07-06 14:40:19.961912 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/db/client_database.py
+-rw-r--r--   0        0        0     3792 2023-07-06 14:40:19.962101 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/db/server_actor_database.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.962266 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/handlers/__init__.py
+-rw-r--r--   0        0        0    13211 2023-07-06 14:40:19.962490 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py
+-rw-r--r--   0        0        0     2955 2023-07-06 14:40:19.962670 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/handlers/config_token.py
+-rw-r--r--   0        0        0     2286 2023-07-06 14:40:19.962952 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py
+-rw-r--r--   0        0        0     7556 2023-07-06 14:40:19.963150 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/handlers/handler_processor.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.963334 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/substrate/__init__.py
+-rw-r--r--   0        0        0     3612 2023-07-06 14:40:19.963647 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/substrate/authority_substrate.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.963874 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/substrate/db/__init__.py
+-rw-r--r--   0        0        0     4365 2023-07-06 14:40:19.964116 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py
+-rw-r--r--   0        0        0    16974 2023-07-06 14:40:19.964376 fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.964609 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/__init__.py
+-rw-r--r--   0        0        0    28449 2024-02-19 14:44:58.094716 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/authority_calendar_policy.py
+-rw-r--r--   0        0        0     8891 2023-07-06 14:40:19.965192 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/broker_calendar_policy.py
+-rw-r--r--   0        0        0    67508 2024-02-15 17:39:56.157344 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/broker_simpler_units_policy.py
+-rw-r--r--   0        0        0    19787 2024-02-15 17:39:56.158233 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/controller_calendar_policy.py
+-rw-r--r--   0        0        0     9815 2023-07-06 14:40:19.966140 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/controller_simple_policy.py
+-rw-r--r--   0        0        0    10156 2024-01-22 16:38:27.640224 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/controller_ticket_review_policy.py
+-rw-r--r--   0        0        0     1814 2023-07-06 14:40:19.966667 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/fifo_queue.py
+-rw-r--r--   0        0        0     2981 2023-07-06 14:40:19.967022 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/inventory.py
+-rw-r--r--   0        0        0     2785 2023-07-06 14:40:19.967293 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/inventory_for_type.py
+-rw-r--r--   0        0        0    14503 2023-07-06 14:40:19.967543 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/network_node_control.py
+-rw-r--r--   0        0        0    30968 2024-02-15 17:39:56.160477 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/network_node_inventory.py
+-rw-r--r--   0        0        0     5961 2023-12-01 02:09:02.686548 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/network_service_control.py
+-rw-r--r--   0        0        0    23429 2024-02-19 14:44:58.095454 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/network_service_inventory.py
+-rw-r--r--   0        0        0     2032 2023-07-06 14:40:19.969184 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/queue_wrapper.py
+-rw-r--r--   0        0        0     5157 2023-07-06 14:40:19.969467 fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/resource_control.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.969656 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/__init__.py
+-rw-r--r--   0        0        0     1821 2023-07-06 14:40:19.969919 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/actor_location.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.970121 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/__init__.py
+-rw-r--r--   0        0        0     8305 2024-01-22 16:38:27.642867 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py
+-rw-r--r--   0        0        0     8924 2023-07-06 14:40:19.970530 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py
+-rw-r--r--   0        0        0     6744 2023-07-06 14:40:19.970730 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py
+-rw-r--r--   0        0        0     4809 2023-07-06 14:40:19.970883 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py
+-rw-r--r--   0        0        0     8927 2024-01-22 16:38:27.644032 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/kafka_retun.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.971273 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/services/__init__.py
+-rw-r--r--   0        0        0    12672 2024-02-05 19:27:31.143225 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/services/actor_service.py
+-rw-r--r--   0        0        0     7627 2023-07-06 14:40:19.971702 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/services/authority_service.py
+-rw-r--r--   0        0        0     8288 2023-07-06 14:40:19.971959 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/services/broker_service.py
+-rw-r--r--   0        0        0     1380 2023-07-06 14:40:19.972189 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/services/controller_service.py
+-rw-r--r--   0        0        0    19239 2024-01-22 16:38:27.645754 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/translate.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.972644 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/local/__init__.py
+-rw-r--r--   0        0        0     4948 2023-07-06 14:40:19.972828 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/local/local_authority.py
+-rw-r--r--   0        0        0     5754 2023-07-06 14:40:19.973005 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/local/local_broker.py
+-rw-r--r--   0        0        0     6924 2023-07-06 14:40:19.973194 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/local/local_proxy.py
+-rw-r--r--   0        0        0     2868 2023-07-06 14:40:19.973364 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/local/local_proxy_factory.py
+-rw-r--r--   0        0        0     6762 2023-07-06 14:40:19.973574 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/local/local_return.py
+-rw-r--r--   0        0        0     8222 2023-07-06 14:40:19.973802 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/proxy.py
+-rw-r--r--   0        0        0     3013 2023-07-06 14:40:19.974020 fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/proxy_factory.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.974198 fabric_cf-1.6.2rc0/fabric_cf/actor/core/registry/__init__.py
+-rw-r--r--   0        0        0     7672 2023-07-06 14:40:19.974361 fabric_cf-1.6.2rc0/fabric_cf/actor/core/registry/actor_registry.py
+-rw-r--r--   0        0        0     2177 2023-07-06 14:40:19.974574 fabric_cf-1.6.2rc0/fabric_cf/actor/core/registry/callback_registry.py
+-rw-r--r--   0        0        0     4926 2023-07-06 14:40:19.974770 fabric_cf-1.6.2rc0/fabric_cf/actor/core/registry/peer_registry.py
+-rw-r--r--   0        0        0     3912 2023-07-06 14:40:19.974918 fabric_cf-1.6.2rc0/fabric_cf/actor/core/registry/proxy_registry.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.975103 fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/__init__.py
+-rw-r--r--   0        0        0     7165 2023-07-06 14:40:19.975407 fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/actor_clock.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.975636 fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/calendar/__init__.py
+-rw-r--r--   0        0        0     8224 2023-07-06 14:40:19.975920 fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/calendar/authority_calendar.py
+-rw-r--r--   0        0        0     1667 2023-07-06 14:40:19.976183 fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/calendar/base_calendar.py
+-rw-r--r--   0        0        0    11573 2023-07-06 14:40:19.976431 fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/calendar/broker_calendar.py
+-rw-r--r--   0        0        0     9733 2023-07-06 14:40:19.976701 fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/calendar/client_calendar.py
+-rw-r--r--   0        0        0     5239 2023-07-06 14:40:19.976932 fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/calendar/controller_calendar.py
+-rw-r--r--   0        0        0     2550 2023-07-06 14:40:19.977120 fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/calendar/source_calendar.py
+-rw-r--r--   0        0        0    15769 2023-07-06 14:40:19.977531 fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/term.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.977752 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/__init__.py
+-rw-r--r--   0        0        0     2213 2023-07-06 14:40:19.978018 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/bids.py
+-rw-r--r--   0        0        0     2905 2023-07-06 14:40:19.978525 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/client.py
+-rw-r--r--   0        0        0     2063 2023-07-06 14:40:19.978808 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/graceful_interrupt_handler.py
+-rw-r--r--   0        0        0     2163 2023-07-06 14:40:19.979101 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/id.py
+-rw-r--r--   0        0        0     1488 2023-07-06 14:40:19.979278 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/iterable_queue.py
+-rw-r--r--   0        0        0     2263 2023-07-06 14:40:19.979510 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/kernel_timer.py
+-rw-r--r--   0        0        0     3711 2024-01-22 16:38:27.646909 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/log_helper.py
+-rw-r--r--   0        0        0     2238 2023-07-06 14:40:19.979946 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/notice.py
+-rw-r--r--   0        0        0     1999 2023-07-06 14:40:19.980116 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/reflection_utils.py
+-rw-r--r--   0        0        0     8380 2023-07-06 14:40:19.980424 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/reservation_holdings.py
+-rw-r--r--   0        0        0     8864 2023-07-06 14:40:19.980689 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/reservation_list.py
+-rw-r--r--   0        0        0     6700 2023-07-06 14:40:19.980886 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/reservation_set.py
+-rw-r--r--   0        0        0     3144 2023-07-06 14:40:19.981141 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/reservation_state.py
+-rw-r--r--   0        0        0     2250 2023-07-06 14:40:19.981342 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/resource_type.py
+-rw-r--r--   0        0        0     1690 2023-07-06 14:40:19.981517 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/rpc_exception.py
+-rw-r--r--   0        0        0     4440 2024-02-12 19:17:43.249488 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/update_data.py
+-rw-r--r--   0        0        0     4619 2024-01-22 16:38:27.647929 fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/utils.py
+-rw-r--r--   0        0        0     8939 2024-02-15 17:39:56.162928 fabric_cf-1.6.2rc0/fabric_cf/actor/db/__init__.py
+-rw-r--r--   0        0        0    67567 2024-02-15 17:39:56.163775 fabric_cf-1.6.2rc0/fabric_cf/actor/db/psql_database.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.983496 fabric_cf-1.6.2rc0/fabric_cf/actor/fim/__init__.py
+-rw-r--r--   0        0        0     6326 2023-07-06 14:40:19.983705 fabric_cf-1.6.2rc0/fabric_cf/actor/fim/asm_update_thread.py
+-rw-r--r--   0        0        0    27908 2024-02-15 17:39:56.164466 fabric_cf-1.6.2rc0/fabric_cf/actor/fim/fim_helper.py
+-rw-r--r--   0        0        0        1 2023-07-06 14:40:19.984284 fabric_cf-1.6.2rc0/fabric_cf/actor/fim/plugins/__init__.py
+-rw-r--r--   0        0        0        1 2023-07-06 14:40:19.984503 fabric_cf-1.6.2rc0/fabric_cf/actor/fim/plugins/broker/__init__.py
+-rw-r--r--   0        0        0    27496 2024-02-15 17:39:56.164888 fabric_cf-1.6.2rc0/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.985039 fabric_cf-1.6.2rc0/fabric_cf/actor/handlers/__init__.py
+-rw-r--r--   0        0        0     3015 2023-07-06 14:40:19.985319 fabric_cf-1.6.2rc0/fabric_cf/actor/handlers/handler_base.py
+-rw-r--r--   0        0        0    11187 2023-07-06 14:40:19.985524 fabric_cf-1.6.2rc0/fabric_cf/actor/handlers/no_op_handler.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.985687 fabric_cf-1.6.2rc0/fabric_cf/actor/security/__init__.py
+-rw-r--r--   0        0        0     4736 2024-01-22 16:38:27.648990 fabric_cf-1.6.2rc0/fabric_cf/actor/security/access_checker.py
+-rw-r--r--   0        0        0     3168 2024-01-22 16:38:27.649962 fabric_cf-1.6.2rc0/fabric_cf/actor/security/auth_token.py
+-rw-r--r--   0        0        0     1561 2024-01-22 16:38:27.650914 fabric_cf-1.6.2rc0/fabric_cf/actor/security/fabric_token.py
+-rw-r--r--   0        0        0     5856 2024-01-22 16:38:27.651975 fabric_cf-1.6.2rc0/fabric_cf/actor/security/pdp_auth.py
+-rw-r--r--   0        0        0     4758 2024-01-22 16:38:27.652899 fabric_cf-1.6.2rc0/fabric_cf/actor/security/token_validator.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.986694 fabric_cf-1.6.2rc0/fabric_cf/actor/test/__init__.py
+-rw-r--r--   0        0        0    10932 2023-07-06 14:40:19.986896 fabric_cf-1.6.2rc0/fabric_cf/actor/test/base_test_case.py
+-rw-r--r--   0        0        0     4679 2023-07-06 14:40:19.987086 fabric_cf-1.6.2rc0/fabric_cf/actor/test/client_callback_helper.py
+-rw-r--r--   0        0        0     4639 2023-07-06 14:40:19.987375 fabric_cf-1.6.2rc0/fabric_cf/actor/test/config/config.jenkins.yaml
+-rw-r--r--   0        0        0     4305 2023-07-06 14:40:19.987535 fabric_cf-1.6.2rc0/fabric_cf/actor/test/config/config.orchestrator.yaml
+-rw-r--r--   0        0        0     4696 2023-07-06 14:40:19.987673 fabric_cf-1.6.2rc0/fabric_cf/actor/test/config/config.test.yaml
+-rw-r--r--   0        0        0     5376 2023-07-06 14:40:19.987829 fabric_cf-1.6.2rc0/fabric_cf/actor/test/controller_callback_helper.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.987976 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.988137 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/container/__init__.py
+-rw-r--r--   0        0        0     2815 2023-07-06 14:40:19.988405 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/container/container_database_test.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.988557 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/core/__init__.py
+-rw-r--r--   0        0        0     4091 2023-07-06 14:40:19.988847 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/core/unit_test.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.989004 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/kernel/__init__.py
+-rw-r--r--   0        0        0    21480 2023-07-06 14:40:19.989244 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/kernel/kernel_test.py
+-rw-r--r--   0        0        0     3378 2023-07-06 14:40:19.989463 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/kernel/tick_test.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.989634 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/plugins/__init__.py
+-rw-r--r--   0        0        0     3176 2023-07-06 14:40:19.989812 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/plugins/actor_database_test.py
+-rw-r--r--   0        0        0     4729 2023-07-06 14:40:19.990071 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py
+-rw-r--r--   0        0        0     1963 2023-07-06 14:40:19.990259 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/plugins/authority_substrate_test.py
+-rw-r--r--   0        0        0     3263 2023-07-06 14:40:19.990435 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/plugins/substrate_database_test.py
+-rw-r--r--   0        0        0     2280 2023-07-06 14:40:19.991829 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/plugins/substrate_test_base.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.992082 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/__init__.py
+-rw-r--r--   0        0        0    21995 2023-07-06 14:40:19.992331 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py
+-rw-r--r--   0        0        0    23678 2023-07-06 14:40:19.992681 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py
+-rw-r--r--   0        0        0     4515 2023-07-06 14:40:19.993078 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py
+-rw-r--r--   0        0        0     1561 2023-07-06 14:40:19.993380 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py
+-rw-r--r--   0        0        0     8437 2023-07-06 14:40:19.993618 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/controller_test_wrapper.py
+-rw-r--r--   0        0        0     7719 2023-07-06 14:40:19.993823 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py
+-rw-r--r--   0        0        0     1586 2023-07-06 14:40:19.993986 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.994155 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/time/__init__.py
+-rw-r--r--   0        0        0     3786 2023-07-06 14:40:19.994406 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/time/actor_clock_test.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.994579 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/time/calendar/__init__.py
+-rw-r--r--   0        0        0     4290 2023-07-06 14:40:19.994779 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py
+-rw-r--r--   0        0        0     2225 2023-07-06 14:40:19.995009 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py
+-rw-r--r--   0        0        0    14887 2023-07-06 14:40:19.995232 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/time/term_test.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.995401 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/util/__init__.py
+-rw-r--r--   0        0        0     8041 2023-07-06 14:40:19.995626 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/util/reservation_holdings_test.py
+-rw-r--r--   0        0        0     5072 2023-07-06 14:40:19.995872 fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/util/reservation_list_test.py
+-rw-r--r--   0        0        0     3738 2023-07-06 14:40:19.996064 fabric_cf-1.6.2rc0/fabric_cf/actor/test/dummy_authority_proxy.py
+-rw-r--r--   0        0        0     1953 2023-07-06 14:40:19.996233 fabric_cf-1.6.2rc0/fabric_cf/actor/test/dummy_proxy.py
+-rw-r--r--   0        0        0     2498 2023-08-29 19:20:39.689504 fabric_cf-1.6.2rc0/fabric_cf/actor/test/fim_test_helper.py
+-rw-r--r--   0        0        0       92 2023-07-06 14:40:19.996635 fabric_cf-1.6.2rc0/fabric_cf/actor/test/schema/key.avsc
+-rw-r--r--   0        0        0    27389 2023-07-06 14:40:19.996847 fabric_cf-1.6.2rc0/fabric_cf/actor/test/schema/message.avsc
+-rw-r--r--   0        0        0     5358 2023-08-29 19:21:00.479457 fabric_cf-1.6.2rc0/fabric_cf/actor/test/test_abqm.py
+-rw-r--r--   0        0        0     1892 2023-07-06 14:40:19.997319 fabric_cf-1.6.2rc0/fabric_cf/actor/test/test_actor.py
+-rw-r--r--   0        0        0     1249 2023-07-06 14:40:19.997537 fabric_cf-1.6.2rc0/fabric_cf/actor/test/test_exception.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.997709 fabric_cf-1.6.2rc0/fabric_cf/aits/__init__.py
+-rw-r--r--   0        0        0     4826 2023-07-06 14:40:19.997962 fabric_cf-1.6.2rc0/fabric_cf/aits/config/config.broker.yaml
+-rw-r--r--   0        0        0     4808 2023-07-06 14:40:19.998148 fabric_cf-1.6.2rc0/fabric_cf/aits/config/config.netam.yaml
+-rw-r--r--   0        0        0     4414 2023-07-06 14:40:19.998315 fabric_cf-1.6.2rc0/fabric_cf/aits/config/config.orchestrator.yaml
+-rw-r--r--   0        0        0     4788 2023-07-06 14:40:19.998464 fabric_cf-1.6.2rc0/fabric_cf/aits/config/config.siteam.yaml
+-rw-r--r--   0        0        0    49220 2023-07-06 14:40:19.998792 fabric_cf-1.6.2rc0/fabric_cf/aits/integration_test.py
+-rw-r--r--   0        0        0     7393 2023-07-06 14:40:19.999015 fabric_cf-1.6.2rc0/fabric_cf/aits/kafka_processor.py
+-rw-r--r--   0        0        0     8633 2023-07-06 14:40:19.999246 fabric_cf-1.6.2rc0/fabric_cf/aits/manage_helper.py
+-rw-r--r--   0        0        0     8339 2023-07-06 14:40:19.999482 fabric_cf-1.6.2rc0/fabric_cf/aits/orchestrator_helper.py
+-rw-r--r--   0        0        0    16414 2024-01-22 16:38:27.654744 fabric_cf-1.6.2rc0/fabric_cf/authority/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:19.999946 fabric_cf-1.6.2rc0/fabric_cf/authority/__init__.py
+-rw-r--r--   0        0        0     2164 2023-07-06 14:40:20.000130 fabric_cf-1.6.2rc0/fabric_cf/authority/__main__.py
+-rw-r--r--   0        0        0     1503 2024-01-22 16:38:27.655589 fabric_cf-1.6.2rc0/fabric_cf/authority/al2s_handler_config.yml
+-rw-r--r--   0        0        0    32973 2023-07-06 14:40:20.000429 fabric_cf-1.6.2rc0/fabric_cf/authority/am-yes.xml
+-rw-r--r--   0        0        0     5125 2024-02-15 17:39:56.165295 fabric_cf-1.6.2rc0/fabric_cf/authority/config.al2s.am.yaml
+-rw-r--r--   0        0        0     5219 2024-02-15 17:39:56.165586 fabric_cf-1.6.2rc0/fabric_cf/authority/config.net.am.yaml
+-rw-r--r--   0        0        0     5589 2024-02-15 17:39:56.165822 fabric_cf-1.6.2rc0/fabric_cf/authority/config.site.am.geni.yaml
+-rw-r--r--   0        0        0     5083 2024-02-15 17:39:56.166190 fabric_cf-1.6.2rc0/fabric_cf/authority/config.site.am.yaml
+-rw-r--r--   0        0        0     3431 2024-01-22 16:38:27.660843 fabric_cf-1.6.2rc0/fabric_cf/authority/docker-compose.geni.yml
+-rw-r--r--   0        0        0     3340 2024-02-24 02:42:52.685976 fabric_cf-1.6.2rc0/fabric_cf/authority/docker-compose.yml
+-rw-r--r--   0        0        0     1191 2023-07-06 14:40:20.001777 fabric_cf-1.6.2rc0/fabric_cf/authority/env.template
+-rw-r--r--   0        0        0    16080 2023-07-06 14:40:20.001955 fabric_cf-1.6.2rc0/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml
+-rw-r--r--   0        0        0     1588 2023-07-06 14:40:20.002362 fabric_cf-1.6.2rc0/fabric_cf/authority/net_handler_config.yml
+-rw-r--r--   0        0        0     1523 2023-07-06 14:40:20.002545 fabric_cf-1.6.2rc0/fabric_cf/authority/oess_handler_config.yml
+-rw-r--r--   0        0        0     1380 2023-07-06 14:40:20.002705 fabric_cf-1.6.2rc0/fabric_cf/authority/pdp.xml
+-rwxr-xr-x   0        0        0     2446 2023-07-06 14:40:20.003053 fabric_cf-1.6.2rc0/fabric_cf/authority/setup.sh
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:20.003243 fabric_cf-1.6.2rc0/fabric_cf/authority/test/__init__.py
+-rw-r--r--   0        0        0     2463 2023-07-06 14:40:20.003608 fabric_cf-1.6.2rc0/fabric_cf/authority/test/al2s_am.py
+-rw-r--r--   0        0        0     2459 2023-07-06 14:40:20.003800 fabric_cf-1.6.2rc0/fabric_cf/authority/test/net_am.py
+-rw-r--r--   0        0        0     2456 2023-07-06 14:40:20.004030 fabric_cf-1.6.2rc0/fabric_cf/authority/test/site_am.py
+-rw-r--r--   0        0        0     2461 2023-07-06 14:40:20.004325 fabric_cf-1.6.2rc0/fabric_cf/authority/test/site_am_geni.py
+-rw-r--r--   0        0        0     4834 2024-02-15 17:39:56.167061 fabric_cf-1.6.2rc0/fabric_cf/authority/test/test-al2sam.yaml
+-rw-r--r--   0        0        0     4944 2024-02-15 17:39:56.167727 fabric_cf-1.6.2rc0/fabric_cf/authority/test/test-netam.yaml
+-rw-r--r--   0        0        0     5175 2024-02-15 17:39:56.168748 fabric_cf-1.6.2rc0/fabric_cf/authority/test/test.geni.yaml
+-rw-r--r--   0        0        0     4761 2024-02-15 17:39:56.169733 fabric_cf-1.6.2rc0/fabric_cf/authority/test/test.yaml
+-rw-r--r--   0        0        0     3189 2024-01-22 16:38:27.668968 fabric_cf-1.6.2rc0/fabric_cf/authority/vm_handler_config.yml
+-rw-r--r--   0        0        0     1448 2023-07-06 14:40:20.005355 fabric_cf-1.6.2rc0/fabric_cf/authority/vnic_net_handler_config.yml
+-rw-r--r--   0        0        0    14262 2023-07-06 14:40:20.005654 fabric_cf-1.6.2rc0/fabric_cf/broker/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:20.005739 fabric_cf-1.6.2rc0/fabric_cf/broker/__init__.py
+-rw-r--r--   0        0        0     2290 2023-07-06 14:40:20.005953 fabric_cf-1.6.2rc0/fabric_cf/broker/__main__.py
+-rw-r--r--   0        0        0    27944 2023-07-06 14:40:20.006218 fabric_cf-1.6.2rc0/fabric_cf/broker/broker-yes.xml
+-rw-r--r--   0        0        0     5222 2024-02-15 17:39:56.170241 fabric_cf-1.6.2rc0/fabric_cf/broker/config.broker.yaml
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:20.006704 fabric_cf-1.6.2rc0/fabric_cf/broker/core/__init__.py
+-rw-r--r--   0        0        0     3314 2023-07-06 14:40:20.006887 fabric_cf-1.6.2rc0/fabric_cf/broker/core/broker_kernel.py
+-rw-r--r--   0        0        0     3139 2024-02-24 02:42:45.493292 fabric_cf-1.6.2rc0/fabric_cf/broker/docker-compose.yml
+-rw-r--r--   0        0        0     1195 2023-07-06 14:40:20.007248 fabric_cf-1.6.2rc0/fabric_cf/broker/env.template
+-rw-r--r--   0        0        0    16080 2023-07-06 14:40:20.007412 fabric_cf-1.6.2rc0/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml
+-rw-r--r--   0        0        0     1380 2023-07-06 14:40:20.007566 fabric_cf-1.6.2rc0/fabric_cf/broker/pdp.xml
+-rwxr-xr-x   0        0        0     2239 2023-07-06 14:40:20.007731 fabric_cf-1.6.2rc0/fabric_cf/broker/setup.sh
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:20.007889 fabric_cf-1.6.2rc0/fabric_cf/broker/test/__init__.py
+-rw-r--r--   0        0        0     2507 2023-07-06 14:40:20.008088 fabric_cf-1.6.2rc0/fabric_cf/broker/test/broker.py
+-rw-r--r--   0        0        0     5236 2024-02-15 17:39:56.172112 fabric_cf-1.6.2rc0/fabric_cf/broker/test/test.yaml
+-rw-r--r--   0        0        0    20305 2023-07-06 14:40:20.008659 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:20.008780 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0        0        0     3355 2023-07-06 14:40:20.008979 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/__main__.py
+-rw-r--r--   0        0        0     1757 2023-07-06 14:40:20.009241 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/certs/fullchain.pem
+-rw-r--r--   0        0        0     3272 2023-07-06 14:40:20.009402 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/certs/privkey.pem
+-rw-r--r--   0        0        0     5088 2024-02-19 14:44:58.098651 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/config.orchestrator.yaml
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:20.009701 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/__init__.py
+-rw-r--r--   0        0        0     3026 2024-02-15 17:39:56.173873 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/active_status_checker.py
+-rw-r--r--   0        0        0     3247 2023-07-12 19:30:09.758686 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/bqm_wrapper.py
+-rw-r--r--   0        0        0     1556 2023-07-06 14:40:20.010274 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/exceptions.py
+-rw-r--r--   0        0        0     1884 2023-07-06 14:40:20.010462 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/i_status_update_callback.py
+-rw-r--r--   0        0        0    46479 2024-02-19 14:44:58.099723 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/orchestrator_handler.py
+-rw-r--r--   0        0        0     7423 2023-07-12 19:30:09.758992 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/orchestrator_kernel.py
+-rw-r--r--   0        0        0    36011 2024-01-22 16:38:27.673275 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py
+-rw-r--r--   0        0        0     3581 2023-07-06 14:40:20.011490 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/reservation_converter.py
+-rw-r--r--   0        0        0     4880 2023-07-06 14:40:20.011649 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/reservation_status_update.py
+-rw-r--r--   0        0        0     7876 2023-07-06 14:40:20.011878 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/reservation_status_update_thread.py
+-rw-r--r--   0        0        0     7219 2023-07-06 14:40:20.012054 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/response_builder.py
+-rw-r--r--   0        0        0     8722 2023-07-06 14:40:20.012245 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/slice_defer_thread.py
+-rw-r--r--   0        0        0     1972 2023-07-06 14:40:20.012433 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/status_checker.py
+-rw-r--r--   0        0        0     1581 2023-07-06 14:40:20.012642 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/watch_entry.py
+-rw-r--r--   0        0        0     3505 2024-02-24 02:43:00.047016 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/docker-compose.yml
+-rw-r--r--   0        0        0     1201 2023-07-06 14:40:20.012989 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/env.template
+-rw-r--r--   0        0        0    74275 2024-01-22 16:38:27.676544 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml
+-rw-r--r--   0        0        0     1626 2023-07-06 14:40:20.013737 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/nginx/default.conf
+-rw-r--r--   0        0        0    64528 2024-01-22 16:38:27.677758 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/openapi.json
+-rw-r--r--   0        0        0    30829 2023-07-06 14:40:20.014329 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/orchestrator-yes.xml
+-rw-r--r--   0        0        0     1548 2023-07-06 14:40:20.014528 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/pdp.xml
+-rwxr-xr-x   0        0        0     2284 2023-07-06 14:40:20.014684 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/setup.sh
+-rw-r--r--   0        0        0      430 2023-07-21 13:05:26.706807 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/__init__.py
+-rw-r--r--   0        0        0      392 2023-07-21 13:05:26.712379 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:05:26.687107 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/controllers/__init__.py
+-rw-r--r--   0        0        0      309 2024-01-22 16:38:27.678841 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/controllers/authorization_controller.py
+-rw-r--r--   0        0        0     1948 2024-01-22 16:38:27.680272 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/controllers/poas_controller.py
+-rw-r--r--   0        0        0     1249 2023-07-21 14:27:27.362230 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py
+-rw-r--r--   0        0        0     7375 2024-01-22 16:38:27.681314 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py
+-rw-r--r--   0        0        0     1094 2023-07-21 14:27:53.536237 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py
+-rw-r--r--   0        0        0      305 2023-07-21 14:28:03.310778 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/controllers/version_controller.py
+-rw-r--r--   0        0        0      631 2023-07-21 13:05:26.686191 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/encoder.py
+-rw-r--r--   0        0        0     2849 2024-01-22 16:38:27.682326 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/__init__.py
+-rw-r--r--   0        0        0     1889 2023-07-21 13:05:26.681811 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/base_model_.py
+-rw-r--r--   0        0        0     3400 2023-07-21 13:05:26.678341 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/poa.py
+-rw-r--r--   0        0        0     5315 2023-07-21 13:05:26.685259 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/poa_data.py
+-rw-r--r--   0        0        0     2647 2024-01-22 16:38:27.683283 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/poa_post.py
+-rw-r--r--   0        0        0     3539 2024-01-22 16:38:27.684009 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/poa_post_data.py
+-rw-r--r--   0        0        0     2458 2024-01-22 16:38:27.684893 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/poa_post_data_keys.py
+-rw-r--r--   0        0        0     2484 2024-01-22 16:38:27.685792 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     1628 2023-07-21 13:05:26.679846 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/resource.py
+-rw-r--r--   0        0        0     3564 2023-07-21 13:05:26.682401 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/resources.py
+-rw-r--r--   0        0        0     7311 2023-07-21 13:05:26.678076 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/slice.py
+-rw-r--r--   0        0        0     3616 2023-07-21 13:05:26.675485 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/slice_details.py
+-rw-r--r--   0        0        0     5251 2023-07-21 13:05:26.683801 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/slices.py
+-rw-r--r--   0        0        0     2634 2023-07-21 13:05:26.682083 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/slices_post.py
+-rw-r--r--   0        0        0     8995 2023-07-21 13:05:26.685624 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/sliver.py
+-rw-r--r--   0        0        0     5301 2023-07-21 13:05:26.683526 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/slivers.py
+-rw-r--r--   0        0        0     3896 2023-07-21 13:05:26.684094 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     2464 2023-07-21 13:05:26.678890 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     4929 2023-07-21 13:05:26.681517 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     2870 2023-07-21 13:05:26.680712 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py
+-rw-r--r--   0        0        0     1983 2023-07-21 13:05:26.681255 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py
+-rw-r--r--   0        0        0     4503 2023-07-21 13:05:26.684376 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     3984 2023-07-21 13:05:26.683221 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     2512 2023-07-21 13:05:26.675987 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     3879 2023-07-21 13:05:26.682775 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py
+-rw-r--r--   0        0        0     2461 2023-07-21 13:05:26.679526 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     3846 2023-07-21 13:05:26.680992 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py
+-rw-r--r--   0        0        0     2446 2023-07-21 13:05:26.684653 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     4233 2023-07-21 13:05:26.679207 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     2635 2023-07-21 13:05:26.677106 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3540 2023-07-21 13:05:26.677698 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/version.py
+-rw-r--r--   0        0        0     2536 2023-07-21 13:05:26.677423 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/version_data.py
+-rw-r--r--   0        0        0        0 2023-07-21 13:05:26.696979 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/__init__.py
+-rw-r--r--   0        0        0     1355 2023-07-21 14:26:34.212959 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py
+-rw-r--r--   0        0        0     1997 2023-07-21 13:05:26.696810 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/constants.py
+-rw-r--r--   0        0        0     5537 2023-07-21 13:05:26.696497 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/cors_response.py
+-rw-r--r--   0        0        0     5471 2024-01-22 16:38:27.686829 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/poas_controller.py
+-rw-r--r--   0        0        0     4321 2023-07-21 13:05:26.703189 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/resources_controller.py
+-rw-r--r--   0        0        0    15437 2023-07-21 13:05:26.701619 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/slices_controller.py
+-rw-r--r--   0        0        0     4642 2023-07-21 13:05:26.702268 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py
+-rw-r--r--   0        0        0     2530 2023-07-21 13:05:26.701151 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/utils.py
+-rw-r--r--   0        0        0     2632 2023-07-21 13:05:26.702831 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/version_controller.py
+-rw-r--r--   0        0        0    46662 2024-01-22 16:38:27.688350 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml
+-rw-r--r--   0        0        0      438 2023-07-21 13:05:26.672917 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/test/__init__.py
+-rw-r--r--   0        0        0     2531 2023-07-21 13:16:16.850784 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/test/test_poas_controller.py
+-rw-r--r--   0        0        0     2094 2023-07-21 13:16:26.523105 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py
+-rw-r--r--   0        0        0     5917 2023-07-21 13:16:33.995263 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py
+-rw-r--r--   0        0        0     1989 2023-07-21 13:16:44.547066 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py
+-rw-r--r--   0        0        0      855 2023-07-21 13:16:53.155233 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py
+-rw-r--r--   0        0        0      809 2023-07-21 13:05:26.686486 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/type_util.py
+-rw-r--r--   0        0        0     3452 2023-07-21 13:05:26.674386 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/util.py
+-rw-r--r--   0        0        0        0 2023-07-06 14:40:20.026771 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/test/__init__.py
+-rw-r--r--   0        0        0     3542 2023-07-06 14:40:20.026956 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/test/orchestrator.py
+-rwxr-xr-x   0        0        0       78 2023-07-06 14:40:20.027092 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/test/test.sh
+-rw-r--r--   0        0        0     4560 2024-02-15 17:39:56.176013 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/test/test.yaml
+-rwxr-xr-x   0        0        0     2900 2023-07-06 14:40:20.027470 fabric_cf-1.6.2rc0/fabric_cf/orchestrator/update_swagger_stub.sh
+-rw-r--r--   0        0        0    18177 2023-07-06 14:40:20.027906 fabric_cf-1.6.2rc0/images/am-pod.png
+-rw-r--r--   0        0        0    74927 2023-07-06 14:40:20.028627 fabric_cf-1.6.2rc0/images/am.png
+-rw-r--r--   0        0        0    18471 2023-07-06 14:40:20.028960 fabric_cf-1.6.2rc0/images/broker-pod.png
+-rw-r--r--   0        0        0    73799 2023-07-06 14:40:20.029590 fabric_cf-1.6.2rc0/images/broker.png
+-rw-r--r--   0        0        0    90831 2023-07-06 14:40:20.030329 fabric_cf-1.6.2rc0/images/cf.png
+-rw-r--r--   0        0        0    19611 2023-07-06 14:40:20.030664 fabric_cf-1.6.2rc0/images/orchestrator-pod.png
+-rw-r--r--   0        0        0    78622 2023-07-06 14:40:20.031328 fabric_cf-1.6.2rc0/images/orchestrator.png
+-rw-r--r--   0        0        0    14808 2023-07-06 14:40:20.040989 fabric_cf-1.6.2rc0/neo4j/abqm.graphml
+-rw-r--r--   0        0        0     1757 2023-07-06 14:40:20.041291 fabric_cf-1.6.2rc0/neo4j/certs/fullchain.pem
+-rw-r--r--   0        0        0     3272 2023-07-06 14:40:20.041462 fabric_cf-1.6.2rc0/neo4j/certs/privkey.pem
+-rwxr-xr-x   0        0        0       91 2023-07-06 14:40:20.041625 fabric_cf-1.6.2rc0/orchestrator.sh
+-rw-r--r--   0        0        0      980 2024-02-15 17:39:56.177452 fabric_cf-1.6.2rc0/psql.upgrade
+-rw-r--r--   0        0        0     1317 2024-02-15 17:39:56.178227 fabric_cf-1.6.2rc0/pyproject.toml
+-rwxr-xr-x   0        0        0     2594 2023-07-06 14:40:20.042295 fabric_cf-1.6.2rc0/secrets/create-certs.sh
+-rw-r--r--   0        0        0    12796 2023-07-06 14:40:20.042623 fabric_cf-1.6.2rc0/tools/audit.py
+-rw-r--r--   0        0        0     9897 2024-02-15 17:39:56.179350 fabric_cf-1.6.2rc0/tools/db_cli.py
+-rw-r--r--   0        0        0      357 2024-02-15 17:39:56.180113 fabric_cf-1.6.2rc0/tools/install.sh
+-rw-r--r--   0        0        0      143 2023-07-06 14:40:20.043220 fabric_cf-1.6.2rc0/tox.ini
+-rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 fabric_cf-1.6.2rc0/PKG-INFO
```

### Comparing `fabric_cf-1.6.2/.gitignore` & `fabric_cf-1.6.2rc0/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/Dockerfile-auth` & `fabric_cf-1.6.2rc0/Dockerfile-auth`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/Dockerfile-broker` & `fabric_cf-1.6.2rc0/Dockerfile-broker`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/Dockerfile-cf` & `fabric_cf-1.6.2rc0/Dockerfile-cf`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/Dockerfile-orchestrator` & `fabric_cf-1.6.2rc0/Dockerfile-orchestrator`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/LICENSE` & `fabric_cf-1.6.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/README.md` & `fabric_cf-1.6.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/cleanup_old_schema_from_schema_registry.sh` & `fabric_cf-1.6.2rc0/cleanup_old_schema_from_schema_registry.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/docker-compose-kafka.yaml` & `fabric_cf-1.6.2rc0/docker-compose-kafka.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/docker-compose-no-ssl-kafka.yaml` & `fabric_cf-1.6.2rc0/docker-compose-no-ssl-kafka.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/docker-compose-test.yaml` & `fabric_cf-1.6.2rc0/docker-compose-test.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/env.template.test` & `fabric_cf-1.6.2rc0/env.template.test`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabricNo.AnyActorNoPolicy.xml` & `fabric_cf-1.6.2rc0/fabricNo.AnyActorNoPolicy.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/Design.md` & `fabric_cf-1.6.2rc0/fabric_cf/Design.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/boot/configuration.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/boot/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/boot/configuration_exception.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/boot/configuration_exception.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/boot/configuration_loader.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/boot/configuration_loader.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/boot/configuration_processor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/boot/configuration_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_container.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_event.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_identity.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_identity.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_management_object.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_mixin.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_actor_runnable.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_actor_runnable.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_authority.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_authority_policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_authority_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_authority_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_authority_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_authority_reservation.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_authority_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_base_plugin.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_base_plugin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_broker_mixin.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_broker_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_broker_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_broker_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_broker_reservation.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_broker_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_callback_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_callback_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_client_actor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_client_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_client_actor_management_object.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_client_actor_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_client_callback_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_client_callback_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_client_policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_client_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_client_reservation.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_client_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_component.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_component.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_concrete_set.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_concrete_set.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_container_clock.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_container_clock.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_container_database.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_container_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_controller_policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_controller_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_controller_reservation.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_controller_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_database.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_delegation.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_delegation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_event.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_management_object.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_actor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_authority.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_container.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_proxy_factory.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_query_response_handler.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_query_response_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_reservation_mixin.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_reservation_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_reservation_resources.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_reservation_resources.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_reservation_status.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_reservation_status.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_resource_control.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_resource_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_response_handler.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_response_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_rpc_request_state.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_rpc_request_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_server_actor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_server_policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_server_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_server_reservation.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_server_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_slice.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_slice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_substrate.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_substrate.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_substrate_database.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_substrate_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_tick.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_tick.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_ticker.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_ticker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_timer_queue.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_timer_queue.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/apis/abc_timer_task.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/apis/abc_timer_task.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/common/constants.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/common/constants.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/common/event_logger.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/common/event_logger.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/common/exceptions.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/common/resource_config.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/common/resource_config.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/container/container.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/container/db/container_database.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/db/container_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/container/globals.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/globals.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/container/maintenance.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/maintenance.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/container/message_service.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/message_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/container/protocol_descriptor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/protocol_descriptor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/container/remote_actor_cache.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/remote_actor_cache.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/container/rpc_consumer.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/rpc_consumer.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/container/rpc_producer.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/container/rpc_producer.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/actor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/actor_identity.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/actor_identity.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/authority.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/authority_policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/authority_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/broker.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/broker_policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/broker_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/event_processor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/event_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/inventory_slice_manager.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/inventory_slice_manager.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/rpc_request_state.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/rpc_request_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/ticket.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/ticket.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/unit.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/unit.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/core/unit_set.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/core/unit_set.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/delegation/broker_delegation.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/delegation/broker_delegation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/delegation/broker_delegation_factory.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/delegation/broker_delegation_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/delegation/delegation.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/delegation/delegation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/delegation/delegation_factory.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/delegation/delegation_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/delegation/resource_ticket.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/delegation/resource_ticket.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/authority_reservation.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/authority_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/broker_query_model_publisher.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/broker_query_model_publisher.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/broker_reservation.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/broker_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/claim_timeout.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/claim_timeout.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/failed_rpc.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/failed_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/failed_rpc_event.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/failed_rpc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_failed_rpc.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_failed_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_poa_rpc.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_poa_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_query_rpc.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_query_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_rpc.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/incoming_rpc_event.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/incoming_rpc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/kernel.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/kernel_tick.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/kernel_tick.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/kernel_wrapper.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/kernel_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/poa.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/poa.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/predecessor_state.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/predecessor_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/query_timeout.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/query_timeout.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/request_types.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/request_types.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/reservation.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/reservation_client.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/reservation_client.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/reservation_server.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/reservation_server.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/reservation_states.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/reservation_states.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/resource_set.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/resource_set.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/retry_rpc.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/retry_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/retry_rpc_event.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/retry_rpc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/rpc_executor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/rpc_executor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/rpc_manager.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/rpc_manager.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/rpc_manager_singleton.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/rpc_manager_singleton.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/rpc_request.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/rpc_request.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/rpc_request_type.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/rpc_request_type.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/sequence_comparison_codes.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/sequence_comparison_codes.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/slice.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/slice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/slice_state_machine.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/slice_state_machine.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/slice_table.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/slice_table.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/kernel/tick.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/kernel/tick.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/actor_management_object.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/actor_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/authority_management_object.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/authority_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/broker_management_object.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/broker_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/client_actor_management_object_helper.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/client_actor_management_object_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/container_management_object.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/container_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/controller_management_object.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/controller_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/converter.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/converter.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/error.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/error.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_actor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_authority.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_broker.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_container.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/kafka/services/kafka_service.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/kafka/services/kafka_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_actor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_authority.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_broker.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_container.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/local/local_server_actor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/local/local_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/management_object.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/management_object_manager.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/management_object_manager.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/management_utils.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/management_utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/messages/client_mng.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/messages/client_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/messages/event_mng.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/messages/event_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/messages/result_client_mng.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/messages/result_client_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/messages/result_event_mng.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/messages/result_event_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/manage/server_actor_management_object.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/manage/server_actor_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/plugins/base_plugin.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/plugins/db/actor_database.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/db/actor_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/plugins/db/client_database.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/db/client_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/plugins/db/server_actor_database.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/db/server_actor_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/plugins/handlers/config_token.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/handlers/config_token.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/plugins/handlers/handler_processor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/handlers/handler_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/plugins/substrate/authority_substrate.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/substrate/authority_substrate.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/authority_calendar_policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/authority_calendar_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/broker_calendar_policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/broker_calendar_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/broker_simpler_units_policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/broker_simpler_units_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/controller_calendar_policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/controller_calendar_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/controller_simple_policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/controller_simple_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/controller_ticket_review_policy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/controller_ticket_review_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/fifo_queue.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/fifo_queue.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/inventory.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/inventory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/inventory_for_type.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/inventory_for_type.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/network_node_control.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/network_node_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/network_node_inventory.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/network_node_inventory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/network_service_control.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/network_service_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/network_service_inventory.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/network_service_inventory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/queue_wrapper.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/policy/resource_control.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/policy/resource_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/actor_location.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/actor_location.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/kafka_retun.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/kafka_retun.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/services/actor_service.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/services/actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/services/authority_service.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/services/authority_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/services/broker_service.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/services/broker_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/services/controller_service.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/services/controller_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/kafka/translate.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/kafka/translate.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/local/local_authority.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/local/local_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/local/local_broker.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/local/local_broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/local/local_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/local/local_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/local/local_proxy_factory.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/local/local_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/local/local_return.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/local/local_return.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/proxies/proxy_factory.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/proxies/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/registry/actor_registry.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/registry/actor_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/registry/callback_registry.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/registry/callback_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/registry/peer_registry.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/registry/peer_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/registry/proxy_registry.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/registry/proxy_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/time/actor_clock.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/actor_clock.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/time/calendar/authority_calendar.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/calendar/authority_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/time/calendar/base_calendar.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/calendar/base_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/time/calendar/broker_calendar.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/calendar/broker_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/time/calendar/client_calendar.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/calendar/client_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/time/calendar/controller_calendar.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/calendar/controller_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/time/calendar/source_calendar.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/calendar/source_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/time/term.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/time/term.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/bids.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/bids.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/client.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/client.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/graceful_interrupt_handler.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/graceful_interrupt_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/id.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/id.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/iterable_queue.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/iterable_queue.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/kernel_timer.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/kernel_timer.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/log_helper.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/log_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/notice.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/notice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/reflection_utils.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/reflection_utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/reservation_holdings.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/reservation_holdings.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/reservation_list.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/reservation_list.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/reservation_set.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/reservation_set.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/reservation_state.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/reservation_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/resource_type.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/resource_type.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/rpc_exception.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/rpc_exception.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/update_data.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/update_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/core/util/utils.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/core/util/utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/db/__init__.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/db/psql_database.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/db/psql_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/fim/asm_update_thread.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/fim/asm_update_thread.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/fim/fim_helper.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/fim/fim_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/handlers/handler_base.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/handlers/handler_base.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/handlers/no_op_handler.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/handlers/no_op_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/security/access_checker.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/security/access_checker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/security/auth_token.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/security/auth_token.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/security/fabric_token.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/security/fabric_token.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/security/pdp_auth.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/security/pdp_auth.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/security/token_validator.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/security/token_validator.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/base_test_case.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/client_callback_helper.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/client_callback_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/config/config.jenkins.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/config/config.jenkins.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/config/config.orchestrator.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/config/config.orchestrator.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/config/config.test.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/config/config.test.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/controller_callback_helper.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/controller_callback_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/container/container_database_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/container/container_database_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/core/unit_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/core/unit_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/kernel/kernel_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/kernel/kernel_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/kernel/tick_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/kernel/tick_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/plugins/actor_database_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/plugins/actor_database_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/plugins/authority_substrate_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/plugins/authority_substrate_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/plugins/substrate_database_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/plugins/substrate_database_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/plugins/substrate_test_base.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/plugins/substrate_test_base.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/controller_test_wrapper.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/controller_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/time/actor_clock_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/time/actor_clock_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/time/term_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/time/term_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/util/reservation_holdings_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/util/reservation_holdings_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/core/util/reservation_list_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/core/util/reservation_list_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/dummy_authority_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/dummy_authority_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/dummy_proxy.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/dummy_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/fim_test_helper.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/fim_test_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/schema/message.avsc` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/schema/message.avsc`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/test_abqm.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/test_abqm.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/test_actor.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/test_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/actor/test/test_exception.py` & `fabric_cf-1.6.2rc0/fabric_cf/actor/test/test_exception.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/aits/config/config.broker.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/aits/config/config.broker.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/aits/config/config.netam.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/aits/config/config.netam.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/aits/config/config.orchestrator.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/aits/config/config.orchestrator.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/aits/config/config.siteam.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/aits/config/config.siteam.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/aits/integration_test.py` & `fabric_cf-1.6.2rc0/fabric_cf/aits/integration_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/aits/kafka_processor.py` & `fabric_cf-1.6.2rc0/fabric_cf/aits/kafka_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/aits/manage_helper.py` & `fabric_cf-1.6.2rc0/fabric_cf/aits/manage_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/aits/orchestrator_helper.py` & `fabric_cf-1.6.2rc0/fabric_cf/aits/orchestrator_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/Readme.md` & `fabric_cf-1.6.2rc0/fabric_cf/authority/Readme.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/__main__.py` & `fabric_cf-1.6.2rc0/fabric_cf/authority/__main__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/al2s_handler_config.yml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/al2s_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/am-yes.xml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/am-yes.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/config.al2s.am.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/config.al2s.am.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/config.net.am.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/config.net.am.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/config.site.am.geni.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/config.site.am.geni.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/config.site.am.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/config.site.am.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/docker-compose.geni.yml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/docker-compose.geni.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/docker-compose.yml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/env.template` & `fabric_cf-1.6.2rc0/fabric_cf/authority/env.template`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/net_handler_config.yml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/net_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/oess_handler_config.yml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/oess_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/pdp.xml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/pdp.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/setup.sh` & `fabric_cf-1.6.2rc0/fabric_cf/authority/setup.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/test/al2s_am.py` & `fabric_cf-1.6.2rc0/fabric_cf/authority/test/al2s_am.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/test/net_am.py` & `fabric_cf-1.6.2rc0/fabric_cf/authority/test/net_am.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/test/site_am.py` & `fabric_cf-1.6.2rc0/fabric_cf/authority/test/site_am.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/test/site_am_geni.py` & `fabric_cf-1.6.2rc0/fabric_cf/authority/test/site_am_geni.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/test/test-al2sam.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/test/test-al2sam.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/test/test-netam.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/test/test-netam.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/test/test.geni.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/test/test.geni.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/test/test.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/test/test.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/vm_handler_config.yml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/vm_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/authority/vnic_net_handler_config.yml` & `fabric_cf-1.6.2rc0/fabric_cf/authority/vnic_net_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/broker/Readme.md` & `fabric_cf-1.6.2rc0/fabric_cf/broker/Readme.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/broker/__main__.py` & `fabric_cf-1.6.2rc0/fabric_cf/broker/__main__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/broker/broker-yes.xml` & `fabric_cf-1.6.2rc0/fabric_cf/broker/broker-yes.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/broker/config.broker.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/broker/config.broker.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/broker/core/broker_kernel.py` & `fabric_cf-1.6.2rc0/fabric_cf/broker/core/broker_kernel.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/broker/docker-compose.yml` & `fabric_cf-1.6.2rc0/fabric_cf/broker/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/broker/env.template` & `fabric_cf-1.6.2rc0/fabric_cf/broker/env.template`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml` & `fabric_cf-1.6.2rc0/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/broker/pdp.xml` & `fabric_cf-1.6.2rc0/fabric_cf/broker/pdp.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/broker/setup.sh` & `fabric_cf-1.6.2rc0/fabric_cf/broker/setup.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/broker/test/broker.py` & `fabric_cf-1.6.2rc0/fabric_cf/broker/test/broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/broker/test/test.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/broker/test/test.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/README.md` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/README.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/__main__.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/__main__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/certs/fullchain.pem` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/certs/fullchain.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/certs/privkey.pem` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/certs/privkey.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/config.orchestrator.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/config.orchestrator.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/active_status_checker.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/active_status_checker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/bqm_wrapper.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/bqm_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/exceptions.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/i_status_update_callback.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/i_status_update_callback.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/orchestrator_handler.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/orchestrator_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/orchestrator_kernel.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/orchestrator_kernel.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/reservation_converter.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/reservation_converter.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/reservation_status_update.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/reservation_status_update.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/reservation_status_update_thread.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/reservation_status_update_thread.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/response_builder.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/response_builder.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/slice_defer_thread.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/slice_defer_thread.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/status_checker.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/status_checker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/core/watch_entry.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/core/watch_entry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/docker-compose.yml` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/env.template` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/env.template`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/nginx/default.conf` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/nginx/default.conf`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/openapi.json` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/openapi.json`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/orchestrator-yes.xml` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/orchestrator-yes.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/pdp.xml` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/pdp.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/setup.sh` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/setup.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/controllers/poas_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/controllers/poas_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/encoder.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/encoder.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/__init__.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/base_model_.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/poa.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/poa.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/poa_data.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/poa_post.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/poa_post.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/poa_post_data.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/poa_post_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/poa_post_data_keys.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/poa_post_data_keys.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/poa_post_data_vcpu_cpu_map.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/poa_post_data_vcpu_cpu_map.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/resource.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/resources.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/slice.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/slice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/slice_details.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/slices.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/slices_post.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/sliver.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/sliver.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/slivers.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/version.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/models/version_data.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/constants.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/constants.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/cors_response.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/cors_response.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/poas_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/poas_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/resources_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/resources_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/slices_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/slices_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/utils.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/response/version_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/response/version_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/test/test_poas_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/test/test_poas_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/type_util.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/type_util.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/swagger_server/util.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/swagger_server/util.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/test/orchestrator.py` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/test/orchestrator.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/test/test.yaml` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/test/test.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/fabric_cf/orchestrator/update_swagger_stub.sh` & `fabric_cf-1.6.2rc0/fabric_cf/orchestrator/update_swagger_stub.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/images/am-pod.png` & `fabric_cf-1.6.2rc0/images/am-pod.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/images/am.png` & `fabric_cf-1.6.2rc0/images/am.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/images/broker-pod.png` & `fabric_cf-1.6.2rc0/images/broker-pod.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/images/broker.png` & `fabric_cf-1.6.2rc0/images/broker.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/images/cf.png` & `fabric_cf-1.6.2rc0/images/cf.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/images/orchestrator-pod.png` & `fabric_cf-1.6.2rc0/images/orchestrator-pod.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/images/orchestrator.png` & `fabric_cf-1.6.2rc0/images/orchestrator.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/neo4j/abqm.graphml` & `fabric_cf-1.6.2rc0/neo4j/abqm.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/neo4j/certs/fullchain.pem` & `fabric_cf-1.6.2rc0/neo4j/certs/fullchain.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/neo4j/certs/privkey.pem` & `fabric_cf-1.6.2rc0/neo4j/certs/privkey.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/psql.upgrade` & `fabric_cf-1.6.2rc0/psql.upgrade`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/pyproject.toml` & `fabric_cf-1.6.2rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/secrets/create-certs.sh` & `fabric_cf-1.6.2rc0/secrets/create-certs.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/tools/audit.py` & `fabric_cf-1.6.2rc0/tools/audit.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/tools/db_cli.py` & `fabric_cf-1.6.2rc0/tools/db_cli.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.6.2/PKG-INFO` & `fabric_cf-1.6.2rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric_cf
-Version: 1.6.2
+Version: 1.6.2rc0
 Summary: Fabric Control Framework
 Keywords: Swagger,Fabric Control Framework
 Author-email: Komal Thareja <kthare10@renci.org>, Ilya Baldin <ibaldin@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

