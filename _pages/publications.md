---
layout: page
permalink: /publications/
title: publications
description: I attempt to keep this list up to date. Also check my <a href="https://scholar.google.com/citations?user=WnKjfFEAAAAJ">Google Scholar</a> profile.
years: [2022,2021,2020,2019,2018,2017,2016,2015,2014,2013,2012,2011,2010,2009,2008,2007,2006,2005]
workshops: [2019, 2018, 2017,2015,2014,2013,2012,2005]
journals: [2022,2021, 2020, 2019, 2018, 2017, 2015, 2010]
special_issues: [2020, 2018]
misc: [2012, 2006, 2007]
arxiv: [2022,2021, 2020, 2019, 2018]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>

  {% if page.journals contains y %}
  <strong>Journal Articles</strong>
  {% bibliography -f journals -q @*[year={{y}}]* %}
  {% endif %}

  {% if page.special_issues contains y %}
  <strong>Special Issues</strong>
  {% bibliography -f special_issues -q @*[year={{y}}]* %}
  {% endif %}

  <strong>Conference Publications</strong>
  {% bibliography -f conferences -q @*[year={{y}}]* %}

  {% if page.workshops contains y %}
  <strong>Workshop Publications</strong>
  {% bibliography -f workshops -q @*[year={{y}}]* %}
  {% endif %}

  {% if page.arxiv contains y %}
  <strong>arXiv Preprints</strong>
  {% bibliography -f arxiv -q @*[year={{y}}]* %}
  {% endif %}

  {% if page.misc contains y %}
  <strong>Misc</strong>
  {% bibliography -f misc -q @*[year={{y}}]* %}
  {% endif %}

{% endfor %}
