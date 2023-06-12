# Comparing `tmp/dlhpcstarter-0.1.3.tar.gz` & `tmp/dlhpcstarter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/datasets/work/hb-mlaifsp-mm/work/repositories/dl_hpc_starter_pack/dist/tmp8uxa9cy0/dlhpcstarter-0.1.3.tar", last modified: Mon May  8 01:22:39 2023, max compression
+gzip compressed data, was "/datasets/work/hb-mlaifsp-mm/work/repositories/dl_hpc_starter_pack/dist/tmp6dg5neg_/dlhpcstarter-0.1.4.tar", last modified: Mon Jun 12 23:22:12 2023, max compression
```

## Comparing `dlhpcstarter-0.1.3.tar` & `dlhpcstarter-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    11558 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.3/LICENSE
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25288 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/PKG-INFO
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25540 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.3/README.md
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)       84 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.3/pyproject.toml
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)      807 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/setup.cfg
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)       96 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.3/setup.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/__init__.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     4612 2023-04-23 22:41:30.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/__main__.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     9743 2023-04-23 21:42:40.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/cluster.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     5681 2023-04-23 21:40:40.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/command_line_arguments.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/__init__.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/ext/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/ext/__init__.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     3215 2023-04-16 23:14:24.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/ext/collect_env_details.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/mods/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/mods/__init__.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     8505 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/tools/mods/logger.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)     9793 2023-04-26 01:07:26.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/trainer.py
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    11503 2023-04-24 00:26:55.000000 dlhpcstarter-0.1.3/src/dlhpcstarter/utils.py
-drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25288 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/PKG-INFO
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)      678 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/SOURCES.txt
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)        1 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/dependency_links.txt
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)       61 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/entry_points.txt
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)      201 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/requires.txt
--rw-r--r--   0 nic261   (1140141) hpc-users (319125)       13 2023-05-08 01:22:39.000000 dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/top_level.txt
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-06-12 23:22:12.000000 dlhpcstarter-0.1.4/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    11558 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.4/LICENSE
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25288 2023-06-12 23:22:12.000000 dlhpcstarter-0.1.4/PKG-INFO
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25540 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.4/README.md
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)       84 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.4/pyproject.toml
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)      807 2023-06-12 23:22:12.000000 dlhpcstarter-0.1.4/setup.cfg
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)       96 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.4/setup.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-06-12 23:22:11.000000 dlhpcstarter-0.1.4/src/
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-06-12 23:22:11.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/__init__.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     4612 2023-04-23 22:41:30.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/__main__.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     9589 2023-05-19 10:42:51.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/cluster.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     5681 2023-04-23 21:40:40.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/command_line_arguments.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-06-12 23:22:12.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/tools/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/tools/__init__.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-06-12 23:22:12.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/tools/ext/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/tools/ext/__init__.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     3215 2023-04-16 23:14:24.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/tools/ext/collect_env_details.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-06-12 23:22:12.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/tools/mods/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        0 2022-09-08 10:09:36.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/tools/mods/__init__.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)     8505 2023-03-30 09:11:54.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/tools/mods/logger.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    10269 2023-05-19 11:11:02.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/trainer.py
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    13760 2023-05-15 22:58:51.000000 dlhpcstarter-0.1.4/src/dlhpcstarter/utils.py
+drwxr-xr-x   0 nic261   (1140141) hpc-users (319125)        0 2023-06-12 23:22:12.000000 dlhpcstarter-0.1.4/src/dlhpcstarter.egg-info/
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)    25288 2023-06-12 23:22:11.000000 dlhpcstarter-0.1.4/src/dlhpcstarter.egg-info/PKG-INFO
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)      678 2023-06-12 23:22:11.000000 dlhpcstarter-0.1.4/src/dlhpcstarter.egg-info/SOURCES.txt
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)        1 2023-06-12 23:22:11.000000 dlhpcstarter-0.1.4/src/dlhpcstarter.egg-info/dependency_links.txt
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)       61 2023-06-12 23:22:11.000000 dlhpcstarter-0.1.4/src/dlhpcstarter.egg-info/entry_points.txt
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)      201 2023-06-12 23:22:11.000000 dlhpcstarter-0.1.4/src/dlhpcstarter.egg-info/requires.txt
+-rw-r--r--   0 nic261   (1140141) hpc-users (319125)       13 2023-06-12 23:22:11.000000 dlhpcstarter-0.1.4/src/dlhpcstarter.egg-info/top_level.txt
```

### Comparing `dlhpcstarter-0.1.3/LICENSE` & `dlhpcstarter-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.3/PKG-INFO` & `dlhpcstarter-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlhpcstarter
-Version: 0.1.3
+Version: 0.1.4
 Summary: Deep Learning and HPC Starter Pack
 Home-page: https://github.com/csiro-mlai/dl_hpc_starter_pack
 Author: CSIRO
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
```

### Comparing `dlhpcstarter-0.1.3/README.md` & `dlhpcstarter-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.3/setup.cfg` & `dlhpcstarter-0.1.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dlhpcstarter
-version = 0.1.3
+version = 0.1.4
 description = Deep Learning and HPC Starter Pack
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/csiro-mlai/dl_hpc_starter_pack
 author = CSIRO
 license = Apache License 2.0
 license_file = LICENSE
