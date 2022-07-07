---
title: "MR Elastography"
layout: single-portfolio
excerpt: "<img src='/images/research/MRE.png' alt=''>"
permalink: /research/mre
collection: research
type: "Current Projects"
venue: "University of Wisconsin - Madison"
location: "Madison, WI, USA"
order_number: 9
header: 
  og_image: "research/MRE.png"
---

Background
------
MR elastography (MRE) is a special application of MRI that uses motion encoding (very similar to phase contrast MRI) to quantify tissue stiffness in vivo. Tissue stiffness can change throughout the course of a many disease processes, as seen in tumors and liver fibrosis. MR elastography allows for quantitative analysis of mechanical properties of tissues by producing stiffness maps. This is done by sensitizing motion encoding gradients to the motion of shear waves that are introduced into the body by an acoustic driver (essentially a subwoofer). 

![](/images/research/MRE_3_equipment.png)

We acquire multiple images at difference phases of the wave, called phase offsets, to show how the wave propagates in tissue. This phase offset data is used to produce the final stiffness. The images below show the equipment setup for brain MRE and the acquisition of multiple phase offset images. 

![](/images/research/MRE_4_acquisition.PNG)

In terms of actual clinical applications, MRE is primarily used in the liver to study liver disease (e.g. fibrosis and cirrhosis). One of the major benefits of this technique is that it can be used as a non-invasive diagnostic technique, compared to the gold standard biopsy which is invasive and often painful. The field of MRE has been pioneered by the [research group at the Mayo Clinic](https://www.mayo.edu/research/labs/advanced-medical-imaging-technology/overview) and has recently been applied to the brain to study brain tumors, multiple sclerosis, and even dementia. 

![](/images/research/MRE_5_brain.png)
> Murphy, Matthew et al., CC BY-SA 3.0 <https://creativecommons.org/licenses/by-sa/3.0>, via Wikimedia Commons

With the help of GE Healthcare and the Mayo Clinic, we have implemented brain MRE here at UW-Madison due to interest of several research groups. In my second year of graduate school, I helped create an imaging protocol for brain MRE with the intention of applying brain MRE to study structural brain changes (along with vascular changes) in subjects along the Alzheimer's disease continuum within the [ADRC](https://www.adrc.wisc.edu/) and [WRAP](https://wrap.wisc.edu/) cohorts. To do this, we scanned several volunteers, varying the sequence parameters and positioning of the passive driver under the subject's head to find the optimal scan procedure. We found that there was a significant influence of passive driver placement on subsequent stiffness maps.

#### Phantom Development
In order to further test and validate the MRE PSD/reconstruction that was installed on our scanners, I collaborated with David Rutkowski (former student of Alejandro Roldan) to develop an easy-to-manufature phantom consisting of hydrogels with varying consistency encased in hard plastic container. Specifically, there were 5 compartments of varied mechanical stiffness (created by changing the hydrogel polymer:water proportions). Small biopsy samples were taken from within these 5 compartments for ground-truth mechanical strain testing on a tabletop machine. Brain MRE was performed using the established protocol. MRE images reflected a heterogenous stiffness phantom as expected, with the expeceted benefit of high signal due to the high water content of the hydrogel material. Our results showed excellent correlation with ground-truth mechanical strain testing. However, repeating MRE testing one week after fabrication showed drastic stiffness changes compared to initial fabrication. This is likely caused by evaporation decreasing the water content in the hydrogels, increasing stiffness in these hydrogel modules. 

![](/images/research/MRE_2_phantom.png)

#### Compressed Sensing MRE
In addition to the work described above, I applied compressed sensing approaches to investigate the feasibility of accelerating brain MRE as a final project for *MP710: Advances in Medical Magnetic Resonance* taught by Oliver Wieben. The results were very modest, with only accelerations of up to x1.5 being reliably achieved. However, the regularization factors and undersampling factor were not rigorously tested. Here is an excerpt from the technical note:

> MR elastography (MRE) is a medical imaging technique that is particularly useful in quantifying mechanical properties of tissues by producing a stiffness map (elastogram). Recently, MRE has been applied to the brain to assess stiffness changes in various neurological conditions. Subsequently, compressive sensing (CS) is an image processing technique that aims to accurately reconstruct images from undersampled datasets, which can be used to shorten exam times or improve image quality. This paper aims to assess the feasibility of applying CS towards brain MRE exams. One fully-sampled brain MRE was acquired. K-space data was pseudo-randomly undersampled retrospectively and l^1-wavelet regularized reconstruction was performed. CS reconstructed data were further reconstructed to produce MR elastograms. It was shown using various image quality metrics that undersampling of up to 50% produced accurate MR elastograms.

![](/images/research/MP710.PNG)

### Collaborations: 
[Alejandro Roldan CFD Lab](https://uwcvfd.engr.wisc.edu/), [Wally Block Lab](https://www.medphysics.wisc.edu/blog/staff/block-walter-f/), [Corrine Henak Biomechanics Lab](https://henaklab.engr.wisc.edu/)

Manuscripts
------
### Final Report
[Download](/files/research/Technical Note - MRE Grant Roberts.pdf){: .btn--research}

Abstracts
------
### Oral Presentation
* Rivera-Rivera, L. A., Roberts, G. S., Eisenmenger, L. B., Wieben, O., Johnson, S. C., & Johnson, K. M. Association of Brain Biomechanics and Vascular Dynamics using 4D Flow, MRE and DENSE MRI. ISMRM 28th Annual Meeting & Exhibition; 2020 April 18; Sydney, Australia.