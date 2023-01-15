# Stanford Geothermal Python Sessions -- Beginner

## Workshop Goal

The goal is to provide enough foundation to reduce the frustration of getting started. Learning to code can often feel as futile as picking apart cold spaghetti. A 2 hour python workshop can not cover everything, but we hope to touch on enough that you'll know what to google later. 

- What is Python and why would people learn it?
- Ecosystem: Anaconda, conda, VS Studio Code, terminal, Git (source control), GitHub (website/community)
- How to run Python: in command prompt (shell - python ipython), from a txt file (.py), in a jupyter notebook
- Code along: Introduction to the python language and some key libraries (packages)
- Error reading, debugging, using the internets (blogs, docs, stack overflow, communities).

***
# Setup Instructions

Participants who are new to python:

    We strongly suggest you get set up before the workshop by following the Setup Instructions below. This will guide you through installing Anaconda, which is software designed to make it easy for scientists, engineers and others to start out with python (i.e., no degree in computer science needed). We will run a help cafe just prior to the workshop for anyone having trouble getting set up.

    If you do not have a computer that you can install software on, then you can use the Binder Instance (a web-hosted version) of this tutorial. You will be able to write an execute code into the Binder version, but you will not be able to save your work.  
    
    To use Binder, Click the Binder button below and wait for it to load. The first time you do this, Binder can take up to 10 minutes to load. Click 'show' on the 'Build Logs' bar if you want to watch the Binder environment building. 



More advanced participants:

    You are welcome to use your preferred IDE (Interactive Development Environnement) and approach to managing requirements. 

## Setup Instructions

__Download this tutorial__ from GitHub using the green 'code' button and unzip to somewhere on your computer that is easy to find. We recommend using your Documents folder.

__Download and install [Anaconda individual edition](https://www.anaconda.com/products/individual)__ if you don't already have it. When prompted, accept the default installation settings. See this link for more information on installation for [Windows](https://docs.anaconda.com/anaconda/install/windows/) or for [Mac](https://docs.anaconda.com/anaconda/install/mac-os/).


__Create an environment that contains the packages you need to run this tutorial.__ Using python typically involves assembling existing building blocks that are published as packages (sometimes called libraries). An environment is a place to run a python file that has all of the building blocks required to run it (i.e., the requirements). If you have trouble with this step, please register and come along to the help cafe prior to the workshop. 

In Windows open the anaconda prompt or in macOS open a terminal. Use the prompt/terminal to navigate to where you have saved this repository (hint: use _cd \<path_to_the_repository\>_ to change directory).
 
In the repository folder, you will find an environment.yml file (hint: use _ls_ in MacOS or _dir_ in Windows to list files in your current directory). We will use this file to create an environment that contains the packages we need during the workshop. Execute the following command in the prompt/terminal to create the environment (hint: do not include the $ sign):
 
    $ conda env create -f environment.yml
 
You will see a lot of text scroll past in the the prompt/terminal and may need to respond y + ENTER at some point. The environment is automatically named workshop_env. Once it has built, we need to activate the environment by executing:
 
    $ conda activate workshop_env
 
\(workshop_env\) should now appear on the far left of your current line in the prompt/terminal window. 

__Open the jupyter notebook called 'Code-along.ipynb'.__ Because the previous step put you inside the right environment, you can execute the following command to launch a browser window containing Juypter notebook:

    $ jupyter notebook
 
Jupyter Notebook will open in your default browser as a window. You can use it to open and edit the course material.  

__When you are finished__ with Juypter Notebook, you can close the browser window and go back to the prompt/terminal to kill the process with CTRL + C.

When you come back to the workshop material at a later date, you will probably have to activate the workshop_env environment again before launching Juypter Notebook.
 
 
**Other useful Terminal commands**
 
Print a list of your conda environments
  
    $ conda env list
 
Print a list of what is inside your active environment
  
    $ conda list

To install an additional package into the active environment

    $ pip install <PackageName>


 

 
