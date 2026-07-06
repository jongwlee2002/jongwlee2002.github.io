---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
Hello, I am an undergraduate student in Computer Science at Korea University, and I work as an undergraduate intern at the Generative Intelligence Lab.

## Publications

{% assign featured_publications = site.publications | where: "featured", true | sort: "date" | reverse %}
{% for post in featured_publications %}
  {% include archive-single.html %}
{% endfor %}
