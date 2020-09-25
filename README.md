# moodle-latex-example

# Requirement(s):

## moodle.sty
linux: texlive-latex-extra package on ubuntu

## For image:

### imagemagick: 
converts pdf files to png

### ghostscript: gs (linux) or gswin64c.exe (on windows)
converts jpg to png file

### openssl
encodes the png file to a text file

If the figures are all kept in a specific folder and the command
\graphicspath{} has been used, then also require the patch style file
\graphicxx.sty

## Tikz package
If you are using the package tikz make sure that the tikz package is
loaded after the moodle package and NOT before.

# Run:

    pdflatex -shell-escape example.tex

Creates a file called example-moodle.xml. You can upload this file on
moodle. This single file will also upload the figures!!!

