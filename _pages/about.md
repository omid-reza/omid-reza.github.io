---
layout: archive
permalink: /
title: "Omid Reza Heidari"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Omid Reza Heidari is pursuing his master's studies in computer science at [Concordia University](https://www.concordia.ca/), advised by Professor [Yang Wang](https://users.encs.concordia.ca/~wayang/). Prior to that, he concluded his undergraduate studies at Islamic Azad University. His area of interest includes Computer Vision, Multimodal Vision-Language, etrieval Augmented Generatio, Multimodal AI Agents, and Natural language processing. Recently, he has been working on building a multimodal models.

News
====
{% include base_path %}
{% capture written_year %}'None'{% endcapture %}
{% for post in site.posts %}
  {% capture year %}{{ post.date | date: '%Y' }}{% endcapture %}
  {% if year != written_year %}
    {% capture written_year %}{{ year }}{% endcapture %}
  {% endif %}
  {% include post.html %}
{% endfor %}