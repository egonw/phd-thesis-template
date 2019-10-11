# Manuscript Ryan Miller

Thesis manuscript for editing

## Creating the PDF

To create the PDF, run the following command (e.g. on the Ubuntu from the Microsoft Store, after installing the Windows Subsystem for Linux):

```shell
pdflatex thesis
pdflatex thesis
pdflatex thesis
bibtex thesis1-blx
bibtex thesis2-blx
bibtex thesis3-blx
pdflatex thesis
```

The multiple `pdflatex` calls are deliberate because creating the correct chapter numbers and filling the proper
numbers for cross references (think "see Chapter X") is an iterative process.

## Cleaning the folder

LaTeX makes many temporary files, which clutter the folder. Clean things with:

```shell
\rm -Rf *.aux *.log *.toc *.bbl *.blg *.run.xml *-blx.bib
```
