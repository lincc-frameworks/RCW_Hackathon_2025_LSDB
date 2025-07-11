# LSDB hackathon at the AGN Science Collaboration Meeting 2025

<img src="https://raw.githubusercontent.com/astronomy-commons/lsdb/main/docs/lincc-logo.png" width="300" height="100">

Demos prepared for the [AGN SC 2025 meeting](https://agn.science.lsst.org/?q=meeting2025), Durham, 2025.
The noteboooks showcase working with HATS-partitioned survey catalogs via [LSDB](https://lsdb.io), and time domain analysis with [nested-pandas](https://nested-pandas.readthedocs.io/en/latest/).

### When and where:

Monday 14, 12:30 - 12:50, OCW017 room - [presentation](https://docs.google.com/presentation/d/1FnZF5o-ZdEKGN3tu5d2xakc2o_satLK7Dl4KNnFZeYg/)   
Monday 14, 14:00 - 15:40, OCW116 room - hackathon (guided notebooks)  
Monday 14, 16:10 - 17:30, OCW116 room - hackathon (free coding)

### Main references

* [Slide deck](TBD)
* LSDB ([Main page](https://lsdb.io))([LSDB data](https://data.lsdb.io))([on GitHub](https://github.com/astronomy-commons/lsdb))([on ReadTheDocs](https://lsdb.readthedocs.io/en/latest/))  
  &nbsp;&nbsp;* [Working with Rubin data section in LSDB documentation](https://docs.lsdb.io/en/latest/tutorial_toc/toc_rubin.html)
* HATS ([on GitHub](https://github.com/astronomy-commons/hats))([on ReadTheDocs](https://hats.readthedocs.io/en/stable/))
* nested-pandas ([on GitHub](https://github.com/lincc-frameworks/nested-pandas))([on ReadTheDocs](https://nested-pandas.readthedocs.io/en/stable/))

## Getting Started 

### On Rubin Science Platform

Make sure that you have access to the Rubin Science Platform and follow the instructions at [lsdb.io/dp1](https://lsdb.io/dp1). Note that LSDB data is still in soft launch phase, so you have to install `lsdb` package - e.g., by opening a notebook and running the following command (and restarting the kernel after it):

```
%pip install lsdb
```

After that you should be able to access:
```
lsdb.open_catalog('/rubin/lsdb_data/object_collection')
lsdb.open_catalog('/rubin/lsdb_data/dia_object_collection')
lsdb.open_catalog('/rubin/lsdb_data/object_photoz')
```

If you want to keep your enviroment clean, at the end of the workshop, uninstall `LSDB` and any other packages you may have installed with appropriate commands like
```
%pip uninstall lsdb
```

### Local installation
You can follow along with this demo by creating your own local environment.
If installing in your own hardware, create a virtual environment and install the relevant packages:

```
conda create --name lsdb_env python=3.12
conda activate lsdb_env
pip install lsdb
```

Note that you will have to change the paths to the data to point to local copy of Rubin Data Preview 1 data. 

## Notebooks

### [Notebook 1](Notebook_1.ipynb)

In this notebook we will learn how to:

- Import DASK client
- Load object and source catalogs (lazily)
- Show HATS partitioning with ZTF objects and source
- Perform crossmatching with existing `LSDB` catalogs
- Save the results of a science workflow to disk

### [Notebook 2](Notebook_2.ipynb)

In this notebook we will learn how to:

- What nested pandas is
- Do basic operations on timeseries

### [Notebook 3](Notebook_3.ipynb)

In this notebook we will learn how to:

- How to access photo-z catalog derived from Rubin’s Data Preview 1 with LSDB 

### [Notebook 4](Notebook_4.ipynb)

In this notebook we will learn how to:

- Crossmatch custom list of positions
- How to access Object and diaObject data
- Show lightcurves for both Objects and diaObjects

### [Notebook 5](Notebook_5.ipynb)

In this notebook we provide several AGN-related problems:

- Crossmatch SDSS AGNs with Rubin DP1 photo-z catalog
- Crossmatch large catalog of AGN with Rubin DP1 data
- Run scientific analysis on lightcurves from Rubin DP1

## Acknowledgements

This project is supported by Schmidt Sciences.

This project is based upon work supported by the National Science Foundation under Grant No. AST-2003196.

This project acknowledges support from the DIRAC Institute in the Department of Astronomy at the University of Washington. The DIRAC Institute is supported through generous gifts from the Charles and Lisa Simonyi Fund for Arts and Sciences, and the Washington Research Foundation.
