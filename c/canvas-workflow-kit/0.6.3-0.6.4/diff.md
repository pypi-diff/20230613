# Comparing `tmp/canvas-workflow-kit-0.6.3.tar.gz` & `tmp/canvas-workflow-kit-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvas-workflow-kit-0.6.3.tar", max compression
+gzip compressed data, was "canvas-workflow-kit-0.6.4.tar", max compression
```

## Comparing `canvas-workflow-kit-0.6.3.tar` & `canvas-workflow-kit-0.6.4.tar`

### file list

```diff
@@ -1,655 +1,655 @@
--rw-r--r--   0        0        0        0 2022-01-24 18:22:24.118414 canvas-workflow-kit-0.6.3/canvas_workflow_kit/__init__.py
--rw-r--r--   0        0        0      222 2022-01-24 18:22:24.118633 canvas-workflow-kit-0.6.3/canvas_workflow_kit/action.py
--rw-r--r--   0        0        0      446 2022-01-24 18:22:24.118811 canvas-workflow-kit-0.6.3/canvas_workflow_kit/api.py
--rw-r--r--   0        0        0        0 2022-01-24 18:22:24.118980 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/__init__.py
--rw-r--r--   0        0        0     7262 2022-03-25 15:24:57.922245 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/ccp001v1_symptomatic_surveillance.py
--rw-r--r--   0        0        0     5599 2022-01-24 18:22:24.119450 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/ccp002v1_high_risk_outreach.py
--rw-r--r--   0        0        0     2984 2022-01-24 18:22:24.119637 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/ccp003v1_hypertension.py
--rw-r--r--   0        0        0     2909 2022-01-24 18:22:24.119822 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/ccp004v1_diabetes.py
--rw-r--r--   0        0        0     2890 2022-01-24 18:22:24.120010 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/ccp005v1_asthma.py
--rw-r--r--   0        0        0    10349 2022-01-24 18:22:24.120304 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms122v6_diabetes_hemoglobin_a1c_poor_control.py
--rw-r--r--   0        0        0    10002 2022-01-24 18:22:24.120594 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms123v6_diabetes_foot_exam.py
--rw-r--r--   0        0        0    11932 2022-01-24 18:22:24.120864 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms125v6_breast_cancer_screening.py
--rw-r--r--   0        0        0    15713 2022-01-24 18:22:24.121172 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms130v6_colorectal_cancer_screening.py
--rw-r--r--   0        0        0    10454 2022-07-01 20:11:06.858920 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms131v6_diabetes_eye_exam.py
--rw-r--r--   0        0        0    12568 2022-01-24 18:22:24.122515 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms134v6_diabetes_medical_attention_for_nephropathy.py
--rw-r--r--   0        0        0    24515 2022-03-25 15:24:57.922691 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms138v6_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py
--rw-r--r--   0        0        0     3394 2022-01-24 18:22:24.124704 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms138v6p1.py
--rw-r--r--   0        0        0     3924 2022-01-24 18:22:24.125229 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms138v6p2.py
--rw-r--r--   0        0        0    10891 2022-01-24 18:22:24.125896 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/customer_scan_complex_case_management_referral.py
--rw-r--r--   0        0        0     8629 2022-01-24 18:22:24.126230 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/customer_scan_dementia_assessment.py
--rw-r--r--   0        0        0     3837 2022-01-24 18:22:24.126594 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/customer_scan_hcc_suspect_alert.py
--rw-r--r--   0        0        0     9104 2022-01-24 18:22:24.126824 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/customer_scan_mood_disorder.py
--rw-r--r--   0        0        0     9347 2022-01-24 18:22:24.127125 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/customer_scan_physical_activity_intervention.py
--rw-r--r--   0        0        0     7673 2022-01-24 18:22:24.127569 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/customer_scan_urinary_symptoms_assessment.py
--rw-r--r--   0        0        0     2886 2022-01-24 18:22:24.127995 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/diabetes_quality_measure.py
--rw-r--r--   0        0        0    13314 2022-01-24 18:22:24.128495 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms138v6_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py
--rw-r--r--   0        0        0     8142 2022-01-24 18:22:24.128740 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms139v6_falls_screening_for_future_fall_risk.py
--rw-r--r--   0        0        0     8900 2022-01-24 18:22:24.128977 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms147v7_preventive_care_and_screening_influenza_immunization.py
--rw-r--r--   0        0        0    17371 2022-01-24 18:22:24.129240 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms156v6_use_of_high_risk_medications_in_the_elderly.py
--rw-r--r--   0        0        0     9884 2022-01-24 18:22:24.129496 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms182v6_ischemic_vascular_disease_complete_lipid_profile_and_ldl_c_control.py
--rw-r--r--   0        0        0    19442 2022-01-24 18:22:24.129850 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms2v7_preventive_care_and_screening_screening_for_depression_and_follow_up_plan.py
--rw-r--r--   0        0        0     7967 2022-01-24 18:22:24.130622 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms50v6_closing_the_referral_loop_receipt_of_specialist_report.py
--rw-r--r--   0        0        0    25550 2022-01-24 18:22:24.131754 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms69v6_preventive_care_and_screening_body_mass_index_screening_and_follow_up_plan.py
--rw-r--r--   0        0        0     9553 2022-01-24 18:22:24.132180 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cqm_CMS127v6_pneumococcal.py
--rw-r--r--   0        0        0     3638 2022-01-24 18:22:24.132470 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cqm_CMS160v6_depression.py
--rw-r--r--   0        0        0     1625 2022-01-24 18:22:24.132732 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/quality_measure_document.py
--rw-r--r--   0        0        0     5125 2022-01-24 18:22:24.133209 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/hcc001v1_problem_list_hygiene.py
--rw-r--r--   0        0        0     4937 2022-01-24 18:22:24.133586 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/hcc002v2_ckd_suspect.py
--rw-r--r--   0        0        0     9228 2022-01-24 18:22:24.134066 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/hcc003v1_diabetes_mellitus_with_seconday_complication_suspect.py
--rw-r--r--   0        0        0     3381 2022-01-24 18:22:24.134384 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/hcc004v1_dysrhythmia_suspect.py
--rw-r--r--   0        0        0     3795 2022-01-24 18:22:24.134738 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/hcc005v1_annual_wellness_visit.py
--rw-r--r--   0        0        0      519 2022-01-24 18:22:24.134957 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/helper_population.py
--rw-r--r--   0        0        0     2081 2022-01-24 18:22:24.135172 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/hyperlink_recommendation.py
--rw-r--r--   0        0        0     1032 2022-01-24 18:22:24.135461 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stub_template.py.txt
--rw-r--r--   0        0        0     2291 2022-01-24 18:22:24.135745 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stub_template_user.py.txt
--rw-r--r--   0        0        0    11894 2022-01-24 18:22:24.137659 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/_importlib_modulespec.data.json
--rw-r--r--   0        0        0     1105 2022-01-24 18:22:24.137971 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/_importlib_modulespec.meta.json
--rw-r--r--   0        0        0    12251 2022-01-24 18:22:24.138971 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/abc.data.json
--rw-r--r--   0        0        0     1058 2022-01-24 18:22:24.139232 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/abc.meta.json
--rw-r--r--   0        0        0   601115 2022-01-24 18:22:24.140943 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/builtins.data.json
--rw-r--r--   0        0        0     1099 2022-01-24 18:22:24.141348 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/builtins.meta.json
--rw-r--r--   0        0        0     9837 2022-01-24 18:22:24.141652 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms123v5_diabetes_foot_exam.data.json
--rw-r--r--   0        0        0     1157 2022-01-24 18:22:24.141904 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms123v5_diabetes_foot_exam.meta.json
--rw-r--r--   0        0        0     9613 2022-01-24 18:22:24.142113 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms124v6_cervical_cancer_screening.data.json
--rw-r--r--   0        0        0     1171 2022-01-24 18:22:24.142347 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms124v6_cervical_cancer_screening.meta.json
--rw-r--r--   0        0        0   216922 2022-01-24 18:22:24.143163 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/__init__.data.json
--rw-r--r--   0        0        0     1125 2022-01-24 18:22:24.143370 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/__init__.meta.json
--rw-r--r--   0        0        0     3467 2022-01-24 18:22:24.143565 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/abc.data.json
--rw-r--r--   0        0        0     1088 2022-01-24 18:22:24.143749 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/abc.meta.json
--rw-r--r--   0        0        0     9096 2022-01-24 18:22:24.144081 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/mypy_extensions.data.json
--rw-r--r--   0        0        0     1080 2022-01-24 18:22:24.144301 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/mypy_extensions.meta.json
--rw-r--r--   0        0        0    46004 2022-01-24 18:22:24.144554 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/sys.data.json
--rw-r--r--   0        0        0     1082 2022-01-24 18:22:24.144781 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/sys.meta.json
--rw-r--r--   0        0        0    67237 2022-01-24 18:22:24.145331 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/types.data.json
--rw-r--r--   0        0        0     1091 2022-01-24 18:22:24.145563 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/types.meta.json
--rw-r--r--   0        0        0   306873 2022-01-24 18:22:24.146132 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/typing.data.json
--rw-r--r--   0        0        0     1094 2022-01-24 18:22:24.146335 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/typing.meta.json
--rw-r--r--   0        0        0    12618 2022-01-24 18:22:24.146571 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms117v9_childhood_immunization_status.py
--rw-r--r--   0        0        0     6916 2022-01-24 18:22:24.146811 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms122v9_diabetes_hemoglobin_a1c_poor_control.py
--rw-r--r--   0        0        0     5274 2022-01-24 18:22:24.147165 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms124v9_cervical_cancer_screening.py
--rw-r--r--   0        0        0     6301 2022-01-24 18:22:24.147478 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms125v9_breast_cancer_screening.py
--rw-r--r--   0        0        0     7569 2022-01-24 18:22:24.147833 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms127v9_pneumococcal_vaccination_status_for_older_adults.py
--rw-r--r--   0        0        0    10387 2022-01-24 18:22:24.148711 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms128v9_anti_depressant_medication_management.py
--rw-r--r--   0        0        0     7647 2022-01-24 18:22:24.149094 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms129v10_prostate_cancer_avoidance_of_overuse_of_bone_scan_for_staging_low_risk_prostate_cancer_patients.py
--rw-r--r--   0        0        0     6119 2022-01-24 18:22:24.149302 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms130v9_colorectal_cancer_screening.py
--rw-r--r--   0        0        0     7376 2022-01-24 18:22:24.149585 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms131v9_diabetes_eye_exam.py
--rw-r--r--   0        0        0    10990 2022-01-24 18:22:24.149934 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms133v9_cataracts_20_40_or_better_visual_acuity_within_90_days_following_cataract_surgery.py
--rw-r--r--   0        0        0    10284 2022-01-24 18:22:24.150271 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms134v9_diabetes_medical_attention_for_nephropathy.py
--rw-r--r--   0        0        0    11991 2022-01-24 18:22:24.150627 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms135v9_heart_failure_angiotensin_converting_enzyme_inhibitor_or_angiotensin_receptor_blocker_or_angiotensin_receptor_neprilysin_inhibitor_therapy_for_left_ventricular_systolic_dysfunction.py
--rw-r--r--   0        0        0    15664 2022-01-24 18:22:24.151308 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms136v10_follow_up_care_for_children_prescribed_adhd_medication.py
--rw-r--r--   0        0        0    12563 2022-01-24 18:22:24.151690 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms137v9_initiation_and_engagement_of_alcohol_and_other_drug_dependence_treatment.py
--rw-r--r--   0        0        0    11350 2022-01-24 18:22:24.152066 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms138v9_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py
--rw-r--r--   0        0        0     6105 2022-01-24 18:22:24.152445 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms139v9_falls_screening_for_future_fall_risk.py
--rw-r--r--   0        0        0     7917 2022-01-24 18:22:24.152878 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms142v9_diabetic_retinopathy_communication_with_the_physician_managing_ongoing_diabetes_care.py
--rw-r--r--   0        0        0     6525 2022-01-24 18:22:24.153238 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms143v9_primary_open_angle_glaucoma_optic_nerve_evaluation.py
--rw-r--r--   0        0        0     8623 2022-01-24 18:22:24.153626 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms144v9_heart_failure_beta_blocker_therapy_for_left_ventricular_systolic_dysfunction.py
--rw-r--r--   0        0        0     7002 2022-01-24 18:22:24.154141 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms145v9_coronary_artery_disease_beta_blocker_therapy_prior_myocardial_infarction_or_left_ventricular_systolic_dysfunction.py
--rw-r--r--   0        0        0     5333 2022-01-24 18:22:24.154430 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms146v9_appropriate_testing_for_pharyngitis.py
--rw-r--r--   0        0        0     7666 2022-01-24 18:22:24.154860 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms147v10_preventive_care_and_screening_influenza_immunization.py
--rw-r--r--   0        0        0    11366 2022-01-24 18:22:24.155148 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms149v9_dementia_cognitive_assessment.py
--rw-r--r--   0        0        0     5137 2022-01-24 18:22:24.155438 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms153v9_chlamydia_screening_for_women.py
--rw-r--r--   0        0        0     4797 2022-01-24 18:22:24.155799 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms154v9_appropriate_treatment_for_upper_respiratory_infection.py
--rw-r--r--   0        0        0     7220 2022-01-24 18:22:24.156105 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms155v9_weight_assessment_and_counseling_for_nutrition_and_physical_activity_for_children_and_adolescents.py
--rw-r--r--   0        0        0    10832 2022-01-24 18:22:24.156397 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms156v9_use_of_high_risk_medications_in_older_adults.py
--rw-r--r--   0        0        0     8583 2022-01-24 18:22:24.156709 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms157v9_oncology_medical_and_radiation_pain_intensity_quantified.py
--rw-r--r--   0        0        0    17246 2022-01-24 18:22:24.157156 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms159v9_depression_remission_at_twelve_months.py
--rw-r--r--   0        0        0    13128 2022-01-24 18:22:24.157634 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms161v9_adult_major_depressive_disorder_suicide_risk_assessment.py
--rw-r--r--   0        0        0    13690 2022-01-24 18:22:24.158007 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms165v9_controlling_high_blood_pressure.py
--rw-r--r--   0        0        0     8069 2022-01-24 18:22:24.158343 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms177v9_child_and_adolescent_major_depressive_disorder_suicide_risk_assessment.py
--rw-r--r--   0        0        0    12217 2022-01-24 18:22:24.158600 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms22v9_preventive_care_and_screening_screening_for_high_blood_pressure_and_follow_up_documented.py
--rw-r--r--   0        0        0    12527 2022-01-24 18:22:24.158864 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms249v3_appropriate_use_of_dxa_scans_in_women_under_65_years_who_do_not_meet_the_risk_factor_profile_for_osteoporotic_fracture.py
--rw-r--r--   0        0        0    17320 2022-01-24 18:22:24.159308 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms2v10_preventive_care_and_screening_screening_for_depression_and_follow_up_plan.py
--rw-r--r--   0        0        0    18696 2022-01-24 18:22:24.159707 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms347v4_statin_therapy_for_the_prevention_and_treatment_of_cardiovascular_disease.py
--rw-r--r--   0        0        0     8675 2022-01-24 18:22:24.159948 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms349v3_hiv_screening.py
--rw-r--r--   0        0        0     8513 2022-01-24 18:22:24.160197 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms50v9_closing_the_referral_loop_receipt_of_specialist_report.py
--rw-r--r--   0        0        0     7748 2022-01-24 18:22:24.160429 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms56v9_functional_status_assessment_for_total_hip_replacement.py
--rw-r--r--   0        0        0     6954 2022-01-24 18:22:24.160658 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms645v4_bone_density_evaluation_for_patients_with_prostate_cancer_and_receiving_androgen_deprivation_therapy.py
--rw-r--r--   0        0        0     6655 2022-01-24 18:22:24.160899 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms66v9_functional_status_assessment_for_total_knee_replacement.py
--rw-r--r--   0        0        0    12014 2022-01-24 18:22:24.161138 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms68v10_documentation_of_current_medications_in_the_medical_record.py
--rw-r--r--   0        0        0    21957 2022-01-24 18:22:24.161568 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms69v9_preventive_care_and_screening_body_mass_index_screening_and_follow_up_plan.py
--rw-r--r--   0        0        0     4181 2022-01-24 18:22:24.161804 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms74v10_primary_caries_prevention_intervention_as_offered_by_primary_care_providers,_including_dentists.py
--rw-r--r--   0        0        0     3788 2022-01-24 18:22:24.162066 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms75v9_children_who_have_dental_decay_or_cavities.py
--rw-r--r--   0        0        0     7673 2022-01-24 18:22:24.162408 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms771v2_urinary_symptom_score_change_6_12_months_after_diagnosis_of_benign_prostatic_hyperplasia.py
--rw-r--r--   0        0        0     5787 2022-01-24 18:22:24.162671 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms90v10_functional_status_assessments_for_congestive_heart_failure.py
--rw-r--r--   0        0        0        0 2022-01-24 18:22:24.162901 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-01-24 18:22:24.163127 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mixins/__init__.py
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.230397 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/billing_line_items.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.163720 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.163869 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.164022 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.164193 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.164396 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.164785 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/medications.json
--rw-r--r--   0        0        0       90 2022-01-24 18:22:24.164956 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.165228 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.232032 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/billing_line_items.json
--rw-r--r--   0        0        0      416 2022-01-24 18:22:24.165822 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.165994 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.166171 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/instructions.json
--rw-r--r--   0        0        0      663 2022-01-24 18:22:24.166405 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.166656 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.166951 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/medications.json
--rw-r--r--   0        0        0       94 2022-01-24 18:22:24.167225 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.167501 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.232880 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/billing_line_items.json
--rw-r--r--   0        0        0      416 2022-01-24 18:22:24.168133 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.168361 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.168623 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.168858 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/interviews.json
--rw-r--r--   0        0        0      596 2023-05-10 02:05:38.780247 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.169443 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/medications.json
--rw-r--r--   0        0        0       94 2022-01-24 18:22:24.169673 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.169935 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.234071 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/billing_line_items.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.170337 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.170482 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.170620 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.170781 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.171003 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.171201 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/medications.json
--rw-r--r--   0        0        0       90 2022-01-24 18:22:24.171468 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.171760 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.235249 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/billing_line_items.json
--rw-r--r--   0        0        0      416 2022-01-24 18:22:24.172510 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.172740 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.172968 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.173186 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.173398 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.173614 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/medications.json
--rw-r--r--   0        0        0       94 2022-01-24 18:22:24.173860 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.174495 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.236291 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/billing_line_items.json
--rw-r--r--   0        0        0      416 2022-01-24 18:22:24.176659 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.176896 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.177056 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/instructions.json
--rw-r--r--   0        0        0      666 2022-01-24 18:22:24.177236 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.177386 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.177544 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/medications.json
--rw-r--r--   0        0        0       94 2022-01-24 18:22:24.177758 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.177961 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.237767 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/billing_line_items.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.178474 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/conditions.json
--rw-r--r--   0        0        0        4 2022-01-24 18:22:24.178618 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/imaging_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.178833 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.179076 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.179273 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.179425 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.179631 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/medications.json
--rw-r--r--   0        0        0      100 2022-01-24 18:22:24.179814 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.179961 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/referral_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.180101 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.239253 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/billing_line_items.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.180471 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/conditions.json
--rw-r--r--   0        0        0      298 2022-01-24 18:22:24.180630 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/imaging_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.180774 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.180913 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.181202 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.181454 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.181688 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/medications.json
--rw-r--r--   0        0        0      100 2022-01-24 18:22:24.181890 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.182122 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/referral_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.182339 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.240447 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/billing_line_items.json
--rw-r--r--   0        0        0      284 2022-01-24 18:22:24.182958 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.183244 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/imaging_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.183503 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.183759 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.183956 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.184152 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.184308 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/medications.json
--rw-r--r--   0        0        0      100 2022-01-24 18:22:24.184508 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.184768 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/referral_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.185012 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.241430 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_due/billing_line_items.json
--rw-r--r--   0        0        0       78 2022-01-24 18:22:24.185549 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_due/patient.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.242196 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_satisfied/billing_line_items.json
--rw-r--r--   0        0        0      208 2022-01-24 18:22:24.186397 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_satisfied/imaging_reports.json
--rw-r--r--   0        0        0      114 2023-05-10 02:00:32.209805 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_satisfied/lab_reports.json
--rw-r--r--   0        0        0       78 2022-01-24 18:22:24.186736 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_satisfied/patient.json
--rw-r--r--   0        0        0      203 2022-01-24 18:22:24.186926 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_satisfied/referral_reports.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.243527 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/billing_line_items.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.187594 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.188114 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.188374 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.188647 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.188928 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.189187 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/medications.json
--rw-r--r--   0        0        0       90 2022-01-24 18:22:24.189485 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.189656 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/referral_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.189884 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.244205 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/billing_line_items.json
--rw-r--r--   0        0        0      416 2022-01-24 18:22:24.190480 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.190652 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.190822 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.191009 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.191225 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.191476 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/medications.json
--rw-r--r--   0        0        0       94 2022-01-24 18:22:24.191652 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.191805 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/referral_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.191940 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.244881 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/billing_line_items.json
--rw-r--r--   0        0        0      416 2022-01-24 18:22:24.192403 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.192593 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.192757 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.192905 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.193059 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.193206 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/medications.json
--rw-r--r--   0        0        0       94 2022-01-24 18:22:24.193346 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/patient.json
--rw-r--r--   0        0        0      564 2022-01-24 18:22:24.193507 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/referral_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.193653 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.245811 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/billing_line_items.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.194076 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.194221 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.194396 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.194548 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.194752 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.194953 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/medications.json
--rw-r--r--   0        0        0       94 2022-01-24 18:22:24.195150 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.195308 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.246817 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/billing_line_items.json
--rw-r--r--   0        0        0      658 2022-01-24 18:22:24.195662 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.195792 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/immunizations.json
--rw-r--r--   0        0        0      219 2022-01-24 18:22:24.195935 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.196117 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/interviews.json
--rw-r--r--   0        0        0      233 2023-05-10 02:00:54.526610 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/lab_reports.json
--rw-r--r--   0        0        0      276 2022-01-24 18:22:24.196405 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/medications.json
--rw-r--r--   0        0        0       94 2022-01-24 18:22:24.196537 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/patient.json
--rw-r--r--   0        0        0      269 2022-01-24 18:22:24.196671 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/referral_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.196797 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.247450 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes_only/billing_line_items.json
--rw-r--r--   0        0        0      416 2022-01-24 18:22:24.197168 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes_only/conditions.json
--rw-r--r--   0        0        0       94 2022-01-24 18:22:24.197307 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes_only/patient.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.259324 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms138v6/billing_line_items.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.197713 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms138v6/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.197840 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms138v6/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.198042 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms138v6/medications.json
--rw-r--r--   0        0        0      100 2022-01-24 18:22:24.198209 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms138v6/patient.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.260326 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetes_mixin/billing_line_items.json
--rw-r--r--   0        0        0      416 2022-01-24 18:22:24.198731 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetes_mixin/conditions.json
--rw-r--r--   0        0        0       95 2022-01-24 18:22:24.198905 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetes_mixin/patient.json
--rw-r--r--   0        0        0      448 2022-01-24 18:22:24.199225 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.199384 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.199579 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.199742 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.199938 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.200155 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/medications.json
--rw-r--r--   0        0        0      108 2022-01-24 18:22:24.200385 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.200606 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/vital_signs.json
--rw-r--r--   0        0        0      351 2022-01-24 18:22:24.201247 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.201473 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/immunizations.json
--rw-r--r--   0        0        0      533 2022-01-24 18:22:24.201745 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/instructions.json
--rw-r--r--   0        0        0     8462 2022-01-24 18:22:24.202031 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.202195 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/lab_reports.json
--rw-r--r--   0        0        0    14914 2022-01-24 18:22:24.202541 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/medications.json
--rw-r--r--   0        0        0      108 2022-01-24 18:22:24.202759 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.202933 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/vital_signs.json
--rw-r--r--   0        0        0      632 2022-01-24 18:22:24.203237 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.203491 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.203685 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.203882 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.204116 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.204441 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/medications.json
--rw-r--r--   0        0        0       78 2022-01-24 18:22:24.204649 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.204819 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/vital_signs.json
--rw-r--r--   0        0        0      513 2022-01-24 18:22:24.205066 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.205227 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.205386 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.205548 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/interviews.json
--rw-r--r--   0        0        0      403 2023-05-10 02:02:28.255357 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.205895 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/medications.json
--rw-r--r--   0        0        0      133 2022-01-24 18:22:24.206041 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.206179 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/vital_signs.json
--rw-r--r--   0        0        0      369 2022-01-24 18:22:24.206407 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.206585 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.206729 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.206964 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.207202 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.207671 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/medications.json
--rw-r--r--   0        0        0       78 2022-01-24 18:22:24.208040 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.208225 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/vital_signs.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.208463 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.208608 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.208823 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.209044 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.209270 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.209552 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/medications.json
--rw-r--r--   0        0        0       78 2022-01-24 18:22:24.209763 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.210010 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/vital_signs.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.210255 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.210431 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.210574 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.210721 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.210904 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.211170 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/medications.json
--rw-r--r--   0        0        0       78 2022-01-24 18:22:24.211347 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.211499 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/vital_signs.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.211765 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.211921 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.212079 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.212231 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.212388 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.212603 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/medications.json
--rw-r--r--   0        0        0      116 2022-01-24 18:22:24.212757 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:24.212904 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/vital_signs.json
--rw-r--r--   0        0        0    23878 2022-01-24 18:22:24.213165 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_ccp001v1_symptomatic_surveillance.py
--rw-r--r--   0        0        0    19759 2022-01-24 18:22:24.213412 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_ccp002v1_high_risk_outreach.py
--rw-r--r--   0        0        0     8282 2022-01-24 18:22:24.213625 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_ccp003v1_hypertension.py
--rw-r--r--   0        0        0     8240 2022-01-24 18:22:24.213838 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_ccp004v1_diabetes.py
--rw-r--r--   0        0        0     8201 2022-01-24 18:22:24.214048 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_ccp005v1_asthma.py
--rw-r--r--   0        0        0    18063 2022-07-01 20:11:06.859263 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms122v6_diabetes_hemoglobin_a1c_poor_control.py
--rw-r--r--   0        0        0    16610 2022-07-01 20:11:06.859608 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms123v6_diabetes_foot_exam.py
--rw-r--r--   0        0        0    23648 2022-07-01 20:11:06.859959 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms125v6_breast_cancer_screening.py
--rw-r--r--   0        0        0    30237 2022-07-01 20:11:06.865305 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms130v6_colorectal_cancer_screening.py
--rw-r--r--   0        0        0    21800 2022-07-01 20:11:06.865737 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms131v6_diabetes_eye_exam.py
--rw-r--r--   0        0        0    19107 2022-07-01 20:11:06.866100 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms134v6_diabetes_medical_attention_for_nephropathy.py
--rw-r--r--   0        0        0    49276 2022-07-01 20:11:06.866598 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms138v6_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py
--rw-r--r--   0        0        0    22181 2022-07-01 20:11:06.867115 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms138v6p1.py
--rw-r--r--   0        0        0    25266 2022-07-01 20:11:06.867637 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms138v6p2.py
--rw-r--r--   0        0        0    10949 2022-07-01 20:11:06.873417 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_diabetes_quality_measure.py
--rw-r--r--   0        0        0    16283 2022-01-24 18:22:24.219181 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_hcc001v1_problem_list_hygiene.py
--rw-r--r--   0        0        0    13281 2022-01-24 18:22:24.219535 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_hcc002v2_ckd_suspect.py
--rw-r--r--   0        0        0    34017 2022-01-24 18:22:24.219804 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_hcc003v1_diabetes_mellitus_with_seconday_complication_suspect.py
--rw-r--r--   0        0        0    12234 2022-01-24 18:22:24.220114 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_hcc004v1_dysrhythmia_suspect.py
--rw-r--r--   0        0        0     9296 2022-07-01 20:11:06.873889 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_hcc005v1_annual_wellness_visit.py
--rw-r--r--   0        0        0     1692 2022-01-24 18:22:24.220606 canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_helper_population.py
--rwxr-xr-x   0        0        0    12678 2022-07-01 20:11:06.874784 canvas-workflow-kit-0.6.3/canvas_workflow_kit/canvas_cli.py
--rw-r--r--   0        0        0     3493 2022-01-24 18:22:24.221281 canvas-workflow-kit-0.6.3/canvas_workflow_kit/canvas_code_set.py
--rw-r--r--   0        0        0     3978 2023-05-08 20:27:45.689601 canvas-workflow-kit-0.6.3/canvas_workflow_kit/constants.py
--rw-r--r--   0        0        0      852 2022-01-24 18:22:24.221783 canvas-workflow-kit-0.6.3/canvas_workflow_kit/events.py
--rwxr-xr-x   0        0        0    12515 2022-01-24 18:22:24.222185 canvas-workflow-kit-0.6.3/canvas_workflow_kit/generate_cqms_stubs.py
--rw-r--r--   0        0        0     1360 2022-01-24 18:22:24.222626 canvas-workflow-kit-0.6.3/canvas_workflow_kit/internal/attrdict.py
--rw-r--r--   0        0        0     3384 2023-04-24 18:35:18.261857 canvas-workflow-kit-0.6.3/canvas_workflow_kit/internal/integration_messages.py
--rw-r--r--   0        0        0     1210 2022-01-24 18:22:24.222895 canvas-workflow-kit-0.6.3/canvas_workflow_kit/internal/string.py
--rw-r--r--   0        0        0     2029 2022-01-24 18:22:24.223204 canvas-workflow-kit-0.6.3/canvas_workflow_kit/intervention.py
--rw-r--r--   0        0        0      932 2022-01-24 18:22:24.223569 canvas-workflow-kit-0.6.3/canvas_workflow_kit/metaclass.py
--rw-r--r--   0        0        0    10674 2023-05-08 21:53:32.507485 canvas-workflow-kit-0.6.3/canvas_workflow_kit/patient.py
--rw-r--r--   0        0        0    25693 2023-05-09 20:30:38.942303 canvas-workflow-kit-0.6.3/canvas_workflow_kit/patient_recordset.py
--rw-r--r--   0        0        0    22919 2023-04-24 18:35:18.263646 canvas-workflow-kit-0.6.3/canvas_workflow_kit/protocol.py
--rw-r--r--   0        0        0    15189 2022-09-12 21:43:31.107454 canvas-workflow-kit-0.6.3/canvas_workflow_kit/recommendation.py
--rw-r--r--   0        0        0     1365 2022-01-24 18:22:25.197299 canvas-workflow-kit-0.6.3/canvas_workflow_kit/settings.py
--rw-r--r--   0        0        0        0 2022-01-24 18:22:25.197473 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/__init__.py
--rw-r--r--   0        0        0     1612 2022-01-24 18:22:25.197673 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/base.py
--rw-r--r--   0        0        0        0 2022-01-24 18:22:25.197836 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/get_protocols_unittest/__init__.py
--rw-r--r--   0        0        0     5139 2022-01-24 18:22:25.198025 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/get_protocols_unittest/protocol_unittest.py
--rw-r--r--   0        0        0        3 2023-04-24 18:35:18.263881 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/appointments.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.198540 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/billing_line_items.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.198699 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/conditions.json
--rw-r--r--   0        0        0        3 2022-09-12 21:45:44.061343 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/consents.json
--rw-r--r--   0        0        0        3 2023-04-24 18:35:18.263999 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/external_events.json
--rw-r--r--   0        0        0        2 2022-09-12 21:45:44.062431 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/groups.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.198864 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/imaging_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.199017 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.199154 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/inpatientStay.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.199289 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.199431 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.199603 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/lab_orders.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.199603 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.199750 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/medications.json
--rw-r--r--   0        0        0      106 2022-01-24 18:22:25.199914 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/patient.json
--rw-r--r--   0        0        0        3 2022-04-27 22:44:55.538708 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/prescriptions.json
--rw-r--r--   0        0        0        3 2022-04-28 22:56:13.276213 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/procedures.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.200117 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/protocol_overrides.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.200839 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/referral_reports.json
--rw-r--r--   0        0        0        3 2022-09-12 21:45:44.062707 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/tasks.py
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.202186 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty/vitalsigns.json
--rw-r--r--   0        0        0      719 2022-01-24 18:22:25.198277 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty.json
--rw-r--r--   0        0        0     4523 2023-04-24 18:35:18.269650 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/appointments.json
--rw-r--r--   0        0        0      325 2022-04-28 22:56:13.279929 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/billing_line_items.json
--rw-r--r--   0        0        0     3024 2022-01-24 18:22:25.203348 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/conditions.json
--rw-r--r--   0        0        0     1675 2022-09-12 21:45:44.068285 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/consents.json
--rw-r--r--   0        0        0      449 2023-04-24 18:35:18.269889 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/external_events.json
--rw-r--r--   0        0        0      146 2022-09-12 21:45:44.069326 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/groups.json
--rw-r--r--   0        0        0      747 2022-01-24 18:22:25.203793 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/imaging_reports.json
--rw-r--r--   0        0        0      328 2022-01-24 18:22:25.204329 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/immunizations.json
--rw-r--r--   0        0        0      155 2022-01-24 18:22:25.204559 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/inpatientStay.json
--rw-r--r--   0        0        0      197 2022-01-24 18:22:25.204884 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/instructions.json
--rw-r--r--   0        0        0      898 2022-01-24 18:22:25.205414 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/interviews.json
--rw-r--r--   0        0        0     1147 2023-05-08 21:09:23.301050 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/lab_orders.json
--rw-r--r--   0        0        0     1443 2023-05-10 02:07:22.574425 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/lab_reports.json
--rw-r--r--   0        0        0      544 2022-01-24 18:22:25.205812 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/medications.json
--rw-r--r--   0        0        0      409 2022-01-24 18:22:25.205998 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/patient.json
--rw-r--r--   0        0        0      700 2022-04-27 22:44:55.546421 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/prescriptions.json
--rw-r--r--   0        0        0      486 2022-04-28 22:56:13.307651 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/procedures.json
--rw-r--r--   0        0        0      649 2022-01-24 18:22:25.206165 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/protocol_overrides.json
--rw-r--r--   0        0        0      315 2022-01-24 18:22:25.206334 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/referral_reports.json
--rw-r--r--   0        0        0     4238 2022-01-24 18:22:25.206497 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/referrals.json
--rw-r--r--   0        0        0     1571 2022-09-12 21:45:44.074048 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/tasks.json
--rw-r--r--   0        0        0      260 2022-01-24 18:22:25.206698 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/vital_signs.json
--rw-r--r--   0        0        0     7367 2022-04-28 22:56:13.279197 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full.json
--rw-r--r--   0        0        0     1030 2023-04-24 18:35:18.275606 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/appointments.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.207006 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/billing_line_items.json
--rw-r--r--   0        0        0      724 2022-01-24 18:22:25.207195 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/conditions.json
--rw-r--r--   0        0        0      730 2022-09-12 21:45:44.091760 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/consents.json
--rw-r--r--   0        0        0        3 2023-04-24 18:35:18.275810 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/external_events.json
--rw-r--r--   0        0        0        2 2022-09-12 21:45:44.092132 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/groups.json
--rw-r--r--   0        0        0      450 2022-01-24 18:22:25.207424 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/imaging_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.207734 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.207982 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/inpatientStay.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.208325 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/instructions.json
--rw-r--r--   0        0        0      283 2022-01-24 18:22:25.208620 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/interviews.json
--rw-r--r--   0        0        0        3 2023-05-08 21:09:49.522219 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/lab_orders.json
--rw-r--r--   0        0        0      505 2023-05-10 02:07:38.880384 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/lab_reports.json
--rw-r--r--   0        0        0      270 2022-01-24 18:22:25.209256 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/medications.json
--rw-r--r--   0        0        0      409 2022-01-24 18:22:25.209440 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/patient.json
--rw-r--r--   0        0        0        3 2022-04-27 22:44:55.546733 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/prescriptions.json
--rw-r--r--   0        0        0        3 2022-04-28 22:56:13.307958 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/procedures.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.209720 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/protocol_overrides.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.209985 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/referral_reports.json
--rw-r--r--   0        0        0        3 2022-09-12 21:45:44.092379 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/tasks.json
--rw-r--r--   0        0        0      174 2022-01-24 18:22:25.210192 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/vital_signs.json
--rw-r--r--   0        0        0        0 2022-01-24 18:22:25.210346 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/__init__.py
--rw-r--r--   0        0        0      246 2022-01-24 18:22:25.210603 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/base.py
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.211209 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.211375 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.211517 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.211885 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.212194 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.212489 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1/medications.json
--rw-r--r--   0        0        0      108 2022-01-24 18:22:25.212666 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1/patient.json
--rw-r--r--   0        0        0     1355 2022-01-24 18:22:25.213027 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1/vital_signs.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.213593 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.213901 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/immunizations.json
--rw-r--r--   0        0        0      888 2022-01-24 18:22:25.214181 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.214498 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.214773 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.215012 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/medications.json
--rw-r--r--   0        0        0      108 2022-01-24 18:22:25.215238 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/patient.json
--rw-r--r--   0        0        0     1355 2022-01-24 18:22:25.215582 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/vital_signs.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.215829 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi2/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.216742 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi2/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.217011 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi2/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.217182 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi2/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.217669 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi2/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.218062 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi2/medications.json
--rw-r--r--   0        0        0      108 2022-01-24 18:22:25.218303 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi2/patient.json
--rw-r--r--   0        0        0     1355 2022-01-24 18:22:25.218700 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi2/vital_signs.json
--rw-r--r--   0        0        0    28246 2022-01-24 18:22:25.219159 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/conditions.json
--rw-r--r--   0        0        0     1279 2022-01-24 18:22:25.219532 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.219817 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/instructions.json
--rw-r--r--   0        0        0     2251 2022-01-24 18:22:25.220186 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.220730 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/lab_reports.json
--rw-r--r--   0        0        0    17754 2022-01-24 18:22:25.221022 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/medications.json
--rw-r--r--   0        0        0     2758 2022-01-24 18:22:25.221301 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/patient.json
--rw-r--r--   0        0        0     6346 2022-01-24 18:22:25.222497 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/vital_signs.json
--rw-r--r--   0        0        0    28246 2022-01-24 18:22:25.224306 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/conditions.json
--rw-r--r--   0        0        0     1279 2022-01-24 18:22:25.225300 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/immunizations.json
--rw-r--r--   0        0        0      908 2022-01-24 18:22:25.226426 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/instructions.json
--rw-r--r--   0        0        0     2251 2022-01-24 18:22:25.228211 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.229773 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/lab_reports.json
--rw-r--r--   0        0        0    17754 2022-01-24 18:22:25.231885 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/medications.json
--rw-r--r--   0        0        0     2758 2022-01-24 18:22:25.233870 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/patient.json
--rw-r--r--   0        0        0     6346 2022-01-24 18:22:25.234254 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/vital_signs.json
--rw-r--r--   0        0        0      295 2022-04-28 22:56:13.308902 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/billing_line_items.json
--rw-r--r--   0        0        0      405 2022-01-24 18:22:25.235113 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.235318 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.235656 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.235958 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.236130 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.236273 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/medications.json
--rw-r--r--   0        0        0      108 2022-01-24 18:22:25.236414 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.236613 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.309308 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/billing_line_items.json
--rw-r--r--   0        0        0      531 2022-01-24 18:22:25.237009 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.237240 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.237424 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.237571 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/interviews.json
--rw-r--r--   0        0        0      541 2023-05-10 02:09:45.684116 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.238061 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/medications.json
--rw-r--r--   0        0        0      108 2022-01-24 18:22:25.238215 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.238359 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.310111 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/billing_line_items.json
--rw-r--r--   0        0        0      531 2022-01-24 18:22:25.238897 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.239132 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.239413 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.239603 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/interviews.json
--rw-r--r--   0        0        0      541 2023-05-10 02:09:58.414804 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.239962 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/medications.json
--rw-r--r--   0        0        0      108 2022-01-24 18:22:25.240100 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.240286 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/vital_signs.json
--rw-r--r--   0        0        0      163 2022-04-28 22:56:13.310532 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/billing_line_items.json
--rw-r--r--   0        0        0      531 2022-01-24 18:22:25.240723 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.240878 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.241022 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.241199 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/interviews.json
--rw-r--r--   0        0        0      542 2023-05-10 02:10:10.490687 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.241557 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/medications.json
--rw-r--r--   0        0        0      108 2022-01-24 18:22:25.241721 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.241861 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/vital_signs.json
--rw-r--r--   0        0        0      504 2022-01-24 18:22:25.242081 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/example/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.242219 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/example/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.242375 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/example/instructions.json
--rw-r--r--   0        0        0      219 2022-01-24 18:22:25.242514 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/example/interviews.json
--rw-r--r--   0        0        0     2192 2023-05-10 02:10:25.921733 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/example/lab_reports.json
--rw-r--r--   0        0        0     1137 2022-01-24 18:22:25.242781 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/example/medications.json
--rw-r--r--   0        0        0     2684 2022-01-24 18:22:25.242957 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/example/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.243102 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/example/vital_signs.json
--rw-r--r--   0        0        0    33067 2022-01-24 18:22:25.243408 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fall1/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.243594 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fall1/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.243726 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fall1/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.243857 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fall1/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.243985 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fall1/lab_reports.json
--rw-r--r--   0        0        0    14732 2022-01-24 18:22:25.244182 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fall1/medications.json
--rw-r--r--   0        0        0     2842 2022-01-24 18:22:25.244409 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fall1/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.244576 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fall1/vital_signs.json
--rw-r--r--   0        0        0      149 2022-04-28 22:56:13.312270 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/feet1/billing_line_items.json
--rw-r--r--   0        0        0      405 2022-01-24 18:22:25.244992 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/feet1/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.245133 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/feet1/immunizations.json
--rw-r--r--   0        0        0       81 2022-01-24 18:22:25.245270 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/feet1/instructions.json
--rw-r--r--   0        0        0      656 2022-01-24 18:22:25.245419 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/feet1/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.245611 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/feet1/lab_reports.json
--rw-r--r--   0        0        0      807 2022-01-24 18:22:25.245805 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/feet1/medications.json
--rw-r--r--   0        0        0      108 2022-01-24 18:22:25.245992 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/feet1/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.246183 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/feet1/vital_signs.json
--rw-r--r--   0        0        0     1396 2022-01-24 18:22:25.246422 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fluvax/conditions.json
--rw-r--r--   0        0        0     1280 2022-01-24 18:22:25.246576 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fluvax/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.246788 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fluvax/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.246957 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fluvax/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.247168 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fluvax/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.247480 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fluvax/medications.json
--rw-r--r--   0        0        0      108 2022-01-24 18:22:25.247715 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fluvax/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.247993 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fluvax/vital_signs.json
--rw-r--r--   0        0        0     8774 2022-01-24 18:22:25.248353 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/#medications.json#
--rw-r--r--   0        0        0     5923 2022-01-24 18:22:25.248631 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.248928 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.249163 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.249387 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.249603 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/lab_reports.json
--rw-r--r--   0        0        0     7312 2022-01-24 18:22:25.249961 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/medications.json
--rw-r--r--   0        0        0     2967 2022-01-24 18:22:25.250642 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.250933 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/referrals.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.251264 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/vital_signs.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.251597 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.251974 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.252527 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/instructions.json
--rw-r--r--   0        0        0     1668 2022-01-24 18:22:25.253137 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.253396 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.253634 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/medications.json
--rw-r--r--   0        0        0     2684 2022-01-24 18:22:25.253977 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/patient.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.254249 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/vital_signs.json
--rw-r--r--   0        0        0     9323 2022-01-24 18:22:25.254671 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/referral/conditions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.254858 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/referral/immunizations.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.255091 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/referral/instructions.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.255379 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/referral/interviews.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.255667 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/referral/lab_reports.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.255910 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/referral/medications.json
--rw-r--r--   0        0        0     2925 2022-01-24 18:22:25.256082 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/referral/patient.json
--rw-r--r--   0        0        0     1170 2022-01-24 18:22:25.256248 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/referral/referrals.json
--rw-r--r--   0        0        0        3 2022-01-24 18:22:25.256465 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/referral/vital_signs.json
--rw-r--r--   0        0        0      686 2022-01-24 18:22:25.256720 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_interviews.py
--rw-r--r--   0        0        0     1101 2022-01-24 18:22:25.256901 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_labs.py
--rw-r--r--   0        0        0      787 2022-01-24 18:22:25.257103 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_medications.py
--rw-r--r--   0        0        0     5609 2022-01-24 18:22:25.257333 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_protocols.py
--rw-r--r--   0        0        0     1038 2022-01-24 18:22:25.257553 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_recommendations.py
--rw-r--r--   0        0        0       78 2022-01-24 18:22:25.257701 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_search.py
--rw-r--r--   0        0        0      840 2022-01-24 18:22:25.257857 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_value_sets.py
--rw-r--r--   0        0        0      897 2022-01-24 18:22:25.258099 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_vitalsigns.py
--rw-r--r--   0        0        0      814 2022-01-24 18:22:25.258356 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_action.py
--rw-r--r--   0        0        0     4695 2022-01-24 18:22:25.258646 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_canvas_code_set.py
--rw-r--r--   0        0        0     7767 2022-01-24 18:22:25.259257 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_intervention.py
--rw-r--r--   0        0        0    16623 2023-05-08 21:11:15.231795 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_patient.py
--rw-r--r--   0        0        0    63407 2023-05-10 02:08:49.737442 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_patient_recordset.py
--rw-r--r--   0        0        0    32479 2022-01-24 18:22:25.260562 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_protocol.py
--rw-r--r--   0        0        0    20656 2022-03-25 15:24:57.959886 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_recommendation.py
--rw-r--r--   0        0        0     6317 2022-01-24 18:22:25.261095 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_template.py
--rw-r--r--   0        0        0     3254 2022-01-24 18:22:25.261296 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_timeframe.py
--rw-r--r--   0        0        0        0 2022-01-24 18:22:25.261469 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/__init__.py
--rw-r--r--   0        0        0       63 2022-01-24 18:22:25.261707 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/hcc_codes.txt
--rw-r--r--   0        0        0     1312 2022-01-24 18:22:25.261940 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/hcc_file.txt
--rw-r--r--   0        0        0      553 2022-01-24 18:22:25.262093 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/hcc_labels.txt
--rw-r--r--   0        0        0      518 2022-01-24 18:22:25.262318 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/hcc_methods.txt
--rw-r--r--   0        0        0      552 2022-01-24 18:22:25.262494 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/hcc_sample.tsv
--rw-r--r--   0        0        0     1238 2022-01-24 18:22:25.262727 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/test_hcc2018.py
--rw-r--r--   0        0        0     4109 2022-01-24 18:22:25.262921 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/test_specials.py
--rw-r--r--   0        0        0     7030 2022-01-24 18:22:25.263151 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/test_value_set.py
--rw-r--r--   0        0        0     1116 2022-03-25 15:24:57.960115 canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/test_value_sets.py
--rw-r--r--   0        0        0      964 2022-01-24 18:22:25.263321 canvas-workflow-kit-0.6.3/canvas_workflow_kit/timeframe.py
--rw-r--r--   0        0        0     2156 2022-01-24 18:22:25.263521 canvas-workflow-kit-0.6.3/canvas_workflow_kit/utils.py
--rw-r--r--   0        0        0       32 2022-03-25 15:24:57.960352 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/__init__.py
--rw-r--r--   0        0        0     1126 2022-01-24 18:22:25.264054 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/customer_value_sets/scan.py
--rw-r--r--   0        0        0  2129005 2022-01-24 18:22:25.269826 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/hcc2018.py
--rw-r--r--   0        0        0  2236826 2022-01-24 18:22:25.286856 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/medication_class_path2018.py
--rw-r--r--   0        0        0     3993 2022-01-24 18:22:25.287268 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/specials.py
--rw-r--r--   0        0        0  1895881 2022-01-24 18:22:25.324339 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2017.py
--rw-r--r--   0        0        0  1180064 2022-01-24 18:22:25.328255 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2018.py
--rw-r--r--   0        0        0  1167962 2022-01-24 18:22:25.331114 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2019.py
--rw-r--r--   0        0        0  1281481 2022-01-24 18:22:25.335642 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2020.py
--rw-r--r--   0        0        0      494 2022-01-24 18:22:25.336139 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/__init__.py
--rw-r--r--   0        0        0      831 2022-01-24 18:22:25.336367 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/allergy.py
--rw-r--r--   0        0        0     5248 2022-01-24 18:22:25.336580 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/assessment.py
--rw-r--r--   0        0        0     5849 2022-01-24 18:22:25.336830 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/assessment_performed.py
--rw-r--r--   0        0        0     9096 2022-01-24 18:22:25.337101 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/communication.py
--rw-r--r--   0        0        0     1864 2022-01-24 18:22:25.337319 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/device.py
--rw-r--r--   0        0        0   970486 2022-01-24 18:22:25.341293 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/diagnosis.py
--rw-r--r--   0        0        0    34446 2022-01-24 18:22:25.341827 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/encounter.py
--rw-r--r--   0        0        0    36666 2022-01-24 18:22:25.342246 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/encounter_performed.py
--rw-r--r--   0        0        0    11438 2022-01-24 18:22:25.342568 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/immunization.py
--rw-r--r--   0        0        0    29810 2022-01-24 18:22:25.342958 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/lab_test.py
--rw-r--r--   0        0        0   128273 2022-01-24 18:22:25.343588 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/medication.py
--rw-r--r--   0        0        0     3632 2022-01-24 18:22:25.343855 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/other.py
--rw-r--r--   0        0        0    10063 2022-01-24 18:22:25.344034 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/patient_characteristic.py
--rw-r--r--   0        0        0     4931 2022-01-24 18:22:25.344207 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/physical_exam.py
--rw-r--r--   0        0        0    78882 2022-01-24 18:22:25.344751 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/procedure.py
--rw-r--r--   0        0        0    42821 2022-01-24 18:22:25.345186 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/procedure_performed.py
--rw-r--r--   0        0        0     4780 2022-01-24 18:22:25.345404 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/rationale.py
--rw-r--r--   0        0        0     3127 2022-01-24 18:22:25.345605 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/result.py
--rw-r--r--   0        0        0     1033 2022-03-25 15:24:57.960685 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/adverse_event.py
--rw-r--r--   0        0        0    11133 2022-03-25 15:24:57.960950 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/allergy.py
--rw-r--r--   0        0        0     8287 2022-03-25 15:24:57.961154 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/assessment.py
--rw-r--r--   0        0        0    18037 2022-03-25 15:24:57.961421 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/communication.py
--rw-r--r--   0        0        0  3409267 2022-03-25 15:24:57.975175 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/condition.py
--rw-r--r--   0        0        0    12984 2022-03-25 15:24:57.975659 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/device.py
--rw-r--r--   0        0        0   301935 2022-03-25 15:24:57.977187 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/diagnostic_study.py
--rw-r--r--   0        0        0   370966 2022-03-25 15:24:57.978813 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/encounter.py
--rw-r--r--   0        0        0    13190 2022-03-25 15:24:57.979075 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/immunization.py
--rw-r--r--   0        0        0    13207 2022-03-25 15:24:57.979333 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/individual_characteristic.py
--rw-r--r--   0        0        0    79797 2022-03-25 15:24:57.979862 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/intervention.py
--rw-r--r--   0        0        0    77877 2022-03-25 15:24:57.980365 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/laboratory_test.py
--rw-r--r--   0        0        0   316408 2022-03-25 15:24:57.981664 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/medication.py
--rw-r--r--   0        0        0     7646 2022-03-25 15:24:57.981905 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/physical_exam.py
--rw-r--r--   0        0        0   367765 2022-03-25 15:24:57.983433 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/procedure.py
--rw-r--r--   0        0        0     9397 2022-03-25 15:24:57.983676 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/symptom.py
--rw-r--r--   0        0        0     1647 2022-01-24 18:22:25.345780 canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/value_set.py
--rw-r--r--   0        0        0      970 2023-05-10 02:12:07.625341 canvas-workflow-kit-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     4938 2023-05-10 02:12:27.222297 canvas-workflow-kit-0.6.3/setup.py
--rw-r--r--   0        0        0      701 2023-05-10 02:12:27.222555 canvas-workflow-kit-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-01-24 18:22:24.118414 canvas-workflow-kit-0.6.4/canvas_workflow_kit/__init__.py
+-rw-r--r--   0        0        0      222 2022-01-24 18:22:24.118633 canvas-workflow-kit-0.6.4/canvas_workflow_kit/action.py
+-rw-r--r--   0        0        0      446 2022-01-24 18:22:24.118811 canvas-workflow-kit-0.6.4/canvas_workflow_kit/api.py
+-rw-r--r--   0        0        0        0 2022-01-24 18:22:24.118980 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/__init__.py
+-rw-r--r--   0        0        0     7262 2022-03-25 15:24:57.922245 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/ccp001v1_symptomatic_surveillance.py
+-rw-r--r--   0        0        0     5599 2022-01-24 18:22:24.119450 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/ccp002v1_high_risk_outreach.py
+-rw-r--r--   0        0        0     2984 2022-01-24 18:22:24.119637 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/ccp003v1_hypertension.py
+-rw-r--r--   0        0        0     2909 2022-01-24 18:22:24.119822 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/ccp004v1_diabetes.py
+-rw-r--r--   0        0        0     2890 2022-01-24 18:22:24.120010 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/ccp005v1_asthma.py
+-rw-r--r--   0        0        0    10349 2022-01-24 18:22:24.120304 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms122v6_diabetes_hemoglobin_a1c_poor_control.py
+-rw-r--r--   0        0        0    10002 2022-01-24 18:22:24.120594 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms123v6_diabetes_foot_exam.py
+-rw-r--r--   0        0        0    11932 2022-01-24 18:22:24.120864 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms125v6_breast_cancer_screening.py
+-rw-r--r--   0        0        0    15713 2022-01-24 18:22:24.121172 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms130v6_colorectal_cancer_screening.py
+-rw-r--r--   0        0        0    10454 2022-07-01 20:11:06.858920 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms131v6_diabetes_eye_exam.py
+-rw-r--r--   0        0        0    12568 2022-01-24 18:22:24.122515 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms134v6_diabetes_medical_attention_for_nephropathy.py
+-rw-r--r--   0        0        0    24515 2022-03-25 15:24:57.922691 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms138v6_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py
+-rw-r--r--   0        0        0     3394 2022-01-24 18:22:24.124704 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms138v6p1.py
+-rw-r--r--   0        0        0     3924 2022-01-24 18:22:24.125229 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms138v6p2.py
+-rw-r--r--   0        0        0    10891 2022-01-24 18:22:24.125896 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/customer_scan_complex_case_management_referral.py
+-rw-r--r--   0        0        0     8629 2022-01-24 18:22:24.126230 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/customer_scan_dementia_assessment.py
+-rw-r--r--   0        0        0     3837 2022-01-24 18:22:24.126594 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/customer_scan_hcc_suspect_alert.py
+-rw-r--r--   0        0        0     9104 2022-01-24 18:22:24.126824 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/customer_scan_mood_disorder.py
+-rw-r--r--   0        0        0     9347 2022-01-24 18:22:24.127125 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/customer_scan_physical_activity_intervention.py
+-rw-r--r--   0        0        0     7673 2022-01-24 18:22:24.127569 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/customer_scan_urinary_symptoms_assessment.py
+-rw-r--r--   0        0        0     2886 2022-01-24 18:22:24.127995 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/diabetes_quality_measure.py
+-rw-r--r--   0        0        0    13314 2022-01-24 18:22:24.128495 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms138v6_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py
+-rw-r--r--   0        0        0     8142 2022-01-24 18:22:24.128740 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms139v6_falls_screening_for_future_fall_risk.py
+-rw-r--r--   0        0        0     8900 2022-01-24 18:22:24.128977 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms147v7_preventive_care_and_screening_influenza_immunization.py
+-rw-r--r--   0        0        0    17371 2022-01-24 18:22:24.129240 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms156v6_use_of_high_risk_medications_in_the_elderly.py
+-rw-r--r--   0        0        0     9884 2022-01-24 18:22:24.129496 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms182v6_ischemic_vascular_disease_complete_lipid_profile_and_ldl_c_control.py
+-rw-r--r--   0        0        0    19442 2022-01-24 18:22:24.129850 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms2v7_preventive_care_and_screening_screening_for_depression_and_follow_up_plan.py
+-rw-r--r--   0        0        0     7967 2022-01-24 18:22:24.130622 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms50v6_closing_the_referral_loop_receipt_of_specialist_report.py
+-rw-r--r--   0        0        0    25550 2022-01-24 18:22:24.131754 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms69v6_preventive_care_and_screening_body_mass_index_screening_and_follow_up_plan.py
+-rw-r--r--   0        0        0     9553 2022-01-24 18:22:24.132180 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cqm_CMS127v6_pneumococcal.py
+-rw-r--r--   0        0        0     3638 2022-01-24 18:22:24.132470 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cqm_CMS160v6_depression.py
+-rw-r--r--   0        0        0     1625 2022-01-24 18:22:24.132732 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/quality_measure_document.py
+-rw-r--r--   0        0        0     5125 2022-01-24 18:22:24.133209 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/hcc001v1_problem_list_hygiene.py
+-rw-r--r--   0        0        0     4937 2022-01-24 18:22:24.133586 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/hcc002v2_ckd_suspect.py
+-rw-r--r--   0        0        0     9228 2022-01-24 18:22:24.134066 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/hcc003v1_diabetes_mellitus_with_seconday_complication_suspect.py
+-rw-r--r--   0        0        0     3381 2022-01-24 18:22:24.134384 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/hcc004v1_dysrhythmia_suspect.py
+-rw-r--r--   0        0        0     3795 2022-01-24 18:22:24.134738 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/hcc005v1_annual_wellness_visit.py
+-rw-r--r--   0        0        0      519 2022-01-24 18:22:24.134957 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/helper_population.py
+-rw-r--r--   0        0        0     2081 2022-01-24 18:22:24.135172 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/hyperlink_recommendation.py
+-rw-r--r--   0        0        0     1032 2022-01-24 18:22:24.135461 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stub_template.py.txt
+-rw-r--r--   0        0        0     2291 2022-01-24 18:22:24.135745 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stub_template_user.py.txt
+-rw-r--r--   0        0        0    11894 2022-01-24 18:22:24.137659 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/_importlib_modulespec.data.json
+-rw-r--r--   0        0        0     1105 2022-01-24 18:22:24.137971 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/_importlib_modulespec.meta.json
+-rw-r--r--   0        0        0    12251 2022-01-24 18:22:24.138971 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/abc.data.json
+-rw-r--r--   0        0        0     1058 2022-01-24 18:22:24.139232 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/abc.meta.json
+-rw-r--r--   0        0        0   601115 2022-01-24 18:22:24.140943 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/builtins.data.json
+-rw-r--r--   0        0        0     1099 2022-01-24 18:22:24.141348 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/builtins.meta.json
+-rw-r--r--   0        0        0     9837 2022-01-24 18:22:24.141652 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms123v5_diabetes_foot_exam.data.json
+-rw-r--r--   0        0        0     1157 2022-01-24 18:22:24.141904 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms123v5_diabetes_foot_exam.meta.json
+-rw-r--r--   0        0        0     9613 2022-01-24 18:22:24.142113 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms124v6_cervical_cancer_screening.data.json
+-rw-r--r--   0        0        0     1171 2022-01-24 18:22:24.142347 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms124v6_cervical_cancer_screening.meta.json
+-rw-r--r--   0        0        0   216922 2022-01-24 18:22:24.143163 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/__init__.data.json
+-rw-r--r--   0        0        0     1125 2022-01-24 18:22:24.143370 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3467 2022-01-24 18:22:24.143565 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/abc.data.json
+-rw-r--r--   0        0        0     1088 2022-01-24 18:22:24.143749 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/abc.meta.json
+-rw-r--r--   0        0        0     9096 2022-01-24 18:22:24.144081 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/mypy_extensions.data.json
+-rw-r--r--   0        0        0     1080 2022-01-24 18:22:24.144301 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/mypy_extensions.meta.json
+-rw-r--r--   0        0        0    46004 2022-01-24 18:22:24.144554 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/sys.data.json
+-rw-r--r--   0        0        0     1082 2022-01-24 18:22:24.144781 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/sys.meta.json
+-rw-r--r--   0        0        0    67237 2022-01-24 18:22:24.145331 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/types.data.json
+-rw-r--r--   0        0        0     1091 2022-01-24 18:22:24.145563 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/types.meta.json
+-rw-r--r--   0        0        0   306873 2022-01-24 18:22:24.146132 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/typing.data.json
+-rw-r--r--   0        0        0     1094 2022-01-24 18:22:24.146335 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/typing.meta.json
+-rw-r--r--   0        0        0    12618 2022-01-24 18:22:24.146571 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms117v9_childhood_immunization_status.py
+-rw-r--r--   0        0        0     6916 2022-01-24 18:22:24.146811 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms122v9_diabetes_hemoglobin_a1c_poor_control.py
+-rw-r--r--   0        0        0     5274 2022-01-24 18:22:24.147165 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms124v9_cervical_cancer_screening.py
+-rw-r--r--   0        0        0     6301 2022-01-24 18:22:24.147478 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms125v9_breast_cancer_screening.py
+-rw-r--r--   0        0        0     7569 2022-01-24 18:22:24.147833 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms127v9_pneumococcal_vaccination_status_for_older_adults.py
+-rw-r--r--   0        0        0    10387 2022-01-24 18:22:24.148711 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms128v9_anti_depressant_medication_management.py
+-rw-r--r--   0        0        0     7647 2022-01-24 18:22:24.149094 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms129v10_prostate_cancer_avoidance_of_overuse_of_bone_scan_for_staging_low_risk_prostate_cancer_patients.py
+-rw-r--r--   0        0        0     6119 2022-01-24 18:22:24.149302 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms130v9_colorectal_cancer_screening.py
+-rw-r--r--   0        0        0     7376 2022-01-24 18:22:24.149585 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms131v9_diabetes_eye_exam.py
+-rw-r--r--   0        0        0    10990 2022-01-24 18:22:24.149934 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms133v9_cataracts_20_40_or_better_visual_acuity_within_90_days_following_cataract_surgery.py
+-rw-r--r--   0        0        0    10284 2022-01-24 18:22:24.150271 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms134v9_diabetes_medical_attention_for_nephropathy.py
+-rw-r--r--   0        0        0    11991 2022-01-24 18:22:24.150627 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms135v9_heart_failure_angiotensin_converting_enzyme_inhibitor_or_angiotensin_receptor_blocker_or_angiotensin_receptor_neprilysin_inhibitor_therapy_for_left_ventricular_systolic_dysfunction.py
+-rw-r--r--   0        0        0    15664 2022-01-24 18:22:24.151308 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms136v10_follow_up_care_for_children_prescribed_adhd_medication.py
+-rw-r--r--   0        0        0    12563 2022-01-24 18:22:24.151690 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms137v9_initiation_and_engagement_of_alcohol_and_other_drug_dependence_treatment.py
+-rw-r--r--   0        0        0    11350 2022-01-24 18:22:24.152066 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms138v9_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py
+-rw-r--r--   0        0        0     6105 2022-01-24 18:22:24.152445 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms139v9_falls_screening_for_future_fall_risk.py
+-rw-r--r--   0        0        0     7917 2022-01-24 18:22:24.152878 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms142v9_diabetic_retinopathy_communication_with_the_physician_managing_ongoing_diabetes_care.py
+-rw-r--r--   0        0        0     6525 2022-01-24 18:22:24.153238 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms143v9_primary_open_angle_glaucoma_optic_nerve_evaluation.py
+-rw-r--r--   0        0        0     8623 2022-01-24 18:22:24.153626 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms144v9_heart_failure_beta_blocker_therapy_for_left_ventricular_systolic_dysfunction.py
+-rw-r--r--   0        0        0     7002 2022-01-24 18:22:24.154141 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms145v9_coronary_artery_disease_beta_blocker_therapy_prior_myocardial_infarction_or_left_ventricular_systolic_dysfunction.py
+-rw-r--r--   0        0        0     5333 2022-01-24 18:22:24.154430 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms146v9_appropriate_testing_for_pharyngitis.py
+-rw-r--r--   0        0        0     7666 2022-01-24 18:22:24.154860 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms147v10_preventive_care_and_screening_influenza_immunization.py
+-rw-r--r--   0        0        0    11366 2022-01-24 18:22:24.155148 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms149v9_dementia_cognitive_assessment.py
+-rw-r--r--   0        0        0     5137 2022-01-24 18:22:24.155438 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms153v9_chlamydia_screening_for_women.py
+-rw-r--r--   0        0        0     4797 2022-01-24 18:22:24.155799 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms154v9_appropriate_treatment_for_upper_respiratory_infection.py
+-rw-r--r--   0        0        0     7220 2022-01-24 18:22:24.156105 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms155v9_weight_assessment_and_counseling_for_nutrition_and_physical_activity_for_children_and_adolescents.py
+-rw-r--r--   0        0        0    10832 2022-01-24 18:22:24.156397 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms156v9_use_of_high_risk_medications_in_older_adults.py
+-rw-r--r--   0        0        0     8583 2022-01-24 18:22:24.156709 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms157v9_oncology_medical_and_radiation_pain_intensity_quantified.py
+-rw-r--r--   0        0        0    17246 2022-01-24 18:22:24.157156 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms159v9_depression_remission_at_twelve_months.py
+-rw-r--r--   0        0        0    13128 2022-01-24 18:22:24.157634 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms161v9_adult_major_depressive_disorder_suicide_risk_assessment.py
+-rw-r--r--   0        0        0    13690 2022-01-24 18:22:24.158007 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms165v9_controlling_high_blood_pressure.py
+-rw-r--r--   0        0        0     8069 2022-01-24 18:22:24.158343 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms177v9_child_and_adolescent_major_depressive_disorder_suicide_risk_assessment.py
+-rw-r--r--   0        0        0    12217 2022-01-24 18:22:24.158600 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms22v9_preventive_care_and_screening_screening_for_high_blood_pressure_and_follow_up_documented.py
+-rw-r--r--   0        0        0    12527 2022-01-24 18:22:24.158864 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms249v3_appropriate_use_of_dxa_scans_in_women_under_65_years_who_do_not_meet_the_risk_factor_profile_for_osteoporotic_fracture.py
+-rw-r--r--   0        0        0    17320 2022-01-24 18:22:24.159308 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms2v10_preventive_care_and_screening_screening_for_depression_and_follow_up_plan.py
+-rw-r--r--   0        0        0    18696 2022-01-24 18:22:24.159707 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms347v4_statin_therapy_for_the_prevention_and_treatment_of_cardiovascular_disease.py
+-rw-r--r--   0        0        0     8675 2022-01-24 18:22:24.159948 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms349v3_hiv_screening.py
+-rw-r--r--   0        0        0     8513 2022-01-24 18:22:24.160197 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms50v9_closing_the_referral_loop_receipt_of_specialist_report.py
+-rw-r--r--   0        0        0     7748 2022-01-24 18:22:24.160429 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms56v9_functional_status_assessment_for_total_hip_replacement.py
+-rw-r--r--   0        0        0     6954 2022-01-24 18:22:24.160658 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms645v4_bone_density_evaluation_for_patients_with_prostate_cancer_and_receiving_androgen_deprivation_therapy.py
+-rw-r--r--   0        0        0     6655 2022-01-24 18:22:24.160899 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms66v9_functional_status_assessment_for_total_knee_replacement.py
+-rw-r--r--   0        0        0    12014 2022-01-24 18:22:24.161138 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms68v10_documentation_of_current_medications_in_the_medical_record.py
+-rw-r--r--   0        0        0    21957 2022-01-24 18:22:24.161568 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms69v9_preventive_care_and_screening_body_mass_index_screening_and_follow_up_plan.py
+-rw-r--r--   0        0        0     4181 2022-01-24 18:22:24.161804 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms74v10_primary_caries_prevention_intervention_as_offered_by_primary_care_providers,_including_dentists.py
+-rw-r--r--   0        0        0     3788 2022-01-24 18:22:24.162066 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms75v9_children_who_have_dental_decay_or_cavities.py
+-rw-r--r--   0        0        0     7673 2022-01-24 18:22:24.162408 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms771v2_urinary_symptom_score_change_6_12_months_after_diagnosis_of_benign_prostatic_hyperplasia.py
+-rw-r--r--   0        0        0     5787 2022-01-24 18:22:24.162671 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms90v10_functional_status_assessments_for_congestive_heart_failure.py
+-rw-r--r--   0        0        0        0 2022-01-24 18:22:24.162901 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-24 18:22:24.163127 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.230397 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/billing_line_items.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.163720 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.163869 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.164022 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.164193 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.164396 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.164785 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/medications.json
+-rw-r--r--   0        0        0       90 2022-01-24 18:22:24.164956 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.165228 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_no/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.232032 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/billing_line_items.json
+-rw-r--r--   0        0        0      416 2022-01-24 18:22:24.165822 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.165994 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.166171 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/instructions.json
+-rw-r--r--   0        0        0      663 2022-01-24 18:22:24.166405 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.166656 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.166951 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/medications.json
+-rw-r--r--   0        0        0       94 2022-01-24 18:22:24.167225 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.167501 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.232880 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/billing_line_items.json
+-rw-r--r--   0        0        0      416 2022-01-24 18:22:24.168133 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.168361 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.168623 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.168858 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/interviews.json
+-rw-r--r--   0        0        0      596 2023-06-13 16:13:36.752173 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.169443 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/medications.json
+-rw-r--r--   0        0        0       94 2022-01-24 18:22:24.169673 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.169935 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.234071 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/billing_line_items.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.170337 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.170482 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.170620 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.170781 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.171003 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.171201 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/medications.json
+-rw-r--r--   0        0        0       90 2022-01-24 18:22:24.171468 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.171760 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_no/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.235249 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/billing_line_items.json
+-rw-r--r--   0        0        0      416 2022-01-24 18:22:24.172510 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.172740 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.172968 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.173186 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.173398 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.173614 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/medications.json
+-rw-r--r--   0        0        0       94 2022-01-24 18:22:24.173860 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.174495 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yes/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.236291 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/billing_line_items.json
+-rw-r--r--   0        0        0      416 2022-01-24 18:22:24.176659 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.176896 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.177056 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/instructions.json
+-rw-r--r--   0        0        0      666 2022-01-24 18:22:24.177236 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.177386 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.177544 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/medications.json
+-rw-r--r--   0        0        0       94 2022-01-24 18:22:24.177758 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.177961 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.237767 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/billing_line_items.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.178474 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/conditions.json
+-rw-r--r--   0        0        0        4 2022-01-24 18:22:24.178618 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/imaging_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.178833 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.179076 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.179273 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.179425 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.179631 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/medications.json
+-rw-r--r--   0        0        0      100 2022-01-24 18:22:24.179814 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.179961 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/referral_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.180101 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_due/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.239253 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/billing_line_items.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.180471 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/conditions.json
+-rw-r--r--   0        0        0      298 2022-01-24 18:22:24.180630 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/imaging_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.180774 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.180913 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.181202 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.181454 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.181688 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/medications.json
+-rw-r--r--   0        0        0      100 2022-01-24 18:22:24.181890 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.182122 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/referral_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.182339 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mammography/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.240447 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/billing_line_items.json
+-rw-r--r--   0        0        0      284 2022-01-24 18:22:24.182958 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.183244 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/imaging_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.183503 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.183759 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.183956 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.184152 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.184308 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/medications.json
+-rw-r--r--   0        0        0      100 2022-01-24 18:22:24.184508 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.184768 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/referral_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.185012 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms125v6_woman_mastectomy/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.241430 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_due/billing_line_items.json
+-rw-r--r--   0        0        0       78 2022-01-24 18:22:24.185549 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_due/patient.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.242196 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_satisfied/billing_line_items.json
+-rw-r--r--   0        0        0      208 2022-01-24 18:22:24.186397 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_satisfied/imaging_reports.json
+-rw-r--r--   0        0        0      114 2023-06-13 16:13:36.753926 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_satisfied/lab_reports.json
+-rw-r--r--   0        0        0       78 2022-01-24 18:22:24.186736 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_satisfied/patient.json
+-rw-r--r--   0        0        0      203 2022-01-24 18:22:24.186926 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms130v6_patient_satisfied/referral_reports.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.243527 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/billing_line_items.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.187594 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.188114 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.188374 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.188647 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.188928 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.189187 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/medications.json
+-rw-r--r--   0        0        0       90 2022-01-24 18:22:24.189485 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.189656 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/referral_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.189884 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_no/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.244205 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/billing_line_items.json
+-rw-r--r--   0        0        0      416 2022-01-24 18:22:24.190480 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.190652 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.190822 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.191009 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.191225 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.191476 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/medications.json
+-rw-r--r--   0        0        0       94 2022-01-24 18:22:24.191652 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.191805 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/referral_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.191940 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yesnoreferralreport/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.244881 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/billing_line_items.json
+-rw-r--r--   0        0        0      416 2022-01-24 18:22:24.192403 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.192593 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.192757 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.192905 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.193059 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.193206 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/medications.json
+-rw-r--r--   0        0        0       94 2022-01-24 18:22:24.193346 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/patient.json
+-rw-r--r--   0        0        0      564 2022-01-24 18:22:24.193507 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/referral_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.193653 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.245811 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/billing_line_items.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.194076 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.194221 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.194396 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.194548 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.194752 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.194953 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/medications.json
+-rw-r--r--   0        0        0       94 2022-01-24 18:22:24.195150 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.195308 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_no/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.246817 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/billing_line_items.json
+-rw-r--r--   0        0        0      658 2022-01-24 18:22:24.195662 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.195792 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/immunizations.json
+-rw-r--r--   0        0        0      219 2022-01-24 18:22:24.195935 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.196117 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/interviews.json
+-rw-r--r--   0        0        0      233 2023-06-13 16:13:36.755827 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/lab_reports.json
+-rw-r--r--   0        0        0      276 2022-01-24 18:22:24.196405 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/medications.json
+-rw-r--r--   0        0        0       94 2022-01-24 18:22:24.196537 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/patient.json
+-rw-r--r--   0        0        0      269 2022-01-24 18:22:24.196671 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/referral_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.196797 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.247450 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes_only/billing_line_items.json
+-rw-r--r--   0        0        0      416 2022-01-24 18:22:24.197168 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes_only/conditions.json
+-rw-r--r--   0        0        0       94 2022-01-24 18:22:24.197307 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes_only/patient.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.259324 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms138v6/billing_line_items.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.197713 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms138v6/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.197840 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms138v6/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.198042 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms138v6/medications.json
+-rw-r--r--   0        0        0      100 2022-01-24 18:22:24.198209 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms138v6/patient.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.260326 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetes_mixin/billing_line_items.json
+-rw-r--r--   0        0        0      416 2022-01-24 18:22:24.198731 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetes_mixin/conditions.json
+-rw-r--r--   0        0        0       95 2022-01-24 18:22:24.198905 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetes_mixin/patient.json
+-rw-r--r--   0        0        0      448 2022-01-24 18:22:24.199225 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.199384 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.199579 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.199742 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.199938 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.200155 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/medications.json
+-rw-r--r--   0        0        0      108 2022-01-24 18:22:24.200385 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.200606 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/diabetic1/vital_signs.json
+-rw-r--r--   0        0        0      351 2022-01-24 18:22:24.201247 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.201473 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/immunizations.json
+-rw-r--r--   0        0        0      533 2022-01-24 18:22:24.201745 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/instructions.json
+-rw-r--r--   0        0        0     8462 2022-01-24 18:22:24.202031 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.202195 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/lab_reports.json
+-rw-r--r--   0        0        0    14914 2022-01-24 18:22:24.202541 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/medications.json
+-rw-r--r--   0        0        0      108 2022-01-24 18:22:24.202759 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.202933 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/vital_signs.json
+-rw-r--r--   0        0        0      632 2022-01-24 18:22:24.203237 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.203491 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.203685 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.203882 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.204116 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.204441 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/medications.json
+-rw-r--r--   0        0        0       78 2022-01-24 18:22:24.204649 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.204819 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/vital_signs.json
+-rw-r--r--   0        0        0      513 2022-01-24 18:22:24.205066 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.205227 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.205386 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.205548 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/interviews.json
+-rw-r--r--   0        0        0      403 2023-06-13 16:13:36.757786 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.205895 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/medications.json
+-rw-r--r--   0        0        0      133 2022-01-24 18:22:24.206041 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.206179 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/vital_signs.json
+-rw-r--r--   0        0        0      369 2022-01-24 18:22:24.206407 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.206585 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.206729 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.206964 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.207202 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.207671 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/medications.json
+-rw-r--r--   0        0        0       78 2022-01-24 18:22:24.208040 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.208225 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc003v1_diagnosed/vital_signs.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.208463 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.208608 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.208823 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.209044 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.209270 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.209552 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/medications.json
+-rw-r--r--   0        0        0       78 2022-01-24 18:22:24.209763 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.210010 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc004v1/vital_signs.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.210255 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.210431 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.210574 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.210721 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.210904 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.211170 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/medications.json
+-rw-r--r--   0        0        0       78 2022-01-24 18:22:24.211347 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.211499 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc005v1/vital_signs.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.211765 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.211921 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.212079 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.212231 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.212388 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.212603 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/medications.json
+-rw-r--r--   0        0        0      116 2022-01-24 18:22:24.212757 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:24.212904 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/patient/vital_signs.json
+-rw-r--r--   0        0        0    23878 2022-01-24 18:22:24.213165 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_ccp001v1_symptomatic_surveillance.py
+-rw-r--r--   0        0        0    19759 2022-01-24 18:22:24.213412 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_ccp002v1_high_risk_outreach.py
+-rw-r--r--   0        0        0     8282 2022-01-24 18:22:24.213625 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_ccp003v1_hypertension.py
+-rw-r--r--   0        0        0     8240 2022-01-24 18:22:24.213838 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_ccp004v1_diabetes.py
+-rw-r--r--   0        0        0     8201 2022-01-24 18:22:24.214048 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_ccp005v1_asthma.py
+-rw-r--r--   0        0        0    18063 2022-07-01 20:11:06.859263 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms122v6_diabetes_hemoglobin_a1c_poor_control.py
+-rw-r--r--   0        0        0    16610 2022-07-01 20:11:06.859608 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms123v6_diabetes_foot_exam.py
+-rw-r--r--   0        0        0    23648 2022-07-01 20:11:06.859959 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms125v6_breast_cancer_screening.py
+-rw-r--r--   0        0        0    30237 2022-07-01 20:11:06.865305 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms130v6_colorectal_cancer_screening.py
+-rw-r--r--   0        0        0    21800 2022-07-01 20:11:06.865737 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms131v6_diabetes_eye_exam.py
+-rw-r--r--   0        0        0    19107 2022-07-01 20:11:06.866100 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms134v6_diabetes_medical_attention_for_nephropathy.py
+-rw-r--r--   0        0        0    49276 2022-07-01 20:11:06.866598 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms138v6_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py
+-rw-r--r--   0        0        0    22181 2022-07-01 20:11:06.867115 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms138v6p1.py
+-rw-r--r--   0        0        0    25266 2022-07-01 20:11:06.867637 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms138v6p2.py
+-rw-r--r--   0        0        0    10949 2022-07-01 20:11:06.873417 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_diabetes_quality_measure.py
+-rw-r--r--   0        0        0    16283 2022-01-24 18:22:24.219181 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_hcc001v1_problem_list_hygiene.py
+-rw-r--r--   0        0        0    13281 2022-01-24 18:22:24.219535 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_hcc002v2_ckd_suspect.py
+-rw-r--r--   0        0        0    34017 2022-01-24 18:22:24.219804 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_hcc003v1_diabetes_mellitus_with_seconday_complication_suspect.py
+-rw-r--r--   0        0        0    12234 2022-01-24 18:22:24.220114 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_hcc004v1_dysrhythmia_suspect.py
+-rw-r--r--   0        0        0     9296 2022-07-01 20:11:06.873889 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_hcc005v1_annual_wellness_visit.py
+-rw-r--r--   0        0        0     1692 2022-01-24 18:22:24.220606 canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_helper_population.py
+-rwxr-xr-x   0        0        0    12678 2022-07-01 20:11:06.874784 canvas-workflow-kit-0.6.4/canvas_workflow_kit/canvas_cli.py
+-rw-r--r--   0        0        0     3493 2022-01-24 18:22:24.221281 canvas-workflow-kit-0.6.4/canvas_workflow_kit/canvas_code_set.py
+-rw-r--r--   0        0        0     4009 2023-06-13 16:13:36.758615 canvas-workflow-kit-0.6.4/canvas_workflow_kit/constants.py
+-rw-r--r--   0        0        0      852 2022-01-24 18:22:24.221783 canvas-workflow-kit-0.6.4/canvas_workflow_kit/events.py
+-rwxr-xr-x   0        0        0    12515 2022-01-24 18:22:24.222185 canvas-workflow-kit-0.6.4/canvas_workflow_kit/generate_cqms_stubs.py
+-rw-r--r--   0        0        0     1360 2022-01-24 18:22:24.222626 canvas-workflow-kit-0.6.4/canvas_workflow_kit/internal/attrdict.py
+-rw-r--r--   0        0        0     3384 2023-04-24 18:35:18.261857 canvas-workflow-kit-0.6.4/canvas_workflow_kit/internal/integration_messages.py
+-rw-r--r--   0        0        0     1210 2022-01-24 18:22:24.222895 canvas-workflow-kit-0.6.4/canvas_workflow_kit/internal/string.py
+-rw-r--r--   0        0        0     2029 2022-01-24 18:22:24.223204 canvas-workflow-kit-0.6.4/canvas_workflow_kit/intervention.py
+-rw-r--r--   0        0        0      932 2022-01-24 18:22:24.223569 canvas-workflow-kit-0.6.4/canvas_workflow_kit/metaclass.py
+-rw-r--r--   0        0        0    10674 2023-06-13 16:13:36.761567 canvas-workflow-kit-0.6.4/canvas_workflow_kit/patient.py
+-rw-r--r--   0        0        0    25693 2023-06-13 16:13:36.764147 canvas-workflow-kit-0.6.4/canvas_workflow_kit/patient_recordset.py
+-rw-r--r--   0        0        0    22919 2023-04-24 18:35:18.263646 canvas-workflow-kit-0.6.4/canvas_workflow_kit/protocol.py
+-rw-r--r--   0        0        0    15651 2023-06-13 16:13:36.765662 canvas-workflow-kit-0.6.4/canvas_workflow_kit/recommendation.py
+-rw-r--r--   0        0        0     1365 2022-01-24 18:22:25.197299 canvas-workflow-kit-0.6.4/canvas_workflow_kit/settings.py
+-rw-r--r--   0        0        0        0 2022-01-24 18:22:25.197473 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/__init__.py
+-rw-r--r--   0        0        0     1612 2022-01-24 18:22:25.197673 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/base.py
+-rw-r--r--   0        0        0        0 2022-01-24 18:22:25.197836 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/get_protocols_unittest/__init__.py
+-rw-r--r--   0        0        0     5139 2022-01-24 18:22:25.198025 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/get_protocols_unittest/protocol_unittest.py
+-rw-r--r--   0        0        0        3 2023-04-24 18:35:18.263881 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/appointments.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.198540 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/billing_line_items.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.198699 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/conditions.json
+-rw-r--r--   0        0        0        3 2022-09-12 21:45:44.061343 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/consents.json
+-rw-r--r--   0        0        0        3 2023-04-24 18:35:18.263999 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/external_events.json
+-rw-r--r--   0        0        0        2 2022-09-12 21:45:44.062431 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/groups.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.198864 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/imaging_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.199017 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.199154 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/inpatientStay.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.199289 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.199431 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/interviews.json
+-rw-r--r--   0        0        0        3 2023-06-13 16:13:36.765899 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/lab_orders.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.199603 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.199750 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/medications.json
+-rw-r--r--   0        0        0      106 2022-01-24 18:22:25.199914 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/patient.json
+-rw-r--r--   0        0        0        3 2022-04-27 22:44:55.538708 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/prescriptions.json
+-rw-r--r--   0        0        0        3 2022-04-28 22:56:13.276213 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/procedures.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.200117 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/protocol_overrides.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.200839 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/referral_reports.json
+-rw-r--r--   0        0        0        3 2022-09-12 21:45:44.062707 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/tasks.py
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.202186 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty/vitalsigns.json
+-rw-r--r--   0        0        0      719 2022-01-24 18:22:25.198277 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty.json
+-rw-r--r--   0        0        0     4523 2023-04-24 18:35:18.269650 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/appointments.json
+-rw-r--r--   0        0        0      325 2022-04-28 22:56:13.279929 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/billing_line_items.json
+-rw-r--r--   0        0        0     3024 2022-01-24 18:22:25.203348 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/conditions.json
+-rw-r--r--   0        0        0     1675 2022-09-12 21:45:44.068285 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/consents.json
+-rw-r--r--   0        0        0      449 2023-04-24 18:35:18.269889 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/external_events.json
+-rw-r--r--   0        0        0      146 2022-09-12 21:45:44.069326 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/groups.json
+-rw-r--r--   0        0        0      747 2022-01-24 18:22:25.203793 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/imaging_reports.json
+-rw-r--r--   0        0        0      328 2022-01-24 18:22:25.204329 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/immunizations.json
+-rw-r--r--   0        0        0      155 2022-01-24 18:22:25.204559 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/inpatientStay.json
+-rw-r--r--   0        0        0      197 2022-01-24 18:22:25.204884 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/instructions.json
+-rw-r--r--   0        0        0      898 2022-01-24 18:22:25.205414 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/interviews.json
+-rw-r--r--   0        0        0     1147 2023-06-13 16:13:36.767971 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/lab_orders.json
+-rw-r--r--   0        0        0     1443 2023-06-13 16:13:36.769896 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/lab_reports.json
+-rw-r--r--   0        0        0      544 2022-01-24 18:22:25.205812 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/medications.json
+-rw-r--r--   0        0        0      409 2022-01-24 18:22:25.205998 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/patient.json
+-rw-r--r--   0        0        0      700 2022-04-27 22:44:55.546421 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/prescriptions.json
+-rw-r--r--   0        0        0      486 2022-04-28 22:56:13.307651 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/procedures.json
+-rw-r--r--   0        0        0      649 2022-01-24 18:22:25.206165 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/protocol_overrides.json
+-rw-r--r--   0        0        0      315 2022-01-24 18:22:25.206334 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/referral_reports.json
+-rw-r--r--   0        0        0     4238 2022-01-24 18:22:25.206497 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/referrals.json
+-rw-r--r--   0        0        0     1571 2022-09-12 21:45:44.074048 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/tasks.json
+-rw-r--r--   0        0        0      260 2022-01-24 18:22:25.206698 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/vital_signs.json
+-rw-r--r--   0        0        0     7367 2022-04-28 22:56:13.279197 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full.json
+-rw-r--r--   0        0        0     1030 2023-04-24 18:35:18.275606 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/appointments.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.207006 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/billing_line_items.json
+-rw-r--r--   0        0        0      724 2022-01-24 18:22:25.207195 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/conditions.json
+-rw-r--r--   0        0        0      730 2022-09-12 21:45:44.091760 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/consents.json
+-rw-r--r--   0        0        0        3 2023-04-24 18:35:18.275810 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/external_events.json
+-rw-r--r--   0        0        0        2 2022-09-12 21:45:44.092132 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/groups.json
+-rw-r--r--   0        0        0      450 2022-01-24 18:22:25.207424 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/imaging_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.207734 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.207982 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/inpatientStay.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.208325 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/instructions.json
+-rw-r--r--   0        0        0      283 2022-01-24 18:22:25.208620 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/interviews.json
+-rw-r--r--   0        0        0        3 2023-06-13 16:13:36.770115 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/lab_orders.json
+-rw-r--r--   0        0        0      505 2023-06-13 16:13:36.771824 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/lab_reports.json
+-rw-r--r--   0        0        0      270 2022-01-24 18:22:25.209256 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/medications.json
+-rw-r--r--   0        0        0      409 2022-01-24 18:22:25.209440 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/patient.json
+-rw-r--r--   0        0        0        3 2022-04-27 22:44:55.546733 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/prescriptions.json
+-rw-r--r--   0        0        0        3 2022-04-28 22:56:13.307958 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/procedures.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.209720 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/protocol_overrides.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.209985 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/referral_reports.json
+-rw-r--r--   0        0        0        3 2022-09-12 21:45:44.092379 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/tasks.json
+-rw-r--r--   0        0        0      174 2022-01-24 18:22:25.210192 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/vital_signs.json
+-rw-r--r--   0        0        0        0 2022-01-24 18:22:25.210346 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/__init__.py
+-rw-r--r--   0        0        0      246 2022-01-24 18:22:25.210603 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/base.py
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.211209 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.211375 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.211517 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.211885 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.212194 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.212489 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1/medications.json
+-rw-r--r--   0        0        0      108 2022-01-24 18:22:25.212666 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1/patient.json
+-rw-r--r--   0        0        0     1355 2022-01-24 18:22:25.213027 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1/vital_signs.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.213593 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.213901 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/immunizations.json
+-rw-r--r--   0        0        0      888 2022-01-24 18:22:25.214181 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.214498 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.214773 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.215012 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/medications.json
+-rw-r--r--   0        0        0      108 2022-01-24 18:22:25.215238 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/patient.json
+-rw-r--r--   0        0        0     1355 2022-01-24 18:22:25.215582 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/vital_signs.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.215829 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi2/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.216742 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi2/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.217011 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi2/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.217182 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi2/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.217669 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi2/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.218062 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi2/medications.json
+-rw-r--r--   0        0        0      108 2022-01-24 18:22:25.218303 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi2/patient.json
+-rw-r--r--   0        0        0     1355 2022-01-24 18:22:25.218700 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi2/vital_signs.json
+-rw-r--r--   0        0        0    28246 2022-01-24 18:22:25.219159 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/conditions.json
+-rw-r--r--   0        0        0     1279 2022-01-24 18:22:25.219532 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.219817 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/instructions.json
+-rw-r--r--   0        0        0     2251 2022-01-24 18:22:25.220186 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.220730 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/lab_reports.json
+-rw-r--r--   0        0        0    17754 2022-01-24 18:22:25.221022 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/medications.json
+-rw-r--r--   0        0        0     2758 2022-01-24 18:22:25.221301 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/patient.json
+-rw-r--r--   0        0        0     6346 2022-01-24 18:22:25.222497 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/vital_signs.json
+-rw-r--r--   0        0        0    28246 2022-01-24 18:22:25.224306 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/conditions.json
+-rw-r--r--   0        0        0     1279 2022-01-24 18:22:25.225300 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/immunizations.json
+-rw-r--r--   0        0        0      908 2022-01-24 18:22:25.226426 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/instructions.json
+-rw-r--r--   0        0        0     2251 2022-01-24 18:22:25.228211 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.229773 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/lab_reports.json
+-rw-r--r--   0        0        0    17754 2022-01-24 18:22:25.231885 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/medications.json
+-rw-r--r--   0        0        0     2758 2022-01-24 18:22:25.233870 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/patient.json
+-rw-r--r--   0        0        0     6346 2022-01-24 18:22:25.234254 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/vital_signs.json
+-rw-r--r--   0        0        0      295 2022-04-28 22:56:13.308902 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/billing_line_items.json
+-rw-r--r--   0        0        0      405 2022-01-24 18:22:25.235113 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.235318 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.235656 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.235958 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.236130 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.236273 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/medications.json
+-rw-r--r--   0        0        0      108 2022-01-24 18:22:25.236414 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.236613 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic1/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.309308 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/billing_line_items.json
+-rw-r--r--   0        0        0      531 2022-01-24 18:22:25.237009 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.237240 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.237424 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.237571 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/interviews.json
+-rw-r--r--   0        0        0      541 2023-06-13 16:13:36.773794 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.238061 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/medications.json
+-rw-r--r--   0        0        0      108 2022-01-24 18:22:25.238215 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.238359 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.310111 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/billing_line_items.json
+-rw-r--r--   0        0        0      531 2022-01-24 18:22:25.238897 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.239132 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.239413 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.239603 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/interviews.json
+-rw-r--r--   0        0        0      541 2023-06-13 16:13:36.775824 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.239962 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/medications.json
+-rw-r--r--   0        0        0      108 2022-01-24 18:22:25.240100 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.240286 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/vital_signs.json
+-rw-r--r--   0        0        0      163 2022-04-28 22:56:13.310532 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/billing_line_items.json
+-rw-r--r--   0        0        0      531 2022-01-24 18:22:25.240723 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.240878 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.241022 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.241199 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/interviews.json
+-rw-r--r--   0        0        0      542 2023-06-13 16:13:36.777871 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.241557 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/medications.json
+-rw-r--r--   0        0        0      108 2022-01-24 18:22:25.241721 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.241861 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/vital_signs.json
+-rw-r--r--   0        0        0      504 2022-01-24 18:22:25.242081 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/example/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.242219 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/example/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.242375 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/example/instructions.json
+-rw-r--r--   0        0        0      219 2022-01-24 18:22:25.242514 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/example/interviews.json
+-rw-r--r--   0        0        0     2192 2023-06-13 16:13:36.799963 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/example/lab_reports.json
+-rw-r--r--   0        0        0     1137 2022-01-24 18:22:25.242781 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/example/medications.json
+-rw-r--r--   0        0        0     2684 2022-01-24 18:22:25.242957 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/example/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.243102 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/example/vital_signs.json
+-rw-r--r--   0        0        0    33067 2022-01-24 18:22:25.243408 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fall1/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.243594 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fall1/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.243726 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fall1/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.243857 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fall1/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.243985 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fall1/lab_reports.json
+-rw-r--r--   0        0        0    14732 2022-01-24 18:22:25.244182 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fall1/medications.json
+-rw-r--r--   0        0        0     2842 2022-01-24 18:22:25.244409 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fall1/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.244576 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fall1/vital_signs.json
+-rw-r--r--   0        0        0      149 2022-04-28 22:56:13.312270 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/feet1/billing_line_items.json
+-rw-r--r--   0        0        0      405 2022-01-24 18:22:25.244992 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/feet1/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.245133 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/feet1/immunizations.json
+-rw-r--r--   0        0        0       81 2022-01-24 18:22:25.245270 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/feet1/instructions.json
+-rw-r--r--   0        0        0      656 2022-01-24 18:22:25.245419 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/feet1/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.245611 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/feet1/lab_reports.json
+-rw-r--r--   0        0        0      807 2022-01-24 18:22:25.245805 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/feet1/medications.json
+-rw-r--r--   0        0        0      108 2022-01-24 18:22:25.245992 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/feet1/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.246183 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/feet1/vital_signs.json
+-rw-r--r--   0        0        0     1396 2022-01-24 18:22:25.246422 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fluvax/conditions.json
+-rw-r--r--   0        0        0     1280 2022-01-24 18:22:25.246576 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fluvax/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.246788 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fluvax/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.246957 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fluvax/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.247168 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fluvax/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.247480 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fluvax/medications.json
+-rw-r--r--   0        0        0      108 2022-01-24 18:22:25.247715 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fluvax/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.247993 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fluvax/vital_signs.json
+-rw-r--r--   0        0        0     8774 2022-01-24 18:22:25.248353 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/#medications.json#
+-rw-r--r--   0        0        0     5923 2022-01-24 18:22:25.248631 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.248928 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.249163 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.249387 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.249603 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/lab_reports.json
+-rw-r--r--   0        0        0     7312 2022-01-24 18:22:25.249961 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/medications.json
+-rw-r--r--   0        0        0     2967 2022-01-24 18:22:25.250642 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.250933 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/referrals.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.251264 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/vital_signs.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.251597 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.251974 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.252527 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/instructions.json
+-rw-r--r--   0        0        0     1668 2022-01-24 18:22:25.253137 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.253396 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.253634 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/medications.json
+-rw-r--r--   0        0        0     2684 2022-01-24 18:22:25.253977 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/patient.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.254249 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/vital_signs.json
+-rw-r--r--   0        0        0     9323 2022-01-24 18:22:25.254671 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/referral/conditions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.254858 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/referral/immunizations.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.255091 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/referral/instructions.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.255379 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/referral/interviews.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.255667 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/referral/lab_reports.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.255910 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/referral/medications.json
+-rw-r--r--   0        0        0     2925 2022-01-24 18:22:25.256082 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/referral/patient.json
+-rw-r--r--   0        0        0     1170 2022-01-24 18:22:25.256248 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/referral/referrals.json
+-rw-r--r--   0        0        0        3 2022-01-24 18:22:25.256465 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/referral/vital_signs.json
+-rw-r--r--   0        0        0      686 2022-01-24 18:22:25.256720 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_interviews.py
+-rw-r--r--   0        0        0     1101 2022-01-24 18:22:25.256901 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_labs.py
+-rw-r--r--   0        0        0      787 2022-01-24 18:22:25.257103 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_medications.py
+-rw-r--r--   0        0        0     5609 2022-01-24 18:22:25.257333 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_protocols.py
+-rw-r--r--   0        0        0     1038 2022-01-24 18:22:25.257553 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_recommendations.py
+-rw-r--r--   0        0        0       78 2022-01-24 18:22:25.257701 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_search.py
+-rw-r--r--   0        0        0      840 2022-01-24 18:22:25.257857 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_value_sets.py
+-rw-r--r--   0        0        0      897 2022-01-24 18:22:25.258099 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_vitalsigns.py
+-rw-r--r--   0        0        0      814 2022-01-24 18:22:25.258356 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_action.py
+-rw-r--r--   0        0        0     4695 2022-01-24 18:22:25.258646 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_canvas_code_set.py
+-rw-r--r--   0        0        0     7767 2022-01-24 18:22:25.259257 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_intervention.py
+-rw-r--r--   0        0        0    16623 2023-06-13 16:13:36.823299 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_patient.py
+-rw-r--r--   0        0        0    63407 2023-06-13 16:13:36.828012 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_patient_recordset.py
+-rw-r--r--   0        0        0    32479 2022-01-24 18:22:25.260562 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_protocol.py
+-rw-r--r--   0        0        0    21355 2023-06-13 16:13:36.830864 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_recommendation.py
+-rw-r--r--   0        0        0     6317 2022-01-24 18:22:25.261095 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_template.py
+-rw-r--r--   0        0        0     3254 2022-01-24 18:22:25.261296 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_timeframe.py
+-rw-r--r--   0        0        0        0 2022-01-24 18:22:25.261469 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/__init__.py
+-rw-r--r--   0        0        0       63 2022-01-24 18:22:25.261707 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/hcc_codes.txt
+-rw-r--r--   0        0        0     1312 2022-01-24 18:22:25.261940 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/hcc_file.txt
+-rw-r--r--   0        0        0      553 2022-01-24 18:22:25.262093 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/hcc_labels.txt
+-rw-r--r--   0        0        0      518 2022-01-24 18:22:25.262318 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/hcc_methods.txt
+-rw-r--r--   0        0        0      552 2022-01-24 18:22:25.262494 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/hcc_sample.tsv
+-rw-r--r--   0        0        0     1238 2022-01-24 18:22:25.262727 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/test_hcc2018.py
+-rw-r--r--   0        0        0     4109 2022-01-24 18:22:25.262921 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/test_specials.py
+-rw-r--r--   0        0        0     7030 2022-01-24 18:22:25.263151 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/test_value_set.py
+-rw-r--r--   0        0        0     1116 2022-03-25 15:24:57.960115 canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/test_value_sets.py
+-rw-r--r--   0        0        0      964 2022-01-24 18:22:25.263321 canvas-workflow-kit-0.6.4/canvas_workflow_kit/timeframe.py
+-rw-r--r--   0        0        0     2156 2022-01-24 18:22:25.263521 canvas-workflow-kit-0.6.4/canvas_workflow_kit/utils.py
+-rw-r--r--   0        0        0       32 2022-03-25 15:24:57.960352 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/__init__.py
+-rw-r--r--   0        0        0     1126 2022-01-24 18:22:25.264054 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/customer_value_sets/scan.py
+-rw-r--r--   0        0        0  2129005 2022-01-24 18:22:25.269826 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/hcc2018.py
+-rw-r--r--   0        0        0  2236826 2022-01-24 18:22:25.286856 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/medication_class_path2018.py
+-rw-r--r--   0        0        0     3993 2022-01-24 18:22:25.287268 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/specials.py
+-rw-r--r--   0        0        0  1895881 2022-01-24 18:22:25.324339 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2017.py
+-rw-r--r--   0        0        0  1180064 2022-01-24 18:22:25.328255 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2018.py
+-rw-r--r--   0        0        0  1167962 2022-01-24 18:22:25.331114 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2019.py
+-rw-r--r--   0        0        0  1281481 2022-01-24 18:22:25.335642 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2020.py
+-rw-r--r--   0        0        0      494 2022-01-24 18:22:25.336139 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/__init__.py
+-rw-r--r--   0        0        0      831 2022-01-24 18:22:25.336367 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/allergy.py
+-rw-r--r--   0        0        0     5248 2022-01-24 18:22:25.336580 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/assessment.py
+-rw-r--r--   0        0        0     5849 2022-01-24 18:22:25.336830 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/assessment_performed.py
+-rw-r--r--   0        0        0     9096 2022-01-24 18:22:25.337101 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/communication.py
+-rw-r--r--   0        0        0     1864 2022-01-24 18:22:25.337319 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/device.py
+-rw-r--r--   0        0        0   970486 2022-01-24 18:22:25.341293 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/diagnosis.py
+-rw-r--r--   0        0        0    34446 2022-01-24 18:22:25.341827 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/encounter.py
+-rw-r--r--   0        0        0    36666 2022-01-24 18:22:25.342246 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/encounter_performed.py
+-rw-r--r--   0        0        0    11438 2022-01-24 18:22:25.342568 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/immunization.py
+-rw-r--r--   0        0        0    29810 2022-01-24 18:22:25.342958 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/lab_test.py
+-rw-r--r--   0        0        0   128273 2022-01-24 18:22:25.343588 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/medication.py
+-rw-r--r--   0        0        0     3632 2022-01-24 18:22:25.343855 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/other.py
+-rw-r--r--   0        0        0    10063 2022-01-24 18:22:25.344034 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/patient_characteristic.py
+-rw-r--r--   0        0        0     4931 2022-01-24 18:22:25.344207 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/physical_exam.py
+-rw-r--r--   0        0        0    78882 2022-01-24 18:22:25.344751 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/procedure.py
+-rw-r--r--   0        0        0    42821 2022-01-24 18:22:25.345186 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/procedure_performed.py
+-rw-r--r--   0        0        0     4780 2022-01-24 18:22:25.345404 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/rationale.py
+-rw-r--r--   0        0        0     3127 2022-01-24 18:22:25.345605 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/result.py
+-rw-r--r--   0        0        0     1033 2022-03-25 15:24:57.960685 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/adverse_event.py
+-rw-r--r--   0        0        0    11133 2022-03-25 15:24:57.960950 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/allergy.py
+-rw-r--r--   0        0        0     8287 2022-03-25 15:24:57.961154 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/assessment.py
+-rw-r--r--   0        0        0    18037 2022-03-25 15:24:57.961421 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/communication.py
+-rw-r--r--   0        0        0  3409267 2022-03-25 15:24:57.975175 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/condition.py
+-rw-r--r--   0        0        0    12984 2022-03-25 15:24:57.975659 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/device.py
+-rw-r--r--   0        0        0   301935 2022-03-25 15:24:57.977187 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/diagnostic_study.py
+-rw-r--r--   0        0        0   370966 2022-03-25 15:24:57.978813 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/encounter.py
+-rw-r--r--   0        0        0    13190 2022-03-25 15:24:57.979075 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/immunization.py
+-rw-r--r--   0        0        0    13207 2022-03-25 15:24:57.979333 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/individual_characteristic.py
+-rw-r--r--   0        0        0    79797 2022-03-25 15:24:57.979862 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/intervention.py
+-rw-r--r--   0        0        0    77877 2022-03-25 15:24:57.980365 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/laboratory_test.py
+-rw-r--r--   0        0        0   316408 2022-03-25 15:24:57.981664 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/medication.py
+-rw-r--r--   0        0        0     7646 2022-03-25 15:24:57.981905 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/physical_exam.py
+-rw-r--r--   0        0        0   367765 2022-03-25 15:24:57.983433 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/procedure.py
+-rw-r--r--   0        0        0     9397 2022-03-25 15:24:57.983676 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/symptom.py
+-rw-r--r--   0        0        0     1647 2022-01-24 18:22:25.345780 canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/value_set.py
+-rw-r--r--   0        0        0      969 2023-06-13 16:26:58.999939 canvas-workflow-kit-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     4952 2023-06-13 16:27:14.689433 canvas-workflow-kit-0.6.4/setup.py
+-rw-r--r--   0        0        0      718 2023-06-13 16:27:14.689827 canvas-workflow-kit-0.6.4/PKG-INFO
```

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/ccp001v1_symptomatic_surveillance.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/ccp001v1_symptomatic_surveillance.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/ccp002v1_high_risk_outreach.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/ccp002v1_high_risk_outreach.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/ccp003v1_hypertension.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/ccp003v1_hypertension.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/ccp004v1_diabetes.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/ccp004v1_diabetes.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/ccp005v1_asthma.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/ccp005v1_asthma.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms122v6_diabetes_hemoglobin_a1c_poor_control.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms122v6_diabetes_hemoglobin_a1c_poor_control.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms123v6_diabetes_foot_exam.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms123v6_diabetes_foot_exam.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms125v6_breast_cancer_screening.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms125v6_breast_cancer_screening.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms130v6_colorectal_cancer_screening.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms130v6_colorectal_cancer_screening.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms131v6_diabetes_eye_exam.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms131v6_diabetes_eye_exam.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms134v6_diabetes_medical_attention_for_nephropathy.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms134v6_diabetes_medical_attention_for_nephropathy.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms138v6_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms138v6_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms138v6p1.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms138v6p1.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/cms138v6p2.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/cms138v6p2.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/customer_scan_complex_case_management_referral.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/customer_scan_complex_case_management_referral.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/customer_scan_dementia_assessment.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/customer_scan_dementia_assessment.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/customer_scan_hcc_suspect_alert.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/customer_scan_hcc_suspect_alert.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/customer_scan_mood_disorder.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/customer_scan_mood_disorder.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/customer_scan_physical_activity_intervention.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/customer_scan_physical_activity_intervention.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/customer_scan_urinary_symptoms_assessment.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/customer_scan_urinary_symptoms_assessment.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/diabetes_quality_measure.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/diabetes_quality_measure.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms138v6_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms138v6_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms139v6_falls_screening_for_future_fall_risk.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms139v6_falls_screening_for_future_fall_risk.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms147v7_preventive_care_and_screening_influenza_immunization.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms147v7_preventive_care_and_screening_influenza_immunization.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms156v6_use_of_high_risk_medications_in_the_elderly.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms156v6_use_of_high_risk_medications_in_the_elderly.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms182v6_ischemic_vascular_disease_complete_lipid_profile_and_ldl_c_control.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms182v6_ischemic_vascular_disease_complete_lipid_profile_and_ldl_c_control.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms2v7_preventive_care_and_screening_screening_for_depression_and_follow_up_plan.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms2v7_preventive_care_and_screening_screening_for_depression_and_follow_up_plan.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms50v6_closing_the_referral_loop_receipt_of_specialist_report.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms50v6_closing_the_referral_loop_receipt_of_specialist_report.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cms69v6_preventive_care_and_screening_body_mass_index_screening_and_follow_up_plan.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cms69v6_preventive_care_and_screening_body_mass_index_screening_and_follow_up_plan.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cqm_CMS127v6_pneumococcal.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cqm_CMS127v6_pneumococcal.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/cqm_CMS160v6_depression.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/cqm_CMS160v6_depression.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/future/quality_measure_document.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/future/quality_measure_document.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/hcc001v1_problem_list_hygiene.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/hcc001v1_problem_list_hygiene.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/hcc002v2_ckd_suspect.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/hcc002v2_ckd_suspect.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/hcc003v1_diabetes_mellitus_with_seconday_complication_suspect.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/hcc003v1_diabetes_mellitus_with_seconday_complication_suspect.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/hcc004v1_dysrhythmia_suspect.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/hcc004v1_dysrhythmia_suspect.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/hcc005v1_annual_wellness_visit.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/hcc005v1_annual_wellness_visit.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/helper_population.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/helper_population.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/hyperlink_recommendation.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/hyperlink_recommendation.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stub_template.py.txt` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stub_template.py.txt`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stub_template_user.py.txt` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stub_template_user.py.txt`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/_importlib_modulespec.data.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/_importlib_modulespec.data.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/_importlib_modulespec.meta.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/_importlib_modulespec.meta.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/abc.data.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/abc.data.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/abc.meta.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/abc.meta.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/builtins.data.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/builtins.data.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/builtins.meta.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms123v5_diabetes_foot_exam.data.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms123v5_diabetes_foot_exam.data.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms123v5_diabetes_foot_exam.meta.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms123v5_diabetes_foot_exam.meta.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms124v6_cervical_cancer_screening.data.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms124v6_cervical_cancer_screening.data.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms124v6_cervical_cancer_screening.meta.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/cms124v6_cervical_cancer_screening.meta.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/__init__.data.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/__init__.meta.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/abc.data.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/abc.meta.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/mypy_extensions.data.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/mypy_extensions.data.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/mypy_extensions.meta.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/mypy_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/sys.data.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/sys.data.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/sys.meta.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/sys.meta.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/types.data.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/types.data.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/types.meta.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/types.meta.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/typing.data.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/typing.data.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/typing.meta.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/.mypy_cache/3.6/typing.meta.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms117v9_childhood_immunization_status.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms117v9_childhood_immunization_status.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms122v9_diabetes_hemoglobin_a1c_poor_control.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms122v9_diabetes_hemoglobin_a1c_poor_control.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms124v9_cervical_cancer_screening.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms124v9_cervical_cancer_screening.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms125v9_breast_cancer_screening.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms125v9_breast_cancer_screening.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms127v9_pneumococcal_vaccination_status_for_older_adults.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms127v9_pneumococcal_vaccination_status_for_older_adults.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms128v9_anti_depressant_medication_management.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms128v9_anti_depressant_medication_management.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms129v10_prostate_cancer_avoidance_of_overuse_of_bone_scan_for_staging_low_risk_prostate_cancer_patients.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms129v10_prostate_cancer_avoidance_of_overuse_of_bone_scan_for_staging_low_risk_prostate_cancer_patients.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms130v9_colorectal_cancer_screening.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms130v9_colorectal_cancer_screening.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms131v9_diabetes_eye_exam.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms131v9_diabetes_eye_exam.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms133v9_cataracts_20_40_or_better_visual_acuity_within_90_days_following_cataract_surgery.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms133v9_cataracts_20_40_or_better_visual_acuity_within_90_days_following_cataract_surgery.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms134v9_diabetes_medical_attention_for_nephropathy.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms134v9_diabetes_medical_attention_for_nephropathy.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms135v9_heart_failure_angiotensin_converting_enzyme_inhibitor_or_angiotensin_receptor_blocker_or_angiotensin_receptor_neprilysin_inhibitor_therapy_for_left_ventricular_systolic_dysfunction.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms135v9_heart_failure_angiotensin_converting_enzyme_inhibitor_or_angiotensin_receptor_blocker_or_angiotensin_receptor_neprilysin_inhibitor_therapy_for_left_ventricular_systolic_dysfunction.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms136v10_follow_up_care_for_children_prescribed_adhd_medication.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms136v10_follow_up_care_for_children_prescribed_adhd_medication.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms137v9_initiation_and_engagement_of_alcohol_and_other_drug_dependence_treatment.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms137v9_initiation_and_engagement_of_alcohol_and_other_drug_dependence_treatment.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms138v9_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms138v9_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms139v9_falls_screening_for_future_fall_risk.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms139v9_falls_screening_for_future_fall_risk.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms142v9_diabetic_retinopathy_communication_with_the_physician_managing_ongoing_diabetes_care.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms142v9_diabetic_retinopathy_communication_with_the_physician_managing_ongoing_diabetes_care.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms143v9_primary_open_angle_glaucoma_optic_nerve_evaluation.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms143v9_primary_open_angle_glaucoma_optic_nerve_evaluation.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms144v9_heart_failure_beta_blocker_therapy_for_left_ventricular_systolic_dysfunction.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms144v9_heart_failure_beta_blocker_therapy_for_left_ventricular_systolic_dysfunction.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms145v9_coronary_artery_disease_beta_blocker_therapy_prior_myocardial_infarction_or_left_ventricular_systolic_dysfunction.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms145v9_coronary_artery_disease_beta_blocker_therapy_prior_myocardial_infarction_or_left_ventricular_systolic_dysfunction.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms146v9_appropriate_testing_for_pharyngitis.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms146v9_appropriate_testing_for_pharyngitis.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms147v10_preventive_care_and_screening_influenza_immunization.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms147v10_preventive_care_and_screening_influenza_immunization.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms149v9_dementia_cognitive_assessment.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms149v9_dementia_cognitive_assessment.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms153v9_chlamydia_screening_for_women.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms153v9_chlamydia_screening_for_women.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms154v9_appropriate_treatment_for_upper_respiratory_infection.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms154v9_appropriate_treatment_for_upper_respiratory_infection.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms155v9_weight_assessment_and_counseling_for_nutrition_and_physical_activity_for_children_and_adolescents.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms155v9_weight_assessment_and_counseling_for_nutrition_and_physical_activity_for_children_and_adolescents.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms156v9_use_of_high_risk_medications_in_older_adults.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms156v9_use_of_high_risk_medications_in_older_adults.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms157v9_oncology_medical_and_radiation_pain_intensity_quantified.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms157v9_oncology_medical_and_radiation_pain_intensity_quantified.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms159v9_depression_remission_at_twelve_months.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms159v9_depression_remission_at_twelve_months.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms161v9_adult_major_depressive_disorder_suicide_risk_assessment.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms161v9_adult_major_depressive_disorder_suicide_risk_assessment.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms165v9_controlling_high_blood_pressure.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms165v9_controlling_high_blood_pressure.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms177v9_child_and_adolescent_major_depressive_disorder_suicide_risk_assessment.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms177v9_child_and_adolescent_major_depressive_disorder_suicide_risk_assessment.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms22v9_preventive_care_and_screening_screening_for_high_blood_pressure_and_follow_up_documented.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms22v9_preventive_care_and_screening_screening_for_high_blood_pressure_and_follow_up_documented.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms249v3_appropriate_use_of_dxa_scans_in_women_under_65_years_who_do_not_meet_the_risk_factor_profile_for_osteoporotic_fracture.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms249v3_appropriate_use_of_dxa_scans_in_women_under_65_years_who_do_not_meet_the_risk_factor_profile_for_osteoporotic_fracture.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms2v10_preventive_care_and_screening_screening_for_depression_and_follow_up_plan.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms2v10_preventive_care_and_screening_screening_for_depression_and_follow_up_plan.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms347v4_statin_therapy_for_the_prevention_and_treatment_of_cardiovascular_disease.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms347v4_statin_therapy_for_the_prevention_and_treatment_of_cardiovascular_disease.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms349v3_hiv_screening.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms349v3_hiv_screening.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms50v9_closing_the_referral_loop_receipt_of_specialist_report.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms50v9_closing_the_referral_loop_receipt_of_specialist_report.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms56v9_functional_status_assessment_for_total_hip_replacement.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms56v9_functional_status_assessment_for_total_hip_replacement.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms645v4_bone_density_evaluation_for_patients_with_prostate_cancer_and_receiving_androgen_deprivation_therapy.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms645v4_bone_density_evaluation_for_patients_with_prostate_cancer_and_receiving_androgen_deprivation_therapy.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms66v9_functional_status_assessment_for_total_knee_replacement.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms66v9_functional_status_assessment_for_total_knee_replacement.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms68v10_documentation_of_current_medications_in_the_medical_record.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms68v10_documentation_of_current_medications_in_the_medical_record.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms69v9_preventive_care_and_screening_body_mass_index_screening_and_follow_up_plan.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms69v9_preventive_care_and_screening_body_mass_index_screening_and_follow_up_plan.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms74v10_primary_caries_prevention_intervention_as_offered_by_primary_care_providers,_including_dentists.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms74v10_primary_caries_prevention_intervention_as_offered_by_primary_care_providers,_including_dentists.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms75v9_children_who_have_dental_decay_or_cavities.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms75v9_children_who_have_dental_decay_or_cavities.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms771v2_urinary_symptom_score_change_6_12_months_after_diagnosis_of_benign_prostatic_hyperplasia.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms771v2_urinary_symptom_score_change_6_12_months_after_diagnosis_of_benign_prostatic_hyperplasia.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/stubs/cms90v10_functional_status_assessments_for_congestive_heart_failure.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/stubs/cms90v10_functional_status_assessments_for_congestive_heart_failure.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/interviews.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yesnotest/interviews.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/lab_reports.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms122v6_diabetes_yeswithtest/lab_reports.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/interviews.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms123v6_diabetes_yesdone/interviews.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/referral_reports.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms131v6_diabetes_yeswithreferralreport/referral_reports.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/cms134v6_diabetes_yes/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/instructions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/instructions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/interviews.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/interviews.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/medications.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/feet1/medications.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc001v1/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/mock_data/hcc002v2_diagnosed/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_ccp001v1_symptomatic_surveillance.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_ccp001v1_symptomatic_surveillance.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_ccp002v1_high_risk_outreach.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_ccp002v1_high_risk_outreach.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_ccp003v1_hypertension.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_ccp003v1_hypertension.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_ccp004v1_diabetes.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_ccp004v1_diabetes.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_ccp005v1_asthma.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_ccp005v1_asthma.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms122v6_diabetes_hemoglobin_a1c_poor_control.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms122v6_diabetes_hemoglobin_a1c_poor_control.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms123v6_diabetes_foot_exam.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms123v6_diabetes_foot_exam.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms125v6_breast_cancer_screening.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms125v6_breast_cancer_screening.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms130v6_colorectal_cancer_screening.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms130v6_colorectal_cancer_screening.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms131v6_diabetes_eye_exam.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms131v6_diabetes_eye_exam.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms134v6_diabetes_medical_attention_for_nephropathy.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms134v6_diabetes_medical_attention_for_nephropathy.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms138v6_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms138v6_preventive_care_and_screening_tobacco_use_screening_and_cessation_intervention.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms138v6p1.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms138v6p1.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_cms138v6p2.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_cms138v6p2.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_diabetes_quality_measure.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_diabetes_quality_measure.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_hcc001v1_problem_list_hygiene.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_hcc001v1_problem_list_hygiene.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_hcc002v2_ckd_suspect.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_hcc002v2_ckd_suspect.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_hcc003v1_diabetes_mellitus_with_seconday_complication_suspect.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_hcc003v1_diabetes_mellitus_with_seconday_complication_suspect.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_hcc004v1_dysrhythmia_suspect.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_hcc004v1_dysrhythmia_suspect.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_hcc005v1_annual_wellness_visit.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_hcc005v1_annual_wellness_visit.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/builtin_cqms/tests/test_helper_population.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/builtin_cqms/tests/test_helper_population.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/canvas_cli.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/canvas_cli.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/canvas_code_set.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/canvas_code_set.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/constants.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from enum import Enum
 
 COMMAND_TYPE_ALLERGY = 'allergy'
+COMMAND_TYPE_ASSESS = 'assess'
 COMMAND_TYPE_DIAGNOSE = 'diagnose'
 COMMAND_TYPE_FOLLOWUP = 'followUp'
 COMMAND_TYPE_IMAGING = 'imagingOrder'
 COMMAND_TYPE_IMMUNIZATION = 'immunization'
 COMMAND_TYPE_INSTRUCTION = 'instruct'
 COMMAND_TYPE_INTERVIEW = 'interview'
 COMMAND_TYPE_LAB_ORDER = 'labOrder'
```

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/events.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/events.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/generate_cqms_stubs.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/generate_cqms_stubs.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/internal/attrdict.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/internal/attrdict.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/internal/integration_messages.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/internal/integration_messages.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/internal/string.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/internal/string.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/intervention.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/intervention.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/metaclass.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/metaclass.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/patient.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/patient.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/patient_recordset.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/patient_recordset.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/protocol.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/protocol.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/recommendation.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/recommendation.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 """
 
 from typing import List, Optional, Type, Dict
 
 from .constants import (
     COMMAND_TYPE_ALLERGY,
+    COMMAND_TYPE_ASSESS,
     COMMAND_TYPE_DIAGNOSE,
     COMMAND_TYPE_FOLLOWUP,
     COMMAND_TYPE_IMAGING,
     COMMAND_TYPE_IMMUNIZATION,
     COMMAND_TYPE_INSTRUCTION,
     COMMAND_TYPE_INTERVIEW,
     COMMAND_TYPE_LAB_ORDER,
@@ -117,14 +118,27 @@
 
         command = self.command_filter(COMMAND_TYPE_ALLERGY, [allergy])
 
         super().__init__(
             key, rank, button, title=title, narrative=narrative, command=command, context=context
         )
 
+class AssessRecommendation(Recommendation):
+    """
+    A recommendation specifying an assessment of the patient's condition.
+    """
+
+    def __init__(self, key, patient: Patient, rank=RANK_MAX, button='Assess', title=None, context=None):
+        command = {'type': COMMAND_TYPE_ASSESS}
+
+        if not title:
+            title = 'Assess condition'
+
+        super().__init__(key, rank, button, title, command=command, context=context)
+
 
 class DiagnoseRecommendation(Recommendation):
     """
     A recommendation specifying a condition to diagnose the patient.
     """
 
     def __init__(
```

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/settings.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/settings.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/base.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/base.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/get_protocols_unittest/protocol_unittest.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/get_protocols_unittest/protocol_unittest.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/empty.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/empty.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/appointments.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/appointments.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/consents.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/consents.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/imaging_reports.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/imaging_reports.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/interviews.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/interviews.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/lab_orders.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/lab_orders.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/lab_reports.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/lab_reports.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/medications.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/medications.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/prescriptions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/prescriptions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/protocol_overrides.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/protocol_overrides.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/referrals.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/referrals.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full/tasks.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full/tasks.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/full.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/full.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/appointments.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/appointments.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/mock_data/partial/consents.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/mock_data/partial/consents.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1/vital_signs.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1/vital_signs.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/instructions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/instructions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/vital_signs.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi1_with_instruction/vital_signs.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/bmi2/vital_signs.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/bmi2/vital_signs.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/immunizations.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/immunizations.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/interviews.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/interviews.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/medications.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/medications.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/patient.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/patient.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression1/vital_signs.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression1/vital_signs.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/immunizations.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/immunizations.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/instructions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/instructions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/interviews.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/interviews.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/medications.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/medications.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/patient.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/patient.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/depression2/vital_signs.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/depression2/vital_signs.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/lab_reports.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic2/lab_reports.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/lab_reports.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic3/lab_reports.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/lab_reports.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/diabetic4/lab_reports.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/example/lab_reports.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/example/lab_reports.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/example/medications.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/example/medications.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/example/patient.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/example/patient.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fall1/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fall1/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fall1/medications.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fall1/medications.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fall1/patient.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fall1/patient.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/feet1/interviews.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/feet1/interviews.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/feet1/medications.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/feet1/medications.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fluvax/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fluvax/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/fluvax/immunizations.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/fluvax/immunizations.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/#medications.json#` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/#medications.json#`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/medications.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/medications.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/patient.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/highrisk1/patient.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/interviews.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/interviews.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/patient.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/nonsmoker/patient.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/referral/conditions.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/referral/conditions.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/referral/patient.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/referral/patient.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/mock_data/referral/referrals.json` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/mock_data/referral/referrals.json`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_interviews.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_interviews.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_labs.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_labs.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_medications.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_medications.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_protocols.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_protocols.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_recommendations.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_recommendations.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_value_sets.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_value_sets.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/sdk/test_vitalsigns.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/sdk/test_vitalsigns.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_action.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_canvas_code_set.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_canvas_code_set.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_intervention.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_intervention.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_patient.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_patient.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_patient_recordset.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_patient_recordset.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_protocol.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_recommendation.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_recommendation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from canvas_workflow_kit.intervention import Intervention
 from canvas_workflow_kit.patient import Patient
 from canvas_workflow_kit.recommendation import (
     AllergyRecommendation,
+    AssessRecommendation,
     DiagnoseRecommendation,
     FollowUpRecommendation,
     HyperlinkRecommendation,
     ImagingRecommendation,
     ImmunizationRecommendation,
     InstructionRecommendation,
     InterviewRecommendation,
@@ -534,14 +535,31 @@
         self.assertIsInstance(rec, Intervention)
         self.assertEqual(rec.key, 'KEY!')
         self.assertEqual(rec.title, 'Something needs to be done')
         self.assertEqual(rec.rank, 4)
         self.assertEqual(rec.button, 'Try this')
         self.assertEqual(rec.href, 'https://www.google.com/search?q=broccoli')
 
+class AssessRecommendationTest(SDKBaseTest):
+
+    def test___init__(self):
+        patient = self.load_patient('full')
+        self.assertIsInstance(patient, Patient)
+
+        rec = AssessRecommendation(key='KEY-ID', rank=123,
+                                   patient=patient, context={'background': 'FooBar'})
+
+        self.assertIsInstance(rec, Recommendation)
+        self.assertEqual(rec.key, 'KEY-ID')
+        self.assertEqual(rec.rank, 123)
+        self.assertEqual(rec.button, 'Assess')
+        self.assertEqual(rec.title, 'Assess condition')
+        self.assertEqual({'type': 'assess'}, rec.command)
+        self.assertEqual(rec.context['background'], 'FooBar')
+
 
 # --- helpers ---
 class HelperCommand(SDKBaseTest):
 
     def equal_commands(self, expected: dict, result: dict):
         self.assertTrue(('type' in result) and (result['type'] == expected['type']))
         self.assertTrue(('filter' in result) and ('coding' in result['filter']))
```

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_template.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/test_timeframe.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/test_timeframe.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/hcc_file.txt` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/hcc_file.txt`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/hcc_labels.txt` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/hcc_labels.txt`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/hcc_methods.txt` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/hcc_methods.txt`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/hcc_sample.tsv` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/hcc_sample.tsv`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/test_hcc2018.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/test_hcc2018.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/test_specials.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/test_specials.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/test_value_set.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/test_value_set.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/tests/value_set/test_value_sets.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/tests/value_set/test_value_sets.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/timeframe.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/timeframe.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/utils.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/utils.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/customer_value_sets/scan.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/customer_value_sets/scan.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/hcc2018.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/hcc2018.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/medication_class_path2018.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/medication_class_path2018.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/specials.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/specials.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2017.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2017.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2018.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2018.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2019.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2019.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2020.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2020.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/allergy.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/allergy.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/assessment.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/assessment.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/assessment_performed.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/assessment_performed.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/communication.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/communication.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/device.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/device.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/diagnosis.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/diagnosis.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/encounter.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/encounter.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/encounter_performed.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/encounter_performed.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/immunization.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/immunization.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/lab_test.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/lab_test.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/medication.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/medication.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/other.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/other.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/patient_characteristic.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/patient_characteristic.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/physical_exam.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/physical_exam.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/procedure.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/procedure.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/procedure_performed.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/procedure_performed.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/rationale.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/rationale.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2021/result.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2021/result.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/adverse_event.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/adverse_event.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/allergy.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/allergy.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/assessment.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/assessment.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/communication.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/communication.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/condition.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/condition.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/device.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/device.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/diagnostic_study.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/diagnostic_study.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/encounter.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/encounter.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/immunization.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/immunization.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/individual_characteristic.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/individual_characteristic.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/intervention.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/intervention.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/laboratory_test.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/laboratory_test.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/medication.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/medication.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/physical_exam.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/physical_exam.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/procedure.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/procedure.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/v2022/symptom.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/v2022/symptom.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/canvas_workflow_kit/value_set/value_set.py` & `canvas-workflow-kit-0.6.4/canvas_workflow_kit/value_set/value_set.py`

 * *Files identical despite different names*

### Comparing `canvas-workflow-kit-0.6.3/pyproject.toml` & `canvas-workflow-kit-0.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "canvas-workflow-kit"
-version = "0.6.3"
+version = "0.6.4"
 description = "Development kit to empower customization of your Canvas instance"
 authors = ["Canvas Team <engineering@canvasmedical.com>"]
 exclude = ["canvas_workflow_kit/schemas", "canvas_workflow_kit/scripts"]
 
 # Be cautious adding dependencies. These also will get installed to home-app.
 # Dependencies should be loosely versioned to not cause conflicts when installed to home-app.
 
 [tool.poetry.dependencies]
 python = "^3.7"
-arrow = "^1.*"
+arrow = "1.*"
 cached-property = "1.5.*"
 requests = "2.*"
 memoization = "0.4.*"
 python-decouple = "3.*"
 click = "*"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `canvas-workflow-kit-0.6.3/setup.py` & `canvas-workflow-kit-0.6.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,27 +67,27 @@
                                    'mock_data/feet1/*',
                                    'mock_data/fluvax/*',
                                    'mock_data/highrisk1/*',
                                    'mock_data/nonsmoker/*',
                                    'mock_data/referral/*']}
 
 install_requires = \
-['arrow',
+['arrow>=1.0.0,<2.0.0',
  'cached-property>=1.5.0,<1.6.0',
  'click',
  'memoization>=0.4.0,<0.5.0',
  'python-decouple>=3.0.0,<4.0.0',
  'requests>=2.0.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['canvas-cli = canvas_workflow_kit.canvas_cli:cli']}
 
 setup_kwargs = {
     'name': 'canvas-workflow-kit',
-    'version': '0.6.3',
+    'version': '0.6.4',
     'description': 'Development kit to empower customization of your Canvas instance',
     'long_description': None,
     'author': 'Canvas Team',
     'author_email': 'engineering@canvasmedical.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `canvas-workflow-kit-0.6.3/PKG-INFO` & `canvas-workflow-kit-0.6.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: canvas-workflow-kit
-Version: 0.6.3
+Version: 0.6.4
 Summary: Development kit to empower customization of your Canvas instance
 Author: Canvas Team
 Author-email: engineering@canvasmedical.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: arrow
+Requires-Dist: arrow (>=1.0.0,<2.0.0)
 Requires-Dist: cached-property (>=1.5.0,<1.6.0)
 Requires-Dist: click
 Requires-Dist: memoization (>=0.4.0,<0.5.0)
 Requires-Dist: python-decouple (>=3.0.0,<4.0.0)
 Requires-Dist: requests (>=2.0.0,<3.0.0)
```

