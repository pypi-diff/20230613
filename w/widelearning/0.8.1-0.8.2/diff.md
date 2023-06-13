# Comparing `tmp/widelearning-0.8.1.tar.gz` & `tmp/widelearning-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widelearning-0.8.1.tar", max compression
+gzip compressed data, was "widelearning-0.8.2.tar", max compression
```

## Comparing `widelearning-0.8.1.tar` & `widelearning-0.8.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1979 2023-05-27 13:49:07.193982 widelearning-0.8.1/README.md
--rw-r--r--   0        0        0      398 2023-05-27 15:44:42.462114 widelearning-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    84289 2023-05-27 15:37:36.521245 widelearning-0.8.1/widelearning.py
--rw-r--r--   0        0        0     2502 2023-05-27 15:44:52.152811 widelearning-0.8.1/setup.py
--rw-r--r--   0        0        0     2618 2023-05-27 15:44:52.153128 widelearning-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    26878 2023-06-13 02:58:21.703305 widelearning-0.8.2/README.md
+-rw-r--r--   0        0        0      398 2023-06-13 03:01:56.550675 widelearning-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0   101719 2023-06-13 02:56:07.080027 widelearning-0.8.2/widelearning.py
+-rw-r--r--   0        0        0    27864 2023-06-13 03:02:20.788100 widelearning-0.8.2/setup.py
+-rw-r--r--   0        0        0    27517 2023-06-13 03:02:20.789262 widelearning-0.8.2/PKG-INFO
```

### Comparing `widelearning-0.8.1/widelearning.py` & `widelearning-0.8.2/widelearning.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,16 +4,32 @@
 import os
 import shutil
 import glob
 import math as m
 import requests
 import csv
 
-# 1.  
 def txt_kernel(file_path):	
+    '''
+    Функция преобразования сгенерированного ядра для вставки в структуру TensorFlow 
+    (для черно-белых, одноканальных изображений)
+
+    Параметры
+    ----------
+    file_path : str
+        путь к текстовому файлу, содержащему сверточное ядро, записанное в следующем виде 
+        (с запятыми в конце каждой строки):
+        1,2,3,
+        4,5,6,
+        7,8,9,
+
+    Пример использования:
+    wdl.txt_kernel('horizontal.txt')
+
+    '''
     f = open(file_path, 'r')
 	
     weights = []
 
     for i in f:
         weights.append(i.strip().split(','))
 
@@ -25,16 +41,34 @@
             ii[i1] = [[int(elem)]]
             
     with open('kernel.txt', 'w') as file:
         file.write(str(weights))
 
     return weights 
 
-# 2.
 def add_kernel(path, init_kernel):
+    '''
+    Функция позволяет устанавливать дополнительные ядра сверточного слоя к уже установленным исходным
+    (для черно-белых, одноканальных изображений)
+
+    Параметры
+    ----------
+    path : str
+        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра, 
+        добавляемого к исходным
+    init_kernel : list
+        значения исходного/ых ядер, к которым происходит добавление. 
+        Это может быть либо переменная, которой присвоено значение исходных ядер, 
+        либо сами значения, полученные после преобразования с помощью функции txt_kernel:
+        [[[[1]], [[2]], [[3]]], [[[4]], [[5]], [[6]]], [[[7]], [[8]], [[9]]]].
+
+    Пример использования:
+    wdl.add_kernel('vertical.txt', w1)
+
+    '''
     ff = open(path, 'r')
     
     w1 = init_kernel
 
     weights = []
 
     for i in ff:
@@ -52,48 +86,87 @@
             w1[i][j][0].append(weights[i][j])
 
     with open('kernel.txt', 'w') as file:
         file.write(str(w1))
         
     return w1
 
-# 3.    
-# horizontal(32, [-7,-5,-3,-1,1,3,5,7])
 def horizontal(dim, values):
