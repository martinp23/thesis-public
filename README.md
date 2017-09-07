# thesis-public

This is the first two chapters of my DPhil thesis from the University of Oxford. The full version will eventually be released from here: https://ora.ox.ac.uk/objects/uuid:58a35932-320c-47dc-828e-0d121d693fd8

The purpose of this repository is to provide a (somewhat clear, maybe) example of the use of LaTeX for an organic(-ish) chemistry thesis. It adds some conversion of journal names to abbreviations, incorporates an example of the use of the chemnum package, and some possibly helpful chemistry-related commands.

The template is taken from here: https://www.oxfordechoes.com/oxford-thesis-template/

How to build?

pdflatex --shell-escape thesis
biber thesis
pdflatex --shell-escape thesis
pdflatex --shell-escape thesis



I used MikTeX on Windows. The list of packages is in the thesis.dep file. If you find builds failing, as a first step remove all of the Aux files. I also used LaTeXTools in Sublime Text 3.
