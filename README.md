# Stanford Geothermal Python Sessions -- Beginner

## Workshop Outline

This workshop is designed to reduce frustration of getting started. We can't cover everything in a short workshop, but I hope to touch on enough that you'll know what to google as you embark on your Python journey. 

Topics covered:
- What is Python and why (geothermal) people would use it
- The code ecosystem: Anaconda, conda, VS Studio Code, terminal, Git (source control), GitHub (website), and more
- How to run Python in command prompt (shell - python, ipython), from a txt file (.py), and in a jupyter notebook (.ipynb)
- Introduction to some elements of the python language and some key 'packages'
- Error reading, debugging, effective use of the internet (blogs, docs, stack overflow, communities)

***
# Setup Instructions

__Participants who are new to python:__

You will need to set up your computer before the workshop by following the instructions below that guide you through installing the Anaconda software package. Anaconda designed to make it easy for scientists, engineers and others to start using with Python.

Anaconda is free to use for students and people doing individual projects. People who work in large corporations need to buy a license to use Anaconda. The start of Rob's [introduction to Python](https://www.youtube.com/watch?v=wF9ZlPOCwIc&t=193s) describes how to use just 'conda', which people in large corporations can do without breaching any software license agreements. Because it works 'out of the box', I would recommend using Anaconda if you can. 

If you do not have a computer that you can install software on, then you can use the 'Binder Instance' of this tutorial. It is a web-hosted version of the tutorial inside which you will be able to write an execute code. However, you will not be able to save your work.  
    
To use Binder, click the button below and wait for it to load. The first time you do this, Binder can take up to 5 - 10 minutes to load, so do this for the first time before coming to the workshop. Click 'show' on the 'Build Logs' bar if you want to watch the Binder instance building. 

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ICWallis/Stanford-Geothermal-Python-Sessions--Beginner/main)

I will run a help session on the Friday prior to the workshop for anyone having trouble getting set up. You must register by Wednesday 1 February to attend this.

__More advanced participants:__

You are welcome to use your preferred IDE (Interactive Development Environnement) and method of managing requirements. 

## Setup Instructions

__Download this tutorial__ from GitHub (you're here now), use the green 'code' button (near the top, right) to download these files as a zip. This set of files hosted on GitHub is referred to as a 'repository' or 'repo'. Unzip the repository somewhere on your computer that is easy to find and is not buried too deep in your file system. I recommend your Documents folder.

__Download and install [Anaconda distribution](https://www.anaconda.com/products/distribution)__ (previously called individual edition). When prompted, accept the default installation settings. For more information on installation, see [this for Windows](https://docs.anaconda.com/anaconda/install/windows/) or for [this for Mac](https://docs.anaconda.com/anaconda/install/mac-os/).

[This video](https://www.youtube.com/watch?v=FdatS_NKVrM) is a couple of years old, but still nicely demonstrates the Anaconda download process and how to work with the terminal/anaconda prompt. 

As demonstrated in the video, we should install a package in the Anaconda "base" environment that enables you to use all kernels when running the Jupyter Lab IDE. In Windows, open the anaconda prompt (search for it in the start menu or look under the Anaconda software group). In macOS, open a terminal. The start of the line of text that appears should read '(base)' and this tells you that you are in the 'base' conda environment (more on this later). Type the following command and hit enter to execute the command (hint: do not include the $ sign, copy-paste usually also works): 

    $ conda install nb_conda_kernel

__Create an environment that contains the packages you need to run this tutorial.__ Using Python typically involves assembling existing building blocks that were published as 'packages'. An environment is a place that contains all of the required building blocks (referred to as the 'requirements' or 'dependencies') that you need to run a given Python file. The requirements for this tutorial are listed in the environment.yml file.

In Windows, open the anaconda prompt. In macOS, open a terminal. Use the prompt/terminal to navigate to where you have saved this repository (hint: use _cd \<path_to_the_repository\>_ to change directory). [This tutorial and video](https://medium.com/geekculture/basic-bash-commands-c54933183c89) demo's how to navigate with the prompt/terminal.
 
Once you have navigated into the repository folder, you will find the environment.yml file (hint: use _ls_ in MacOS or _dir_ in Windows to list files in your current directory). We will use this file to create an environment that contains the packages needed during the workshop. Execute the following command in the prompt/terminal to create the environment:
 
    $ conda env create -f environment.yml
 
This will take a few minutes and will see a lot of text scroll past in the the prompt/terminal. You may need to respond y then press ENTER if asked to do so. The environment is automatically named sgw_env. Once it has built, we need to activate the environment by executing:
 
    $ conda activate sgw_env
 
\(sgw_env\) should now appear at the start of your current line in the prompt/terminal window.

Refer to [this page](https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) for mor information on making and managing conda environments.

__Open the jupyter notebook called 'Code-along.ipynb'.__ Because the previous step put you inside the right environment (conda activate sgw_env), you can now launch the Jupyter lab IDE (interactive development environnement, where you will write/run code). Into your terminal/prompt type the following and it return:

    $ jupyter lab
 
This command will launch Jupyter Lab inside your default browser application. Jupyter Lab will run on any modern browser (e.g., firefox, chrome), but may have issues with historic browsers (e.g., safari).

__When you are finished__ with Juypter Lab, close the browser window and go back to the prompt/terminal to 'kill the process'. This is done by clicking on the prompt/terminal and typing CTRL + C.

When you come back to the workshop material at a later date, you may have to activate the sgw_env environment again before launching Juypter Lab. 

There are other ways to make environments and launch jupyter lab (or other code editors) using the Anaconda "navigator" software. However, I strongly recommend you take the time to get familiar with using the prompt/terminal. 
 
 
**Other useful Terminal commands**
 
Print a list of your conda environments
  
    $ conda env list
 
Print a list of what is inside your active environment
  
    $ conda list

To install an additional package into the active environment

    $ pip install <PackageName>


 

 
