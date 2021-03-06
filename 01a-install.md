# Install software on your computer


### Install [git](http://git-scm.com/).

You have it installed if you can run `git --version` at the command
line and get output like `git version 2.3.5`.


### Install [Anaconda](http://continuum.io/downloads).

There are two things you can verify to check your install.

First, from the command line, all of the following should start up
some kind of Python interpreter:

```bash
python
ipython
ipython notebook
spyder
```

Second, inside any of those Python interpreters, you should be able to
do all of these without error:

```python
import numpy
import scipy
import matplotlib
import pandas
import statsmodels
import sklearn
```

### Install [Homebrew](http://brew.sh/) on Mac

If you use a Mac, install Homebrew if you don't
have it yet. You could use Homebrew to manage your `git` and `python`
installs as well, but the methods given above are very good and more
cross-platform.

---

### Q1. Python Version 2 or 3

**Course material for the bootcamp is compatible with Python versions 2.7 and 3.0. All HackerRank Python pre-work is configured for Python 3 only.  Therefore, Python 3 is the recommended version.**  

Did you install Python 2 or 3? Why?  

>> I installed Python 3 as it has the latest features and the major libraries like scipy,numpy and other related packages are available in Python3. 
>> Python 2 is planned to phase out by 2020 so I think its better to be acquainted with Python 3 instead of Python 2.

### Q2. Which Python Version Installed   

How can you check the version of Python installed if you happen to be on an unfamiliar computer?

>> Python version can be checked using the Terminal or using one of the Python Interpreters.
>> 
>> In the interpreter by using the following code:
>> ```python 
>> import sys
>> print(str(sys.version_info[0])+'.'+str(sys.version_info[1]))
>> ```
>> 
>> In the Terminal by using the following command:
>> ```console
>> python --version
>> ```
