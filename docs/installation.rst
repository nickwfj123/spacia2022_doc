Installation
======

Build Environment
--------

**Required Dependencies:**

- R: ``R>=4.0``, ``coda``, ``ggmcmc``, ``rcpp``, ``RcppArmadillo``, ``rjson``.
- Python: ``R>=3.8``, ``matplotlib``, ``pandas``, ``scipy``, ``scikit-learn``. 

We strongly recommend using conda to manage the installation of all dependencies. To do this, simply run:
::

  conda create --name spacia
  conda activate spacia
  # conda config --add channels conda-forge ##If you do not have this channel added before#
  conda install r-base=4.0 r-coda r-ggmcmc r-rcpp r-RcppArmadillo
  conda install python=3.8 pandas scikit-learn numpy scipy matplotlib


Download Repo
--------
Download this repo:

::

  git clone [repo_path]

The total installation time is around 10 mintunes. If error occuors, please upgrade pip and try again.

**Note:**  If you are on a macOS and do not have the Xcode Command Line Tools installed, please do so by running ``xcode-select --install`` in terminal.
  
Test Installation
--------
Test Spacia using a simple test script by: 
``python test.py``

The output should look like this:
::

  Testing Spacia with a single gene as response feature and simple aggregation
  Test Succeeded.
  Testing Spacia with multiple genes as response feature and no agg mode
  Test Succeeded.
  Testing Spacia with multiple genes as response feature and pca agg mode
  Test Succeeded.
