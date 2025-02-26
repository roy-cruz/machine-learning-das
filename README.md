<!-- ![logo](logo.png) -->

______________________________________________________________________

<p align="center">
  <a href="#introduction">Introduction</a> •
  <a href="#setup">Setup</a> •
  <a href="#links">Links</a> •
  <a href="#credits">Credits</a>
</p>

______________________________________________________________________

[![Jupyter Book Badge](https://jupyterbook.org/badge.svg)](https://FNALLPC.github.io/machine-learning-das)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/FNALLPC/machine-learning-das/HEAD)
[![Codestyle](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/FNALLPC/machine-learning-das/master.svg)](https://results.pre-commit.ci/latest/github/FNALLPC/machine-learning-das/master)

______________________________________________________________________


# CMS Machine Learning Data Analysis School (DAS) Short Exercise


## Introduction

This is a set of tutorials for the LPC Data Analysis School (DAS) Machine Learning Short Exercise. 
They are intended to show you how to build machine learning models in python, using `xgboost`, `Keras`, `TensorFlow`, and `PyTorch`, and use them in your `ROOT`-based analyses. 
We will build event-level classifiers for differentiating VBF Higgs and standard model background 4 muon events and jet-level classifiers for differentiating boosted W boson jets from QCD jets using BDTs, and dense and convolutional neural networks.
We will also explore more advanced models such as graph neural networks (GNNs), variational autoencoders (VAEs), and generative adversarial networks (GANs) on simple datasets.

## Setup

### Vanderbilt Jupyterhub (Recommended!)

The recommended method for running the tutorials live is the Vanderbilt Jupyterhub, follow the instructions [here](https://fnallpc.github.io/machine-learning-das/setup/vanderbilt-jupyterhub/vanderbilt.html).

### FNAL LPC

Not as well supported, but instructions are [here](https://fnallpc.github.io/machine-learning-das/setup/lpc.html).

### Locally

All these notebooks can be run on your local machine as well. 
It can often be useful to test your models and pipelines locally, but it is not recommended to run full trainings as these can be resource-intensive.

To run locally, run these commands from your terminal:

```bash
# Download the setup bash file for your machine from here https://github.com/conda-forge/miniforge#mambaforge
# e.g. wget https://github.com/conda-forge/miniforge/releases/latest/download/Mambaforge-Linux-x86_64.sh
# Install: (the mamba directory can end up taking O(1-10GB) so make sure the directory you're using allows that quota)
chmod u+x Mambaforge-Linux-x86_64.sh
./Mambaforge-Linux-x86_64.sh  # follow instructions in the installation

git clone https://github.com/FNALLPC/machine-learning-das/
cd machine-learning-das
mamba create -f environment.yml
mamba activate machine-learning-das
jupyter lab  # this will create a JupyterLab instance from which you can run all the notebooks.
```

### Binder

You can launch this repository in a "Binder" instance using: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/FNALLPC/machine-learning-das/HEAD),
or for a specific notebook by navigating to the rocket icon on the website and clicking on the Binder option.

![launch_notebooks](figures/launch_notebooks.png)

This may be a more convenient, but it has not been well tested and the set-up time can be slow.

## Setup

### Google Colab

Each notebook can also be launched in a Google Colab instance by clicking "Google Colab" option in the menu bar above. 
To use this, you will have to install any extra libraries needed for the tutorial yourself and re-download the relevant datasets each time.


## Links

The indico page for the DAS is: https://indico.cern.ch/e/cmsdas2024

The Mattermost for live support is: [https://mattermost.web.cern.ch/cmsdaslpc2024/channels/shortexmachinelearning](https://mattermost.web.cern.ch/cmsdaslpc2024/channels/shortexmachinelearning)

The datasets we will use are located here: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3901869.svg)](https://doi.org/10.5281/zenodo.3901869)


## Credits

This project is created using the excellent open source [Jupyter Book project](https://jupyterbook.org/) and the [executablebooks/cookiecutter-jupyter-book template](https://github.com/executablebooks/cookiecutter-jupyter-book).
