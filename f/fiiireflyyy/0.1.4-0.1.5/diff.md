# Comparing `tmp/fiiireflyyy-0.1.4.tar.gz` & `tmp/fiiireflyyy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiiireflyyy-0.1.4.tar", last modified: Tue Jun 13 13:02:42 2023, max compression
+gzip compressed data, was "fiiireflyyy-0.1.5.tar", last modified: Tue Jun 13 13:35:45 2023, max compression
```

## Comparing `fiiireflyyy-0.1.4.tar` & `fiiireflyyy-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:02:42.059917 fiiireflyyy-0.1.4/
--rw-rw-rw-   0        0        0      669 2023-06-13 13:02:42.059917 fiiireflyyy-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     6290 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 13:02:42.054916 fiiireflyyy-0.1.4/fiiireflyyy/
--rw-rw-rw-   0        0        0      153 2023-06-13 12:11:31.000000 fiiireflyyy-0.1.4/fiiireflyyy/__init__.py
--rw-rw-rw-   0        0        0     4312 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.4/fiiireflyyy/firefiles.py
--rw-rw-rw-   0        0        0    51273 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.4/fiiireflyyy/firelearn.py
--rw-rw-rw-   0        0        0    14713 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.4/fiiireflyyy/fireprocess.py
--rw-rw-rw-   0        0        0    15817 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.4/fiiireflyyy/flimage.py
--rw-rw-rw-   0        0        0      649 2023-06-13 12:15:44.000000 fiiireflyyy-0.1.4/fiiireflyyy/logic_gates.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:02:42.058917 fiiireflyyy-0.1.4/fiiireflyyy.egg-info/
--rw-rw-rw-   0        0        0      669 2023-06-13 13:02:41.000000 fiiireflyyy-0.1.4/fiiireflyyy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-06-13 13:02:42.000000 fiiireflyyy-0.1.4/fiiireflyyy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:02:41.000000 fiiireflyyy-0.1.4/fiiireflyyy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-06-13 13:02:41.000000 fiiireflyyy-0.1.4/fiiireflyyy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 13:02:41.000000 fiiireflyyy-0.1.4/fiiireflyyy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 13:02:42.063918 fiiireflyyy-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1113 2023-06-13 13:01:52.000000 fiiireflyyy-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:35:45.969043 fiiireflyyy-0.1.5/
+-rw-rw-rw-   0        0        0      669 2023-06-13 13:35:45.969043 fiiireflyyy-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6290 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 13:35:45.964043 fiiireflyyy-0.1.5/fiiireflyyy/
+-rw-rw-rw-   0        0        0      153 2023-06-13 12:11:31.000000 fiiireflyyy-0.1.5/fiiireflyyy/__init__.py
+-rw-rw-rw-   0        0        0     4312 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.5/fiiireflyyy/firefiles.py
+-rw-rw-rw-   0        0        0    38407 2023-06-13 13:30:29.000000 fiiireflyyy-0.1.5/fiiireflyyy/firelearn.py
+-rw-rw-rw-   0        0        0    14713 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.5/fiiireflyyy/fireprocess.py
+-rw-rw-rw-   0        0        0    15817 2023-06-13 09:58:55.000000 fiiireflyyy-0.1.5/fiiireflyyy/flimage.py
+-rw-rw-rw-   0        0        0      649 2023-06-13 12:15:44.000000 fiiireflyyy-0.1.5/fiiireflyyy/logic_gates.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:35:45.968044 fiiireflyyy-0.1.5/fiiireflyyy.egg-info/
+-rw-rw-rw-   0        0        0      669 2023-06-13 13:35:45.000000 fiiireflyyy-0.1.5/fiiireflyyy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-06-13 13:35:45.000000 fiiireflyyy-0.1.5/fiiireflyyy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 13:35:45.000000 fiiireflyyy-0.1.5/fiiireflyyy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-06-13 13:35:45.000000 fiiireflyyy-0.1.5/fiiireflyyy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 13:35:45.000000 fiiireflyyy-0.1.5/fiiireflyyy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 13:35:45.972045 fiiireflyyy-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2023-06-13 13:34:57.000000 fiiireflyyy-0.1.5/setup.py
```

### Comparing `fiiireflyyy-0.1.4/PKG-INFO` & `fiiireflyyy-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiiireflyyy
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package covering miscellaneous uses, from system management to machine learning and image or data processing. Developed for personal uses.
 Author: fiiireflyyy (Willy Lutz)
 Author-email: <lutz0willy@gmail.com>
 Keywords: python,machine learning,deep learning,data analysis,system management,data processing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fiiireflyyy-0.1.4/README.txt` & `fiiireflyyy-0.1.5/README.txt`

 * *Files identical despite different names*

### Comparing `fiiireflyyy-0.1.4/fiiireflyyy/firefiles.py` & `fiiireflyyy-0.1.5/fiiireflyyy/firefiles.py`

 * *Files identical despite different names*

### Comparing `fiiireflyyy-0.1.4/fiiireflyyy/firelearn.py` & `fiiireflyyy-0.1.5/fiiireflyyy/firelearn.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,28 +2,23 @@
 import pathlib
 import pickle
 import shutil
 import sys
 from random import randint
 
 import seaborn as sns
