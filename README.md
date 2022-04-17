# DragonFly
B.Tech Project Slides

This repository houses the latex beamer template for creating presentation slides, reporting the works done in the project.

## [References](references.md)


## Compiling Latex document
1. Move into the required directory using `cd` command
2. Compile the main tex file into pdf using pdflatex.
  ```bash
  pdflatex main.tex
  ```
  If your project have bib files, you need a series of compilation
  ```bash
  pdflatex main.tex
  bibtex main
  pdflatex main.tex
  pdflatex main.tex
  ```
  If you prefer to change the location of intermediate build files, use the following command to build and compile
  ```bash
  pdflatex --output-directory=/tmp main.tex
  ```

3. (Optional) Remove the build files using git. The git un-tracked files can be removed using the `clean`. **Warning this removes all un-tracked files from the directory. Check the gitignore file**.
  ```bash
  git clean -xf
  ```