+    '''
+    Функция для генерации линейного сверточного ядра горизонтального типа
+
+    Параметры
+    ----------
+    dim : int
+        размерность генерируемой матрицы 
+    values : list
+        список значений, которые будут использоваться для заполнения матрицы.
+
+    Пример использования:
+    wdl.horizontal(32, [-7,-5,-3,-1,1,3,5,7])
+
+    '''
     horizontal = []
     for i in range(dim):
         row = []
         for j in range(dim):
             row.append(values[i % len(values)])
         horizontal.append(row)
         
     with open('horizontal.txt', 'w') as f:
         for row in horizontal:
             f.write(','.join(str(x) for x in row) + ',\n')
     return horizontal
 
-# 4.
-# vertical(32, [-7,-5,-3,-1,1,3,5,7])	
 def vertical(dim, values):
+    '''
+    Функция для генерации линейного сверточного ядра вертикального типа
+
+    Параметры
+    ----------
+    dim : int
+        размерность генерируемой матрицы 
+    values : list
+        список значений, которые будут использоваться для заполнения матрицы.
+
+    Пример использования:
+    wdl.vertical(32, [-7,-5,-3,-1,1,3,5,7])
+
+    '''
     vertical = []
     for i in range(dim):
         row = []
         for j in range(dim):
             row.append(values[j % len(values)])
         vertical.append(row)
         
     with open('vertical.txt', 'w') as f:    
         for row in vertical:
             f.write(','.join(str(x) for x in row) + ',\n')
     return vertical
-
-# 5.
-# diagonal([-7, -5, -3, -1], [1, 3, 5, 7], 1, 32)	
+	
 def diagonal(up, down, d, dimension):
+    '''
+    Функция для генерации линейного сверточного ядра диагонального типа
+
+    Parameters
+    ----------
+    up : list
+        список значений, которые будут размещены над диагональю выходной матрицы
+    down : list
+        список значений, которые будут размещены ниже диагонали
+    d : int
+        значение, из которого состоит диагональ.
+    dimension : int
+        размерность генерируемого ядра
 
+    Пример использования:
+    wdl.diagonal([-7, -5, -3, -1], [1, 3, 5, 7], 1, 32)	
+
+    '''
     matrix = [[0 for i in range(dimension)] for j in range(dimension)] 
     for i in range(dimension):
         for j in range(dimension):
             if i == j: 
                 matrix[i][j] = d
             elif i < j: 
                 matrix[i][j] = up[(j-i-1) % len(up)]
@@ -111,33 +184,65 @@
     with open('diagonal2.txt', 'w') as file:
         for i in matrix2:
             for j in i:
                 file.write(str(j) + ',')
             file.write('\n')
     
     return matrix
-
-# 6.     
+    
 def show_kernel(N, name):
+    '''
+    Функция вывода коэффициентов сверточного ядра на экран пользователя
+
+    Параметры
+    ----------
+    N : int
+        номер слоя, для которого необходимо вывести значения весовых коэффициентов
+    name : object
+        объект модели нейронной сети
+        название переменной, которой присвоена структура модели
 
+    Пример использования:
+    wdl.show_kernel(0, model)
+
+    '''
     ff = name.layers[N].get_weights()
 
     for nn in range(len(ff[0][0][0][0])):
       print('\n' + f'Номер сверточного ядра: {nn}')
       for kk in range(len(ff[0][0][0])):
         print(f'-----------ЦВЕТОВОЙ КАНАЛ №{kk}-----------')
         for i in range(len(ff[0])):
           for j in range(len(ff[0][i])):
             print(ff[0][i][j][kk][nn], end=',')
           print()
         print('\n')
-
-# 7.        
+      
 def txt_kernel_rgb(k1, k2, k3): 
+    '''
+    Функция преобразования сгенерированного ядра для вставки в структуру TensorFlow 
+    (для цветных, трехканальных изображений)
+    
+    Параметры
+    ----------
+    k1 : str
+        путь к текстовому файлу, содержащему сверточное ядро первого цветового канала R, записанное в следующем виде 
+        (с запятыми в конце каждой строки):
+        1,2,3,
+        4,5,6,
+        7,8,9,
+    k2 : str
+        путь к текстовому файлу, содержащему сверточное ядро второго цветового канала G
+    k3 : str
+        путь к текстовому файлу, содержащему сверточное ядро третьего цветового канала B
 
+    Пример использования:
+    wdl.txt_kernel_rgb('k1.txt', 'k2.txt', 'k3.txt')
+
+    '''
     f1 = open(k1, 'r')
     f2 = open(k2, 'r')
     f3 = open(k3, 'r')
 	
     w1 = []
 
     for i in f1:
