---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

## Conference

{% for post in site.conference reversed %}
  {% include archive-single.html %}
{% endfor %}

<!-- ## Journal -->

<!-- {% for post in site.journal reversed %}
  {% include archive-single.html %}
{% endfor %} -->

## Preprint

{% for post in site.preprint reversed %}
  {% include archive-single.html %}
{% endfor %}
