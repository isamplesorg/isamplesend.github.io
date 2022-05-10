= isamplesorg.github.io

image:https://github.com/isamplesorg/isamplesorg.github.io/workflows/Build%20Pages/badge.svg[Action Status]

This repository provides the https://isamplesorg.github.io/[iSamples web site].

It is a https://www.sphinx-doc.org/en/master/[Sphinx] project configured to used the
https://sphinx-book-theme.readthedocs.io/en/latest/[sphinx-book-theme] and supports
both Markdown footnote:[Markdown support is provided by https://myst-nb.readthedocs.io/en/latest/[MyST-NB]
which is an extension to https://myst-parser.readthedocs.io/en/latest/[MyST]] and
reStructuredText footnote:[See: Sphinx https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html[reStructuredText]] formats.

The pages are built automatically and published to the `gh-pages` branch 
after a commit to the main branch. The automated build process is performed 
using https://github.com/isamplesorg/isamplesorg.github.io/actions[GitHub Actions]
using the workflow at link:blob/main/.github/workflows/gh-pages.yml[`.github/workflows/gh-pages.yml`].

== Development

Dependencies are managed using https://python-poetry.org/[Poetry]. To setup a local
work environment:

----
git clone
cd isamplesorg.github.io
poetry install
----

Building the docs:

----
cd docs
make html
----

or to start a webserver locally and and automatically
refresh pages on edit:

----
cd docs
make livehtml
----



