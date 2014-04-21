---
layout: default
course: cs360
---

Assignments
===========

### Homework

{% for p in site.pages | sort: 'path' %} {% if p.categories contains "homework" and p.course == page.course %}
* [{{ site.data[p.course][p.hw].title }}]({{ site.baseurl }}{{ p.url }}) {% endif %} {% endfor %}

