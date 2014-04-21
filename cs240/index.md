---
layout: default
course: cs240
categories: coursepage
---

{% unless site.data.current.courses contains page.course %}
_Course is currently inactive_
------------------------------
{% endunless %}

{{ site.data.catalog[page.course].title }}
==========================================

### Description

{{ site.data.catalog[page.course].description }}

### Links

* [Syllabus](syllabus.html)
* [Schedule](schedule.html)
* [Assignments](assignments)

