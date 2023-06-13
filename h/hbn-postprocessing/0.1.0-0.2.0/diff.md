# Comparing `tmp/hbn_postprocessing-0.1.0.tar.gz` & `tmp/hbn_postprocessing-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hbn_postprocessing-0.1.0.tar", max compression
+gzip compressed data, was "hbn_postprocessing-0.2.0.tar", max compression
```

## Comparing `hbn_postprocessing-0.1.0.tar` & `hbn_postprocessing-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       70 2023-05-11 19:33:07.365330 hbn_postprocessing-0.1.0/README.md
--rw-r--r--   0        0        0       38 2023-05-12 16:53:18.721105 hbn_postprocessing-0.1.0/hbn_postprocessing/__init__.py
--rw-r--r--   0        0        0     2524 2023-05-12 19:03:30.776826 hbn_postprocessing-0.1.0/hbn_postprocessing/file_count.py
--rw-r--r--   0        0        0     1046 2023-05-12 19:05:10.882933 hbn_postprocessing-0.1.0/hbn_postprocessing/html.py
--rw-r--r--   0        0        0     1948 2023-05-12 19:07:08.409406 hbn_postprocessing-0.1.0/hbn_postprocessing/jobs.py
--rw-r--r--   0        0        0     1160 2023-05-12 19:09:12.476015 hbn_postprocessing-0.1.0/hbn_postprocessing/main.py
--rw-r--r--   0        0        0     2096 2023-05-12 19:09:15.916087 hbn_postprocessing-0.1.0/hbn_postprocessing/motion.py
--rw-r--r--   0        0        0      833 2023-05-12 19:00:23.976893 hbn_postprocessing-0.1.0/hbn_postprocessing/utils.py
--rw-r--r--   0        0        0     1265 2023-05-12 19:18:18.238980 hbn_postprocessing-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 hbn_postprocessing-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       70 2023-05-11 19:33:07.365330 hbn_postprocessing-0.2.0/README.md
+-rw-r--r--   0        0        0       38 2023-05-12 16:53:18.721105 hbn_postprocessing-0.2.0/hbn_postprocessing/__init__.py
+-rw-r--r--   0        0        0     2697 2023-06-13 19:43:38.223130 hbn_postprocessing-0.2.0/hbn_postprocessing/file_count.py
+-rw-r--r--   0        0        0     1158 2023-06-13 19:43:17.626702 hbn_postprocessing-0.2.0/hbn_postprocessing/html.py
+-rw-r--r--   0        0        0     2058 2023-06-13 19:48:15.792904 hbn_postprocessing-0.2.0/hbn_postprocessing/jobs.py
+-rw-r--r--   0        0        0     1411 2023-06-13 19:53:47.475811 hbn_postprocessing-0.2.0/hbn_postprocessing/main.py
+-rw-r--r--   0        0        0     2199 2023-06-13 19:56:13.470853 hbn_postprocessing-0.2.0/hbn_postprocessing/motion.py
+-rw-r--r--   0        0        0      833 2023-05-12 19:00:23.976893 hbn_postprocessing-0.2.0/hbn_postprocessing/utils.py
+-rw-r--r--   0        0        0     1265 2023-06-13 18:48:58.739363 hbn_postprocessing-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 hbn_postprocessing-0.2.0/PKG-INFO
```

### Comparing `hbn_postprocessing-0.1.0/hbn_postprocessing/file_count.py` & `hbn_postprocessing-0.2.0/hbn_postprocessing/file_count.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,46 +35,53 @@
 }
 
 
 def count_files(bids_dir: os.PathLike[str] | str, subj_id: str) -> dict[str, int | str]:
     """Count the T1w, bold, and fMRI_epi files for the subject."""
     subj_dir = Path(bids_dir) / f"sub-{subj_id}"
     content = glob_dir(subj_dir, "*", filter_=lambda path: path.is_dir())
-    sub_dict: dict[str, int | str] = {"id": subj_id}
+    sub_dict: dict[str, int | str] = {"participant_id": f"sub-{subj_id}"}
 
     for datatype_dir in content:
         datatype = datatype_dir.name
         if datatype not in DATATYPE_SPECS:
             continue
         sub_dict.update(DATATYPE_SPECS[datatype].count_files(datatype_dir))
 
     return sub_dict
 
 
 def count_all_files(
     bids_dir: os.PathLike[str] | str,
     out_dir: os.PathLike[str] | str,
-) -> None:
+) -> pd.DataFrame:
     """Write CSVs with relevant image counts."""
     bids_path = Path(bids_dir)