```

### Comparing `dlhpcstarter-0.1.3/src/dlhpcstarter/__main__.py` & `dlhpcstarter-0.1.4/src/dlhpcstarter/__main__.py`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.3/src/dlhpcstarter/cluster.py` & `dlhpcstarter-0.1.4/src/dlhpcstarter/cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -99,60 +99,60 @@
 
     def run(self):
         if self.resubmit:
             print('Setting signal to automatically requeue the job before timeout.')
             signal.signal(signal.SIGUSR1, self.sig_handler)
             signal.signal(signal.SIGTERM, self.term_handler)
         else:
-            print("Automatic requeuing has not been set. The job will not be requeued after timeout.")
+            print('Automatic requeuing has not been set. The job will not be requeued after timeout.')
         try:
             self.fnc(self.fnc_kwargs)
 
         except Exception as e:
             print('Caught exception in worker thread', e)
             traceback.print_exc()
             raise SystemExit
 
     def schedule_experiment(self, session):
-        timestamp = datetime.datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
-        timestamp = 'session_{}_{}'.format(session, timestamp)
+        timestamp = datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
+        timestamp = f'session_{session}_{timestamp}'
 
         # Generate and save cluster manager script
-        manager_cmd_script_path = os.path.join(self.manager_files_log_path, '{}.sh'.format(timestamp))
+        manager_cmd_script_path = os.path.join(self.manager_files_log_path, f'{timestamp}.sh')
         if self.manager == 'slurm':
             manager_cmd = self.build_slurm_command(manager_cmd_script_path, timestamp, session)
         else:
             raise ValueError(f'{self.manager} is not a valid manager.')
         self.save_manager_cmd(manager_cmd, manager_cmd_script_path)
 
         # Run script to launch job
         print('\nLaunching experiment...')
-        result = call('{} {}'.format(self.run_cmd[self.manager], manager_cmd_script_path), shell=True)
+        result = call(f'{self.run_cmd[self.manager]} {manager_cmd_script_path}', shell=True)
         if result == 0:
             print(f'Launched experiment {manager_cmd_script_path}.')
         else:
             print('Launch failed...')
 
     def call_resume(self):
         job_id = os.environ['SLURM_JOB_ID']
-        cmd = 'scontrol requeue {}'.format(job_id)
+        cmd = f'scontrol requeue {job_id}'
         print(f'\nRequeing job {job_id}...')
         result = call(cmd, shell=True)
         if result == 0:
             print(f'Requeued job {job_id}.')
         else:
             print('Requeue failed...')
         os._exit(0)
 
     def sig_handler(self, signum, frame):
-        print(f"Caught signal: {signum}")
+        print(f'Caught signal: {signum}')
         self.call_resume()
 
     def term_handler(self, signum, frame):
-        print("Bypassing sigterm.")
+        print('Bypassing sigterm.')
 
     def save_manager_cmd(self, manager_cmd, manager_cmd_script_path):
         with open(manager_cmd_script_path, mode='w') as file:
             file.write(manager_cmd)
 
     def get_max_session_number(self, path):
         files = os.listdir(path)
@@ -182,79 +182,80 @@
             if not os.path.exists(out_path):
                 os.makedirs(out_path)
             self.out_log_path = out_path
 
     def build_slurm_command(self, manager_cmd_script_path, timestamp, session):
 
         sub_commands = ['#!/bin/bash -l']
-        sub_commands.append('#SBATCH --job-name={}'.format('{}session_{}'.format(self.job_display_name, session)))
+        sub_commands.append(f'#SBATCH --job-name={self.job_display_name}session_{session}')
 
         if self.log_out:
-            out_path = os.path.join(self.out_log_path, '{}_%j.out'.format(timestamp))
-            sub_commands.append('#SBATCH --output={}'.format(out_path))
+            out_path = os.path.join(self.out_log_path, f'{timestamp}_%j.out')
+            sub_commands.append(f'#SBATCH --output={out_path}')
 
         if self.log_err:
-            err_path = os.path.join(self.err_log_path, '{}_%j.err'.format(timestamp))
-            sub_commands.append('#SBATCH --error={}'.format(err_path))
+            err_path = os.path.join(self.err_log_path, f'{timestamp}_%j.err')
+            sub_commands.append(f'#SBATCH --error={err_path}')
         sub_commands.append(f'#SBATCH --time={self.time_limit:s}')
 
-        if self.begin != "now":
-            sub_commands.append('#SBATCH --begin={}'.format(self.begin))
+        if self.begin != 'now':
+            sub_commands.append(f'#SBATCH --begin={self.begin}')
 
         if self.num_gpus:
-            sub_commands.append('#SBATCH --gres=gpu:{}'.format(self.num_gpus))
+            sub_commands.append(f'#SBATCH --gres=gpu:{self.num_gpus}')
 
         if self.num_workers > 0:
-            sub_commands.append('#SBATCH --cpus-per-task={}'.format(self.num_workers))
+            sub_commands.append(f'#SBATCH --cpus-per-task={self.num_workers}')
 
-        sub_commands.append('#SBATCH --nodes={}'.format(self.num_nodes))
-        sub_commands.append('#SBATCH --mem={}'.format(self.memory))
+        sub_commands.append(f'#SBATCH --nodes={self.num_nodes}')
+        sub_commands.append(f'#SBATCH --mem={self.memory}')
         sub_commands.append(f'#SBATCH --signal=USR1@{6 * 60}')
+        sub_commands.append(f'#SBATCH --open-mode=append')
 
         mail_type = []
         if self.notify_on_end:
             mail_type.append('END')
         if self.notify_on_fail:
             mail_type.append('FAIL')
         if len(mail_type) > 0 and self.email is not None:
-            sub_commands.append('#SBATCH --mail-type={}'.format(','.join(mail_type)))
-            sub_commands.append('#SBATCH --mail-user={}'.format(self.email))
+            sub_commands.append(f'#SBATCH --mail-type={",".join(mail_type)}')
+            sub_commands.append(f'#SBATCH --mail-user={self.email}')
 
         for (cmd, value) in self.manager_commands:
             if value:
-                sub_commands.append('#SBATCH --{}={}'.format(cmd, value))
+                sub_commands.append(f'#SBATCH --{cmd}={value}')
             else:
-                sub_commands.append('#SBATCH --{}'.format(cmd))
+                sub_commands.append(f'#SBATCH --{cmd}')
 
         sub_commands = [x.lstrip() for x in sub_commands]
 
         for cmd in self.commands:
             sub_commands.append(cmd)
 
         args_string = self.args_to_string(self.fnc_kwargs)
-        args_string = '{} --{} {}'.format(args_string, "slurm_cmd_path", manager_cmd_script_path)
+        args_string = f'{args_string} --slurm_cmd_path {manager_cmd_script_path}'
 
         if self.entrypoint:
             cmd = f'{self.entrypoint} {args_string}'
         else:
-            cmd = '{} {} {}'.format(self.python_cmd, self.script_name, args_string)
+            cmd = f'{self.python_cmd} {self.script_name} {args_string}'
         if not self.no_srun:
             cmd = 'srun ' + cmd
         sub_commands.append(cmd)
 
         return '\n'.join(sub_commands)
 
     def args_to_string(self, args):
         params = []
         for k, v in vars(args).items():
             if v is not None:
                 if self.escape(v):
-                    cmd = '--{} \"{}\"'.format(k, v)
+                    cmd = '--{k} \"{v}\"'
                 else:
-                    cmd = '--{} {}'.format(k, v)
+                    cmd = f'--{k} {v}'
                 params.append(cmd)
         return ' '.join(params)
 
     def escape(self, v):
         v = str(v)
         return '[' in v or ';' in v or ' ' in v
```

