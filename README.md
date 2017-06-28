# Ubuntu 16.04 for Python3 Data Scientist
This repository contains Dockerfile of [Python3](https://www.python.org/download/releases/3.0/) for Docker's automated build published to the public [Docker Hub Registry](https://hub.docker.com/).

## Base Docker Image
* dockerfile/ubuntu

## Python 3 Packages

### Fundamentals
* NumPy
* SciPy
* Pandas
* Jupyter
* PIL

### Math and Statistics
* SymPy
* Statsmodels

### Machine Learning
* Theano
* Tensorflow
* Keras
* Gensim
* SciKit-Learn
* NLTK

### Plotting and Visualization
* MatPlotLib
* Bokeh
* Ggplot
* Seaborn

### Profiling
* memory profiler
* line profiler

## Installation 
1. Install [Docker](https://docs.docker.com/engine/installation/).
2. Download automated build from public [Docker Hub Registry](https://hub.docker.com/): 
```{engine=bash}
docker pull alessandroadamo/ubuntu-ds-python3
```
alternatively, you can build an image from Dockerfile: 
```{engine=bash}
docker build -t="alessandroadamo/ubuntu-ds-python3" github.com/alessandroadamo/ubuntu-ds-python3
```

## Usage

### Run Interactively
```{engine=bash}
sudo docker run -it alessandroadamo/ubuntu-ds-python3 /bin/bash
```

### Run Jupyter
```{engine=bash}
docker run -d -p 8888:8888 -v [your path]:/home/ds/notebooks alessandroadamo/ubuntu-ds-python3
```