-    file_count_df = pd.DataFrame(
-        [
-            count_files(bids_path, sub_dir.name.split("-")[1])
-            for sub_dir in glob_dir(
-                bids_path,
-                "sub-*",
-                filter_=lambda path: path.is_dir(),
-            )
-        ],
+    file_count_df = (
+        pd.DataFrame(
+            [
+                count_files(bids_path, sub_dir.name.split("-")[1])
+                for sub_dir in glob_dir(
+                    bids_path,
+                    "sub-*",
+                    filter_=lambda path: path.is_dir(),
+                )
+            ],
+        )
+        .astype({"participant_id": pd.StringDtype()})
+        .set_index("participant_id")
     )
     out_path = Path(out_dir)
-    file_count_df.to_csv(out_path / "BIDS-count_all.csv", sep=",", index=False)
+    file_count_df.to_csv(out_path / "BIDS-count_all.csv", sep=",")
     exclude_df = file_count_df.loc[
         lambda df: (df["t1_files"] == 0) | (df["fmap_files"] == 0),
         :,
     ]
-    exclude_df.to_csv(out_path / "BIDS-count_exclude.csv", sep=",", index=False)
-    file_count_df.loc[lambda df: ~df["id"].isin(exclude_df["id"]), :].to_csv(
+    exclude_df.to_csv(out_path / "BIDS-count_exclude.csv", sep=",")
+    file_count_df.loc[
+        lambda df: ~df.index.isin(exclude_df.index),
+        :,
+    ].to_csv(
         out_path / "BIDS-count_include.csv",
         sep=",",
-        index=False,
     )
+    return file_count_df
```

### Comparing `hbn_postprocessing-0.1.0/hbn_postprocessing/html.py` & `hbn_postprocessing-0.2.0/hbn_postprocessing/html.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,28 +8,32 @@
 from hbn_postprocessing.utils import glob_dir
 
 
 def check_html(
     fmriprep_out_dir: os.PathLike[str] | str,
     participants_path: os.PathLike[str] | str,
     out_dir: os.PathLike[str] | str,
-) -> None:
+) -> pd.DataFrame:
     """Write a set of summary CSVs checking if participants have an HTML file."""
     html_files = {file_.stem for file_ in glob_dir(fmriprep_out_dir, "*.html*")}
-    participants = pd.read_csv(participants_path)
+    participants = (
+        pd.read_csv(participants_path)
+        .astype({"participant_id": pd.StringDtype()})
+    )
     matches = participants.assign(
         html=participants["participant_id"]
         .isin(html_files)
         .replace([True, False], ["yes", "no"]),
-    )
+    ).set_index("participant_id")
     out_path = Path(out_dir)
-    matches.to_csv(out_path / "html-check_all.csv", sep=",", index=False)
+    matches.to_csv(out_path / "html-check_all.csv", sep=",")
     matches[matches["html"] == "no"].to_csv(
         out_path / "html-check_no.csv",
         sep=",",
         index=False,
     )
     matches[matches["html"] == "yes"].to_csv(
         out_path / "html-check_yes.csv",
         sep=",",
         index=False,
     )
+    return matches
```

### Comparing `hbn_postprocessing-0.1.0/hbn_postprocessing/jobs.py` & `hbn_postprocessing-0.2.0/hbn_postprocessing/jobs.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,43 +4,46 @@
 from pathlib import Path
 
 import pandas as pd
 
 from hbn_postprocessing.utils import glob_dir
 
 STARTED_THRESHOLD_KB = 10
-COMPLETED_THRESHOLD_KB = 400
+COMPLETED_THRESHOLD_KB = 4000
 
 
 def _process_job_file(file_: Path) -> dict[str, str | float]:
     with file_.open() as file_content:
         out_content = file_content.read()
     subj_id = out_content.partition("participant_label ")[2][0:12]
     size_kb = file_.stat().st_size / 1000
     return {"name": file_.name, "p_id": subj_id, "size_kb": size_kb}
 
 
 def check_jobs(
     jobs_dir: os.PathLike[str] | str,
     out_dir: os.PathLike[str] | str,
-) -> None:
+) -> pd.DataFrame:
     """Parse a dir of ".out" files to check for incomplete jobs."""
     out_files = glob_dir(jobs_dir, "*.out*")
     file_info = [_process_job_file(file_) for file_ in out_files]