### Comparing `dlhpcstarter-0.1.3/src/dlhpcstarter/command_line_arguments.py` & `dlhpcstarter-0.1.4/src/dlhpcstarter/command_line_arguments.py`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.3/src/dlhpcstarter/tools/ext/collect_env_details.py` & `dlhpcstarter-0.1.4/src/dlhpcstarter/tools/ext/collect_env_details.py`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.3/src/dlhpcstarter/tools/mods/logger.py` & `dlhpcstarter-0.1.4/src/dlhpcstarter/tools/mods/logger.py`

 * *Files identical despite different names*

### Comparing `dlhpcstarter-0.1.3/src/dlhpcstarter/trainer.py` & `dlhpcstarter-0.1.4/src/dlhpcstarter/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from lightning.pytorch import Trainer
 from lightning.pytorch.callbacks import (EarlyStopping, LearningRateMonitor,
                                          ModelCheckpoint)
 from lightning.pytorch.loggers import NeptuneLogger
 from lightning.pytorch.loggers.csv_logs import CSVLogger
 from lightning.pytorch.loggers.tensorboard import TensorBoardLogger
+from lightning.pytorch.strategies import DeepSpeedStrategy
 
 logging.getLogger(
     "neptune.new.internal.operation_processors.async_operation_processor",
 ).setLevel(logging.CRITICAL)
 from lightning.pytorch.plugins.environments import SLURMEnvironment
 
 
