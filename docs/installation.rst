Installation
======

Build Environment
--------

**Required Dependencies:**

- R: ``R>=4.0``, ``coda``, ``ggmcmc``, ``rcpp``, ``RcppArmadillo``.
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

**Note:**
  
Test Installation
--------
Todo
