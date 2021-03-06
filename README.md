# transformers

This repository contains several scripts for transformation of bibliographic
records, used in GBV library union network (*Kommentare sind auch auf Deutsch
möglich*).

# Overview

Each transformer script is located in one subdirectory named by input and
output formats.

## Unit tests

Unit tests can be added in subdirectory `test`. There must be a script called
`runtest.sh` in each transformer directory, to actually exectute the tests.
Test should print output in Tests Anything Protocol (TAP) format. To run tests
of all transformers, call `testall.sh`.

[![Build Status](https://travis-ci.org/gbv/transformers.png)](https://travis-ci.org/gbv/transformers)

See `testrunner` for useful bash functions to write tests.

# List of transformers

## marcxml2mods

Für den GBV angepasste Version des XSL-Stylesheets der LOC für die
Transformation von MARCXML nach MODS3.6

## pica2gndlx

Developer version of transformation from GND authority records in PICAXML to
GND Light XML.

## mods2rdf

Experimental transformation from MODS to RDF/XML

## gndlx2mads

Experimental transformation from GNDLX to MADS

# Related work

This repository does not contain specific tools for (mass) conversion of
records but only the scripts for single steps. The following projects include
similar works for conversion of bibliographic records:

* The [CultureGraph](http://www.culturegraph.org/) project has developed a tool
  suite for metadata processing, called [metafacture](https://github.com/culturegraph/metafacture-core/wiki).
* [LibreCat/Catmandu](http://www.librecat.org/) includes a metadata conversion
  framework

