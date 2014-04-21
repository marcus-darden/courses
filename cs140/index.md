---
layout: default
course: cs140
categories: coursepage
---

{% assign course = site.data[page.course] %}

{% unless site.data.current.courses contains page.course %}
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

