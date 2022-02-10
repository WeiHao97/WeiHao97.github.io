---
layout: archive
title: ""
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}
# <i class="fa fa-fw fa-briefcase "></i> CV

Education
======
* Ph.D in ML Systems, Columbia University, 2025 (expected)
* B.S. in Computer Science and Mathematics, UW-Madison, 2019

Work experience
======
* Summer 2022: Research Internship at MSR, System Group, Redmond
* Summer 2020: Research Internship at Max Planck Institute for Software Systems
* Summer 2018: Research Internship at Citrine Informatics
  
Skills
======
* C++/Python/Cuda/Linux

Publications
======
  <ul>{% for post in site.publications  reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks  reversed %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching  reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
