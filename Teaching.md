---
layout: page
title: Teaching
class: teaching
permalink: /teaching/
---


{:.hidden}

## Current Teaching

Parental leave

## Teaching Practice

## Past Teaching

<section class="teaching-list">
  {% for inst in site.data.courses %}
    <article class="teaching-institution">
      <h3 id="y{{ forloop.index0 }}">{{ inst.location }}</h3>
      <ul>
        {% for course in inst.courses %}
          <li>{{ course.title }}</li>
        {% endfor %}
      </ul>
    </article>
  {% endfor %}
</section>