@@ -179,19 +284,49 @@
 
     for i in range(len(w1[0])):
         for j in range(len(w1[0])):
             w1[i][j].append(w3[i][j])
 			
     return w1
 
-#w1 = txt_kernel_rgb('k1.txt', 'k2.txt', 'k3.txt')
-
-# 8. 
 def add_kernel_rgb(k1, k2, k3, w):
+    '''
+    Функция позволяет устанавливать дополнительные ядра сверточного слоя к уже установленным исходным
+    (для цветных, трехканальных изображений)
+
+    Параметры
+    ----------
+    path : str
+        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра, 
+        добавляемого к исходным
+    init_kernel : list
+        значения исходного/ых ядер, к которым происходит добавление. 
+        Это может быть либо переменная, которой присвоено значение исходных ядер, 
+        либо сами значения, полученные после преобразования с помощью функции txt_kernel_rgb
+
+    Параметры
+    ----------
+    k1 : str
+        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра первого цветового канала R, 
+        добавляемого к исходным в данном цветовом канале
+    k2 : str
+        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра второго цветового канала G, 
+        добавляемого к исходным в данном цветовом канале
+    k3 : str
+        путь к файлу в формате txt, который содержит значения сгенерированного сверточного ядра первого цветового канала B, 
+        добавляемого к исходным в данном цветовом канале
+    w : list
+        значения исходного/ых ядер, к которым происходит добавление. 
+        Это может быть либо переменная, которой присвоено значение исходных ядер, 
+        либо сами значения, полученные после преобразования с помощью функции txt_kernel_rgb
 
+    Пример использования:
+    wdl.add_kernel_rgb('k1.txt', 'k2.txt', 'k3.txt', w1)
+
+    '''
     f1 = open(k1, 'r')
     f2 = open(k2, 'r')
     f3 = open(k3, 'r')
 	
     w11 = []
 
     for i in f1:
@@ -238,21 +373,31 @@
 	########################################
     for i in range(len(w1)):
         for j in range(len(w1)):
             w[i][j][2].append(w33[i][j])
 	########################################
 	
     return w
-
-#w2 = add_kernel_rgb('k3.txt', 'k2.txt', 'k1.txt', weights1)
-# 9.       
+      
 def select_top(path, label):
-    # label - название столбца с метками классов ('Wine')
-    # z - индекс в переборе меток классов
-    all_classes = pd.read_csv(path)#('wine_train.csv')
+    '''
+    Функция позволяет получить грубое первоначальное приближение вектора весов
+
+    Параметры
+    ----------
+    path : str
+        путь к целочисленной обучающей выборке в формате csv
+    label : str
+        название столбца с метками классов
+
+    Пример использования:
+    wdl.select_top('KAHRAMAN_train.csv', 'UNS')
+
+    '''
+    all_classes = pd.read_csv(path)
     all_classes.drop(all_classes.columns[0], axis=1, inplace=True)
 
     uniq = pd.unique(all_classes[[label]].values.ravel('K'))
     uniq = list(uniq)
     
     
     for o in range(len(uniq)):
@@ -411,30 +556,38 @@
         for file in files:
             data = pd.read_csv(file)
             combined = pd.concat([combined, data])
         combined.drop(combined.columns[0], axis=1, inplace=True)
         combined.to_csv(f'train_{top}{other}.csv')
     
         os.chdir(oldpwd)
-        
-        #weights_all_categories.append(weights)
 
 def grad_boost(path, t, oth, l, s, from_initial, weights_main):
