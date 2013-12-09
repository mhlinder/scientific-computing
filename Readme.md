Scientific Computing for Scientists
===================================

## Manifesto
Who needs scientific computing? These days, nearly everyone can benefit from the tools and concepts of scientific computing, from professional researchers in the sciences, to humanists looking to incorporate quantitative methodology, to anyone looking to process data in a systematic way.

But what is scientific computing? Scientific computing is not the use of computers as an afterthought in research; it is the intelligent use of computers for organizing and processing data, and for communicating the results of this empirical and simulated work. Computers are unique, powerful tools for organization and analysis, and scientific computing is the exploitation of the particular advantages of computers to aid in our ability to learn about the world around us.

We have witnessed firsthand, however, the difficulty of practicing scientific computing because the development and use of the tools of scientific computing are [heavily de-emphasized](TODO) within academia. Science as it is currently practiced is often poorly organized on computers, with messy code and undocumented data the norm. We hope to make this the exception, by providing a series of suggestions for the effective practice of science on computers. We believe that science should be well-documented, reproducible and highly organized, and our suggestions below seek to make the practice of this type of science as effortless as possible.

We believe that scientific computing need not be something Professional Researches pawn off to their RAs, nor considered "dirty work," nor even be complicated or difficult. We believe scientific computing can be fun, and powerful, and provide innovative solutions to problems. When used properly, computers can do things no human can do, but it is only by spending time and energy developing computational tools, skills and understanding that computers can be used to their full potential.

We put forth here a template for conducting scientific research ("science" here defined very loosely, and involving most quantitative work) with the aid of computers. Our individual workflows differ, as do the tools we use. These should differ for you, too, tailored to your preferences, field and abilities. We seek only to present some heuristics and organizational techniques that we have found greatly increase our scientific output, and might help you, too.

We consider this a guide to Scientific Computing for Scientists, and we consider it a work in progress. Please contact us with any omissions, mistakes or comments.

Signed,
Matt Cocci, M. Henry Linder and Max Livingston


## Get to know your tools
The tools of the scientific trade have changed dramatically in the past handful of decades, from analogue, physical tools (beakers, thermometers, _paper_) to digital tools (spreadsheets, academic databases, computational programming). The tools available to scientists are extensive and it can be difficult to identify the "best of those tools."

We admit: we will be unable to do justice to the full spectrum of computational scientific tools. We won't come anywhere close to identifying these "best tools." Instead, we hope to present a framework for finding the best tools for _you_, and for developing a workflow that makes the practice of science as streamlined and organized as possible, simultaenously.

