---
layout: page
title:  Sampling
description: The sampling hypothesis suggests that the brain neither represents nor calculates with probabilities but approximates probabilistic calculations by drawing samples from memory or mental simulation. But what kind of samples does it produce? In this project we aim to uncover what kind of sampling algorithm best describes human inferences?
img: /assets/img/mcmcsamples.png
importance: 1
---


Sampling for inference. But which sampler? Autocorrelation and 1/f 

Group tasks: sampling together?


<!-- Human responses are fundamentally noisy. Usually this noise is assumed to be a random fluctuation independent of the underlying signal, a nuisance variable, that can be removed by averaging results or counterbalancing experimental designs. However, studies investigating the properties of the noise in cognitive psychology have found that it deviates significantly from these assumptions .

First, while continuous responses are usually assumed to be normally distributed, results from free recall studies have found that the distribution of inter-response intervals is often heavy-tailed and can resemble Levy flights. For example, when participants were asked to name animals as they came to mind, most retrieval times were short, but infrequently retrieval times were much longer.

Second, when participants provide repeated estimates of a temporal duration or a magnitude, their responses do not only depend on their previous estimate, as predicted by a random-walk model, but on all previous estimates. These long-range autocorrelations are best described as $1/f$ noise.  -->

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/directsamples.png' | relative_url }}" alt="" title="direct samples"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/mcmcsamples.png' | relative_url }}" alt="" title="mcmc samples"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/mc3samples.png' | relative_url }}" alt="" title="mc3 samples"/>
    </div>
</div>
<div class="caption">
The behavior of three sampling procedures in a patchy environment. <b>Left:</b> Direct sampling does not require a starting position and subsequent samples are drawn independently from the underlying distribution. As a result, successive samples cover the whole distribution. <b>Center: </b> In contrast, MCMC requires a starting state (solid gray point). Successive samples are proposed by performing a random walk, biased towards regions of high probability of the underlying distribution. However, these proposals do not allow the rapid exploration of multiple modes. Instead, the sampler will slowly traverse the space, and in many cases, never explore far-away modes. <b>Right </b> MC3 also rests on a starting state and iteratively explores the underlying distribution. However, since it does so in multiple parallel chains at higher temperatures, it will occasionally jump into far-away modes.</div>

<!-- Every project has a beautiful feature showcase page.
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
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/1.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/3.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/5.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/5.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

You can also put regular text between your rows of images.
Say you wanted to write a little bit about your project before you posted the rest of the images.
You describe how you toiled, sweated, *bled* for your project, and then... you reveal it's glory in the next row of images.


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/6.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/11.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>


The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/" target="_blank">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

```html
<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/6.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/11.jpg' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
``` -->
