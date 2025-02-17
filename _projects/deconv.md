---
layout: page
title: Isotropic 3D Microscopy
description: System- and Sample-agnostic Isotropic 3D Microscopy by Weakly Physics-informed, Domain-shift-resistant Axial Deblurring
img: assets/img/project/deconv/deconv.png
importance: 2
category: work
related_publications: han2024system
---

## Overview

<div class="col-md-12" style="text-align: center;"> 
{% include figure.html path='assets/img/project/deconv/overview.png' class="img-fluid z-depth-1 rounded" width="100%"-%}
 </div>
 <div class="caption">
    Axial deblurring with SSAI-3D
</div>

Three-dimensional subcellular imaging is essential for biomedical research, but the diffraction limit of optical microscopy compromises axial resolution, hindering accurate three-dimensional structural analysis. This challenge is particularly pronounced in label-free imaging of thick, heterogeneous tissues, where assumptions about data distribution (e.g. sparsity, label-specific distribution, and lateral-axial similarity) and system priors (e.g. independent and identically distributed noise and linear shift-invariant point-spread functions are often invalid). Here, we introduce SSAI-3D, a weakly physics-informed, domain-shift-resistant framework for robust isotropic three-dimensional imaging. SSAI-3D enables robust axial deblurring by generating a diverse, noise-resilient, sample-informed training dataset and sparsely fine-tuning a large pre-trained blind deblurring network. SSAI-3D is applied to label-free nonlinear imaging of living organoids, freshly excised human endometrium tissue, and mouse whisker pads, and further validated in publicly available ground-truth-paired experimental datasets of three-dimensional heterogeneous biological tissues with unknown blurring and noise across different microscopy systems.

<div class="col-md-12" style="text-align: center;"> 
{% include figure.html path='assets/img/project/deconv/NCHighlight.png' class="img-fluid z-depth-1 rounded" width="100%"-%}
 </div>
 <div class="caption">
    The research was selected in <a ref="https://www.nature.com/collections/idhhgedgig">Nature Communications Editors' Highlights</a>.
</div>

## Highlights

- **Imaging:** SSAI-3D as an axial deblurring methodology that is generalizable to diverse 3D imaging systems and 3D biological samples.
- **AI:** A sparse fine-tuning methodology capable of leveraging features learned from large pre-trained models and customizing them to small domain-specific datasets.
- **Biology:** Facilitates downstream biological analysis validated with publicly available ground-truth-paired experimental datasets with unknown system and sample properties.


## Results

### Mechanisms of sparse fine-tuning

<div class="col-md-12" style="text-align: center;"> 
{% include figure.html path='assets/img/project/deconv/sparse.png' class="img-fluid z-depth-1 rounded" width="100%"-%}
 </div>
 <div class="caption">
    Sparse fine-tuning leverages features learned from large pre-trained models and efficiently customizes them to out-of-distribution datasets.
</div>

### Generalizability across real-life imaging

<div class="col-md-12" style="text-align: center;"> 
{% include figure.html path='assets/img/project/deconv/generalizability.png' class="img-fluid z-depth-1 rounded" width="100%"-%}
 </div>
 <div class="caption">
    Generalizability across different systems and samples.
</div>

### Validation with hardware-corrected isotropic imaging

<div class="col-md-12" style="text-align: center;"> 
{% include figure.html path='assets/img/project/deconv/demo1.png' class="img-fluid z-depth-1 rounded" width="100%"-%}
 </div>
 <div class="caption">
    Comparison of software-corrected (SSAI-3D) and hardware-corrected (mesoSPIM) axial image of mouse brain from light-sheet microscopy.
</div>

<div class="col-md-12" style="text-align: center;"> 
{% include figure.html path='assets/img/project/deconv/demo2.png' class="img-fluid z-depth-1 rounded" width="100%"-%}
 </div>
 <div class="caption">
    Comparison of software-corrected (SSAI-3D) and hardware-corrected (multiview confocal) axial image of mitochondria from confocal microscopy. 
</div>