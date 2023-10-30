# Notes

You can use miniconda to install via a gazillion youtube videos or the offical docs [here](https://developer.apple.com/metal/tensorflow-plugin/)


# My approach

```
$ cd ~/progs
$ mkdir myvenvs
$ cd myvenvs
# this will install to root dir
#$ python3 -m venv ~/venv-metal
# this will install to this dir
$ python3 -m venv venv-metal
# go back to the progs dir
$ cd ..
# activate the env
$ source myvenvs/venv-metal/bin/activate
# update pip
# Note at this point, python and python3 are equivalent.
(venv-metal) $ python -m pip install -U pip
# install base tensorflow
$ python -m pip install tensorflow
# install metal tensorflow
$ python -m pip install tensorflow-metal
```
# Test it

## From Jeff Heatons Git

Shamelessly ripped off from

* [repo](https://github.com/jeffheaton/t81_558_deep_learning)
* [platform dump](https://github.com/jeffheaton/t81_558_deep_learning/blob/master/install/tensorflow-install-march-2023.ipynb)


Install the base modules

```
python -m pip install pandas
python3 -m pip install scikit-learn
```

Jeff's mod is out of date so use this one.  Keras no longer has a version.  Its part of tensorflow.

```
# What version of Python do you have?
import sys

from tensorflow import keras
import pandas as pd
import sklearn as sk
import tensorflow as tf

print(f"Tensor Flow Version: {tf.__version__}")
print()
print(f"Python {sys.version}")
print(f"Pandas {pd.__version__}")
print(f"Scikit-Learn {sk.__version__}")
gpu = len(tf.config.list_physical_devices('GPU'))>0
print("GPU is", "available" if gpu else "NOT AVAILABLE")
```

Make sure it prints GPU is available.

```
(venv-metal)  davis@foo ~/progs > python3 testy.py
Tensor Flow Version: 2.14.0

Python 3.9.6 (default, Sep 26 2022, 11:37:49)
[Clang 14.0.0 (clang-1400.0.29.202)]
Pandas 2.1.2
Scikit-Learn 1.3.2
GPU is available
```