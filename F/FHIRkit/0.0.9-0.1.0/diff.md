# Comparing `tmp/FHIRkit-0.0.9.tar.gz` & `tmp/fhirkit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FHIRkit-0.0.9.tar", last modified: Sun May  1 06:52:01 2022, max compression
+gzip compressed data, was "fhirkit-0.1.0.tar", max compression
```

## Comparing `FHIRkit-0.0.9.tar` & `fhirkit-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,61 @@
-drwxr-xr-x   0 axelvanraes   (501) staff       (20)        0 2022-05-01 06:52:01.336513 FHIRkit-0.0.9/
-drwxr-xr-x   0 axelvanraes   (501) staff       (20)        0 2022-05-01 06:52:01.332555 FHIRkit-0.0.9/FHIRkit.egg-info/
--rw-r--r--   0 axelvanraes   (501) staff       (20)      538 2022-05-01 06:52:01.000000 FHIRkit-0.0.9/FHIRkit.egg-info/PKG-INFO
--rw-r--r--   0 axelvanraes   (501) staff       (20)      699 2022-05-01 06:52:01.000000 FHIRkit-0.0.9/FHIRkit.egg-info/SOURCES.txt
--rw-r--r--   0 axelvanraes   (501) staff       (20)        1 2022-05-01 06:52:01.000000 FHIRkit-0.0.9/FHIRkit.egg-info/dependency_links.txt
--rw-r--r--   0 axelvanraes   (501) staff       (20)       18 2022-05-01 06:52:01.000000 FHIRkit-0.0.9/FHIRkit.egg-info/requires.txt
--rw-r--r--   0 axelvanraes   (501) staff       (20)        8 2022-05-01 06:52:01.000000 FHIRkit-0.0.9/FHIRkit.egg-info/top_level.txt
--rw-r--r--   0 axelvanraes   (501) staff       (20)     1094 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/LICENSE.md
--rw-r--r--   0 axelvanraes   (501) staff       (20)      538 2022-05-01 06:52:01.336158 FHIRkit-0.0.9/PKG-INFO
--rw-r--r--   0 axelvanraes   (501) staff       (20)       71 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/README.md
-drwxr-xr-x   0 axelvanraes   (501) staff       (20)        0 2022-05-01 06:52:01.335141 FHIRkit-0.0.9/fhirkit/
--rw-r--r--   0 axelvanraes   (501) staff       (20)     1318 2022-05-01 06:22:32.000000 FHIRkit-0.0.9/fhirkit/Bundle.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     5440 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/ChoiceTypeMixin.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     5944 2022-05-01 06:51:03.000000 FHIRkit-0.0.9/fhirkit/CodeSystem.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)      381 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/CompositionValueSet.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     2620 2022-05-01 06:23:24.000000 FHIRkit-0.0.9/fhirkit/Observation.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     1248 2022-05-01 06:23:40.000000 FHIRkit-0.0.9/fhirkit/OperationOutcome.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     2668 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/Parameter.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     2090 2022-05-01 06:25:21.000000 FHIRkit-0.0.9/fhirkit/Procedure.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     4487 2022-05-01 06:50:11.000000 FHIRkit-0.0.9/fhirkit/Resource.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     1962 2022-04-22 12:20:17.000000 FHIRkit-0.0.9/fhirkit/Server.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     1254 2022-04-22 12:20:17.000000 FHIRkit-0.0.9/fhirkit/SimpleFHIRServer.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     4873 2022-05-01 06:50:33.000000 FHIRkit-0.0.9/fhirkit/ValueSet.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)      365 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/__init__.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)      411 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/data_types.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     4949 2022-05-01 06:50:00.000000 FHIRkit-0.0.9/fhirkit/elements.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)      181 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/metadata_types.py
-drwxr-xr-x   0 axelvanraes   (501) staff       (20)        0 2022-05-01 06:52:01.335923 FHIRkit-0.0.9/fhirkit/snomed/
--rw-r--r--   0 axelvanraes   (501) staff       (20)     3515 2022-05-01 06:25:05.000000 FHIRkit-0.0.9/fhirkit/snomed/ValueSet.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)      125 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/snomed/__init__.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)       35 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/snomed/consts.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     1742 2022-04-22 12:04:21.000000 FHIRkit-0.0.9/fhirkit/snomed/elements.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)     7387 2022-04-22 13:40:46.000000 FHIRkit-0.0.9/fhirkit/snomed/terminology.py
--rw-r--r--   0 axelvanraes   (501) staff       (20)      100 2022-02-08 13:17:47.000000 FHIRkit-0.0.9/pyproject.toml
--rw-r--r--   0 axelvanraes   (501) staff       (20)       38 2022-05-01 06:52:01.336572 FHIRkit-0.0.9/setup.cfg
--rw-r--r--   0 axelvanraes   (501) staff       (20)      656 2022-05-01 06:51:44.000000 FHIRkit-0.0.9/setup.py
+-rw-r--r--   0        0        0     1094 2022-04-22 12:04:21.381197 fhirkit-0.1.0/LICENSE.md
+-rw-r--r--   0        0        0     2029 2022-07-05 12:32:50.506000 fhirkit-0.1.0/README.md
+-rw-r--r--   0        0        0      519 2022-12-22 10:36:31.966808 fhirkit-0.1.0/fhirkit/AllergyIntolerance.py
+-rw-r--r--   0        0        0     4080 2023-05-07 18:20:08.553342 fhirkit-0.1.0/fhirkit/BaseModel.py
+-rw-r--r--   0        0        0     1774 2022-12-22 10:36:31.967024 fhirkit-0.1.0/fhirkit/Bundle.py
+-rw-r--r--   0        0        0      291 2022-10-16 13:55:20.803787 fhirkit-0.1.0/fhirkit/CarePlan.py
+-rw-r--r--   0        0        0      275 2022-07-05 13:42:03.317401 fhirkit-0.1.0/fhirkit/CareTeam.py
+-rw-r--r--   0        0        0     1806 2023-01-20 16:56:35.262451 fhirkit-0.1.0/fhirkit/ClinicalImpression.py
+-rw-r--r--   0        0        0     5490 2023-05-23 08:05:55.237472 fhirkit-0.1.0/fhirkit/CodeSystem.py
+-rw-r--r--   0        0        0     2722 2023-02-16 13:55:38.147678 fhirkit-0.1.0/fhirkit/Composition.py
+-rw-r--r--   0        0        0      381 2022-04-22 12:04:21.383580 fhirkit-0.1.0/fhirkit/CompositionValueSet.py
+-rw-r--r--   0        0        0     5527 2023-05-07 18:20:08.553910 fhirkit-0.1.0/fhirkit/Condition.py
+-rw-r--r--   0        0        0     1020 2023-05-07 18:20:08.554044 fhirkit-0.1.0/fhirkit/Coverage.py
+-rw-r--r--   0        0        0      269 2023-05-23 07:50:16.138796 fhirkit-0.1.0/fhirkit/Device.py
+-rw-r--r--   0        0        0     1614 2023-01-20 16:56:35.263808 fhirkit-0.1.0/fhirkit/DiagnosticReport.py
+-rw-r--r--   0        0        0      302 2022-07-05 13:42:22.509774 fhirkit-0.1.0/fhirkit/DocumentReference.py
+-rw-r--r--   0        0        0     8049 2023-05-07 18:20:08.554838 fhirkit-0.1.0/fhirkit/Encounter.py
+-rw-r--r--   0        0        0      287 2022-07-05 13:42:38.175881 fhirkit-0.1.0/fhirkit/ImagingStudy.py
+-rw-r--r--   0        0        0      287 2022-07-05 13:42:42.441413 fhirkit-0.1.0/fhirkit/Immunization.py
+-rw-r--r--   0        0        0     1591 2022-12-22 10:33:00.422460 fhirkit-0.1.0/fhirkit/Location.py
+-rw-r--r--   0        0        0      281 2022-07-05 13:42:51.346675 fhirkit-0.1.0/fhirkit/Medication.py
+-rw-r--r--   0        0        0      337 2022-07-05 13:42:55.435328 fhirkit-0.1.0/fhirkit/MedicationAdministration.py
+-rw-r--r--   0        0        0      302 2022-07-05 13:42:58.629005 fhirkit-0.1.0/fhirkit/MedicationRequest.py
+-rw-r--r--   0        0        0      322 2022-07-05 13:49:07.575913 fhirkit-0.1.0/fhirkit/MedicationStatement.py
+-rw-r--r--   0        0        0     3658 2023-02-16 13:55:38.147863 fhirkit-0.1.0/fhirkit/Observation.py
+-rw-r--r--   0        0        0     1286 2022-07-19 14:55:47.271304 fhirkit-0.1.0/fhirkit/OperationOutcome.py
+-rw-r--r--   0        0        0     2440 2023-05-22 13:04:33.766917 fhirkit-0.1.0/fhirkit/Organization.py
+-rw-r--r--   0        0        0     2120 2022-07-20 15:15:13.788912 fhirkit-0.1.0/fhirkit/Parameter.py
+-rw-r--r--   0        0        0     3496 2023-05-07 18:20:08.555303 fhirkit-0.1.0/fhirkit/Patient.py
+-rw-r--r--   0        0        0     2547 2023-05-07 18:20:08.556092 fhirkit-0.1.0/fhirkit/Practitioner.py
+-rw-r--r--   0        0        0     3791 2023-05-07 18:20:08.556969 fhirkit-0.1.0/fhirkit/PractitionerRole.py
+-rw-r--r--   0        0        0     5966 2023-05-07 18:20:08.557179 fhirkit-0.1.0/fhirkit/Procedure.py
+-rw-r--r--   0        0        0      281 2022-08-14 11:45:44.118911 fhirkit-0.1.0/fhirkit/Provenance.py
+-rw-r--r--   0        0        0     2943 2023-05-08 07:04:17.842502 fhirkit-0.1.0/fhirkit/Resource.py
+-rw-r--r--   0        0        0     2828 2023-02-16 13:55:38.169585 fhirkit-0.1.0/fhirkit/Server.py
+-rw-r--r--   0        0        0    10578 2023-02-16 13:56:16.230095 fhirkit-0.1.0/fhirkit/SimpleFHIRStore.py
+-rw-r--r--   0        0        0      293 2022-08-14 11:50:43.251431 fhirkit-0.1.0/fhirkit/SupplyDelivery.py
+-rw-r--r--   0        0        0      650 2022-12-22 10:36:31.970229 fhirkit-0.1.0/fhirkit/TerminologyServer.py
+-rw-r--r--   0        0        0     6228 2023-05-22 14:12:40.854533 fhirkit-0.1.0/fhirkit/ValueSet.py
+-rw-r--r--   0        0        0     1842 2023-05-07 18:20:08.558497 fhirkit-0.1.0/fhirkit/__init__.py
+-rw-r--r--   0        0        0       83 2022-07-20 15:52:50.507783 fhirkit-0.1.0/fhirkit/choice_type/__init__.py
+-rw-r--r--   0        0        0     5630 2022-07-20 15:57:33.924942 fhirkit-0.1.0/fhirkit/choice_type/choice_type.py
+-rw-r--r--   0        0        0     1207 2022-12-22 10:36:31.971529 fhirkit-0.1.0/fhirkit/choice_type/validators.py
+-rw-r--r--   0        0        0     1583 2022-07-23 07:15:14.050513 fhirkit-0.1.0/fhirkit/elements/Timing.py
+-rw-r--r--   0        0        0      926 2022-07-23 07:01:36.217241 fhirkit-0.1.0/fhirkit/elements/UsageContext.py
+-rw-r--r--   0        0        0       90 2022-07-19 16:29:33.220298 fhirkit-0.1.0/fhirkit/elements/__init__.py
+-rw-r--r--   0        0        0    10875 2023-05-22 13:04:33.771342 fhirkit-0.1.0/fhirkit/elements/elements.py
+-rw-r--r--   0        0        0     1075 2023-05-07 18:20:08.559365 fhirkit-0.1.0/fhirkit/metadata_types.py
+-rw-r--r--   0        0        0      495 2022-12-22 10:36:31.972058 fhirkit-0.1.0/fhirkit/parse.py
+-rw-r--r--   0        0        0     7228 2023-05-08 07:27:12.193111 fhirkit-0.1.0/fhirkit/primitive_datatypes.py
+-rw-r--r--   0        0        0  3105532 2023-06-09 18:12:56.788995 fhirkit-0.1.0/fhirkit/r5.py
+-rw-r--r--   0        0        0       62 2022-04-22 12:04:21.386086 fhirkit-0.1.0/fhirkit/setup.cfg
+-rw-r--r--   0        0        0     4697 2023-02-16 13:55:38.170341 fhirkit-0.1.0/fhirkit/snomed/ValueSet.py
+-rw-r--r--   0        0        0      125 2022-04-22 12:04:21.386293 fhirkit-0.1.0/fhirkit/snomed/__init__.py
+-rw-r--r--   0        0        0       35 2022-04-22 12:04:21.386364 fhirkit-0.1.0/fhirkit/snomed/consts.py
+-rw-r--r--   0        0        0     1648 2022-07-20 09:32:25.820588 fhirkit-0.1.0/fhirkit/snomed/elements.py
+-rw-r--r--   0        0        0     8174 2023-02-16 13:55:38.170504 fhirkit-0.1.0/fhirkit/snomed/terminology.py
+-rw-r--r--   0        0        0       34 2023-01-20 16:56:35.265286 fhirkit-0.1.0/fhirkit/tiro/__init__.py
+-rw-r--r--   0        0        0      583 2023-01-20 16:56:35.265401 fhirkit-0.1.0/fhirkit/tiro/elements.py
+-rw-r--r--   0        0        0      336 2023-06-09 18:19:46.713411 fhirkit-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2491 1970-01-01 00:00:00.000000 fhirkit-0.1.0/PKG-INFO
```

### Comparing `FHIRkit-0.0.9/LICENSE.md` & `fhirkit-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.0.9/fhirkit/CodeSystem.py` & `fhirkit-0.1.0/fhirkit/CodeSystem.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,71 @@
 from __future__ import annotations
