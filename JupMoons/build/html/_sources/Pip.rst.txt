Using PIP/make on a Mac.
========================

Runing Mac OS 10.15.2 (feb 2020). I need PIP in order to install some packages (in particular, Sphinx for creating documnetation). Pip as is, on the Mac, does not seem to run, 

After reading a lot on line, I decided to use Homebrew to get an up-to-date verison of Python (Mac uses 2.7.16, which is ridiculous). 

- brew install python
- brew link --overwrite python

Now to install sphinx with pip, I use

- pip3 install sphinx

I then did:

- brew install python
- brew unlink python && brew link python
- brew link --overwrite python
- brew install sphinx-doc
- echo 'export PATH="/usr/local/opt/sphinx-doc/bin:$PATH"' >> ~/.zshrc

Somewhere, I did this: 

- pip3 install sphinx

But I'm not sure that was a good idea. IN any case, it does not have the sphinx-quickstart command, so I don't know why I need it. (Maybe I don't)


On a Mac, you also need to have the developer tools installed, in order for the "make" command to run. Need to run this in the terminal:
- xcode-select --install