-    # path - путь к обучающей выборке
-    # t - метка целевого класса в виде списка
-    # oth - список меток оставшхся классов
-    # l- название столбца с метками классов ('Wine')
-    # s - шаг градиента
-    
-    # from_initial - 1, если вектор берется из select_top (грубое приближение), 
-    # 0 - если вектор снова корректируется (после grad_boost)
-    
-    # weights_main - весовые коэффиценты в виде списка
-    # zz - индекс в переборе элементов вектора весов
-    
+    '''
+    Вспомогательная функция для корректировки весовых коэффициентов с помощью градиентного уточнения, одиночный проход по вектору
+
+    Параметры
+    ----------
+    path : str
+        путь к обучающей выборке, подаваемой на вход функции select_top
+    t : list
+        метка выбранного на этапе первоначального приближения целевого класса
+    oth : list
+        список, содержащий метки оставшихся классов, которые не относятся к целевому
+    l : str
+        название столбца с метками классов
+    s : int
+        шаг изменения значений элементов вектора весов, шаг градиентного уточнения;
+    from_initial : int
+        1, если вектор берется из select_top (грубое приближение), 
+        0 - если вектор снова корректируется (после grad_boost)
+    weights_main : list
+        вектор весов для корректировки
+
+    '''
     weights_all = []
     
     for zz_i in range(len(weights_main)):
         
         
         zz = zz_i
     
@@ -800,29 +953,37 @@
         
             print()
             
             
     print(weights_all)
     return weights_all
 
-#grad_boost("kahraman_train4.csv", ['high'], ['middle', 'low', 'very_low'], 'UNS', 1, 1, [-47.32524271844662, 358.46601941747576, 480.09708737864077, -221.2135922330097, 260.9077669902913])
-
 def grad_boost_save_files(path, t, oth, l, s, from_initial, weights_main):
-    # path - путь к обучающей выборке
-    # t - метка целевого класса в виде списка
-    # oth - список меток оставшхся классов
-    # l- название столбца с метками классов ('Wine')
-    # s - шаг градиента
-    
-    # from_initial - 1, если вектор берется из select_top (грубое приближение), 
-    # 0 - если вектор снова корректируется (после grad_boost)
-    
-    # weights_main - весовые коэффиценты в виде списка
-    # zz - индекс в переборе элементов вектора весов
-    
+    '''
+    Вспомогательная функция для сохранения усеченных обучающих выборок и скорректированных векторов весов после градиентного уточнения
+
+    Параметры
+    ----------
+    path : str
+        путь к обучающей выборке, подаваемой на вход функции select_top
+    t : list
+        метка выбранного на этапе первоначального приближения целевого класса
+    oth : list
+        список, содержащий метки оставшихся классов, которые не относятся к целевому
+    l : str
+        название столбца с метками классов
+    s : int
+        шаг изменения значений элементов вектора весов, шаг градиентного уточнения;
+    from_initial : int
+        1, если вектор берется из select_top (грубое приближение), 
+        0 - если вектор снова корректируется (после grad_boost)
+    weights_main : list
+        вектор весов для корректировки
+
+    '''
     weights_all = []
     
     for zz_i in range(len(weights_main)):
         
         
         zz = zz_i
     
@@ -1217,16 +1378,29 @@
             weights[zz]+=step  
         
             print()
             
     print(weights_all)
     return weights_all
 
-# 10.  
 def select_top_binary(path, label):
+    '''
+    Функция позволяет получить грубое первоначальное приближение вектора весов для бинарной обучающей выборки
+
+    Параметры
+    ----------
+    path : str
+        путь к целочисленной бинарной обучающей выборке в формате csv
+    label : str
+        название столбца с метками классов
+
+    Пример использования:
+    wdl.select_top_binary('train_6.csv', 'UNS')
+
+    '''
     all_classes_main = pd.read_csv(path)
     all_classes_main.drop(all_classes_main.columns[0], axis=1, inplace=True)
     
     uniq = pd.unique(all_classes_main[[label]].values.ravel('K'))
     uniq = list(uniq)
     
     for o in range(len(uniq)):
@@ -1371,23 +1545,39 @@
         print('OTHER - ', other) 
         print('СУММА отсеченных сверху и снизу = ', sum_up_down)
         print(weights)
         print('DISTANCE = ', distance)
         print('+++++++++++++++++++++++++++++++++++++++')
         print()      
 
