---
layout: page
title: Research
class: projects
permalink: /research/
---


{:.hidden}
# Research 

<div class="grid">
  {% for project in site.data.research %}
    {% include project.html project=project %}
  {% endfor %}
</div>
