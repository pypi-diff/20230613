# Comparing `tmp/micro_trainer_transformers-0.0.2.tar.gz` & `tmp/micro_trainer_transformers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micro_trainer_transformers-0.0.2.tar", last modified: Tue May 16 12:03:58 2023, max compression
+gzip compressed data, was "micro_trainer_transformers-0.0.3.tar", last modified: Mon Jun 12 23:04:32 2023, max compression
```

## Comparing `micro_trainer_transformers-0.0.2.tar` & `micro_trainer_transformers-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-05-16 12:03:58.670513 micro_trainer_transformers-0.0.2/
--rw-rw-r--   0 joefox    (1000) joefox    (1000)      786 2023-05-16 12:03:58.670513 micro_trainer_transformers-0.0.2/PKG-INFO
--rw-rw-r--   0 joefox    (1000) joefox    (1000)      219 2023-05-09 13:47:07.000000 micro_trainer_transformers-0.0.2/README.md
-drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-05-16 12:03:58.670513 micro_trainer_transformers-0.0.2/micro_trainer_transformers/
--rw-rw-r--   0 joefox    (1000) joefox    (1000)      197 2023-05-01 21:14:11.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/__init__.py
--rw-rw-r--   0 joefox    (1000) joefox    (1000)    20528 2023-05-03 14:18:14.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/arguments.py
--rw-rw-r--   0 joefox    (1000) joefox    (1000)     7975 2023-05-16 11:28:00.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/core_args.py
--rw-rw-r--   0 joefox    (1000) joefox    (1000)    15197 2023-05-16 11:47:17.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/core_optim.py
--rw-rw-r--   0 joefox    (1000) joefox    (1000)    19353 2023-05-16 11:28:53.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/core_train.py
--rw-rw-r--   0 joefox    (1000) joefox    (1000)     2926 2023-05-01 20:45:05.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/trainer.py
--rw-rw-r--   0 joefox    (1000) joefox    (1000)     2285 2023-05-14 07:21:18.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/utils.py
-drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-05-16 12:03:58.670513 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/
--rw-rw-r--   0 joefox    (1000) joefox    (1000)      786 2023-05-16 12:03:58.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/PKG-INFO
--rw-rw-r--   0 joefox    (1000) joefox    (1000)      605 2023-05-16 12:03:58.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/SOURCES.txt
--rw-rw-r--   0 joefox    (1000) joefox    (1000)        1 2023-05-16 12:03:58.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/dependency_links.txt
--rw-rw-r--   0 joefox    (1000) joefox    (1000)       20 2023-05-16 12:03:58.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/entry_points.txt
--rw-rw-r--   0 joefox    (1000) joefox    (1000)       37 2023-05-16 12:03:58.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/requires.txt
--rw-rw-r--   0 joefox    (1000) joefox    (1000)       27 2023-05-16 12:03:58.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/top_level.txt
--rw-rw-r--   0 joefox    (1000) joefox    (1000)       79 2023-05-16 12:03:58.674513 micro_trainer_transformers-0.0.2/setup.cfg
--rw-rw-r--   0 joefox    (1000) joefox    (1000)      989 2023-05-12 19:02:04.000000 micro_trainer_transformers-0.0.2/setup.py
+drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-06-12 23:04:32.556986 micro_trainer_transformers-0.0.3/
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      786 2023-06-12 23:04:32.556986 micro_trainer_transformers-0.0.3/PKG-INFO
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      219 2023-05-09 13:47:07.000000 micro_trainer_transformers-0.0.3/README.md
+drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-06-12 23:04:32.552986 micro_trainer_transformers-0.0.3/micro_trainer_transformers/
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      197 2023-05-01 21:14:11.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers/__init__.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)    20528 2023-05-03 14:18:14.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers/arguments.py
+drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-06-12 23:04:32.556986 micro_trainer_transformers-0.0.3/micro_trainer_transformers/collators/
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       60 2023-06-12 22:17:48.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers/collators/__init__.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)     4303 2023-06-12 22:17:12.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers/collators/albert_collator.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)     8209 2023-06-12 23:01:48.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers/core_args.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)    15197 2023-05-16 11:47:17.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers/core_optim.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)    21504 2023-06-12 19:41:52.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers/core_train.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)     2926 2023-05-01 20:45:05.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers/trainer.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)     2285 2023-05-14 07:21:18.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers/utils.py
+drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-06-12 23:04:32.556986 micro_trainer_transformers-0.0.3/micro_trainer_transformers.egg-info/
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      786 2023-06-12 23:04:32.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers.egg-info/PKG-INFO
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      710 2023-06-12 23:04:32.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers.egg-info/SOURCES.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)        1 2023-06-12 23:04:32.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers.egg-info/dependency_links.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       20 2023-06-12 23:04:32.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers.egg-info/entry_points.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       40 2023-06-12 23:04:32.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers.egg-info/requires.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       27 2023-06-12 23:04:32.000000 micro_trainer_transformers-0.0.3/micro_trainer_transformers.egg-info/top_level.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       79 2023-06-12 23:04:32.556986 micro_trainer_transformers-0.0.3/setup.cfg
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      992 2023-06-12 23:03:11.000000 micro_trainer_transformers-0.0.3/setup.py
```

### Comparing `micro_trainer_transformers-0.0.2/PKG-INFO` & `micro_trainer_transformers-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micro_trainer_transformers
-Version: 0.0.2
+Version: 0.0.3
 Summary: Micro version train modules Transformers trainer....
 Home-page: https://github.com/utrobinmv/micro_trainer_transformers
 Author: Utrobin Mikhail
 Author-email: utrobinmv@yandex.ru
 License: Apache
 Description: Micro version train modules Transformers trainer....
