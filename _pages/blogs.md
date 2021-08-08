---
title:  "Portfolio"
layout: archive
permalink: /portfolio/
author_profile: true
entries_layout: grid
classes: wide
---

{% for post in site.posts %}
  {% include archive-single.html type="grid"%}
{% endfor %}
