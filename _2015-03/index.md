---
index: true
name: "2015-03"
---

Hello world of 2015!

{% assign name = page.name %}
looping through {{ page.name}}
  {% for page in site.[name] %
  {% if page.index == null %}
## [{{ page.title }}]({{ page.url }}) - {{ page.category }}
{{ page.content | markdownify }}
***
  {% else %}
  *PAGE page {{ page.title }} SKIPPED.*
  {% endif %}
  {% endfor %}    
{% endfor %}
