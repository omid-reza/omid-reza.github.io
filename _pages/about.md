---
layout: archive
permalink: /
title: "Omid Reza Heidari"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Omid Reza is a PhD student at Concordia University supervised by [Yassine Yaakoubi](https://yaakoubi.github.io/). He recieved his M.Sc. from [Concordia University](https://www.concordia.ca/), under the supervision of Professor [Yang Wang](https://users.encs.concordia.ca/~wayang/) and Professor [Xinxin Zuo](https://sites.google.com/site/xinxinzuohome/). He, prior to that, concluded his undergraduate studies at Islamic Azad University. His area of interest includes Multimodal Vision-Language, Large Language Models, LLM Agents, and Reinforcement Learning.

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
