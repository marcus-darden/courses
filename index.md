---
layout: default
title: "Prof. Marcus M. Darden's Coursepages"
---
{% assign pages = site.pages | sort: 'path' %}
## Contact Info

Office: Mott 112  
email: marcus.darden@cs.olivetcollege.edu  
Office Hours: {{ site.data.current.officehours }}  

## {{ site.data.current.semester }} {{ site.data.current.year }} Courses

{% for p in pages %} {% if p.layout == 'coursepage' and site.data.current.courses contains p.course %}
* [{{ site.data.catalog[p.course].title }}]({{ site.baseurl }}{{ p.url }}) {% endif %} {% endfor %}

## Other courses

{% for p in pages %} {% if p.layout == 'coursepage' %} {% unless site.data.current.courses contains p.course %}
* [{{ site.data.catalog[p.course].title }}]({{ site.baseurl }}{{ p.url }}) {% endunless %} {% endif %} {% endfor %}

