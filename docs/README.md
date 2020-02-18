## Welcome to AISAR!

[![License](http://img.shields.io/:license-mit-blue.svg)](https://github.com/xiechou/AISAR.git)
[![Badges](http://img.shields.io/:badges-7/7-ff6799.svg)](https://github.com/xiechou/AISAR.git)

AISAR is a Python package for InSAR (Interferometric Synthetic Aperture Radar) time series analysis.
It reads stack of orginal SLC data, and produces three dimensional (2D in space and 1D in time) ground displacement.   

### 1. Installation   

#### 1.1 Pre-requisite
We recommend using Anaconda to install the python environment and the prerequisite packages. You will need:   
- [Python2.7](https://www.continuum.io/downloads)
- Numpy
- Scipy
- h5py
- Matplotlib
- 

* Go to the area where you want to install the code:

```
cd ~/aisar
```

* Install the code using the commands below (you need a reasonable recent git version ). 

```
bash
[ -f ~/local_git/miniconda3/bin/git ] && alias git=~/local_git/miniconda3/bin/git	

git clone https://github.com/xiechou/AISAR.git ;
cd aisar


cd setup
rm -r ../3rdparty/miniconda3
miniconda_version=Miniconda3-4.6.14-Linux-x86_64.sh
wget http://repo.continuum.io/miniconda/$miniconda_version --no-check-certificate #; if ($? != 0) exit; 
chmod 755 $miniconda_version
mkdir -p ../3rdparty
./$miniconda_version -b -p ../3rdparty/miniconda3
../3rdparty/miniconda3/bin/conda config --add channels conda-forge
../3rdparty/miniconda3/bin/conda install --yes --file ./conda.txt
```
##### 1.2 AISAR   
To use the package add the path to AISAR directory to your $PYTHONPATH and add AISAR to your $path. Depending on your shell you may use commands such as the following examples to setup pysar:   

    cd ~/Documents/development/python
    git clone https://github.com/xiechou/AISAR.git
   
Then add the following to your source file:
For bash user, add to your .bashrc file:   
    export AISAR_HOME="~/python/AISAR"
    export PYTHONPATH=${PYSAR_HOME}:${PYTHONPATH}   
    export PATH="${PYSAR_HOME}/pysar:$PATH"   
   
  
### 2. Running AISAR


    .py 

   
### 3. Documentation
   