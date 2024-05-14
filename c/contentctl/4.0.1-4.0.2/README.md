# Comparing `tmp/contentctl-4.0.1.tar.gz` & `tmp/contentctl-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contentctl-4.0.1.tar", max compression
+gzip compressed data, was "contentctl-4.0.2.tar", max compression
```

## Comparing `contentctl-4.0.1.tar` & `contentctl-4.0.2.tar`

### file list

```diff
@@ -1,167 +1,167 @@
--rw-r--r--   0        0        0    11344 2024-05-07 02:00:52.753300 contentctl-4.0.1/LICENSE.md
--rw-r--r--   0        0        0    18472 2024-05-07 02:00:52.753300 contentctl-4.0.1/README.md
--rw-r--r--   0        0        0       22 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/__init__.py
--rw-r--r--   0        0        0     1418 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/acs_deploy.py
--rw-r--r--   0        0        0     2999 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/apav_deploy.py
--rw-r--r--   0        0        0     6965 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/api_deploy.py
--rw-r--r--   0        0        0     4765 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/build.py
--rw-r--r--   0        0        0      704 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/convert.py
--rw-r--r--   0        0        0     8818 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/DetectionTestingManager.py
--rw-r--r--   0        0        0     8666 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/GitService.py
--rw-r--r--   0        0        0     2259 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
--rw-r--r--   0        0        0    53141 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
--rw-r--r--   0        0        0     6846 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
--rw-r--r--   0        0        0      370 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
--rw-r--r--   0        0        0     3244 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/progress_bar.py
--rw-r--r--   0        0        0     7013 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingView.py
--rw-r--r--   0        0        0     2050 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
--rw-r--r--   0        0        0     1123 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
--rw-r--r--   0        0        0     4706 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
--rw-r--r--   0        0        0      863 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/doc_gen.py
--rw-r--r--   0        0        0     1749 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/initialize.py
--rw-r--r--   0        0        0     9333 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/initialize_old.py
--rw-r--r--   0        0        0    12628 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/inspect.py
--rw-r--r--   0        0        0     5792 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/new_content.py
--rw-r--r--   0        0        0    13115 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/release_notes.py
--rw-r--r--   0        0        0     1583 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/reporting.py
--rw-r--r--   0        0        0     4896 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/test.py
--rw-r--r--   0        0        0     2363 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/actions/validate.py
--rw-r--r--   0        0        0    10083 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/contentctl.py
--rw-r--r--   0        0        0     6732 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/enrichments/attack_enrichment.py
--rw-r--r--   0        0        0     3934 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/enrichments/cve_enrichment.py
--rw-r--r--   0        0        0     3418 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/enrichments/splunk_app_enrichment.py
--rw-r--r--   0        0        0     7139 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/helper/link_validator.py
--rw-r--r--   0        0        0        0 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/helper/logger.py
--rw-r--r--   0        0        0    15659 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/helper/utils.py
--rw-r--r--   0        0        0     5861 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/input/backend_splunk_ba.py
--rw-r--r--   0        0        0    10716 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/input/director.py
--rw-r--r--   0        0        0     5718 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/input/new_content_questions.py
--rw-r--r--   0        0        0    19391 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/input/sigma_converter.py
--rw-r--r--   0        0        0     8377 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/input/ssa_detection_builder.py
--rw-r--r--   0        0        0     1475 2024-05-07 02:00:52.753300 contentctl-4.0.1/contentctl/input/yml_reader.py
--rw-r--r--   0        0        0    30167 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/abstract_security_content_objects/detection_abstract.py
--rw-r--r--   0        0        0     8065 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py
--rw-r--r--   0        0        0     1335 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/alert_action.py
--rw-r--r--   0        0        0     8979 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/atomic.py
--rw-r--r--   0        0        0     1028 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/base_test.py
--rw-r--r--   0        0        0     4752 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/base_test_result.py
--rw-r--r--   0        0        0     2248 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/baseline.py
--rw-r--r--   0        0        0     2978 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/baseline_tags.py
--rw-r--r--   0        0        0    43708 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/config.py
--rw-r--r--   0        0        0     3468 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/constants.py
--rw-r--r--   0        0        0    36891 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/correlation_search.py
--rw-r--r--   0        0        0      405 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/data_source.py
--rw-r--r--   0        0        0     2651 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment.py
--rw-r--r--   0        0        0      147 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment_email.py
--rw-r--r--   0        0        0      198 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment_notable.py
--rw-r--r--   0        0        0      207 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment_phantom.py
--rw-r--r--   0        0        0      125 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment_rba.py
--rw-r--r--   0        0        0      198 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment_scheduling.py
--rw-r--r--   0        0        0      135 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/deployment_slack.py
--rw-r--r--   0        0        0      620 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/detection.py
--rw-r--r--   0        0        0    10238 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/detection_tags.py
--rw-r--r--   0        0        0    14030 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/enums.py
--rw-r--r--   0        0        0     1273 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/integration_test.py
--rw-r--r--   0        0        0      370 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/integration_test_result.py
--rw-r--r--   0        0        0     2620 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/investigation.py
--rw-r--r--   0        0        0     1280 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/investigation_tags.py
--rw-r--r--   0        0        0     4556 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/lookup.py
--rw-r--r--   0        0        0     2451 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/macro.py
--rw-r--r--   0        0        0     1073 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/mitre_attack_enrichment.py
--rw-r--r--   0        0        0     1605 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/notable_action.py
--rw-r--r--   0        0        0     1156 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/observable.py
--rw-r--r--   0        0        0     2469 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/playbook.py
--rw-r--r--   0        0        0     1436 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/playbook_tags.py
--rw-r--r--   0        0        0     4288 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/risk_analysis_action.py
--rw-r--r--   0        0        0      904 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/risk_object.py
--rw-r--r--   0        0        0      234 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/security_content_object.py
--rw-r--r--   0        0        0     5873 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/ssa_detection.py
--rw-r--r--   0        0        0     5224 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/ssa_detection_tags.py
--rw-r--r--   0        0        0     4526 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/story.py
--rw-r--r--   0        0        0     2169 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/story_tags.py
--rw-r--r--   0        0        0     2600 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/test_group.py
--rw-r--r--   0        0        0      711 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/threat_object.py
--rw-r--r--   0        0        0     1655 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/unit_test.py
--rw-r--r--   0        0        0      480 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/unit_test_attack_data.py
--rw-r--r--   0        0        0      227 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/unit_test_baseline.py
--rw-r--r--   0        0        0      199 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/unit_test_old.py
--rw-r--r--   0        0        0     2940 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/unit_test_result.py
--rw-r--r--   0        0        0      653 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/objects/unit_test_ssa.py
--rw-r--r--   0        0        0     9085 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/api_json_output.py
--rw-r--r--   0        0        0     2304 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/attack_nav_output.py
--rw-r--r--   0        0        0     2219 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/attack_nav_writer.py
--rw-r--r--   0        0        0     5950 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/ba_yml_output.py
--rw-r--r--   0        0        0    10147 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/conf_output.py
--rw-r--r--   0        0        0     8280 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/conf_writer.py
--rw-r--r--   0        0        0      960 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/detection_writer.py
--rw-r--r--   0        0        0     3238 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/doc_md_output.py
--rw-r--r--   0        0        0     3935 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/finding_report_writer.py
--rw-r--r--   0        0        0     1119 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/jinja_writer.py
--rw-r--r--   0        0        0     1007 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/json_writer.py
--rw-r--r--   0        0        0     2321 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/new_content_yml_output.py
--rw-r--r--   0        0        0     2751 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/svg_output.py
--rw-r--r--   0        0        0      917 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/analyticstories_detections.j2
--rw-r--r--   0        0        0      515 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/analyticstories_investigations.j2
--rw-r--r--   0        0        0      668 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/analyticstories_stories.j2
--rw-r--r--   0        0        0      737 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/app.conf.j2
--rw-r--r--   0        0        0     1063 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/app.manifest.j2
--rw-r--r--   0        0        0      181 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/collections.j2
--rw-r--r--   0        0        0       54 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/content-version.j2
--rw-r--r--   0        0        0      670 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/detection_count.j2
--rw-r--r--   0        0        0      631 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/detection_coverage.j2
--rw-r--r--   0        0        0     1012 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_detection_page.j2
--rw-r--r--   0        0        0     6596 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_detections.j2
--rw-r--r--   0        0        0     1471 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_navigation.j2
--rw-r--r--   0        0        0      203 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_navigation_pages.j2
--rw-r--r--   0        0        0     1681 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_playbooks.j2
--rw-r--r--   0        0        0      679 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_playbooks_page.j2
--rw-r--r--   0        0        0     1827 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_stories.j2
--rw-r--r--   0        0        0      874 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/doc_story_page.j2
--rw-r--r--   0        0        0     1003 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/es_investigations_investigations.j2
--rw-r--r--   0        0        0      388 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/es_investigations_stories.j2
--rw-r--r--   0        0        0     1753 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/finding_report.j2
--rw-r--r--   0        0        0      201 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/header.j2
--rw-r--r--   0        0        0      390 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/macros.j2
--rw-r--r--   0        0        0      221 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/panel.j2
--rw-r--r--   0        0        0     1743 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/savedsearches_baselines.j2
--rw-r--r--   0        0        0     6805 2024-05-07 02:00:52.757300 contentctl-4.0.1/contentctl/output/templates/savedsearches_detections.j2
--rw-r--r--   0        0        0     1259 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/output/templates/savedsearches_investigations.j2
--rw-r--r--   0        0        0     1456 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/output/templates/transforms.j2
--rw-r--r--   0        0        0      925 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/output/templates/workflow_actions.j2
--rw-r--r--   0        0        0     2682 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/output/yml_output.py
--rw-r--r--   0        0        0      271 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/output/yml_writer.py
--rw-r--r--   0        0        0      133 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/README
--rw-r--r--   0        0        0     6390 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_default.yml
--rw-r--r--   0        0        0      897 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/README/essoc_story_detail.txt
--rw-r--r--   0        0        0     2538 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/README/essoc_summary.txt
--rw-r--r--   0        0        0     2432 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/README/essoc_usage_dashboard.txt
--rw-r--r--   0        0        0      366 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/README.md
--rw-r--r--   0        0        0      168 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/analytic_stories.conf
--rw-r--r--   0        0        0      685 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/app.conf
--rw-r--r--   0        0        0      319 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/commands.conf
--rw-r--r--   0        0        0       34 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/content-version.conf
--rw-r--r--   0        0        0      236 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/data/ui/nav/default.xml
--rw-r--r--   0        0        0     8635 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/data/ui/views/escu_summary.xml
--rw-r--r--   0        0        0      696 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/data/ui/views/feedback.xml
--rw-r--r--   0        0        0      156 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/distsearch.conf
--rw-r--r--   0        0        0     4257 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/usage_searches.conf
--rw-r--r--   0        0        0      168 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/default/use_case_library.conf
--rw-r--r--   0        0        0    66072 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/lookups/mitre_enrichment.csv
--rw-r--r--   0        0        0      423 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/metadata/default.meta
--rw-r--r--   0        0        0     3658 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/static/appIcon.png
--rw-r--r--   0        0        0     2656 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/static/appIconAlt.png
--rw-r--r--   0        0        0     7442 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/static/appIconAlt_2x.png
--rw-r--r--   0        0        0     3657 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/app_template/static/appIcon_2x.png
--rw-r--r--   0        0        0     9381 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/datamodels_cim.conf
--rw-r--r--   0        0        0      480 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/datamodels_custom.conf
--rw-r--r--   0        0        0      418 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_anomaly.yml
--rw-r--r--   0        0        0      334 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_baseline.yml
--rw-r--r--   0        0        0      519 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_correlation.yml
--rw-r--r--   0        0        0      329 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_hunting.yml
--rw-r--r--   0        0        0      548 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_ttp.yml
--rw-r--r--   0        0        0     3323 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/detections/anomalous_usage_of_7zip.yml
--rw-r--r--   0        0        0      159 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/macros/security_content_ctime.yml
--rw-r--r--   0        0        0      162 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/macros/security_content_summariesonly.yml
--rw-r--r--   0        0        0     3063 2024-05-07 02:00:52.761300 contentctl-4.0.1/contentctl/templates/stories/cobalt_strike.yml
--rw-r--r--   0        0        0      849 2024-05-07 02:00:52.761300 contentctl-4.0.1/pyproject.toml
--rw-r--r--   0        0        0    19705 1970-01-01 00:00:00.000000 contentctl-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-05-14 16:27:15.929205 contentctl-4.0.2/LICENSE.md
+-rw-r--r--   0        0        0    18472 2024-05-14 16:27:15.929205 contentctl-4.0.2/README.md
+-rw-r--r--   0        0        0       22 2024-05-14 16:27:15.929205 contentctl-4.0.2/contentctl/__init__.py
+-rw-r--r--   0        0        0     1418 2024-05-14 16:27:15.929205 contentctl-4.0.2/contentctl/actions/acs_deploy.py
+-rw-r--r--   0        0        0     2999 2024-05-14 16:27:15.929205 contentctl-4.0.2/contentctl/actions/apav_deploy.py
+-rw-r--r--   0        0        0     6965 2024-05-14 16:27:15.929205 contentctl-4.0.2/contentctl/actions/api_deploy.py
+-rw-r--r--   0        0        0     4765 2024-05-14 16:27:15.929205 contentctl-4.0.2/contentctl/actions/build.py
+-rw-r--r--   0        0        0      704 2024-05-14 16:27:15.929205 contentctl-4.0.2/contentctl/actions/convert.py
+-rw-r--r--   0        0        0     8818 2024-05-14 16:27:15.929205 contentctl-4.0.2/contentctl/actions/detection_testing/DetectionTestingManager.py
+-rw-r--r--   0        0        0     8666 2024-05-14 16:27:15.929205 contentctl-4.0.2/contentctl/actions/detection_testing/GitService.py
+-rw-r--r--   0        0        0     2259 2024-05-14 16:27:15.929205 contentctl-4.0.2/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
+-rw-r--r--   0        0        0    53141 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
+-rw-r--r--   0        0        0     6846 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
+-rw-r--r--   0        0        0      370 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
+-rw-r--r--   0        0        0     3244 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/detection_testing/progress_bar.py
+-rw-r--r--   0        0        0     7013 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/detection_testing/views/DetectionTestingView.py
+-rw-r--r--   0        0        0     2050 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
+-rw-r--r--   0        0        0     1123 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
+-rw-r--r--   0        0        0     4706 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
+-rw-r--r--   0        0        0      863 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/doc_gen.py
+-rw-r--r--   0        0        0     1749 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/initialize.py
+-rw-r--r--   0        0        0     9333 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/initialize_old.py
+-rw-r--r--   0        0        0    12628 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/inspect.py
+-rw-r--r--   0        0        0     5792 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/new_content.py
+-rw-r--r--   0        0        0    13115 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/release_notes.py
+-rw-r--r--   0        0        0     1583 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/reporting.py
+-rw-r--r--   0        0        0     4896 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/test.py
+-rw-r--r--   0        0        0     2363 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/actions/validate.py
+-rw-r--r--   0        0        0    10083 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/contentctl.py
+-rw-r--r--   0        0        0     6732 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/enrichments/attack_enrichment.py
+-rw-r--r--   0        0        0     3934 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/enrichments/cve_enrichment.py
+-rw-r--r--   0        0        0     3418 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/enrichments/splunk_app_enrichment.py
+-rw-r--r--   0        0        0     7139 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/helper/link_validator.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/helper/logger.py
+-rw-r--r--   0        0        0    15659 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/helper/utils.py
+-rw-r--r--   0        0        0     5861 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/input/backend_splunk_ba.py
+-rw-r--r--   0        0        0    10716 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/input/director.py
+-rw-r--r--   0        0        0     5718 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/input/new_content_questions.py
+-rw-r--r--   0        0        0    19391 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/input/sigma_converter.py
+-rw-r--r--   0        0        0     8377 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/input/ssa_detection_builder.py
+-rw-r--r--   0        0        0     1475 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/input/yml_reader.py
+-rw-r--r--   0        0        0    30167 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/abstract_security_content_objects/detection_abstract.py
+-rw-r--r--   0        0        0     8065 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py
+-rw-r--r--   0        0        0     1335 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/alert_action.py
+-rw-r--r--   0        0        0     8979 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/atomic.py
+-rw-r--r--   0        0        0     1028 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/base_test.py
+-rw-r--r--   0        0        0     4752 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/base_test_result.py
+-rw-r--r--   0        0        0     2248 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/baseline.py
+-rw-r--r--   0        0        0     2978 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/baseline_tags.py
+-rw-r--r--   0        0        0    43708 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/config.py
+-rw-r--r--   0        0        0     3468 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/constants.py
+-rw-r--r--   0        0        0    36891 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/correlation_search.py
+-rw-r--r--   0        0        0      405 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/data_source.py
+-rw-r--r--   0        0        0     2651 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/deployment.py
+-rw-r--r--   0        0        0      147 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/deployment_email.py
+-rw-r--r--   0        0        0      198 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/deployment_notable.py
+-rw-r--r--   0        0        0      207 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/deployment_phantom.py
+-rw-r--r--   0        0        0      125 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/deployment_rba.py
+-rw-r--r--   0        0        0      198 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/deployment_scheduling.py
+-rw-r--r--   0        0        0      135 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/deployment_slack.py
+-rw-r--r--   0        0        0      620 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/detection.py
+-rw-r--r--   0        0        0    10238 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/detection_tags.py
+-rw-r--r--   0        0        0    14030 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/enums.py
+-rw-r--r--   0        0        0     1273 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/integration_test.py
+-rw-r--r--   0        0        0      370 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/integration_test_result.py
+-rw-r--r--   0        0        0     2620 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/investigation.py
+-rw-r--r--   0        0        0     1280 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/investigation_tags.py
+-rw-r--r--   0        0        0     4556 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/lookup.py
+-rw-r--r--   0        0        0     2451 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/macro.py
+-rw-r--r--   0        0        0     1073 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/mitre_attack_enrichment.py
+-rw-r--r--   0        0        0     1605 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/notable_action.py
+-rw-r--r--   0        0        0     1156 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/observable.py
+-rw-r--r--   0        0        0     2469 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/playbook.py
+-rw-r--r--   0        0        0     1436 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/playbook_tags.py
+-rw-r--r--   0        0        0     4288 2024-05-14 16:27:15.933205 contentctl-4.0.2/contentctl/objects/risk_analysis_action.py
+-rw-r--r--   0        0        0      904 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/risk_object.py
+-rw-r--r--   0        0        0      234 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/security_content_object.py
+-rw-r--r--   0        0        0     5873 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/ssa_detection.py
+-rw-r--r--   0        0        0     5224 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/ssa_detection_tags.py
+-rw-r--r--   0        0        0     4526 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/story.py
+-rw-r--r--   0        0        0     2169 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/story_tags.py
+-rw-r--r--   0        0        0     2600 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/test_group.py
+-rw-r--r--   0        0        0      711 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/threat_object.py
+-rw-r--r--   0        0        0     1655 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/unit_test.py
+-rw-r--r--   0        0        0      480 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/unit_test_attack_data.py
+-rw-r--r--   0        0        0      227 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/unit_test_baseline.py
+-rw-r--r--   0        0        0      199 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/unit_test_old.py
+-rw-r--r--   0        0        0     2940 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/unit_test_result.py
+-rw-r--r--   0        0        0      653 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/objects/unit_test_ssa.py
+-rw-r--r--   0        0        0     9085 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/api_json_output.py
+-rw-r--r--   0        0        0     2304 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/attack_nav_output.py
+-rw-r--r--   0        0        0     2219 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/attack_nav_writer.py
+-rw-r--r--   0        0        0     5950 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/ba_yml_output.py
+-rw-r--r--   0        0        0    10147 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/conf_output.py
+-rw-r--r--   0        0        0     8281 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/conf_writer.py
+-rw-r--r--   0        0        0      960 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/detection_writer.py
+-rw-r--r--   0        0        0     3238 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/doc_md_output.py
+-rw-r--r--   0        0        0     3935 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/finding_report_writer.py
+-rw-r--r--   0        0        0     1119 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/jinja_writer.py
+-rw-r--r--   0        0        0     1007 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/json_writer.py
+-rw-r--r--   0        0        0     2321 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/new_content_yml_output.py
+-rw-r--r--   0        0        0     2751 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/svg_output.py
+-rw-r--r--   0        0        0      917 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/analyticstories_detections.j2
+-rw-r--r--   0        0        0      515 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/analyticstories_investigations.j2
+-rw-r--r--   0        0        0      668 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/analyticstories_stories.j2
+-rw-r--r--   0        0        0      737 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/app.conf.j2
+-rw-r--r--   0        0        0     1063 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/app.manifest.j2
+-rw-r--r--   0        0        0      181 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/collections.j2
+-rw-r--r--   0        0        0       54 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/content-version.j2
+-rw-r--r--   0        0        0      670 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/detection_count.j2
+-rw-r--r--   0        0        0      631 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/detection_coverage.j2
+-rw-r--r--   0        0        0     1012 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/doc_detection_page.j2
+-rw-r--r--   0        0        0     6596 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/doc_detections.j2
+-rw-r--r--   0        0        0     1471 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/doc_navigation.j2
+-rw-r--r--   0        0        0      203 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/doc_navigation_pages.j2
+-rw-r--r--   0        0        0     1681 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/doc_playbooks.j2
+-rw-r--r--   0        0        0      679 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/doc_playbooks_page.j2
+-rw-r--r--   0        0        0     1827 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/doc_stories.j2
+-rw-r--r--   0        0        0      874 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/doc_story_page.j2
+-rw-r--r--   0        0        0     1013 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/es_investigations_investigations.j2
+-rw-r--r--   0        0        0      388 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/es_investigations_stories.j2
+-rw-r--r--   0        0        0     1753 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/finding_report.j2
+-rw-r--r--   0        0        0      201 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/header.j2
+-rw-r--r--   0        0        0      390 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/macros.j2
+-rw-r--r--   0        0        0      221 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/panel.j2
+-rw-r--r--   0        0        0     1743 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/savedsearches_baselines.j2
+-rw-r--r--   0        0        0     6805 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/savedsearches_detections.j2
+-rw-r--r--   0        0        0     1259 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/savedsearches_investigations.j2
+-rw-r--r--   0        0        0     1456 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/transforms.j2
+-rw-r--r--   0        0        0      925 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/templates/workflow_actions.j2
+-rw-r--r--   0        0        0     2682 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/yml_output.py
+-rw-r--r--   0        0        0      271 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/output/yml_writer.py
+-rw-r--r--   0        0        0      133 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/README
+-rw-r--r--   0        0        0     6390 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_default.yml
+-rw-r--r--   0        0        0      897 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/README/essoc_story_detail.txt
+-rw-r--r--   0        0        0     2538 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/README/essoc_summary.txt
+-rw-r--r--   0        0        0     2432 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/README/essoc_usage_dashboard.txt
+-rw-r--r--   0        0        0      366 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/README.md
+-rw-r--r--   0        0        0      168 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/default/analytic_stories.conf
+-rw-r--r--   0        0        0      685 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/default/app.conf
+-rw-r--r--   0        0        0      319 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/default/commands.conf
+-rw-r--r--   0        0        0       34 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/default/content-version.conf
+-rw-r--r--   0        0        0      236 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/default/data/ui/nav/default.xml
+-rw-r--r--   0        0        0     8635 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/default/data/ui/views/escu_summary.xml
+-rw-r--r--   0        0        0      696 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/default/data/ui/views/feedback.xml
+-rw-r--r--   0        0        0      156 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/default/distsearch.conf
+-rw-r--r--   0        0        0     4257 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/default/usage_searches.conf
+-rw-r--r--   0        0        0      168 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/default/use_case_library.conf
+-rw-r--r--   0        0        0    66072 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/lookups/mitre_enrichment.csv
+-rw-r--r--   0        0        0      423 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/metadata/default.meta
+-rw-r--r--   0        0        0     3658 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/static/appIcon.png
+-rw-r--r--   0        0        0     2656 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/static/appIconAlt.png
+-rw-r--r--   0        0        0     7442 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/static/appIconAlt_2x.png
+-rw-r--r--   0        0        0     3657 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/app_template/static/appIcon_2x.png
+-rw-r--r--   0        0        0     9381 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/datamodels_cim.conf
+-rw-r--r--   0        0        0      480 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/datamodels_custom.conf
+-rw-r--r--   0        0        0      418 2024-05-14 16:27:15.937205 contentctl-4.0.2/contentctl/templates/deployments/escu_default_configuration_anomaly.yml
+-rw-r--r--   0        0        0      334 2024-05-14 16:27:15.941205 contentctl-4.0.2/contentctl/templates/deployments/escu_default_configuration_baseline.yml
+-rw-r--r--   0        0        0      519 2024-05-14 16:27:15.941205 contentctl-4.0.2/contentctl/templates/deployments/escu_default_configuration_correlation.yml
+-rw-r--r--   0        0        0      329 2024-05-14 16:27:15.941205 contentctl-4.0.2/contentctl/templates/deployments/escu_default_configuration_hunting.yml
+-rw-r--r--   0        0        0      548 2024-05-14 16:27:15.941205 contentctl-4.0.2/contentctl/templates/deployments/escu_default_configuration_ttp.yml
+-rw-r--r--   0        0        0     3323 2024-05-14 16:27:15.941205 contentctl-4.0.2/contentctl/templates/detections/anomalous_usage_of_7zip.yml
+-rw-r--r--   0        0        0      159 2024-05-14 16:27:15.941205 contentctl-4.0.2/contentctl/templates/macros/security_content_ctime.yml
+-rw-r--r--   0        0        0      162 2024-05-14 16:27:15.941205 contentctl-4.0.2/contentctl/templates/macros/security_content_summariesonly.yml
+-rw-r--r--   0        0        0     3063 2024-05-14 16:27:15.941205 contentctl-4.0.2/contentctl/templates/stories/cobalt_strike.yml
+-rw-r--r--   0        0        0      849 2024-05-14 16:27:15.941205 contentctl-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0    19705 1970-01-01 00:00:00.000000 contentctl-4.0.2/PKG-INFO
```

### Comparing `contentctl-4.0.1/LICENSE.md` & `contentctl-4.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/README.md` & `contentctl-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/acs_deploy.py` & `contentctl-4.0.2/contentctl/actions/acs_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/apav_deploy.py` & `contentctl-4.0.2/contentctl/actions/apav_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/api_deploy.py` & `contentctl-4.0.2/contentctl/actions/api_deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/build.py` & `contentctl-4.0.2/contentctl/actions/build.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/convert.py` & `contentctl-4.0.2/contentctl/actions/convert.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/detection_testing/DetectionTestingManager.py` & `contentctl-4.0.2/contentctl/actions/detection_testing/DetectionTestingManager.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/detection_testing/GitService.py` & `contentctl-4.0.2/contentctl/actions/detection_testing/GitService.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/detection_testing/generate_detection_coverage_badge.py` & `contentctl-4.0.2/contentctl/actions/detection_testing/generate_detection_coverage_badge.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py` & `contentctl-4.0.2/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py` & `contentctl-4.0.2/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/detection_testing/progress_bar.py` & `contentctl-4.0.2/contentctl/actions/detection_testing/progress_bar.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingView.py` & `contentctl-4.0.2/contentctl/actions/detection_testing/views/DetectionTestingView.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py` & `contentctl-4.0.2/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py` & `contentctl-4.0.2/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py` & `contentctl-4.0.2/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/doc_gen.py` & `contentctl-4.0.2/contentctl/actions/doc_gen.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/initialize.py` & `contentctl-4.0.2/contentctl/actions/initialize.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/initialize_old.py` & `contentctl-4.0.2/contentctl/actions/initialize_old.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/inspect.py` & `contentctl-4.0.2/contentctl/actions/inspect.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/new_content.py` & `contentctl-4.0.2/contentctl/actions/new_content.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/release_notes.py` & `contentctl-4.0.2/contentctl/actions/release_notes.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/reporting.py` & `contentctl-4.0.2/contentctl/actions/reporting.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/test.py` & `contentctl-4.0.2/contentctl/actions/test.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/actions/validate.py` & `contentctl-4.0.2/contentctl/actions/validate.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/contentctl.py` & `contentctl-4.0.2/contentctl/contentctl.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/enrichments/attack_enrichment.py` & `contentctl-4.0.2/contentctl/enrichments/attack_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/enrichments/cve_enrichment.py` & `contentctl-4.0.2/contentctl/enrichments/cve_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/enrichments/splunk_app_enrichment.py` & `contentctl-4.0.2/contentctl/enrichments/splunk_app_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/helper/link_validator.py` & `contentctl-4.0.2/contentctl/helper/link_validator.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/helper/utils.py` & `contentctl-4.0.2/contentctl/helper/utils.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/input/backend_splunk_ba.py` & `contentctl-4.0.2/contentctl/input/backend_splunk_ba.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/input/director.py` & `contentctl-4.0.2/contentctl/input/director.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/input/new_content_questions.py` & `contentctl-4.0.2/contentctl/input/new_content_questions.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/input/sigma_converter.py` & `contentctl-4.0.2/contentctl/input/sigma_converter.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/input/ssa_detection_builder.py` & `contentctl-4.0.2/contentctl/input/ssa_detection_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/input/yml_reader.py` & `contentctl-4.0.2/contentctl/input/yml_reader.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/abstract_security_content_objects/detection_abstract.py` & `contentctl-4.0.2/contentctl/objects/abstract_security_content_objects/detection_abstract.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py` & `contentctl-4.0.2/contentctl/objects/abstract_security_content_objects/security_content_object_abstract.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/alert_action.py` & `contentctl-4.0.2/contentctl/objects/alert_action.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/atomic.py` & `contentctl-4.0.2/contentctl/objects/atomic.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/base_test.py` & `contentctl-4.0.2/contentctl/objects/base_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/base_test_result.py` & `contentctl-4.0.2/contentctl/objects/base_test_result.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/baseline.py` & `contentctl-4.0.2/contentctl/objects/baseline.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/baseline_tags.py` & `contentctl-4.0.2/contentctl/objects/baseline_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/config.py` & `contentctl-4.0.2/contentctl/objects/config.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/constants.py` & `contentctl-4.0.2/contentctl/objects/constants.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/correlation_search.py` & `contentctl-4.0.2/contentctl/objects/correlation_search.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/deployment.py` & `contentctl-4.0.2/contentctl/objects/deployment.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/detection.py` & `contentctl-4.0.2/contentctl/objects/detection.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/detection_tags.py` & `contentctl-4.0.2/contentctl/objects/detection_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/enums.py` & `contentctl-4.0.2/contentctl/objects/enums.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/integration_test.py` & `contentctl-4.0.2/contentctl/objects/integration_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/investigation.py` & `contentctl-4.0.2/contentctl/objects/investigation.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/investigation_tags.py` & `contentctl-4.0.2/contentctl/objects/investigation_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/lookup.py` & `contentctl-4.0.2/contentctl/objects/lookup.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/macro.py` & `contentctl-4.0.2/contentctl/objects/macro.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/mitre_attack_enrichment.py` & `contentctl-4.0.2/contentctl/objects/mitre_attack_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/notable_action.py` & `contentctl-4.0.2/contentctl/objects/notable_action.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/observable.py` & `contentctl-4.0.2/contentctl/objects/observable.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/playbook.py` & `contentctl-4.0.2/contentctl/objects/playbook.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/playbook_tags.py` & `contentctl-4.0.2/contentctl/objects/playbook_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/risk_analysis_action.py` & `contentctl-4.0.2/contentctl/objects/risk_analysis_action.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/risk_object.py` & `contentctl-4.0.2/contentctl/objects/risk_object.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/ssa_detection.py` & `contentctl-4.0.2/contentctl/objects/ssa_detection.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/ssa_detection_tags.py` & `contentctl-4.0.2/contentctl/objects/ssa_detection_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/story.py` & `contentctl-4.0.2/contentctl/objects/story.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/story_tags.py` & `contentctl-4.0.2/contentctl/objects/story_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/test_group.py` & `contentctl-4.0.2/contentctl/objects/test_group.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/threat_object.py` & `contentctl-4.0.2/contentctl/objects/threat_object.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/unit_test.py` & `contentctl-4.0.2/contentctl/objects/unit_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/unit_test_result.py` & `contentctl-4.0.2/contentctl/objects/unit_test_result.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/objects/unit_test_ssa.py` & `contentctl-4.0.2/contentctl/objects/unit_test_ssa.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/api_json_output.py` & `contentctl-4.0.2/contentctl/output/api_json_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/attack_nav_output.py` & `contentctl-4.0.2/contentctl/output/attack_nav_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/attack_nav_writer.py` & `contentctl-4.0.2/contentctl/output/attack_nav_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/ba_yml_output.py` & `contentctl-4.0.2/contentctl/output/ba_yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/conf_output.py` & `contentctl-4.0.2/contentctl/output/conf_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/conf_writer.py` & `contentctl-4.0.2/contentctl/output/conf_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     
     @staticmethod
     def escapeNewlines(obj:Any):
         # Ensure that any newlines that occur in a string are escaped with a \.
         # Failing to do so will result in an improperly formatted conf files that
         # cannot be parsed
         if isinstance(obj,str):
