# Comparing `tmp/panml-1.0.4.tar.gz` & `tmp/panml-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-1.0.4.tar", last modified: Sun Jun 11 23:54:53 2023, max compression
+gzip compressed data, was "panml-1.0.5.tar", last modified: Tue Jun 13 12:17:58 2023, max compression
```

## Comparing `panml-1.0.4.tar` & `panml-1.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 23:54:53.229612 panml-1.0.4/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-1.0.4/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-11 23:54:53.229876 panml-1.0.4/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-1.0.4/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 23:54:53.222976 panml-1.0.4/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-1.0.4/panml/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 23:54:53.225399 panml-1.0.4/panml/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.4/panml/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-06-08 13:09:32.000000 panml-1.0.4/panml/clustering/faiss.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     5841 2023-06-08 13:09:32.000000 panml-1.0.4/panml/constants.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     1749 2023-06-08 13:09:32.000000 panml-1.0.4/panml/environments.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 23:54:53.226875 panml-1.0.4/panml/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.4/panml/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    24206 2023-06-11 00:54:36.000000 panml-1.0.4/panml/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    15604 2023-06-11 23:54:12.000000 panml-1.0.4/panml/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2739 2023-06-11 00:13:19.000000 panml-1.0.4/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     2451 2023-06-08 13:09:32.000000 panml-1.0.4/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 23:54:53.224777 panml-1.0.4/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-11 23:54:53.000000 panml-1.0.4/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      442 2023-06-11 23:54:53.000000 panml-1.0.4/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-11 23:54:53.000000 panml-1.0.4/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-11 23:54:53.000000 panml-1.0.4/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-11 23:54:53.000000 panml-1.0.4/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-11 23:54:53.230605 panml-1.0.4/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2406 2023-06-11 23:54:12.000000 panml-1.0.4/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-11 23:54:53.228330 panml-1.0.4/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-06-07 05:36:34.000000 panml-1.0.4/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-1.0.4/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-13 12:17:58.634343 panml-1.0.5/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-1.0.5/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-13 12:17:58.634773 panml-1.0.5/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13498 2023-06-05 12:56:17.000000 panml-1.0.5/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-13 12:17:58.625393 panml-1.0.5/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-1.0.5/panml/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-13 12:17:58.628113 panml-1.0.5/panml/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.5/panml/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-06-08 13:09:32.000000 panml-1.0.5/panml/clustering/faiss.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     5841 2023-06-08 13:09:32.000000 panml-1.0.5/panml/constants.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1749 2023-06-08 13:09:32.000000 panml-1.0.5/panml/environments.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-13 12:17:58.630118 panml-1.0.5/panml/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-06-08 13:09:32.000000 panml-1.0.5/panml/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    24488 2023-06-13 12:17:33.000000 panml-1.0.5/panml/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    15604 2023-06-11 23:54:12.000000 panml-1.0.5/panml/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2739 2023-06-11 00:13:19.000000 panml-1.0.5/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2451 2023-06-08 13:09:32.000000 panml-1.0.5/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-13 12:17:58.627248 panml-1.0.5/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)    14676 2023-06-13 12:17:58.000000 panml-1.0.5/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      442 2023-06-13 12:17:58.000000 panml-1.0.5/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-06-13 12:17:58.000000 panml-1.0.5/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      227 2023-06-13 12:17:58.000000 panml-1.0.5/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-06-13 12:17:58.000000 panml-1.0.5/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-06-13 12:17:58.635806 panml-1.0.5/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2406 2023-06-13 12:17:33.000000 panml-1.0.5/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-06-13 12:17:58.632817 panml-1.0.5/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-06-07 05:36:34.000000 panml-1.0.5/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-1.0.5/test/test_VectorEngine.py
```

### Comparing `panml-1.0.4/LICENSE` & `panml-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-1.0.4/PKG-INFO` & `panml-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 1.0.4
+Version: 1.0.5
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-1.0.4/README.md` & `panml-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `panml-1.0.4/panml/clustering/faiss.py` & `panml-1.0.5/panml/clustering/faiss.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.4/panml/constants.py` & `panml-1.0.5/panml/constants.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.4/panml/environments.py` & `panml-1.0.5/panml/environments.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.4/panml/llm/huggingface.py` & `panml-1.0.5/panml/llm/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,50 +59,58 @@
                     try:
                         if torch.backends.mps.is_available():
                             self.device = 'mps'
                         else:
                             print('CUDA (GPU support) is not available')
                     except:
                         print('CUDA (GPU support) is not available')
-        print(f'Model processing is set on {self.device.upper()}')
 
         # Set model
         if source == 'huggingface':
             if 'flan' in self.model_name:
                 self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.model_name, **model_args)
             elif 'bert' in self.model_name:
                 self.model_hf = AutoModelForMaskedLM.from_pretrained(self.model_name, **model_args)
             else:
                 self.model_hf = AutoModelForCausalLM.from_pretrained(self.model_name, **model_args)
         elif source == 'local':
             if load_peft_lora:
                 # Set LoRA trained model
                 self.peft_config = PeftConfig.from_pretrained(self.model_name)
-                if 'flan' in self.model_name:
-                    self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.peft_config.base_model_name_or_path, **model_args, local_files_only=True)
-                elif 'bert' in self.model_name:
-                    self.model_hf = AutoModelForMaskedLM.from_pretrained(self.peft_config.base_model_name_or_path, **model_args, local_files_only=True)
+                if 'flan' in self.peft_config.base_model_name_or_path:
+                    self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.peft_config.base_model_name_or_path, **model_args)
+                elif 'bert' in self.peft_config.base_model_name_or_path:
+                    self.model_hf = AutoModelForMaskedLM.from_pretrained(self.peft_config.base_model_name_or_path, **model_args)
                 else:
-                    self.model_hf = AutoModelForCausalLM.from_pretrained(self.peft_config.base_model_name_or_path, **model_args, local_files_only=True)
-                self.model_hf = PeftModel.from_pretrained(self.model_hf, self.peft_config)
+                    self.model_hf = AutoModelForCausalLM.from_pretrained(self.peft_config.base_model_name_or_path, **model_args)
+                self.model_hf = PeftModel.from_pretrained(self.model_hf, self.model_name)
             else:
                 # Set non-LoRA trained model
                 if 'flan' in self.model_name:
                     self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
                 elif 'bert' in self.model_name:
                     self.model_hf = AutoModelForMaskedLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
                 else:
                     self.model_hf = AutoModelForCausalLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
         
+        # Display model properties
+        # CPU/GPU setup, max context tokens for the model
+        max_context_tokens_msg = ''
+        try:
+            max_context_tokens_msg = f"Max context tokens length: {self.model_hf.config.n_positions}"
+        except:
+            pass
+        print(f"Model processing is set on {self.device.upper()}. {max_context_tokens_msg}")
+
         # Set tokenizer
         if load_peft_lora:
-            # Set LoRA trained model's tokenizer
+            # Get tokenizer name from peft base model
             self.tokenizer = AutoTokenizer.from_pretrained(self.peft_config.base_model_name_or_path)
         else:
-            # Set non-LoRA trained model's tokenizer
+            # Get non-LoRA trained model's tokenizer
             if self.model_hf.config.tokenizer_class:
                 self.tokenizer = AutoTokenizer.from_pretrained(self.model_hf.config.tokenizer_class.lower().replace('tokenizer', ''), mirror='https://huggingface.co')
             else:
                 self.tokenizer = AutoTokenizer.from_pretrained(self.model_name, mirror='https://huggingface.co')
         self.tokenizer.pad_token = '[PAD]' # set padding token
         try:
             self.tokenizer.deprecation_warnings["Asking-to-pad-a-fast-tokenizer"] = True # turn off warning for fast tokenizer as we are tokenizing data before training
@@ -176,16 +184,16 @@
         probability: token probabilities if available
         perplexity: perplexity score if available
         '''
         output_context = {
             'text': None
         }
         
-        input_ids = self.tokenizer.encode(text, return_tensors='pt').to(torch.device(self.device))
-        output = self.model_hf.generate(input_ids, 
+        input_batch = self.tokenizer(text, return_tensors='pt').to(torch.device(self.device))
+        output = self.model_hf.generate(**input_batch, 
                                         max_length=max_length,
                                         pad_token_id=self.model_hf.config.eos_token_id,
                                         num_return_sequences=num_return_sequences, 
                                         temperature=temperature,
                                         top_p=top_p,
                                         top_k=top_k,
                                         no_repeat_ngram_size=no_repeat_ngram_size,
@@ -374,15 +382,15 @@
                 optim=train_args['optimizer'], # model optimisation function
                 num_train_epochs=train_args['num_train_epochs'], # total number of training epochs
                 per_device_train_batch_size=train_args['per_device_train_batch_size'],  # batch size per device during training
                 per_device_eval_batch_size=train_args['per_device_eval_batch_size'],   # batch size for evaluation
                 warmup_steps=train_args['warmup_steps'], # number of warmup steps for learning rate scheduler
                 weight_decay=train_args['weight_decay'], # strength of weight decay
                 logging_steps=train_args['logging_steps'],
-                output_dir=train_args['output_dir'], # output directory
+                output_dir='./results', # output directory
                 logging_dir=train_args['logging_dir'], # log directory
             )
 
             trainer = Seq2SeqTrainer(
                 model=self.model_hf,
                 args=training_args,
                 train_dataset=tokenized_data.remove_columns(['text']),
@@ -413,22 +421,22 @@
                 model=self.model_hf,
                 args=training_args,
                 train_dataset=tokenized_data.remove_columns(['text']),
                 eval_dataset=tokenized_data.remove_columns(['text']),
                 data_collator=data_collator,
             )
 
-        trainer.train() # Execute training
+        trainer.train() # execute training
 
         print('Getting evaluations...')
         self.evaluation_result = trainer.evaluate() # save evaluation result
         
         if train_args['save_model']:
-            trainer.save_model(f'./results/model_{train_args["title"]}') # save trained model
-            self.tokenizer._tokenizer.save(f'./results/model_{train_args["title"]}/tokenizer.json') # save tokenizer
+            self.model_hf.save_pretrained(f'{train_args["output_dir"]}/model_{train_args["title"]}') # save model
+            self.tokenizer._tokenizer.save(f'{train_args["output_dir"]}/model_{train_args["title"]}/tokenizer.json') # save tokenizer
 
         print('Task completed')
         
     # Save model
     def save(self, save_dir: str=None) -> None:
         '''
         Save the model on demand
@@ -437,9 +445,9 @@
         save_dir: relative path of the file. If directory is not provided, the default directory is set to ".results/model_<model_name>"
 
         Returns:
         None. File is saved at the specified location
         '''
         if save_dir is None:
             save_dir = f'./results/model_{self.model_name}'
-        self.model_hf.save_pretrained(save_dir) # save model
-        self.tokenizer._tokenizer.save(f'{save_dir}/tokenizer.json') # save tokenizer
+        self.model_hf.save_pretrained(save_dir)
+        self.tokenizer._tokenizer.save(f'{save_dir}/tokenizer.json')
```

### Comparing `panml-1.0.4/panml/llm/openai.py` & `panml-1.0.5/panml/llm/openai.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.4/panml/models.py` & `panml-1.0.5/panml/models.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.4/panml/search.py` & `panml-1.0.5/panml/search.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.4/panml.egg-info/PKG-INFO` & `panml-1.0.5/panml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 1.0.4
+Version: 1.0.5
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-1.0.4/setup.py` & `panml-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '1.0.4', # version
+  version = '1.0.5', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'PanML team', # team name
   author_email = 'teampanml@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
```

### Comparing `panml-1.0.4/test/test_ModelPack.py` & `panml-1.0.5/test/test_ModelPack.py`

 * *Files identical despite different names*

### Comparing `panml-1.0.4/test/test_VectorEngine.py` & `panml-1.0.5/test/test_VectorEngine.py`

 * *Files identical despite different names*