```

### Comparing `micro_trainer_transformers-0.0.2/micro_trainer_transformers/arguments.py` & `micro_trainer_transformers-0.0.3/micro_trainer_transformers/arguments.py`

 * *Files identical despite different names*

### Comparing `micro_trainer_transformers-0.0.2/micro_trainer_transformers/core_args.py` & `micro_trainer_transformers-0.0.3/micro_trainer_transformers/core_args.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,19 +55,21 @@
     #log
     log_every_n_steps: int = 20
     
     #floating point
     tf32: Optional[bool] = None #Включить ли режим tf32, доступный в Ampere и более новых архитектурах GPU. Это экспериментальный API, и он может измениться.
     bf16: bool = False #Использовать ли точность bf16 (смешанную) вместо 32-битной. Требуется архитектура NVIDIA Ampere или выше или использование процессора (no_cuda). Это экспериментальный API, и он может измениться.
     fp16: bool = False #Использовать ли точность fp16 (смешанную) вместо 32-битной
+    torch_compile: bool = False #If set to `True`, модель будет завернута в `torch.compile`.
 
     #project    
     project_name: str = 'debug_classificate'
     model_master_name: str = 'linear_simple'
     model_comment: str = ''
+    root_path_checkpoint = '/checkpoints'
 
     
     def __init__(self):
         
         self.accum_param()
         self.change_dir()
 
@@ -90,20 +92,20 @@
 
     def change_dir(self):
         #not edit
         self.run_time: int = current_time_in_second()
         self.version: str = time_in_second_to_textdate(self.run_time)
         self.model_name: str = self.model_master_name + '_'+ self.version + ('_debug' if self.debug else '')
         
-        self.path_checkpoint: str = '/checkpoints/' + self.project_name + '/' + \
+        self.path_checkpoint: str = self.root_path_checkpoint + '/' + self.project_name + '/' + \
             self.version + '_' + \
             self.model_master_name  + ('_debug' if self.debug else '') + '/' 
             
         self.path_log: str = self.path_checkpoint + 'logs/'
-        self.path_best_model: str = '/checkpoints/save_models/'
+        self.path_best_model: str = self.root_path_checkpoint + '/save_models/'
         pass
 
     def from_hf_training_arguments(self, project_name: str, model_master_name: str, ta: TrainingArguments):
         self.project_name = project_name
         self.model_master_name = model_master_name
 
         #ignore parameters
@@ -133,14 +135,15 @@
         #Убрал так как метрика по умолчанию 'loss', а у меня 'valid_loss'
         # if ta.metric_for_best_model: 
         #     self.metric_monitor_name = ta.metric_for_best_model
 
         self.tf32 = ta.tf32
         self.bf16 = ta.bf16
         self.fp16 = ta.fp16
