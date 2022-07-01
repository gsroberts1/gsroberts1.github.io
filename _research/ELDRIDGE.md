---
title: "Preterm Birth Study"
layout: single-portfolio
excerpt: "<img src='/images/research/ELDRIDGE.png' alt=''>"
permalink: /research/eldridge
collection: research
type: "Current Projects"
venue: "University of Wisconsin - Madison"
location: "Madison, WI, USA"
order_number: 13
header: 
  og_image: "research/ELDRIDGE.png"
---

Background
------
### Preterm Birth
Preterm birth has been linked to an elevated risk of heart failure and cardiopulmonary disease later in life. With improved neonatal care and survival, most infants born preterm are now reaching adulthood. In this study, we used 4D flow MRI coupled with an exercise challenge to assess the impact of preterm birth on right heart flow dynamics in otherwise healthy adolescents and young adults who were born preterm.

My primary contribution to this work was the analysis of 4D flow MRI exams from 11 preterm young adults and 17 preterm adolescents before and after exercise (56 total datasets analyzed). These subjects were drawn from the Newborn Lung Project (NLP) cohort at the University of Wisconsin-Madison. Stroke volume, cardiac output, and flow in the main pulmonary artery were quantified with 4D flow MRI. Kinetic energy and vorticity were measured in the right ventricle. All parameters were measured at rest and during exercise at a power corresponding to 70% VO2max for each subject. For exercise imaging, each subject exercised in a supine position in the scanner bore with a commercial MR-compatible recumbent stepper (Cardio Stepper Module). 

We found that stroke volume decreased in preterm born subjects relative to healthy controls. This resulted in reduced capacity to increase cardiac output after exercise for preterms. Additionally, elevated right ventricular vorticity and kinetic energy were observed during diastole, suggesting altered flow dynamics, along with streamline visualizations showing disrupted diastolic filling vortices.

### Gating Characterization
While a large majority of this study was completed by Jacob Macdonald, I also helped develop the cardiac/respiratory gating code for this project (in additiona to the Ensight flow analysis). These gating scripts parsed the acquired peripheral gating signal from the pulse oximeter to visualize beat-to-beat RR intervals over the course of the MRI scan. Additionally, the code also parsed respiratory signal from the respiratory bellows to also display respiratory phase over the scan. Our 4D flow MRI reconstructions rely heavily on the accuracy of the cardiac/respiratory gating and if bad gating signals are being acquired, MRI image quality and flow quantification accuracy decreased. Unsurprisingly, this happened relatively frequently during exercise when the subject was moving in the MRI scanner. In these cases, we would often visualize "missed heartbeats", where the gating signal was not recorded. This effectively increased the average estimated RR interval, which adversely altered flow values. Jacob and I developed a sliding window method to estimate these missed heartbeats and retrospectively correct these gating files, which improved reconstructions. I also developed code in Matlab to assess beat-to-beat variations using Poincare plots. 

![](/images/research/ELDRIDGE_2_missedHB.PNG)
![](/images/research/ELDRIDGE_1_poincare.png)

Since this project, I have further expanded the gating code and is currently being used in our [QVT analysis tool](https://github.com/uwmri/QVT)

![](/images/research/ELDRIDGE_3_gatingTool.PNG)

Abstracts
------
### Poster Presentation
* MacDonald, J. M., Roberts, G. S., & Wieben, O. ECG Characterization and Correction during Exercise Stress Imaging. Joint Annual Meeting ISMRM-ESMRMB; 2018 June 16; Paris, France.

Manuscripts
------
### Accepted
* Macdonald, J. A., Roberts, G. S., Corrado, P. A., Beshish, A. G., Barton, G. P., Goss, K. N., Eldridge, M. W., Francois, C. J., & Wieben, O. (2021). Irregular Right Heart Flow Dynamics in Children and Young Adults Born Preterm. Journal of Cardiovascular Magnetic Resonance, 10.1186/s12968-021-00816-2.
