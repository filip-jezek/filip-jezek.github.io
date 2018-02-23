We are building the WEB INDEX for current ISSUE!  
V4.0

## Table of contents
{:.no_toc}

* seed TOC list
{:toc}


{% assign name = page.name %}
{% assign cat = "vendor" %}

{% assign cat_posts = ((site.[name] | where:"category", cat %}
{{ cat_posts.size }}

{% if cat_posts.size > 0 %}
## Modelica association
{% endif %}

{% for page in cat_posts %}
### [{{ page.title }}]({{ page.url }}) - {{ page.category }} {#{{page.title | handleize }}}
{{ page.content | markdownify }}
{% if page.author %}
*This article is provided by {{ page.author }}*  
{% endif %}

***

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
