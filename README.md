# LSDB Demo at the AGN Science Collaboration Meeting 2025

<img src="https://raw.githubusercontent.com/astronomy-commons/lsdb/main/docs/lincc-logo.png" width="300" height="100">

Demonstration prepared for the [AGN SC 2025 meeting], Durham, 2025.
This demo showcases working with HATS-partitioned survey catalogs via [LSDB](https://lsdb.readthedocs.io/en/stable/), and time domain analysis with [nested-pandas](https://nested-pandas.readthedocs.io/en/latest/).

### Main references

* [Slide deck](TBD)
* LSDB ([on GitHub](https://github.com/astronomy-commons/lsdb)) 
  ([on ReadTheDocs](https://lsdb.readthedocs.io/en/stable/))
* HATS ([on GitHub](https://github.com/astronomy-commons/hats))
  ([on ReadTheDocs](https://hats.readthedocs.io/en/stable/))
* nested-pandas ([on GitHub](https://github.com/lincc-frameworks/nested-pandas)) 
  ([on ReadTheDocs](https://nested-pandas.readthedocs.io/en/stable/))

## Getting Started 

You can follow along with this demo by creating your own local environment.

### Local installation

If installing in your own hardware, create a virtual environment and install the relevant packages:

```
>> conda create --name lincc python=3.12
>> conda activate lincc
>> pip install lsdb
```

## Notebooks

### [Notebook 1](TBD)

In this notebook we will learn how to:

- Load object and source catalogs (lazily)
- Perform crossmatching with existing `LSDB` catalogs
- Save the results of a science workflow to disk

## Acknowledgements

This project is supported by Schmidt Sciences.

This project is based upon work supported by the National Science Foundation under Grant No. AST-2003196.

This project acknowledges support from the DIRAC Institute in the Department of Astronomy at the University of Washington. The DIRAC Institute is supported through generous gifts from the Charles and Lisa Simonyi Fund for Arts and Sciences, and the Washington Research Foundation.
