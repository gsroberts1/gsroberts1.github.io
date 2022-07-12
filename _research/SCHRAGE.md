---
title: "MetSyn Image Registration"
layout: single-portfolio
excerpt: "<img src='/images/research/SCHRAGE.png' alt=''>"
permalink: /research/metsyn
collection: research
type: "Current Projects"
venue: "University of Wisconsin - Madison"
location: "Madison, WI, USA"
order_number: 8
header: 
  og_image: "research/SCHRAGE.png"
---

Background
------
In 2021, we were approached by another research group ([Schrage Lab](https://cvrc.wisc.edu/staff/schrage-william/)) studying regional cerebral blood flow (CBF) in individuals with metabolic syndrome (MetSyn). To test the contribution of cyclooxygenase enzyme on energy regulation, subjects were administered indomethacin. The effect of this drug reduced CBF and blood velocities in both controls and subjects with MetSyn. Because Venc parameters were constant (100 cm/s) before and after administration of indomethacin, reductions in blood velocities adversely affected angiogram quality which made it extremely difficult to perform hemodynamic analysis.

Our first attempt at this problem was to adjust our complex difference "formula" by weighting the magnitude and phase of our signal separately, increasing the weight of the magnitude image (see the [paper](https://onlinelibrary.wiley.com/doi/full/10.1002/jmri.23501) by Kecskemeti et al). However, this was not sufficient in increasing angiogram quality. Our second attempt was to apply compressed sensing and local low rank reconstructions to improve phase signal. While this did improve image quality, it was still not sufficient in recreating angiograms from the baseline (non-indomethacin) scans. 

Our last attempt, which proved to be sucessful, was to apply image registration techniques to register the indomethacin scans to the high-quality baseline scans. Image registration was applied in Matlab and was required because there were slight differences in patient positioning between scan sessions, which caused the datasets to be unaligned. First, 3D rigid registration was performed on magnitude-weighted complex difference with a gradient descent optimizer and Mattes mutual information metric. Deformable registration was then applied using a demons algorithm for fine-tuning. After registering the complex difference angiograms, magnitude and velocity data were also co-registered using the obtained rigid transformations and deformable displacement fields. After all indomethacin data were aligned to the baseline scan, the complex difference angiograms from the baseline scan were used to create a vessel centerline structure for the indomethacin scans. The [new cranial 4D flow analysis tool](/_research/QVT), which we helped integrate into their workflow, was used to calculate hemodynamic parameters necessary for their study on MetSyn. 

![](/images/research/SCHRAGE.png)

Code
------
[Angiogram weighting and registration code](/files/research/MetSyn_registration_code.zip)

Manuscripts
------
### In Preparation
* Carter, K. J., Ward, A. T., Kellawan, J. M., Harrell, J. W., Peltonen, G. L., Roberts, G. S., Al-Subu, A., Hagen, S. A., Serlin, R. C., Eldridge, M., Wieben, O., & Schrage, W. G. Reduced Resting Macrovascular and Microvascular Cerebral Blood Flow in Young Adults with Metabolic Syndrome: Exploring Mechanisms. Submitted to JCBFM.
