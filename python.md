Introduction to Scientific Computing in Python
==============================================
This is not a programming tutorial, and this will not teach you to do science. This document will lay out a setup for conducting scientific research in the Python programming language, yes; but the primary key to successfully using Python for science is to enjoy it and to work at it. The key is that *you* have to care enough to put time and effort into computing in Python. And if that's your kind of thing, you will learn to totally kick scientific ass in Python. You'll stop programming, and start researching.

Python makes scientific computing seamless in many ways, but it is also not the only tool for conducting analysis. Different contexts demand different approaches to problem-solving. For statistical modeling and graphics, [R](http://www.r-project.org/) can't be beat. [MATLAB](http://www.mathworks.com/products/matlab/) is the dominant language in use in economics, and for good reason: it handles large datasets very well. [Julia](http://julialang.org/) may suit the needs of more algorithmic, large-data research, and FORTRAN, C, RATS, Mathematica and Perl all have many merits. Choose the right tool for the right job, but remember that Python can be a great tool in many contexts.

Once you've found your tool, whether it's Python or something else, you should learn that language, learn it well, learn it until it reads and writes like the back of your hand. Learn to write idiomatic (for the language you're using) code, and learn to do everything in a single language.

Installing Python---for statistical work, geographic work or any other numeric- and data-oriented type of work---is best accomplished with a scientific computing Python distribution such as [Anaconda](https://store.continuum.io/cshop/anaconda/). Among other packages, this will install a handful of Python package managers like pip and conda. These will make it easier obtain packages and keep your Python libraries organized.

Familiarizing yourself with [Git](http://git-scm.com/) will also make your life managing Python easier; packages not available through a package manager can be installed with relative ease from Github.

We primarily use Python in our day-to-day programming, be it simple scripting or extensive software development. Python is a great multi-purpose, fully-featured programming language. Python does it all, and does it easily. Python can reliably be your go-to language for just about any problem.

Two things are worth noting with Python, that might make another language more appropriate for you: Python is an interpreted language, and Python was not designed with science as its primary purpose.

Because Python is interpreted, some programs will run very slowly (see: heavy use of the `for` loop). This is true of any interpreted language (R, MATLAB, Stata), and most computationally intense algorithms will already be implemented very quickly; but at the margins, you might need to use C if heavy computation on very large data is time-sensitive and frequent.

Because Python was not designed specifically for science, many of the scientific features Python has are add-ons. These libraries are robust, reliable, and optimized; but they often operate with an intermediary layer between the Python interpreter and their functions. This doesn't inhibit Python's function-set; it merely means things like linear algebra aren't as direct or simple as in MATLAB, or statistical modeling requires a few more steps than in R.

If you are interested in using Python, you might check out the book _Python for Data Science_, which describes in detail many packages Python has for data analysis and scientific computing.


IPython
=======
Use IPython. There are many, many tutorials on IPython, so I need not go into detail; suffice it to say IPython will change the way you code.

Packages
========
Below are a handful of packages that facilitate Python work in data-heavy and numerical contexts. Uniformly, these data structures, functions and techniques will improve your daily life, in addition to mysterious curative powers and rumors of increased longevity.
* `numpy`
* `pandas`
* `matplotlib`
* `pickle`
* `scipy`
* `cython`
* `networkx`, `sklearn`

GIS in Python
=============
Python has a fairly robust set of modules for doing GIS work. These libraries---a variety of convenience functions, objects, classes, methods---make interacting with and manipulating geographic data intuitive and straightforward.

Packages
--------
* `fiona`
* `pyproj`
* `shapely`
* `geopandas`

Advanced
========
Installing packages from Github
