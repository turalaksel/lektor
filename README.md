# Lektor

[![Tests master](https://github.com/lektor/lektor/workflows/Tests%20master/badge.svg)](https://github.com/lektor/lektor/actions?query=workflow%3A%22Tests+master%22)
[![Code Coverage](https://codecov.io/gh/lektor/lektor/branch/master/graph/badge.svg)](https://codecov.io/gh/lektor/lektor)
[![PyPI version](https://badge.fury.io/py/Lektor.svg)](https://pypi.org/project/Lektor/)
[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Lektor.svg)](https://pypi.org/project/Lektor/)
<img alt="node:?" src="https://img.shields.io/badge/node-%3E=8-blue.svg"/>
[![Join the chat at https://gitter.im/lektor/lektor](https://badges.gitter.im/lektor/lektor.svg)](https://gitter.im/lektor/lektor?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Lektor is a static website generator.  It builds out an entire project
from static files into many individual HTML pages and has a built-in
admin UI and minimal desktop app.

<img src="https://raw.githubusercontent.com/lektor/lektor-assets/master/screenshots/admin.png" width="100%">

To see how it works look at the ``example`` folder which contains a
very basic project to get started.

For a more complete website look at [lektor/lektor-website](https://github.com/lektor/lektor-website)
which contains the sourcecode for the official lektor website. We also have the example project at the
top level of this repository `example/` that is a lean example of the wide variety of the features
of Lektor.

## How do I use this?

For installation instructions head to the official documentation:

* [Installation](https://www.getlektor.com/docs/installation/)
* [Quickstart](https://www.getlektor.com/docs/quickstart/)

## Want to develop on Lektor?

This gets you started:

```
$ git clone https://github.com/lektor/lektor
$ cd lektor
$ virtualenv venv
$ . venv/bin/activate
$ pip install --editable .
$ make build-js
$ make install-git-hooks
$ export LEKTOR_DEV=1
$ cp -r example example-project
$ lektor --project example-project server
```

If you want to run the test suite:

```
$ virtualenv venv
$ . venv/bin/activate
$ pip install --editable ".[test]"
$ make test
```
