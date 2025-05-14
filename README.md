
For compiling a reference for each chapter.

latex  main          # 1st LaTeX: creates main.aux, chapter1.aux, chapter2.aux …
bibtex chapter1      # produces chapter1.bbl
bibtex chapter2      # produces chapter2.bbl
# … one bibtex call for every chapter that has references …

latex  main          # 2nd LaTeX: incorporates the .bbl files
latex  main          # 3rd LaTeX: resolves cross-refs, table of contents, etc.
