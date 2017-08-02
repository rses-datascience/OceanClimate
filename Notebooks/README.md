# Ocean Science Notebooks

This folder contains various [Jupyter Notebooks](http://jupyter.org/) with tutorials and data processing examples.

## Contents

### Tutorials
* [Python very-basics](Tutorials/Python_Very_Basics.ipynb)

### Examples
* [Anand2003_Reprocessing](Examples/Anand2003_Reprocessing.ipynb): A detailed example of using Python and Jupyter Notebooks to reproduce the Mg/Ca-Temperature relationship of [Anand et al, 2003](http://dx.doi.org/10.1029/2002PA000846).

## How to use these Notebooks

Notebooks can be read online by clicking on the links above, or downloaded and run on your own computer. If you'd like to do the latter, you need to install a few things first. There are three sets of instructions below - follow either, as appropriate.

### Option 1: Complete Beginner

If you've never touched python before, or are feeling intimidated by Terminal windows, this is for you. It's the simplest possible 'way in' to Python and Jupyter. In future, you might want to transition to Option 2... but this'll do for now.

1. Install [Anaconda](https://www.continuum.io/downloads).
    This is a commercially maintained Python 'distribution', which contains curated versions everything you'll need to get started. Anaconda is designed to be reliable and stable, so might not always have the very latest versions of packages, but it's *more* than enough to get you started.
2. Launch the [Anaconda Navigator](https://docs.continuum.io/anaconda/navigator/) app.
    This provides a user-friendly, graphical ('point and click') way in to Python and Jupyter, where you can install/uninstall modules, manage 'environments' and launch Notebooks without having to go near a terminal. If you're so inclined, you can also launch a Notbeook from the terminal by typing `jupyter notebook`.
3. Pyth-ON!


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
4. Pyth-ON!

### Option 3: Experienced User
If you're a Python officionado, just make sure you have Jupyter and dependecies installed.
