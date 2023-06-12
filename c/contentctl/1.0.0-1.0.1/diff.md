# Comparing `tmp/contentctl-1.0.0.tar.gz` & `tmp/contentctl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contentctl-1.0.0.tar", max compression
+gzip compressed data, was "contentctl-1.0.1.tar", max compression
```

## Comparing `contentctl-1.0.0.tar` & `contentctl-1.0.1.tar`

### file list

```diff
@@ -1,126 +1,124 @@
--rw-r--r--   0        0        0    11344 2023-03-13 08:07:40.310193 contentctl-1.0.0/LICENSE.md
--rw-r--r--   0        0        0    15553 2023-03-23 08:07:40.389843 contentctl-1.0.0/README.md
--rw-r--r--   0        0        0     2328 2023-01-04 17:47:48.369162 contentctl-1.0.0/contentctl/Res.yml
--rw-r--r--   0        0        0       22 2022-09-20 05:51:29.811617 contentctl-1.0.0/contentctl/__init__.py
--rw-r--r--   0        0        0     5844 2023-03-23 08:16:57.899843 contentctl-1.0.0/contentctl/actions/deploy.py
--rw-r--r--   0        0        0     5580 2023-03-23 08:07:40.389843 contentctl-1.0.0/contentctl/actions/detection_testing/DataManipulation.py
--rw-r--r--   0        0        0     7180 2023-03-23 08:17:14.719843 contentctl-1.0.0/contentctl/actions/detection_testing/DetectionTestingManager.py
--rw-r--r--   0        0        0    16208 2023-03-23 08:17:15.409843 contentctl-1.0.0/contentctl/actions/detection_testing/GitHubService.py
--rw-r--r--   0        0        0     2259 2023-01-04 17:47:48.369162 contentctl-1.0.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
--rw-r--r--   0        0        0    27291 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
--rw-r--r--   0        0        0     4016 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
--rw-r--r--   0        0        0      363 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
--rw-r--r--   0        0        0     3902 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/actions/detection_testing/views/DetectionTestingView.py
--rw-r--r--   0        0        0     2050 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
--rw-r--r--   0        0        0     1363 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
--rw-r--r--   0        0        0     4711 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
--rw-r--r--   0        0        0      857 2023-03-23 08:16:58.679843 contentctl-1.0.0/contentctl/actions/doc_gen.py
--rw-r--r--   0        0        0     3288 2023-03-23 08:16:59.379843 contentctl-1.0.0/contentctl/actions/generate.py
--rw-r--r--   0        0        0     1921 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/actions/initialize.py
--rw-r--r--   0        0        0     9333 2023-03-23 08:17:05.729843 contentctl-1.0.0/contentctl/actions/initialize_old.py
--rw-r--r--   0        0        0      920 2023-03-23 08:17:07.069843 contentctl-1.0.0/contentctl/actions/new_content.py
--rw-r--r--   0        0        0     1022 2023-03-23 08:17:07.899843 contentctl-1.0.0/contentctl/actions/reporting.py
--rw-r--r--   0        0        0     3014 2023-03-23 08:17:13.349843 contentctl-1.0.0/contentctl/actions/test.py
--rw-r--r--   0        0        0     2741 2023-03-23 08:17:14.059843 contentctl-1.0.0/contentctl/actions/validate.py
--rw-r--r--   0        0        0    13836 2023-03-23 08:16:56.899843 contentctl-1.0.0/contentctl/contentctl.py
--rw-r--r--   0        0        0     3885 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/enrichments/attack_enrichment.py
--rw-r--r--   0        0        0      713 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/enrichments/cve_enrichment.py
--rw-r--r--   0        0        0     1944 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/enrichments/splunk_app_enrichment.py
--rw-r--r--   0        0        0      584 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/helper/config_handler.py
--rw-r--r--   0        0        0     1070 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/helper/link_validator.py
--rw-r--r--   0        0        0        0 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/helper/logger.py
--rw-r--r--   0        0        0    15314 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/helper/utils.py
--rw-r--r--   0        0        0     1857 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/input/baseline_builder.py
--rw-r--r--   0        0        0     2227 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/input/basic_builder.py
--rw-r--r--   0        0        0    11747 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/input/detection_builder.py
--rw-r--r--   0        0        0    11127 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/input/director.py
--rw-r--r--   0        0        0     1244 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/input/investigation_builder.py
--rw-r--r--   0        0        0     4485 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/input/new_content_generator.py
--rw-r--r--   0        0        0     4576 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/input/new_content_questions.py
--rw-r--r--   0        0        0     1954 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/input/playbook_builder.py
--rw-r--r--   0        0        0     4738 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/input/story_builder.py
--rw-r--r--   0        0        0      814 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/input/yml_reader.py
--rw-r--r--   0        0        0     7621 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/app.py
--rw-r--r--   0        0        0     2560 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/baseline.py
--rw-r--r--   0        0        0      711 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/objects/baseline_tags.py
--rw-r--r--   0        0        0     1864 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/objects/config.py
--rw-r--r--   0        0        0     2290 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/objects/constants.py
--rw-r--r--   0        0        0     1913 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/deployment.py
--rw-r--r--   0        0        0      141 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/objects/deployment_email.py
--rw-r--r--   0        0        0      164 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/objects/deployment_notable.py
--rw-r--r--   0        0        0      201 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/objects/deployment_phantom.py
--rw-r--r--   0        0        0      111 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/objects/deployment_rba.py
--rw-r--r--   0        0        0      193 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/objects/deployment_scheduling.py
--rw-r--r--   0        0        0      129 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/objects/deployment_slack.py
--rw-r--r--   0        0        0     6191 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/detection.py
--rw-r--r--   0        0        0     4283 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/detection_tags.py
--rw-r--r--   0        0        0     1647 2023-03-23 08:07:40.389843 contentctl-1.0.0/contentctl/objects/enums.py
--rw-r--r--   0        0        0     2444 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/investigation.py
--rw-r--r--   0        0        0      191 2023-01-04 17:47:48.379162 contentctl-1.0.0/contentctl/objects/investigation_tags.py
--rw-r--r--   0        0        0      425 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/lookup.py
--rw-r--r--   0        0        0      271 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/macro.py
--rw-r--r--   0        0        0      219 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/objects/mitre_attack_enrichment.py
--rw-r--r--   0        0        0      589 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/playbook.py
--rw-r--r--   0        0        0      315 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/objects/playbook_tags.py
--rw-r--r--   0        0        0     6522 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/repo_config.py
--rw-r--r--   0        0        0      139 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/security_content_object.py
--rw-r--r--   0        0        0     1696 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/story.py
--rw-r--r--   0        0        0      926 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/story_tags.py
--rw-r--r--   0        0        0    22375 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/test_config.py
--rw-r--r--   0        0        0      316 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/unit_test.py
--rw-r--r--   0        0        0      605 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/unit_test_attack_data.py
--rw-r--r--   0        0        0      255 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/objects/unit_test_baseline.py
--rw-r--r--   0        0        0     8186 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/unit_test_result.py
--rw-r--r--   0        0        0      602 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/objects/unit_test_test.py
--rw-r--r--   0        0        0     3089 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/output/api_json_output.py
--rw-r--r--   0        0        0     1701 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/output/attack_nav_output.py
--rw-r--r--   0        0        0     2130 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/attack_nav_writer.py
--rw-r--r--   0        0        0     3946 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/output/ba_yml_output.py
--rw-r--r--   0        0        0     5756 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/output/conf_output.py
--rw-r--r--   0        0        0     2728 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/output/conf_writer.py
--rw-r--r--   0        0        0     3238 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/output/doc_md_output.py
--rw-r--r--   0        0        0     3050 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/output/finding_report_writer.py
--rw-r--r--   0        0        0     1089 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/jinja_writer.py
--rw-r--r--   0        0        0      210 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/json_writer.py
--rw-r--r--   0        0        0     3065 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/output/new_content_yml_output.py
--rw-r--r--   0        0        0     1059 2023-03-23 08:17:26.309843 contentctl-1.0.0/contentctl/output/svg_output.py
--rw-r--r--   0        0        0      745 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/analyticstories_detections.j2
--rw-r--r--   0        0        0      496 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/analyticstories_investigations.j2
--rw-r--r--   0        0        0      586 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/analyticstories_stories.j2
--rw-r--r--   0        0        0      180 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/collections.j2
--rw-r--r--   0        0        0      670 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/detection_count.j2
--rw-r--r--   0        0        0      671 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/detection_coverage.j2
--rw-r--r--   0        0        0     1002 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/doc_detection_page.j2
--rw-r--r--   0        0        0     6586 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/doc_detections.j2
--rw-r--r--   0        0        0     1471 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/doc_navigation.j2
--rw-r--r--   0        0        0      203 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/doc_navigation_pages.j2
--rw-r--r--   0        0        0     1681 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/doc_playbooks.j2
--rw-r--r--   0        0        0      679 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/doc_playbooks_page.j2
--rw-r--r--   0        0        0     1822 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/doc_stories.j2
--rw-r--r--   0        0        0      874 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/doc_story_page.j2
--rw-r--r--   0        0        0      994 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/es_investigations_investigations.j2
--rw-r--r--   0        0        0      369 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/es_investigations_stories.j2
--rw-r--r--   0        0        0     1432 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/finding_report.j2
--rw-r--r--   0        0        0      190 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/header.j2
--rw-r--r--   0        0        0      424 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/macros.j2
--rw-r--r--   0        0        0      282 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/macros_detections.j2
--rw-r--r--   0        0        0      221 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/panel.j2
--rw-r--r--   0        0        0     1840 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/savedsearches_baselines.j2
--rw-r--r--   0        0        0     5290 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/savedsearches_detections.j2
--rw-r--r--   0        0        0     1380 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/savedsearches_investigations.j2
--rw-r--r--   0        0        0     1416 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/transforms.j2
--rw-r--r--   0        0        0      925 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/templates/workflow_actions.j2
--rw-r--r--   0        0        0      235 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/output/yml_writer.py
--rw-r--r--   0        0        0     3843 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/templates/app_default.yml
--rw-r--r--   0        0        0      662 2023-03-23 08:07:40.399843 contentctl-1.0.0/contentctl/templates/contentctl_default.yml
--rw-r--r--   0        0        0     9381 2023-03-23 08:07:40.399843 contentctl-1.0.0/contentctl/templates/datamodels_cim.conf
--rw-r--r--   0        0        0      480 2023-03-23 08:07:40.399843 contentctl-1.0.0/contentctl/templates/datamodels_custom.conf
--rw-r--r--   0        0        0     3262 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml
--rw-r--r--   0        0        0      159 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/templates/macros/security_content_ctime.yml
--rw-r--r--   0        0        0      162 2023-01-04 17:47:48.389162 contentctl-1.0.0/contentctl/templates/macros/security_content_summariesonly.yml
--rw-r--r--   0        0        0       90 2023-01-04 17:47:48.399162 contentctl-1.0.0/contentctl/templates/splunk_app/metadata/default.meta
--rw-r--r--   0        0        0     3086 2023-01-04 17:47:48.399162 contentctl-1.0.0/contentctl/templates/stories/cobalt_strike.yml
--rw-r--r--   0        0        0      501 2023-01-04 17:47:48.399162 contentctl-1.0.0/contentctl/templates/tests/anomalous_usage_of_7zip.test.yml
--rw-r--r--   0        0        0      736 2023-03-23 08:14:34.089843 contentctl-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    17444 2023-03-23 08:17:33.507336 contentctl-1.0.0/setup.py
--rw-r--r--   0        0        0    16608 2023-03-23 08:17:33.507971 contentctl-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-06-12 22:32:39.582106 contentctl-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0    17554 2023-06-12 22:32:39.582106 contentctl-1.0.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/__init__.py
+-rw-r--r--   0        0        0     5844 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/deploy.py
+-rw-r--r--   0        0        0     5580 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/DataManipulation.py
+-rw-r--r--   0        0        0     7180 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/DetectionTestingManager.py
+-rw-r--r--   0        0        0    16208 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/GitHubService.py
+-rw-r--r--   0        0        0     2259 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/generate_detection_coverage_badge.py
+-rw-r--r--   0        0        0    27291 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py
+-rw-r--r--   0        0        0     4051 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py
+-rw-r--r--   0        0        0      363 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureServer.py
+-rw-r--r--   0        0        0     3902 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingView.py
+-rw-r--r--   0        0        0     2050 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py
+-rw-r--r--   0        0        0     1363 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py
+-rw-r--r--   0        0        0     4711 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py
+-rw-r--r--   0        0        0      857 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/doc_gen.py
+-rw-r--r--   0        0        0     3288 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/generate.py
+-rw-r--r--   0        0        0     1921 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/initialize.py
+-rw-r--r--   0        0        0     9333 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/initialize_old.py
+-rw-r--r--   0        0        0      920 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/new_content.py
+-rw-r--r--   0        0        0     1022 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/reporting.py
+-rw-r--r--   0        0        0     3014 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/test.py
+-rw-r--r--   0        0        0     2741 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/actions/validate.py
+-rw-r--r--   0        0        0    13836 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/contentctl.py
+-rw-r--r--   0        0        0     3885 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/enrichments/attack_enrichment.py
+-rw-r--r--   0        0        0      713 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/enrichments/cve_enrichment.py
+-rw-r--r--   0        0        0     1944 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/enrichments/splunk_app_enrichment.py
+-rw-r--r--   0        0        0      584 2023-06-12 22:32:39.582106 contentctl-1.0.1/contentctl/helper/config_handler.py
+-rw-r--r--   0        0        0     1070 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/helper/link_validator.py
+-rw-r--r--   0        0        0        0 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/helper/logger.py
+-rw-r--r--   0        0        0    15314 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/helper/utils.py
+-rw-r--r--   0        0        0     1857 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/baseline_builder.py
+-rw-r--r--   0        0        0     2227 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/basic_builder.py
+-rw-r--r--   0        0        0    11747 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/detection_builder.py
+-rw-r--r--   0        0        0    11127 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/director.py
+-rw-r--r--   0        0        0     1244 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/investigation_builder.py
+-rw-r--r--   0        0        0     4485 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/new_content_generator.py
+-rw-r--r--   0        0        0     4576 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/new_content_questions.py
+-rw-r--r--   0        0        0     1954 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/playbook_builder.py
+-rw-r--r--   0        0        0     4738 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/story_builder.py
+-rw-r--r--   0        0        0      814 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/input/yml_reader.py
+-rw-r--r--   0        0        0     7621 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/app.py
+-rw-r--r--   0        0        0     2560 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/baseline.py
+-rw-r--r--   0        0        0      711 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/baseline_tags.py
+-rw-r--r--   0        0        0     1864 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/config.py
+-rw-r--r--   0        0        0     2290 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/constants.py
+-rw-r--r--   0        0        0     1913 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment.py
+-rw-r--r--   0        0        0      141 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment_email.py
+-rw-r--r--   0        0        0      164 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment_notable.py
+-rw-r--r--   0        0        0      201 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment_phantom.py
+-rw-r--r--   0        0        0      111 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment_rba.py
+-rw-r--r--   0        0        0      193 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment_scheduling.py
+-rw-r--r--   0        0        0      129 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/deployment_slack.py
+-rw-r--r--   0        0        0     6191 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/detection.py
+-rw-r--r--   0        0        0     4283 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/detection_tags.py
+-rw-r--r--   0        0        0     1647 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/enums.py
+-rw-r--r--   0        0        0     2444 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/investigation.py
+-rw-r--r--   0        0        0      191 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/investigation_tags.py
+-rw-r--r--   0        0        0      425 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/lookup.py
+-rw-r--r--   0        0        0      271 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/macro.py
+-rw-r--r--   0        0        0      219 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/mitre_attack_enrichment.py
+-rw-r--r--   0        0        0      589 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/playbook.py
+-rw-r--r--   0        0        0      315 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/playbook_tags.py
+-rw-r--r--   0        0        0     6522 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/repo_config.py
+-rw-r--r--   0        0        0      139 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/security_content_object.py
+-rw-r--r--   0        0        0     1696 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/story.py
+-rw-r--r--   0        0        0      926 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/story_tags.py
+-rw-r--r--   0        0        0    22399 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/test_config.py
+-rw-r--r--   0        0        0      316 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/unit_test.py
+-rw-r--r--   0        0        0      605 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/unit_test_attack_data.py
+-rw-r--r--   0        0        0      255 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/unit_test_baseline.py
+-rw-r--r--   0        0        0     8186 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/unit_test_result.py
+-rw-r--r--   0        0        0      602 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/objects/unit_test_test.py
+-rw-r--r--   0        0        0     3089 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/api_json_output.py
+-rw-r--r--   0        0        0     1701 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/attack_nav_output.py
+-rw-r--r--   0        0        0     2130 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/attack_nav_writer.py
+-rw-r--r--   0        0        0     3946 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/ba_yml_output.py
+-rw-r--r--   0        0        0     5756 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/conf_output.py
+-rw-r--r--   0        0        0     2728 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/conf_writer.py
+-rw-r--r--   0        0        0     3238 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/doc_md_output.py
+-rw-r--r--   0        0        0     3050 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/finding_report_writer.py
+-rw-r--r--   0        0        0     1089 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/jinja_writer.py
+-rw-r--r--   0        0        0      210 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/json_writer.py
+-rw-r--r--   0        0        0     3065 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/new_content_yml_output.py
+-rw-r--r--   0        0        0     1059 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/svg_output.py
+-rw-r--r--   0        0        0      745 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/analyticstories_detections.j2
+-rw-r--r--   0        0        0      496 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/analyticstories_investigations.j2
+-rw-r--r--   0        0        0      586 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/analyticstories_stories.j2
+-rw-r--r--   0        0        0      180 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/collections.j2
+-rw-r--r--   0        0        0      670 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/detection_count.j2
+-rw-r--r--   0        0        0      671 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/detection_coverage.j2
+-rw-r--r--   0        0        0     1002 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_detection_page.j2
+-rw-r--r--   0        0        0     6586 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_detections.j2
+-rw-r--r--   0        0        0     1471 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_navigation.j2
+-rw-r--r--   0        0        0      203 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_navigation_pages.j2
+-rw-r--r--   0        0        0     1681 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_playbooks.j2
+-rw-r--r--   0        0        0      679 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_playbooks_page.j2
+-rw-r--r--   0        0        0     1822 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_stories.j2
+-rw-r--r--   0        0        0      874 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/doc_story_page.j2
+-rw-r--r--   0        0        0      994 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/es_investigations_investigations.j2
+-rw-r--r--   0        0        0      369 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/es_investigations_stories.j2
+-rw-r--r--   0        0        0     1432 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/finding_report.j2
+-rw-r--r--   0        0        0      190 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/header.j2
+-rw-r--r--   0        0        0      424 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/macros.j2
+-rw-r--r--   0        0        0      282 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/macros_detections.j2
+-rw-r--r--   0        0        0      221 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/panel.j2
+-rw-r--r--   0        0        0     1840 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/savedsearches_baselines.j2
+-rw-r--r--   0        0        0     5290 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/savedsearches_detections.j2
+-rw-r--r--   0        0        0     1380 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/savedsearches_investigations.j2
+-rw-r--r--   0        0        0     1416 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/transforms.j2
+-rw-r--r--   0        0        0      925 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/templates/workflow_actions.j2
+-rw-r--r--   0        0        0      235 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/output/yml_writer.py
+-rw-r--r--   0        0        0     3843 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/templates/app_default.yml
+-rw-r--r--   0        0        0      662 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/templates/contentctl_default.yml
+-rw-r--r--   0        0        0     9381 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/templates/datamodels_cim.conf
+-rw-r--r--   0        0        0      480 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/templates/datamodels_custom.conf
+-rw-r--r--   0        0        0     3262 2023-06-12 22:32:39.586106 contentctl-1.0.1/contentctl/templates/detections/anomalous_usage_of_7zip.yml
+-rw-r--r--   0        0        0      159 2023-06-12 22:32:39.590106 contentctl-1.0.1/contentctl/templates/macros/security_content_ctime.yml
+-rw-r--r--   0        0        0      162 2023-06-12 22:32:39.590106 contentctl-1.0.1/contentctl/templates/macros/security_content_summariesonly.yml
+-rw-r--r--   0        0        0       90 2023-06-12 22:32:39.590106 contentctl-1.0.1/contentctl/templates/splunk_app/metadata/default.meta
+-rw-r--r--   0        0        0     3086 2023-06-12 22:32:39.590106 contentctl-1.0.1/contentctl/templates/stories/cobalt_strike.yml
+-rw-r--r--   0        0        0      501 2023-06-12 22:32:39.590106 contentctl-1.0.1/contentctl/templates/tests/anomalous_usage_of_7zip.test.yml
+-rw-r--r--   0        0        0      729 2023-06-12 22:32:39.590106 contentctl-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    18660 1970-01-01 00:00:00.000000 contentctl-1.0.1/PKG-INFO
```

### Comparing `contentctl-1.0.0/LICENSE.md` & `contentctl-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/README.md` & `contentctl-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,40 +4,37 @@
 <img src="docs/contentctl_logo_white.png" title="In case you're wondering, it's a capybara" alt="contentctl logo" width="250" height="250"></p>
 
 
 
 
 # Introduction
 #### Security Is Hard 
