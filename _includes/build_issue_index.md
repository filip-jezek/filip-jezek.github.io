We are building the WEB INDEX for current ISSUE!
V2.0

{% assign name = page.name %}
{% for page in site.[name] %}

{% unless page.index %} 
## [{{ page.title }}]({{ page.url }}) - {{ page.category }}
  {{ page.content | markdownify }}
  *{{ page.author }}*
***
{% endunless %}
{% endfor %}