+        self.torch_compile = ta.torch_compile
         
         if ta.warmup_steps > 0:
             self.warmup_steps = ta.warmup_steps
         elif ta.warmup_ratio > 0:
             self.warmup_steps = int(ta.max_steps * ta.warmup_ratio)
 
         if ta.greater_is_better:
```

### Comparing `micro_trainer_transformers-0.0.2/micro_trainer_transformers/core_optim.py` & `micro_trainer_transformers-0.0.3/micro_trainer_transformers/core_optim.py`

 * *Files identical despite different names*

### Comparing `micro_trainer_transformers-0.0.2/micro_trainer_transformers/core_train.py` & `micro_trainer_transformers-0.0.3/micro_trainer_transformers/core_train.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         self.data_collator = data_collator
         self.compute_metrics_fn = compute_metrics
         
         self.loss_fn = self.training_params.loss_fn
         
         self.pbar_train = tqdm(desc='Total training model',leave=True,position=2) 
         
-        self.train_mode_start = False 
+        self.train_mode_start = False
+        self.save_first_valid_batch = False
+        self.first_valid_batch = None
 
     def setup(self, stage=None):
         pass
 
     def prepare_data(self):
         pass
 
@@ -290,14 +292,18 @@
     ) -> torch.Tensor:
         
         if isinstance(batch, dict):
             batch_size = len(batch[list(batch.keys())[0]])
         else:
             batch_size = len(batch["labels"])
             
+        if self.save_first_valid_batch:
+           self.first_valid_batch = batch
+           self.save_first_valid_batch = False
+            
         loss = self.common_step(batch, batch_idx, valid = True)
         
         self.log("valid_loss", loss, on_step=False, 
                  on_epoch=True, prog_bar=True, 
                  batch_size=batch_size)
 
     def on_validation_epoch_start(self):
@@ -397,62 +403,120 @@
             max_train_kwargs = {'max_steps': max_train_steps}
 
         precision = 32
         if self.training_params.bf16:
             precision = "bf16"
         elif self.training_params.fp16:
             precision = 16
-        
+
+        if self.training_params.tf32:
+            torch.backends.cuda.matmul.allow_tf32 = True # allow tf32 on matmul
+            torch.backends.cudnn.allow_tf32 = True # allow tf32 on cudnn
+
+        if self.training_params.torch_compile:
+            print("compiling the model... (takes a ~minute)")
+            #unoptimized_model = model
+            self.model = torch.compile(self.model) # requires PyTorch 2.0            
+
         #, max_steps=max_train_steps
         self.trainer = pl.Trainer(accelerator="auto", devices="auto", 
                 **max_train_kwargs,
+                precision=precision,
                 val_check_interval=val_check_interval,
                 accumulate_grad_batches=self.training_params.gradient_accumulation_steps,
                 check_val_every_n_epoch=check_val_every_n_epoch,
                 default_root_dir=self.training_params.path_best_model,
                 logger=loggers,
                 gradient_clip_val=self.training_params.max_grad_norm,
                 callbacks=callbacks,
                 reload_dataloaders_every_n_epochs = 1 if self.training_params.data_streaming_train else 0,
                 limit_val_batches = self.training_params.limit_val_batches,
                 log_every_n_steps = self.training_params.log_every_n_steps,
                 num_sanity_val_steps=2,
                 )
 
-    def model_vis(self):
+    def model_vis_save(self):
+        '''
+        Сохраняет визуализацию сетки
+        '''
+        
+        self.create_trainer()
+        
+        self.trainer.num_sanity_val_steps = 0
+        self.trainer.limit_train_batches = 0
+        self.trainer.limit_val_batches = 1
+        
+        self.save_first_valid_batch = True
+        
+        self.trainer.validate(self,ckpt_path=None)
+        
         #https://github.com/mert-kurttutan/torchview
         from torchview import draw_graph
+        import os.path
 
