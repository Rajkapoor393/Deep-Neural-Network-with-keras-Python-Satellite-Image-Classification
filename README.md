## Deep Neural Network with keras-Python: Satellite-Image Classification
![Python 3.6](https://img.shields.io/badge/Python-3.6-brightgreen.svg) 
<img src="https://img.shields.io/badge/Keras%20-%23D00000.svg?&style=for-the-badge&logo=Keras&logoColor=white"/>
<img src="https://img.shields.io/badge/TensorFlow%20-%23FF6F00.svg?&style=for-the-badge&logo=TensorFlow&logoColor=white" />

This tutorial  will show how to implement [Deep Neural Network](https://en.wikipedia.org/wiki/Deep_learning) for [pixel based](https://gis.stackexchange.com/questions/237461/distinction-between-pixel-based-and-object-based-classification) [supervised classification ](https://articles.extension.org/pages/40214/whats-the-difference-between-a-supervised-and-unsupervised-image-classification) of [Sentinel-2 multispectral images](https://sentinel.esa.int/web/sentinel/missions/sentinel-2) using [keras](https://keras.io/#installation/) package in [Anaconda 5.1 Python 3.6](https://www.anaconda.com/download/#download/) under [Windows 10](https://www.microsoft.com/en-us/software-download/windows10).

[keras](https://keras.rstudio.com/) is a popular Python package for deep neural networks with multiple backends, including [TensorFlow](https://www.tensorflow.org/), [Microsoft Cognitive Toolkit (CNTK)](https://docs.microsoft.com/en-us/cognitive-toolkit/), and [Theano](http://deeplearning.net/software/theano/). The keras package is able to provide a flexible and feature-rich API and can run both [CPU and GUP version of TensorFlow](https://www.tensorflow.org/install/install_windows) in both Windows and Linux.  If you want to run this tutorial with [GUP version of TensorFlow](https://www.tensorflow.org/install/install_windows) you need following prerequisites in your system:   

*[NVIDIA GUP](https://developer.nvidia.com/cuda-gpus): First, you must make sure weather your computer is running with [NVIDIAÂ® GPU](https://developer.nvidia.com/cuda-gpus) or not. Follow the instruction as described  [here](http://nvidia.custhelp.com/app/answers/detail/a_id/2040/~/identifying-the-graphics-card-model-and-device-id-in-a-pc).  

*[CUDA Toolkit v9.0](https://developer.nvidia.com/cuda-90-download-archive?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exelocal): If you have an NVIDIAÂ® GPU in your system, you need to download and install [CUDA Toolkit  v9.0](https://developer.nvidia.com/cuda-90-download-archive?target_os=Windows&target_arch=x86_64&target_version=10&target_type=exelocal). Detail installation steps can be found [here](http://nvidia.custhelp.com/app/answers/detail/a_id/2040/~/identifying-the-graphics-card-model-and-device-id-in-a-pc).

*[cuDNN v7.0](https://developer.nvidia.com/cudnn): The download the zip file version [cuDNN v7.0](https://developer.nvidia.com/cudnn) for your CUDA Toolkit v9.0.You need to extract the zip file and add the location where you extracted it to your system PATH.  Detail installation steps can be found here [here](F:/DeepLearning_tutorial/Satellite_Image_Calssification/h20_R_ImageCalssification/keras_R/Detail installation steps are described here). 

Detail installation steps of Keras backend Tensorflow can be found [here](https://keras.io/#installation).

First, we will split "point_data" into a training set (75% of the data), a validation set (12%) and a test set (13%) data.The validation data set will be used to optimize the model parameters during training process.The model's performance will be tested with the data set and then we will predict landuse clasess on grid data set. 

<div align="center">

### Show some ❤️ by starring this repository!

</div>
