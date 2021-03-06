# Introduction to sMRI (Pre)processing and Analysis in Python

[source: SDC-BIDS-sMRI](https://github.com/carpentries-incubator/SDC-BIDS-sMRI)

---

The primary goals are to:
* Understand the basics of structural MR image acquisition
* Familiarize yourself with structural MR image (pre)processing pipelines
* Perform and visualize group-level neuroanatomical analyses

Things to keep in mind:

* Magnetic resonance (MR) imaging is a medical imaging technique used to visualize anatomy and the physiological processes of the body. MR imaging scanners use strong magnetic fields, magnetic field gradients, and radio waves to generate images of the organs in the body.
* In structural neuroimaging, MR scans can refer to several different image modalities including, T1-weighted, T2-weighted, diffusion weighted images (DWI), Proton-Density (PD), Fluid attenuation inversion recovery (FLAIR) etc.
* An MR (pre)processing pipeline is a set of sequential image processing tasks performed on acquired MR scans prior to the statistical analysis.
* MR software packages: In order to standardize and simplify computational effort, several software packages encapsulate MR (pre)processing pipelines. This will 1) help developers to improve the underlying algorithms and 2) help users to customize the neuroimaging pipelines according to specific dataset requirements.

## [Setup](https://carpentries-incubator.github.io/SDC-BIDS-sMRI/setup.html)

Setting up Python environment first, using Anaconda.

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

## [sMRI Clean Up](https://carpentries-incubator.github.io/SDC-BIDS-sMRI/02-Image_Cleanup/index.html)

Questions: 
* What are the sources of noise and artifacts in MR images?
* How do we extract/mask the brain

Objectives:
* Visualize bias fields and motion artifacts
* Generate brain masks

Check the details in [sMRI Clean-up](2-sMRI_Clean-up.ipynb).

##  [sMRI Spatial Normalization](https://carpentries-incubator.github.io/SDC-BIDS-sMRI/03-Image_Spatial_Normalization/index.html)

Questions:
* What are reference coordinate systems
* What are 'templates', 'atlases'?
* What is spatial normalization?

Objectives:
* Understand reference spaces and registration process

Check the details in [sMRI Spatial Normalization](3-sMRI_Spatial_Normalization.ipynb)

##  [sMRI Segmentation and Parcellation](https://carpentries-incubator.github.io/SDC-BIDS-sMRI/04-Image_Quantification/index.html)

Objectives:
* Understand and visualize tissue segmentation
* Manipulate atlases to extract regions of interests
* Visualize and interact with both volumetric and surface data

Check the details in [sMRI Segmentation and Parcellation](4-sMRI%20Segmentation%20and%20Parcellation.ipynb)

## [sMRI Quality Control](https://carpentries-incubator.github.io/SDC-BIDS-sMRI/05-Image_QC/index.html)

Objectives:

* Visualize processing failures
* Familiarize with automatic QC tools
 
Check the details in [sMRI Quality Control](5-sMRI_Quality_Control.ipynb)

## [sMRI Statistical Analysis](https://carpentries-incubator.github.io/SDC-BIDS-sMRI/06-Statistical_Analysis/index.html)

Objectives:

* Understand the main metrics characterizing the brain morphology
* Extract and rely on a set of metrics to assess the effect of age on multiple cortical regions
* Understand and implement voxel based morphometry to investigate the effect of age without predefined regions.

There is some deprecated function which cannot visualize modulation correctly. I will fix it later.

Check the details in [sMRI Statistical Analysis](6-sMRI_Statistical_Analysis.ipynb)

## [sMRI Reproducibility Considerations](https://carpentries-incubator.github.io/SDC-BIDS-sMRI/07-Reproducibility/index.html)

Objectives
* Understand impact of software and atlas choices

Check the details in [sMRI Analysis: Reproducibility Considerations
](7-sMRI_Analysis_Reproducibility_Considerations.ipynb)