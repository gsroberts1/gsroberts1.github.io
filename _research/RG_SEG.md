---
title: "Mumford-Shah Region Growing Segmentation"
layout: single-portfolio
excerpt: "<img src='/images/research/MP574.PNG' alt=''>"
permalink: /research/mp574
collection: research
type: "Current Projects"
venue: "University of Wisconsin - Madison"
location: "Madison, WI, USA"
order_number: 15
header: 
  og_image: "research/MP574.PNG"
---

Background
------
This was the final project for the *MP574: Image Processing* taught by [Diego Hernando](https://radiology.wisc.edu/profile/diego-hernando-706/) and [Sean Fain](https://medicine.uiowa.edu/radiology/profile/sean-fain). For this group project (with Timothy Ruesink and Lawrence Lechuga), we developed a novel region-growing algorithm that utilized a cost function (Mumford-Shah functional) to balance smoothness within a subregion, length of boundaries of subregions (to avoid spatial overfitting), and data consistency. We applied this segmentation to brain MRI images (from the BRATS-SMIR public database) with the goal of semantic segmentation of brain tumors. All members of the group contributed equally to this work. The abstract for the final paper is provided below:

> Segmentation is a vital task in modern medical image processing that serves to reduce data analysis only to specific subregions that are of clinical interest. Advances in medical imaging technologies have provided the medical and scientific communities with larger datasets of ever-increasing image quality. There is an inherent need for robust segmentation methods that can extract clinically important information automatically, as opposed to performing time-consuming manual segmentation which is still done today in some clinical applications. The goal of this project was two-fold – (1) to recreate a multi-stage segmentation algorithm that combines both region-growing with a simplified Mumford-Shah (SMS) functional and (2) to develop a novel region-growing algorithm using the same formulation but with added flexibility in initialization conditions and adjustments to the cost function calculation, in hopes of increasing efficiency and accuracy.

Manuscripts
------
### Final Report
[Download](/files/research/Region-Growing with Mumford-Shah Functional - Grant Roberts.pdf){: .btn--research}
Code can be found in the appendix of the final report.

