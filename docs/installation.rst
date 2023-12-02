Installation
======

Build Environment
--------

**Required Dependencies:**

- R: ``R>=4.0``
- Python: ``R>=3.8``

**R Packages:**

- ``code==0.19-4``
- ``ggmcmc==1.5.1.1``
- ``Rcpp==1.0.9``
- ``RcppArmadillo==0.11.2.3.1``
- ``rjson==0.2.21``

**Python Packages**

- ``matplotlib==3.7.2``
- ``pandas==2.0.3``
- ``scipy==1.10.1``
- ``scikit-learn==1.3.0``
- ``numpy==1.24.3``

We strongly recommend using conda to manage the installation of all dependencies. To set up the environment and install specific versions, run the following commands:
::

  conda create --name spacia
  conda activate spacia
  # conda config --add channels conda-forge # If you do not have this channel added before
  conda install r-base=4.0.5 r-coda=0.19-4 r-ggmcmc=1.5.1.1 r-rcpp=1.0.9 r-RcppArmadillo=0.11.2.3.1 r-rjson=0.2.21
  conda install python=3.8 pandas=2.0.3 scikit-learn=1.3.0 numpy=1.24.3 scipy=1.10.1 matplotlib=3.7.2

Then, download this repo.
::

  git clone [repo_path]

The total installation time is around 10 minutes. If an error occurs, please upgrade pip and try again.

Note: If you are on a macOS and do not have the Xcode Command Line Tools installed, please do so by running ``xcode-select --install`` in terminal.
  
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

Note: You may get some warning messages from the Rcpp package, but this does not affect the performance of the software.

**About the test data**

The test data is a randomly generated dataset for the purpose of validating the installation only.

The test itself contains ~2,500 cells and it should finish in 5 minutes.

The purpose of the test is only to validate the installation, and the there is no interpretation associated with the test results.

We have also included the simulation dataset used in our manuscript in ``/data/simulation``.
