---
course: cs140
---

Assignments
===========

### Homework

{% for p in site.pages %}
  {% if p.categories contains "homework" and p.course == page.course %}
* [{{ p.title }}]({{ p.url }})
  {% endif %}
{% endfor %}
