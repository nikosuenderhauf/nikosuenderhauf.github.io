---
layout: page
title: projects
permalink: /projects/
description: A growing collection of your cool projects.

social: true
enable_katex: true

---

Coming soon ...

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
