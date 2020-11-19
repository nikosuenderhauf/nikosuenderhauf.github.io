---
layout: page
title: Visual Place Recognition in Changing Environments
description:
---


The picture below illustrates the idea of place recognition: An autonomous robot that operates in an environment (for example our university campus) should be able to recognize different places when it comes back to them after some time. This is important to support reliable navigation, mapping, and localisation. Robust place recognition is therefore a crucial capability for an autonomous robot.

<div class="img_row">
<img class="col half" src="/assets/img/projects/placeRecognition.png"/>
<img class="col half" src="/assets/img/projects/placeRecChallenges.png"/>
</div>



The problem of visual place recognition gets challenging if the visual appearance of these places changed in the meantime. This usually happens due to changes in the lighting conditions (think day vs. night or early morning vs. late afternoon), shadows, different weather conditions, or even different seasons.
We develop algorithms for vision-based place recognition that can deal with these changes in visual appearance.


A general overview of the topic can be found in our survey paper:
{% bibliography -f journals -q @*[id=Lowry15]* %}




### Convolutional Networks for Place Recognition under Challenging Conditions (ongoing since 2014)
In two papers published at RSS and IROS 2015 we explored how Convolutional Networks can be utilized for robust visual place recognition. We found that the features from middle layers of these networks are robust against appearance changes and can be used as change-robust landmark descriptors. Since then, Sourav Garg has pushed the topic forward with publications at ICRA and RSS 2018.



#### Publications
 {% bibliography -f journals -q @*[id=ming2021probabilistic]* %}
 {% bibliography -f journals -q @*[id=garg2019semantic]* %}
 {% bibliography -f conferences -q @*[id=garg2019look]* %}
 {% bibliography -f conferences -q @*[id=garg2018lost]* %}
 {% bibliography -f conferences -q @*[id=Garg18]* %}
 {% bibliography -f conferences -q @*[id=Suenderhauf15a]* %}
 {% bibliography -f conferences -q @*[id=Suenderhauf15]* %}

### Predicting Appearance Changes (2013 – 2015)
![](/assets/img/projects/changePrediction.png){: .col .half}
In earlier work, conducted at TU Chemnitz with colleagues Peer Neubert and Peter Protzel, we explored the possibilities of predicting the visual changes in appearance between different seasons.

This is a more active approach to robust place recognition, since it aims at reaching robustness not by becoming invariant to changes, but rather  learn them from experience, and use the learned model to predict how a place would appear under different conditions (e.g. in winter or in summer).

Coming from the pre-deep learning era, our results look rather coarse. A number of groups have applied generative adverserial networks (GANs) to this problem and achieved far more superior results.


#### Publications

 {% bibliography -f journals -q @*[id=neubert2015superpixel]* %}
 {% bibliography -f conferences -q @*[id=Neubert13b]* %}
 {% bibliography -f workshops -q @*[id=Suenderhauf13b ]* %}
 {% bibliography -f workshops -q @*[id=Suenderhauf13d ]* %}


### BRIEF-Gist (2011)
 {% bibliography -f conferences -q @*[id=Suenderhauf11]* %}
