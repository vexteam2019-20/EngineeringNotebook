# Engineering Notebook

Welcome! This is our virtual engineering notebook for 2019-20. Find the compiled `.pdf` file [here](https://github.com/vexteam2019-20/EngineeringNotebook/blob/master/src/main.pdf).

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/92f1e7b5af7a42e096bf52b91ee0e8d7)](https://www.codacy.com/manual/rishiosaur/EngineeringNotebook?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=vexteam2019-20/EngineeringNotebook&amp;utm_campaign=Badge_Grade)

## Building

### Setup

First, `git clone` this repository, then run `npm i`, assuming you're on the latest version of `node`. This will install `husky-hooks`, which we're using for quality control.

### LaTeX

This notebook is created using the LaTeX language, and so it requires installation of the LaTeX language.

Build it using `xelatex main.tex -pdf` to build a pdf, assuming you're in the same directory as `main.tex`.

Clear all auxillary files using `latexmk -c`

### NPM Commands

We have a selection of useful `npm` commands, like:

`npm test`: Compiles project, then deletes output files if compilation is successful.

`npm run clean`: Runs `latexmk -c` on your files. This is also run as a pre-commit hook.

## Contributing

### Folders

The folder structure goes like this:

`sections/<Strategizing|Designing|Building|Testing|Programming>`.

In order to contribute, you must place a `.tex` file in the appropriate subdirectory, and add it to the `main.tex` file.

### Files

Your `.tex` file body must be of the form:

```latex
\section{\textbf{<Describe your contributions>}: <date>}

<Contributions, laid out with \subsections>.
```

### Commits

Your commits are always cleaned before they are commited, so you don't have to worry about writing bad code, or useless files.