-# 11.
 def grad_binary(path, t, oth, l, s, weights_main):
-    #path = 'trainW07_1.csv'
-    #t = ['low']
-    #oth = ['middle']
-    #l = 'UNS'
-    #s = 1
-    #from_initial = 1
-    #weights_main = [-663.0, -8850.0, -610.0, -16520.0, -1202.0] 
+    '''
+    Функция осуществляет градиентное уточнение полученного после первоначального приближения вектора весов 
+    для бинарной обучающей выборки
+
+    Параметры
+    ----------
+    path : str
+        путь к бинарной обучающей выборке, подаваемой на вход функции select_top
+    t : list
+        метка выбранного на этапе первоначального приближения целевого класса
+    oth : list
+        список, содержащий метки оставшихся классов, которые не относятся к целевому
+    l : str
+        название столбца с метками классов
+    s : int
+        шаг изменения значений элементов вектора весов, шаг градиентного уточнения
+    weights_main : list
+        вектор весов, значения которого необходимо изменить с целью получения большего количества 
+        отсеченных экземпляров обучающей выборки
+
+    Пример использования:
+    wdl.grad_binary('train_6.csv', ['Low'], ['Middle'], 'UNS', 1, [1009.0, 48.0, -929.0, -1056.0, -13.0])
+
+    '''
     from_initial = 1
 
     for zz_i in range(len(weights_main)):
         zz = zz_i
         step = s
         label = l
         top = t
@@ -1806,27 +1996,38 @@
                 os.chdir(oldpwd)
                 
                 break
                 
                 
             weights[zz]+=step  
  
-                
-# grad("trainW08_4.csv", ['very_low'], ['high', 'low', 'middle'], 'UNS', [-837.2851063829785, 1654.2510638297872, -485.82978723404267, 1729.021276595745, 19057.587234042556])
-# 12. 
 def grad(path, t, oth, l, s, weights):
-    #path = "trainW08_4.csv"#"kahraman_train.csv"
-    #t = ['high']#['very_low']
-    #oth = ['very_low', 'low', 'middle']#['high', 'low', 'middle']
-    #l = 'UNS'
-    #s = 1
+    '''
+    Функция осуществляет градиентное уточнение полученного после первоначального приближения вектора весов 
 
-    #weights = [-837.2851063829785, 1654.2510638297872, -485.82978723404267, 1729.021276595745, 19057.587234042556]
-    #[-4745.458204334365, -5586.578947368422, -5510.185758513931, -8949.30959752322, -18447.66253869969]
+    Параметры
+    ----------
+    path : str
+        путь к обучающей выборке, подаваемой на вход функции select_top
+    t : list
+        метка выбранного на этапе первоначального приближения целевого класса
+    oth : list
+        список, содержащий метки оставшихся классов, которые не относятся к целевому
+    l : str
+        название столбца с метками классов
+    s : int
+        шаг изменения значений элементов вектора весов, шаг градиентного уточнения
+    weights_main : list
+        вектор весов, значения которого необходимо изменить с целью получения большего количества 
+        отсеченных экземпляров обучающей выборки
 
+    Пример использования:
+    wdl.grad('KAHRAMAN_train.csv', ['High'], ['very_low', 'Low', 'Middle'], 'UNS', 1, [455.02247191011236, 552.8764044943821, 273.38202247191015, 518.2921348314607, 2276.179775280899])
+
+    '''
     weights_all = grad_boost(path, t, oth, l, s, 1, weights)
 
     with open('weights_all==0.txt', 'w') as file:
         file.write(str(weights_all))
 
     up_element = 0
     for i1 in range(len(weights)):
@@ -1914,17 +2115,32 @@
         with open(f'weights=={ii}.txt', 'w') as file:
             file.write(str(weights) + '\nUP = ' + str(up_main) + '\nDOWN = ' + str(down_main) + '\nDistance = ' + str(distance_main))
 
         print('++++++++++++++++++++++++++++++++++++++')
         print()
         ii += 1    
 
-# data_int('forest.csv', 'dec_forest.txt', 'forest')           
-# 13. 
 def data_int(path, decimal, name):
