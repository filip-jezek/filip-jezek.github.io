This is a message to you..

{% assign name = page.name %}
## Modelica association
{% assign cat = "ma" %}

{% for page in site.[name] %}
{% if page.category == cat and page.index != true %}
* [{{ page.title }}]({{ page.path }}) *{{ page.content | slice 0, 20 }} ...*
{% endif %}

{% endif %}
{% endfor %}

## Vendor news
{% assign cat = "vendor" %}

{% for page in site.[name] %}
{% if page.category == cat and page.index != true %}
* [{{ page.title }}]({{ page.path }}) *{{ page.content | slice 0, 20 }} ...*
{% endif %}

{% endif %}
{% endfor %}