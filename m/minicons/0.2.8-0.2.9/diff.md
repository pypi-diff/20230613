# Comparing `tmp/minicons-0.2.8.tar.gz` & `tmp/minicons-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minicons-0.2.8.tar", max compression
+gzip compressed data, was "minicons-0.2.9.tar", max compression
```

## Comparing `minicons-0.2.8.tar` & `minicons-0.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2020-11-17 20:25:09.485643 minicons-0.2.8/LICENSE
--rw-r--r--   0        0        0     3745 2022-07-01 21:57:10.221101 minicons-0.2.8/README.md
--rw-r--r--   0        0        0       22 2022-10-19 00:13:32.863573 minicons-0.2.8/minicons/__init__.py
--rw-r--r--   0        0        0        0 2021-12-10 06:02:25.181372 minicons-0.2.8/minicons/bin/__init__.py
--rw-r--r--   0        0        0     7665 2022-06-05 01:09:59.830091 minicons-0.2.8/minicons/bin/score_cli.py
--rw-r--r--   0        0        0        0 2021-12-14 23:46:05.106830 minicons-0.2.8/minicons/bin/sentence_score_cli.py
--rw-r--r--   0        0        0    13909 2022-10-19 00:13:36.233226 minicons-0.2.8/minicons/cwe.py
--rw-r--r--   0        0        0    67812 2022-07-01 21:57:10.222589 minicons-0.2.8/minicons/scorer.py
--rw-r--r--   0        0        0     3058 2021-03-18 18:15:17.719568 minicons-0.2.8/minicons/supervised.py
--rw-r--r--   0        0        0     3046 2022-06-05 00:49:28.863753 minicons-0.2.8/minicons/utils.py
--rw-r--r--   0        0        0      868 2022-10-19 00:13:30.855288 minicons-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     4808 2022-10-19 00:13:47.036273 minicons-0.2.8/setup.py
--rw-r--r--   0        0        0     4562 2022-10-19 00:13:47.036682 minicons-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2020-11-17 20:25:09.485643 minicons-0.2.9/LICENSE
+-rw-r--r--   0        0        0     3745 2022-07-01 21:57:10.221101 minicons-0.2.9/README.md
+-rw-r--r--   0        0        0       22 2022-10-19 00:19:30.847733 minicons-0.2.9/minicons/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-10 06:02:25.181372 minicons-0.2.9/minicons/bin/__init__.py
+-rw-r--r--   0        0        0     7665 2022-06-05 01:09:59.830091 minicons-0.2.9/minicons/bin/score_cli.py
+-rw-r--r--   0        0        0        0 2021-12-14 23:46:05.106830 minicons-0.2.9/minicons/bin/sentence_score_cli.py
+-rw-r--r--   0        0        0    13965 2022-10-19 00:19:23.470514 minicons-0.2.9/minicons/cwe.py
+-rw-r--r--   0        0        0    67812 2022-07-01 21:57:10.222589 minicons-0.2.9/minicons/scorer.py
+-rw-r--r--   0        0        0     3058 2021-03-18 18:15:17.719568 minicons-0.2.9/minicons/supervised.py
+-rw-r--r--   0        0        0     3046 2022-06-05 00:49:28.863753 minicons-0.2.9/minicons/utils.py
+-rw-r--r--   0        0        0      868 2022-10-19 00:19:27.426642 minicons-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4808 2022-10-19 00:19:46.238456 minicons-0.2.9/setup.py
+-rw-r--r--   0        0        0     4562 2022-10-19 00:19:46.238882 minicons-0.2.9/PKG-INFO
```

### Comparing `minicons-0.2.8/LICENSE` & `minicons-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `minicons-0.2.8/README.md` & `minicons-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `minicons-0.2.8/minicons/bin/score_cli.py` & `minicons-0.2.9/minicons/bin/score_cli.py`

 * *Files identical despite different names*

### Comparing `minicons-0.2.8/minicons/cwe.py` & `minicons-0.2.9/minicons/cwe.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,18 +72,19 @@
 
         # Encode sentence into ids stored in the model's embedding layer(s).
         encoded = self.tokenizer(sentences, padding = 'longest', return_tensors="pt")
         encoded = encoded.to(self.device)
 
         input_ids = encoded['input_ids']
         attention_mask = encoded['attention_mask'].unsqueeze(-1)
-        # if 'cuda' in self.device:
-        #     attention_mask = attention_mask.cpu()
+        if 'cuda' in self.device:
+            attention_mask = attention_mask.cpu()
 
         if layer == 'static' or layer == 'pre':
+            attention_mask = attention_mask.to(self.device)
             hidden_states = [self.model.embeddings.word_embeddings.weight.detach()[i] for i in input_ids]
             hidden_states = torch.stack(hidden_states)
             hidden_states = hidden_states * attention_mask
         else:
         # Compute hidden states for the sentence for the given layer.
             output = self.model(**encoded)
