Modular Programming
===================

Sure, you could always just write the entirety of your analysis in one single, monster do file, m-script, .py file, etc. 

Yes it's true that for _all_ of your observations and datasets, you could write One Script to find them, and&mdash;in the R environment&mdash;cbind them, i.e. One Script to rule them all.

_But_ chances are, you could probably gain a thing or two by sensibly modularizing your code into smaller pieces that you can more easily test, optimize, reuse, and share. We'll discuss each in turn.


### Testing Your Code

Imagine you've spent time writing the perfect (and sequential) program: one that proceeds step-by-step to find the Answer to the Ultimate Question of Life, the Universe, and Everything. You hit run.  You wait patiently for 7.5 million years while it calculates the Answer (or perhaps executes a moderately long for-loop in R) only to find out that, after 6.5 million years, there was a bug in the program.  An error message was thrown. Looks like you'll have to change the code, wait 6.5 million years to see if this bug shows up again (because it's sequential, after all), hoping for the best in the meantime.

Now that would be pretty stupid on multiple levels, but let's focus on one:  Why write the program in such a way that you have to run 6.5 million years-worth of code _again_ before you can see if the bug has been fixed?

But yet, we've probably all done this (albeit on less than thrilling timescales)&mdash;particularly in languages like Python and Matlab, which encourage a "run, catch error, fix, re-run, repeat" approach.  For programs that have short runtimes, this is fine; no harm done.  But if you're scaling to the level of a serious research project, you might consider adding some modularity to your codebase and workflow. 

By modularizing, you can test small portions at a time without having to re-run the entire gambit.  You're not tied to executing a very long program sequentially. For programs with non-trivial runtimes, this can be a huge time-saver when checking for and fixing errors. 

Finally, for languages that give less-than-intelligible error messages, modularity can even allow greater precision in error-tracing. You can trace directly to functions or procedures, rather than searching through thousands of lines in a long program if the error messages don't list the line number.

### Matching Languages and Tools to Tasks

If you've written code in multiple languages, you're well-aware that some languages are better suited for certain tasks.  For example, I'd rather do matrix algebra in Matlab.  When it comes to text-processing, Python or sed and awk probably rank highest. But, if you asked me to do either of those things in Stata before it's time to run regressions, I'd probably do [this] (http://stream1.gifsoup.com/view4/3211019/ron-swanson-vs-computer-o.gif).

Now back to modularity. If your code is split up sensibly into separable tasks, there's always room to speed up runtime or simplify steps by taking output from one program (in one language) and using it as input for the next program (in possibly another language). Often, you'll be able to tie the two together by scripting in one of the underlying languages or by sewing everything together with a bash script or make file.  So if you know multiple languages (and enough of them to really understand their strenghts), why not take advantage?

### Reusing Code

Reusuing code is perhaps the main motivation for modularity. There are so many more programs to write, interesting questions to answer, and books to read (which you may/will promptly substitute with "seasons of Doctor Who to watch"), that it's not worth your time to re-write the same code over and over again, if you can help.

And you can help it. How? With modularity. With wrapper functions. Use them both. (And these are not the droids you're looking for.)

You can go about your business and move along your projects more quickly if you have a few cross-project, general-purpose functions or procedures that you "wrap" in project-specific code.

As an example, take a gradient descent algorithm in Matlab called `gradient_descent.m`. The basic idea will remain the same regardless of any particular project: find the gradient, descend the hill. Now rather than rewrite this procedure for each project, write _one_ that is project-independent. Specifically, this general program will take a function and a starting point, numerically approximate the gradient, update, and call itself again (unless some threshold is met).  Anything project-specific can be done in a program like `gradient_descent_myproject.m`, which induces all of the inputs into a suitable form, passes them as arguments to `gradient_descent.m`, then translates the output back to results for the individual project. 

So to sum up, your goal should be to write it once, use it often. If your code consists of modular pieces well-targeted at one specific function, you're well on your way to this goal.

### Sharing Your Work

Modularity goes a long way in encouraging and enabling others to use your code and extend your work. 

If you're writing modular code and implementing it across projects, then someone else can too. And aside from helping others, this also means a fresh set of eyes on your code and your analysis which might direct suggestions, improvements, and errors back to you for consideration.  (Combined with a version control system like Git, you can then easily incorporate this into your own code, reconciling differences with ease.) It also means that others can more easily take your analysis, modify it a bit, and furnish you with endless and duly-deserved citations (okay, maybe one or two).


