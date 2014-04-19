---
---

Courses:

{% for p in site.pages %}
{% if p.categories contains 'coursepage' and site.data.current.courses contains p.course %}
* [{{ p.title }}]({{ site.url }}{{ p.url }})
{% endif %}
{% endfor %}

