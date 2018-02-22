We are building the WEB INDEX for current ISSUE!  
V4.0

## Table of contents
{:.no_toc}

* seed TOC list
{:toc}

{% assign name = page.name %}
## Modelica association
{% assign cat = "ma" %}
{% for page in site.[name] %}
{% if page.category == cat and page.index != true %}
### [{{ page.title }}]({{ page.url }}) - {{ page.category }}
{{ page.content | markdownify }}
{% if page.author %}
*This article is provided by {{ page.author }}*  
{% endif %}

***

{% endif %}
{% endfor %}

## Vendor news
{% assign cat = "vendor" %}
{% for page in site.[name] %}
{% if page.category == cat and page.index != true %}
### [{{ page.title }}]({{ page.url }}) - {{ page.category }}
{{ page.content | markdownify }}
{% if page.author %}
*This article is provided by {{ page.author }}*  
{% endif %}

***

{% endif %}
{% endfor %}
