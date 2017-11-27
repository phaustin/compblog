# Source for https://clouds.eos.ubc.ca/compcomm/

This repository contains the source: https://gitlab.math.ubc.ca/phaustin/compblog

## Building the Blog

Clone the repository & make sure submodules are included

```
$ git clone https://gitlab.math.ubc.ca/phaustin/compblog
$ git submodule update --init --recursive
```

Install the required packages:

```
$ conda create -n pelican-blog python=3.6 jupyter notebook
$ source activate pelican-blog
$ pip install pelican Markdown ghp-import
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
