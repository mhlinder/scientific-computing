Scientific Computing for Scientists
===================================

## Manifesto
Why practice scientific computing? Scientific computing is not merely using computers as an aid to science; it's intelligently using computers to organize and process data, and to write up the results of empirical work and simulation.

Science need not be something Professional Researchers pawn off to their RAs.

### Leave a paper trail
* Documentation / Latex

[Git](http://git-scm.com/) is version control software, which will keep track of changes you make to files---code, documentation, data---and allow you to look back into the history of your projects. Git is a killer app for project management and version control: you can set up a [workflow](https://www.atlassian.com/git/workflows) defining your interaction with your files, or design your own. You can learn git [here](http://gitready.com/) or [here](http://git-scm.com/book).

### Learn how to use your tools
* Google
* The terminal
* Package management / Homebrew
* Excel
* A text editor

### Learn how to program
* General-purpose languages: Python, R, MATLAB
* Specific-purpose languages: Awk, Sed, Bash, Stata

## Tools
### A text editor
A text editor is an important component of scientific computing: it's a primary interface for manipulating files and code. It's a personal choice. Just don't use Notepad.

[Vim](http://www.vim.org/) and [Emacs](http://www.gnu.org/software/emacs/) have fierce adherents but very steep learning curves. If you learn one, you will turn into a text-editing ninja.

[Sublime Text](http://www.sublimetext.com/) and [TextWrangler](http://www.barebones.com/products/textwrangler/) are good for Macs; Sublime Text and [Notepad++](http://notepad-plus-plus.org/) are good for Windows.

The specific text editor you use is much less important than that you are comfortable with it. Your text editor is a tool for communicating with a computer, and you should expect to invest many hours writing text; why not make yourself as comfortable as possible?

## Programming languages
Like your choice of text editor, the choice of programming language is very personal. Different programming languages excel at different tasks, and different scientific communities have different preferences for languages. Some languages are good at analyzing data; some are good for mathematics; some are good at matrix algebra; some are good at everything, with mathematics as a special case.

Learn how to program by programming; use Google to fill in the gaps in your knowledge, and just go for it when it comes to projects. Use it for everything you can. Even if it will take longer to figure out how to program it than it would take to do it by hand, you'll be learning how to do it quicker next time.

You will have to choose some programming language. My personal choice is Python, but I'll summarize some other languages, too.

### Python
Python is a great multi-purpose, fully-featured programming language. Python does it all, and does it easily. Python can reliably be your go-to language for just about any problem.

Two things are worth noting with Python, that might make another language more appropriate for you: Python is an interpreted language, and Python was not designed with science as its primary purpose.

Because Python is interpreted, some programs will run very slowly (see: heavy use of the `for` loop). This is true of any interpreted language (R, MATLAB, Stata), and most computationally intense algorithms will already be implemented very quickly; but at the margins, you might need to use C if heavy computation on very large data is time-sensitive and frequent.

Because Python was not designed specifically for science, many of the scientific features Python has are add-ons. These libraries are robust, reliable, and optimized; but they often operate with an intermediary layer between the Python interpreter and their functions. This doesn't inhibit Python's function-set; it merely means things like linear algebra aren't as direct or simple as in MATLAB, or statistical modeling requires a few more steps than in R.

If you are interested in using Python, you might check out the book _Python for Data Science_, which describes in detail many packages Python has for data analysis and scientific computing.

Python is effortless to install and manage with [Anaconda](https://store.continuum.io/cshop/anaconda/), which is oriented towards scientific computing.

Use the [iPython](http://ipython.org/) Python shell. It changed the way that I program, and provides incredibly effective interaction with your code.

### Other languages
R, Stata, MATLAB, Julia

### Awk and Sed
