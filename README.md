# ECG based AF Classifier using CNNs
This is  a simple program to conduct sentiment analysis on any given user input. This is my first Machine Learning model.

## Dependencies:
  1. Python 3
  2. Pandas
  3. Numpy
  4. Matplotlib
  5. Tensorflow
  6. Keras

## Installation for Python 3
Visit: https://www.python.org/downloads/ and download the version suitable for your System

## Installation for Pandas
Open Command Prompt (Windows) or Terminal (Linux) and type in the following command:
~~~     
pip install pandas
~~~

Visit: [Pandas Install Instructions](https://pandas.pydata.org/pandas-docs/stable/install.html) for details.

## Installation for Numpy
Open Command Prompt (Windows) or Terminal (Linux) and type in the following command:
~~~     
pip install numpy
~~~

Visit: [Numpy Install Instructions](https://www.scipy.org/install.html) for details.

## Installation for Matplotlib
Open Command Prompt (Windows) or Terminal (Linux) and type in the following command:
~~~     
pip install matplotlib
~~~

Visit: [Matplotlib Install Instructions](https://matplotlib.org/users/installing.html) for details.

## Installation for Tensorflow
There are two formats of Tensorflow. One is for the CPU version and the other is for GPU version (Nvidia only)

The CPU installation is quite straight forward installation by the following command:

~~~
pip install tensorflow
~~~

The GPU version requires the installation of CUDA and cuDNN drivers from Nvidia. This is a relatively complicated process and it is suggested to visit the official guide for this.

Visit: [Tensorflow GPU Install Instructions](https://www.tensorflow.org/install/gpu) for details.

## Installation for Keras
Even though Keras comes built inside tensorflow, in this repository, the code that is used is using the external Keras library. It can be downloaded using the following method.

Open Command Prompt (Windows) or Terminal (Linux) and type in the following command:
~~~     
pip install keras
~~~

Visit: [Keras Install Instructions](https://keras.io/#installation) for details.

## How to use?
1. Download the dataset from [HERE](https://physionet.org/cgi-bin/atm/ATM) and select the following parameters:
   1. Database - `PAF Prediction Challenge Database (afpdb)`
   2. Record - nXX (for each `Normal Patient` data) and pXX (for each `Abnoramal Patient` data)
   3. Length - `to end`
   4. Time Format - `Samples`
   5. Toolbox - `Export signals to CSV`
2. Put them in the desired path and change the path of the `Data_Preprocessing.ipynb` to be able to read the signals from the downloaded CSVs.
3. Save the processed dataset as a Numpy Object in the desired location.
4. In the file `Model.ipynb` read the saved processed dataset and train the model.
5. Any unknown dataset can be then classifed by using `model.predict()` function after the `model` has been trained succesfully. 