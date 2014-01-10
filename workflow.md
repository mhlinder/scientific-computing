A Computational Workflow
========================
In the course of conducting scientific research, data is amassed, PDFs are read, programs are written, new data is generated, plots are made, papers get written. We believe firmly in the importance of reproducibility, but all too often, not even the original researcher can reproduce code-based results, much less a third party. This scares us, and it should scare you too. It's said that good programmers don't make more mistakes, they just know to look for them more often, and this holds in scientific computing as well: science that cannot be reproduced is hardly science at all.

The key is recognizing that you will make mistakes, and that this is OK. Everyone, in the course of research, makes mistakes. Far more important is documenting _what_ you did, and how, so that you can catch those mistakes quicker. Down the line, this will have the added benefit of making your scientific computations reproducible.

What do we mean? We're talking about workflow, the intelligent design of the scientific process so that it is well-documented, transparent and reproducible. This means writing down everything you do, organizing it clearly and providing access to all steps involved in producing some results.

We propose a simple model, one intended to be personalized according to your personal needs. There are three components to this organizational system:
1. Version control
2. Documentation
3. Structure
We'll step through these one-by-one.

Version Control
===============
Good version control software is at the core of good scientific practice. We use [Git](http://git-scm.com), but [Mercurial](http://mercurial.selenic.com/) and [Subversion](http://subversion.tigris.org/) are good, too. Whatever you choose, make sure to _use_ it. Version control software allows you to leave a paper trail behind you, by recording the status of a set of files at various points in time. This means you will know what a do-file looked like two months ago, or allow you to check how you were calculating a growth rate before the current approach. This prevents you from losing historical information, on the one hand, and prevents multiple version of code with names suggesting slightly different contents on the other hand.

Version control is passive: just update it every time you change something, and you'll be able to trace your project's life back to the beginnings. You don't have to do much; it's not labor-intensive; but it will give you peace of mind.

Documentation
=============
No one will know what your project does, how the code works and what the code does and what the charts mean, without an explanation, and documentation does just that. This is a more active process than using version control, because you are expressing your project in the form of comments in code and explanatory documents. Code comments should explain what pieces of code do, and why. Documents should explain assumptions and ideas, more of a birds-eye perspective on the process.
