---
layout: page
title: Scene Understanding, Semantic SLAM, Implicit Representations
description:
---

Making a robot understand what it sees is one of the most fascinating goals in my current research.
To this end, we develop novel methods for _Semantic Mapping_ and [Semantic SLAM](http://www.semanticslam.ai) by combining object detection with simultaneous localisation and mapping (SLAM) techniques. We furthermore work on [Bayesian Deep Learning](uncertainty) for object detection, to better understand the uncertainty of a deep network's predictions and integrate deep learning into robotics in a probabilistic way.

<!-- The problem of Simultaneous Localization and Mapping (SLAM) describes the process of a robot building a map of its unknown environment, and at the same time using this still incomplete map to determine the robot’s position, and to navigate.

SLAM is not unlike what seafarers in the past had to do when they explored the coast of a new continent for the first time.

Most current SLAM systems are still based on primitive geometric features such as points, lines, or planes. The created maps therefore carry geometric information, but no immediate semantic information. For instance in the image below, we see a map consisting of many individual points.

For us humans it is quite easy to identify individual objects such as monitors or chairs in this point cloud map. We automatically connect meaning (semantics) to the geometric structure we see. For a robot however, interpreting the map in this semantic way is a very hard problem.

A robot that uses this point cloud map – for instance for navigation – can understand that something is in its way, but it does not know what kind of object it is: which of these many points are part of a chair? Which represent a monitor? Which belong to a human office worker?

**Semantic Mapping** enriches the geometric map by semantic information. We can see below how some points in the map got identified as belonging to an object of a certain type. We illustrate this by assigning different colors to different object types, e.g. light blue for monitors and dark blue for keyboards.


**Semantic SLAM** goes one step further. Semantic SLAM uses objects as the central entities in the map (instead of primitives such as points). The objects carry semantic meaning, such as class labels or affordances. This -->



### Mapping with Implicit Representations and Neural Radiance Fields

{% bibliography -f conferences -q @*[id=suenderhauf2022nerf]* %}
{% bibliography -f arxiv -q @*[id=abouchakra2022particle]* %}
{% bibliography -f arxiv -q @*[id=abouchakra2022implicit]* %}


### Semantic SLAM and Semantic Mapping
We work on novel approaches to SLAM (Simultaneous Localization and Mapping) that create semantically meaningful maps by combining geometric and semantic information.

We believe such semantically enriched maps will help robots understand our complex world and will ultimately increase the range and sophistication of interactions that robots can have in domestic and industrial deployment scenarios.

<!-- Read more on our dedicated project website [semanticslam.ai](http://www.semanticslam.ai). -->

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/w1-INFCpc20" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</center>

{% bibliography -f arxiv -q @*[id=deitke2022retro]* %}
{% bibliography -f journals -q @*[id=hall2022benchbot]* %}
{% bibliography -f arxiv -q @*[id=hall2020challenge]* %}
{% bibliography -f arxiv -q @*[id=talbot2020benchbot]* %}
{% bibliography -f conferences -q @*[id=bista2021mapping]* %}
{% bibliography -f journals -q @*[id=nicholson18quadricslam]* %}
{% bibliography -f conferences -q @*[id=hosseinzadeh2018structure]* %}
{% bibliography -f arxiv -q @*[id=Jablonsky18geometric]* %}
{% bibliography -f workshops -q @*[id=nicholson18quadricslam]* %}
{% bibliography -f conferences -q @*[id=Suenderhauf17a]* %}
{% bibliography -f conferences -q @*[id=Suenderhauf16]* %}
{% bibliography -f workshops -q @*[id=Suenderhauf15d]* %}

---


### Scene Understanding
{% bibliography -f conferences -q @*[id=Trung18]* %}
{% bibliography -f conferences -q @*[id=Rezazadegan15]* %}
{% bibliography -f workshops -q @*[id=Suenderhauf15b]* %}

---

### Scene Understanding: Hazard Detection
{% bibliography -f journals -q @*[id=McMahon17]* %}
{% bibliography -f conferences -q @*[id=McMahon17a]* %}
{% bibliography -f conferences -q @*[id=McMahon15b]* %}
