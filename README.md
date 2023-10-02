# MyPgZero
Learning and tinkering with pgzero

## Setting up in Conda

My prefered environment manager is [Conda](https://conda.io/).  This can be installed
via Anaconda, Miniconda, or Miniforge.  Pgzero is included in the conda-forge repository.
A clean conda-forge environment with pgzero can be set up as follows:

* Install conda and open a shell prompt that can access conda.
* Create a new environment, with a name of your choice:
  * `conda create --name mypgzero`
* Activate the new environment:
  * `conda activate mypgzero`
* If needed, add "conda-forge" to the environment's channel list.
  * `conda config --env --add channels conda-forge`
* How do you know if the above is needed?  Check the environment settings.
  * Method 1: `conda info`: look for "channel URLs".  The top couple of URLs sholud have "conda-forge" in them.
  * Method 2: `conda config --show channels`:  Should list "conda-forge".
  * Method 3: `conda config --show-sources`: Should list "conda-forge".
* Install the pgzero package.  Conda will automatically install all dependencies.
  * `conda install pgzero`
