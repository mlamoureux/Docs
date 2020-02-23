Creating Documentation
======================

Using  Read The Docs
^^^^^^^^^^^^^^^^^^^^

I'm using a system called Read The Docs. You can read about it here ar: [readthedocs.org](https://readthedocs.org/)

The idea is simple:

- create a bunch of files
- push it to your github repo
- let the Read The Docs system publish it on the web for you.

There is a bit more to it than that. You should first create the documentation set on your own computer, using the Sphinx software. To install Sphinx, you need to run pip from within a terminal window:

- pip install Sphinx

If you plan to use MarkDown as your language, you should also install this extension

- pip install recommonmark

Also, you will have to add the following line to your conf.pu file (once it is created), like this:

- pip install recommonmark

Otherwise, you will be using reStrucutre Text files for the documentation. 

For the advantages of reStrucutured Text (.rst) files over Markdown (.md) files, check out the blog by [www.ericholscher.com/blog](https://www.ericholscher.com/blog/2016/mar/15/dont-use-markdown-for-technical-docs/)

For me (MLamoureux), I plan to use Markdown, since that is what I am familiar with. 

Using Sphinx
============

Don't forget to do a pip install, to get the software. You only need to do this once on your system

- pip install sphinx

(On a Max, you might need to do install Python3 and use pip3. YOu may also need to install XCode developer tools. See next section.)

Now, create a new directory  (folder) somewhere on your hard drive. From the terminal, cd into that directory, then  run quickstart to set things up with Sphinx.

- cd thatDirectory
- sphinx-quickstart


This will create several files in the current directory. IN ths new "source" directory is a file called index.rst, which you will list the files you want compiled into the documentation. You don't need to list the file extension. You do have to get the spacing right. 