---
---

Prof. Marcus M. Darden
======================

### Courses

{% for p in site.pages %}
{% if p.categories contains 'coursepage' and site.data.current.courses contains p.course %}
* [{{ p.title }}]({{ site.baseurl }}{{ p.url }})
{% endif %}
{% endfor %}

