Learn How to Program
============

You must now resign yourself to learning to program. This is a good life skill to have, an increasing expectation in both academia and industry. Many&mdash;most?&mdash;tasks can only be completed with a programming language, and you will waste a LOT of time trying to circumvent learning to program.

Like your choice of text editor, the choice of programming language is very personal. Different programming languages excel at different tasks, and different scientific communities have different preferences for languages. Some languages are good at analyzing data; some are good for mathematics; some are good at matrix algebra; some are good at everything, with mathematics as a special case.

Learn how to program by programming; use Google to fill in the gaps in your knowledge, and just go for it when it comes to projects. Use it for everything you can. Even if it will take longer to figure out how to program it than it would take to do it by hand, you'll be learning how to do it quicker next time.

You will have to choose some programming language. My personal choice is Python, but I'll summarize some other languages, too.

## Python
See also [Python](python.md)

## Programming Languages

Python may not address your needs, or may not be to your tastes. Fear not: there are literally thousands of programming languages to choose from. If you're doing statistics, we recommend [R](TODO), or [Stata](TODO) for a less programming-intensive language; if you're doing a lot of scripting, you might check out [Ruby](TODO); if you do a lot of linear algebra, [MATLAB](TODO) may be for you, and [Mathematica](TODO) is great for symbolic math. For those with performance-sensitive tasks&mdash;be it large datasets; long, loop-heavy software; or just a need for speed&mdash;should look at [Julia](TODO), which has the syntax of Python, the linear algebra of MATLAB, and the speed of C/C++; or check out the latter two, which are low-level and notoriously unfriendly to beginners, but also the industry choice for low-latency, high-speed computing.

We do recommend you find a programming language suited to as many of your needs as possible. A chief advantage of languages like Python and R is that they are open source, and have vibrant communities that develop a wide range of software packages for the languages. Often, a package exists to accomplish specific tasks so you don't have to write it from scratch, and we recommend looking into the availability of such packages in a language before committing yourself to learning it completely.

Three other languages stand out as oft-overlooked, but immensely powerful, especially for those dealing with large datasets that may need to be reorganized: Bash, [sed](TODO) and [awk](TODO). Bash is, in fact, the most widely used "shell" in the terminal: it defines the keywords you use to accomplish tasks, and these keywords can be strung together to make a small program called a script. Bash scripting is an excellent interface for plugging together a variety of individual programs, such as reading a comma-delimited data file, matching a certain pattern, cutting out only the data you need, and reformatting it for your needs. Bash scripting is a key tool in the arsenal of the scientist looking to optimize her workflow.

Sed and Awk are storied tools for processing text, and process it line-by-line instead of requiring that you load the entire data into, say, a spreadsheet (i.e., loading it into your computer's memory). Sed matches and alters patterns in text, while awk incorporates some of the features of sed, plus offering a pretty fully-featured programming language for more advanced tasks. Both allow you to manipulate very large data files, with minimal by-hand editing. They have steep learning curves, but this is mitigated by the sheer power they provide on the commandline.
