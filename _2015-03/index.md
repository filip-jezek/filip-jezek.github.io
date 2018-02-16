---
index: true
name: "2015-03"
---

Hello world of 2015!


{% assign name = page.name %}
looping through {{ page.name}}
  {% for page in site.[name] %}
  {% if page.index or page.index == null or page.index == false %}
  *PAGE page {{ page.title }} SKIPPED.*

{% else %}
  ## [{{ page.title }}]({{ page.url }}) - {{ page.category }}
  {{ page.content | markdownify }}
  ***
  {% endif %}
  {% endfor %}    
{% endfor %}
