# MyPgZero
Learning and tinkering with pgzero

## Setting up in Conda

My prefered environment manager is [Conda](https://conda.io/).  This can be installed
via Anaconda, Miniconda, or Miniforge.  Either way, a clean pgzero environment can be
set up as follows:

* Install conda and open a shell prompt that can access conda.
* Create a new environment, with a name of your choice:
  * `conda create --name mypgzero`
* Activate the new environment:
  * `conda activate mypgzero`
* Add "conda-forge" to the environment's channel list.
  * `conda config --env --add channels conda-forge`
* Check the environment settings.  The `conda-forge` channel should before `defaults`.
  * Method 1: `conda info`: look for "channel URLs".  The top couple of URLs sholud have "conda-forge" in them.
  * Method 2: `conda config --show channels`:  Should list "conda-forge" before "defaults".
  * Method 3: `conda config --show-sources`: Should list "conda-forge" in the environment's .condarc file.
* Install the pgzero package.  Conda will automatically install all dependencies.
  * `conda install pgzero`
