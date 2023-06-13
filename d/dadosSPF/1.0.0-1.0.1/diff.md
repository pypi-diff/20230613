# Comparing `tmp/dadosSPF-1.0.0.tar.gz` & `tmp/dadosSPF-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dadosSPF-1.0.0.tar", last modified: Mon May 15 15:03:48 2023, max compression
+gzip compressed data, was "dist/dadosSPF-1.0.1.tar", last modified: Tue Jun 13 13:23:37 2023, max compression
```

## Comparing `dadosSPF-1.0.0.tar` & `dadosSPF-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-05-15 15:03:48.000000 dadosSPF-1.0.0/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1287 2023-05-15 15:03:48.000000 dadosSPF-1.0.0/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      767 2023-05-15 15:01:34.000000 dadosSPF-1.0.0/README.md
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-05-15 15:03:48.000000 dadosSPF-1.0.0/dadosSPF/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-05-15 14:50:31.000000 dadosSPF-1.0.0/dadosSPF/__init__.py
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)    34322 2023-05-15 14:54:25.000000 dadosSPF-1.0.0/dadosSPF/dadosSPF.py
-drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-05-15 15:03:48.000000 dadosSPF-1.0.0/dadosSPF.egg-info/
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1287 2023-05-15 15:03:47.000000 dadosSPF-1.0.0/dadosSPF.egg-info/PKG-INFO
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      219 2023-05-15 15:03:48.000000 dadosSPF-1.0.0/dadosSPF.egg-info/SOURCES.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-05-15 15:03:47.000000 dadosSPF-1.0.0/dadosSPF.egg-info/dependency_links.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-05-15 15:03:47.000000 dadosSPF-1.0.0/dadosSPF.egg-info/requires.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-05-15 15:03:47.000000 dadosSPF-1.0.0/dadosSPF.egg-info/top_level.txt
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2023-05-15 15:03:48.000000 dadosSPF-1.0.0/setup.cfg
--rw-r--r--   0 cdsw      (8536) cdsw      (8536)      533 2023-05-15 15:03:43.000000 dadosSPF-1.0.0/setup.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1309 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      781 2023-06-13 13:23:21.000000 dadosSPF-1.0.1/README.md
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-06-13 13:21:19.000000 dadosSPF-1.0.1/dadosSPF/__init__.py
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)    37006 2023-06-13 13:21:19.000000 dadosSPF-1.0.1/dadosSPF/dadosSPF.py
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/
+drwxr-sr-x   0 cdsw      (8536) cdsw      (8536)        0 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1328 2023-06-13 13:22:55.000000 dadosSPF-1.0.1/dadosSPF.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      219 2023-06-13 13:21:19.000000 dadosSPF-1.0.1/dadosSPF.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       33 2023-06-13 13:22:59.000000 dadosSPF-1.0.1/dadosSPF.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-06-13 13:21:19.000000 dadosSPF-1.0.1/dadosSPF.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)     1309 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/PKG-INFO
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      459 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/SOURCES.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        1 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/dependency_links.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       23 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/requires.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)        9 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/dadosSPF.egg-info/top_level.txt
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)       38 2023-06-13 13:23:37.000000 dadosSPF-1.0.1/setup.cfg
+-rw-r--r--   0 cdsw      (8536) cdsw      (8536)      533 2023-06-13 13:23:28.000000 dadosSPF-1.0.1/setup.py
```

### Comparing `dadosSPF-1.0.0/PKG-INFO` & `dadosSPF-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
         
         ## Getting Started
         #### Dependencies