-from email.generator import Generator
-from typing import Any, ClassVar, Optional, Sequence, Set, TypeVar, Union
+from typing import (
+    Any,
+    ClassVar,
+    Iterable,
+    Optional,
+    Sequence,
+    Set,
+    TypeVar,
+    Union,
+    Generator,
+)
+
+from fhirkit.choice_type import ChoiceType
 
 try:
     from typing import Literal
 except ImportError:
-    from typing_extensions import Literal
+    from typing_extensions import Literal  # type: ignore
 
-from pydantic import AnyUrl, Field, StrictBool, StrictStr, validator
-from fhirkit.Resource import CanonicalResource, DomainResource
-from fhirkit.ChoiceTypeMixin import ChoiceTypeMixinBase, validate_choice_types
+from pydantic import Field, StrictBool, StrictStr, validator
+from fhirkit.Resource import CanonicalResource
+from fhirkit.choice_type import deterimine_choice_type
 from fhirkit.elements import (
     BackboneElement,
     CodeableConcept,
     Coding,
     Identifier,
     UsageContext,
 )
-from fhirkit.data_types import Code, dateTime
+from fhirkit.primitive_datatypes import URI, Code, dateTime, date
 from fhirkit.metadata_types import ContactDetail
 
 
 class CodeLookupError(KeyError):
     pass
 
 
 class CSConceptDesignation(BackboneElement):
     language: Optional[Code]
     use: Optional[Coding]
     value: str
 
 
