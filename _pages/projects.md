---
layout: page
title: research
permalink: /projects/
description: past and current research projects.

social: true
enable_katex: true

---


### Robot Learning
<a href="learningtonavigate"><img class="col one" src="/assets/img/projects/robot_learning_showcase.png"/></a>
How can robots best learn to interact with the world, manipulate objects, and navigate in challenging environments, all to execute complex tasks, such as tidying up an apartment or assist humans in their everyday domestic chores? I am interested in developing learning-based approaches are effective and efficient, and scale to complicated long-horizon tasks. We combine modern techniques such as imitation learning, LLMs, Vision-Language Models, and reinforcement learning with classical control and navigation. [Read more …](learningtonavigate)



### Scene Understanding, Semantic SLAM, and Implicit Representations
<a href="sceneunderstanding"><img class="col one" src="/assets/img/projects/scenegraph.png"/></a>
Making a robot understand what it sees is a fascinating goal in my current research.
In the past we developed novel methods for _Semantic_ Mapping and SLAM by combining object detection with simultaneous localisation and mapping (SLAM) techniques, representing the environment as a scene graph.
More recently, we have investigated a fresh take on the problem and represent the environment with NeRFs or Gaussian Splatting. [Read more …](sceneunderstanding)


<!-- Our ongoing research in scene understanding will help to provide answers to a robot’s questions like „What are these objects I can see in front of me?“ (object detection and recognition), „What can I do with these objects?“ (affordance detection), „Am I in an office, a kitchen, or a living room? What can I expect to find here?“ (semantic mapping, holistic scene understanding.

Furthermore, we work towards making semantic perception robust enough to be used on autonomous robots. To achieve this goal, we analyse the key differences between robotic vision and computer vision (where great breakthroughs have happened since 2013 with the advent of convolutional networks), and adapt learning procedures and network architectures accordingly.  -->



### Uncertainty and Realiability of Deep Learning for Robotic Perception
<a href="uncertainty"><img class="col one" src="/assets/img/projects/uncertainty.png"/></a>
In order to fully integrate deep
learning into robotics, it is important that deep learning systems
can reliably estimate the uncertainty in their predictions.
This would allow robots to treat a deep neural network
like any other sensor, and use the established Bayesian
techniques to fuse the network’s predictions
with prior knowledge or other sensor measurements, or to
accumulate information over time.
We focus on Bayesian Deep Learning approaches for the specific use case of object detection on a robot in open-set conditions. [Read more …](uncertainty)



### Robotic Vision Evaluation and Benchmarking
Big benchmark competitions like [ILSVRC](http://www.image-net.org/challenges/LSVRC/) or [COCO](http://cocodataset.org) fuelled much of the progress in computer vision and deep learning over the past years. We aim to recreate this success for robotic vision.

To this end, we develop a set of new benchmark challenges for robotic vision that evaluate probabilistic object detection, scene understanding, uncertainty estimation, continuous learning for domain adaptation, continuous learning to incorporate previuosly unseen classes,
active learning, and active vision.
We combine the variety and complexity of real-world data with the flexibility of synthetic graphics and physics engines.
[Read more …](http://www.roboticvisionchallenge.org)


### Visual Place Recognition in Changing Environments
<a href="placerecognition"><img class="col one" src="/assets/img/projects/placeRec.png"/></a>
An autonomous robot that operates on our campus should be able to recognize different places when it comes back to them after some time. This is important to support reliable navigation and localisation and therefore enable the robot to perform a useful task.

The problem of visual place recognition gets challenging if the visual appearance of these places changed in the meantime. This usually happens due to changes in the lighting conditions (think day vs. night or early morning vs. late afternoon), shadows, different weather conditions, or even different seasons.

<a name="past projects"></a>

We develop algorithms for vision-based place recognition that can deal with these changes in visual appearance. [Read more …](placerecognition)

---

## Past Projects

### The DLR SpaceBot Cup (2013)
<div class="img_row">
<a href="spacebotcup"><img class="col one" src="/assets/img/projects/spacebot/robot.png"/></a>
<a href="spacebotcup"><img class="col two" src="/assets/img/projects/spacebot/alle_Roboter.png"/></a>
</div>
<div class="col three caption">
      (Left) Our two robots, Phobos and Deimos, in the rugged Mars-like terrain after the contest. (Right) The robots of all teams after the competition.
</div>


In 2013, ten teams from German universities and research institutes participated in a national robot competition called SpaceBot Cup, organized by the DLR Space Administration.

The robots had one hour to autonomously explore and map a challenging Mars-like environment, find, transport, and manipulate two objects, and navigate back to the landing site. Localization without GPS in an unstructured environment was a major issue as was mobile manipulation and very restricted communication. We entered the competition with a multi-robot system of two rovers operating on the ground plus a quadrotor UAV simulating an observing orbiting satellite.

We relied on ROS as the software infrastructure. Despite (or because of) faults, communication loss and break- downs, it was a valuable experience with many lessons learned. [Read more …](spacebotcup)



### Switchable Constraints for Robust SLAM (2011 – 2013)
<a href="switchableConstraints"><img class="col one" src="/assets/img/projects/manhattan.png"/></a>
Current state of the art solutions of the SLAM problem are based on efﬁcient sparse optimization techniques and represent the problem as probabilistic constraint graphs. The optimizer, the so called back-end of the system, relies heavily on the topological correctness of the graph structure and is not robust against misplaced constraint edges. Especially edges representing false positive loop closures will lead to the divergence of current solvers.

We propose to augment the original optimization problem by a new set of hidden variables. These switch variables allow the optimizer to estimate the optimal graph topology and the optimal covariance for each potential outlier constraint. Despite the increased number of variables, the sparse structure of the problem is maintained, which allows efficient calculations. [Read more …](switchableConstraints)


### Multipath Mitigation for GNSS-based Vehicle Localization (2012 – 2013)
<a href="gnss"><img class="col one" src="/assets/img/projects/3Sats.png"/></a>
A common challenge for vehicle localization based on global navigation satellite systems (GNSS) is the multipath problem when high buildings block the direct line of sight to one or several satellites. The blocked signals may still reach the receiver on the ground via one or several reflections on building structures or the ground. Since the signal path is longer for the reflected signal, ranging errors occur that can either prolongate the observed pseudorange or, due to correlation effects, shorten it. This leads to severely biased position estimates.

We work on methods for mitigation of such effects and apply approaches of robust estimation using graphical models.  [Read more …](gnss)

### Application of Biologically Inspired Methods for Autonomous Navigation and SLAM (2010)

[<img class="col one pad10" src="/assets/img/projects/poseCellNetwork.png"/>](bioinspired)
Since the 1970’s different types of neurons involved in spacial navigation have been identified in the brains of rats, primates and humans. Several experiments of different researchers show that these cells code the position and orientation of the animal in its environment.
Neurologists and theoretical biologists have been developing models that help to understand the behaviour of animals as well as humans in different situations. These models explain the workings of the different cell assemblies and their connections with other areas in the brain.

We are interested in these developements and want to derive efficient algorithms that help solving navigation tasks and SLAM on autonomous mobile robots. Our goal is explicitly not to mimic the behaviour of the involved biological processes on the level of single neurons or even spike trains. Instead, we want to understand the principles behind these biological processes and project them onto higher levels of abstraction that are suitable for implementation and application on autonomous systems. [Read more …](bioinspired)



### Autonomous Quadrotor UAVs (2007 – 2009)
[<img class="col one pad10" src="/assets/img/projects/pelican.png"/>](UAVs)
In 2007 we started working with quadrotors by using 3 AscTec Hummingbirds shortly after they became available. From the beginning, our research has focused on fully autonomous systems in indoor/GPS-denied environments without external sensors or computation. Since this required additional on-board sensors and computing power we got an AscTec Pelican quadrotor in 2010 because of its higher available payload.

The results of several projects using these MAVs with additional sensors and modifications have been published in a number of papers, e.g. an autonomous landing procedure by using a camera and a self-made optical flow sensor or [one of the first autonomous indoor flights using a Kinect on the Pelican](https://youtu.be/kmMzc2-ray0). This work has been conducted in close collaboration with [Sven Lange](https://www.tu-chemnitz.de/etit/proaut/en/team/svenLange.html) and other colleagues at Chemnitz University of Technology. Check out their project website for up-to-date information. [Read more …](UAVs)

<center><iframe width="560" height="315" src="https://www.youtube.com/embed/kmMzc2-ray0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe></center>


### Stereo Odometry and Visual Odometry (2004 – 2007)
<img class="col one pad10" src="/assets/img/projects/pointMatching.png"/>
Estimating its ego-motion is one of the most important capabilities for an autonomous mobile platform. Without reliable ego-motion estimation no long-term navigation is possible. Besides odometry, inertial sensors, DGPS, laser range finders and so on, vision based algorithms can contribute a lot of information. Stereo odometry is a vision based motion estimation algorithm that estimates the ego-motion of a stereo camera through its environment by evaluating the captured images.

Stereo Odometry was the topic of my first scientific research project. I started working on it during a research internship at [LAAS / CNRS](http://www.laas.fr) in Toulouse, France under the supervision of [Simon Lacroix](https://scholar.google.com.au/citations?user=7cgLDwUAAAAJ&hl=en&oi=ao) and [Kurt Konolige](https://scholar.google.com.au/citations?user=hczHVxEAAAAJ&hl=en).


### RoboKing – Organizing a Nation-Wide Robotics Competition for Students (2004 – 2008)
[<img class="col one pad10" src="/assets/img/projects/roboking/3.jpg"/>](roboking)
RoboKing was an annual robotics challenge for high school students between 12 and 19 years of age. It was organized by a team of students and research associates working at the chair of Automation Technology at Chemnitz University of Technology in Germany.

Our goal was to raise student’s interest in robotics and engineering and computer science in general, and to motivate them to study an engineering subject at university.

I was part of the organizing team during all these years, which was both a great fun and a fantastic experience. [Read more …](roboking)

<!--
**A bit of Text**

Some maths:

$$
\begin{align*}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{align*}
$$

Some Code:


{% highlight python %}
def test(a=1):
  # Example can be run directly in your JavaScript console
  import numpy as np
  for i in range(5):
    a=[x.strip('.') for x in b{i}]
{% endhighlight %}

~~~py
def test(a=1):
  # Example can be run directly in your JavaScript console
  import numpy as np
  for i in range(5):
    a=[x.strip('.') for x in b{i}]

~~~


<div class="img_row">
    <img class="col one" src="/assets/img/12.jpg" alt="" title="example image"/>
    <img class="col one" src="/assets/img/12.jpg" alt="" title="example image"/>
    <img class="col one" src="/assets/img/12.jpg" alt="" title="example image"/>
</div>


<div class="col three caption">
    Caption photos easily. On the left, a road goes through a tunnel. Middle, leaves artistically fall in a hipster photoshoot. Right, in another hipster photoshoot, a lumberjack grasps a handful of pine needles.
</div>
<div class="img_row">
    <img class="col three" src="{{ site.baseurl }}/assets/img/5.jpg" alt="" title="example image"/>
</div>


![image](/assets/img/12.jpg){:width='33%'}
<div class="col three caption">
    This image can also have a caption. It's like magic.
</div>

-->
<!--

{% for project in site.projects %}

{% if project.redirect %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ project.redirect }}" target="_blank">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>
{% else %}

<div class="project ">
    <div class="thumbnail">
        <a href="{{ project.url | prepend: site.baseurl | prepend: site.url }}">
        {% if project.img %}
        <img class="thumbnail" src="{{ project.img | prepend: site.baseurl | prepend: site.url }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}    
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endif %}

{% endfor %} -->
