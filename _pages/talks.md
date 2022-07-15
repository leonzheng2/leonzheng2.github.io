---
layout: archive
title: "Talks and presentations"
permalink: /talks/
author_profile: true
---

[//]: # (<p style="text-decoration:underline;"><a href="/talkmap.html">See a map of all the places I've given a talk!</a></p>)

Most slides are made with Powerpoint, but the given links usually give access to pdf versions which are lighter but may contain small glitches or low-quality images. Contact me if you want the .pptx version. You are more than welcome to re-use some illustrations from my slides.

> **Thesis defense**: *Sketching for Large-Scale Learning of Mixture Models* (Oct. 2017) [[Slides]](https://nkeriven.github.io/files/keriven_defense.pdf){:target="_blank"}

{% for post in site.talks reversed %}
  {% include archive-single.html %}
{% endfor %}