```

### Comparing `minicons-0.2.8/minicons/scorer.py` & `minicons-0.2.9/minicons/scorer.py`

 * *Files identical despite different names*

### Comparing `minicons-0.2.8/minicons/supervised.py` & `minicons-0.2.9/minicons/supervised.py`

 * *Files identical despite different names*

### Comparing `minicons-0.2.8/minicons/utils.py` & `minicons-0.2.9/minicons/utils.py`

 * *Files identical despite different names*

### Comparing `minicons-0.2.8/pyproject.toml` & `minicons-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "minicons"
-version = "0.2.8"
+version = "0.2.9"
 description = "A package of useful functions to analyze transformer based language models."
 authors = ["Kanishka Misra <kmisra@purdue.edu>", "Aaron Mueller <amueller@jhu.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kanishkamisra/minicons"
 repository = "https://github.com/kanishkamisra/minicons"
 keywords = ["transformers", "language models", "nlp", "interpretability"]
```

### Comparing `minicons-0.2.8/setup.py` & `minicons-0.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'urllib3>=1.26.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['minicons = minicons.bin.score_cli:process']}
 
 setup_kwargs = {
     'name': 'minicons',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'A package of useful functions to analyze transformer based language models.',
     'long_description': '# minicons: Enabling Flexible Behavioral and Representational Analyses of Transformer Language Models\n\n[![Downloads](https://static.pepy.tech/personalized-badge/minicons?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/minicons)\n\nThis repo is a wrapper around the `transformers` [library](https://huggingface.co/transformers) from hugging face :hugs:\n\n<!-- TODO: Description-->\n\n\n\n## Installation\n\nInstall from Pypi using:\n\n```pip install minicons```\n\n## Supported Functionality\n\n- Extract word representations from Contextualized Word Embeddings\n- Score sequences using language model scoring techniques, including masked language models following [Salazar et al. (2020)](https://www.aclweb.org/anthology/2020.acl-main.240.pdf).\n\n\n## Examples\n\n1. Extract word representations from contextualized word embeddings:\n\n```py\nfrom minicons import cwe\n\nmodel = cwe.CWE(\'bert-base-uncased\')\n\ncontext_words = [("I went to the bank to withdraw money.", "bank"), \n                 ("i was at the bank of the river ganga!", "bank")]\n\nprint(model.extract_representation(context_words, layer = 12))\n\n\'\'\' \ntensor([[ 0.5399, -0.2461, -0.0968,  ..., -0.4670, -0.5312, -0.0549],\n        [-0.8258, -0.4308,  0.2744,  ..., -0.5987, -0.6984,  0.2087]],\n       grad_fn=<MeanBackward1>)\n\'\'\'\n```\n\n2. Compute sentence acceptability measures (surprisals) using Word Prediction Models:\n\n```py\nfrom minicons import scorer\n\nmlm_model = scorer.MaskedLMScorer(\'bert-base-uncased\', \'cpu\')\nilm_model = scorer.IncrementalLMScorer(\'distilgpt2\', \'cpu\')\ns2s_model = scorer.Seq2SeqScorer(\'t5-base\', \'cpu\')\n\nstimuli = ["The keys to the cabinet are on the table.",\n           "The keys to the cabinet is on the table."]\n\n# use sequence_score with different reduction options: \n# Sequence Surprisal - lambda x: -x.sum(0).item()\n# Sequence Log-probability - lambda x: x.sum(0).item()\n# Sequence Surprisal, normalized by number of tokens - lambda x: -x.mean(0).item()\n# Sequence Log-probability, normalized by number of tokens - lambda x: x.mean(0).item()\n# and so on...\n\nprint(ilm_model.sequence_score(stimuli, reduction = lambda x: -x.sum(0).item()))\n\n\'\'\'\n[39.879737854003906, 42.75846481323242]\n\'\'\'\n\n# MLM scoring, inspired by Salazar et al., 2020\nprint(mlm_model.sequence_score(stimuli, reduction = lambda x: -x.sum(0).item()))\n\'\'\'\n[13.962685585021973, 23.415111541748047]\n\'\'\'\n\n# Seq2seq scoring\n## Blank source sequence, target sequence specified in `stimuli`\nprint(s2s_model.sequence_score(stimuli, source_format = \'blank\')\n## Source sequence is the same as the target sequence in `stimuli`\nprint(s2s_model.sequence_score(stimuli, source_format = \'copy\')\n\'\'\'\n[-7.910910129547119, -7.835635185241699]\n[-10.555519104003906, -9.532546997070312]\n\'\'\'\n```\n\n## Tutorials\n\n- [Introduction to using LM-scoring methods using minicons](https://kanishka.xyz/post/minicons-running-large-scale-behavioral-analyses-on-transformer-lms/)\n- [Computing sentence and token surprisals using minicons](examples/surprisals.md)\n- [Extracting word/phrase representations using minicons](examples/word_representations.md)\n\n## Recent Updates\n- **November 6, 2021:** MLM scoring has been fixed! You can now use `model.token_score()` and `model.sequence_score()` with `MaskedLMScorers` as well!\n- **June 4, 2022:** Added support for Seq2seq models. Thanks to [Aaron Mueller](https://github.com/aaronmueller) 🥳\n\n## Citation\n\nIf you use `minicons`, please cite the following paper:\n\n```tex\n@article{misra2022minicons,\n    title={minicons: Enabling Flexible Behavioral and Representational Analyses of Transformer Language Models},\n    author={Kanishka Misra},\n    journal={arXiv preprint arXiv:2203.13112},\n    year={2022}\n}\n```\n',
     'author': 'Kanishka Misra',
     'author_email': 'kmisra@purdue.edu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/kanishkamisra/minicons',
```

### Comparing `minicons-0.2.8/PKG-INFO` & `minicons-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minicons
-Version: 0.2.8
+Version: 0.2.9
 Summary: A package of useful functions to analyze transformer based language models.
 Home-page: https://github.com/kanishkamisra/minicons
 License: MIT
 Keywords: transformers,language models,nlp,interpretability
 Author: Kanishka Misra
 Author-email: kmisra@purdue.edu
 Requires-Python: >=3.7.1,<4
```