-            return obj.replace(f"\n","\\\n")
+            return obj.replace(f"\n"," \\\n")
         else:
             return obj
 
 
     @staticmethod
     def writeConfFileHeader(app_output_path:pathlib.Path, config: build) -> pathlib.Path:
         output = ConfWriter.writeFileHeader(app_output_path, config)
```

### Comparing `contentctl-4.0.1/contentctl/output/detection_writer.py` & `contentctl-4.0.2/contentctl/output/detection_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/doc_md_output.py` & `contentctl-4.0.2/contentctl/output/doc_md_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/finding_report_writer.py` & `contentctl-4.0.2/contentctl/output/finding_report_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/jinja_writer.py` & `contentctl-4.0.2/contentctl/output/jinja_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/json_writer.py` & `contentctl-4.0.2/contentctl/output/json_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/new_content_yml_output.py` & `contentctl-4.0.2/contentctl/output/new_content_yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/svg_output.py` & `contentctl-4.0.2/contentctl/output/svg_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/analyticstories_detections.j2` & `contentctl-4.0.2/contentctl/output/templates/analyticstories_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/analyticstories_investigations.j2` & `contentctl-4.0.2/contentctl/output/templates/analyticstories_investigations.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/analyticstories_stories.j2` & `contentctl-4.0.2/contentctl/output/templates/analyticstories_stories.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/app.conf.j2` & `contentctl-4.0.2/contentctl/output/templates/app.conf.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/app.manifest.j2` & `contentctl-4.0.2/contentctl/output/templates/app.manifest.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/detection_count.j2` & `contentctl-4.0.2/contentctl/output/templates/detection_count.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/detection_coverage.j2` & `contentctl-4.0.2/contentctl/output/templates/detection_coverage.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/doc_detection_page.j2` & `contentctl-4.0.2/contentctl/output/templates/doc_detection_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/doc_detections.j2` & `contentctl-4.0.2/contentctl/output/templates/doc_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/doc_navigation.j2` & `contentctl-4.0.2/contentctl/output/templates/doc_navigation.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/doc_playbooks.j2` & `contentctl-4.0.2/contentctl/output/templates/doc_playbooks.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/doc_playbooks_page.j2` & `contentctl-4.0.2/contentctl/output/templates/doc_playbooks_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/doc_stories.j2` & `contentctl-4.0.2/contentctl/output/templates/doc_stories.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/doc_story_page.j2` & `contentctl-4.0.2/contentctl/output/templates/doc_story_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/es_investigations_investigations.j2` & `contentctl-4.0.2/contentctl/output/templates/es_investigations_investigations.j2`

 * *Files 3% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 [panel://workbench_panel_{{ response_task.lowercase_name }}___response_task]
 label = {{ response_task.name }}
 description = {{ response_task.description | escapeNewlines() }}
 disabled = 0
 tokens = {\
 {% for token in response_task.inputs %}
 {% if token == 'user' %}
-  "user": {\
-    "valuePrefix": "\"",\
-    "valueSuffix": "\"",\
-    "delimiter": " OR {{ token }}=",\
-    "valueType": "primitive",\
-    "value": "identity",\
-    "default": "null"\
-    }\{% elif token == 'dest'%}
+    "user": {\
+      "valuePrefix": "\"",\
+      "valueSuffix": "\"",\
+      "delimiter": " OR {{ token }}=",\
+      "valueType": "primitive",\
+      "value": "identity",\
+      "default": "null"\
+    }{% elif token == 'dest'%}
     "dest": {\
       "valuePrefix": "\"",\
       "valueSuffix": "\"",\
       "delimiter": " OR {{ token }}=",\
       "valueType": "primitive",\
       "value": "asset",\
       "default": "null"\
-    }\{% else %}
+    }{% else %}
     "{{ token }}": {\
       "valuePrefix": "\"",\
       "valueSuffix": "\"",\
       "delimiter": " OR {{ token }}=",\
       "valueType": "primitive",\
       "value": "file",\
       "default": "null"\
-    }\{% endif %}{{ "," if not loop.last }}
+    }{% endif %}{{ "," if not loop.last }}\
 {% endfor %}
-  }\
+}\
 
 
 {% endfor %}
```

