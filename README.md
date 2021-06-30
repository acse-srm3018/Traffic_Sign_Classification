# Traffic_Sign_Classification

## Description
In this project, the goal is to create a deep learning model to recognize traffic signs. In this project, the deep learning model was built that by training model using German traffic sign images and then classify the unlabeled traffic signs. The deep learning model will be built using tensorflow and we will also understand various ways to preprocess images using OpenCV and also use a cloud GPU service provider.

## Datasets
The Dataset which used in this project is the German Traffic Sign Benchmark is a multi-class, single-image classification challenge held at the International Joint Conference on Neural Networks (IJCNN) 2011. The datasets can be found and downloaded from this [link](https://bitbucket.org/jadslim/german-traffic-signs).
The Image dataset consists of 43 classes (Unique traffic sign images). Training Set has 34799 Images , Test set has 12630 images and the validation set has 4410 images.

## Setup 
### Configure and Manage Your Environment with Anaconda

Per the Anaconda [docs](http://conda.pydata.org/docs):

> Conda is an open source package management system and environment management system 
for installing multiple versions of software packages and their dependencies and 
switching easily between them. It works on Linux, OS X and Windows, and was created 
for Python programs but can package and distribute any software.

Using Anaconda consists of the following:

1. Install [`miniconda`](http://conda.pydata.org/miniconda.html) on your computer, by selecting the latest Python version for your operating system. If you already have `conda` or `miniconda` installed, you should be able to skip this step and move on to step 2.
2. Create and activate * a new `conda` [environment](http://conda.pydata.org/docs/using/envs.html).

\* Each time you wish to work on any exercises, activate your `conda` environment!

---

### 1. Installation

**Download** the latest version of `miniconda` that matches your system.

|        | Linux | Mac | Windows | 
|--------|-------|-----|---------|
| 64-bit | [64-bit (bash installer)][lin64] | [64-bit (bash installer)][mac64] | [64-bit (exe installer)][win64]
| 32-bit | [32-bit (bash installer)][lin32] |  | [32-bit (exe installer)][win32]

[win64]: https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86_64.exe
[win32]: https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86.exe
[mac64]: https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
[lin64]: https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
[lin32]: https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86.sh

**Install** [miniconda](http://conda.pydata.org/miniconda.html) on your machine. Detailed instructions:

- **Linux:** http://conda.pydata.org/docs/install/quick.html#linux-miniconda-install
- **Mac:** http://conda.pydata.org/docs/install/quick.html#os-x-miniconda-install
- **Windows:** http://conda.pydata.org/docs/install/quick.html#windows-miniconda-install

### 2. Create and Activate the Environment

For Windows users, these following commands need to be executed from the **Anaconda prompt** as opposed to a Windows terminal window. For Mac, a normal terminal window will work. 

1. **Clone** the repository, and navigate to the downloaded folder. This may take a minute or two to clone due to the included image data.
  
  ```sh
  git clone https://github.com/wolfapple/traffic-sign-recognition.git
  cd traffic-sign-recognition
  ```

2. **Create** (and activate) a new environment, named `traffic-sign-recognition`. Running this command will create a new `conda` environment that is provisioned with all libraries you need to be successful in this program.
  
  - __Linux__ or __Mac__: 
  ```sh
  conda env create -f environment.yaml
  source activate traffic-sign-recognition
  ```
  - __Windows__: 
  ```sh
  conda env create -f environment.yaml
  activate traffic-sign-recognition
  ```
  
  At this point your command line should look something like: `(traffic-sign-recognition) <User>:traffic-sign-recognition <user>$`. The `(traffic-sign-recognition)` indicates that your environment has been activated, and you can proceed with further package installations.

3. **Verify** that the environment was created in your environments:  
  
  ```sh
  conda info --envs
  ```

4. **Cleanup** downloaded libraries (remove tarballs, zip files, etc):
  
  ```sh
  conda clean -tp
  ```

5. **That's it!**
  
  Now most of the libraries are available to you. Very occasionally, you will see a repository with an addition requirements file, which exists should you want to use TensorFlow and Keras, for example. In this case, you're encouraged to install another library to your existing environment, or create a new environment for a specific project.
  
  To exit the environment when you have completed your work session, simply close the terminal window.
  
### 3. Uninstalling

To uninstall the environment:

  ```sh
  conda env remove -n traffic-sign-recognition
  ```

### Dependencies
Install all the dependencies:
- Tensorflow
- Keras
- Numpy
- Pandas
- Pickle
- Matplotlib

### Run 
Run the ipython notebook file traffic_sign.ipynb using jupyter notebook