The most important tool in our arsenal will sound trivial, silly and blatant; but trust us, this is the tool we use most, the tool we benefit from the most, and the tool with the greatest potential for scientific use. We are talking, of course, of [Google](http://www.google.com), or any other search engine. It would be impossible to summarize the benefits of a good search engine to the modern scientist, but a few of our regular uses include:

* Finding data
* Finding answers to technical questions, and documentation for various scientific programs.
* Finding research by others

You can think of a search as a supernatural finding utility, one that can answer nearly every question you have and obtain nearly any information you need. Do not underestimate the power of search: if you have a question, a problem or an informational need, someone before you has probably needed the same thing, and documented it online. Keep your search engine dear to your heart, and use it constantly.

Most other tools will need to be installed, and it is important to give some thought to how you install software. A positive trend in software installation is package management, and package managers are ubiquitous. The general idea of a package manager is the ability to keep track of which software is installed and _how up to date that software is_, as effortlessly as possible. A package manager allows you to install software once---normally from a central repository, so you need not look around for it---and to update that software at whim. THis is essentail for keeping your tools up-to-date, and allows you to free up your attention to do science, not manage your programs.

On Macs one can use the App Store for some programs, and tools such as [Homebrew](TODO) and [MacPorts](TODO) allow you to dramatically widen your arsenal. These tools trace their ancestors to Linux package managers, which vary by distribution; we recommend you use whatever your distribution uses (`pacman` for [Arch](TODO), `aptitude` for [Debian](TODO) and [Ubuntu](TODO), and so on). In our daily research, we use Mac or Linux software, so we are less familiar with options available for Windows, but we are confident solutions exist there, as well.

The first line of defense for scientific researchers is an office suite. We use both [Microsoft Office](TODO) and [OpenOffice](TODO), and open standards allow interoperability between the two. The important thing is that you have access to a word processor for writing up results; a spreadsheet editor for basic (or advanced) data manipulation (cleaning, reshaping, analyzing); and presentation software for communicating results to others. In particular, although we are committed to programming for nearly every task, a spreadsheet editor is an indispensible tool for any researcher who uses data. Spreadsheets are intuitive to use and very powerful; often, much pre-processing can be done in a spreadsheet, limiting the need to program, and often using a spreadsheet is simply easier.

As a scientist, you will be interacting with much more text than just that found in word processors: you will need to examine data, make notes, and write code. In theory you might use a word processor for these purposes, but *strike that from your brain and never think that again*. It's like using a spoon to cut a steak, it's heinous and will cause you to die an early death. When you have text that needs to be formatted, use a word processor; *when you have text that is just text, always use a word processor*.

Choosing a text editor is a personal process; just don't use Notepad. Think of a text editor as your primary interface for interacting with information.

[Vim](http://www.vim.org/) and [Emacs](http://www.gnu.org/software/emacs/) have fierce adherents but very steep learning curves. If you learn one, you will turn into a text-editing ninja.

[Sublime Text](http://www.sublimetext.com/) and [TextWrangler](http://www.barebones.com/products/textwrangler/) are good for Macs; Sublime Text and [Notepad++](http://notepad-plus-plus.org/) are good for Windows.

The specific text editor you use is much less important than that you are comfortable with it. Your text editor is a tool for communicating with a computer, and you should expect to invest many hours writing text; why not make yourself as comfortable as possible?

Finally, embrace using the terminal. The terminal is daunting and foreign to beginners, but it is immensely powerful and will ultimately give you ultimate control over your work. The terminal allows you to interact directly with the nitty-gritty parts of code, files and your computer in general. The terminal is also integrally linked to the operating system you use. Research servers are almost uniformly Linux-based, and you will interact with them through the terminal. If you run Linux or Mac (which share common ancestors), the terminal is built-in and will operate similar to the terminal on a server. Windows has different architecture, which can be accessed with the [PowerShell](TODO). However, we recommend you familiarize yourself with Linux-style computing, and if you're on Windows, you can do this with [Cygwin](TODO), which emulates the Linux filesystem structure and provides many open-source tools.

## Learn how to program
You must now resign yourself to learning to program. This is a good life skill to have, an increasing expectation in both academia and industry. Many---most?---tasks can only be completed with a programming language, and you will waste a LOT of time trying to circumvent learning to program.

Like your choice of text editor, the choice of programming language is very personal. Different programming languages excel at different tasks, and different scientific communities have different preferences for languages. Some languages are good at analyzing data; some are good for mathematics; some are good at matrix algebra; some are good at everything, with mathematics as a special case.

Learn how to program by programming; use Google to fill in the gaps in your knowledge, and just go for it when it comes to projects. Use it for everything you can. Even if it will take longer to figure out how to program it than it would take to do it by hand, you'll be learning how to do it quicker next time.

You will have to choose some programming language. My personal choice is Python, but I'll summarize some other languages, too.

### Python
We primarily use Python in our day-to-day programming, be it simple scripting or extensive software development. Python is a great multi-purpose, fully-featured programming language. Python does it all, and does it easily. Python can reliably be your go-to language for just about any problem.

Two things are worth noting with Python, that might make another language more appropriate for you: Python is an interpreted language, and Python was not designed with science as its primary purpose.

Because Python is interpreted, some programs will run very slowly (see: heavy use of the `for` loop). This is true of any interpreted language (R, MATLAB, Stata), and most computationally intense algorithms will already be implemented very quickly; but at the margins, you might need to use C if heavy computation on very large data is time-sensitive and frequent.

Because Python was not designed specifically for science, many of the scientific features Python has are add-ons. These libraries are robust, reliable, and optimized; but they often operate with an intermediary layer between the Python interpreter and their functions. This doesn't inhibit Python's function-set; it merely means things like linear algebra aren't as direct or simple as in MATLAB, or statistical modeling requires a few more steps than in R.

If you are interested in using Python, you might check out the book _Python for Data Science_, which describes in detail many packages Python has for data analysis and scientific computing.

Python is effortless to install and manage with [Anaconda](https://store.continuum.io/cshop/anaconda/), which is oriented towards scientific computing.

Use the [iPython](http://ipython.org/) Python shell. It changed the way that we program, and provides incredibly effective interaction with your code.

### Other languages
Python may not address your needs, or may not be to your tastes. Fear not: there are literally thousands of programming languages to choose from. If you're doing statistics, we recommend [R](TODO), or [Stata](TODO) for a less programming-intensive language; if you're doing a lot of scripting, you might check out [Ruby](TODO); if you do a lot of linear algebra, [MATLAB](TODO) may be for you, and [Mathematica](TODO) is great for symbolic math. For those with performance-sensitive tasks---be it large datasets; long, loop-heavy software; or just a need for speed---should look at [Julia](TODO), which has the syntax of Python, the linear algebra of MATLAB, and the speed of C/C++; or check out the latter two, which are low-level and notoriously unfriendly to beginners, but also the industry choice for low-latency, high-speed computing.

We do recommend you find a programming language suited to as many of your needs as possible. A chief advantage of languages like Python and R is that they are open source, and have vibrant communities that develop a wide range of software packages for the languages. Often, a package exists to accomplish specific tasks so you don't have to write it from scratch, and we recommend looking into the availability of such packages in a language before committing yourself to learning it completely.

Three other languages stand out as oft-overlooked, but immensely powerful, especially for those dealing with large datasets that may need to be reorganized: Bash, [sed](TODO) and [awk](TODO). Bash is, in fact, the most widely used "shell" in the terminal: it defines the keywords you use to accomplish tasks, and these keywords can be strung together to make a small program called a script. Bash scripting is an excellent interface for plugging together a variety of individual programs, such as reading a comma-delimited data file, matching a certain pattern, cutting out only the data you need, and reformatting it for your needs. Bash scripting is a key tool in the arsenal of the scientist looking to optimize her workflow.

Sed and Awk are storied tools for processing text, and process it line-by-line instead of requiring that you load the entire data into, say, a spreadsheet (i.e., loading it into your computer's memory). Sed matches and alters patterns in text, while awk incorporates some of the features of sed, plus offering a pretty fully-featured programming language for more advanced tasks. Both allow you to manipulate very large data files, with minimal by-hand editing. They have steep learning curves, but this is mitigated by the sheer power they provide on the commandline.

### Choosing New Languages

Whether out of scientific neccessity, sheer boredom, or shameless nerdiness, every researcher will consider learning a new language. So then the question becomes "Given what I already know, what new language would add the most value to my scientific computing toolkit?" Clearly, that depends cruciallly upon the tasks you intend to accomplish, the preferences of coworkers and coauthors, the language of any code you might inherit, etc. 

_However_, leaving aside such idiosyncratic considerations and supposing that you have a say in the matter, two general guidelines seem reasonable: 

1. Learn something really new or different to expand the _scope_ of your toolkit.
2. If you're going to learn a new language that's similar to one you already know, there should be a speed/efficiency improvement (whether that's in terms of computing time or your coding time).



## Leave a paper trail

* Documentation / Latex
* Twitter, email, blogs, github

[Git](http://git-scm.com/) is version control software, which will keep track of changes you make to files---code, documentation, data---and allow you to look back into the history of your projects. Git is a killer app for project management and version control: you can set up a [workflow](https://www.atlassian.com/git/workflows) defining your interaction with your files, or design your own. You can learn git [here](http://gitready.com/) or [here](http://git-scm.com/book).

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
