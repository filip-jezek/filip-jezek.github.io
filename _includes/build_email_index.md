This is a message to you..  
V1.0

{% assign name = page.name %}

## Modelica association
{% assign cat = "association" %}

{% for page in site.[name] %}
{% if page.category == cat and page.index != true %}
* [{{ page.title }}]({{site.url}}/{{ name }}/{{ page.path }}\#{{ page.title | slugify }})
{% endif %}
{% endfor %}

## Vendor news
{% assign cat = "vendor" %}
Hey, {{ cat }}!

{% for page in site.[name] %}
{% if page.category == cat and page.index != true %}
* [{{ page.title }}]({{ page.path }})
{% endif %}
{% endfor %}
