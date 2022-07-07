---
title: "Automating Background Phase Correction in Cranial 4D Flow MRI"
collection: talks
type: "Conference Power Pitch"
permalink: /talks/2019-08-27-power-pitch-1
venue: "SMRA 31st Annual International Conference"
date: 2019-08-27
location: "Nantes, France"
---
### Description
My first in-person presentation was a powerpitch at SMRA in 2019. Powerpitches are typically short (~3 minute) elevator pitches designed to quickly grab the interest of the audience. For this work, I discuss the findings from our study on the effects of [automating background phase correction](https://gsroberts1.github.io/research/bgpc) in our reconstruction pipeline. When we were initially developing our [cranial 4D flow analysis tool](https://gsroberts1.github.io/research/qvt), we were constantly looking for ways to decrease manual interaction and the time needed to load 4D flow data for post-processing. One of the manual steps in our processing pipeline was background phase correction, which corrects eddy-current phase errors created by the flow-encoding gradients. In this presentation, I showed that an automatic phase correction implementation in the reconstruction actually outperforms manual background phase correction. This justified the use of skipping the manual correction step if background phase correction was done in the reconstruction, streamlining our tool. 

### Length
3 minutes

### Download
You can download a PDF version of the presentation slides [here](/files/bgpc_smra.pdf).


