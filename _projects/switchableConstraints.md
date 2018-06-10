---
layout: page
title: Switchable Constraints for Robust SLAM (2011 - 2013)
description:
---


<img class="col two right" src="/assets/img/projects/switchable/frontEndBackEnd.png"/>

Current state of the art solutions of the SLAM problem are based on efﬁcient sparse optimization techniques and represent the problem as probabilistic constraint graphs.

For example in pose graphs the nodes represent poses and the edes between them express spatial information (e.g. obtained from odometry) and information on loop closures. The task of constructing the graph is delegated to a front-end that has access to the available sensor information.

The optimizer, the so called back-end of the system, relies heavily on the topological correctness of the graph structure and is not robust against misplaced constraint edges. Especially edges representing false positive loop closures will lead to the divergence of current solvers.






### Our solution

<img class="col two right" src="/assets/img/projects/switchable/factorGraph_robust.png"/>

We developed a novel problem formulation that allows the back-end to change parts of the topological structure of the graph during the optimization process.

The back-end can thereby discard loop closures and converge towards correct solutions even in the presence of false positive loop closures. This largely increases the overall robustness of the SLAM system and closes a gap between the sensor-driven front-end and the back-end optimizers.

We propose to augment the original optimization problem by a new set of hidden variables. These switch variables allow the optimizer to estimate the optimal graph topology and the optimal covariance for each potential outlier constraint. Despite the increased number of variables, the sparse structure of the problem is maintained, which allows efficient calculations.

### Results


For the evaluation we added false positive loop closures to several standard datasets that are commonly used in the SLAM community. These false positive loop closures were added following different policies to achieve a realistic distribution. Despite a vast number of false loop closure constraints, our proposed robust method is able to converge to a correct solution, discarding all outlier constraints.

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/U6VFweDGn1o" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</center>

<div class="img_row">
<img class="col one" src="/assets/img/projects/switchable/manhattan1.png"/>
<img class="col one" src="/assets/img/projects/switchable/manhattan2.png"/>
<img class="col one" src="/assets/img/projects/switchable/sphere.png"/>
</div>


<img class="col one right" src="/assets/img/projects/switchable/stlucia.png"/>
This works for a large real-world dataset as well. We tested it on the St. Lucia Dataset which covers 66 km of suburban roads. The only sensor information are the images of a webcam mounted on top of a car. The vehicle’s ego-motion and the place recognition were performed using very simple methods (like BRIEF-Gist) on these images. Despite the large number of false positive loop closure detections caused by the simplistic place recognition module, the SLAM system is able to perform well and create a semi-metric map that is almost correct. (Thanks to Michael Milford for providing the dataset.)

### Download the Source Code and Datasets
Vertigo (Versatile Extensions for Robust Inference using Graphical Models) provides a C++ implementation of the switchable constraints approach I developed during my [thesis](http://nbn-resolving.de/urn:nbn:de:bsz:ch1-qucosa-86443). It is an extension library for g2o and gtsam 2.0 and enables g2o or gtsam to solve pose graph SLAM problems in 2D and 3D despite a large number of false positive loop closure constraints. In addition, a remplementation of the max-mixture model described in [(Olson and Agrawal, 2012)](http://roboticsproceedings.org/rss08/p40.html) for g2o and gtsam is also contained.

Furthermore, Vertigo contains a number of standard pose graph SLAM datasets and a script to spoil them with false positive loop closure constraints. These datasets have been used in our evaluations. They can serve as a set of benchmark datasets for future developments in robust pose graph SLAM.

Download: Vertigo is available at [openslam.org](http://openslam.org).

You can use SVN to check it out: svn co https://svn.openslam.org/data/svn/vertigo

### Publications   
Please see the publications below for further details.

   {% bibliography -f conferences -q @*[id=Suenderhauf12e]* %}
   {% bibliography -f conferences -q @*[id=Suenderhauf13a]* %}
   {% bibliography -f conferences -q @*[id=Suenderhauf12]* %}
   {% bibliography -f misc -q @*[id=Suenderhauf12b]* %}

We successfully applied our approach to robust optimization to the problem of [multipath and NLOS mitigation in satellite-based localization](/projects/gnss):
  {% bibliography -f conferences -q @*[id=Suenderhauf13c]* %}
  {% bibliography -f conferences -q @*[id=Suenderhauf12c]* %}
