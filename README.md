# README

## What this is

These are notes to the lecture "Mathematik III" by Prof. Dr. Peter Hauck in
WS13/14. No correctness can be guaranteed. If you find any mistakes (and there
definitely are some), feel free to put up a pull request or post somehing in
the issue section.

## How to compile

### From command line

    pdflatex -synctex=1 -shell-escape -interaction=nonstopmode MatheIII\_Skript.tex

### Required files

This file does not compile on its own. What you will need is the
[uni\_tue\_template](https://github.com/k0nze/uni_tue_template) that provides
all packages and self- defined commands that are needed for compilation. If you
put it into the same directory as the other tex files, it should compile. If
not, you are probably missing some required packages. See latex log for
troubleshooting.

### Set booleans

The main file sets the boolean _compileall_. You'll want to set it to true,
unless you're currently developing something and do not want the whole document
to be compiled all the time.

### Compile from script

Part of the repository is a compile script. This does exactly what we mentioned
in the section above. It gets a parameter {true|false} and compiles the
document for you. Here's how to do it (for instance):

    cd /where/your/repo/is
    chmod +x ./compile
    ./compile
