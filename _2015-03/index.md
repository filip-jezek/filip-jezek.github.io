---
index: true
name: "2015-03"
---

Hello world of 2015!


{% assign name = page.name %}
looping through {{ page.name}}
{% for page in site.[name] %}
{% if page.index %} 
  *PAGE {{ page.title }} index exists.*
{% endif %}

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
  {% endfor %}
