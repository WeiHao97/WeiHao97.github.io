---
layout: modern
title: "CV"
permalink: /cv/
description: "Curriculum vitae of Wei Hao — education, experience, awards, and publications."
redirect_from:
  - /resume
---

<header class="hero">
  <div class="wrap page-hd">
    <p class="eyebrow">Curriculum Vitae</p>
    <h1>CV</h1>
    <p>PhD in Computer Science, Columbia University. Research on reliable and secure AI systems.{% if site.author.googlescholar %} See also <a href="{{ site.author.googlescholar }}" target="_blank" rel="noopener">Google Scholar</a>.{% endif %}</p>
  </div>
</header>

<section class="section">
  <div class="wrap">

    <div class="section__head"><div><span class="section__kicker">Education</span></div></div>
    <div class="awards" style="margin-bottom:48px">
      <div class="award"><div class="award__yr tnum">2025</div><div><div class="award__name">Ph.D., Computer Science — Columbia University</div><div class="award__desc">Machine-learning systems. Co-advised by Asaf Cidon and Junfeng Yang.</div></div><div class="award__tag">New York</div></div>
      <div class="award"><div class="award__yr tnum">2019</div><div><div class="award__name">B.S., Computer Science &amp; Applied Mathematics — UW–Madison</div><div class="award__desc">Advised by Shivaram Venkataraman.</div></div><div class="award__tag">Madison</div></div>
    </div>

    <div class="section__head"><div><span class="section__kicker">Experience</span></div></div>
    <div class="awards" style="margin-bottom:48px">
      <div class="award"><div class="award__yr tnum">2024</div><div><div class="award__name">Research Scientist</div><div class="award__desc">AI security in production.</div></div><div class="award__tag">Barracuda Networks</div></div>
      <div class="award"><div class="award__yr tnum">2022-2023</div><div><div class="award__name">Research Scientist</div><div class="award__desc">ML model management system with Deepak Narayanan and Amar Phanishayee.</div></div><div class="award__tag">Microsoft Research (Systems Group)</div></div>
      <div class="award"><div class="award__yr tnum">2020</div><div><div class="award__name">Research Intern</div><div class="award__desc">DNN serving system, with Jonathan Mace.</div></div><div class="award__tag">Max Planck Institute for Software Systems</div></div>
      <div class="award"><div class="award__yr tnum">2018</div><div><div class="award__name">Research Intern</div><div class="award__desc">DNN for defect detection.</div></div><div class="award__tag">Citrine Informatics</div></div>
    </div>

    <div class="section__head"><div><span class="section__kicker">Honors</span></div></div>
    <div class="awards" style="margin-bottom:48px">
      {% for a in site.data.awards %}
      <div class="award">
        <div class="award__yr tnum">{{ a.year }}</div>
        <div><div class="award__name">{% if a.url %}<a href="{{ a.url }}" target="_blank" rel="noopener">{{ a.name }}</a>{% else %}{{ a.name }}{% endif %}</div>{% if a.desc and a.desc != "" %}<div class="award__desc">{{ a.desc }}</div>{% endif %}</div>
        <div class="award__tag">{{ a.tag }}</div>
      </div>
      {% endfor %}
    </div>

    <div class="section__head"><div><span class="section__kicker">Skills</span></div></div>
    <p class="prose" style="margin-bottom:48px"><strong>Languages &amp; tools:</strong> C++, Python, CUDA, Linux.</p>

    <div class="section__head"><div><span class="section__kicker">Publications</span></div><a class="section__more" href="{{ '/publications/' | relative_url }}">All →</a></div>
    <div class="pubs">
      {% assign pubs = site.publications | sort: "date" | reverse %}
      {% for post in pubs %}{% include redesign/pub.html post=post %}{% endfor %}
    </div>

  </div>
</section>
