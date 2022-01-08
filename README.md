# Working with MRI Data in Python
 
[source:Introduction to Working with MRI Data in Python](https://carpentries-incubator.github.io/SDC-BIDS-IntroMRI/index.html)

---

The lesson will introduce different types of MRI modalities and how they can be easily organized and shared. This lesson is also a pre-requisite for the [Structural](https://carpentries-incubator.github.io/SDC-BIDS-sMRI), [Functional](https://carpentries-incubator.github.io/SDC-BIDS-fMRI) and [Diffusion](https://carpentries-incubator.github.io/SDC-BIDS-dMRI) MRI Data Analysis lessons, which go more in-depth into their respective MRI modalities.

## Setup

Check the details in [Setup](0-Setup.ipynb) notebook.

Necessary packages:

```
pip install nibabel, nilearn, pybids
conda install -c conda-forge dcm2niix datalad
```

## From the scanner to our computer

Objectives:
* Understand how different MRI modalities differ and what each one represents
* Become familiar with converting MRI data from DICOM to NIfTI

Check the details in [Scanner to Computer](1-Scanner_to_computer.ipynb) notebook.

## Anatomy of a NIfTI

Objectives
* Introduce Python data types
* Load an MRI scan into Python and understand how the data is stored
* Understand what a voxel is
* Introduce MRI coordinate systems
* View and manipulate image data

Check the details in [Anatomy of a NIfTI](2-Anatomy_of_a_NIfTI.ipynb)
