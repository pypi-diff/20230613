# Comparing `tmp/fhirkit-0.1.0.tar.gz` & `tmp/FHIRkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fhirkit-0.1.0.tar", max compression
+gzip compressed data, was "FHIRkit-0.1.1.tar", last modified: Tue Jun 13 08:27:43 2023, max compression
```

## Comparing `fhirkit-0.1.0.tar` & `FHIRkit-0.1.1.tar`

### file list

```diff
@@ -1,61 +1,80 @@
--rw-r--r--   0        0        0     1094 2022-04-22 12:04:21.381197 fhirkit-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     2029 2022-07-05 12:32:50.506000 fhirkit-0.1.0/README.md
--rw-r--r--   0        0        0      519 2022-12-22 10:36:31.966808 fhirkit-0.1.0/fhirkit/AllergyIntolerance.py
--rw-r--r--   0        0        0     4080 2023-05-07 18:20:08.553342 fhirkit-0.1.0/fhirkit/BaseModel.py
--rw-r--r--   0        0        0     1774 2022-12-22 10:36:31.967024 fhirkit-0.1.0/fhirkit/Bundle.py
--rw-r--r--   0        0        0      291 2022-10-16 13:55:20.803787 fhirkit-0.1.0/fhirkit/CarePlan.py
--rw-r--r--   0        0        0      275 2022-07-05 13:42:03.317401 fhirkit-0.1.0/fhirkit/CareTeam.py
--rw-r--r--   0        0        0     1806 2023-01-20 16:56:35.262451 fhirkit-0.1.0/fhirkit/ClinicalImpression.py
--rw-r--r--   0        0        0     5490 2023-05-23 08:05:55.237472 fhirkit-0.1.0/fhirkit/CodeSystem.py
--rw-r--r--   0        0        0     2722 2023-02-16 13:55:38.147678 fhirkit-0.1.0/fhirkit/Composition.py
--rw-r--r--   0        0        0      381 2022-04-22 12:04:21.383580 fhirkit-0.1.0/fhirkit/CompositionValueSet.py
--rw-r--r--   0        0        0     5527 2023-05-07 18:20:08.553910 fhirkit-0.1.0/fhirkit/Condition.py
--rw-r--r--   0        0        0     1020 2023-05-07 18:20:08.554044 fhirkit-0.1.0/fhirkit/Coverage.py
--rw-r--r--   0        0        0      269 2023-05-23 07:50:16.138796 fhirkit-0.1.0/fhirkit/Device.py
--rw-r--r--   0        0        0     1614 2023-01-20 16:56:35.263808 fhirkit-0.1.0/fhirkit/DiagnosticReport.py
--rw-r--r--   0        0        0      302 2022-07-05 13:42:22.509774 fhirkit-0.1.0/fhirkit/DocumentReference.py
--rw-r--r--   0        0        0     8049 2023-05-07 18:20:08.554838 fhirkit-0.1.0/fhirkit/Encounter.py
--rw-r--r--   0        0        0      287 2022-07-05 13:42:38.175881 fhirkit-0.1.0/fhirkit/ImagingStudy.py
--rw-r--r--   0        0        0      287 2022-07-05 13:42:42.441413 fhirkit-0.1.0/fhirkit/Immunization.py
--rw-r--r--   0        0        0     1591 2022-12-22 10:33:00.422460 fhirkit-0.1.0/fhirkit/Location.py
--rw-r--r--   0        0        0      281 2022-07-05 13:42:51.346675 fhirkit-0.1.0/fhirkit/Medication.py
--rw-r--r--   0        0        0      337 2022-07-05 13:42:55.435328 fhirkit-0.1.0/fhirkit/MedicationAdministration.py
--rw-r--r--   0        0        0      302 2022-07-05 13:42:58.629005 fhirkit-0.1.0/fhirkit/MedicationRequest.py
--rw-r--r--   0        0        0      322 2022-07-05 13:49:07.575913 fhirkit-0.1.0/fhirkit/MedicationStatement.py
--rw-r--r--   0        0        0     3658 2023-02-16 13:55:38.147863 fhirkit-0.1.0/fhirkit/Observation.py
--rw-r--r--   0        0        0     1286 2022-07-19 14:55:47.271304 fhirkit-0.1.0/fhirkit/OperationOutcome.py
--rw-r--r--   0        0        0     2440 2023-05-22 13:04:33.766917 fhirkit-0.1.0/fhirkit/Organization.py
--rw-r--r--   0        0        0     2120 2022-07-20 15:15:13.788912 fhirkit-0.1.0/fhirkit/Parameter.py
--rw-r--r--   0        0        0     3496 2023-05-07 18:20:08.555303 fhirkit-0.1.0/fhirkit/Patient.py
--rw-r--r--   0        0        0     2547 2023-05-07 18:20:08.556092 fhirkit-0.1.0/fhirkit/Practitioner.py
--rw-r--r--   0        0        0     3791 2023-05-07 18:20:08.556969 fhirkit-0.1.0/fhirkit/PractitionerRole.py
--rw-r--r--   0        0        0     5966 2023-05-07 18:20:08.557179 fhirkit-0.1.0/fhirkit/Procedure.py
--rw-r--r--   0        0        0      281 2022-08-14 11:45:44.118911 fhirkit-0.1.0/fhirkit/Provenance.py
--rw-r--r--   0        0        0     2943 2023-05-08 07:04:17.842502 fhirkit-0.1.0/fhirkit/Resource.py
--rw-r--r--   0        0        0     2828 2023-02-16 13:55:38.169585 fhirkit-0.1.0/fhirkit/Server.py
--rw-r--r--   0        0        0    10578 2023-02-16 13:56:16.230095 fhirkit-0.1.0/fhirkit/SimpleFHIRStore.py
--rw-r--r--   0        0        0      293 2022-08-14 11:50:43.251431 fhirkit-0.1.0/fhirkit/SupplyDelivery.py
--rw-r--r--   0        0        0      650 2022-12-22 10:36:31.970229 fhirkit-0.1.0/fhirkit/TerminologyServer.py
--rw-r--r--   0        0        0     6228 2023-05-22 14:12:40.854533 fhirkit-0.1.0/fhirkit/ValueSet.py
--rw-r--r--   0        0        0     1842 2023-05-07 18:20:08.558497 fhirkit-0.1.0/fhirkit/__init__.py
--rw-r--r--   0        0        0       83 2022-07-20 15:52:50.507783 fhirkit-0.1.0/fhirkit/choice_type/__init__.py
--rw-r--r--   0        0        0     5630 2022-07-20 15:57:33.924942 fhirkit-0.1.0/fhirkit/choice_type/choice_type.py
--rw-r--r--   0        0        0     1207 2022-12-22 10:36:31.971529 fhirkit-0.1.0/fhirkit/choice_type/validators.py
--rw-r--r--   0        0        0     1583 2022-07-23 07:15:14.050513 fhirkit-0.1.0/fhirkit/elements/Timing.py
--rw-r--r--   0        0        0      926 2022-07-23 07:01:36.217241 fhirkit-0.1.0/fhirkit/elements/UsageContext.py
--rw-r--r--   0        0        0       90 2022-07-19 16:29:33.220298 fhirkit-0.1.0/fhirkit/elements/__init__.py
--rw-r--r--   0        0        0    10875 2023-05-22 13:04:33.771342 fhirkit-0.1.0/fhirkit/elements/elements.py
--rw-r--r--   0        0        0     1075 2023-05-07 18:20:08.559365 fhirkit-0.1.0/fhirkit/metadata_types.py
--rw-r--r--   0        0        0      495 2022-12-22 10:36:31.972058 fhirkit-0.1.0/fhirkit/parse.py
--rw-r--r--   0        0        0     7228 2023-05-08 07:27:12.193111 fhirkit-0.1.0/fhirkit/primitive_datatypes.py
--rw-r--r--   0        0        0  3105532 2023-06-09 18:12:56.788995 fhirkit-0.1.0/fhirkit/r5.py
--rw-r--r--   0        0        0       62 2022-04-22 12:04:21.386086 fhirkit-0.1.0/fhirkit/setup.cfg
--rw-r--r--   0        0        0     4697 2023-02-16 13:55:38.170341 fhirkit-0.1.0/fhirkit/snomed/ValueSet.py
--rw-r--r--   0        0        0      125 2022-04-22 12:04:21.386293 fhirkit-0.1.0/fhirkit/snomed/__init__.py
--rw-r--r--   0        0        0       35 2022-04-22 12:04:21.386364 fhirkit-0.1.0/fhirkit/snomed/consts.py
--rw-r--r--   0        0        0     1648 2022-07-20 09:32:25.820588 fhirkit-0.1.0/fhirkit/snomed/elements.py
--rw-r--r--   0        0        0     8174 2023-02-16 13:55:38.170504 fhirkit-0.1.0/fhirkit/snomed/terminology.py
--rw-r--r--   0        0        0       34 2023-01-20 16:56:35.265286 fhirkit-0.1.0/fhirkit/tiro/__init__.py
--rw-r--r--   0        0        0      583 2023-01-20 16:56:35.265401 fhirkit-0.1.0/fhirkit/tiro/elements.py
--rw-r--r--   0        0        0      336 2023-06-09 18:19:46.713411 fhirkit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 fhirkit-0.1.0/PKG-INFO
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.160193 FHIRkit-0.1.1/
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.131153 FHIRkit-0.1.1/FHIRkit.egg-info/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2476 2023-06-13 08:27:43.000000 FHIRkit-0.1.1/FHIRkit.egg-info/PKG-INFO
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1696 2023-06-13 08:27:43.000000 FHIRkit-0.1.1/FHIRkit.egg-info/SOURCES.txt
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)        1 2023-06-13 08:27:43.000000 FHIRkit-0.1.1/FHIRkit.egg-info/dependency_links.txt
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       23 2023-06-13 08:27:43.000000 FHIRkit-0.1.1/FHIRkit.egg-info/requires.txt
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       13 2023-06-13 08:27:43.000000 FHIRkit-0.1.1/FHIRkit.egg-info/top_level.txt
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1094 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/LICENSE.md
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2476 2023-06-13 08:27:43.159877 FHIRkit-0.1.1/PKG-INFO
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2029 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/README.md
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.149657 FHIRkit-0.1.1/fhirkit/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      519 2022-12-22 10:38:55.000000 FHIRkit-0.1.1/fhirkit/AllergyIntolerance.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     4080 2023-04-10 09:45:08.000000 FHIRkit-0.1.1/fhirkit/BaseModel.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1774 2022-12-22 10:38:55.000000 FHIRkit-0.1.1/fhirkit/Bundle.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      291 2023-06-13 07:52:05.000000 FHIRkit-0.1.1/fhirkit/CarePlan.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      275 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/CareTeam.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1806 2023-01-15 15:30:45.000000 FHIRkit-0.1.1/fhirkit/ClinicalImpression.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     5490 2023-06-13 07:52:07.000000 FHIRkit-0.1.1/fhirkit/CodeSystem.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2722 2023-01-27 09:58:51.000000 FHIRkit-0.1.1/fhirkit/Composition.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      381 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/CompositionValueSet.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     5527 2023-02-17 17:20:01.000000 FHIRkit-0.1.1/fhirkit/Condition.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1020 2023-04-27 13:46:13.000000 FHIRkit-0.1.1/fhirkit/Coverage.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      269 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/Device.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1614 2023-01-13 16:13:41.000000 FHIRkit-0.1.1/fhirkit/DiagnosticReport.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      302 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/DocumentReference.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     8049 2023-02-17 17:20:01.000000 FHIRkit-0.1.1/fhirkit/Encounter.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      287 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/ImagingStudy.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      287 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/Immunization.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1591 2022-10-20 12:40:00.000000 FHIRkit-0.1.1/fhirkit/Location.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      281 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/Medication.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      337 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/MedicationAdministration.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      302 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/MedicationRequest.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      322 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/MedicationStatement.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     3658 2023-06-13 07:52:05.000000 FHIRkit-0.1.1/fhirkit/Observation.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1286 2022-10-24 13:24:49.000000 FHIRkit-0.1.1/fhirkit/OperationOutcome.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2440 2023-05-22 08:57:29.000000 FHIRkit-0.1.1/fhirkit/Organization.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2120 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/Parameter.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     3496 2023-04-13 07:10:47.000000 FHIRkit-0.1.1/fhirkit/Patient.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2547 2023-02-17 17:20:01.000000 FHIRkit-0.1.1/fhirkit/Practitioner.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     3791 2023-02-17 17:20:01.000000 FHIRkit-0.1.1/fhirkit/PractitionerRole.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     5966 2023-04-10 09:33:00.000000 FHIRkit-0.1.1/fhirkit/Procedure.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      281 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/Provenance.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2943 2023-05-22 08:59:19.000000 FHIRkit-0.1.1/fhirkit/Resource.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2828 2023-02-17 17:19:01.000000 FHIRkit-0.1.1/fhirkit/Server.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)    10578 2023-04-13 07:11:11.000000 FHIRkit-0.1.1/fhirkit/SimpleFHIRStore.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      293 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/SupplyDelivery.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      650 2022-12-22 10:38:55.000000 FHIRkit-0.1.1/fhirkit/TerminologyServer.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     6228 2023-06-13 07:52:07.000000 FHIRkit-0.1.1/fhirkit/ValueSet.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1842 2023-06-13 07:52:05.000000 FHIRkit-0.1.1/fhirkit/__init__.py
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.154351 FHIRkit-0.1.1/fhirkit/choice_type/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       83 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/choice_type/__init__.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     5630 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/choice_type/choice_type.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1207 2022-12-22 10:38:55.000000 FHIRkit-0.1.1/fhirkit/choice_type/validators.py
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.155946 FHIRkit-0.1.1/fhirkit/elements/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1583 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/elements/Timing.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      926 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/elements/UsageContext.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       90 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/elements/__init__.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)    10875 2023-06-13 07:52:07.000000 FHIRkit-0.1.1/fhirkit/elements/elements.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1075 2023-02-17 17:20:01.000000 FHIRkit-0.1.1/fhirkit/metadata_types.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      495 2022-12-22 10:38:55.000000 FHIRkit-0.1.1/fhirkit/parse.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     7228 2023-05-22 08:59:19.000000 FHIRkit-0.1.1/fhirkit/primitive_datatypes.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)  2467556 2023-06-13 08:03:49.000000 FHIRkit-0.1.1/fhirkit/r4.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)  3105532 2023-06-13 07:52:07.000000 FHIRkit-0.1.1/fhirkit/r5.py
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.157372 FHIRkit-0.1.1/fhirkit/snomed/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     4697 2023-02-17 17:19:01.000000 FHIRkit-0.1.1/fhirkit/snomed/ValueSet.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      125 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/snomed/__init__.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       35 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/snomed/consts.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1648 2023-01-13 08:53:58.000000 FHIRkit-0.1.1/fhirkit/snomed/elements.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     8174 2023-02-17 17:19:01.000000 FHIRkit-0.1.1/fhirkit/snomed/terminology.py
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.158329 FHIRkit-0.1.1/fhirkit/tiro/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       34 2023-01-13 08:55:47.000000 FHIRkit-0.1.1/fhirkit/tiro/__init__.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      583 2023-01-20 15:20:02.000000 FHIRkit-0.1.1/fhirkit/tiro/elements.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      336 2023-06-13 07:52:07.000000 FHIRkit-0.1.1/pyproject.toml
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       38 2023-06-13 08:27:43.160268 FHIRkit-0.1.1/setup.cfg
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      664 2023-06-13 08:27:32.000000 FHIRkit-0.1.1/setup.py
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.159403 FHIRkit-0.1.1/test/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)        0 2023-02-17 17:19:01.000000 FHIRkit-0.1.1/test/__init__.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      262 2023-02-20 09:07:12.000000 FHIRkit-0.1.1/test/test_meta.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      455 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/test/test_observation.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      483 2022-12-22 10:38:55.000000 FHIRkit-0.1.1/test/test_reference.py
```

### Comparing `fhirkit-0.1.0/LICENSE.md` & `FHIRkit-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/README.md` & `FHIRkit-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/AllergyIntolerance.py` & `FHIRkit-0.1.1/fhirkit/AllergyIntolerance.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/BaseModel.py` & `FHIRkit-0.1.1/fhirkit/BaseModel.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Bundle.py` & `FHIRkit-0.1.1/fhirkit/Bundle.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/ClinicalImpression.py` & `FHIRkit-0.1.1/fhirkit/ClinicalImpression.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/CodeSystem.py` & `FHIRkit-0.1.1/fhirkit/CodeSystem.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Composition.py` & `FHIRkit-0.1.1/fhirkit/Composition.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Condition.py` & `FHIRkit-0.1.1/fhirkit/Condition.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Coverage.py` & `FHIRkit-0.1.1/fhirkit/Coverage.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/DiagnosticReport.py` & `FHIRkit-0.1.1/fhirkit/DiagnosticReport.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Encounter.py` & `FHIRkit-0.1.1/fhirkit/Encounter.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Location.py` & `FHIRkit-0.1.1/fhirkit/Location.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Observation.py` & `FHIRkit-0.1.1/fhirkit/Observation.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/OperationOutcome.py` & `FHIRkit-0.1.1/fhirkit/OperationOutcome.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Organization.py` & `FHIRkit-0.1.1/fhirkit/Organization.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Parameter.py` & `FHIRkit-0.1.1/fhirkit/Parameter.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Patient.py` & `FHIRkit-0.1.1/fhirkit/Patient.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Practitioner.py` & `FHIRkit-0.1.1/fhirkit/Practitioner.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/PractitionerRole.py` & `FHIRkit-0.1.1/fhirkit/PractitionerRole.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Procedure.py` & `FHIRkit-0.1.1/fhirkit/Procedure.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Resource.py` & `FHIRkit-0.1.1/fhirkit/Resource.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/Server.py` & `FHIRkit-0.1.1/fhirkit/Server.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/SimpleFHIRStore.py` & `FHIRkit-0.1.1/fhirkit/SimpleFHIRStore.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/TerminologyServer.py` & `FHIRkit-0.1.1/fhirkit/TerminologyServer.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/ValueSet.py` & `FHIRkit-0.1.1/fhirkit/ValueSet.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/__init__.py` & `FHIRkit-0.1.1/fhirkit/__init__.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/choice_type/choice_type.py` & `FHIRkit-0.1.1/fhirkit/choice_type/choice_type.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/choice_type/validators.py` & `FHIRkit-0.1.1/fhirkit/choice_type/validators.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/elements/Timing.py` & `FHIRkit-0.1.1/fhirkit/elements/Timing.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/elements/UsageContext.py` & `FHIRkit-0.1.1/fhirkit/elements/UsageContext.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/elements/elements.py` & `FHIRkit-0.1.1/fhirkit/elements/elements.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/metadata_types.py` & `FHIRkit-0.1.1/fhirkit/metadata_types.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/primitive_datatypes.py` & `FHIRkit-0.1.1/fhirkit/primitive_datatypes.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/r5.py` & `FHIRkit-0.1.1/fhirkit/r5.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/snomed/ValueSet.py` & `FHIRkit-0.1.1/fhirkit/snomed/ValueSet.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/snomed/elements.py` & `FHIRkit-0.1.1/fhirkit/snomed/elements.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/snomed/terminology.py` & `FHIRkit-0.1.1/fhirkit/snomed/terminology.py`

 * *Files identical despite different names*

### Comparing `fhirkit-0.1.0/fhirkit/tiro/elements.py` & `FHIRkit-0.1.1/fhirkit/tiro/elements.py`

 * *Files identical despite different names*

