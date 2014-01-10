Get to Know Your Tools
======================
The tools of the scientific trade have changed dramatically in the past handful of decades, from analogue, physical tools (beakers, thermometers, _paper_) to digital tools (spreadsheets, academic databases, computational programming). The tools available to scientists are extensive and it can be difficult to identify the "best of those tools."

We admit: we will be unable to do justice to the full spectrum of computational scientific tools. We won't come anywhere close to identifying these "best tools." Instead, we hope to present a framework for finding the best tools for _you_, and for developing a workflow that makes practicing computational science streamlined and organized.

### The Holy Grail
The most important tool in our arsenal will sound trivial, silly and blatant; but trust us, this is the tool that we use most, yields the best results and has the greatest potential for scientific use. We are talking, of course, about [Google](http://www.google.com), or any other search engine.

It would be impossible to summarize the benefits of a good search engine to the modern scientist, but a few of our regular uses include:

* Finding data.
* Finding answers to technical questions and documentation for scientific programs.
* Finding research by others.

You can think of search as a supernatural finding utility, one that can answer your every question and obtain any information you could desire. Invariably, someone has had the same question, information need or problem you do and documented their results online; do not underestimate the power of search. Keep your search engine dear to your heart, use it constantly, and you will be rewarded with all the riches of heaven. Or at least omniscience and the ability to solve any problem.

### Package Management
Aside from search, most tools need to be installed to your computer, and it is important to give some thought to how you do this. A positive trend is package management, and package managers are ubiquitous. Generally, a package manager keeps track of which software is installed on your system and _how up to date that software is_. A package manager allows you to install software once&mdash;normally from a central repository, so you don't need to find it&mdash;and update it as necessary. This is essential for keeping your tools up-to-date, and allows you to free up your attention to do science, not manage your programs.

On Macs you can use the App Store for some programs, and [Homebrew](http://brew.sh/) and [MacPorts](http://www.macports.org/) allow you to exponentially widen your arsenal. These tools trace their ancestry to \*nix package managers; if you use Linux, we recommend you use whatever your distribution uses (e.g., `pacman` for [Arch](https://www.archlinux.org/), `aptitude` for [Debian](http://www.debian.org/) and [Ubuntu](http://www.ubuntu.com/), and so on&mdash;our examples reveal our preferences). In our daily research, we use Mac and Linux software, so we are less familiar with options available for Windows, but we are confident solutions exist there, as well.

### Office Software
The first line of defense for scientific researchers is an office suite. We use both Microsoft Office and [OpenOffice](https://www.openoffice.org/), and open standards allow interoperability between the two. The important thing is that you have access to a word processor for writing up results; a spreadsheet editor for basic (or advanced) data manipulation (cleaning, reshaping, analyzing); and presentation software for communicating results to others. In particular, although we are committed to programming for nearly every task, a spreadsheet editor is an indispensible tool for any researcher who uses data. Spreadsheets are intuitive and easy to use and can be very powerful; often, much pre-processing can be done in a spreadsheet, limiting the need to program, and often using a spreadsheet is simply easier.

### Text Editors
As a scientist, you will be interacting with much more text than just that found in word processors: you will need to examine data, make notes, and write code. In theory you might use a word processor for these purposes, but _strike that from your brain and never think that again_. It's like using a spoon to cut a steak, it's heinous and will cause you to die an early death. When you have text that needs to be formatted, you _may_ use a word processor; _when you have text that is just text, always use a text editor_.

Choosing a text editor is a personal process; just don't use Notepad. Think of a text editor as your primary interface for interacting with information.

[Vim](http://www.vim.org/) and [Emacs](http://www.gnu.org/software/emacs/) have fierce adherents but very steep learning curves. If you learn one, you will turn into a text-editing ninja.

[Sublime Text](http://www.sublimetext.com/) and [TextWrangler](http://www.barebones.com/products/textwrangler/) are good for Macs; Sublime Text and [Notepad++](http://notepad-plus-plus.org/) are good for Windows.

The specific text editor you use is much less important than that you are comfortable with it. Your text editor is a tool for communicating with a computer, and you should expect to invest many hours writing text; why not make yourself as comfortable as possible?

### The Terminal
Finally, embrace using the terminal. The terminal is daunting and foreign to beginners, but it is immensely powerful and will ultimately give you ultimate control over your work. The terminal allows you to interact directly with the nitty-gritty parts of code, files and your computer in general. The terminal is also integrally linked to the operating system you use. Research servers are almost uniformly Linux-based, and you will interact with them through the terminal. If you run Linux or Mac (which share common ancestors), the terminal is built-in and will operate similar to the terminal on a server. Windows has different architecture, which can be accessed with the [PowerShell](TODO). However, we recommend you familiarize yourself with Linux-style computing, and if you're on Windows, you can do this with [Cygwin](TODO), which emulates the Linux filesystem structure and provides many open-source tools.
