---
layout: page
title: Gait Analysis
description: Modeling how we walk and extracting the representations.
img: assets/img/12.jpg
importance: 1
category: work
related_publications: false
---

<h2>Gait Assessor</h2>
<p>This project showcases my work that I have started in making a robust Gait analysis Model. It features a journal of my experience by diving into the research. Finally a visual showcase to demonstrate the application in detail.</p>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <!--remember to use bib data{%cite source %} -->
    Showing the Gait cycle in key parts. Cited from <a href="www.google.com">source</a>.
</div>
<h3>Prior Research</h3>
<p>Extracting pose maps is easy in this day and age. With all the tool sets available and the contemporary state of machine learning, I was able to prototype a novel edge based bottom-up pose estimator from Google's Mediapipe framework. If your interested check it out here on <a href="www.github.com/google-ai-edge/mediapipe">Github</a>. This gave a real representation of what I have been looking for. Using this prototype I started learning the layers of depth that Gait Analysis requires. I am currently experimenting on a naive Temporal Segmentation Model attempting to predict the ground truth label on Gait characteristics. The datasets I'm using are multi-variant and controlled. As I get further on experimentation I plan to release all my findings and throw a hypothesis for pushing this area of research forward.</p>
<h3>The current Research shows</h3>
<p>This topic still needs more datasets in real world environments. However, the current point in progress of computer vision models shows an increase in reliability of computer vision models using Temporal and Spatial feature map representations. The current state of the art <a href="https://github.com/ShiqiYu/OpenGait">Open Gait Modeling</a> approach has built several backbones to predict in more real world unconstrained environments. They have been able to do this by fusing 2 channels of perception. The first channel being a skeletal map also known as a pose estimator. This is the typical bottom up pose algorithm that represents key points within the skeletal frame of any human object. The current backbone for skeletal mapping is SkeletonGait. The second channel is shown to be a silhouette map which has been primarily used in prior models to extract full body shadows. The backbone for this model is DeepGaitV2. After each representation is extracted these are than fused to extract the average representation of both channels of perception into a multi-modal. </p>
<h3>Sources</h3>
