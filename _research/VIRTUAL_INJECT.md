---
title: "Virtual Injection"
layout: single-portfolio
excerpt: "<img src='/images/research/VIRTUAL_INJECT.png' alt=''>"
permalink: /research/inject
collection: research
type: "Current Projects"
venue: "University of Wisconsin - Madison"
location: "Madison, WI, USA"
order_number: 5
header: 
  og_image: "research/VIRTUAL_INJECT.png"
---

Background
------
Streamlines are a particularly useful tool for visualizing 3D velocity fields, such as those generated from 4D flow MRI. In fact, it is quite difficult to fully visualize 3D velocity fields in a 3D dimensional volume over multiple cardiac phases on a voxel-by-voxel basis. Streamlines (and pathlines) simulate the path of a massless particle traveling through a velocity field, much like the smoke trails that are seen when testing car aerodynamics in wind tunnels. In the same way, streamlines can demonstrate complex flow patterns within vessels in the brain. In previous studies, streamlines have been used for studying intracarotid plaques and for characterizing cerebrovascular malformations. However, there are artifacts inherent to phase contrast imaging that degrade the quality of velocity fields, specifically, displacement artifacts (deterministic) and velocity noise (stochastic). These velocity-related artifacts can generate non-realistic streamline trajectories and can cause streamlines to prematurely exit the vessel wall and ultimately terminate. The purpose of this study was to try and improve 4D flow streamlines by integrating several correction methods and constraints to improve selective blood flow tracking and emulate “virtual injections”. Specifically, using iterative displacement correction (as originally described by [Thunberg et al](https://pubmed.ncbi.nlm.nih.gov/12412037/)), probabilistic streamlines ([Friman et al](https://pubmed.ncbi.nlm.nih.gov/20879427/)), and incorporating soft boundary and fluid constraints to encourage streamlines to stay within vessel walls.

![](/images/research/VI_1_injectMovie.gif)

This project originally started with Mike Loecher (one of Oliver Wieben's former students) back in 2014. He put in a significant amount of effort towards the virtual injection project as a whole, including conception of the original idea, contributing a significant amount of code for displacement and stochastic corrections, and implementation in several clinical/volunteer cases. This work was presented at several conferences and was included in his thesis but was never written as a dedicated paper. 

When my advisor Dr. Laura Eisenmenger joined UW-Madison in 2018 as a neuroradiologist, she was very interested in revitalizing this project for the purpose of performing "venous tracking". Transvenous embolization is a surgical method commonly used to treat vein of Galen malformations and dural arteriovenous fistulas. However, transvenous embolization is gaining a considerable amount of interest in treating arteriovenous malformations (and was the subject of many presentations given at the [World AVM conference](https://avm2022.org) in 2022). As part of this renewed interest in virtual injections, I took the initiative to revitalize and improve the existing code written by Mike (which by all means, was already well-written), add an in silico flow phantom study, apply this technique in 10 volunteers to measure the improvements that our corrections provided, and implement virtual injections in several clinical cases: arteriovenous malformation, dural arteriovenous malformation, and intracranial aneurysm.

![](/images/research/VI_3_gui.png)
> Our current (somewhat primitive) graphical user interface for emulating virtual injections.

The results from this study showed that iterative displacement corrections significantly improve streamline length. Secondly, the use of probabilistic streamlines (essentially Monte Carlo simulations) allowed for better "filling" of the vasculature when creating many streamlines. Stricly speaking, this is not "correcting" for stochastic noise but is instead showing the *distribution* of possible streamline trajectories. Lastly, the boundary constraint encouraged streamlines to stay within the vessel wall (as defined by the complex difference angiogram) and the fluid constraint prevented sudden trajectory changes with each step. By integrating these corrections, we observed significant improvements in streamline quality and length.

![](/images/research/VI_2_corrections.png)

Importantly, there is a great deal of flexibility generating "virtual injections" using 4D flow MRI:
1. After obtaining a 4D flow MRI dataset, virtual injections can be retrospectively generated at any vessel location within the 3D imaging volume. Because arterial injection imaging methods are often prone to mixing of non-opacified blood, this is particularly beneficial for assessing venous structures.
2. Virtual injections can be generated at multiple seed locations, with each location assigned a different color. Blood flow mixing can then be visually assessed by looking at the mixing of various colors.   
3. In addition to forward propogating streamlines, reverse streamlines can be created by inverting the velocity field. This was particularly useful for identifying feeding arteries in an AVM and for assessing filling rates of draining veins. 
4. 4D flow MRI can provide additional quantitative hemodynamic measures, such as volumetric flow rate, arterial pulsatility, intravascular pressure, wall shear stress, among others. These metrics, which have been validated and tested in various intracranial pathologies, can further assist in comprehensive hemodynamic assessments. 
5. 4D flow MRI is non-invasive and does not require injection of an actual contrast agent.
6. Image acceleration techniques can allow 4D flow scans to be performed in short scan times (e.g., 6-minute PCVIPR sequence used in this study). 

![](/images/research/VIRTUAL_INJECT.png)

Alma Spahic (currently advised by Laura Eisenmenger and Oliver Wiebe) will improve the functionality of our graphical user interface, making it easier for clinicians to implement this tool to study intracranial flow. 

Code
------
[Virtual Injection (Python)](github.com/gsroberts1/Virtual-Injection)

Abstracts
------
### Oral Presentation
* Eisenmenger, L. B., Roberts, G. S., Loecher, M. W., Rivera-Rivera, L. A., Turski, P. A., Johnson, K. M., & Wieben, O. Venous Mapping of Vascular Malformations using Cranial 4D Flow MRI with Improved ‘Virtual Injections’. 2020 ISMRM & SMRT Virtual Conference & Exhibition; 2020 August 08.

### Poster Presentation
* Roberts, G. S., Loecher, M. W., Rivera-Rivera, L. A., Turski, P. A., Johnson, K. M., Wieben, O., & Eisenmenger, L. B. Venous Mapping of Vascular Malformations using Cranial 4D Flow MRI. ASNR 58th Annual Meeting of the American Society of Neuroradiology; 2020 May 30; Las Vegas, NV, USA.
* Eisenmenger, L. B., Roberts, G. S., Loecher, M. W., Rivera-Rivera, L. A., Turski, P. A., Johnson, K. M., & Wieben, O. 4D flow MRI Characterization of High-Risk Dural Arteriovenous Fistula Features. ASNR 58th Annual Meeting of the American Society of Neuroradiology; 2020 May 30; Las Vegas, NV, USA.

Manuscripts
------
### Accepted
* Roberts, G. S., Loecher, M. W., Johnson, K. M., Spahic, A., Turski, P. A., Eisenmenger, L. B., & Wieben, O. (2022). Virtual Injections Using 4D Flow MRI with Displacement Corrections and Constrained Probabilistic Streamlines. Magnetic Resonance in Medicine. 10.1002/mrm.29134

Awards
------
* 2020 - ASNR Certificate of Merit; Venous Mapping of Vascular Malformations using Cranial 4D Flow MRI; ASNR 2020; Educational Exhibit.
* 2022 - [MRM Cover Image](https://onlinelibrary.wiley.com/doi/epdf/10.1002/mrm.29203)