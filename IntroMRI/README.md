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

## Brain Imaging Data Structure (BIDS)

Objectives
* Organize data in a simple and intuitive way
* Use `BIDS Validator` to validate your data

Check the details in [Brain Imaging Data Structure (BIDS)](3-Brain_Imaging_Data_Structure_(BIDS).ipynb).
## Open MRI Datasets

Objectives

* Introduce some open MRI datasets
* Operations on these datasets

Check the details in [Open MRI Datasets](4-Open_MRI_Datasets.ipynb).

## Reference

Michael Joseph, Jerrold Jeyachandra, and Erin Dickie (eds):
"Data Carpentry: Introduction to MRI Data Analysis." Version 2019.11, November 2019,
https://github.com/carpentries-incubator/SDC-BIDS-IntroMRI