-        Você precisa do Python 3.7 ou posterior para usar safraPyFunctions.
+        Você precisa do Python 3.7 ou posterior para usar dadosSPF.
         Você pode encontrá-lo em [python.org] (https://www.python.org/).
         Você precisa do PySpark 2.4.7 para usar safraPyFunctions.
         Você pode encontrá-lo em [spark.apache.org] (https://spark.apache.org/docs/latest/api/python/).
         
         You also need pandas, holidays and impyla packages, which is available from [PyPI](https://pypi.org). If you have pip, just run:
         '''
         pip install pandas
         pip install holidays
         pip install impyla
+        pip install unidecode
         '''
         #### Installation
         Clone this repo to your local machine using:
         '''
         git clone https://gitlab.com.br/dados-migracao/dadosSPF
         '''
```

### Comparing `dadosSPF-1.0.0/README.md` & `dadosSPF-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # dadosSPF
 
 ## Getting Started
 #### Dependencies
-Você precisa do Python 3.7 ou posterior para usar safraPyFunctions.
+Você precisa do Python 3.7 ou posterior para usar dadosSPF.
 Você pode encontrá-lo em [python.org] (https://www.python.org/).
 Você precisa do PySpark 2.4.7 para usar safraPyFunctions.
 Você pode encontrá-lo em [spark.apache.org] (https://spark.apache.org/docs/latest/api/python/).
 
 You also need pandas, holidays and impyla packages, which is available from [PyPI](https://pypi.org). If you have pip, just run:
 '''
 pip install pandas
 pip install holidays
 pip install impyla
+pip install unidecode
 '''
 #### Installation
 Clone this repo to your local machine using:
 '''
 git clone https://gitlab.com.br/dados-migracao/dadosSPF
 '''
```

### Comparing `dadosSPF-1.0.0/dadosSPF/dadosSPF.py` & `dadosSPF-1.0.1/dadosSPF/dadosSPF.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 __author__ =     "CARLOS PIVETA"
 __collaborators__ = "CARLOS PIVETA"
 __license__ =    "DADOS"
-__version__ =    "1.0.0"
+__version__ =    "1.0.1"
 __maintainer__ = "CARLOS PIVETA"
 __status__ =     "Production"
 
 import os
 import re
 import sys
 import glob
 import shutil
 import zipfile
 import logging
 import warnings
 import holidays
 import pandas as pd
+from unidecode import unidecode
 from impala.dbapi import connect
 from impala.util import as_pandas
 from pyspark.sql import SQLContext
 from pyspark.sql import SparkSession
 from pyspark.sql.types import StringType
 from datetime import date,datetime,timedelta
 from pyspark.sql import Row, functions as spf
@@ -610,67 +611,74 @@
         caminhoArquivo str
             caminho onde será armazenado o csv
         nomeArquivo str
             nome do arquivo a ser salvo
         
         """
         
+        if caminhoArquivo== None:
+            sys.exit('Pasta não Encontrada')
+            
         if caminhoArquivo[-1] != '/':
             caminhoArquivo = caminhoArquivo+'/'
+        
+        if not os.path.isdir(caminhoArquivo):       
+            os.makedirs(caminhoArquivo)
+        
         hora = str(datetime.now()+timedelta(hours=-3)).replace('-','').replace(':','').replace(' ','_')[:15]
         arquivo = "{}{}_{}.csv".format(caminhoArquivo,nomeArquivo,hora)
         try:
             if tpDf.upper() == 'SPARK':
                     df.coalesce(1).write.option('header', 'True').format('csv').save(arquivo)
             elif tpDf.upper() == 'PANDAS':
                     df.to_csv(arquivo, sep=';')
             else:
                 raise ValueError("ERRO! Formato NÃO suportado !!!")
             print("csv {} salvo !!!".format(nomeArquivo))   
         except Exception as e:
             print("ERRO! csv {} NÃO salvo !!!".format(nomeArquivo))
             print(e)
     
-    def replaceTbQuery(self,vQuery,vTabelas,limit_dev = 'limit 100'):
-        list_tables = vTabelas.upper().split(",")
-        for tb in list_tables:
-            nmTb = tb.split(".")[1]
-            if (self.environment == "DEV"):
-                tbName = self.sandbox+"."+tb.split(".")[1];
-            else:
-                tbName=tb;
-            vQuery = vQuery.replace(nmTb,nmTb.lower());
-            vQuery = vQuery.replace(tb.lower(),tbName);  
-            vQuery = vQuery.replace(tb.lower(),tbName.lower());  
-            vQuery = vQuery.replace(tb,tbName);
-        if(vQuery.lower().find("select")>=0):
-            vQuery = vQuery+" "+limit_dev
-        return vQuery;
-    
-    def SaveFileProces(self,DF_INSERT,vTable,vEtapa,paths3):
-        """
-        Função utilizada pelo time de CRM
-        """
-        pos = len(vTable.split("_"))-1
-        contexto = vTable.split("_")[pos]
-        etapa = "0"+vEtapa+"_"+contexto.upper()
-        pathFile ="{0}_{1}/parquet_tmp/{2}/".format(paths3,contexto,etapa)
-        DF_INSERT\
-         .write\
-         .format("parquet")\
-         .mode("overwrite")\
-         .save(pathFile)
-        print(f"Arquivo salvo em: {pathFile}");
-    
-    def CheckPoint(self,df,table,paths3):
-        pathTable = "{0}/temp/{1}/".format(paths3,table)
-        self.spark.sparkContext.setCheckpointDir(pathTable)
-        df = df.checkpoint()
-        df.createOrReplaceTempView(table)
-        return df
+#     def replaceTbQuery(self,vQuery,vTabelas,limit_dev = 'limit 100'):
+#         list_tables = vTabelas.upper().split(",")
+#         for tb in list_tables:
+#             nmTb = tb.split(".")[1]
+#             if (self.environment == "DEV"):
+#                 tbName = self.sandbox+"."+tb.split(".")[1];
+#             else:
+#                 tbName=tb;
+#             vQuery = vQuery.replace(nmTb,nmTb.lower());
+#             vQuery = vQuery.replace(tb.lower(),tbName);  
+#             vQuery = vQuery.replace(tb.lower(),tbName.lower());  
+#             vQuery = vQuery.replace(tb,tbName);
+#         if(vQuery.lower().find("select")>=0):
+#             vQuery = vQuery+" "+limit_dev
+#         return vQuery;
+    
+#     def SaveFileProces(self,DF_INSERT,vTable,vEtapa,paths3):
+#         """
+#         Função utilizada pelo time de CRM
+#         """
+#         pos = len(vTable.split("_"))-1
+#         contexto = vTable.split("_")[pos]
+#         etapa = "0"+vEtapa+"_"+contexto.upper()
+#         pathFile ="{0}_{1}/parquet_tmp/{2}/".format(paths3,contexto,etapa)
+#         DF_INSERT\
+#          .write\
+#          .format("parquet")\
+#          .mode("overwrite")\
+#          .save(pathFile)
+#         print(f"Arquivo salvo em: {pathFile}");
+    
+#     def CheckPoint(self,df,table,paths3):
+#         pathTable = "{0}/temp/{1}/".format(paths3,table)
+#         self.spark.sparkContext.setCheckpointDir(pathTable)
+#         df = df.checkpoint()
+#         df.createOrReplaceTempView(table)
+#         return df
     
     def SetNullToString(self,df):
         """
         df2 = sc.SetNullToString(df)
 
         Função para alterar os valores Null para a string ''
 
@@ -680,39 +688,84 @@
             dataframe o qual será convertido
 
         """
         ##Converte todos os campos em String e nome das colunas tudo em CAIXA ALTA
         df = df.select([spf.when(spf.col(x).cast(StringType()).isNull(),spf.lit("")).otherwise(spf.concat(spf.lit('"'),spf.col(x), spf.lit('"')).cast(StringType())).alias(x.upper()) for x in df.columns])
         return df
 
-    def csvToSandbox(self,pasta = './arquivos/',delimiter = ';',header = 'true' ):
+    def csvToSandbox(self,pasta = './arquivos/',delimiter = None,header = 'true' ):
+        """
+        s.csvToSandbox(self,pasta = './arquivos/',delimiter = None,header = 'true' )
+        
+        Função para carregar arquivos de texte em um dataframe no sandbox
+        
+        Parameters
+        ----------
+        pasta str
+            caminho onde está armazenado o csv
+        delimiter str
+            campo delimitador do csv, caso seja None ele tentará usar ';' e ','
+        header str
+            Marcação se o arquivo tem cabeçalho ou não (sempre em minusculo)
+        
+        """
         spark = self.getSpark()
 
         if pasta[-1] != '/':
             pasta = pasta + '/'
 
         if os.path.isdir(pasta) == False:
             sys.exit('Pasta não Encontrada')
 
         if not os.path.isdir(pasta+'carregados/'):       
             os.makedirs(pasta+'carregados/')
 
         list_of_files = glob.glob(pasta+'*.csv')
         if len(list_of_files) > 0:
             for file in list_of_files:
+                move = False
                 try:
                     arq = file.replace(pasta,'')
-                    nm = arq.replace('.csv','')
-                    df_Carga = spark.read.option("delimiter", ";").option("header", "true").csv(pasta+arq)
+                    nm = unidecode(arq.replace('.csv','').replace(' ','_').replace('(','').replace(')',''))
+                    if delimiter == None:
+                        df_Carga = spark.read.option("delimiter", ';').option("header", "true").csv(pasta+arq)
+                        if len(df_Carga.columns) == 1:
+                            df_Carga = spark.read.option("delimiter", ',').option("header", "true").csv(pasta+arq)
+                    else:
+                        df_Carga = spark.read.option("delimiter", delimiter).option("header", "true").csv(pasta+arq)
+                        
+                    df_Carga = self.setColumnsUp(df_Carga)
+                    for i in df_Carga.columns:
+                        if i[0] == '_':
+                            df_Carga = df_Carga.withColumnRenamed(i, i[1:])
+                            i = i[1:]
+                        df_Carga = df_Carga.withColumnRenamed(i, unidecode(i))
+                    
+                    df_cols = df_Carga.columns
+
+                    # INDEX DAS COLUNAS DUPLICADAS
+                    duplicate_col_index = [idx for idx,
+                                           val in enumerate(df_cols) if val in df_cols[:idx]]
+
+                    # CRIANDO LISDA DAS DUPLICADAS
+                    for i in duplicate_col_index:
+                        df_cols[i] = df_cols[i] + '_'+ str(i)
+                    
+                    # RENAME
+                    df_Carga = df_Carga.toDF(*df_cols)
+                    df_Carga = df_Carga.select([spf.col(col).alias(re.sub("[^0-9a-zA-Z$]+","",col)) for col in df_Carga.columns])
                     self.saveSandbox(df_Carga,nm)
+                    move = True
                     del df_Carga
-                    shutil.move(file, pasta+'carregados/'+arq)
                 except Exception as e:
                     print('ERRO!!! Arquivo {} NÃO carregado'.format(file))
+                    move = False
                     print(e)
+                if move == True:
+                    shutil.move(file, pasta+'carregados/'+arq)
         else:
             print('Sem arquivos para serem carregados')
             
 # -------------------------------------------------------------------------------------------------------------------------------
 # | CLASS TOOLS
 # -------------------------------------------------------------------------------------------------------------------------------
 
@@ -825,21 +878,30 @@
             
     def zipFolder(self,strPasta = './pastaorigem/' ,strSaida = './nomepasta/nomearquivodestino'):
         try:
             shutil.make_archive(strSaida, 'zip', strPasta)
         except Exception as e:
             print('ERRO! AO COMPACTAR A PASTA')
             print(e)
+            
+    def zipFile(self, arquivo,pasta):
+        if pasta[-1] != '/':
+            pasta = pasta + '/'
+        with zipfile.ZipFile(f"{arquivo}.zip", mode="w") as archive:
+            archive.write(pasta+arquivo)
     
     def unzipFile(self,arquivo ="file.zip", pasta = 'targetdir'):
+        if pasta[-1] != '/':
+            pasta = pasta + '/'
         try:
-            with zipfile.ZipFile("file.zip","r") as zip_ref:
-                zip_ref.extractall("targetdir")
+            with zipfile.ZipFile(arquivo,"r") as zip_ref:
+                zip_ref.extractall(pasta)
         except Exception as e:
             print('ERRO! AO EXTRAIR O ARQUIVO')
             print(e)
+    
                                 
 # -------------------------------------------------------------------------------------------------------------------------------
 # | EASY IMPORTS
 # -------------------------------------------------------------------------------------------------------------------------------                                
 sqlConn =  conn()
 tools = tool()
```

### Comparing `dadosSPF-1.0.0/dadosSPF.egg-info/PKG-INFO` & `dadosSPF-1.0.1/dadosSPF.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: dadosSPF
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pacote de funções uteis para o desenvolvimento na cloudera
 Home-page: https://gitlab.com.br/dadosSPF
 Author: Carlos Piveta
 Author-email: cepo496@gmail.com
 License: MIT License
 Description: # dadosSPF
         
         ## Getting Started
         #### Dependencies
-        Você precisa do Python 3.7 ou posterior para usar safraPyFunctions.
+        Você precisa do Python 3.7 ou posterior para usar dadosSPF.
         Você pode encontrá-lo em [python.org] (https://www.python.org/).
         Você precisa do PySpark 2.4.7 para usar safraPyFunctions.
         Você pode encontrá-lo em [spark.apache.org] (https://spark.apache.org/docs/latest/api/python/).
         
         You also need pandas, holidays and impyla packages, which is available from [PyPI](https://pypi.org). If you have pip, just run:
         '''
         pip install pandas
         pip install holidays
         pip install impyla
+        pip install unidecode
         '''
         #### Installation
         Clone this repo to your local machine using:
         '''
         git clone https://gitlab.com.br/dados-migracao/dadosSPF
         '''
```

### Comparing `dadosSPF-1.0.0/setup.py` & `dadosSPF-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(
     name='dadosSPF',
-    version='1.0.0',
+    version='1.0.1',
     url='https://gitlab.com.br/dadosSPF',
     license='MIT License',
     author='Carlos Piveta',
 	long_description=readme,
     long_description_content_type="text/markdown",
     author_email='cepo496@gmail.com',
     keywords='Pacote',
```

