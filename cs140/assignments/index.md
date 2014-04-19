---
course: cs140
---

Assignments
===========

### Homework

{% for p in site.pages %}
  {% if p.categories contains "homework" and p.course == page.course %}
* [{{ p.title }}]({{ site.url }}{{ p.url }})
  {% endif %}
{% endfor %}

