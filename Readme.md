Scientific Computing for Scientists
===================================

## Manifesto
Why practice scientific computing? Scientific computing is not merely using computers as an aid to science; it's intelligently using computers to organize and process data, and to write up the results of empirical work and simulation.

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

## LaTeX

So you've done the hard work.  You've gathered and cleaned the data, performed your analysis, and tracked it all with Github. And after all of that, when it comes time to report your results, your effort deserves to be rewarded with something more capable and less undergrad than Microsoft Word.

In particular, Latex offers scientific researchers the best workflow in document preparation because it beats alternatives in three main areas:

    1. Composing documents
    2. Updating those documents with new output
    3. Searching through and backing up your work

The rest of this section covers each in turn.

### Composing Documents 

First, Latex beats other document preparation systems because, when preparing results, it gets out of the way for simple tasks, but allows total control and customization when you need it. 

Everyone who uses Microsoft Word has experienced how frustrating software can be when it gets in the way of composing a document. As your file grows in length or formatting complexity, you might encounter the following thoughts and frustrations:

* "Only God knows what alignment/margins will follow once I hit tab/backspace/enter here."
* "My professor knew I copy/pasted from Wikipedia because parts of my document were in Calibri, while other parts were in Times New Roman. These default text settings mean I always have to reformat."
* "Why is there sometimes this extra white space between paragraphs, sometimes not?"
* "Every time I change the text, this picture moves. And now the last line of this other page is jumping back and forth between one page and the next with even the slightest of changes."
* "Ugh. I have to buy a new computer. I can't believe I smashed this one in a fit of formatting rage."
* "If this is my life, I'm now ready to walk into the light."

(Of course, these aren't huge annoyances if you'd rather be formatting text in Microsoft Word rather than sharing interesting results and performing scientific research. And you know what they say: _De gustibus, MS Word est horrendum_.) 


Enter Latex. After an initial fixed cost of installation and setting up a proper preamble, you can write freely without disturbance in your favorite text editor. You can zip around and edit text quickly in vim or emacs, leaving to Latex the placement of figures, spacing, section headers, etc. (which it will do consistently and uniformly across the document). This allows the author to focus on content, at least until the final compilation.  Then, if some fussing is necessary to get the document looking a certain way, Latex offers full and total control of the format. 

So Latex offers two modes of composition well-suited to scientific research: a low-cost, content-centric mode and a control-freak, OCD mode. The former produces high-quality documents without much fussing and at very low cost, while the latter allows customization to any level necessary for the needs a particular project.  Together, they provide a superior working environment compared to Microsoft Word's muddled middle-of-the-road strategy, which promises constant visual reminders of its formatting problems without the proper tools to resolve them fully and reliably. 

(Note: This section even left aside Latex's superb typesetting of mathematics, which has no real rival.)

### Updating Your Documents 

Second, Latex produces documents which can be updated easily 
and _programmatically_. Say your document includes a plot. Even if that plot changes, the tex file won't. Instead, the tex file--which includes the name/path of the figure--can remain untouched while you simply update the pdf or eps file itself. In this way, you can easily update plots by just overwriting them with new versions. No more tedious, "copy/paste" in Word (which also happens to scale very poorly).  

Similarly, you can do the same for tables by writing them programmatically to individual files. Then a simple "\include" statement in your tex file will grab and read the text.

### Searching and Backing Up Your Work

Third and finally, tex files are plain text with markup. So if you want to search your documents, just use grep or awk like you do for source code.  These tools are quick and reliable, plus you probably already use them.  It's handy to be able to search through everything you wrote in a few seconds rather than letting some search program slog through your more complicated Word files.  Oh, and since they're searchable like code, tex files are also amenable to backup on Github.

So if I haven't convinced you that Latex is the best document preparation system for scientific computing, please provide your email and check your inbox for another five pages of ranting, beautifully composed (of course) in Latex. 
