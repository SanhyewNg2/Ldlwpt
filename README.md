# Sanhyew's Notebook: "Learning Deep Learning with PyTorch"


## What is this notebook?

This notebook is my recording and refinement on the materials and experiments of deep learning with PyTorch.

Originally I was an Electro-Optics engineer that focuses on camera systems. At that time, my research area was digital image processing including image enhancement, multi-spectral image fusion and so on. I recognized that deep learning is my continuous research direction, so I get into deep learning using Python. 

After a while, after a lot of studies and practices, I thought it is necessary for me  to record and refine all materials and experiments in an organized structure. I think Jupyter notebook is the best recording tool of code execution. A typical sample is the book ["Dive Into Deep Learning"](https://d2l.ai/). This book made my thought solidified.

Every person has his mode and way in doing anything. And I think making his own things makes him clever. This notebook is a result of such thinking.


### Features of this notebook:

* The best writings taken from all available resources (books, documentations, courses, and so on) 
* Better structured (organized) from basic to advanced 
* Continuously updated 

by Sanhyew Ng



-------------------------------
## Installation


### Python Environment

If you’re in between “beginning” and “advanced”, 
    please go with “beginning” if you want to keep things simple, 
    and with “advanced” if you want to work according to best practices that go a longer way in the future.


#### BEGINNING USERS

On all of Windows, macOS, and Linux:

 - Install [Anaconda](https://www.anaconda.com/distribution/) (it installs all packages you need and all other tools mentioned below).
 - For writing and executing code, use notebooks in [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/index.html) for exploratory and interactive computing, and [Spyder](https://www.spyder-ide.org/) or [Visual Studio Code](https://code.visualstudio.com/) for writing scripts and packages.
 - Use [Anaconda Navigator](https://docs.anaconda.com/anaconda/navigator/) to manage your packages and start JupyterLab, Spyder, or Visual Studio Code.


#### ADVANCED USERS


##### Windows or macOS

 - Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
 - Keep the `base` conda environment minimal, and use one or more [conda environments](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#) to install the package you need for the task or project you’re working on.
 - Unless you’re fine with only the packages in the defaults channel, make conda-forge your default channel via [setting the channel priority](https://conda-forge.org/docs/user/introduction.html#how-can-i-install-packages-from-conda-forge).


##### Linux
If you’re fine with slightly outdated packages and prefer stability over being able to use the latest versions of libraries:
 - Use your OS package manager for as much as possible (Python itself, NumPy, and other libraries).
 - Install packages not provided by your package manager with pip install somepackage --user.

If you use a GPU:
 - Install [Miniconda](https://docs.conda.io/en/latest/miniconda.html).
 - Keep the `base` conda environment minimal, and use one or more [conda environments](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#) to install the package you need for the task or project you’re working on.
 - Use the defaults conda channel (conda-forge doesn’t have good support for GPU packages yet).


#### Alternative if you prefer pip/PyPI

For users who know, from personal preference or reading about the main differences between conda and pip below, they prefer a pip/PyPI-based solution, we recommend:
 - Install Python from [python.org](https://www.python.org/downloads/), [Homebrew](https://brew.sh/), or your Linux package manager.
 - Use [Poetry](https://python-poetry.org/) as the most well-maintained tool that provides a dependency resolver and environment management capabilities in a similar fashion as conda does.


### Python Packages

You should be able to create 
a new environment as follows:

```bash
conda create --name Sanhyew_Ldlwpt python=3.10
conda activate Sanhyew_Ldlwpt
```

Before installing any deep learning framework, please first check whether or not
you have proper GPUs on your machine (the GPUs that power the display on a standard laptop are not relevant for our purposes).
For example, if your computer has NVIDIA GPUs and has installed [CUDA](https://developer.nvidia.com/cuda-downloads), then you are all set.

If your machine does not house any GPU, there is no need to worry just yet.
Your CPU provides more than enough horsepower to get you through the first few chapters. Just remember that you will want to access GPUs before running larger models.

To install the the CPU version, execute the following command.
```bash
conda install pytorch torchvision torchaudio torchtext cpuonly -c pytorch
```

The next step is to install
the `d2l` package that encapsulates
frequently used functions and classes:

```bash
pip install d2l
```

## Running and Editing Codes

Now we can start the Jupyter Notebook server by running:

```bash
jupyter notebook
```

At this point, you can open http://localhost:8888 (it may have already opened automatically) in your Web browser.
Then we can run the code for each section of the book.

Better option is to use [VS Code](https://code.visualstudio.com/).

