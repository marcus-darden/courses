---
---

Prof. Marcus M. Darden
======================

### Contact Info

Office: Mott 112
email: marcus.darden@cs.olivetcollege.edu
Office Hours: {{ site.data.current.officehours }}

### {{ site.data.current.semester }} {{ site.data.current.year }} Courses

{% for p in site.pages %}
{% if p.categories contains 'coursepage' and site.data.current.courses contains p.course %}
* [{{ p.title }}]({{ site.baseurl }}{{ p.url }})
{% endif %}
{% endfor %}

### Other courses

{% for p in site.pages %}
{% if p.categories contains 'coursepage' %}
{% unless site.data.current.courses contains p.course %}
* [{{ p.title }}]({{ site.baseurl }}{{ p.url }})
{% endunless %}
{% endif %}
{% endfor %}

