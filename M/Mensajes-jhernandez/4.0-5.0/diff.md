# Comparing `tmp/Mensajes-jhernandez-4.0.tar.gz` & `tmp/Mensajes-jhernandez-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mensajes-jhernandez-4.0.tar", last modified: Tue Jun 13 16:08:38 2023, max compression
+gzip compressed data, was "Mensajes-jhernandez-5.0.tar", last modified: Tue Jun 13 17:39:06 2023, max compression
```

## Comparing `Mensajes-jhernandez-4.0.tar` & `Mensajes-jhernandez-5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 16:08:38.324697 Mensajes-jhernandez-4.0/
--rw-rw-rw-   0        0        0     1219 2023-06-13 15:57:45.000000 Mensajes-jhernandez-4.0/LICENSE
--rw-rw-rw-   0        0        0      166 2023-06-13 15:58:04.000000 Mensajes-jhernandez-4.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-13 16:08:38.299257 Mensajes-jhernandez-4.0/Mensajes_jhernandez.egg-info/
--rw-rw-rw-   0        0        0      581 2023-06-13 16:08:38.000000 Mensajes-jhernandez-4.0/Mensajes_jhernandez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2023-06-13 16:08:38.000000 Mensajes-jhernandez-4.0/Mensajes_jhernandez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 16:08:38.000000 Mensajes-jhernandez-4.0/Mensajes_jhernandez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 16:08:38.000000 Mensajes-jhernandez-4.0/Mensajes_jhernandez.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-13 16:08:38.000000 Mensajes-jhernandez-4.0/Mensajes_jhernandez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      581 2023-06-13 16:08:38.323697 Mensajes-jhernandez-4.0/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-06-13 15:57:50.000000 Mensajes-jhernandez-4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 16:08:38.306247 Mensajes-jhernandez-4.0/mensajes/
--rw-rw-rw-   0        0        0       37 2023-04-01 22:51:13.000000 Mensajes-jhernandez-4.0/mensajes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:08:38.312246 Mensajes-jhernandez-4.0/mensajes/adios/
--rw-rw-rw-   0        0        0       46 2023-04-01 22:58:19.000000 Mensajes-jhernandez-4.0/mensajes/adios/__init__.py
--rw-rw-rw-   0        0        0      257 2023-04-01 23:17:24.000000 Mensajes-jhernandez-4.0/mensajes/adios/despedidas.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:08:38.319306 Mensajes-jhernandez-4.0/mensajes/hola/
--rw-rw-rw-   0        0        0       45 2023-04-01 22:54:25.000000 Mensajes-jhernandez-4.0/mensajes/hola/__init__.py
--rw-rw-rw-   0        0        0      744 2023-06-12 15:14:58.000000 Mensajes-jhernandez-4.0/mensajes/hola/saludos.py
--rw-rw-rw-   0        0        0       63 2023-06-13 15:58:09.000000 Mensajes-jhernandez-4.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 16:08:38.325705 Mensajes-jhernandez-4.0/setup.cfg
--rw-rw-rw-   0        0        0     4152 2023-06-13 16:08:11.000000 Mensajes-jhernandez-4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 16:08:38.322697 Mensajes-jhernandez-4.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:58:00.000000 Mensajes-jhernandez-4.0/tests/__init__.py
--rw-rw-rw-   0        0        0      638 2023-06-13 15:57:55.000000 Mensajes-jhernandez-4.0/tests/test_hola.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:39:06.468071 Mensajes-jhernandez-5.0/
+-rw-rw-rw-   0        0        0     1219 2023-06-13 15:57:45.000000 Mensajes-jhernandez-5.0/LICENSE
+-rw-rw-rw-   0        0        0      166 2023-06-13 15:58:04.000000 Mensajes-jhernandez-5.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-13 17:39:06.441184 Mensajes-jhernandez-5.0/Mensajes_jhernandez.egg-info/
+-rw-rw-rw-   0        0        0      581 2023-06-13 17:39:06.000000 Mensajes-jhernandez-5.0/Mensajes_jhernandez.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-06-13 17:39:06.000000 Mensajes-jhernandez-5.0/Mensajes_jhernandez.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:39:06.000000 Mensajes-jhernandez-5.0/Mensajes_jhernandez.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-13 17:39:06.000000 Mensajes-jhernandez-5.0/Mensajes_jhernandez.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-13 17:39:06.000000 Mensajes-jhernandez-5.0/Mensajes_jhernandez.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      581 2023-06-13 17:39:06.467068 Mensajes-jhernandez-5.0/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-06-13 16:29:04.000000 Mensajes-jhernandez-5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 17:39:06.443365 Mensajes-jhernandez-5.0/mensajes/
+-rw-rw-rw-   0        0        0       37 2023-04-01 22:51:13.000000 Mensajes-jhernandez-5.0/mensajes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:39:06.452066 Mensajes-jhernandez-5.0/mensajes/adios/
+-rw-rw-rw-   0        0        0       46 2023-04-01 22:58:19.000000 Mensajes-jhernandez-5.0/mensajes/adios/__init__.py
+-rw-rw-rw-   0        0        0      257 2023-04-01 23:17:24.000000 Mensajes-jhernandez-5.0/mensajes/adios/despedidas.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:39:06.458586 Mensajes-jhernandez-5.0/mensajes/hola/
+-rw-rw-rw-   0        0        0       45 2023-04-01 22:54:25.000000 Mensajes-jhernandez-5.0/mensajes/hola/__init__.py
+-rw-rw-rw-   0        0        0      747 2023-06-13 17:37:58.000000 Mensajes-jhernandez-5.0/mensajes/hola/saludos.py
+-rw-rw-rw-   0        0        0       63 2023-06-13 15:58:09.000000 Mensajes-jhernandez-5.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:39:06.468071 Mensajes-jhernandez-5.0/setup.cfg
+-rw-rw-rw-   0        0        0     4858 2023-06-13 17:38:33.000000 Mensajes-jhernandez-5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:39:06.462583 Mensajes-jhernandez-5.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:58:00.000000 Mensajes-jhernandez-5.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      638 2023-06-13 15:57:55.000000 Mensajes-jhernandez-5.0/tests/test_hola.py
```

### Comparing `Mensajes-jhernandez-4.0/LICENSE` & `Mensajes-jhernandez-5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Mensajes-jhernandez-4.0/Mensajes_jhernandez.egg-info/PKG-INFO` & `Mensajes-jhernandez-5.0/Mensajes_jhernandez.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-jhernandez
-Version: 4.0
+Version: 5.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.jesus.dev
 Author: Jesús Hernández Marcial
 Author-email: jesus@jesus.dev
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Mensajes-jhernandez-4.0/PKG-INFO` & `Mensajes-jhernandez-5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-jhernandez
-Version: 4.0
+Version: 5.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.jesus.dev
 Author: Jesús Hernández Marcial
 Author-email: jesus@jesus.dev
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Mensajes-jhernandez-4.0/mensajes/hola/saludos.py` & `Mensajes-jhernandez-5.0/mensajes/hola/saludos.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np # esto solo después de que se intala pip install numpy
 
 def saludar():
     print("Hola, te saludo desde saludos.saludar()")
 
 def prueba():
