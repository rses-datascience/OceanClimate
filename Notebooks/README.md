# Ocean Science Notebooks

This folder contains various [Jupyter Notebooks](http://jupyter.org/) with tutorials and data processing examples relevant to the ocean sciences.

## Contents

### Tutorials
* [Python very-basics](Tutorials/Python_very-basics.ipynb)
<!-- * [Git very-basics](Tutorials/Git_Very_Basics.ipynb) -->

### Examples
* [Anand2003_Reprocessing](Examples/Anand2003_Reprocessing.ipynb): A detailed example of using Python and Jupyter Notebooks to reproduce the Mg/Ca-Temperature relationship of [Anand et al, 2003](http://dx.doi.org/10.1029/2002PA000846).

## How to use these Notebooks

Notebooks can be read online by clicking on the links above, or downloaded and run on your own computer. If you'd like to do the latter, you need to install a few things first. There are three sets of instructions below - pick one, as appropriate.

### Option 1: Complete Beginner

If you've never touched Python before, or are feeling intimidated by Terminal windows, this is for you. It's the simplest possible 'way in' to Python and Jupyter. In future, you might want to transition to Option 2... but this approach is totally fine, and it won't stop you doing anything.

1. Install [Anaconda](https://www.continuum.io/downloads).
    This is a commercially maintained Python 'distribution', which contains curated versions everything you'll need to get started. Anaconda is designed to be reliable and stable, so might not always have the very latest versions of packages, but it's *more* than enough to get you started.
2. Launch the [Anaconda Navigator](https://docs.continuum.io/anaconda/navigator/) app.
    This provides a user-friendly, graphical ('point and click') way in to Python and Jupyter, where you can install/uninstall modules, manage 'environments' and launch Notebooks without having to go near a terminal. If you're so inclined, you can also launch a Notbeook from the terminal by typing `jupyter notebook`.

You now have Python and Jupyter Notebooks installed on your computer. This next bit will download the contents of the OceanScience repository to your computer, so you can run it yourself.

1. [Download and install Git](https://git-scm.com/downloads)
2. [Download and install SourceTree](https://www.sourcetreeapp.com/), a user-friendly graphical interface to Git.
3. In the 'repository browser' of SourceTree click '+ New Repository' and choose 'Clone from URL'. Paste `https://github.com/rses-datascience/OceanClimate` into the 'Source URL' box, specify where you'd like to save it in the box below, and click 'Clone'.

You now have the entire OceanScience repository on your computer, in a run-able and modify-able state! Whenever you open SourceTree in future, it will tell you if there are any updates that you can download ('Pull') from the repository.

If you're just getting started in Python, I recommend going over the [Python very-basics](Tutorials/Python_very-basics.ipynb) Notebook for some tips.

### Option 2: Dedicated Beginner / Intermediate

1. Install [Docker](https://www.docker.com/).
    Docker provides a convenient way of installing software so that it 'just works' on any computer or platform.
2. Install the [Jupyter Data Science docker 'container'](https://hub.docker.com/r/jupyter/datascience-notebook/) that has everything you need to get started in Jupyter Notebook. To do this, make sure docker is running (open the application), then open a terminal window and type:"
```bash
docker pull jupyter/datascience-notebook
```
3. Start the 'container' by replacing `my_path` in the following with your desired directory, and running:
```bash
docker run -it --rm -p 8888:8888 -v /my_path/:/home/jovyan/work jupyter/datascience-notebook
```
4. [Download and install Git](https://git-scm.com/downloads)
5. [Download and install SourceTree](https://www.sourcetreeapp.com/), a user-friendly graphical interface to Git.
6. In the 'repository browser' of SourceTree click '+ New Repository' and choose 'Clone from URL'. Paste `https://github.com/rses-datascience/OceanClimate` into the 'Source URL' box, specify where you'd like to save it in the box below, and click 'Clone'.
7. Pyth-ON!

### Option 3: Experienced User
If you're a Python officionado, just make sure you have Git, Jupyter and all dependecies installed, and clone the OceanClimate repository.