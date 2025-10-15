---
layout: page
title: "Home"
class: home
---

# Hi, I'm Bohan Zhou

<div class="columns" markdown="1">

<div class="intro" markdown="1">
I'm a visiting assistant professor at the [UCSB](https://math.ucsb.edu) fortunately mentored by [Matt Jacobs](https://web.math.ucsb.edu/~majaco/).

I am an applied mathematician with interests in developing provable and practical methodologies for analyzing data distributions. My research mostly originates from real-world problems, following channels created by optimal transport (OT) theory, it fluxes into scientific computation, calculus of variations, optimization, network theory, fluid dynamics and data science.

I received my Ph.D. at UCDavis advised by [Qinglan Xia](https://www.math.ucdavis.edu/~qlxia/). After that, I was a Byrne Instructor in Applied Mathematics at Dartmouth College, in the group of [Anne Gelb](https://math.dartmouth.edu/~annegelb/) partially funded by the [ONR-MURI](https://math.la.asu.edu/~muri/index.html) program. {% comment %} Earlier, I received my B.S. at Zhejiang University, where I completed my undergraduate thesis under supervision of [Prof. Zhi (George) Lin](http://www.math.zju.edu.cn/linzhi/).{% endcomment %}


Here is my complete [CV]({{site.baseurl}}/BohanZhou-CV.pdf). (*Last Update: Sep, 2025*)


</div>

<div class="me" markdown="1">
<picture>
  <source srcset='{{site.baseurl}}/assets/images/Zhou.jpg' type='image/jpg' />
  <img
    src='{{site.baseurl}}/assets/images/Zhou.jpg'
    alt='Bohan Zhou'>
</picture>

{:.no-list}
* <a href="mailto:{{ site.email }}">{{ site.email }}</a>
* South Hall 6702, UCSB, CA.
</div>

</div>

## Recent <a href="{{ "/publications/" | relative_url }}">Papers</a>
<a href="https://arxiv.org/a/0000-0002-8930-0098.html"><i class="fab fa-scroll" aria-hidden="true"></i> ArXiv</a>
<a href="https://scholar.google.com/citations?user=Fc4gd7oAAAAJ&hl=en&oi=sra"><i class="fab fa-google" aria-hidden="true"></i> Google Scholar</a>

<div class="featured-publications">
  {% assign sorted_publications = site.publications | sort: 'year' | reverse %}
  {% for pub in sorted_publications %}
    {% if pub.highlight %}
      <a href="{{ pub.pdf }}" class="publication">
        <strong>{{ pub.title }}</strong>
        <span class="authors">{% for author in pub.authors %}{{ author }}{% unless forloop.last %}, {% endunless %}{% endfor %}</span>.
        <br>
        <i>{% if pub.status %}({{ pub.status }}){% endif %} {% if pub.venue %}{{ pub.venue }}, {% endif %}{{ pub.year }}</i>.
        {% for award in pub.awards %}<br/><span class="award"><i class="fas fa-{% if award == "Best Paper Award" %}trophy{% else %}award{% endif %}" aria-hidden="true"></i> {{ award }}</span>{% endfor %}
      </a>
    {% endif %}
  {% endfor %}
</div>

<a href="{{ "/publications/" | relative_url }}" class="button">
  <i class="fas fa-chevron-circle-right"></i>
  Show All Papers
</a>
