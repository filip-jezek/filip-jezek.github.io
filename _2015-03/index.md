---
index: true
name: "2015-03"
layout: default
---

Hello world of 2015!


{% assign name = page.name %}
{% for page in site.[name] %}

{% unless page.index %} 
## [{{ page.title }}]({{ page.url }}) - {{ page.category }}
  {{ page.content | markdownify }}
***
{% endunless %}

{% comment %}
{% if page.index == null %} 
  *PAGE {{ page.title }} null.*
{% endif %}

{% if page.index != true %} 
  *PAGE {{ page.title }} untrue.*
{% endif %}

{% if page.index == "hitparada" %}
  ## [{{ page.title }}]({{ page.url }}) - {{ page.category }}
  {{ page.content | markdownify }}
  ***
  {% endif %}
{% endcomment %}
  {% endfor %}
