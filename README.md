# Weights and Biases Tutorial on HiperGator
>This Requires a Weights and Biases Account (https://wandb.ai/site)

## Weights and Biases Setup
1. Once you login, navigate to: https://wandb.ai/settings
2. Select, Danger Zone -> API Keys -> New Key

## Installation
1. Begin by cloning this repository to your chosen directory `\path\to\directory\`:

```
cd \path\to\directory\
git clone https://github.com/aa14av/wandb-tutorial.git
cd wandb-tutorial
```

2. Once the repository is cloned, open `example.ipynb` and select the kernel `Tensorflow-2.7.0`
   
3. Copy/paste this API Key you generated earlier into the `example.ipynb` at:
   
```Python
import os, sys
sys.path.append(os.path.join(os.path.dirname(os.getcwd()),'.local','bin'))

import cv2, itertools, warnings, shutil, random
import wandb as wb
from wandb.keras import WandbMetricsLogger
import pandas as pd
import numpy as np
from pathlib import Path

import seaborn as sns
import matplotlib.pyplot as plt
import matplotlib.image as img

from PIL import Image
from random import randint
warnings.filterwarnings('ignore')

from imblearn.over_sampling import SMOTE
from sklearn.model_selection import train_test_split
from sklearn.metrics import matthews_corrcoef as MCC
from sklearn.metrics import balanced_accuracy_score as BAS
from sklearn.metrics import classification_report, confusion_matrix

from tensorflow import keras
from keras import layers
import tensorflow as tf
import tensorflow_addons as tfa
from tensorflow.keras.preprocessing import image_dataset_from_directory
from keras.utils.vis_utils import plot_model
from tensorflow.keras import Sequential, Input
from tensorflow.keras.layers import Dense, Dropout
from tensorflow.keras.layers import Conv2D, Flatten
from tensorflow.keras.callbacks import ReduceLROnPlateau
from tensorflow.keras.applications.inception_v3 import InceptionV3
from tensorflow.keras.preprocessing.image import ImageDataGenerator as IDG
from tensorflow.keras.layers import SeparableConv2D, BatchNormalization, GlobalAveragePooling2D

from distutils.dir_util import copy_tree, remove_tree

print("TensorFlow Version:", tf.__version__)
wb.login(); # USE YOUR API KEY TO LOGIN HERE
```