-Anyone who has managed a [SOC](acronym) will tell you it's hard work.  SOC Managers, Detection Engineers, and Cybersecurity Professionals must understand and manage countless tools and data sources while ensuring the reliability and security of their network and applications.  At the same time, they must be able to detect and react to data breeches, vulnerabilities, and performance degradation in minutes - not seconds or hours.
+Anyone who has managed a [SOC](#acronyms) will tell you it's hard work.  SOC Managers, Detection Engineers, and Cybersecurity Professionals must understand and manage countless tools and data sources while ensuring the reliability and security of their network and applications.  At the same time, they must be able to detect and react to data breeches, vulnerabilities, and performance degradation in minutes - not seconds or hours.
 These responsibilities leave little time for writing new content - let alone documentation, maintenance, and testing of legacy content.  Existing solutions like Wikis, JIRA tickets, Excel Spreadsheets, and "asking that one team member who knows everything" don't scale and spread information across various systems.       
 #### contentctl Makes It ~~Easy~~ Less Hard 
 contentctl is a single application that support the full cycle of security content development (each of the links below will redirect to the appropriate section of the README/Wiki):
 
-- [Create Content Packs](contentctl-init) - Version-Controlled collections of searches, documentation, and test data
-- [Add New Content](contentctl-new-content) - searches, macros, lookups, and other content
-- [Statically Validate](contentctl-validate) Content Against a Well-Defined Baseline
-- [Building](contentctl-build) a Content Pack for your target - Use a supported output format or design your own
-- [Generate](contentctl-generate) documentation, MITRE Maps, and a website that makes your Content Pack searchable and easy to understand  
-- [Test](contentctl-test) your Content Pack on a running Splunk Instance
-- [Deploy](contentctl-deploy) your Content Pack to Splunk Cloud Instance, via REST API, or create a Splunkbase Application for manual deployment   
- 
+- [Create Content Packs](#contentctl-init) - Version-Controlled collections of searches, documentation, and test data
+- [Add New Content](#contentctl-new---type-type) - searches, macros, lookups, and other content
+- [Statically Validate](#contentctl-validate) Content Against a Well-Defined Baseline
+- [Building](#contentctl-build) a Content Pack for your target - Use a supported output format or design your own
+- [Test](#contentctl-test) your Content Pack on a running Splunk Instance
+- [Deploy](#contentctl-deploy) your Content Pack to Splunk Cloud Instance, via REST API, or create a Splunkbase Application for manual deployment   
  
  
  # Ecosystem
 | Project               | Description                                             |
 | --------------------- | ------------------------------------------------------- |
 | [Splunk Attack Range](https://github.com/splunk/attack_range)          | Easily deploy a preconfigured Splunk Environment locally or on AWS containing a Splunk Instance, Windows and Linux Machines, and Attacker Tools like Kali Linux.  Automatically simulate attacks or run your own|
 | [PurpleSharp Attack Simulation](https://github.com/mvelazc0/PurpleSharp) | Open source adversary simulation tool for Windows Active Directory environments (integrated into Attack Range)|
 | [Red Canary Atomic Red Team](https://github.com/redcanaryco/atomic-red-team)          | Library of attack simulations mapped to the MITRE ATT&CK® framework (integrated into Attack Range)|
 | [Splunk Attack Data](https://github.com/splunk/attack_data)          | Repository of Attack Simulation Data for writing and Testing Detections|                         |
 | [Splunk Security Content](https://github.com/splunk/security_content)          | Splunk Threat Research Team's Content included in the [Enterprise Security Content Update App (ESCU)](https://splunkbase.splunk.com/app/3449)|
 | [Splunk contentctl](https://github.com/splunk/contentctl)          | Generate, validate, build, test, and deploy custom Security Content|
 | [SigmaHQ Sigma Rules](https://github.com/SigmaHQ/sigma) | Official Repository for Sigma Rules. These rules are an excellent starting point for new content. |
-| [Other Important Project(s)](https://github.com/otherorg/projectname)          | Additional projects that STRT uses or contributes to|
 
 
 
 
 ## Workflow
 ```mermaid
 graph TD
@@ -60,23 +57,25 @@
 | Operating System | Supported | Passing Intregration Tests | 
 | ---------------- | --------- | ------ |
 | Windows 10       | Yes       | Not tested yet |
 | Windows 11       | Yes       | Not tested yet |
 | Ununtu 20.04 LTS | Yes       | YES (locally + GitHub Actions) |
 | *Ubuntu 22.04 LTS| Yes       | YES (locally + GitHub Actions) |
 | macOS Montery 12       | Yes       | Not tested yet |
-| macOS Ventura 13       | Yes       | Yes (locally) |
+| macOS Ventura 13       | Yes (Intel and Apple Silicon)      | Yes (locally) |
 
-| Requirement | Required | Description |  Passing Integration Tests |
+| Requirement | Supported | Description |  Passing Integration Tests |
 | --------------------- | ----- | ---- | ------ |
-| Python <3.9 | Not Supported | No support planned.  contentctl tool uses modern language constructs not supported ion Python3.8 and below | N/A |
-| Python 3.9 | Required | contentctl tool is written in Python | Yes (locally + GitHub Actions) |
-| Python 3.10 | Not Supported (yet) | Will be supported | Yes (in GitHub Actions) |
-| Python 3.11 | Not Supported (yet) | Will be supported | Yes (in GitHub Actions)  |
-| Docker (local or remote) | Recommended | A running Splunk Server is required for Dynamic Testing.  contentctl can automatically create, configure, and destroy this server as a Splunk container during the lifetime of a test. | (locally + GitHub Actions) |
+| Python <3.9 | No | No support planned.  contentctl tool uses modern language constructs not supported ion Python3.8 and below | N/A |
+| Python 3.9 | Yes | contentctl tool is written in Python | Yes (locally + GitHub Actions) |
+| Python 3.10 | Yes | contentctl tool is written in Python | Yes (locally + GitHub Actions) |
+| Python 3.11 | Yes | contentctl tool is written in Python | Yes (locally + GitHub Actions)  |
+| Docker (local) | Yes | A running Splunk Server is required for Dynamic Testing.  contentctl can automatically create, configure, and destroy this server as a Splunk container during the lifetime of a test. | (locally + GitHub Actions) |
+| Docker (remote) | Planned | A running Splunk Server is required for Dynamic Testing.  contentctl can automatically create, configure, and destroy this server as a Splunk container during the lifetime of a test. | No |
+
 
 
 **Because contentctl uses a large number of dependencies, it's recommended to install contentctl in a virtual environment. 
 The instructions below use "poetry" and follow this recommendation.  Poetry will automatically create a new virtual environment for you.  
 It is typically recommended to install poetry to the Global Python Environment.**
 
 #### Install via pip (coming soon): 
@@ -84,57 +83,65 @@
 python3.9 -m venv .venv
 source .venv/bin/activate
 pip install splunk-contentctl
 ```
 
 #### From Source (advanced)
 ```
-git clone git@github.com:splunk/contentctl.git
+git clone https://github.com/splunk/contentctl
 cd contentctl
 python3.9 -m pip install poetry
 poetry install
 poetry shell
 contentctl --help
 ```
 
 
 # Usage
 
 ### contentctl init
-Creates a new Content Pack in the current directory as well as a configuration file called [contentctl.yml](contentctl.yml) which contains a number of important configuration options.
+Creates a new Content Pack in the current directory as well as a configuration file called [contentctl.yml](/contentctl/templates/contentctl_default.yml) which contains a number of important configuration options.
 The content pack contains a wide variety of content types:
-- [detections](detection)
-- [baselines](baseline)
-- [lookups](lookup)
-- [macros](macro)
-- [stories](story)
-
-### contentctl new [--type TYPE]
-Choose TYPE {detection, story} to create new content for the Content Pack.  The tool will interactively ask a series of questions required for generating a basic piece of content and automatically add it to the Content Pack.
+- [detections](/contentctl/objects/detection.py) - A piece of content that wraps and enriches a Splunk Search.  [Example Detection](/contentctl/templates/detections/anomalous_usage_of_7zip.yml)
+- [baselines](/contentctl/objects/baseline.py) - This content is not currently supported.
+- [lookups](/contentctl//objects/lookup.py) - Static files, such as CSVs, that can be loaded into Splunk for use in lookup commands.  [Example Lookup](https://github.com/splunk/security_content/blob/develop/lookups/attacker_tools.csv)
+- [macros](/contentctl/objects/macro.py) - Common code that is re-used across a wide set of detections.  [Example Macro](/contentctl/templates/macros/security_content_summariesonly.yml) 
+- [stories](/contentctl/objects/story.py) - Analytic Stories Allow a developer to tie together a group of detections, for example detections that all relate to Ransomware. [Example Analytic Story](/contentctl/templates/stories/cobalt_strike.yml)
 
 ### contentctl validate
 Performs static validation on all of the content in this Content Pack.  Writing validation is extremely complex.  Each piece of content can one or dozens of fields ranging from free text to numbers to references to other content.  contentctl's build in validation ensures that a number of conditions are met:
 - Required fields in content are defined
 - Values in fields are appropriate.  For example, if content references a Datamodel, then that Datamodel must be valid. Similarly, numeric values that must fall within a certain range must be validated.
 - If a piece of content references other content, then it exists.  For example, if a detection makes use of a macro then the existence and correctness of the macro must be validated.
 - There are no conflicts between content.  For example, two detections cannot have the same name.
 If any of these conditions are not met, then a descriptive error will be printed and contentctl will return a nonzero exit code.  This makes it suitable for running in an automated workflow or other CICD context.  Instead of exiting on the first error, _contentctl validate_ will continue validating all content so that it can present all relevant error before exiting.
 
 ### contentctl build
-Generates Content Packs in the output format defined in the [contentctl.yml](contentctl.yml) configuration file.  These outputs may include {splunk_app, api, ba}.  When _contentctl build_ runs, it first performs a _contentctl validate_ in order to ensure that a valid app is generated.  Note that it is *NOT* required or recommended to run _contentctl validate_ separately if the intention is to build a Content Pack.
+Generates Content Packs in the output format defined in the [contentctl.yml](/contentctl/templates/contentctl_default.yml) configuration file.  These outputs may include {splunk_app, api, ba}.  When _contentctl build_ runs, it first performs a _contentctl validate_ in order to ensure that a valid app is generated.  Note that it is *NOT* required or recommended to run _contentctl validate_ separately if the intention is to build a Content Pack.
+
+### contentctl report 
+This section is under active development.  It will allow you to a [MITRE Map](https://mitremap.splunkresearch.com/) showing your coverage of MITRE Techniques.  The link here shows the generation of that MITRE Map using the content in Splunk's [security_content repo](https://github.com/splunk/security_content).
+
+### contentctl new [--type TYPE]
+Choose TYPE {detection, story} to create new content for the Content Pack.  The tool will interactively ask a series of questions required for generating a basic piece of content and automatically add it to the Content Pack.
 
-### contentctl report
 ### contentctl inspect
+This section is under development.  It will enable the user to perform an appinspect of the content pack in preparation for deployment onto a Splunk Instance or via Splunk Cloud.
+
 ### contentctl deploy
-The reason to build content is so that it can be deployed to your environment.  However, deploying content to multiple servers and different types of infrastructure can be tricky and time-consuming.  contentctl makes this easy by supporting a number of different deployment mechanisms. Deployment targets can be defined in [contentctl.yml](contentctl.yml).
+The reason to build content is so that it can be deployed to your environment.  However, deploying content to multiple servers and different types of infrastructure can be tricky and time-consuming.  contentctl makes this easy by supporting a number of different deployment mechanisms. Deployment targets can be defined in [contentctl.yml](/contentctl/templates/contentctl_default.yml).
 - Deploy via API - Using the REST API, individual pieces of content are deployed to a running server.  This is a great way to deploy all of the content in a content pack, but can also be used to deploy individual peices of content.
 - Deploy to Splunk Cloud via ACS - Using the Automated Private App Vetting (APAV) Feature of the Admin Config Service (ACS), Splunk Cloud customers can easily deploy custom apps to their environments.   
+
 ### contentctl docs
+This section is under active development.  It will allow you to easily generate verbose [web-based documentation](https://research.splunk.com) from all of your content.  The link here shows the generation of that documentation using the content in Splunk's [security_content repo](https://github.com/splunk/security_content).
+
 ### contentctl test
-The static validation performed by *contentctl validate* can only take you so far.  While it's powerful, and fast, it can only tell determine if the content is *syntactically* correct.  *contentctl test* can test your content on real Splunk Infrastructure to ensure there are no errors in your SPL, raw data can be properly ingested/processed/accelerated on your server, your search finds the event(s) you're looking for in raw data, and even provides high-level runtime performance metrics about your searches.    The following diagram shows this workflow at a high level
+The static validation performed by *contentctl validate* can only take you so far.  While it's powerful, and fast, it can only tell determine if the content is *syntactically* correct.  *contentctl test* can test your content on real Splunk Infrastructure to ensure there are no errors in your SPL, raw data can be properly ingested/processed/accelerated on your server, your search finds the event(s) you're looking for in raw data, and even provides high-level runtime performance metrics about your searches.    As part of this workflow, a large number of apps will be installed by default.  You can see, and edit, the list of apps in the [app_default.yml](/contentctl/templates/app_default.yml) file.  We plan on making this even easier to update in the future, so stay tuned for updates.
+The following diagram shows this workflow at a high level.
 
 ```mermaid
 graph TD
 SplunkContainer--start-->SplunkInstance
 SplunkServer-->SplunkInstance
 SplunkInstance--Install Apps-->ConfiguredInstance
 SplunkInstance--Configure Settings-->ConfiguredInstance
@@ -175,15 +182,15 @@
 
 # Acronyms
 | Acronym | Meaning| Description | 
 | --------------------- | ------------------------------------------------------- | ---- |
 | SOC | Security Operation Center | Description of a SoC | 
 | DaC | Detection as Code | A systematic approach applying DevOps priciples to Detection Engineering. DaC enables Continuous Integration and Continuous Delivery of Detectionsa via automated validation, testing, and deployment |
 | CICD | Continuous Integration/Continuous Delivery | A modern DevOps practice that encourages users to make small, frequent changes which are automatically tested and deployed. This contrasts with legacy approaches that emphasize large changes which may be manually tested an infrequently deployed. |
-| ACS| Admin Config Service | The [Splunk Admin Configu Service](https://docs.splunk.com/Documentation/SplunkCloud/9.0.2209/Config/ACSIntro) is a cloud-native API that provides programmatic self-service administration capabilities for Splunk Cloud Platform. One of its features, Automated Private App Vetting (APAV) enables the installation of custom app on Splunk Cloud instances. | 
+| ACS| Admin Config Service | The [Splunk Admin Config Service](https://docs.splunk.com/Documentation/SplunkCloud/9.0.2209/Config/ACSIntro) is a cloud-native API that provides programmatic self-service administration capabilities for Splunk Cloud Platform. One of its features, Automated Private App Vetting (APAV) enables the installation of custom app on Splunk Cloud instances. | 
 | APAV | Automated Private App Vetting | [Automated Private App Vetting](https://docs.splunk.com/Documentation/SplunkCloud/9.0.2209/Config/ManageApps) enables admins to use the ACS API to install, upgrade, and uninstall apps directly on your Splunk Cloud Platform deployment without assistance from Splunk Support. |
 
 
 # License
 Copyright 2023 Splunk Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at
```

### Comparing `contentctl-1.0.0/contentctl/actions/deploy.py` & `contentctl-1.0.1/contentctl/actions/deploy.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/detection_testing/DataManipulation.py` & `contentctl-1.0.1/contentctl/actions/detection_testing/DataManipulation.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/detection_testing/DetectionTestingManager.py` & `contentctl-1.0.1/contentctl/actions/detection_testing/DetectionTestingManager.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/detection_testing/GitHubService.py` & `contentctl-1.0.1/contentctl/actions/detection_testing/GitHubService.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/detection_testing/generate_detection_coverage_badge.py` & `contentctl-1.0.1/contentctl/actions/detection_testing/generate_detection_coverage_badge.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py` & `contentctl-1.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructure.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py` & `contentctl-1.0.1/contentctl/actions/detection_testing/infrastructures/DetectionTestingInfrastructureContainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         container = self.get_docker_client().containers.create(
             self.config.full_image_path,
             ports=ports_dict,
             environment=environment,
             name=self.get_name(),
             mounts=mounts,
             detach=True,
+            platform="linux/amd64"
         )
 
         return container
 
     def removeContainer(self, removeVolumes: bool = True, forceRemove: bool = True):
 
         try:
```

### Comparing `contentctl-1.0.0/contentctl/actions/detection_testing/views/DetectionTestingView.py` & `contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingView.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py` & `contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewCLI.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py` & `contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewFile.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py` & `contentctl-1.0.1/contentctl/actions/detection_testing/views/DetectionTestingViewWeb.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/doc_gen.py` & `contentctl-1.0.1/contentctl/actions/doc_gen.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/generate.py` & `contentctl-1.0.1/contentctl/actions/generate.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/initialize.py` & `contentctl-1.0.1/contentctl/actions/initialize.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/initialize_old.py` & `contentctl-1.0.1/contentctl/actions/initialize_old.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/new_content.py` & `contentctl-1.0.1/contentctl/actions/new_content.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/reporting.py` & `contentctl-1.0.1/contentctl/actions/reporting.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/test.py` & `contentctl-1.0.1/contentctl/actions/test.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/actions/validate.py` & `contentctl-1.0.1/contentctl/actions/validate.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/contentctl.py` & `contentctl-1.0.1/contentctl/contentctl.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/enrichments/attack_enrichment.py` & `contentctl-1.0.1/contentctl/enrichments/attack_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/enrichments/cve_enrichment.py` & `contentctl-1.0.1/contentctl/enrichments/cve_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/enrichments/splunk_app_enrichment.py` & `contentctl-1.0.1/contentctl/enrichments/splunk_app_enrichment.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/helper/config_handler.py` & `contentctl-1.0.1/contentctl/helper/config_handler.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/helper/link_validator.py` & `contentctl-1.0.1/contentctl/helper/link_validator.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/helper/utils.py` & `contentctl-1.0.1/contentctl/helper/utils.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/input/baseline_builder.py` & `contentctl-1.0.1/contentctl/input/baseline_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/input/basic_builder.py` & `contentctl-1.0.1/contentctl/input/basic_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/input/detection_builder.py` & `contentctl-1.0.1/contentctl/input/detection_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/input/director.py` & `contentctl-1.0.1/contentctl/input/director.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/input/investigation_builder.py` & `contentctl-1.0.1/contentctl/input/investigation_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/input/new_content_generator.py` & `contentctl-1.0.1/contentctl/input/new_content_generator.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/input/new_content_questions.py` & `contentctl-1.0.1/contentctl/input/new_content_questions.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/input/playbook_builder.py` & `contentctl-1.0.1/contentctl/input/playbook_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/input/story_builder.py` & `contentctl-1.0.1/contentctl/input/story_builder.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/input/yml_reader.py` & `contentctl-1.0.1/contentctl/input/yml_reader.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/app.py` & `contentctl-1.0.1/contentctl/objects/app.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/baseline.py` & `contentctl-1.0.1/contentctl/objects/baseline.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/baseline_tags.py` & `contentctl-1.0.1/contentctl/objects/baseline_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/config.py` & `contentctl-1.0.1/contentctl/objects/config.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/constants.py` & `contentctl-1.0.1/contentctl/objects/constants.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/deployment.py` & `contentctl-1.0.1/contentctl/objects/deployment.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/detection.py` & `contentctl-1.0.1/contentctl/objects/detection.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/detection_tags.py` & `contentctl-1.0.1/contentctl/objects/detection_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/enums.py` & `contentctl-1.0.1/contentctl/objects/enums.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/investigation.py` & `contentctl-1.0.1/contentctl/objects/investigation.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/playbook.py` & `contentctl-1.0.1/contentctl/objects/playbook.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/repo_config.py` & `contentctl-1.0.1/contentctl/objects/repo_config.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/story.py` & `contentctl-1.0.1/contentctl/objects/story.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/story_tags.py` & `contentctl-1.0.1/contentctl/objects/story_tags.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/test_config.py` & `contentctl-1.0.1/contentctl/objects/test_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
                 # connectivity to docker server is validated previously
                 client = docker.from_env()
                 print(
                     f"Getting the latest version of the container image: {v}...",
                     end="",
                     flush=True,
                 )
-                client.images.pull(v)
+                client.images.pull(v, platform="linux/amd64")
                 print("done")
             except docker.errors.APIError as e:
                 print("error")
                 if e.is_client_error():
                     if "invalid reference format" in str(e.explanation):
                         simple_explanation = f"The format of the docker image reference is incorrect. Please use a valid image reference"
                     else:
```

### Comparing `contentctl-1.0.0/contentctl/objects/unit_test_attack_data.py` & `contentctl-1.0.1/contentctl/objects/unit_test_attack_data.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/unit_test_result.py` & `contentctl-1.0.1/contentctl/objects/unit_test_result.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/objects/unit_test_test.py` & `contentctl-1.0.1/contentctl/objects/unit_test_test.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/api_json_output.py` & `contentctl-1.0.1/contentctl/output/api_json_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/attack_nav_output.py` & `contentctl-1.0.1/contentctl/output/attack_nav_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/attack_nav_writer.py` & `contentctl-1.0.1/contentctl/output/attack_nav_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/ba_yml_output.py` & `contentctl-1.0.1/contentctl/output/ba_yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/conf_output.py` & `contentctl-1.0.1/contentctl/output/conf_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/conf_writer.py` & `contentctl-1.0.1/contentctl/output/conf_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/doc_md_output.py` & `contentctl-1.0.1/contentctl/output/doc_md_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/finding_report_writer.py` & `contentctl-1.0.1/contentctl/output/finding_report_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/jinja_writer.py` & `contentctl-1.0.1/contentctl/output/jinja_writer.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/new_content_yml_output.py` & `contentctl-1.0.1/contentctl/output/new_content_yml_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/svg_output.py` & `contentctl-1.0.1/contentctl/output/svg_output.py`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/analyticstories_detections.j2` & `contentctl-1.0.1/contentctl/output/templates/analyticstories_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/analyticstories_stories.j2` & `contentctl-1.0.1/contentctl/output/templates/analyticstories_stories.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/detection_count.j2` & `contentctl-1.0.1/contentctl/output/templates/detection_count.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/detection_coverage.j2` & `contentctl-1.0.1/contentctl/output/templates/detection_coverage.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/doc_detection_page.j2` & `contentctl-1.0.1/contentctl/output/templates/doc_detection_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/doc_detections.j2` & `contentctl-1.0.1/contentctl/output/templates/doc_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/doc_navigation.j2` & `contentctl-1.0.1/contentctl/output/templates/doc_navigation.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/doc_playbooks.j2` & `contentctl-1.0.1/contentctl/output/templates/doc_playbooks.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/doc_playbooks_page.j2` & `contentctl-1.0.1/contentctl/output/templates/doc_playbooks_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/doc_stories.j2` & `contentctl-1.0.1/contentctl/output/templates/doc_stories.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/doc_story_page.j2` & `contentctl-1.0.1/contentctl/output/templates/doc_story_page.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/es_investigations_investigations.j2` & `contentctl-1.0.1/contentctl/output/templates/es_investigations_investigations.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/finding_report.j2` & `contentctl-1.0.1/contentctl/output/templates/finding_report.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/savedsearches_baselines.j2` & `contentctl-1.0.1/contentctl/output/templates/savedsearches_baselines.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/savedsearches_detections.j2` & `contentctl-1.0.1/contentctl/output/templates/savedsearches_detections.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/savedsearches_investigations.j2` & `contentctl-1.0.1/contentctl/output/templates/savedsearches_investigations.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/transforms.j2` & `contentctl-1.0.1/contentctl/output/templates/transforms.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/output/templates/workflow_actions.j2` & `contentctl-1.0.1/contentctl/output/templates/workflow_actions.j2`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/templates/app_default.yml` & `contentctl-1.0.1/contentctl/templates/app_default.yml`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/templates/contentctl_default.yml` & `contentctl-1.0.1/contentctl/templates/contentctl_default.yml`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/templates/datamodels_cim.conf` & `contentctl-1.0.1/contentctl/templates/datamodels_cim.conf`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/templates/detections/anomalous_usage_of_7zip.yml` & `contentctl-1.0.1/contentctl/templates/detections/anomalous_usage_of_7zip.yml`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/contentctl/templates/stories/cobalt_strike.yml` & `contentctl-1.0.1/contentctl/templates/stories/cobalt_strike.yml`

 * *Files identical despite different names*

### Comparing `contentctl-1.0.0/pyproject.toml` & `contentctl-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "contentctl"
-version = "1.0.0"
+version = "1.0.1"
 description = "Splunk Content Control Tool"
 authors = ["STRT <research@splunk.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
-contentctl = 'splunk_contentctl.contentctl:main'
+contentctl = 'contentctl.contentctl:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^1.10.2"
 PyYAML = "^6.0"
 requests = "^2.28.1"
 pycvesearch = "^1.2"
```

### Comparing `contentctl-1.0.0/setup.py` & `contentctl-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,231 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: contentctl
+Version: 1.0.1
+Summary: Splunk Content Control Tool
+License: Apache 2.0
+Author: STRT
+Author-email: research@splunk.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: attackcti (>=0.3.7,<0.4.0)
+Requires-Dist: bottle (>=0.12.23,<0.13.0)
+Requires-Dist: docker (>=6.0.1,<7.0.0)
+Requires-Dist: gitpython (>=3.1.29,<4.0.0)
+Requires-Dist: pycvesearch (>=1.2,<2.0)
+Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: questionary (>=1.10.0,<2.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
+Requires-Dist: splunk-sdk (>=1.7.2,<2.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: validators (>=0.20.0,<0.21.0)
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Description-Content-Type: text/markdown
+
+
+# contentctl
+<p align="center">
+<img src="docs/contentctl_logo_white.png" title="In case you're wondering, it's a capybara" alt="contentctl logo" width="250" height="250"></p>
+
+
+
+
+# Introduction
+#### Security Is Hard 
+Anyone who has managed a [SOC](#acronyms) will tell you it's hard work.  SOC Managers, Detection Engineers, and Cybersecurity Professionals must understand and manage countless tools and data sources while ensuring the reliability and security of their network and applications.  At the same time, they must be able to detect and react to data breeches, vulnerabilities, and performance degradation in minutes - not seconds or hours.
+These responsibilities leave little time for writing new content - let alone documentation, maintenance, and testing of legacy content.  Existing solutions like Wikis, JIRA tickets, Excel Spreadsheets, and "asking that one team member who knows everything" don't scale and spread information across various systems.       
+#### contentctl Makes It ~~Easy~~ Less Hard 
+contentctl is a single application that support the full cycle of security content development (each of the links below will redirect to the appropriate section of the README/Wiki):
+
+- [Create Content Packs](#contentctl-init) - Version-Controlled collections of searches, documentation, and test data
+- [Add New Content](#contentctl-new---type-type) - searches, macros, lookups, and other content
+- [Statically Validate](#contentctl-validate) Content Against a Well-Defined Baseline
+- [Building](#contentctl-build) a Content Pack for your target - Use a supported output format or design your own
+- [Test](#contentctl-test) your Content Pack on a running Splunk Instance
+- [Deploy](#contentctl-deploy) your Content Pack to Splunk Cloud Instance, via REST API, or create a Splunkbase Application for manual deployment   
+ 
+ 
+ # Ecosystem
+| Project               | Description                                             |
+| --------------------- | ------------------------------------------------------- |
+| [Splunk Attack Range](https://github.com/splunk/attack_range)          | Easily deploy a preconfigured Splunk Environment locally or on AWS containing a Splunk Instance, Windows and Linux Machines, and Attacker Tools like Kali Linux.  Automatically simulate attacks or run your own|
+| [PurpleSharp Attack Simulation](https://github.com/mvelazc0/PurpleSharp) | Open source adversary simulation tool for Windows Active Directory environments (integrated into Attack Range)|
+| [Red Canary Atomic Red Team](https://github.com/redcanaryco/atomic-red-team)          | Library of attack simulations mapped to the MITRE ATT&CK® framework (integrated into Attack Range)|
+| [Splunk Attack Data](https://github.com/splunk/attack_data)          | Repository of Attack Simulation Data for writing and Testing Detections|                         |
+| [Splunk Security Content](https://github.com/splunk/security_content)          | Splunk Threat Research Team's Content included in the [Enterprise Security Content Update App (ESCU)](https://splunkbase.splunk.com/app/3449)|
+| [Splunk contentctl](https://github.com/splunk/contentctl)          | Generate, validate, build, test, and deploy custom Security Content|
+| [SigmaHQ Sigma Rules](https://github.com/SigmaHQ/sigma) | Official Repository for Sigma Rules. These rules are an excellent starting point for new content. |
+
+
+
+
+## Workflow
+```mermaid
+graph TD
+starting_state --contentctl init--> contentPack 
+newContent{new_content} --contentctl new sigma content--> contentPack
+newContent{new_content} --contentctl new spl content--> contentPack
+contentPack --contentctl validate--> ValidatedContent
+ValidatedContent --contentctl build--> SplunkContent
+ValidatedContent --contentctl docs--> WebsiteDocumentation
+ValidatedContent --contentctl docs--> MITRE_mapDocumentation
+SplunkContent --contentctl test via container-->TestResults
+TestResults --contentctl deploy-->SplunkRESTAPI
+TestResults --contentctl deploy-->SplunkbaseApp
+TestResults --contentctl deploy-->SplunkCloudInstance
+```
+
+## Installation
+### Requirements
+Testing is run using [GitHub Hosted Runners](https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners).  Ubuntu22.04 is the recommended configuration.
+| Operating System | Supported | Passing Intregration Tests | 
+| ---------------- | --------- | ------ |
+| Windows 10       | Yes       | Not tested yet |
+| Windows 11       | Yes       | Not tested yet |
+| Ununtu 20.04 LTS | Yes       | YES (locally + GitHub Actions) |
+| *Ubuntu 22.04 LTS| Yes       | YES (locally + GitHub Actions) |
+| macOS Montery 12       | Yes       | Not tested yet |
+| macOS Ventura 13       | Yes (Intel and Apple Silicon)      | Yes (locally) |
+
+| Requirement | Supported | Description |  Passing Integration Tests |
+| --------------------- | ----- | ---- | ------ |
+| Python <3.9 | No | No support planned.  contentctl tool uses modern language constructs not supported ion Python3.8 and below | N/A |
+| Python 3.9 | Yes | contentctl tool is written in Python | Yes (locally + GitHub Actions) |
+| Python 3.10 | Yes | contentctl tool is written in Python | Yes (locally + GitHub Actions) |
+| Python 3.11 | Yes | contentctl tool is written in Python | Yes (locally + GitHub Actions)  |
+| Docker (local) | Yes | A running Splunk Server is required for Dynamic Testing.  contentctl can automatically create, configure, and destroy this server as a Splunk container during the lifetime of a test. | (locally + GitHub Actions) |
+| Docker (remote) | Planned | A running Splunk Server is required for Dynamic Testing.  contentctl can automatically create, configure, and destroy this server as a Splunk container during the lifetime of a test. | No |
+
+
+
+**Because contentctl uses a large number of dependencies, it's recommended to install contentctl in a virtual environment. 
+The instructions below use "poetry" and follow this recommendation.  Poetry will automatically create a new virtual environment for you.  
+It is typically recommended to install poetry to the Global Python Environment.**
+
+#### Install via pip (coming soon): 
+```
+python3.9 -m venv .venv
+source .venv/bin/activate
+pip install splunk-contentctl
+```
+
+#### From Source (advanced)
+```
+git clone https://github.com/splunk/contentctl
+cd contentctl
+python3.9 -m pip install poetry
+poetry install
+poetry shell
+contentctl --help
+```
+
+
+# Usage
+
+### contentctl init
+Creates a new Content Pack in the current directory as well as a configuration file called [contentctl.yml](/contentctl/templates/contentctl_default.yml) which contains a number of important configuration options.
+The content pack contains a wide variety of content types:
+- [detections](/contentctl/objects/detection.py) - A piece of content that wraps and enriches a Splunk Search.  [Example Detection](/contentctl/templates/detections/anomalous_usage_of_7zip.yml)
+- [baselines](/contentctl/objects/baseline.py) - This content is not currently supported.
+- [lookups](/contentctl//objects/lookup.py) - Static files, such as CSVs, that can be loaded into Splunk for use in lookup commands.  [Example Lookup](https://github.com/splunk/security_content/blob/develop/lookups/attacker_tools.csv)
+- [macros](/contentctl/objects/macro.py) - Common code that is re-used across a wide set of detections.  [Example Macro](/contentctl/templates/macros/security_content_summariesonly.yml) 
+- [stories](/contentctl/objects/story.py) - Analytic Stories Allow a developer to tie together a group of detections, for example detections that all relate to Ransomware. [Example Analytic Story](/contentctl/templates/stories/cobalt_strike.yml)
+
+### contentctl validate
+Performs static validation on all of the content in this Content Pack.  Writing validation is extremely complex.  Each piece of content can one or dozens of fields ranging from free text to numbers to references to other content.  contentctl's build in validation ensures that a number of conditions are met:
+- Required fields in content are defined
+- Values in fields are appropriate.  For example, if content references a Datamodel, then that Datamodel must be valid. Similarly, numeric values that must fall within a certain range must be validated.
+- If a piece of content references other content, then it exists.  For example, if a detection makes use of a macro then the existence and correctness of the macro must be validated.
+- There are no conflicts between content.  For example, two detections cannot have the same name.
+If any of these conditions are not met, then a descriptive error will be printed and contentctl will return a nonzero exit code.  This makes it suitable for running in an automated workflow or other CICD context.  Instead of exiting on the first error, _contentctl validate_ will continue validating all content so that it can present all relevant error before exiting.
+
+### contentctl build
+Generates Content Packs in the output format defined in the [contentctl.yml](/contentctl/templates/contentctl_default.yml) configuration file.  These outputs may include {splunk_app, api, ba}.  When _contentctl build_ runs, it first performs a _contentctl validate_ in order to ensure that a valid app is generated.  Note that it is *NOT* required or recommended to run _contentctl validate_ separately if the intention is to build a Content Pack.
+
+### contentctl report 
+This section is under active development.  It will allow you to a [MITRE Map](https://mitremap.splunkresearch.com/) showing your coverage of MITRE Techniques.  The link here shows the generation of that MITRE Map using the content in Splunk's [security_content repo](https://github.com/splunk/security_content).
+
+### contentctl new [--type TYPE]
+Choose TYPE {detection, story} to create new content for the Content Pack.  The tool will interactively ask a series of questions required for generating a basic piece of content and automatically add it to the Content Pack.
+
+### contentctl inspect
+This section is under development.  It will enable the user to perform an appinspect of the content pack in preparation for deployment onto a Splunk Instance or via Splunk Cloud.
+
+### contentctl deploy
+The reason to build content is so that it can be deployed to your environment.  However, deploying content to multiple servers and different types of infrastructure can be tricky and time-consuming.  contentctl makes this easy by supporting a number of different deployment mechanisms. Deployment targets can be defined in [contentctl.yml](/contentctl/templates/contentctl_default.yml).
+- Deploy via API - Using the REST API, individual pieces of content are deployed to a running server.  This is a great way to deploy all of the content in a content pack, but can also be used to deploy individual peices of content.
+- Deploy to Splunk Cloud via ACS - Using the Automated Private App Vetting (APAV) Feature of the Admin Config Service (ACS), Splunk Cloud customers can easily deploy custom apps to their environments.   
+
+### contentctl docs
+This section is under active development.  It will allow you to easily generate verbose [web-based documentation](https://research.splunk.com) from all of your content.  The link here shows the generation of that documentation using the content in Splunk's [security_content repo](https://github.com/splunk/security_content).
+
+### contentctl test
+The static validation performed by *contentctl validate* can only take you so far.  While it's powerful, and fast, it can only tell determine if the content is *syntactically* correct.  *contentctl test* can test your content on real Splunk Infrastructure to ensure there are no errors in your SPL, raw data can be properly ingested/processed/accelerated on your server, your search finds the event(s) you're looking for in raw data, and even provides high-level runtime performance metrics about your searches.    As part of this workflow, a large number of apps will be installed by default.  You can see, and edit, the list of apps in the [app_default.yml](/contentctl/templates/app_default.yml) file.  We plan on making this even easier to update in the future, so stay tuned for updates.
+The following diagram shows this workflow at a high level.
+
+```mermaid
+graph TD
+SplunkContainer--start-->SplunkInstance
+SplunkServer-->SplunkInstance
+SplunkInstance--Install Apps-->ConfiguredInstance
+SplunkInstance--Configure Settings-->ConfiguredInstance
+ContentPack--Deploy-->ConfiguredInstance
+ConfiguredInstance--Start Test-->Testing
+Testing--Test Detection-->Detection
+
+Detection--Replay Raw Data-->Result
+subgraph Test Indidivual Detection
+	Detection--Execute Search-->Result	
+end
+Result--Cleanup-->Testing
+Testing--Cleanup-->TestResults
+```
+
+#### Testing Modes
+There are a number of different testing modes that control which content will be tested.  This can be controlled with the `--mode {}` option at the command line
+- all - This will test all of the content in the content pack. Please note that by default only detections marked production will be tested (detections marked as deprecated or experimental, for example, will be ignored).
+- selected - Detections whose relative paths are provided on the command line will be tested.  This is particularly useful if you would like to troubleshoot or update just a handful of detections and can save a significant amount of time.  For example, to test two detections use the following command `contentctl test --mode selected --detections_list detections/detection_one.yml detections/detection_two.yml`
+- **changes - (not currently supported) If you have a large number of detections and use a branching workflow to create new content or update content, then this is an easy way to automatically find and test only that content automatically.  This prevents you from needing to explicitly list the subset of content to test using "selected"** 
+
+#### Testing Behavior
+contentctl test's default mode allows it to quickly test all content with requiring user interaction.  This makes it suitable for local tests as well as CI/CD workflows.  However, users often want to troubleshoot a test if it fails.  contentctl allows you to change the tool's behavior if and/or when a test fails:
+- --behavior never_pause - The default behavior.  If a test does not pass, the tool begins the next test immediately
+- --behavior pause_on_failure - If a test fails, then additional information about that test, and the raw SPL of the test, is printed to the terminal.  A user may then click (or CMD+Click) the "LINK" to begin interactively debugging the failed test on the Splunk Server.  Note that the credentials for the server are printed out at the very beginning of the test.  After you have finished debugging the failure, hit "Return" in the terminal to move on to the next test. The attack_data for this test remains loaded on the server for debugging until the user moves on to the next test.
+- --behavior always_pause - Similar to pause_on_failure, but this pauses after every test regardless of whether it passes or fails.  
+
+
+1. **init** - Initilialize a new repo from scratch so you can easily add your own content to a custom application. 
+2. **new** - Creates new content (detection, story)
+3. **validate** - Validates written content
+4. **build** - Builds an application suitable for deployment on a search head using Slim, the Splunk Packaging Toolkit
+5. **deploy** - Deploy the security content pack to a Splunk Server
+6. **docs** - Create documentation as Markdown
+7. **reporting** - Create different reporting files such as a Mitre ATT&CK overlay
+
+
+
+# Acronyms
+| Acronym | Meaning| Description | 
+| --------------------- | ------------------------------------------------------- | ---- |
+| SOC | Security Operation Center | Description of a SoC | 
+| DaC | Detection as Code | A systematic approach applying DevOps priciples to Detection Engineering. DaC enables Continuous Integration and Continuous Delivery of Detectionsa via automated validation, testing, and deployment |
+| CICD | Continuous Integration/Continuous Delivery | A modern DevOps practice that encourages users to make small, frequent changes which are automatically tested and deployed. This contrasts with legacy approaches that emphasize large changes which may be manually tested an infrequently deployed. |
+| ACS| Admin Config Service | The [Splunk Admin Config Service](https://docs.splunk.com/Documentation/SplunkCloud/9.0.2209/Config/ACSIntro) is a cloud-native API that provides programmatic self-service administration capabilities for Splunk Cloud Platform. One of its features, Automated Private App Vetting (APAV) enables the installation of custom app on Splunk Cloud instances. | 
+| APAV | Automated Private App Vetting | [Automated Private App Vetting](https://docs.splunk.com/Documentation/SplunkCloud/9.0.2209/Config/ManageApps) enables admins to use the ACS API to install, upgrade, and uninstall apps directly on your Splunk Cloud Platform deployment without assistance from Splunk Support. |
 
-packages = \
-['contentctl',
- 'contentctl.actions',
- 'contentctl.actions.detection_testing',
- 'contentctl.actions.detection_testing.infrastructures',
- 'contentctl.actions.detection_testing.views',
- 'contentctl.enrichments',
- 'contentctl.helper',
- 'contentctl.input',
- 'contentctl.objects',
- 'contentctl.output']
-
-package_data = \
-{'': ['*'],
- 'contentctl': ['templates/*',
-                'templates/detections/*',
-                'templates/macros/*',
-                'templates/splunk_app/metadata/*',
-                'templates/stories/*',
-                'templates/tests/*'],
- 'contentctl.output': ['templates/*']}
-
-install_requires = \
-['Jinja2>=3.1.2,<4.0.0',
- 'PyYAML>=6.0,<7.0',
- 'attackcti>=0.3.7,<0.4.0',
- 'bottle>=0.12.23,<0.13.0',
- 'docker>=6.0.1,<7.0.0',
- 'gitpython>=3.1.29,<4.0.0',
- 'pycvesearch>=1.2,<2.0',
- 'pydantic>=1.10.2,<2.0.0',
- 'questionary>=1.10.0,<2.0.0',
- 'requests>=2.28.1,<3.0.0',
- 'semantic-version>=2.10.0,<3.0.0',
- 'splunk-sdk>=1.7.2,<2.0.0',
- 'tqdm>=4.65.0,<5.0.0',
- 'validators>=0.20.0,<0.21.0',
- 'xmltodict>=0.13.0,<0.14.0']
-
-entry_points = \
-{'console_scripts': ['contentctl = splunk_contentctl.contentctl:main']}
-
-setup_kwargs = {
-    'name': 'contentctl',
-    'version': '1.0.0',
-    'description': 'Splunk Content Control Tool',
-    'long_description': '\n# contentctl\n<p align="center">\n<img src="docs/contentctl_logo_white.png" title="In case you\'re wondering, it\'s a capybara" alt="contentctl logo" width="250" height="250"></p>\n\n\n\n\n# Introduction\n#### Security Is Hard \nAnyone who has managed a [SOC](acronym) will tell you it\'s hard work.  SOC Managers, Detection Engineers, and Cybersecurity Professionals must understand and manage countless tools and data sources while ensuring the reliability and security of their network and applications.  At the same time, they must be able to detect and react to data breeches, vulnerabilities, and performance degradation in minutes - not seconds or hours.\nThese responsibilities leave little time for writing new content - let alone documentation, maintenance, and testing of legacy content.  Existing solutions like Wikis, JIRA tickets, Excel Spreadsheets, and "asking that one team member who knows everything" don\'t scale and spread information across various systems.       \n#### contentctl Makes It ~~Easy~~ Less Hard \ncontentctl is a single application that support the full cycle of security content development (each of the links below will redirect to the appropriate section of the README/Wiki):\n\n- [Create Content Packs](contentctl-init) - Version-Controlled collections of searches, documentation, and test data\n- [Add New Content](contentctl-new-content) - searches, macros, lookups, and other content\n- [Statically Validate](contentctl-validate) Content Against a Well-Defined Baseline\n- [Building](contentctl-build) a Content Pack for your target - Use a supported output format or design your own\n- [Generate](contentctl-generate) documentation, MITRE Maps, and a website that makes your Content Pack searchable and easy to understand  \n- [Test](contentctl-test) your Content Pack on a running Splunk Instance\n- [Deploy](contentctl-deploy) your Content Pack to Splunk Cloud Instance, via REST API, or create a Splunkbase Application for manual deployment   \n \n \n \n # Ecosystem\n| Project               | Description                                             |\n| --------------------- | ------------------------------------------------------- |\n| [Splunk Attack Range](https://github.com/splunk/attack_range)          | Easily deploy a preconfigured Splunk Environment locally or on AWS containing a Splunk Instance, Windows and Linux Machines, and Attacker Tools like Kali Linux.  Automatically simulate attacks or run your own|\n| [PurpleSharp Attack Simulation](https://github.com/mvelazc0/PurpleSharp) | Open source adversary simulation tool for Windows Active Directory environments (integrated into Attack Range)|\n| [Red Canary Atomic Red Team](https://github.com/redcanaryco/atomic-red-team)          | Library of attack simulations mapped to the MITRE ATT&CK® framework (integrated into Attack Range)|\n| [Splunk Attack Data](https://github.com/splunk/attack_data)          | Repository of Attack Simulation Data for writing and Testing Detections|                         |\n| [Splunk Security Content](https://github.com/splunk/security_content)          | Splunk Threat Research Team\'s Content included in the [Enterprise Security Content Update App (ESCU)](https://splunkbase.splunk.com/app/3449)|\n| [Splunk contentctl](https://github.com/splunk/contentctl)          | Generate, validate, build, test, and deploy custom Security Content|\n| [SigmaHQ Sigma Rules](https://github.com/SigmaHQ/sigma) | Official Repository for Sigma Rules. These rules are an excellent starting point for new content. |\n| [Other Important Project(s)](https://github.com/otherorg/projectname)          | Additional projects that STRT uses or contributes to|\n\n\n\n\n## Workflow\n```mermaid\ngraph TD\nstarting_state --contentctl init--> contentPack \nnewContent{new_content} --contentctl new sigma content--> contentPack\nnewContent{new_content} --contentctl new spl content--> contentPack\ncontentPack --contentctl validate--> ValidatedContent\nValidatedContent --contentctl build--> SplunkContent\nValidatedContent --contentctl docs--> WebsiteDocumentation\nValidatedContent --contentctl docs--> MITRE_mapDocumentation\nSplunkContent --contentctl test via container-->TestResults\nTestResults --contentctl deploy-->SplunkRESTAPI\nTestResults --contentctl deploy-->SplunkbaseApp\nTestResults --contentctl deploy-->SplunkCloudInstance\n```\n\n## Installation\n### Requirements\nTesting is run using [GitHub Hosted Runners](https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners).  Ubuntu22.04 is the recommended configuration.\n| Operating System | Supported | Passing Intregration Tests | \n| ---------------- | --------- | ------ |\n| Windows 10       | Yes       | Not tested yet |\n| Windows 11       | Yes       | Not tested yet |\n| Ununtu 20.04 LTS | Yes       | YES (locally + GitHub Actions) |\n| *Ubuntu 22.04 LTS| Yes       | YES (locally + GitHub Actions) |\n| macOS Montery 12       | Yes       | Not tested yet |\n| macOS Ventura 13       | Yes       | Yes (locally) |\n\n| Requirement | Required | Description |  Passing Integration Tests |\n| --------------------- | ----- | ---- | ------ |\n| Python <3.9 | Not Supported | No support planned.  contentctl tool uses modern language constructs not supported ion Python3.8 and below | N/A |\n| Python 3.9 | Required | contentctl tool is written in Python | Yes (locally + GitHub Actions) |\n| Python 3.10 | Not Supported (yet) | Will be supported | Yes (in GitHub Actions) |\n| Python 3.11 | Not Supported (yet) | Will be supported | Yes (in GitHub Actions)  |\n| Docker (local or remote) | Recommended | A running Splunk Server is required for Dynamic Testing.  contentctl can automatically create, configure, and destroy this server as a Splunk container during the lifetime of a test. | (locally + GitHub Actions) |\n\n\n**Because contentctl uses a large number of dependencies, it\'s recommended to install contentctl in a virtual environment. \nThe instructions below use "poetry" and follow this recommendation.  Poetry will automatically create a new virtual environment for you.  \nIt is typically recommended to install poetry to the Global Python Environment.**\n\n#### Install via pip (coming soon): \n```\npython3.9 -m venv .venv\nsource .venv/bin/activate\npip install splunk-contentctl\n```\n\n#### From Source (advanced)\n```\ngit clone git@github.com:splunk/contentctl.git\ncd contentctl\npython3.9 -m pip install poetry\npoetry install\npoetry shell\ncontentctl --help\n```\n\n\n# Usage\n\n### contentctl init\nCreates a new Content Pack in the current directory as well as a configuration file called [contentctl.yml](contentctl.yml) which contains a number of important configuration options.\nThe content pack contains a wide variety of content types:\n- [detections](detection)\n- [baselines](baseline)\n- [lookups](lookup)\n- [macros](macro)\n- [stories](story)\n\n### contentctl new [--type TYPE]\nChoose TYPE {detection, story} to create new content for the Content Pack.  The tool will interactively ask a series of questions required for generating a basic piece of content and automatically add it to the Content Pack.\n\n### contentctl validate\nPerforms static validation on all of the content in this Content Pack.  Writing validation is extremely complex.  Each piece of content can one or dozens of fields ranging from free text to numbers to references to other content.  contentctl\'s build in validation ensures that a number of conditions are met:\n- Required fields in content are defined\n- Values in fields are appropriate.  For example, if content references a Datamodel, then that Datamodel must be valid. Similarly, numeric values that must fall within a certain range must be validated.\n- If a piece of content references other content, then it exists.  For example, if a detection makes use of a macro then the existence and correctness of the macro must be validated.\n- There are no conflicts between content.  For example, two detections cannot have the same name.\nIf any of these conditions are not met, then a descriptive error will be printed and contentctl will return a nonzero exit code.  This makes it suitable for running in an automated workflow or other CICD context.  Instead of exiting on the first error, _contentctl validate_ will continue validating all content so that it can present all relevant error before exiting.\n\n### contentctl build\nGenerates Content Packs in the output format defined in the [contentctl.yml](contentctl.yml) configuration file.  These outputs may include {splunk_app, api, ba}.  When _contentctl build_ runs, it first performs a _contentctl validate_ in order to ensure that a valid app is generated.  Note that it is *NOT* required or recommended to run _contentctl validate_ separately if the intention is to build a Content Pack.\n\n### contentctl report\n### contentctl inspect\n### contentctl deploy\nThe reason to build content is so that it can be deployed to your environment.  However, deploying content to multiple servers and different types of infrastructure can be tricky and time-consuming.  contentctl makes this easy by supporting a number of different deployment mechanisms. Deployment targets can be defined in [contentctl.yml](contentctl.yml).\n- Deploy via API - Using the REST API, individual pieces of content are deployed to a running server.  This is a great way to deploy all of the content in a content pack, but can also be used to deploy individual peices of content.\n- Deploy to Splunk Cloud via ACS - Using the Automated Private App Vetting (APAV) Feature of the Admin Config Service (ACS), Splunk Cloud customers can easily deploy custom apps to their environments.   \n### contentctl docs\n### contentctl test\nThe static validation performed by *contentctl validate* can only take you so far.  While it\'s powerful, and fast, it can only tell determine if the content is *syntactically* correct.  *contentctl test* can test your content on real Splunk Infrastructure to ensure there are no errors in your SPL, raw data can be properly ingested/processed/accelerated on your server, your search finds the event(s) you\'re looking for in raw data, and even provides high-level runtime performance metrics about your searches.    The following diagram shows this workflow at a high level\n\n```mermaid\ngraph TD\nSplunkContainer--start-->SplunkInstance\nSplunkServer-->SplunkInstance\nSplunkInstance--Install Apps-->ConfiguredInstance\nSplunkInstance--Configure Settings-->ConfiguredInstance\nContentPack--Deploy-->ConfiguredInstance\nConfiguredInstance--Start Test-->Testing\nTesting--Test Detection-->Detection\n\nDetection--Replay Raw Data-->Result\nsubgraph Test Indidivual Detection\n\tDetection--Execute Search-->Result\t\nend\nResult--Cleanup-->Testing\nTesting--Cleanup-->TestResults\n```\n\n#### Testing Modes\nThere are a number of different testing modes that control which content will be tested.  This can be controlled with the `--mode {}` option at the command line\n- all - This will test all of the content in the content pack. Please note that by default only detections marked production will be tested (detections marked as deprecated or experimental, for example, will be ignored).\n- selected - Detections whose relative paths are provided on the command line will be tested.  This is particularly useful if you would like to troubleshoot or update just a handful of detections and can save a significant amount of time.  For example, to test two detections use the following command `contentctl test --mode selected --detections_list detections/detection_one.yml detections/detection_two.yml`\n- **changes - (not currently supported) If you have a large number of detections and use a branching workflow to create new content or update content, then this is an easy way to automatically find and test only that content automatically.  This prevents you from needing to explicitly list the subset of content to test using "selected"** \n\n#### Testing Behavior\ncontentctl test\'s default mode allows it to quickly test all content with requiring user interaction.  This makes it suitable for local tests as well as CI/CD workflows.  However, users often want to troubleshoot a test if it fails.  contentctl allows you to change the tool\'s behavior if and/or when a test fails:\n- --behavior never_pause - The default behavior.  If a test does not pass, the tool begins the next test immediately\n- --behavior pause_on_failure - If a test fails, then additional information about that test, and the raw SPL of the test, is printed to the terminal.  A user may then click (or CMD+Click) the "LINK" to begin interactively debugging the failed test on the Splunk Server.  Note that the credentials for the server are printed out at the very beginning of the test.  After you have finished debugging the failure, hit "Return" in the terminal to move on to the next test. The attack_data for this test remains loaded on the server for debugging until the user moves on to the next test.\n- --behavior always_pause - Similar to pause_on_failure, but this pauses after every test regardless of whether it passes or fails.  \n\n\n1. **init** - Initilialize a new repo from scratch so you can easily add your own content to a custom application. \n2. **new** - Creates new content (detection, story)\n3. **validate** - Validates written content\n4. **build** - Builds an application suitable for deployment on a search head using Slim, the Splunk Packaging Toolkit\n5. **deploy** - Deploy the security content pack to a Splunk Server\n6. **docs** - Create documentation as Markdown\n7. **reporting** - Create different reporting files such as a Mitre ATT&CK overlay\n\n\n\n# Acronyms\n| Acronym | Meaning| Description | \n| --------------------- | ------------------------------------------------------- | ---- |\n| SOC | Security Operation Center | Description of a SoC | \n| DaC | Detection as Code | A systematic approach applying DevOps priciples to Detection Engineering. DaC enables Continuous Integration and Continuous Delivery of Detectionsa via automated validation, testing, and deployment |\n| CICD | Continuous Integration/Continuous Delivery | A modern DevOps practice that encourages users to make small, frequent changes which are automatically tested and deployed. This contrasts with legacy approaches that emphasize large changes which may be manually tested an infrequently deployed. |\n| ACS| Admin Config Service | The [Splunk Admin Configu Service](https://docs.splunk.com/Documentation/SplunkCloud/9.0.2209/Config/ACSIntro) is a cloud-native API that provides programmatic self-service administration capabilities for Splunk Cloud Platform. One of its features, Automated Private App Vetting (APAV) enables the installation of custom app on Splunk Cloud instances. | \n| APAV | Automated Private App Vetting | [Automated Private App Vetting](https://docs.splunk.com/Documentation/SplunkCloud/9.0.2209/Config/ManageApps) enables admins to use the ACS API to install, upgrade, and uninstall apps directly on your Splunk Cloud Platform deployment without assistance from Splunk Support. |\n\n\n# License\nCopyright 2023 Splunk Inc.\n\nLicensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at\n\nhttp://www.apache.org/licenses/LICENSE-2.0\n\nUnless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.\n',
-    'author': 'STRT',
-    'author_email': 'research@splunk.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
 
+# License
+Copyright 2023 Splunk Inc.
+
+Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
 
-setup(**setup_kwargs)
```

