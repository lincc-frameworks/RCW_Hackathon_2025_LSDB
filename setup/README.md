# Rubin Science Platform System Guide

This tutorial and hackathon is expected to take place primarily in the Rubin
Science Platform (RSP). This provides a jupyter lab interface, and some compute
resources for running science pipelines.

https://data.lsst.cloud/

## Access

The RSP is the primary point of access to all existing Rubin science data
(currently DP0 and DP1). Accounts are available to all Rubin Data Rights holders; 
verification is manual, so accounts should be request at least 1 week prior to our 
event. If your identity cannot be confirmed via your institution, please use a GitHub 
or an ORCID account to request access.
Instructions to set up an account are available at : 

https://rsp.lsst.io/guides/getting-started/get-an-account

## Start your server

* Go to data.lsst.cloud. You should see something like:

![The RSP main page][assets/01-rsp-main.png]

* You may need to login first. Once you see that page, press "Notebooks"
* This will take you to a server options menu. You can leave the "Image" as
  "Recommended". In "Options", set the size to "Large".

![The RSP Server Options page][assets/02-server-options.png]

* Press "Start"
* The server may take a few minutes to intialize. This is normal.

![The RSP Server loading page][assets/03-server-starting.png]

* Once your server has started, you will be taken to the jupyterlab Welcome page

![RSP JupyterLab Welcome page][assets/04-jupyterlab.png]

## Open Tutorial Notebooks

* You will clone this repository for the tutorial notebooks and solutions.
* First open a terminal window within jupyterlab with `File > New > Terminal`:

![How to open a new terminal window][assets/05-new-terminal.png]

* Copy/paste the following command into the terminal to fetch this repository:

```
$ git clone http://github.dev/lincc-frameworks/RCW_Hackathon_2025_LSDB
```

* This will be cloned into your user home directory. However, the home 
  directory is not the same as the welcome directory!
* To navigate to your home directory in the jupyterlab file viewer, click the root 
  folder in the very upper left

![How to navigate to your home directory][assets/07-home.png]

* From here, navigate to the `RCW_Hackathon_2025_LSDB` directory, and open the first
  notebook, `Notebook_1_Intro.ipynb`.

## Installing LSDB in your kernel

* If this is your first time using LSDB on the RSP, you'll need to install the python
  packages. The first cell in the notebook has an optional line to perform this 
  installation for you.

![Line to install LSDB][assets/08-install-lsdb.png]

* Be sure to uncomment only that line, and make sure you've removed the leading space
  on the line. It needs to start with the `%` to do jupyter "magic"!
* You will see loads of warnings and errors, and they're likely OK!

![Example of warnings from pip installation of LSDB][assets/09-warnings.png]

* You should restart your jupyter kernel for these new packages to be available.
  This is NOT the same as restarting your entire RSP server, and is just the 
  particular python environment used for a notebook.

![How to restart notebook kernel][assets/10-restart.png]

* After restarting, you can run the notebook's second cell, which imports LSDB and
  other dependencies.
* If LSDB has been installed correctly, and is available in the kernel, then you
  should see output with "Version of lsdb is 0.6.x"

![Example output of the second notebook cell with lsdb version][assets/11-lsdb-version.png]

* Note that your version may differ from this screenshot, if we release a new version
  in the days leading up to the hackathon.

## Clean up

* If you got this far, that's probably good enough for your hackathon pre-work!
* If you're done with your work on RSP for the day, it's very good practice to 
  explicitly shut down your RSP server. This frees resources for other scientists.

![How to exist RSP jupyterlab server][assets/12-exit.png]