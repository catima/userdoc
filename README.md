# CATIMA end-user documentation

This repo contains the end-user documentation for CATIMA. Currently, the end-user documentation is in French only, but translations to English and German are planned.

The documentation uses [MkDocs](http://www.mkdocs.org/) to build the pages based on Markdown files in this repo.

For each language, there is one folder (currently the [fr](fr) folder for the French documentation). In each folder, there is a `mkdocs.yml` file specifying the build options, and a `docs` folder containing the documentation itself in Markdown format.

## Prerequisites

In order to view or build the documentation, you need to install [MkDocs](http://www.mkdocs.org/) on your computer. See the [MkDocs](http://www.mkdocs.org/) Website for the installation information.


## Get Started

To view the documentation:

```bash
cd <your-favourite-langage-directory>
mkdocs serve
```

and you should be able to access the documentation in your browser at [http://127.0.0.1:8000](http://127.0.0.1:8000).

To build the documentation:

```bash
cd <your-favourite-language-directory>
mkdocs build
```

and you will find the HTML version of the documentation in the `site` folder.

See the [MkDocs](http://www.mkdocs.org/) Website for more usage information.


