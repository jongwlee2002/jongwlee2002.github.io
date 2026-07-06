---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
Hello, I am an undergraduate student in Computer Science at Korea University, and I work as an undergraduate intern at the Generative Intelligence Lab. My research interests include geometric deep learning, neural dynamics, and scientific simulation. I have contributed to ICML 2026 papers on neural Koopman dynamics and Euler-Poincare neural dynamics.

## Publications

{% assign featured_publications = site.publications | where: "featured", true | sort: "date" | reverse %}
<div class="publication-list">
  {% for post in featured_publications %}
    {% include publication-item.html publication=post %}
  {% endfor %}
</div>
