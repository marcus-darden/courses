---
layout: default
course: cs140
---

Assignments
===========

{% assign pages = site.pages | sort: 'path' %}

### Homework

{% for p in pages %} {% if p.layout == 'homework' and p.course == page.course %}
* [{{ site.data[p.course][p.assignment].title }}]({{ site.baseurl }}{{ p.url }}) {% endif %} {% endfor %}

