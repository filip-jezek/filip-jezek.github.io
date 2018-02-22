This is a message to you..

{% assign name = page.name %}

## Modelica association
{% assign cat = "ma" %}

{% for page in site.[name] %}
{% if page.category == cat and page.index != true %}
* [{{ page.title }}]({{ page.path }})
{% endif %}
{% endfor %}

## Vendor news
{% assign cat = "vendor" %}

{% for page in site.[name] %}
{{ page.title }}, {{ page.category }}...
{% if page.category == cat %}
{% unless page.index %}
* [{{ page.title }}]({{ page.path }})
{% endunless %}
{% endif %}
{% endfor %}
