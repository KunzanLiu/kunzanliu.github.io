---
layout: page
title: Undergrad Research
description: Dimensionality Reduction for RIS-aided Wireless Communications
img: assets/img/project/undergrad/undergrad.png
importance: 1
category: work
related_publications: einstein1956investigations, einstein1950meaning
---

I spent 2.5 wonderful years in Broadband Wireless Communication and Signal Processing Laboratory led by Prof. [Linglong Dai](http://oa.ee.tsinghua.edu.cn/dailinglong/), where I finished my thesis on *Dimensionality Reduction for RIS-aided Wireless Communications*, and I was fortunate to be mentored by [Zijian Zhang](https://zhangzij15.github.io/).

<div class="section" style="margin-top: 20px;">
    <b style="font-size: 24px;">Introduction</b>
    <div class="row">
        <div class="col-md-6">
            Reconfigurable intelligent surface (RIS) is a near-passive antenna array composed of a large number of elements. It can actively reconfigure the wireless channels by properly adjusting the phase-shifts of the incident electromagnetic waves. Benefiting from its characteristics of low cost and power consumption, RIS has been envisioned as a promising technique for future wireless communications. RIS is able to achieve high ar-ray gain that is proportional to the square of the number of RIS elements, which encourages RIS to be designed as large as possible. Although high-dimensional RIS enhances the performance of the system, it also brings about challenges considering size, power consumption, and pilot overhead. Thus, in my undergraduate thesis, we focus on the dimensionality-reduced design and validation of RIS-aided communications, preserving the high array gain of RIS while also addressing challenges in system design.
        </div>

        <div class="col-md-6">
            {% include figure.html path="assets/img/project/undergrad/RIS.png" title="Multiphoton Microscopy" class="img-fluid " style="width: 80px; height: auto;"%}
            <div class="caption" style="text-align: left;">
                <a href="https://www.ni.com/en/innovations/case-studies/23/tsinghua-university-low-power-communications-ris-ai-6g.html">[Source]</a>
            </div>
        </div>
    </div>
</div>



Every project has a beautiful feature showcase page.
It's easy to include images in a flexible 3-column grid format.
Make your photos 1/3, 2/3, or full width.

To give your project a background in the portfolio page, just add the img tag to the front matter like so:

    ---
    layout: page
    title: project
    description: a project with a background image
    img: /assets/img/12.jpg
    ---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal its glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}
```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
```
{% endraw %}
