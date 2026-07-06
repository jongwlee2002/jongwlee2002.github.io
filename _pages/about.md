---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
Hello, I am an undergraduate student in Computer Science at Korea University, and I work as an undergraduate intern at the Generative Intelligence Lab. My primary research interest is AI for Science, with a focus on geometric deep learning, neural dynamics, and scientific simulation.

## Publications

{% assign featured_publications = site.publications | where: "featured", true | sort: "date" | reverse %}
<div class="publication-list">
  {% for post in featured_publications %}
    {% include publication-item.html publication=post %}
  {% endfor %}
</div>
