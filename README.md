# Source for https://clouds.eos.ubc.ca/compcomm/

This repository contains the source: https://gitlab.math.ubc.ca/phaustin/compblog

## Building the Blog

Clone the repository & make sure submodules are included

```
$ git clone https://gitlab.math.ubc.ca/phaustin/compblog
$ cd compblog
$ git submodule add git://github.com/getpelican/pelican-plugins.git plugins/pelican-plugins
$ git submodule add git://github.com/danielfrg/pelican-ipynb.git plugins/ipynb
```

Install the required packages (assuming miniconda 3.6):

```
$ conda installjupyter notebook
$ pip install pelican Markdown
```

Build the html and serve locally:

```
$ make html
$ make serve
$ open http://localhost:8000
```

Deploy to kite

```
$ make publish-to-kite
```
