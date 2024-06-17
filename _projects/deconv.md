---
layout: page
title: Isotropic 3D Microscopy
description: System- and Sample-agnostic Isotropic 3D Microscopy by Weakly Physics-informed, Domain-shift-resistant Axial Deblurring
img: assets/img/project/deconv/deconv.png
importance: 3
category: work
related_publications: han2024system
---

This work is in under review in *Nature Communications*.

## Introduction

Three-dimensional (3D) sub-cellular imaging is highly desirable in biomedical research, as it reveals the intricate spatial organization of organelles, cells, and biological networks. Achieving high-resolution sub-cellular imaging across all three dimensions is crucial for accurately understanding complex biological processes, such as neural circuits, disease pathogenesis, and cellular responses to drugs. However, the fundamental diffraction limit of optical microscopy results in axial resolution that is 2–5 times worse than lateral resolution. This resolution disparity severely hinders isotropic 3D imaging, limiting our ability to faithfully represent the true 3D structure of biological samples and fully realize the potential of 3D imaging in scientific research.

<div class="col-md-12" style="text-align: center;"> 
{% include figure.html path='assets/img/project/deconv/generalizability.png' class="img-fluid z-depth-1 rounded" width="100%"-%}
 </div>
 <div class="caption">
    Fundamental diffraction limit in 3D imaging across diverse systems and samples.
</div>

While recent advances in microscopy theory and instrumentation enable isotropic 3D imaging with certain specialized systems, their reliance on specific hardware, contrast mechanisms, and/or sample preparation limits widespread adoption, particularly for thick, living, and intact biosystems. To make isotropic imaging more accessible across different microscopy modalities, algorithmic approaches seek to address the inverse problem of axial deblurring. In recent years, deconvolution methods based on deep neural networks (DNN), given their effective and flexible learning of data priors, have shown unprecedented performance compared to classical deconvolution methods, such as Richardson-Lucy and fast iterative shrinkage thresholding algorithm (FISTA), on two-dimensional (2D) deconvolution. However, axial resolution restoration is significantly more challenging since acquiring isotropic 3D imaging data as ground truth is impractical for most microscopes, especially in living tissues, making supervised learning methods unsuitable for general isotropic 3D imaging. Despite the existence of a few systems capable of collecting paired isotropic 3D imaging data and generously sharing it, the potential for pre-training a network and generalizing to diverse microscopes and samples is hampered by the significant domain shifts between training and target domains inherent in biomedical imaging.

Domain shift is particularly pronounced in scientific imaging compared to general computer vision, due to the high heterogeneity of microscopy modalities, system properties, sample variation across species and tissues, and the exploratory nature (unseen anomaly detection) of microscopy data. To address these challenges and enable general isotropic 3D imaging, unsupervised generative adversarial network (GAN)-based methods have been proposed to enable deblurring without matched axial image pairs. However, the inherent instability of saddle-point optimization in GAN-based methods leaves them vulnerable to network collapse, potentially generating hallucinations and inconsistencies. Supervised methods leverage similarities between lateral and axial data distributions and employ explicit blurring forward models to achieve high-fidelity isotropic imaging without paired in-distribution data. However, the practical applications of single-stack isotropic recovery using supervised methods are limited for two primary reasons. First, these methods rely on an explicit point-spread function (PSF) model that is assumed to be precisely matched and consistent across the entire imaging volume. In reality, factors such as field curvature, misalignment, and tissue scattering contribute to optical aberrations, resulting in spatially varying PSFs that are sample- and system-dependent, making real-time calibration difficult. This modeling challenge is further exacerbated by noise, especially in low-light conditions. Second, self-supervised methods require assumptions of lateral-axial similarity within single-stack data to learn axial deblurring from synthetic lateral deblurring. While this assumption holds for certain cell and tissue structures (e.g., neurons in the cortex and sinusoids in the liver, as shown in prior axial deblurring works), it breaks down in tissues with high directionality, polarity, or anisotropy, which are common in biological systems such as developing embryos, epithelial glands, and collagen fibers in the extracellular matrix. These challenges are particularly pronounced in label-free imaging of thick heterogeneous tissues, where assumptions about data distribution (e.g. sparsity, label-specific distribution, and lateral-axial similarity) and system priors (e.g. independent and identically distributed (i.i.d.) noise, and linear shift-invariant (LSI) PSFs) are often invalid.


## Principles of SSAI-3D
<div class="col-md-12" style="text-align: center;"> 
{% include figure.html path='assets/img/project/deconv/concept.png' class="img-fluid z-depth-1 rounded" width="100%"-%}
 </div>
 <div class="caption">
    Concept of the weakly physics-informed, domain-shift-resistant axial beblurring for sample- and system-agnostic isotropic 3D (SSAI-3D) microscopy.
</div>

## Mechanism 1: Sparse fine-tuning for robustness in sample domain shift

## Mechanism 2: Self-supervised dataset generation for robustness in system aberrations and noise

## Demo 1: Neuron extraction in mouse brain using light-sheet microscopy

## Demo 2: DNA analysis in mitochondria using confocal microscopy