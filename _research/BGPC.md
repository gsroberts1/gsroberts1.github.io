---
title: "Background Phase Correction"
layout: single-portfolio
excerpt: "<img src='/images/research/BGPC.png' alt=''>"
permalink: /research/bgpc
collection: research
type: "Current Projects"
venue: "University of Wisconsin - Madison"
location: "Madison, WI, USA"
order_number: 7
header: 
  og_image: "research/BGPC.png"
---

Background
------
Back in 2019, we were in the midst of developing and improving [cranial 4D flow analysis tool](/research/qvt). Ultimately, we were hoping to remove as much manual interaction as possible, making the tool completely automated aside from selecting vessels of interesting. At the time, we still had manual step of performing background phase correction (BGPC) immediately after loading in our data. This step is necessary to correct spatial velocity drifts that occur in our images due to eddy currents generated from bipolar gradients, gradient non-linearities, and concomitant magnetic fields. 

![](/images/research/BGPC_1_manual.gif)

To perform this, the user was required to manually delineate background tissue and vessels by adjusting several thresholding parameters. This created a map of velocities within background tissue only (excluding signal from vessel). An N-order polynomial (typically 3rd or 4th order) was then automatically fit to this 3D velocity map and velocities were subtracted from these regression fit to "level out" velocity drift over space. While it did not take much time to perform (maybe 3 minutes), it was still required manual intervention which stopped the mostly automated pipeline.

![](/images/research/BGPC_2_correction.png)

To address this, I applied an automated BGPC that was done during image reconstruction. This automatically estimated the parameters required to delineate background tissue and vessel. In this study, I wanted to evaluate if automatic BGPC completed during reconstruction is sufficient in reducing phase offsets. If the BGPC could be fully-automated, our 4D flow analysis tools could remove this manual which would save post-processing time and increase repeatability between users. Ten healthy 4D flow brain scans were acquired to evaluate the degree of BP errors after: 1) no BPC 2) manual BPC 3) automatic BPC 4) both automatic and manual BPC, which is used in our current pipeline. Effectiveness of each method was evaulated with mean absolute error of the velocity fields. We found that automatic BGPC is sufficient and actually outperformed manual BGPC. It was observed that background tissue was sometimes overestimated manually which lead to signal from vessels being included in the background tissue fitting processing. In summary, we now use automatic BGPC in our image reconstructions which eliminated the need for manual BGPC in our tool, making our tool completely automated aside from vessel selection.

![](/images/research/BGPC_3_results.png)

Abstracts
------
### Oral Presentation
* (Powerpitch) Roberts, G. S., Johnson, K. M., Hoffman, C. A., Eisenmenger, L. B., & Wieben, O. Automating Background Phase Correction in Cranial 4D Flow MRI. Society for Magnetic Resonance Angiography (SMRA) 31st Annual International Conference; 2019 August 27; Nantes, France. 
[Download](/files/research/Automating Background Phase Correction in Cranial 4D Flow MRI - FINAL.pdf){: .btn--research} 
