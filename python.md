Scientific Computing in Python
=============

Introduction to Scientific Computing in Python
============
This is not a programming tutorial, and this will not teach you to do science. This document will lay out a setup for conducting scientific research in the Python programming language, yes; but the primary key to successfully using Python for science is to enjoy it and to work at it. The key is that *you* have to care enough to put time and effort into computing in Python. And if that's your kind of thing, you will learn to totally kick scientific ass in Python. You'll stop programming, and start researching.

Python makes scientific programming seamless in many ways, but it is also not the only tool for conducting analysis. Different contexts demand different approaches to problem-solving. For statistical modeling and graphics, [R](http://www.r-project.org/) can't be beat. [MATLAB](http://www.mathworks.com/products/matlab/) is the dominant language in use in economics, and for good reason: it handles large datasets very well. [Julia](http://julialang.org/) may suit the needs of more algorithmic, large-data research, and FORTRAN, C, RATS, Mathematica and Perl all have many merits. Choose the right tool for the right job, but remember that Python can be a great tool in many contexts.

Python has a fairly robust set of modules for doing GIS work. These libraries---a variety of convenience functions, objects, classes, methods---make interacting with and manipulating geographic data intuitive and straightforward.

Installing Python---for geographic work, statistical work or any other numeric- and data-oriented type of work---is best accomplished with a scientific computing Python distribution such as [Anaconda](https://store.continuum.io/cshop/anaconda/). Among other packages, this will install a handful of Python package managers like pip and conda. These will make it easier obtain packages and keep your Python libraries organized.

Familiarizing yourself with [Git](http://git-scm.com/) will also make your life managing Python easier; packages not available through a package manager can be installed with relative ease from Github.

Packages
========
Below are a handful of packages that facilitate Python work in data-heavy and numerical contexts. Uniformly, these data structures, functions and techniques will improve your daily life, in addition to mysterious curative powers and rumors of increased longevity.
* `numpy`
* `pandas`
* `matplotlib`
* `pickle`
* `scipy`
* `networkx`, `sklearn`

GIS in Python
=============
Packages
--------
* `fiona`
* `pyproj`
* `shapely`
* `geopandas`

Advanced
========
Installing packages from Github