### Comparing `contentctl-4.0.1/contentctl/output/templates/finding_report.j2` & `contentctl-4.0.2/contentctl/output/templates/finding_report.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/savedsearches_baselines.j2` & `contentctl-4.0.2/contentctl/output/templates/savedsearches_baselines.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/savedsearches_detections.j2` & `contentctl-4.0.2/contentctl/output/templates/savedsearches_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/savedsearches_investigations.j2` & `contentctl-4.0.2/contentctl/output/templates/savedsearches_investigations.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/transforms.j2` & `contentctl-4.0.2/contentctl/output/templates/transforms.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/templates/workflow_actions.j2` & `contentctl-4.0.2/contentctl/output/templates/workflow_actions.j2`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/output/yml_output.py` & `contentctl-4.0.2/contentctl/output/yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/app_default.yml` & `contentctl-4.0.2/contentctl/templates/app_default.yml`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/app_template/README/essoc_story_detail.txt` & `contentctl-4.0.2/contentctl/templates/app_template/README/essoc_story_detail.txt`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/app_template/README/essoc_summary.txt` & `contentctl-4.0.2/contentctl/templates/app_template/README/essoc_summary.txt`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/app_template/README/essoc_usage_dashboard.txt` & `contentctl-4.0.2/contentctl/templates/app_template/README/essoc_usage_dashboard.txt`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/app_template/default/app.conf` & `contentctl-4.0.2/contentctl/templates/app_template/default/app.conf`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/app_template/default/data/ui/views/escu_summary.xml` & `contentctl-4.0.2/contentctl/templates/app_template/default/data/ui/views/escu_summary.xml`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/app_template/default/data/ui/views/feedback.xml` & `contentctl-4.0.2/contentctl/templates/app_template/default/data/ui/views/feedback.xml`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/app_template/default/usage_searches.conf` & `contentctl-4.0.2/contentctl/templates/app_template/default/usage_searches.conf`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/app_template/lookups/mitre_enrichment.csv` & `contentctl-4.0.2/contentctl/templates/app_template/lookups/mitre_enrichment.csv`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/app_template/static/appIcon.png` & `contentctl-4.0.2/contentctl/templates/app_template/static/appIcon.png`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/app_template/static/appIconAlt.png` & `contentctl-4.0.2/contentctl/templates/app_template/static/appIconAlt.png`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/app_template/static/appIconAlt_2x.png` & `contentctl-4.0.2/contentctl/templates/app_template/static/appIconAlt_2x.png`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/app_template/static/appIcon_2x.png` & `contentctl-4.0.2/contentctl/templates/app_template/static/appIcon_2x.png`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/datamodels_cim.conf` & `contentctl-4.0.2/contentctl/templates/datamodels_cim.conf`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_correlation.yml` & `contentctl-4.0.2/contentctl/templates/deployments/escu_default_configuration_correlation.yml`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/deployments/escu_default_configuration_ttp.yml` & `contentctl-4.0.2/contentctl/templates/deployments/escu_default_configuration_ttp.yml`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/detections/anomalous_usage_of_7zip.yml` & `contentctl-4.0.2/contentctl/templates/detections/anomalous_usage_of_7zip.yml`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/contentctl/templates/stories/cobalt_strike.yml` & `contentctl-4.0.2/contentctl/templates/stories/cobalt_strike.yml`

 * *Files identical despite different names*

### Comparing `contentctl-4.0.1/pyproject.toml` & `contentctl-4.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contentctl"
-version = "4.0.1"
+version = "4.0.2"
 description = "Splunk Content Control Tool"
 authors = ["STRT <research@splunk.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 contentctl = 'contentctl.contentctl:main'
```

### Comparing `contentctl-4.0.1/PKG-INFO` & `contentctl-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contentctl
-Version: 4.0.1
+Version: 4.0.2
 Summary: Splunk Content Control Tool
 License: Apache 2.0
 Author: STRT
 Author-email: research@splunk.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