-        model_graph = draw_graph(
-            SimpleRNN(), input_size=(2, 3),
-            graph_name='RecursiveNet',
-            roll=True
-        )
-        model_graph.visual_graph        
+        print('=======================')
+        print('Run save graph model:', self.training_params.path_log)
+        
+        old_size = 0
+        for depth in range(100):
+
+            save_name = 'model_'+self.training_params.model_master_name+'_depth_' + str(depth)
+
+            _ = draw_graph(
+                self.model, self.first_valid_batch,
+                graph_name=save_name,
+                depth=depth,
+                save_graph=True,
+                filename=self.training_params.path_log + save_name,
+            )
+
+            real_filename = self.training_params.path_log + save_name+'.png'
+
+            new_size = os.path.getsize(real_filename)
+
+            if new_size == old_size:
+                break
+
+            old_size = new_size
+            
+            print('Save graphviz: ',real_filename)  
 
     def lr_find(self,):
+        '''
+        Проводит поиск learning rate и возвращает оптимальное значение lr
+        
+        Кроме этого делает print
+        и сохраняет график поиска learning rate в папку self.training_params.path_log
+        
+        '''
+        
+        
         self.create_trainer(mode = 'lr_find')
         
         self.train_mode_start = False
         
         lr_finder = self.trainer.tuner.lr_find(self, self.train_dataloader())
         
         #print(lr_finder.results)
         
+        lr_recomend = lr_finder.suggestion()
+        
         print('=======================')
-        print('Recomended lr:', lr_finder.suggestion())
+        print('Recomended lr:', lr_recomend)
         
         fig = lr_finder.plot(suggest=True) # Plot
         fig.show()
         
         save_log_filename = self.training_params.path_log + 'find_lr.jpg'        
         fig.savefig(save_log_filename) 
         
         print('Save image plot result to:', save_log_filename)
         
+        return lr_recomend
+        
     def fit(self,resume_from_checkpoint=None):
         
         self.create_trainer()
 
         save_useful_info(self.training_params.path_log,self.model,self.training_params.__dict__, self.trainer.__dict__)
 
         self.trainer.fit(self,ckpt_path=resume_from_checkpoint)
```

### Comparing `micro_trainer_transformers-0.0.2/micro_trainer_transformers/trainer.py` & `micro_trainer_transformers-0.0.3/micro_trainer_transformers/trainer.py`

 * *Files identical despite different names*

### Comparing `micro_trainer_transformers-0.0.2/micro_trainer_transformers/utils.py` & `micro_trainer_transformers-0.0.3/micro_trainer_transformers/utils.py`

 * *Files identical despite different names*

### Comparing `micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/PKG-INFO` & `micro_trainer_transformers-0.0.3/micro_trainer_transformers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micro-trainer-transformers
-Version: 0.0.2
+Version: 0.0.3
 Summary: Micro version train modules Transformers trainer....
 Home-page: https://github.com/utrobinmv/micro_trainer_transformers
 Author: Utrobin Mikhail
 Author-email: utrobinmv@yandex.ru
 License: Apache
 Description: Micro version train modules Transformers trainer....
```

### Comparing `micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/SOURCES.txt` & `micro_trainer_transformers-0.0.3/micro_trainer_transformers.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -9,8 +9,10 @@
 micro_trainer_transformers/trainer.py
 micro_trainer_transformers/utils.py
 micro_trainer_transformers.egg-info/PKG-INFO
 micro_trainer_transformers.egg-info/SOURCES.txt
 micro_trainer_transformers.egg-info/dependency_links.txt
 micro_trainer_transformers.egg-info/entry_points.txt
 micro_trainer_transformers.egg-info/requires.txt
-micro_trainer_transformers.egg-info/top_level.txt
+micro_trainer_transformers.egg-info/top_level.txt
+micro_trainer_transformers/collators/__init__.py
+micro_trainer_transformers/collators/albert_collator.py
```

### Comparing `micro_trainer_transformers-0.0.2/setup.py` & `micro_trainer_transformers-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 if os.path.exists("README.md"):
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
 
 setuptools.setup(
     name="micro_trainer_transformers",
-    version="0.0.2",
+    version="0.0.3",
     author="Utrobin Mikhail",
     author_email="utrobinmv@yandex.ru",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/utrobinmv/micro_trainer_transformers",
     packages=setuptools.find_packages(),
     license="Apache",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=['pytorch-lightning<2.0','torch','datasets'],
+    install_requires=['pytorch-lightning<=1.9.5','torch','datasets'],
     entry_points={
         "console_scripts": []
     }
 )
```

