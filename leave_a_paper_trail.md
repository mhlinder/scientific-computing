Leave a Paper Trail
===================

* Documentation / Latex
* Twitter, email, blogs, github

[Git](http://git-scm.com/) is version control software, which will keep track of changes you make to files---code, documentation, data---and allow you to look back into the history of your projects. Git is a killer app for project management and version control: you can set up a [workflow](https://www.atlassian.com/git/workflows) defining your interaction with your files, or design your own. You can learn Git [here](http://gitready.com/) or [here](http://git-scm.com/book).

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
