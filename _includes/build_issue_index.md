We are building the WEB INDEX for current ISSUE!
V4.0

{:toc}

{% assign name = page.name %}
## MA
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

## VENDOR
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