-class CSConceptPropertyValueChoiceTypeMixin(ChoiceTypeMixinBase):
-    _choice_type_fields: ClassVar[Set[str]] = [
-        "valueBoolean",
-        "valueString",
-        "valueCode",
-        "valueCoding",
-        "valueDateTime",
-        "valueDecimal",
-    ]
-    _polymorphic_field: ClassVar[Set[str]] = "value"
+class CSConceptProperty(BackboneElement):
+    code: Code
     valueBoolean: Optional[StrictBool] = Field(None)
-    valueString: Optional[StrictStr] = Field(None)
-    valueCode: Optional[Code] = Field(None)
+    valueString: Optional[StrictStr] = Field(None,)
+    valueCode: Optional[Code] = Field(None,)
     valueCoding: Optional[Coding] = Field(None)
     valueDateTime: Optional[dateTime] = Field(None)
     valueDecimal: Optional[float] = Field(None)
-    value: Union[StrictBool, StrictStr, Code, Coding, dateTime, float] = Field(
-        None, exclude=True
-    )
-
-    validate_value = validator("value", pre=True, always=True, allow_reuse=True)(
-        validate_choice_types
-    )
-
-    def __str__(self) -> str:
-        return str(self.value)
 
-
-class CSConceptProperty(BackboneElement, CSConceptPropertyValueChoiceTypeMixin):
-    code: Code
+    @property
+    def value(self)->StrictBool|StrictStr|Code|Coding|dateTime|float:
+        for prop in self.__fields__.keys():
+            if prop.startswith("value"):
+                v = getattr(self, prop)
+                if v is not None:
+                    return v
+        raise RuntimeError("No value found in CSConceptProperty")
 
     def __str__(self) -> str:
