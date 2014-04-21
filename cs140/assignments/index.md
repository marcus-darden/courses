---
layout: default
course: cs140
---

Assignments
===========

### Homework

{% for p in site.pages %}
  {% if p.categories contains "homework" and p.course == page.course %}
* [{{ site.data[p.course][p.hw].title }}]({{ site.baseurl }}{{ p.url }})
  {% endif %}
{% endfor %}

