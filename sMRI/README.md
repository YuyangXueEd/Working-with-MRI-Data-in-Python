# Introduction to sMRI (Pre)processing and Analysis in Python

[source: SDC-BIDS-sMRI](https://github.com/carpentries-incubator/SDC-BIDS-sMRI)

---

The primary goals are to:
* Understand the basics of structural MR image acquisition
* Familiarize yourself with structural MR image (pre)processing pipelines
* Perform and visualize group-level neuronatomical analyses

Things to keep in mind:

* Magnetic resonance (MR) imaging is a medical imaging technique used to visualize anatomy and the physiological processes of the body. MR imaging scanners use strong magnetic fields, magnetic field gradients, and radio waves to generate images of the organs in the body.
* In structural neuroimaging, MR scans can refer to several different image modalities including, T1-weighted, T2-weighted, diffusion weighted images (DWI), Proton-Density (PD), Fluid attenuation inversion recovery (FLAIR) etc.
* An MR (pre)processing pipeline is a set of sequential image processing tasks performed on acquired MR scans prior to the statistical analysis.
* MR software packages: In order to standardize and simplify computational effort, several software packages encapsulate MR (pre)processing pipelines. This will 1) help developers to improve the underlying algorithms and 2) help users to customize the neuroimaging pipelines according to specific dataset requirements.

## [Setup](https://carpentries-incubator.github.io/SDC-BIDS-sMRI/setup.html)

Setting up Python environement first, using Anaconda.

```
conda install -y numpy pandas scipy scikit-learn matplotlib seaborn jupyter ipykernel nb_conda
conda install -y -c conda-forge awscli lxml nilearn nibabel statsmodels
pip install pybids
```

All datasets needed for the notebook examples are inside the `local_data/` directory.

## [sMRI Acquisition and Modalities](https://carpentries-incubator.github.io/SDC-BIDS-sMRI/01-Image_Modalities/index.html)

Questions:
* How is a structural MR image acquired?
* What anatomical features do different modalities capture?

Objectives:
* Visualize and understand difference in T1, T2, PD/FLAIR weighted images.

Check the detail in [sMRI Acquisition and Modalities](1-sMRI_Acquisition_and_Modalities.ipynb).


