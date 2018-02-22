This is a message to you..  
V1.0

{% assign name = page.name %}

## Modelica association
{% assign cat = "association" %}

{% for page in site.[name] %}
{% if page.category == cat and page.index != true %}
* [{{ page.title }}]({{ page.path }})
{% endif %}
{% endfor %}

## Vendor news
{% assign cat = "vendor" %}
Hey, {{ cat }}!

{% for page in site.[name] %}

{{ page.title }}, {{ page.category }}...

{% if page.category == cat and page.index != true %}
[{{ page.title }}]({{ page.path }})
{% endif %}
{% endfor %}
