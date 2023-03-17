---
title: "Normative Cerebral Hemodynamics"
layout: single-portfolio
excerpt: "<img src='/images/research/NORMALS.png' alt=''>"
permalink: /research/normals
collection: research
type: "Current Projects"
venue: "University of Wisconsin - Madison"
location: "Madison, WI, USA"
order_number: 2
header: 
  og_image: "research/NORMALS.png"
---

Background
------
A normal supply of cerebral blood flow (CBF) is extremely important to maintain the metabolic needs of the brain and is thus highly regulated (see [cerebral autoregulation](https://en.wikipedia.org/wiki/Cerebral_autoregulation)). However, age-related neurovascular changes (aterial stiffnening, neurovascular uncoupling, etc) begin to occur which have direct impacts on cerebral hemodynamics. Recent evidence suggests that vascular pathology is a major risk factor for AD-related dementia with several studies indicating that it not only contributes to cognitive decline but also to neuronal loss in AD-related Aβ and tau pathologies. Thus, studying these age-related neurovascular changes are therefore important for understanding normal aging, cerebrovascular disease, and potentially Alzheimer's disease.

To understand these changes, it is important to first establish normal blood flow and flow pulsatility (which reflects downstream resistance) in older adults. While intracranial blood flow and pulsatility have been reported in older populations, these studies were limited either due to smaller population sizes or use of methodologies not well-suited to studying multiple vessel segments. Namely, 2D phase contrast (2DPC) MRI requires tedious plane prescription to measure hemodynamics in multiple vessels and transcranial doppler ultrasound (TCD) which is highly operator dependent. [4D flow MRI](https://pubmed.ncbi.nlm.nih.gov/23090914/) is a powerful, non-invasive phase contrast MRI technique that allows one to acquire blood velocities in a single 3D imaging volume without the need for contrast agents, making it suitable for comprehensive intracranial hemodynamic analysis. Any vessel within the acquired volume can be retrospectively analyzed after imaging, unlike TCD and 2DPC MRI. This makes 4D flow MRI ideal for large-scale studies analyzing vessel-specific hemodynamics. However, obtaining hemodynamics from 4D flow is still very challenging, requiring complex tools. 

Recently, Carson Hoffman and I helped improve a previously established [cranial 4D flow analysis tool](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4592372/) by adding additional visualization tools, interactive features, improved data saving, which increased the overall usability of this Quantitative Velocity Tool ([QVT](/research/qvt)). The primary aim of this study was to measure resting intracranial blood flow and pulsatility in 13 main cerebral arteries and 4 sinuses in a large normative cohort of 759 older adults. In addition, we investigated the effect of age and sex on intracranial blood flow and pulsatility. 

![](/images/research/Normals_3_qvt.png)

We obtained 4D flow datasets from the [ADRC](https://www.adrc.wisc.edu/) and [WRAP](https://wrap.wisc.edu/) cohorts were obtained between 2010 and 2020. Subjects that showed cognitive impairment and had detectable amyloid burden from PET images were excluded. Furthermore, 4D flow datasets were excluded if there was bad image quality or bad cardiac gating, leaving 759 datasets from 759 cognitively unimpaired subjects. Cycle-averaged volumetric flow rates and pulsatility indices were obtained in 17 major vessel segments: cervical internal carotid arteries (ICA-C1), cavernous ICAs (ICA-C3), vertebral arteries (VA), basilar artery (BA), middle cerebral arteries (MCA), posterior cerebral arteries (PCA), straight sinus (STR), superior sagittal sinus (SSS), and transverse sinuses (TS). Left (L) and right (R) sides were assessed separately for bilateral vessels. Total cerebral blood flow (TCBF) was computed as the sum of flow in the cervical ICAs and BA. Anthony Peret and I split the analysis, 457 and 302 cases each, respectively. Each case took around 5-minutes to complete with our new tool (before this would have taken considerably longer and would have had issues with small vessel segments). Overall, this took us about 1.5 months to complete all cases, with several weeks devoted to data organization and curation.

![](/images/research/Normals_1_violin.png)

Normal blood flow and pulsatility values for all vessel segments were obtained and tabulated for the whole group, by age (every half decade), and by sex. Multiple linear regression showed that there was a clear decrease in TCBF over age and there were no sex differences. Additionally, linear mixed effects models showed vessel-specific decreases in blood flow but showed increases in pulsatility with increasing age. 

![](/images/research/Normals_2_tcbf.png)

This investigation represents one of the largest and most comprehensive studies on intracranial macrovascular hemodynamics in older adults. This was made possible with 4D flow MRI, which provides a non-invasive assessment of cerebral blood flow and pulsatility in reasonable scan times. The 4D flow analysis tool that was developed allowed for efficient and repeatable hemodynamic analysis. Normal blood flow and pulsatility values, as have been reported in this study, show strong correlations with age and are an important first step in defining normative cerebral hemodynamics. These vascular changes may be related to increasing vascular stiffness, age-related atrophy, or decreased brain metabolism. Ultimately, knowledge of normal blood flow and pulsatility ranges will help in determining abnormalities caused by cerebrovascular disease or dementia.

Future studies, led by Anthony Peret, will look to associate vascular risk factors (e.g. ASCVD score, blood pressure, etc) and white matter hyperintensity volumes with intracranial blood flow and pulsatility. We also plan to normalize our flow measures by brain volume (from T1-weighted MPnRAGE scans) to see if the decrease in blood flow over age is driven primarily by atrophy. Lastly, we plan to provide our measured flow/pulsatility values internally to other researchers working on the ADRC/WRAP studies. 

### Collaborations: 
[Alzheimer's Disease Research Center](https://www.adrc.wisc.edu/), [Wisconsin Registry for Alzheimer's Prevention](https://wrap.wisc.edu/), [Wisconsin Alzheimer's Institute](https://wai.wisc.edu/), [Sterling Johnson Lab](https://www.waisman.wisc.edu/staff/johnson-sterling/)

Abstracts
------
### Oral Presentation
* Peret, A., Roberts, G. S., Hoffman, C. A., Rivera-Rivera, L. A., Cody, K. A., Rowley, H. A., Wieben, O., Johnson, S. C., Johnson, K. M., & Eisenmenger, L. B. 4D Flow Magnetic Resonance Imaging for the Study of Normal Cerebrovascular Aging in a Large Cohort of Cognitively Normal Older Adults. American Society of Functional Neuroradiology 15th Annual Meeting. 2022 August 27.
* Roberts, G. S., Peret, A., Rivera-Rivera, L. A., Cody, K. A., Rowley, H. A., Wieben, O., Johnson, S. C., Johnson, K. M., & Eisenmenger, L. B. Defining Normative Cerebral Hemodynamics in Cognitively Healthy Older Adults with 4D Flow MRI. Joint Annual Meeting ISMRM-ESMRMB & SMRT 31st Annual Meeting. 2022 May 7.
[Download](/files/research/Normative Flow and Pulsatility in Aging - ISMRM22 Abstract - FINAL.pdf){: .btn--research} 

Manuscripts
------
### In-Preparation
* Roberts, G. S., Peret, A., Hoffman, C. A., Koscik, R. L., Jonaitis, E. M., Rivera-Rivera, L. A., Cody, K. A., Rowley, H. A., Johnson, S. C., Wieben, O., Johnson, K. M., & Eisenmenger, L. B. Normative Cerebral Blood Flow and Pulsatility in Cognitively Unimpaired Older Adults using 4D Flow MRI. In Press with Radiology. 
* Peret, A., Roberts, G. S., Hoffman, C. A., Koscik, R. L., Jonaitis, E. M., Rivera-Rivera, L. A., Cody, K. A., Rowley, H. A., Johnson, S. C., Wieben, O., Johnson, K. M., & Eisenmenger, L. B. 4D Flow Magnetic Resonance Imaging for the Study of Normal Cerebrovascular Aging in a Large Cohort of Cognitively Normal Older Adults. To submit to JAMA Neurology.