+    '''
+    Функция преобразует набор данных, представленный в вещественнозначном виде в целочисленный вид
+
+    Параметры
+    ----------
+    path : str
+        путь к обучающей выборке в формате csv
+    decimal : str
+        путь к текстовому файлу, содержащему в каждой строке число, обозначающее количество десятичных знаков после 
+        запятой в соответствующем столбце выборки
+    name : str
+        аргумент функции, обозначающий желаемое название выходных генерируемых файлов
+
+    Пример использования:
+    wdl.data_int('kahraman.csv', 'dec.txt', 'KAHRAMAN') 
+
+    '''
     data = pd.read_csv(path) 
 
     decimal_places = open(decimal, 'r')
 
     dec = []
 
     for i in decimal_places:
@@ -1987,18 +2203,31 @@
         lstm.append(i)
     
     data_train = data.drop(labels = lstm,axis = 0)
     data_train.to_csv(f'{name}_train.csv')
     
     return data
 
-# 14. 
-# scale_weights('UNS', 'data/', 'weights/')
 def scale_weights(label, data_folder, weights_folder):
-    
+    '''
+    Функция для масштабирования полученных векторов весов в диапазон от -1 до +1
+
+    Параметры
+    ----------
+    label : str
+        название столбца с метками классов
+    data_folder : str
+        путь к папке, содержащей обучающие выборки каждого нейрона
+    weights_folder : str
+        путь к папке, содержащей веса каждого нейрона
+
+    Пример использования:
+    wdl.scale_weights('UNS', 'data/', 'weights/')
+
+    '''
     os.mkdir('scale')
     os.mkdir('result')
     os.mkdir('all_weights')
     
     w = []
 
     # Сортируем список файлов в папке по алфавиту
@@ -2192,18 +2421,32 @@
         content = f.read().replace(',,', ',')
 
     with open("all_weights/weights.txt", "w") as f:
         f.write(content)
     
     return scaled_w
 
-# 15.
-# generate_fa('UNS', 'result', 'scale')
 def generate_fa(label, data_folder, weights_folder):
+    '''
+    Функция, которая на основании проведенного обучения модифицированного полносвязного слоя, генерирует вложенную 
+    логическую функцию активации для проверки весовых коэффициентов на тестовых данных
+
+    Параметры
+    ----------
+    label : str
+        название столбца обучающих выборок, в котором содержатся наименования (метки) классов
+    data_folder : str
+        путь к папке result, сгенерированной в результате выполнения функции scale_weights
+    weights_folder : str
+        путь к каталогу scale, который сгенерирован после применения функции scale_weights
 
+    Пример использования:
+    wdl.generate_fa('UNS', 'result', 'scale')
+
+    '''
     w = []
 
     files1 = sorted(os.listdir(weights_folder))
     files2 = sorted(os.listdir(data_folder))
 
     for i in range(0, len(files1)):
         filename = f"sw_{i}.txt"
@@ -2295,45 +2538,93 @@
                 print(f'            elif(data["SC{ii}"][n]>=1):\n                data["FA"][n]="{firstindex}"')
             if(round(t_down) <= -1):
                 print(f'            elif(data["SC{ii}"][n]<=-1):\n                data["FA"][n]="{lastindex}"')
             
                 
         ii += 1
 
-# 16. 
-# check_test('train_1.csv', 'weights.txt', 'KAHRAMAN_test.csv', 'UNS')
 def check_test(train, weights, test, label):
+    '''
+    Функция осуществляет проверку обучения с помощью правил логического вывода
+
+    Параметры
+    ----------
+    train : str
+        путь к полной целочисленной обучающей выборке
+    weights : str
+        путь к текстовому файлу weights.txt из сгенерированного каталога all_weights после функции scale_weights
+    test : str
+        путь к целочисленной тестовой выборке (в случае проверки обучающей выборки передается путь к полной обучающей выборке, 
+        аналогичный параметру train)
+    label : str
+        название столбца с метками классов
+
+    Пример использования:
+    wdl.check_test('train_1.csv', 'weights.txt', 'KAHRAMAN_test.csv', 'UNS')
+
+    '''
     def getNameColumn(nameFileTrain):
