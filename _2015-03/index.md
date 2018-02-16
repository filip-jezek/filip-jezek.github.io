---
index: true
---

Hello world of 2015!

{% for collection in site.2015-03 %}
{% assign name = collection.label %}
  {% for page in site.[name] %}
  {% if page.index != true %}
## [{{ page.title }}]({{ page.url }}) - {{ page.category }}
{{ page.content | markdownify }}
***
    {% endfor %}    
{% endfor %}