-from tensorflow import keras
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import tensorflow as tf
-from keras import layers
-from keras.models import Sequential, Model, load_model
+
 from matplotlib import transforms
-from keras.preprocessing.image import ImageDataGenerator
-from keras.layers import Dense, Conv2D, MaxPool2D, Flatten, Dropout
-from keras.callbacks import CSVLogger
+
 from keras.utils.np_utils import to_categorical
-from tensorflow.keras.optimizers import Adam
+from keras.models import load_model
 
 from matplotlib.collections import PathCollection
 from matplotlib.legend_handler import HandlerPathCollection, HandlerLine2D
 from matplotlib.patches import Ellipse
 from sklearn.decomposition import PCA
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import train_test_split
@@ -95,304 +90,15 @@
         ff.verify_dir(os.path.join(destination, target))
 
         for file in files:
             if target in file:
                 shutil.copy2(file, os.path.join(destination, target))
 
 
-def basic_keras(model_spec, src, dst, img_size, epochs=10, visualize=False, saving=True):
-    """
-    Compute a basic Keras model for a images binary classification problem.
-
-    :param model_spec: the name of the model. Identical to the root folder that will contain the model.
-    :type model_spec: str
-    :param src: Where to find the data.
-    :type src: str
-    :param dst: Where to save the sorted data
-    :type dst: str
-    :param img_size: the size of the image.
-    :type img_size: tuple[int]
-    :param epochs: The number of epochs of the model. Default at 10.
-    :param visualize: To visualize the model's results
-    :type visualize: bool
-    :param saving: To save the model's results
-    :type saving: bool
-    :return:
-    """
-    # generate_classes(src, dst, targets=['INF', 'NI'])
-    # Getting the dataset
-
-    data_dir = pathlib.Path(dst)
-    image_count = len(list(data_dir.glob('*.png')))
-    print(image_count)
-
-    # loading data
-    batch_size = 8
-    img_height = img_size[0]
-    img_width = img_size[1]
-
-    train_ds = tf.keras.utils.image_dataset_from_directory(
-        data_dir,
-        validation_split=0.2,
-        subset='training',
-        seed=123,
-        image_size=(img_height, img_width),
-        batch_size=batch_size)
-
-    val_ds = tf.keras.utils.image_dataset_from_directory(
-        data_dir,
-        validation_split=0.2,
-        subset='validation',
-        seed=123,
-        image_size=(img_height, img_width),
-        batch_size=batch_size)
-
-    class_names = train_ds.class_names
-    print(class_names)
-
-    # Visualizing data
-    if visualize:
-        plt.figure(figsize=(10, 10))
-        for images, labels in train_ds.take(1):
-            for i in range(9):
-                ax = plt.subplot(3, 3, i + 1)
-                plt.imshow(images[i].numpy().astype("uint8"))
-                plt.title(class_names[labels[i]])
-                plt.axis("off")
-        plt.show()
-
-    for image_batch, labels_batch in train_ds:
-        print(image_batch.shape)
-        print(labels_batch.shape)
-        break
-
-    # Configure the dataset for performance
-
-    AUTOTUNE = tf.data.AUTOTUNE
-
-    train_ds = train_ds.cache().shuffle(
-        1000)  # .prefetch(buffer_size=AUTOTUNE)  # Once loaded, keep the pictures in memory
-    val_ds = val_ds.cache().prefetch(buffer_size=AUTOTUNE)  # Overlaps data preprocessing/model execution while training
-
-    # Data augmentation
-    data_augmentation = keras.Sequential(
-        [
-            layers.RandomFlip("horizontal_and_vertical",
-                              input_shape=(img_height,
-                                           img_width,
-                                           3)),
-            layers.RandomRotation(1.0),
-            layers.RandomZoom(0.5),
-        ]
-    )
-
-    # Basic Keras model
-    num_classes = len(class_names)
-    model = Sequential([
-        data_augmentation,
-        layers.Rescaling(1. / 255),
-        layers.Conv2D(16, 3, padding='same', activation='relu'),
-        layers.MaxPooling2D(),
-        layers.Conv2D(32, 3, padding='same', activation='relu'),
-        layers.MaxPooling2D(),
-        layers.Conv2D(64, 3, padding='same', activation='relu'),
-        layers.MaxPooling2D(),
-        layers.Dropout(0.2),
-        layers.Flatten(),
-        layers.Dense(128, activation='relu'),
-        layers.Dense(num_classes, name="outputs")
-    ])
-
-    model.compile(optimizer='adam',
-                  loss=tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-                  metrics=['accuracy'])
-
-    model.summary()
-
-    # Train the model
-
-    history = model.fit(
-        train_ds,
-        validation_data=val_ds,
-        epochs=epochs
-    )
-
-    # Visualize training
-    acc = history.history['accuracy']
-    val_acc = history.history['val_accuracy']
-
-    loss = history.history['loss']
-    val_loss = history.history['val_loss']
-
-    epochs_range = range(epochs)
-
-    plt.figure(figsize=(8, 8))
-    plt.subplot(1, 2, 1)
-    plt.plot(epochs_range, acc, label='Training Accuracy')
-    plt.plot(epochs_range, val_acc, label='Validation Accuracy')
-    plt.legend(loc='lower right')
-    plt.title('Training and Validation Accuracy')
-
-    plt.subplot(1, 2, 2)
-    plt.plot(epochs_range, loss, label='Training Loss')
-    plt.plot(epochs_range, val_loss, label='Validation Loss')
-    plt.legend(loc='upper right')
-    plt.title('Training and Validation Loss')
-
-    save_path = os.path.join(os.path.join(pathlib.Path(dst).parent.parent.absolute(), "RESULTS"), model_spec,
-                             "training validation acc loss.png")
-    ff.verify_dir(os.path.join(os.path.join(pathlib.Path(dst).parent.parent.absolute(), "RESULTS"), model_spec))
-    if saving:
-        plt.savefig(save_path)
-    if visualize:
-        plt.show()
-    plt.close()
-
-
-def keras_tutorial():
-    """
-    A tutorial use of keras model for image multiclass classification
 
-    :return:
-    """
-    # downloading the test dataset
-    dataset_url = "https://storage.googleapis.com/download.tensorflow.org/example_images/flower_photos.tgz"
-    data_dir = tf.keras.utils.get_file('flower_photos', origin=dataset_url, untar=True)
-    data_dir = pathlib.Path(data_dir)
-    image_count = len(list(data_dir.glob('*/*.jpg')))
-
-    # loading data using keras
-    batch_size = 32
-    img_height = 180
-    img_width = 180
-
-    train_ds = tf.keras.utils.image_dataset_from_directory(
-        data_dir,
-        validation_split=0.2,
-        subset="training",
-        seed=123,
-        image_size=(img_height, img_width),
-        batch_size=batch_size)
-
-    val_ds = tf.keras.utils.image_dataset_from_directory(
-        data_dir,
-        validation_split=0.2,
-        subset="validation",
-        seed=123,
-        image_size=(img_height, img_width),
-        batch_size=batch_size)
-
-    class_names = train_ds.class_names
-    print(class_names)
-
-    # Visualizing data
-    plt.figure(figsize=(10, 10))
-    for images, labels in train_ds.take(1):
-        for i in range(9):
-            ax = plt.subplot(3, 3, i + 1)
-            plt.imshow(images[i].numpy().astype("uint8"))
-            plt.title(class_names[labels[i]])
-            plt.axis("off")
-    plt.show()
-
-    for image_batch, labels_batch in train_ds:
-        print(image_batch.shape)
-        print(labels_batch.shape)
-        break
-
-    # Configure the dataset for performance
-
-    AUTOTUNE = tf.data.AUTOTUNE
-
-    train_ds = train_ds.cache().shuffle(1000).prefetch(buffer_size=AUTOTUNE)  # Once loaded, keep the pictures in memory
-    val_ds = val_ds.cache().prefetch(buffer_size=AUTOTUNE)  # Overlaps data preprocessing/model execution while training
-
-    # Data augmentation
-    data_augmentation = keras.Sequential(
-        [
-            layers.RandomFlip("horizontal",
-                              input_shape=(img_height,
-                                           img_width,
-                                           3)),
-            layers.RandomRotation(0.1),
-            layers.RandomZoom(0.1),
-        ]
-    )
-
-    # Basic Keras model
-    num_classes = len(class_names)
-    model = Sequential([
-        data_augmentation,
-        layers.Rescaling(1. / 255),
-        layers.Conv2D(16, 3, padding='same', activation='relu'),
-        layers.MaxPooling2D(),
-        layers.Conv2D(32, 3, padding='same', activation='relu'),
-        layers.MaxPooling2D(),
-        layers.Conv2D(64, 3, padding='same', activation='relu'),
-        layers.MaxPooling2D(),
-        layers.Dropout(0.2),
-        layers.Flatten(),
-        layers.Dense(128, activation='relu'),
-        layers.Dense(num_classes, name="outputs")
-    ])
-
-    model.compile(optimizer='adam',
-                  loss=tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),
-                  metrics=['accuracy'])
-
-    model.summary()
-
-    # Train the model
-    epochs = 15
-    history = model.fit(
-        train_ds,
-        validation_data=val_ds,
-        epochs=epochs
-    )
-
-    # Visualize training
-    acc = history.history['accuracy']
-    val_acc = history.history['val_accuracy']
-
-    loss = history.history['loss']
-    val_loss = history.history['val_loss']
-
-    epochs_range = range(epochs)
-
-    plt.figure(figsize=(8, 8))
-    plt.subplot(1, 2, 1)
-    plt.plot(epochs_range, acc, label='Training Accuracy')
-    plt.plot(epochs_range, val_acc, label='Validation Accuracy')
-    plt.legend(loc='lower right')
-    plt.title('Training and Validation Accuracy')
-
-    plt.subplot(1, 2, 2)
-    plt.plot(epochs_range, loss, label='Training Loss')
-    plt.plot(epochs_range, val_loss, label='Validation Loss')
-    plt.legend(loc='upper right')
-    plt.title('Training and Validation Loss')
-    plt.show()
-
-    # Predict on new data
-    sunflower_url = "https://storage.googleapis.com/download.tensorflow.org/example_images/592px-Red_sunflower.jpg"
-    sunflower_path = tf.keras.utils.get_file('Red_sunflower', origin=sunflower_url)
-
-    img = tf.keras.utils.load_img(
-        sunflower_path, target_size=(img_height, img_width)
-    )
-    img_array = tf.keras.utils.img_to_array(img)
-    img_array = tf.expand_dims(img_array, 0)  # Create a batch
-
-    predictions = model.predict(img_array)
-    score = tf.nn.softmax(predictions[0])
-
-    print(
-        "This image most likely belongs to {} with a {:.2f} percent confidence."
-        .format(class_names[np.argmax(score)], 100 * np.max(score))
-    )
 
 
 def train_RFC_from_dataset(dataset: pd.DataFrame, savepath=""):
     """
     Train a Random Forest Classifier model from an already formatted dataset.
 
         Parameters
@@ -1211,81 +917,14 @@
     if savepath:
         plt.savefig(os.path.join(savepath, title))
     else:
         plt.show()
     plt.close()
 
 
-def basic_sequential(data, epochs, comment="", model_savepath="", history_savepath=""):
-    """
-    Use of a generic Convolutional network, use for basic image classification.
-    The inputs are of shape (224, 224).
-
-        Parameters
-        ----------
-        data: ndarray shape((n, 2), m)
-            The numpy array containing the data.
-            Each entry is coupled within a tuple with its
-            corresponding label
-        epochs: int
-            number of epochs to train the model on.
-        comment: str, optional, default: ""
-            Add to the name a comment, used when saving
-            the model and for the model name.
-        savepath: str, optional, default: ""
-            If not empty, directory where to save the model.
-        savepath: str, optional, default: ""
-            If not empty, directory where to save the history plot.
-
-    """
-    x_train, x_val, y_train, y_val = split_train_test(data)
-    datagen = ImageDataGenerator(
-        featurewise_center=False,  # set input mean to 0 over the dataset
-        samplewise_center=False,  # set each sample mean to 0
-        featurewise_std_normalization=False,  # divide inputs by std of the dataset
-        samplewise_std_normalization=False,  # divide each input by its std
-        zca_whitening=False,  # apply ZCA whitening
-        rotation_range=180,  # randomly rotate images in the range (degrees, 0 to 180)
-        zoom_range=0.2,  # Randomly zoom image
-        width_shift_range=0,  # randomly shift images horizontally (fraction of total width)
-        height_shift_range=0,  # randomly shift images vertically (fraction of total height)
-        horizontal_flip=False,  # randomly flip images
-        vertical_flip=False,  # randomly flip images
-    )
-
-    datagen.fit(x_train)
-    model = Sequential()
-
-    model.add(Conv2D(32, 7, padding="same", activation="relu", input_shape=(224, 224, 3)))
-    model.add(MaxPool2D())
-
-    model.add(Conv2D(32, 7, padding="same", activation="relu"))
-    model.add(MaxPool2D())
-
-    model.add(Conv2D(64, 7, padding="same", activation="relu"))
-    model.add(MaxPool2D())
-    model.add(Dropout(0.4))
-
-    model.add(Flatten())
-    model.add(Dense(128, activation="relu"))
-    model.add(Dense(2, activation="softmax"))
-
-    opt = Adam(learning_rate=0.000001)
-    model.compile(optimizer=opt, loss="categorical_crossentropy",
-                  metrics=['accuracy'])
-
-    name = f"e={epochs} basic model{comment}"
-
-    csv_logger = CSVLogger(os.path.join(model_savepath, f"{name} history.log"), separator=',', append=False)
-    history = model.fit(x_train, y_train, epochs=epochs, validation_data=(x_val, y_val), callbacks=[csv_logger])
-    if model_savepath:
-        model.save(os.path.join(model_savepath, f"{name}.h5"))
-    if history_savepath:
-        model_history_plot(os.path.join(model_savepath, f"{name} history.log"), savepath=history_savepath)
-
 
 def split_train_test(data, train_size: float = 0.7):
     """
     Split a dataset into train and validation sets for features and labels.
 
         Parameters
         ----------