-    print("Esto es una prueba desde saludos.prueba()")
+    print("Esto es una prueba de la nueva versión 6.0.")
 
 #esto es nuevo para lo de distribución
 def generar_array(numeros): #creará un arreglo por medio de numpy
     return np.arange(numeros) #el arange nos da un rango 
     
 
 def qpw():
```

### Comparing `Mensajes-jhernandez-4.0/setup.py` & `Mensajes-jhernandez-5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,18 +31,19 @@
 #para que se ejecuten 
 
 #como transformar nuestro paquete local en un paquete para publicar en internet en pypi.org
 #nossotros lo publicaremos en test.pypi.org 
 
 setup(
     name="Mensajes-jhernandez", #primero cambiamos el nombre porque es uno común 
-    version='4.0', #vambiamos la versión  y debemos crear una descripcion en el readme.md+
+    version='5.0', #vambiamos la versión  y debemos crear una descripcion en el readme.md+
     long_descriptcion =  open('README.md').read(), # con el readme creado lo abrimos con este método
    
-    long_description_content_type= 'text/markdown',
+    long_description_content_type= 'text/markdown', # esto fue para evitar el error de hace rato
+    #ahora ya no marca errores al hacer el build y el twine check dist/*
 
     #se aplica el método read() falta algo pero lo creamos despues
     description='Un paquete para saludar y despedir',
     author='Jesús Hernández Marcial',
     author_email='jesus@jesus.dev',
     url='https://www.jesus.dev',
     license_files= ['LICENSE'],  ##creamos nuestra licencia que llamará al archivo licence que crearemos
@@ -73,7 +74,20 @@
 #pip install build twine --upgrade esto se tiene que instalar para armar todo el paquete 
 #una vez instalado eso se coloca python -m build para instalar el paquete esto tiene que ser en donde
 # #est´s el arhivo a instalar 
 #ahora para checar que todos los paquetes estén correctamente instalados
 #python -m twine check dist/*   $borramos los tar. gz que no ocupemos 
 
 #al usar lo anterior  se genera un long descriptionerro por el open .read que s e usao
+
+#una vez haciendo lo del long descrition type 
+#si tenemos los paquetes que queremos subir en el dist hacemos lo siguiente 
+#python -m twine upload -r testpypi dist/*
+
+
+#se revisa en la liga que te dieron y ahí estatá el modulo instalado
+# lo instalamos con el comando indicado y revisamos con pip list si est´s en el sistema
+# despues desisntalamos con pip uninstall el nomrbe de lo que querramos desistalar 
+
+#también desinstalamos los repositorios que se opcuparon como numpy
+#ahora subiremos al respositorio oficial usando lo siguiente
+#python -m twine upload dist/*
```

### Comparing `Mensajes-jhernandez-4.0/tests/test_hola.py` & `Mensajes-jhernandez-5.0/tests/test_hola.py`

 * *Files identical despite different names*