@@ -89,22 +90,28 @@
         kwargs - keyword arguments for Trainer.
     """
     accumulate_grad_batches = None
     loggers = [] if loggers is None else loggers
     callbacks = [] if callbacks is None else callbacks
     plugins = [] if plugins is None else plugins
 
+    # Unsure if Lightning's SLURMEnvironment features fault-tolerant training:
     if submit:
-        # Unsure if Lightning's SLURMEnvironment features fault-tolerant training.
         plugins.append(SLURMEnvironment(auto_requeue=False))
 
     # Deepspeed has its own autocast capabilities:
-    if 'strategy' in kwargs and 'precision' in kwargs:
-        if 'deepspeed' in kwargs['strategy'] and kwargs['precision'] == 16:
-            raise ValueError('DeepSpeed and "precision=16" are incompatible as DeepSpeed has its own autocast functionality.')
+    # if 'strategy' in kwargs and 'precision' in kwargs:
+    #     if 'deepspeed' in kwargs['strategy'] and kwargs['precision'] == 16:
+    #         raise ValueError('DeepSpeed and "precision=16" are incompatible as DeepSpeed has its own autocast functionality.')
+
+    # DeepSpeed config:
+    if 'deepspeed_config' in kwargs:
+        kwargs['strategy'] = DeepSpeedStrategy(
+            **kwargs['deepspeed_config']
+        )
 
     # Loggers
     loggers.append(CSVLogger(exp_dir_trial))
     loggers.append(TensorBoardLogger(exp_dir_trial, default_hp_metric=False))
     if neptune_api_key is not None:
         custom_run_id = f'{config_name[:21]}_t_{trial}'
         assert len(custom_run_id) <= 32, '"custom_run_id" must be less than or equal to 32 characters'
@@ -141,16 +148,20 @@
                 save_top_k=save_top_k,
                 every_n_epochs=every_n_epochs,
                 filename='{epoch:d}-{step:d}-{' + monitor + ':f}' if monitor else '{epoch:d}-{step:d}',
                 save_last=True,
             )
         )
         if 'strategy' in kwargs:
-            if 'deepspeed_stage_3' in kwargs['strategy']: 
-                callbacks[-1].FILE_EXTENSION = ""
+            if isinstance(kwargs['strategy'], str):
+                if 'deepspeed_stage_3' in kwargs['strategy']: 
+                    callbacks[-1].FILE_EXTENSION = ""
+            elif isinstance(kwargs['strategy'], DeepSpeedStrategy):
+                if kwargs['deepspeed_config']['stage'] == 3:
+                    callbacks[-1].FILE_EXTENSION = ""
 
     # if every_n_train_steps:
     #     if resumable:
     #         raise ValueError('Cannot resume training from a checkpoint that ended before the epoch ended. Fault '
     #                          'tolerant training needs to be implemented for this: '
     #                          'https://pytorch-lightning.readthedocs.io/en/latest/clouds'
     #                          '/fault_tolerant_training_expert.html#enable-fault-tolerant-behavior-on-your-own-cluster')
```

### Comparing `dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/PKG-INFO` & `dlhpcstarter-0.1.4/src/dlhpcstarter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlhpcstarter
-Version: 0.1.3
+Version: 0.1.4
 Summary: Deep Learning and HPC Starter Pack
 Home-page: https://github.com/csiro-mlai/dl_hpc_starter_pack
 Author: CSIRO
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8
```

### Comparing `dlhpcstarter-0.1.3/src/dlhpcstarter.egg-info/SOURCES.txt` & `dlhpcstarter-0.1.4/src/dlhpcstarter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

