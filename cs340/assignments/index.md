---
layout: default
course: cs340
---

Assignments
===========

{% assign pages = site.pages | sort: 'path' %}

### Homework

{% for p in pages %} {% if p.categories contains "homework" and p.course == page.course %}
* [{{ site.data[p.course][p.hw].title }}]({{ site.baseurl }}{{ p.url }}) {% endif %} {% endfor %}

