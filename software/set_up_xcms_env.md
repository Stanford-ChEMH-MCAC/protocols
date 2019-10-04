## Install mamba

1. Download the appropriate install script for your machine from [the QuantStack website](https://quantstack.net/mamba.html).
	* E.g. for Mac, the link is `https://github.com/QuantStack/mamba/releases/download/0.0.7/minimamba-0.0.7-MacOSX-x86_64-py37.sh`
	
2. Run the installer.
	* E.g. `bash minimamba-0.0.7-MacOSX-x86_64-py37.sh` at the command line.
	* At prompts, choose all the default/recommended values.

## Set up a new environment for your XCMS

1.  Do `mamba create -n xcms-test python=3.7` at a command line.  This will create an (almost)-empty environment called `xcms-test`
2. Activate the new environment with `conda activate xcms-test`
3. Install mamba in the new environment with `conda install mamba`.
4. If not done already, make sure bioconda and conda-forge are in your default channels:
		```
		conda config --add channels defaults
		conda config --add channels bioconda
		conda config --add channels conda-forge
		```
## Install XCMS

1. Run this command `mamba install -c bioconda bioconductor-xcms`
		* This will install R and xcms in your new environment.  Installing the most critical package first is a way to ensure that the version of all other required software (e.g. R) will be compatible with the installed software.
		
2. Verify that you can run xcms:
	1.  Start R (at the command line, enter `r`)
	2.  At the R prompt (`>`), enter `require(xcms)`.  See if it loads without an error.  If so, we're rolling!
		* Note: This message or ones like it are *not* error messages.  They are just warnings:
			  ```Warning message:
				  In fun(libname, pkgname) :
				  mzR has been built against a different Rcpp version (1.0.1)
				  than is installed on your system (1.0.2). This might lead to errors
				  when loading mzR. If you encounter such issues, please send a report,
				  including the output of sessionInfo() to the Bioc support forum at 
				  https://support.bioconductor.org/. For details see also
				  https://github.com/sneumann/mzR/wiki/mzR-Rcpp-compiler-linker-issue.
			  ```
	* Installing XCMS is the hardest, as it requires Rcpp, R, and also Fortran and C++ compilers to be installed on your machine and accessible to R.  The compiled binaries offered in conda are also updated less frequently than those for many other R packages.  So if e.g. try to install R first, then XCMS, you might see that mamba or conda is forced to downgrade your R.
	
## Install other stuff
	
1. To run Jupyter notebooks and use R in them:
		`mamba install -c conda-forge jupyter nb_conda r-irkernel` installs Jupyter and the nb-conda kernel manager.  This makes it possible to use your new XCMS and R installation in Jupyter.
		
2. `mamba install -c conda-forge r-stringi r-tidyverse r-cowplot r-janitor r-viridis r-ggfortify r-ecipex` installs the essential suite of packages for data manipulation in R.
	* For reasons I don't understand, it was required to do `mamba update -c conda-forge r-stringi` to get tidyverse things to start working.  
	
	
## Trying out a Jupyter notebook

You made it!

In this directory is an example Jupyter notebook, `example_xcms_notebook.ipynb`, which downloads files from a MASSive, a repository for raw MS data, and analyzes it in R.

If your install is working you should be able to launch this notebook by doing `jupyter notebook example_xcms_notebook.ipynb &` and begin interacting with it.
