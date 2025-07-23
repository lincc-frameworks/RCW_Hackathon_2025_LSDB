# LSDB hackathon at the Rubin Community Workshop 2025

<img src="https://cdn2.webdamdb.com/1280_2yYofV7cPVE1.png?1607019137" height="200"> [![LINCC Frameworks](https://github.com/astronomy-commons/lsdb/blob/main/docs/lincc-logo.png)](https://lsstdiscoveryalliance.org/programs/lincc-frameworks/)

Demos prepared for the LINCC Frameworks Hackathon at the Rubin Community Workshop, 2025, Tuscon
The noteboooks showcase working with HATS-partitioned survey catalogs via [LSDB](https://lsdb.io), and time domain analysis with [nested-pandas](https://nested-pandas.readthedocs.io/en/latest/).

### When and where:

**Sunday 27 July**

* 9:00am – Hackathon Welcome (at NOIRLab; NOIRLab is a 15 minute walk from the Tucson Marriott University Park or 3 stops on the free Sun Tran light rail)
* 9:30am – LINCC Frameworks Tutorials on LSDB and TDAstro
* 12:30am – Plenary Pitch Session
* 1:00pm – Hacking begins
* 5:00pm – Pizza and sandwich dinner provided; teams may continue working if so desired

**Monday 28 July**

* 9:00am-10:00am – RCW Plenary #1 , at Tucson Marriott University Park; NOIRLab is a 15 minute walk or 3 stops on the free Sun Tran light rail
* 10:30am – Plenary opening session, before hacking resumes
* 4:00pm – Plenary Project Presentations
* 5:00pm – Hackathon Close
* 5:30pm-8:00pm – Casual Social for Hackathon participants

### Event resources

* [Website](https://lsstdiscoveryalliance.org/lincc-frameworks-workshops-and-hackathons/)
* Slack channel
  * We will utilize the `#lincc-frameworks-hack-july2025` channel on LSST-DA slack.
* Pitches
  * Craft your Project Pitch ideas and share them with the other hackathon participants. 
  * Our [Pitch instructions PDF document](https://lsstcorg.sharepoint.com/:b:/g/ES_LXMmSL5VOtEh2ffiiAP8BIfJAFkVFpwfA61gI_OFMxA?e=yDORga) contains some Tips and FAQs and examples from the LF Team. 
  * When you’re ready to share, add your ideas to the [Google Docs Pitches](https://docs.google.com/document/d/10n7OfOHEYK-n0500OzpuSuV92CsmgCHHkaAwS22xcYw/edit?usp=sharing). * We also encourage you to post your ideas on this `#lincc-frameworks-hack-july2025` channel and brainstorm on each other’s posts. If there are things the LINCC Frameworks team might also be able to do in advance to help your project, feel free to ask for that too!
  * All documents we share with you will be available in this [Sharepoint Folder](https://lsstcorg.sharepoint.com/:f:/g/ErkRZva4HklFsmYtPW30P4gBJAD5_IgE4YyGn3g7crDMJw?e=iP5clb).

### Main references

* [Slide deck](https://docs.google.com/presentation/d/1tMBa8964guyaf0DGVZ7NsE2ox6TAkOcITgaTj4gPXWw)
* LSDB ([Main page](https://lsdb.io))([LSDB catalogs](https://data.lsdb.io))([on GitHub](https://github.com/astronomy-commons/lsdb))([on ReadTheDocs](https://lsdb.readthedocs.io/en/latest/))  
  * [Rubin Observatory DP1 documentation page for LSDB](https://dp1.lsst.io/products/lsdb.html)  
  * [Working with Rubin data section in LSDB documentation](https://docs.lsdb.io/en/latest/tutorial_toc/toc_rubin.html)
* HATS ([on GitHub](https://github.com/astronomy-commons/hats))([on ReadTheDocs](https://hats.readthedocs.io/en/stable/))
* nested-pandas ([on GitHub](https://github.com/lincc-frameworks/nested-pandas))([on ReadTheDocs](https://nested-pandas.readthedocs.io/en/stable/))

## Getting Started 

### On Rubin Science Platform

Make sure that you have access to the Rubin Science Platform and follow the instructions at [lsdb.io/dp1](https://lsdb.io/dp1). Note that LSDB data is still in soft launch phase, so you have to install `lsdb` package - e.g., by opening a notebook and running the following command (and restarting the kernel after it):

```
%pip install lsdb
```

For a complete guide to setting up an RSP account and getting LSDB available in
your notebooks, we've put together a [system guide](/setup/) that you might find useful.

## [Notebooks](/tutorials/)

### [Notebook 1](/tutorials/Notebook_1_Intro.ipynb)

In this notebook, we will learn how to:

- Import DASK client
- Load object and source catalogs (lazily)
- Show HATS partitioning with ZTF objects and source
- Perform crossmatching with existing `LSDB` catalogs
- Save the results of a science workflow to disk

### [Notebook 2](/tutorials/Notebook_2_Intro.ipynb)

In this notebook, we will learn:

- How to access photo-z catalog derived from Rubin’s Data Preview 1 with LSDB 

### [Notebook 3](/tutorials/Notebook_3_Intro.ipynb)

In this notebook, we will learn:

- What nested pandas is
- How to do basic operations on timeseries

### [Notebook 4](/tutorials/Notebook_4_Intro.ipynb)

In this notebook, we will learn how to:

- Crossmatch custom list of positions
- Access Object and diaObject data from Rubin DP1
- Show lightcurves for both Objects and diaObjects

### [Notebook 5](/tutorials/Notebook_5_Intro.ipynb)

In this notebook, we provide several AGN-related problems:

- Crossmatch SDSS AGNs with Rubin DP1 photo-z catalog
- Crossmatch a large catalog of AGN with Rubin DP1 data
- Run scientific analysis on lightcurves from Rubin DP1

## Acknowledgements

This project is supported by Schmidt Sciences.

This project is based upon work supported by the National Science Foundation under Grant No. AST-2003196.

This project acknowledges support from the DIRAC Institute in the Department of Astronomy at the University of Washington. The DIRAC Institute is supported through generous gifts from the Charles and Lisa Simonyi Fund for Arts and Sciences, and the Washington Research Foundation.