```

### Comparing `fiiireflyyy-0.1.4/fiiireflyyy/fireprocess.py` & `fiiireflyyy-0.1.5/fiiireflyyy/fireprocess.py`

 * *Files identical despite different names*

### Comparing `fiiireflyyy-0.1.4/fiiireflyyy/flimage.py` & `fiiireflyyy-0.1.5/fiiireflyyy/flimage.py`

 * *Files identical despite different names*

### Comparing `fiiireflyyy-0.1.4/fiiireflyyy/logic_gates.py` & `fiiireflyyy-0.1.5/fiiireflyyy/logic_gates.py`

 * *Files identical despite different names*

### Comparing `fiiireflyyy-0.1.4/fiiireflyyy.egg-info/PKG-INFO` & `fiiireflyyy-0.1.5/fiiireflyyy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiiireflyyy
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package covering miscellaneous uses, from system management to machine learning and image or data processing. Developed for personal uses.
 Author: fiiireflyyy (Willy Lutz)
 Author-email: <lutz0willy@gmail.com>
 Keywords: python,machine learning,deep learning,data analysis,system management,data processing
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fiiireflyyy-0.1.4/setup.py` & `fiiireflyyy-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'A python package covering miscellaneous uses, from system management to machine learning and image or' \
               ' data processing. Developed for personal uses.'
 
 # Setting up
 setup(
     name="fiiireflyyy",
     version=VERSION,
```

