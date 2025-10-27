---
layout: page
title: Research
class: projects
permalink: /publications/
---

<!-- {:.hidden}
# Projects -->

<!-- {:.lead}
Here are some projects I have worked on for school, work, or fun. You can find the code for most of them on [GitHub](https://github.com/domoritz). -->

<div class="grid">
  {% for project in site.research%}
    {% include project.html project=project %}
  {% endfor %}
</div>