-        return str(self.code) + ": " + super().__str__()
-
+        return str(self.code) + ": " + str(self.value)
 
 class CSConcept(BackboneElement):
     code: Code
     display: Optional[str]
     definition: Optional[str]
     designation: Sequence[CSConceptDesignation] = []
     property: Sequence[CSConceptProperty] = []
@@ -91,52 +88,49 @@
         )
 
 
 class CSConceptLookup(CSConcept):
     name: str
 
 
-C = TypeVar("C", bound=CSConcept)
-
-
 def traverse_concepts(
-    s: Sequence[C],
-) -> Generator[C, None, None]:
+    s: Iterable[CSConcept],
+) -> Generator[CSConcept, None, None]:
     for c in s:
         yield c
         if len(c.concept) > 0:
             yield from traverse_concepts(c.concept)
 
 
 class CodeSystem(CanonicalResource):
-    resourceType = Field("CodeSystem", const=True)
-    url: Optional[AnyUrl]
+    resourceType:Literal["CodeSystem"] = Field("CodeSystem", const=True)
+    url: Optional[URI]
     identifier: Sequence[Identifier] = []
     version: Optional[str]
     name: Optional[str]
     title: Optional[str]
     status: Literal["draft", "active", "retired", "unknown"]
     experimental: Optional[bool]
