---
layout: page
title: Robust GNSS-based Vehicle Localization in Urban Environments (2012-2013)
description:
---


A common challenge for vehicle localization based on global navigation satellite systems (GNSS) is the multipath and non-line-of-sight (NLOS) problem.

This problem occurs for instance in urban areas with high buildings: Although the direct line of sight to a satellite is blocked by a building, its signal may still reach the receiver on the ground via one or several reflections on building structures or the ground. Since the signal path is longer for the reflected signal, ranging errors occur that can either prolongate the observed pseudorange or, due to correlation effects, shorten it.

<div class="img_row">
<img class="col one" src="/assets/img/projects/gnss/multipath.png"/>
<img class="col one" src="/assets/img/projects/gnss/nlos.png"/>
<img class="col one" src="/assets/img/projects/gnss/3Sats-outlier.png"/>
</div>
<div class="col three caption">
Multipath and non-line-of-sight effects severely impede the quality of satellite-based localisation in urban environments.
</div>

Multipath effects can also occur when the direct line of sight is free. In this situation, the signal is received directly, but is also reflected on a building or another structure in the vicinity of the receiver. Hence the signal is received multiple times, leading to correlation errors. The observations that are subject to multipath effects can be considered outliers that can severely bias the least squares estimate of the receiver’s position. Even a single multipath measurement can lead to a defective position estimate. The problem gets worse if one considers that in urban environments not only one, but several satellite observations might be affected by multipath effects.


### Our Approach

<img class="right pad20" src="/assets/img/projects/gnss/trajectory.png"/>
Our work transfers the concept of [switchable constraints](/projects/switchableConstraints) from the field of SLAM (Simultaneous Localization and Mapping) in robotics to the domain of GNSS-based localization.

The [switchable constraints](/projects/switchableConstraints) approach is very versatile and can be applied to other least squares problems where outliers have to be expected. Therefore we could successfully transfer the gained insights from SLAM into the domain of GNSS-based localization. Our papers (see below) demonstrate how multipath observations can be identified and rejected during the least squares optimization that solves for the position estimate, without additional a priori knowledge or additional sensor information.

We provide an introduction to factor graphs and how the GNSS-based localization problem can be expressed using such a graph structure. This will help the reader to understand the key idea of the proposed robust optimization scheme. The image on the right presents results acquired from a real-world dataset and compares our proposed solution against a highly accurate ground truth.


### Publications
  {% bibliography -f conferences -q @*[id=Suenderhauf13c]* %}
  {% bibliography -f conferences -q @*[id=Suenderhauf12c]* %}
  {% bibliography -f misc -q @*[id=Suenderhauf12b]* %}
