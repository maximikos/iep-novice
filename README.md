# IEP Website (Sphinx/gh pages)

Maintainance Team : [@maximikos](https://github.com/maximikos) and the student chapter board of [ISIE](https://is4ie.org/)

## Overview

### Repository Structure

TBD

```
.
├── environment.yml
├── source/
│   ├── conf.py
|   ├── index.md
│   └── content/
│       ├── setup/
│       ├── introduction/
│       └── (...other documentation sections)
├── README.md
└── (...)
```

### Sphinx

tbd

### gh pages

tbd

## Quickstart

### Setup Repository

tbd

### Setup Python Environment

tbd

```bash
conda env create -f 'environment.yml'
```

and activate the environment:

```bash
conda activate sphinx_documentation
```

You are now ready to build the website...

### Building the Website

1. You can build the website by __triggering every build manually__: To trigger the build, run [`sphinx-build`](https://www.sphinx-doc.org/en/master/man/sphinx-build.html) from the repository root directory:

```bash
sphinx-build source _build/html -b singlehtml -a
```

| option | value | description |
| ---------------------------- | ----- | ----------- |
| sourcedir | `source` | N/A |
| outdir | `_build/html` | N/A |
| -b | `singlehtml` | create only a single html page |
| -a | N/A | always write all output files |
| `-j` | `auto` | [speed up build by using multiple processes](https://www.sphinx-doc.org/en/master/man/sphinx-build.html#cmdoption-sphinx-build-j) |


You can now preview the website, built as a single html page at:

```
_build/html/homepage.html
```

2. You can also build the website by automatically triggering a build after every change to the source files, providing a "live" preview of changes. To trigger the automated builds, run [`sphinx-autobuild`](https://github.com/executablebooks/sphinx-autobuild) from the repository root directory:

```bash
sphinx-autobuild source _build/html -a -j auto --open-browser
```

| positional argument or option| value | description |
| ---------------------------- | ----- | ----------- |
| sourcedir | `source` | N/A |
| outdir | `_build/html` | N/A |
| `-a` | N/A | always write all output files |
| `-j` | `auto` | [speed up build by using multiple processes](https://www.sphinx-doc.org/en/master/man/sphinx-build.html#cmdoption-sphinx-build-j) |
| `--open-browser` | N/A | automatically open browser |


You can now preview the documentation at (the browser window will open automatically ✨):
http://127.0.0.1:8000/


### Contributing

tbd