-    date: Optional[dateTime]
+    date: Optional[Union[date, dateTime]]
     publisher: Optional[str]
     contact: Sequence[ContactDetail] = []
     description: Optional[str]
     useContext: Sequence[UsageContext] = []
     jurisdiction: Sequence[CodeableConcept] = []
     purpose: Optional[str]
     copyright: Optional[str]
     caseSensitive: Optional[bool]
-    valueSet: Optional[AnyUrl]
+    valueSet: Optional[URI]
     hierarchyMeaning: Optional[
         Literal["grouped-by", "is-a", "part-of", "classified-with"]
     ]
     compositional: Optional[bool]
     versionNeeded: Optional[bool]
     content: Literal["not-present", "example", "fragment", "complete", "supplement"]
-    supplements: Optional[AnyUrl]
+    supplements: Optional[URI]
     count: Optional[int]
     concept: Sequence[CSConcept] = []
 
     def lookup(
         self,
         code: Optional[Code] = None,
         coding: Optional[Coding] = None,
@@ -166,27 +160,23 @@
                     **concept.dict(
                         include={
                             "code",
                             "designation",
                             "property",
                             "display",
                             "version",
-                        },
-                        exclude_unset=True,
+                        }
                     ),
                 )
 
         raise CodeLookupError(
             f"No concept found in CodeSystem for given code/coding. (code={code}, coding={coding})"
         )
 
-    def __iter__(self):
+    def iter(self) -> Generator[CSConcept, None, None]:
         yield from traverse_concepts(self.concept)
 
-    def __getitem__(self, key: Code | Coding) -> CSConceptLookup:
-        if isinstance(key, (Code, str)):
-            return self.lookup(code=key)
-        elif isinstance(key, Coding):
-            return self.lookup(coding=key)
-        raise KeyError("Key should be a Code or a Coding but received " + key)
 
-    CSConcept.update_forward_refs()
+CodeSystem.update_forward_refs()
+for cs_subclass in CodeSystem.__subclasses__():
+    cs_subclass.update_forward_refs()
+CSConcept.update_forward_refs()
```

### Comparing `FHIRkit-0.0.9/fhirkit/Observation.py` & `fhirkit-0.1.0/fhirkit/Resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,108 @@
-from typing import ClassVar, Optional, Sequence, Set, Union
+from __future__ import annotations
+import warnings
+
+from fhirkit.elements.elements import Reference
 
 try:
     from typing import Literal
 except ImportError:
