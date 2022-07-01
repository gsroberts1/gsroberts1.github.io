---
title: "QVT"
layout: single-portfolio
excerpt: "<img src='/images/research/QVT.png' alt=''>"
permalink: /research/qvt
collection: research
type: "Current Projects"
venue: "University of Wisconsin - Madison"
location: "Madison, WI, USA"
order_number: 3
header: 
  og_image: "research/QVT.png"
---

Background
------
4D flow MRI is a time-resolved, 3D phase contrast imaging technique with three-directional velocity encoding that allows for non-invasive acquisitions of volumetric velocity vector fields. In other words, 4D flow MRI can show movement and direction (typically blood) within the brain. By obtaining blood velocities, we can calculate blood flow and other hemodynamic parameters, which have been used to diagnose and characterize a wide range of intracranial disease, such as aneurysms, arteriovenous malformations, and even vascular dementia. 

![](/images/research/QVT_1_pcviprAngio.gif)

Despite great advances in 4D Flow MRI acquisition and reconstruction, efficient and repeatable post-processing methods for cranial 4D flow MRI datasets remain a challenge. The high dimensionality of the reconstructed datasets (1 temporal, 3 spatial dimensions, and 3 velocity directions) and the complexity of the brain vasculature which often requires the simultaneous analysis of numerous vessels and can lead to prohibitively long post-processing times. Typical processing steps usually require manual vessel segmentation and manual placement of double-oblique tangent planes for hemodynamic analysis, approaches that are impractical when analyzing numerous vessels across a large number of datasets. User-dependent manual segmentation and plane placement also reduce the reproducibility of 4D flow MRI-derived hemodynamic parameters. 

Here we introduce an extension to a previously established 4D flow post processing tool1 that automatically segments and quantifies hemodynamic parameters in all vessel segments without the need for user interaction. This simplified post processing pipeline allows for robust and repeatable analysis and provides users the ability to easily visualize and quantify complex cranial 4D flow datasets.

### Background Phase Correction
![](/images/research/BGPC.png)

My contributions: 


Code
------
[QVT (Matlab)](https://github.com/uwmri/QVT)

Abstracts
------
### Oral Presentation
* Hoffman, C. A., Roberts, G. S., Berman, S., Eisenmenger, L. B., & Wieben, O. Towards Automated Cranial 4D Flow Cranial Analysis. Society for Magnetic Resonance Angiography (SMRA) 31st Annual International Conference; 2019 August 27; Nantes, France.

### Poster Presentation
* Hoffman, C. A., Roberts, G. S., Berman, S., Eisenmenger, L. B., & Wieben, O. Automated Cranial 4D Flow MRI Analysis. Alzheimer's Disease and Related Disorders Research Day 2020; 2020 March 5; Madison, WI, USA.
* Roberts, G. S., Johnson, K. M., Hoffman, C. A., Eisenmenger, L. B., & Wieben, O. Automating Background Phase Correction in Cranial 4D Flow MRI. Society for Magnetic Resonance Angiography (SMRA) 31st Annual International Conference; 2019 August 27; Nantes, France.

Manuscripts
------
### In-Preparation
* Hoffman, C. A., Roberts, G. S., Berman, S. E., Eisenmenger, L. B., & Wieben, O. Automated Post-Processing of Cranial 4D Flow MRI. To Resubmit to Journal of Medical Imaging.