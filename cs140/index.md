---
layout: default
categories: coursepage
---

{% assign path = page.path | split: '/' %}
{% assign courseno = path[0] %}
{% assign course = site.data[courseno] %}

{% unless site.data.current.courses contains courseno %}
_Course is currently inactive_
------------------------------
{% endunless %}

{{ course.title }}
==================

### Description

{{ course.description }}

### Links

* [Syllabus](syllabus.html)
* [Schedule](schedule.html)
* [Assignments](assignments)

