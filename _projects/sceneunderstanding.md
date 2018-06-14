---
layout: page
title: Scene Understanding and Semantic SLAM
description:
---

The problem of Simultaneous Localization and Mapping (SLAM) describes the process of a robot building a map of its unknown environment, and at the same time using this still incomplete map to determine the robot’s position, and to navigate.

SLAM is not unlike what seafarers in the past had to do when they explored the coast of a new continent for the first time.

Most current SLAM systems are still based on primitive geometric features such as points, lines, or planes. The created maps therefore carry geometric information, but no immediate semantic information. For instance in the image below, we see a map consisting of many individual points.

For us humans it is quite easy to identify individual objects such as monitors or chairs in this point cloud map. We automatically connect meaning (semantics) to the geometric structure we see. For a robot however, interpreting the map in this semantic way is a very hard problem.

A robot that uses this point cloud map – for instance for navigation – can understand that something is in its way, but it does not know what kind of object it is: which of these many points are part of a chair? Which represent a monitor? Which belong to a human office worker?

**Semantic Mapping** enriches the geometric map by semantic information. We can see below how some points in the map got identified as belonging to an object of a certain type. We illustrate this by assigning different colors to different object types, e.g. light blue for monitors and dark blue for keyboards.


**Semantic SLAM** goes one step further. Semantic SLAM uses objects as the central entities in the map (instead of primitives such as points). The objects carry semantic meaning, such as class labels or affordances. This

### Semantic SLAM and Semantic Mapping
{% bibliography -f workshops -q @*[id=nicholson18quadricslam]* %}
{% bibliography -f conferences -q @*[id=Suenderhauf17a]* %}
{% bibliography -f conferences -q @*[id=Suenderhauf16]* %}
{% bibliography -f workshops -q @*[id=Suenderhauf15d]* %}

---

### Bayesian Deep Learning, and Uncertainty in Object Detection
{% bibliography -f conferences -q @*[id=Miller18]* %}
{% bibliography -f workshops -q @*[id=Miller17a]* %}
{% bibliography -f workshops -q @*[id=Dayoub17]* %}

---

### Scene Understanding
{% bibliography -f conferences -q @*[id=Trung18]* %}
{% bibliography -f conferences -q @*[id=Rezazadegan15]* %}
{% bibliography -f workshops -q @*[id=Suenderhauf15b]* %}

---

### Scene Understanding: Hazard Detection
{% bibliography -f journals -q @*[id=McMahon17]* %}
{% bibliography -f conferences -q @*[id=McMahon15b]* %}
