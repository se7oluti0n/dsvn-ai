Install CUDA and TensorFlow
=====

## 1. Install Cuda

* Goto https://developer.nvidia.com/cuda-downloads
* Download Linux > x86_64 > Ubuntu > 16.04 > deb(network), follow instructions as:
```
    `sudo dpkg -i cuda-repo-ubuntu1604_8.0.44-1_amd64.deb`
    `sudo apt-get update`
    `sudo apt-get install cuda`
```

Done install Cuda

Test CUDA: 
### Install gcc-4.9 & g++-4.9
```
sudo ln -s /usr/bin/gcc-4.4 /usr/local/cuda/bin/gcc
sudo ln -s /usr/bin/g++-4.4 /usr/local/cuda/bin/g++
```
## 2. Install CuDNN

* Download https://developer.nvidia.com/compute/machine-learning/cudnn/secure/v5.1/prod/8.0/cudnn-8.0-linux-x64-v5.1-tgz
* Extract and we have 'cuda' folder
* copy cudnn header file to
```
sudo cp ./cuda/include/* /usr/local/cuda/include
```
* copy cudnn lib to 
```

sudo cp ./cuda/lib64/* /usr/local/cuda/lib64
```

## 3. Install TensorFlow

### 3.1 Install Anaconda3
	Install Anaconda 3 for full python 3.5 enviroment support (including python 3.5, matplotlib, numpy, sklearn, ipython ...)
	
	For Python 2.7, download Anaconda 2

	https://www.continuum.io/downloads#linux
### 3.2 Install TensorFlow
	Follows https://www.tensorflow.org/versions/r0.11/get_started/os_setup.html#anaconda-installation

### 3.3 Install tensorFlow with jupyter
    conda install jupyter notebook
