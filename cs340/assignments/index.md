---
layout: default
course: cs340
---

Assignments
===========

{% assign pages = site.pages | sort: 'path' %}

### Homework

{% for p in pages %} {% if p.categories contains "homework" and p.course == page.course %}
* [{{ p.title }}]({{ site.baseurl }}{{ p.url }}) {% endif %} {% endfor %}

