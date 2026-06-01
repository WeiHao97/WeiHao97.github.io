---
layout: modern
title: "Research"
permalink: /publications/
description: "Peer-reviewed publications by Wei Hao across ML systems, AI security, and AI-misuse detection."
---

<header class="hero">
  <div class="wrap page-hd">
    <p class="eyebrow">Publications</p>
    <h1>Research</h1>
    <p>Peer-reviewed work spanning machine-learning systems, AI security &amp; robustness, and the detection of AI misuse.{% if site.author.googlescholar %} Full list on <a href="{{ site.author.googlescholar }}" target="_blank" rel="noopener">Google Scholar</a>.{% endif %}</p>
  </div>
</header>

<section class="section">
  <div class="wrap">
    {% assign pubs = site.publications | sort: "date" | reverse %}
    {% assign years = pubs | group_by_exp: "p", "p.year" %}
    {% for yr in years %}
      <div class="section__head" style="margin-top:8px">
        <div><span class="section__kicker">{{ yr.name }}</span></div>
      </div>
      <div class="pubs" style="margin-bottom:40px">
        {% for post in yr.items %}
          {% include redesign/pub.html post=post %}
        {% endfor %}
      </div>
    {% endfor %}
  </div>
</section>
