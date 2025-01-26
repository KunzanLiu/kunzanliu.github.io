---
layout: page
title: Undergrad Research
description: Dimensionality reduction for RIS-aided wireless communications
img: assets/img/project/undergrad/undergrad.png
importance: 5
category: work
related_publications: liu2022compact,liu2022active,zhu2023sensing
---

I spent 2.5 wonderful years in Broadband Wireless Communication and Signal Processing Laboratory led by Prof. [Linglong Dai](http://oa.ee.tsinghua.edu.cn/dailinglong/), where I finished my thesis on *Dimensionality Reduction for RIS-aided Wireless Communications*, and I was fortunate to be mentored by [Zijian Zhang](https://zhangzij15.github.io/) and to work with my friend [Yuhao Chen](https://hericenes.github.io/yuhaochen.github.io/).

## Introduction
Reconfigurable intelligent surface (RIS) is a near-passive antenna array composed of a large number of elements. It can actively reconfigure the wireless channels by properly adjusting the phase-shifts of the incident electromagnetic waves. Benefiting from its characteristics of low cost and power consumption, RIS has been envisioned as a promising technique for future wireless communications. RIS is able to achieve high array gain that is proportional to the square of the number of RIS elements, which encourages RIS to be designed as large as possible. Although high-dimensional RIS enhances the performance of the system, it also brings about challenges considering size, power consumption, and pilot overhead. Thus, in my undergraduate thesis, we focus on the dimensionality-reduced design and validation of RIS-aided communications, preserving the high array gain of RIS while also addressing challenges in system design.

<div class="col-md-12" style="text-align: center;"> 
{% include figure.html path='assets/img/project/undergrad/RIS.png' class="img-fluid z-depth-1 rounded" width="50%"-%}
 </div>
 <div class="caption">
    An RIS prototype with 2304 reflection units. <a ref="https://www.ni.com/en/innovations/case-studies/23/tsinghua-university-low-power-communications-ris-ai-6g.html">[Source]</a>
</div>

## Challenge 1: mismatch in size

To tackle the problem of mismatch in size for high-dimensional RIS-aided
system, we propose the concept of user-side RIS (US-RIS) that includes a multi-layer
structure to save the space. We reveal the phenomenon that multi-layer RIS is able to
adjust the magnitude of the signal, based on which we develop a phase-magnitude precoding design to maximize the achievable SNR. Simulation results
verify the superiority of our proposed US-RIS that can enhance the uplink transmission
of the user.

## Challenge 2: high power consumption

To tackle the problem of high power consumption for high-dimensional
RIS-aided system, we propose the concept of sub-connected active RIS, where
multiple RIS elements share a same power amplifier to reduce the number of PAs
for lower power consumption. We theoretically analyze the benefit of the sub-connected active
RIS, and develop a hybrid precoding design to maximize the energy efficiency of
the system. Simulation results verify that our proposed sub-connected active RIS as well as the
precoding design can achieve higher EE in RIS-aided system.

## Challenge 3: large number of pilot overhead

To tackle the problem of large number of pilot overhead for high-dimensional RIS-aided system, we propose the concept of sensing RIS, where a power
detector is additionally integrated in each RIS element for detecting the magnitude of the
signal. We conceive a signaling method to induce a interference random field (IRF), and
propose a corresponding channel state information (CSI) acquisition method. Simulation
results verify that our proposed solution can achieve dimension-independent CSI acquisition in RIS-aided system, which substantially reduces the pilot overhead. We further
set up a hardware validation experiment that preliminarily demonstrates the practicability of our proposed solution.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project/undergrad/3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project/undergrad/1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/project/undergrad/2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Left: US-RIS. Middle: sub-connected active RIS. Right: sensing RIS.
</div>

This thesis was recognized as *Excellent Bachelor Dissertation of Beijing* and *Excellent Bachelor Dissertation of Tsinghua University* in 2022.