---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

I am going to post some of my research here in the very near future. But I am still working on figuring out Jekyll.

Projects
-------

<nbsp>

{% include base_path %}

{% assign ordered_pages = site.research | sort:"order_number" %}

{% for post in ordered_pages %}
  {% include archive-single.html type="grid" %}
{% endfor %}

