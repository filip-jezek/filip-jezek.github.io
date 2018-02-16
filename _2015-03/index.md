---
index: true
---

Hello world of 2015!

{% for collection in site.collections %}
{% assign name = collection.label %}
## {{ name }}
    {% for page in site.[name] %}
  [{{ page.title }}]({{ page.url }}) - {{ page.category }}
    {% endfor %}    
{% endfor %}