+        '''
+        Вспомогательная функция для определения названий всех столбцов, кроме столбца с метками классов
+
+        Параметры
+        ----------
+        nameFileTrain : str
+            путь к обучающей выборке 
+
+        '''
         with open(nameFileTrain, encoding='utf-8') as r_file:
             # Создаем объект DictReader, указываем символ-разделитель ','
             file_reader = csv.DictReader(r_file, delimiter = ',')
             nameColumn  = list(file_reader.fieldnames)  #названия столбцов
         r_file.close()
         del nameColumn[-1]
         del nameColumn[:2]
         return nameColumn
     def getCountNeuronSizeVector(nameFileTrain):
+        '''
+        Вспомогательная функция для определения необходимого количества нейронов в слое
+
+        Параметры
+        ----------
+        nameFileTrain : str
+            путь к обучающей выборке 
+
+        '''
         with open(nameFileTrain, encoding='utf-8') as r_file:
             # Создаем объект DictReader, указываем символ-разделитель ','
             file_reader = csv.DictReader(r_file, delimiter=',')
             nameColumn  = list(file_reader.fieldnames)  #названия столбцов
             sizeVector = len(nameColumn) - 1          #количество столбцов
             countNeurons = 1
             for row in file_reader:
                 countNeurons += 1
         r_file.close()
         return countNeurons, sizeVector
     def initializingDictionaryKeys():
+        '''
+        Вспомогательная функция для инициализации ключей для правила логического вывода
+
+        '''
         iNeuron = 1                             #инициализация
         while iNeuron <= countNeurons:          #ключей
             rulesLogicalInference[iNeuron] = 0  #для
             rulesLogicalInference[-iNeuron] = 0 #правила
             iNeuron += 1                        #логического
         rulesLogicalInference[iNeuron * 10] = 0 #вывода
     def initializationDictionaryValues(nameFileTrain):
+        '''
+        Вспомогательная функция для создания словаря логического вывода
+
+        Параметры
+        ----------
+        nameFileTrain : str
+            путь к обучающей выборке 
+
+        '''
         with open(nameFileTrain, encoding='utf-8') as r_file:
             # Создаем объект DictReader, указываем символ-разделитель ','
             file_reader = csv.DictReader(r_file, delimiter=',')
             nameCol = list(file_reader.fieldnames)  # названия столбцов
             for row in file_reader:
                 iVector = 0
                 for iColumn in nameColumn:  # чтение вектора входов из обучающей выборки
@@ -2406,17 +2697,38 @@
         data = list(reader)
         row_count = len(data) - 1
     #print(row_count)
     
     print('Ошибок = ', len(zz), 'из ', row_count)
     print('Экземпляры №:', zz)
 
-# 17.
-# count_conv_operations(28, 28, 1, 14, 7, 4)
 def count_conv_operations(height, width, color_channels, kernel_size, stride, num_kernels):
+    '''
+    Функция для подсчета количества вычислительных операций в сверточном слое 
+
+    Параметры
+    ----------
+    height : int
+        высота исходного изображения выборки данных
+    width : int
+        ширина исходного изображения
+    color_channels : int
+        количество цветовых каналов изображения 
+        (1 – если изображение представлено в черно-белом одноканальном виде, 3 – если изображение является цветным)
+    kernel_size : int
+        размерность сверточного ядра квадратной формы
+    stride : int
+        шаг прохода сверточного ядра по изображению
+    num_kernels : int
+        количество сверточных ядер в слое
+
+    Пример использования:
+    wdl.count_conv_operations(28, 28, 1, 14, 7, 4)
+
+    '''
     output_height = int((height - kernel_size) / stride) + 1
     output_width = int((width - kernel_size) / stride) + 1
     num_operations = (output_height * output_width * kernel_size * kernel_size * num_kernels * 2)*color_channels
     
     no_bias = (num_operations - ((kernel_size**2)*num_kernels))*color_channels
     print('Кол-во вычислительных операций = ', num_operations)  
     print('Кол-во вычислительных операций (no_bias) = ', no_bias)
```

