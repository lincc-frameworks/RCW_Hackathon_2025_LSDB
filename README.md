# LSDB Demo at the AGN Science Collaboration Meeting 2025

<img src="https://raw.githubusercontent.com/astronomy-commons/lsdb/main/docs/lincc-logo.png" width="300" height="100">

Demonstration prepared for the [AGN SC 2025 meeting](https://agn.science.lsst.org/?q=meeting2025), Durham, 2025.
This demo showcases working with HATS-partitioned survey catalogs via [LSDB](https://lsdb.io), and time domain analysis with [nested-pandas](https://nested-pandas.readthedocs.io/en/latest/).

### When and where:

Monday 14, 12:30 - 12:50, OCW017 room - [presentation](https://docs.google.com/presentation/d/1FnZF5o-ZdEKGN3tu5d2xakc2o_satLK7Dl4KNnFZeYg/)   
Monday 14, 14:00 - 15:40, OCW116 room - hackaton (guided notebooks)  
Monday 14, 16:10 - 17:30, OCW116 room - hackaton (free coding)

### Main references

* [Slide deck](TBD)
* LSDB ([Main page](https://lsdb.io))([LSDB data](https://data.lsdb.io))([on GitHub](https://github.com/astronomy-commons/lsdb))([on ReadTheDocs](https://lsdb.readthedocs.io/en/latest/))  
  &nbsp;&nbsp;* [Working with Rubin data section in LSDB documentation](https://docs.lsdb.io/en/latest/tutorial_toc/toc_rubin.html)
* HATS ([on GitHub](https://github.com/astronomy-commons/hats))([on ReadTheDocs](https://hats.readthedocs.io/en/stable/))
* nested-pandas ([on GitHub](https://github.com/lincc-frameworks/nested-pandas))([on ReadTheDocs](https://nested-pandas.readthedocs.io/en/stable/))

## Getting Started 

### On Rubin Science Platform

Coming soon! 

### Local installation
You can follow along with this demo by creating your own local environment.
If installing in your own hardware, create a virtual environment and install the relevant packages:

```
>> conda create --name linccF python=3.12
>> conda activate linccF
>> pip install lsdb
```

Note that you will have to change the paths to the data to point to local copy of Rubin Data Preview 1 data. 

## Notebooks

### [Notebook 1](Notebook_1.ipynb)

In this notebook we will learn how to:

- Load object and source catalogs (lazily)
- Perform crossmatching with existing `LSDB` catalogs
- Save the results of a science workflow to disk

### [Notebook 2](Notebook_2.ipynb)

In this notebook we will learn how to:

- What nested pandas is
- Do basic operations on timeseries

### [Notebook 3](Notebook_3.ipynb)

In this notebook we will learn how to:

- Open photo-z catalog 
- What is in the photo-z catalog and what methods were used

### [Notebook 4](Notebook_4.ipynb)

In this notebook we will learn how to:

- Crossmatch custom list of positions with Objects and diaObjects
- Apply a simple function (flux to magnitude)
- Show lightcurves for both Objects and diaObjects

- ### [Notebook 5](Notebook_5.ipynb)

In this notebook we give few ideas for AGN work:

- Crossmatch SDSS AGNs with Rubin photo-z catalgo
- Crossmatch large catalog of AGN with Rubin DP1 data
- Run scientific analysis on lightcurves

## Acknowledgements

This project is supported by Schmidt Sciences.

This project is based upon work supported by the National Science Foundation under Grant No. AST-2003196.

This project acknowledges support from the DIRAC Institute in the Department of Astronomy at the University of Washington. The DIRAC Institute is supported through generous gifts from the Charles and Lisa Simonyi Fund for Arts and Sciences, and the Washington Research Foundation.
