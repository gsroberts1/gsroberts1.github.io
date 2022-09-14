---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

Most of my work centralizes around developing post-processing tools to strategies to assess vascular function. The overall goal of my research is to understand the overall impact of vascular aging and vessel stiffness on cerebrovascular hemodynamics and associated structural brain changes.

Projects
-------

<nbsp>

{% include base_path %}

{% assign ordered_pages = site.research | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include archive-single.html type="grid" %}
{% endfor %}