-    size_df = pd.DataFrame(
-        {
-            "file_name": [file_["name"] for file_ in file_info],
-            "p_id": [file_["p_id"] for file_ in file_info],
-            "size_kb": [file_["size_kb"] for file_ in file_info],
-        },
-    ).loc[lambda df: df["p_id"].str.startswith("NDA"), :]
+    size_df = (
+        pd.DataFrame(
+            {
+                "file_name": [file_["name"] for file_ in file_info],
+                "participant_id": [f'sub-{file_["p_id"]}' for file_ in file_info],
+                "size_kb": [file_["size_kb"] for file_ in file_info],
+            },
+        )
+        .astype({"participant_id": pd.StringDtype()})
+        .loc[lambda df: df["participant_id"].str.startswith("sub-NDA"), :]
+    )
     max_size = (
-        size_df.groupby("p_id")
+        size_df.groupby("participant_id")
         .max()
-        .reset_index()
         .assign(
             status=lambda df: df.size_kb.map(
                 lambda size_kb: "not started"
                 if size_kb < STARTED_THRESHOLD_KB
                 else (
                     "partial/error"
                     if size_kb < COMPLETED_THRESHOLD_KB
@@ -51,14 +54,13 @@
     )
 
     out_path = Path(out_dir)
     max_size.to_csv(out_path / "out-size_all.csv")
     max_size.loc[max_size.status != "likely_complete", :].to_csv(
         out_path / "out-size_incomp.csv",
         sep=",",
-        index=False,
     )
     max_size.loc[max_size.status == "likely complete", :].to_csv(
         out_path / "out-size_comp.csv",
         sep=",",
-        index=False,
     )
+    return max_size
```

### Comparing `hbn_postprocessing-0.1.0/hbn_postprocessing/main.py` & `hbn_postprocessing-0.2.0/hbn_postprocessing/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,19 +21,25 @@
     return parser
 
 
 def main() -> None:
     """Run all relevant tasks."""
     args = gen_parser().parse_args()
 
-    count_all_files(args.bids_dir, args.out_dir)
-    check_html(
+    file_count_df = count_all_files(args.bids_dir, args.out_dir)
+    html_check_df = check_html(
         args.fmriprep_dir,
         Path(args.bids_dir) / "participants.tsv",
         args.out_dir,
     )
-    check_jobs(args.jobs_dir, args.out_dir)
-    exclude_by_motion(args.fmriprep_dir, args.out_dir)
+    out_size_df = check_jobs(args.jobs_dir, args.out_dir)
+    motion_outliers_df = exclude_by_motion(args.fmriprep_dir, args.out_dir)
+    file_count_df.join(
+        [html_check_df, out_size_df, motion_outliers_df], how="outer",
+    ).to_csv(
+        Path(args.out_dir) / "overall_summary.csv",
+        sep=",",
+    )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `hbn_postprocessing-0.1.0/hbn_postprocessing/motion.py` & `hbn_postprocessing-0.2.0/hbn_postprocessing/motion.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 def get_framewise_displacement(
     subj_dir: os.PathLike[str] | str,
 ) -> dict[str, str | float]:
     """Get the framewise displacement in each task for a subject."""
     subj_path = Path(subj_dir)
     tsvs = glob_dir(subj_path / "func", "*.tsv*")
-    sub_dict: dict[str, str | float] = {"id": subj_path.name}
+    sub_dict: dict[str, str | float] = {"participant_id": subj_path.name}
     for tsv in tsvs:
         match = re.match(CONFOUNDS_PATTERN, tsv.name)
         if not match:
             raise ValueError
         task = match.group("task")
         run = f"_run-{match.group('run')}" if match.group("run") else ""
         task_run = f"{task}{run}"
@@ -35,29 +35,33 @@
         sub_dict[task_run] = data["framewise_displacement"].tail(-1).mean()
     return sub_dict
 
 
 def exclude_by_motion(
     bids_dir: os.PathLike[str] | str,
     out_dir: os.PathLike[str] | str,
-) -> None:
+) -> pd.DataFrame:
     """Find outliers by framewise displacement per task."""
     subj_dirs = glob_dir(bids_dir, "sub*", filter_=lambda path: path.is_dir())
-    displacement_df = pd.DataFrame(
-        [get_framewise_displacement(subj_dir) for subj_dir in subj_dirs],
+    displacement_df = (
+        pd.DataFrame(
+            [get_framewise_displacement(subj_dir) for subj_dir in subj_dirs],
+        )
+        .astype({"participant_id": pd.StringDtype()})
+        .set_index("participant_id")
     )
-    group_fds = displacement_df.iloc[:, 1:].mean(axis=0)
-    group_sds = displacement_df.iloc[:, 1:].mean(axis=0)
+    group_fds = displacement_df.mean(axis=0)
+    group_sds = displacement_df.mean(axis=0)
     upper_lims = group_fds + (2 * group_sds)
-    for task_run in set(displacement_df.columns) - {"id"}:
+    for task_run in displacement_df.columns:
         displacement_df = displacement_df.assign(
             **{
                 f"{task_run}_is_outlier": displacement_df[task_run]
                 > upper_lims[task_run],
             },
         )
         displacement_df = displacement_df.drop(task_run, axis=1)
     displacement_df.to_csv(
         Path(out_dir) / "motion-outliers_all.csv",
         sep=",",
-        index=False,
     )
+    return displacement_df
```

### Comparing `hbn_postprocessing-0.1.0/hbn_postprocessing/utils.py` & `hbn_postprocessing-0.2.0/hbn_postprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `hbn_postprocessing-0.1.0/pyproject.toml` & `hbn_postprocessing-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hbn-postprocessing"
-version = "0.1.0"
+version = "0.2.0"
 description = "Postprocessing workflow for HBN data"
 authors = ["Tristan Kuehn <tkuehn@uwo.ca>", "Jessica Lammert <jlammert@uwo.ca>"]
 readme = "README.md"
 packages = [{include = "hbn_postprocessing"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `hbn_postprocessing-0.1.0/PKG-INFO` & `hbn_postprocessing-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hbn-postprocessing
-Version: 0.1.0
+Version: 0.2.0
 Summary: Postprocessing workflow for HBN data
 Author: Tristan Kuehn
 Author-email: tkuehn@uwo.ca
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

