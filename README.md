# Stanford Geothermal Python Sessions -- Beginner

## Pain Reduction

The goal is to provide enough foundation to reduce the frustration of getting started. Learning to code can often feel as futile as picking apart cold spaghetti. 

- What is Python and why would people learn it
- Structure: Anaconda, conda, code, code editors (most popular)
- import fly
- Examples: from chem, geophysics, geology, and reservior -- pre-primed code-along
- Running python: in command prompt, from a txt file (.py), in a jupyter notebook 
- Error reading, using the internets. Print debugging.
- Code-along example of building up a bit of code (a plot) non-linear and google some things
- A wee code problem to solve - learning by doing is the best way to learn. Find a wee problem to solve, a calculation, plotting or data handling task. https://automatetheboringstuff.com/  
- Commenting, for future you and others
- On-line (and other) resources for
    1. learning to code
    2. looking up what a particular method does (docs, a big part of coding package knowledge)
    3. Blog posts vs stack overflow vs docs
- Easter egg - zen of python, conventions and syntax
- Find your community - SWUNG, work friend, hackathons etc coding is a social activity. Talking and reading about coding helps.
- Reality check (10 years to learn to code, but useful within a few months)


https://github.com/ddempsey/python_for_geoscientists

***
# Setup Instructions

Get set up before the workshop by installing Anaconda. This is software designed to make it easy for scientists, engineers and others to start out with python (i.e., no degree in computer science needed).

## Anaconda Instructions
 
To run this tutorial, you will need an environment that contains all of the required packages. If you are familiar with setting up your own environment, then go ahead with your usual approach. Otherwise, use the following steps.

Download this tutorial from GitHub using the green 'code' button and unzip to somewhere that is easy to find, such as your Documents folder.
 
Download and instal [Anaconda individual edition](https://www.anaconda.com/products/individual) if you don't already have it. When prompted, accept the default installation settings.

In Windows open the anaconda prompt or in macOS open a terminal. Use the prompt/terminal to navigate to where you have saved this repository (hint: use _cd \<path_to_the_repository\>_ to change directory)
 
In the repository folder, you will find an environment.yml file (hint: use _ls_ in MacOS or _dir_ in Windows to list files in your current directory). We will use this file to create an environment that contains the packages we need during the workshop. Execute the following command in the prompt/terminal to create the environment (hint: do not include the $ sign):
 
    $ conda env create -f environment.yml
 
You will see a lot of text scroll past in the the prompt/terminal and may need to respond y + ENTER at some point. The environment is automatically named workshop_env. Once it has built, we need to activate the environment by executing:
 
    $ conda activate workshop_env
 
\(workshop_env\) should now appear on the far left of your current line in the prompt/terminal window. Now you are inside the right environment, you can execute the following command to launch a browser window containing Juypter notebook:
 
    $ jupyter notebook
 
Now you can open the tutorial notebooks and use them. 

When you are finished with Juypter Notebook, you can close the browser window and go back to the prompt/terminal to kill the process with CTRL + C.
 
When you come back to the workshop material at a later date, you will probably have to activate the workshop_env environment again before launching Juypter Notebook.
 
**Other useful commands**
 
Print a list of your conda environments
  
    $ conda env list
 
Print a list of what is inside your active environment
  
    $ conda list

To install an additional package into the active environment

    $ pip install <PackageName>

***
## Binder Instructions (Backup)

 Click the Binder button below and wait for it to load. The first time you do this, Binder can take up to 10 minutes to load. Click 'show' on the 'Build Logs' bar if you want to watch the Binder environment building. 
 
 When Binder has loaded, it will open the tutorial in Jupyter Lab. You can edit and run the code there. You can also save your work and have it retained during that Binder session. However, once you close your browser, any saved work will be lost. 


BINDER LINK HERE
 

 
