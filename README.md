# thesis-public

This is the first two chapters of my DPhil thesis from the University of Oxford. The full version will eventually be released from here: https://ora.ox.ac.uk/objects/uuid:58a35932-320c-47dc-828e-0d121d693fd8

The purpose of this repository is to provide a (somewhat clear, maybe) example of the use of LaTeX for an organic(-ish) chemistry thesis. It adds some conversion of journal names to abbreviations, incorporates an example of the use of the chemnum package, and some possibly helpful chemistry-related commands.

A note on my use of the chemnum package: the auto-renumbering benefit is somewhat lost by the fact that I have placed a "list of compounds" in the frontmatter of the thesis. If that page were to be removed, then reordering compounds would result in reordering of compound numbers automatically.

The Oxford Thesis template is taken from here: https://www.oxfordechoes.com/oxford-thesis-template/ .

How to build?

```
pdflatex --shell-escape thesis 
biber thesis
pdflatex --shell-escape thesis
pdflatex --shell-escape thesis
```


I used MikTeX on Windows. The list of packages is in the thesis.dep file. If you find builds failing, as a first step remove all of the aux files and check that the pre-requisites are properly installed. Unfortunately it can be a bit of a nightmare getting everything necessary set up, particularly for chemnum. I found the tex stackexchange (http://tex.stackexchange.com) invaluably helpful.
