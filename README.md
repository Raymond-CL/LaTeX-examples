## LaTeX Examples

Here we show some of the examples that is written in LaTeX.

---

### insDLJS

Simple package that includes a Java voice script to your .pdf files.

### thesis template

Thesis template for a degree of Masters or PhD in Central China Normal University
English version (although it is compulsory for students to include a Chinese translated abstract)

- The document class is ctex (so we don't have to wrap CJK around every time we want to include some Chinese)
- most of the stuff can be adjusted in the `settings.tex` file in the `tex/` folder
- the `main.tex` file controls which section to compile, so when you are working on chapter 2, you can comment out the rest of the
  document.
- the compile sequence is as usual:
```
pdflatex -synctex=1 -interaction=nonstopmode  -shell-escape main.tex
bibtex main
pdflatex -synctex=1 -interaction=nonstopmode  -shell-escape main.tex
pdflatex -synctex=1 -interaction=nonstopmode  -shell-escape main.tex
```
- the `ctex` manual is also included in the `manuals` folder for code reference

