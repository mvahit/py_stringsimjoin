============
Installation
============
 
Requirements
------------
    * Python 3.6, 3.7, 3.8, or 3.9
    * C++ compiler (parts of the package are in Cython for efficiency reasons, and you need C++ compiler to compile these parts) 

Platforms
------------
py_stringsimjoin has been tested on Linux (Ubuntu Xenial 16.04.6), macOS (High Sierra 10.13.6),
and Windows 10.

Dependencies
------------
    * pandas (to manage tables of tuples to be joined)
    * joblib (to write code that runs over multiple cores)
    * py_stringmatching (to tokenize and compute similarity scores between strings)
    * pyprind (to display progress bars)
    * six

.. note::

     The py_stringsimjoin installer will automatically install the above required packages.


C Compiler Required
-------------------
Before installing this package, you need to make sure that you have a C compiler installed. This is necessary because this package contains Cython files. Go `here <https://sites.google.com/site/anhaidgroup/projects/magellan/issues>`_ for more information about how to check whether you already have a C compiler and how to install a C compiler.

After you have confirmed that you have a C compiler installed, you are ready to install the package. There are two ways to install py_stringsimjoin package: using pip or source distribution.

Installing Using pip
--------------------
The easiest way to install the package is to use pip, which will retrieve py_stringsimjoin from PyPI then install it::

    pip install py_stringsimjoin
    
Installing from Source Distribution
-------------------------------------
Step 1: Download the source code of the py_stringsimjoin package from `here
<https://github.com/anhaidgroup/py_stringsimjoin/releases>`_. (Download code in tar.gz format for Linux and OS X, and code in zip format for Windows.)

Step 2: Untar or unzip the package and execute the following command from the package root::

    python setup.py install
    
.. note::

    The above command will try to install py_stringsimjoin into the defaul Python directory on your machine. If you do not have installation permission for that directory then you can install the package in your home directory as follows::

        python setup.py install --user

    For more information see the following StackOverflow `link
    <http://stackoverflow.com/questions/14179941/how-to-install-python-packages-without-root-privileges>`_.
