#  :mortar_board: ESM	Tutorial Structure

## :books: Worksheets and Material:

The tutorials include both, coding exercises and calculations done by hand.

There's a worksheet (`X-sheet.pdf`) for every tutorial in `X-tutorial-date/worksheet`.

If the tutorial includes coding exercises (some tutorials have no coding exercises),
there are `jupyter notebooks` (`tutorial-X-task-Y.ipynb`) and data sources provided in `X-tutorial-date/notebooks/data`.

# :blue_book: Python Tutorials

In the tutorials we will repeatedly work with the programming language Python. If you are unfamiliar with the language, you might find the following tutorials useful.

The [Python notebook based notes of Robert Johansson](http://nbviewer.jupyter.org/github/jrjohansson/scientific-python-lectures/tree/master/) are a
comprehensive kick starter.
 * [Lecture 0](http://nbviewer.jupyter.org/github/jrjohansson/scientific-python-lectures/blob/master/Lecture-0-Scientific-Computing-with-Python.ipynb) covers installation and getting ready.
 * [Lecture 1](http://nbviewer.jupyter.org/github/jrjohansson/scientific-python-lectures/blob/master/Lecture-1-Introduction-to-Python-Programming.ipynb)
       zooms through most basic general python control structures (only
       brush over it and stop reading early, i.e. if you read the word
       `classes` you already know too much).
 * [Lecture 2](http://nbviewer.jupyter.org/github/jrjohansson/scientific-python-lectures/blob/master/Lecture-2-Numpy.ipynb) is the most important and closely connected to the exercises.
* You might as well stop now, but if you are hooked, have a look at [Lecture 3](http://nbviewer.jupyter.org/github/jrjohansson/scientific-python-lectures/blob/master/Lecture-3-Scipy.ipynb) for more physics and [Lecture 4](http://nbviewer.jupyter.org/github/jrjohansson/scientific-python-lectures/blob/master/Lecture-4-Matplotlib.ipynb) for prettier graphs.

Further reference material of help is are the website-books http://python-course.eu/ (English), http://python-kurs.eu/ (German); especially of interest might be the [pandas](http://www.python-course.eu/pandas.php) bit in the end, which will make the exercises a breeze at the expense of yet another package to learn.

# :arrow_down: Downloading Tutorial Material

You can download the tutorials with `git` with the following command:

```bash
cd /path/where/your/tutorial/folder/should/be
git clone https://github.com/lisazeyen/ESM_tutorial.git
```
or if you have `ssh` setup at github:
```bash
cd /path/where/your/tutorial/folder/should/be
git clone git@github.com:lisazeyen/ESM_tutorial.git
```


Alternatively, (not as nice as description above) you can download the tutorials as compressed zip-file from
https://github.com/lisazeyen/ESM_tutorial/archive/master.zip

# :wrench: Installation Guide

**If you happen to come across this before the tutorials start,
you may already want to follow the installation instructions already to get started right away, if you face any problems, see next section**

We recommend using the package manager and environment management system `conda` to install the packages we need.

Install [`miniconda`](https://conda.io/docs/user-guide/install/index.html) (or Anaconda). For instructions for your operating system
see https://conda.io/docs/user-guide/install/index.html. 

Create a new `conda` environment from the provided `environment.yml` file with the following set of commands:

Windows:
```bash
conda env create -f environment.yml
activate esm-tutorials
```

macOS and Linux:
```bash
conda env create -f environment.yml
conda activate esm-tutorials
```

On some older Linux installations the last command can be instead

```bash
source activate esm-tutorials
```

For detailed instructions see
https://conda.io/docs/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file.
It will take some time!

With the `conda` environment installed and activated, open a jupyter notebook/lab with the following command in the tutorial folder (where your notebooks are):

```bash
cd /path/where/your/tutorial/folder/should/be
cd esm-tutorials
jupyter lab
```

or

```bash
cd /path/where/your/tutorial/folder/should/be
cd esm-tutorials
jupyter notebook
```
# :ok_woman: Problems with installation

if there are problems with installing and updating the environment you can use ['Binder'](https://mybinder.org/). It will create the enivironment and open a jupyter notebook. To use binder click on the blue badge or follow the link

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lisazeyen/ESM_tutorial.git/master)

https://mybinder.org/v2/gh/lisazeyen/ESM_tutorial.git/master

You should now be ready to do the tutorials :thumbsup:

