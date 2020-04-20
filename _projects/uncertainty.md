---
layout: page
title: Bayesian Deep Learning and Uncertainty in Object Detection
description:
---

In order to fully integrate deep
learning into robotics, it is important that deep learning systems
can reliably estimate the uncertainty in their predictions.
This would allow robots to treat a deep neural network
like any other sensor, and use the established Bayesian
techniques to fuse the network’s predictions
with prior knowledge or other sensor measurements, or to
accumulate information over time.

Deep learning systems, e.g. for classification or detection, typically return scores
from their softmax layers that are proportional to the system’s
confidence, but are not calibrated probabilities, and therefore
not useable in a Bayesian sensor fusion framework.

Current approaches towards uncertainty estimation for
deep learning are calibration techniques, or
Bayesian deep learning with approximations such
as Monte Carlo Dropout or ensemble methods.

Our work focusses on Bayesian Deep Learning approaches for the specific use case of object detection on a robot in open-set conditions.

### Publications

{% bibliography -f arxiv -q @*[id=miller2020cac]* %}
{% bibliography -f conferences -q @*[id=hall2018probability]* %}
{% bibliography -f journals -q @*[id=suenderhauf2019probabilistic]* %}
{% bibliography -f arxiv -q @*[id=hall2018probability]* %}
{% bibliography -f workshops -q @*[id=miller2019benchmarking]* %}
{% bibliography -f conferences -q @*[id=Miller19sampling]* %}
{% bibliography -f conferences -q @*[id=rahman2019traffic]* %}
{% bibliography -f conferences -q @*[id=Miller18]* %}
{% bibliography -f workshops -q @*[id=Miller17a]* %}
{% bibliography -f workshops -q @*[id=Dayoub17]* %}