-    from typing_extensions import Literal
-
-
-from pydantic import Field, validator
-from fhirkit.ChoiceTypeMixin import (
-    ChoiceTypeMixinBase,
-    validate_choice_types,
+    from typing_extensions import Literal  # type: ignore
+from typing import (
+    AbstractSet,
+    Any,
+    List,
+    Dict,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+    Generator,
 )
-from fhirkit.Resource import DomainResource
-from fhirkit.data_types import Code, dateTime
+from pydantic import Extra, Field, PrivateAttr
+from fhirkit.BaseModel import BaseModel
+from fhirkit.primitive_datatypes import URI, Code, Id, Instant, dateTime, date
 from fhirkit.elements import (
+    AbstractFHIRServer,
+    BackboneElement,
     CodeableConcept,
+    Element,
     Identifier,
+    Narrative,
+    Extension,
+    Coding,
     Period,
-    Quantity,
-    Reference,
-    BackboneElement,
+    Range,
+    UsageContext,
+    Meta
 )
+from fhirkit.metadata_types import ContactDetail
 
-# TODO find better solution for multitype value
-class ObservationValueChoiceTypeMixin(ChoiceTypeMixinBase):
-    _choice_type_fields: ClassVar[Set[str]] = [
-        "valueString",
-        "valueQuantity",
-        "valueInteger",
-        "valueCodeableConcept",
-        "valueBoolean",
-    ]
-    _polymorphic_field: ClassVar[Set[str]] = "value"
-    valueString: Optional[str] = None
-    valueQuantity: Optional[Quantity] = None
-    valueInteger: Optional[int] = None
-    valueCodeableConcept: Optional[CodeableConcept] = None
-    valueBoolean: Optional[bool] = None
-    value: Union[str, Quantity, int, CodeableConcept, bool] = None
-
-    validate_value = validator("value", pre=True, always=True, allow_reuse=True)(
-        validate_choice_types
-    )
-
-
-class ObservationEffectiveChoiceTypeMixin(ChoiceTypeMixinBase):
-    _choice_type_fields: ClassVar[Set[str]] = ["effectiveDateTime", "effectivePeriod"]
-    _polymorphic_field: ClassVar[str] = "effective"
-    effectiveDateTime: Optional[dateTime] = None
-    effectivePeriod: Optional[Period] = None
-    effective: Union[dateTime, Period] = None
-
-    validate_effective = validator(
-        "effective", pre=True, always=True, allow_reuse=True
-    )(validate_choice_types)
-
-
-class ObservationComponent(BackboneElement, ObservationValueChoiceTypeMixin):
-    code: CodeableConcept
-
-
-class Observation(
-    DomainResource, ObservationValueChoiceTypeMixin, ObservationEffectiveChoiceTypeMixin
-):
-
-    resourceType = Field("Observation", const=True)
-    identifier: Sequence[Identifier] = Field([], repr=True)
-    status: Literal[
-        "registered",
-        "preliminary",
-        "final",
-        "amended",
-        "corrected",
-        "cancelled",
-        "enterred-in-error",
-        "unknown",
-    ] = Field("final", repr=True)
-    category: Optional[CodeableConcept] = Field(None, repr=True)
-    code: CodeableConcept = Field(..., repr=True)
-    subject: Optional[Reference]
-    encounter: Optional[Reference]
-
-    method: Optional[Code] = Field(None, repr=False)
-    derivedFrom: Optional[Reference]
-
-    component: Sequence[ObservationComponent] = []
+InclusionExclusion = Union[AbstractSet[Union[int, str]], Mapping[Union[int, str], Any]]
+AbstractSetIntStr = AbstractSet[Union[int, str]]
+MappingIntStrAny = Mapping[Union[int, str], Any]
+
+RESOURCE_MODELS = []
+
+class Resource(BaseModel):
+
+    resourceType: str
+    id: Optional[str] = Field(None, repr=False)
+    meta: Optional[Meta] = Field(None, repr=False)
+    implicitRules: Optional[URI] = Field(None, repr=False)
+    language: Optional[Code] = Field(None, repr=False)
+
+    def __init_subclass__(cls) -> None:
+        RESOURCE_MODELS.append(cls)
+
+    def __str__(self) -> str:
+        text = self.resourceType
+        if self.id:
+            text += f"/{self.id}"
+        return text
+
+    class Config:
+        arbitrary_types_allowed = True
+        extra = Extra.allow
+
+    def get_references(self):
+        for k, v in self._iter():
+            if isinstance(v, Reference):
+                yield k, v
+
+    def to_reference(self):
+        return Reference(type=self.resourceType, reference=f"{self.resourceType}/{self.id}")
+
+
+class DomainResource(Resource):
+    text: Optional[Narrative] = Field(None, repr=False)
+    contained: Sequence[Resource] = Field([], repr=False)
+    extension: Sequence[Extension] = Field([], repr=False)
+    modifierExtension: Sequence[Extension] = Field([], repr=False)
+
+    def _repr_html_(self):
+        if self.text:
+            return self.text.div
+        else:
+            return repr(self)
+
+
+class ResourceWithMultiIdentifier(Resource):
+    identifier: Sequence[Identifier] = []
+
+
+class CanonicalResource(DomainResource, ResourceWithMultiIdentifier):
+    url: Optional[URI] = None
+    version: Optional[str] = None
+    name: Optional[str] = None
+    title: Optional[str] = None
+    status: Literal["draft", "active", "retired", "unknown"]
+    experimental: Optional[bool] = None
+    date: Optional[Union[date, dateTime]] = None
+    publisher: Optional[str] = None
+    contact: Sequence[ContactDetail] = []
+    description: Optional[str] = None
+    useContext: Sequence[UsageContext] = []
+    jurisdiction: Sequence[CodeableConcept] = []
+    purpose: Optional[str] = None
+    copyright: Optional[str] = None
```

### Comparing `FHIRkit-0.0.9/fhirkit/OperationOutcome.py` & `fhirkit-0.1.0/fhirkit/OperationOutcome.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 from typing import Optional, Sequence
 from pydantic import Field
 from fhirkit.Resource import DomainResource
 from fhirkit.elements import BackboneElement, CodeableConcept
-from fhirkit.data_types import Code
+from fhirkit.primitive_datatypes import Code
 
 
 class OperationOutcomeIssue(BackboneElement):
     severity: Literal["fatal", "error", "warning", "information"]
     code: Code  # TODO add logic that can bind this to valueset
     details: Optional[CodeableConcept] = None
     diagnostics: Optional[str] = None
@@ -21,15 +21,15 @@
         txt = f"[{self.severity}](issue type={self.code}) "
         if self.diagnostics:
             txt += self.diagnostics
         return txt
 
 
 class OperationOutcome(DomainResource):
-    resourceType = Field("OperationOutcome", const=True)
+    resourceType: Literal["OperationOutcome"] = Field("OperationOutcome", const=True)
     issue: Sequence[OperationOutcomeIssue] = []
 
     def __str__(self) -> str:
         return "OperationOutcome: \n" + "\n\n".join(str(issue) for issue in self.issue)
 
 
 class OperationOutcomeException(Exception):
```

### Comparing `FHIRkit-0.0.9/fhirkit/Parameter.py` & `fhirkit-0.1.0/fhirkit/Parameter.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,41 @@
-from typing import Any, ClassVar, List, Optional, Set, Union
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
+
+from typing import Any, List, Optional, Union
 from pydantic import (
     Field,
     HttpUrl,
     StrictInt,
     StrictStr,
     StrictBool,
     validator,
 )
-from fhirkit.ChoiceTypeMixin import ChoiceTypeMixinBase, validate_choice_types
+from fhirkit.choice_type import deterimine_choice_type
 from fhirkit.Resource import Resource
-from fhirkit.data_types import Code
+from fhirkit.primitive_datatypes import Code
 from fhirkit.elements import BackboneElement, CodeableConcept, Coding
 
 
-class ParameterValueChoiceTypeMixin(ChoiceTypeMixinBase):
-    _choice_type_fields: ClassVar[Set[str]] = [
-        "valueBoolean",
-        "valueString",
-        "valueCode",
-        "valueCoding",
-        "valueCodeableConcept",
-        "valueUri",
-        "valueInteger",
-    ]
-    _polymorphic_field: ClassVar[Set[str]] = "value"
-    valueBoolean: Optional[StrictBool] = Field(None)
-    valueString: Optional[StrictStr] = Field(None)
-    valueCode: Optional[Code] = Field(None)
-    valueCoding: Optional[Coding] = Field(None)
-    valueCodeableConcept: Optional[CodeableConcept] = Field(None)
-    valueUri: Optional[HttpUrl] = Field(None)
-    valueInteger: Optional[StrictInt] = Field(None)
-    value: Union[
-        StrictBool, StrictStr, Code, Coding, CodeableConcept, HttpUrl, StrictInt
-    ] = Field(None, exclude=True)
-
-    validate_value = validator("value", pre=True, always=True, allow_reuse=True)(
-        validate_choice_types
-    )
-
-
 class AbstractParameter(BackboneElement):
     name: str
 
 
-class ValueParameter(
-    AbstractParameter,
-    ParameterValueChoiceTypeMixin,
-):
+class ValueParameter(AbstractParameter):
+    valueBoolean: Optional[bool] = Field(None, exclude=True)
+    value: Union[
+        StrictBool, StrictStr, Code, Coding, CodeableConcept, HttpUrl, StrictInt
+    ] = None
+
+    @validator("value", pre=True, always=True, allow_reuse=True)
+    def validate_value(cls, v, values, field):
+        return deterimine_choice_type(cls, v, values, field)
+
     def __str__(self) -> str:
         return f"{self.name}:{self.value}"
 
 
 class ResourceParameter(AbstractParameter):
     resource: Optional[Resource]
 
@@ -69,15 +53,15 @@
             raise
 
     def __str__(self) -> str:
         return "\n\tpart: \n" + "\n\t".join(" " + str(p) for p in self.part)
 
 
 class Parameters(Resource):
-    resourceType = Field("Parameters", const=True)
+    resourceType: Literal["Parameters"] = Field("Parameters", const=True)
     parameter: List[Union[ValueParameter, ResourceParameter, MultiPartParameter]]
 
     def __getattribute__(self, __name: str) -> Any:
         try:
             return super().__getattribute__(__name)
         except AttributeError:
             for param in self.parameter:
```

### Comparing `FHIRkit-0.0.9/fhirkit/snomed/elements.py` & `fhirkit-0.1.0/fhirkit/snomed/elements.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from typing import Optional
 from pydantic import Field, HttpUrl
-from fhirkit.Server import AbstractFHIRTerminologyServer
 from fhirkit.elements import CodeableConcept, Coding
-from fhirkit.ValueSet import ValueSet
 from .ValueSet import (
     SCTDescendantsFilter,
     SCTImplicitCompose,
     SCTImplicitInclude,
     SCTImplicitValueSet,
 )
 
@@ -22,14 +19,15 @@
             super().__init__(code=code, display=display, **kwargs)
         else:
             super().__init__(*args, **kwargs)  # business as usual, Pydantic takes over
 
     def descendants(self):
         return SCTImplicitValueSet(
             url=f"{self.system}?fhir_vs=isa/{self.code}",
+            status="active",
             compose=SCTImplicitCompose(
                 include=[
                     SCTImplicitInclude(
                         system=self.system,
                         filter=[
                             SCTDescendantsFilter(
                                 property="concept", op="is-a", value=self.code
```

### Comparing `FHIRkit-0.0.9/fhirkit/snomed/terminology.py` & `fhirkit-0.1.0/fhirkit/snomed/terminology.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,46 @@
 from __future__ import annotations
 import logging
 from urllib.parse import urlencode
-import time
-from typing import ClassVar, List, Optional, Union
-from webbrowser import Opera
+
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
+from pydantic import Field
+
+from typing import ClassVar, Optional, Union
+
+try:
+    from typing import Annotated
+except ImportError:
+    from typing_extensions import Annotated
+
 import requests
-from pydantic import HttpUrl, ValidationError, parse_obj_as, parse_raw_as
+from pydantic import Field, HttpUrl, ValidationError, parse_obj_as
 from fhirkit.Parameter import Parameters
-from fhirkit.Server import AbstractFHIRTerminologyServer
-from fhirkit.ValueSet import VSCodingWithDesignation, VSExpansion, ValueSet
-from fhirkit.data_types import Code
+from fhirkit.Server import AbstractFHIRServer
+from fhirkit.TerminologyServer import AbstractFHIRTerminologyServer
+from fhirkit.ValueSet import VSExpansion, ValueSet
+from fhirkit.primitive_datatypes import URI, Code
 from fhirkit.elements import CodeableConcept, Coding
 from fhirkit.OperationOutcome import OperationOutcome, OperationOutcomeException
 
 
 class ExpandedValueset(ValueSet):
+    status: Literal["active"] = Field("active")
     expansion: VSExpansion
 
 
-Response = Union[Parameters, OperationOutcome]
-VSExpansionResponse = Union[ExpandedValueset, OperationOutcome]
+Response = Annotated[
+    Union[Parameters, OperationOutcome], Field(discriminator="resourceType")
+]
+VSExpansionResponse = Annotated[
+    Union[ExpandedValueset, OperationOutcome], Field(discriminator="resourceType")
+]
 
 
 class SCTFHIRTerminologyServer(AbstractFHIRTerminologyServer):
     DEFAULT_URL: ClassVar[
         str
     ] = "https://browser.ihtsdotools.org/snowstorm/snomed-ct/fhir"
     DEFAULT_SERVER: ClassVar[Optional[SCTFHIRTerminologyServer]] = None
@@ -36,14 +53,23 @@
 
     @classmethod
     def default_server(cls):
         if cls.DEFAULT_SERVER is None:
             cls.DEFAULT_SERVER = SCTFHIRTerminologyServer()
         return cls.DEFAULT_SERVER
 
+    def get_terminology_resource(
+        self,
+        resourceType: Optional[str],
+        *,
+        id: Optional[str] = None,
+        url: Optional[URI] = None,
+    ):
+        return super().get_terminology_resource(resourceType, id=id, url=url)
+
     def get_resource(
         self, resourceType: str, *, id: Optional[str] = None, url: Optional[str] = None
     ):
         path = resourceType
         if id:
             path += "/" + id
         req_url = f"{self.base_url}/{path}"
@@ -58,15 +84,15 @@
                     "Received an error from the snowstorm server (%s) after sending the following request %s",
                     raw_response.text,
                     req_url,
                 )
             response = parse_obj_as(Response, raw_response.json())
         except ValidationError:
             raise ConnectionError(
-                f"Received a response that doesn't resemble a FHIR-server. Please check if the server at {self.base_url} is a valid FHIR-server"
+                f"Received a response that doesn't resemble a FHIR-resource. Please check if the server at {self.base_url} is a valid FHIR-server"
             )
         except:
             raise RuntimeWarning(
                 "Failed when calling {endpoint} on {base_url}".format(
                     endpoint=path, base_url=self.base_url
                 )
             )
@@ -114,17 +140,18 @@
                 yield response
 
                 offset = response.expansion.offset + page_size
                 remaining = max(response.expansion.total - offset, 0)
 
             except ValidationError:
                 raise ConnectionError(
-                    f"Received a response that doesn't resemble a FHIR-server. Please check if the server at {self.base_url} is a valid FHIR-server"
+                    f"Received a response that doesn't resemble a FHIR-server. Please check if the server at {self.base_url} is a valid FHIR-server. \n Response:\n\n {raw_response.json()}"
                 )
             except:
+                raise
                 raise RuntimeWarning(
                     "Failed when calling {endpoint} on {base_url}".format(
                         endpoint=path, base_url=self.base_url
                     )
                 )
             else:
 
@@ -191,8 +218,12 @@
 
         if isinstance(response, OperationOutcome):
             raise OperationOutcomeException(response)
 
         return response
 
 
+def get_default_terminology_server():
+    return SCTFHIRTerminologyServer.default_server()
+
+
 DEFAULT_TERMINOLOGY_SERVER = SCTFHIRTerminologyServer()
```

