---
title: "4D Flow MRI - Portal Vein"
layout: single-portfolio
excerpt: "<img src='/images/research/PORTAL.png' alt=''>"
permalink: /research/portal
collection: research
type: "Current Projects"
venue: "University of Wisconsin - Madison"
location: "Madison, WI, USA"
order_number: 10
header: 
  og_image: "research/PORTAL.png"
---

Background
------
After completing the [chronic mesenteric ischemia](/_research/CMI.md) project, I have since been involved in several related projects due to my experience in using tools specific to abdominal 4D flow MRI, specifically [EnSight](https://www.ansys.com/products/fluids/ansys-ensight) and [Mimics](https://www.materialise.com/en/medical/mimics-innovation-suite/mimics), as well as image reconstruction. 

### Portal and Abdominal Review Papers
Several of our collaborators in the Radiology department, [Scott Reeder](https://radiology.wisc.edu/profile/scott-reeder-46/) and [Thekla Oechtering](https://radiology.wisc.edu/profile/thekla-oechtering-2323/), were invited to write several review papers on [Clinical Applications of 4D Flow MRI in the Portal Venous System](https://pubmed.ncbi.nlm.nih.gov/35082218/) and [Abdominal Applications of Quantitative 4D Flow MRI](https://pubmed.ncbi.nlm.nih.gov/34837521/). My primary role for these papers was to create Ensight figures for flow visualization. While this process was quite arduous, requiring semi-automated segmentation of the vasculature, generation of 2D cut-planes for analysis, flow quantification (if necessary), and generation of streamlines/pathlines, we ended up creating some really nice images. 

### Normal Portal Vein Hemodynamics
Quantifying normal blood flow is important for establishing reference blood flow ranges and is thus useful for identifying abnormal flow ranges caused by pathology. This is the idea behind the study, currently being led by Andrew Huang, where N=43 abdominal 4D flow scans from healthy subjects were analyzed to assess volumetric flow rates, peak velocities, vessel diameters, vorticity, and helicity in the portal vein (in a fasting state). My contributions to this study were assessing portal vein vorticity/helicity (along with 2 other readers), generating several figures, and analyzing 6 datasets independently. 

### Weight Loss Study
As a subaim of a larger study evaluating liver structure/function after weight loss surgery, we are currently exploring the effect of weight loss on PV hemodynamics over the course of the regimen. In the early phases of this study, it was observed that image quality was highly degraded to due to radial streaking artifcats caused by subcutaneous fat. To address this, fat saturation, in combintation with iterative SENSE techniques, were applied to mitigate this artifact, resulting in usable 4D flow datasets for hemodynamic analysis.

![](/images/research/PORTAL_1_fatsat.png)

For this project, I helped design the parameters to be used in our offline, custom PCVIPR reconstruction. I wrote and installed configuration files on the GE scanner to allow for image reconstructions to be automatically performed and transferred to our data servers. Alma Spahic (advised by Laura Eisenmenger and Oliver Wieben) has been analyzing these datasets, with recent work submited to ISMRM and SMRA. 

### Collaborations: 
[Scott Reeder Lab](https://qiml.radiology.wisc.edu/staff/reeder-scott/), [Alejandro Roldan CFD Lab](https://uwcvfd.engr.wisc.edu/), [Radius Medical Image Analysis](https://resources.research.wisc.edu/Core/Details/564), Thekla Oechtering, Andrew Huang, Alma Spahic

Awards
------
### Oral Presentation
* Spahic, A., Oechtering, T. H., Roberts, G. S., Roldan-Alzate, A., Reeder, S. B., Wieben, O., & Johnson, K. M. Abdominal 4D Flow MRI in Obese Patients – A Pilot Study. Society for Magnetic Resonance Angiography (SMRA) 33nd Annual International Conference. 2021 September.

### Poster Presentation
* Spahic, A., Roberts, G. S., Wolfson, T., Harris, D., Panagiotopoulos, N., Roldan-Alzate, A., Johnson, K. M., Wieben, O., Sirlin, C. B., Reeder, S. B., & Oechtering, T. H. Portal Venous 4D Flow MRI in Obese Patients Without Known Liver Disease Undergoing Weight Loss Surgery. Joint Annual Meeting ISMRM-ESMRMB & SMRT 31st Annual Meeting. 2022 May 7.

Manuscripts
------
### Submitted
* Oechtering, T. H., Roberts, G. S., Panagiotopoulos, N., Wieben, O., Reeder, S.B., & Roldan-Alzate, A. (2022). Clinical Applications of 4D Flow MRI in the Portal Venous System. Magnetic Resonance in Medical Sciences. 10.2463/mrms.rev.2021-0105
* Oechtering, T. H., Roberts, G. S., Panagiotopoulos, N., Wieben, O., Roldan-Alzate, A., & Reeder, S. B. (2021). Abdominal Applications of Quantitative 4D Flow MRI. Abdominal Radiology. 10.1007/s00261-021-03352-w. 
### In-Preparation
* Huang, A., Roberts, G. S., Reeder, S. B., & Oechtering, T. H. Reference Values for 4D Flow Magnetic Resonance Imaging of the Portal Venous System. To Submit to Abd. Radiol.

