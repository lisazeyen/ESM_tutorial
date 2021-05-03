#  :mortar_board: Energy Systems Tutorials

## :books: Worksheets and Material:

The tutorials include both, coding exercises and calculations done by hand.

There's a worksheet for every tutorial: `tutorial-X/worksheet/X-sheet.pdf`

If the tutorial includes coding exercises (some tutorials have no coding exercises),
there are Jupyter Notebooks (`tutorial-X/notebooks/tutorial-X-task-Y.ipynb`) accompanied with required data
and additional hints..

The exercises should be worked through **before** the tutorial. There are exercises which are covered in the tutorial and task which are for studying at home (marked with a house symbol). Questions on both types of tasks are answered in the tutorial and **all tasks are relevant for the exam**.

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


# :abacus: Tutorials via Binder

You can use [Binder](https://mybinder.org/) to directly run code from the Jupyter Notebooks online without a local installation. It will create the necessary software packages and open a Jupyter Notebook from a remote server. To use binder click on the blue badge or follow the link

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lisazeyen/ESM_tutorial.git/master)

https://mybinder.org/v2/gh/lisazeyen/ESM_tutorial.git/master

It might take a moment, so please be patient :upside_down_face:

You should now be ready to do the tutorials in the browser :partying_face:

# :arrow_down: Download

If you prefer to do the tutorials locally with your own Python installation,
first download the tutorials with `git` with the following command:

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

To manage Python environments, we recommend to use `conda` to install the packages required.

Install [`miniconda`](https://conda.io/projects/conda/en/latest/glossary.html#miniconda-glossary) (or Anaconda). For instructions for your operating system see https://conda.io/projects/conda/en/latest/user-guide/install/index.html. 

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

With the `conda` environment installed and activated, open a Jupyter Notebook with the following command in the tutorial folder (where your notebooks are):

```bash
cd /path/where/your/tutorial/folder/should/be
cd ESM_tutorial
jupyter lab
```

or

```bash
cd /path/where/your/tutorial/folder/should/be
cd ESM_tutorial
jupyter notebook
```


