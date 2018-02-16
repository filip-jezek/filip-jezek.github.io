We are building the WEB INDEX for current ISSUE!

{% assign name = page.name %}
{% for page in site.[name] %}

{% unless page.index %} 
## [{{ page.title }}]({{ page.url }}) - {{ page.category }}
  {{ page.content | markdownify }}
***
{% endunless %}

{% comment %}
{% if page.index == null %} 
  *PAGE {{ page.title }} null.*
{% endif %}

{% if page.index != true %} 
  *PAGE {{ page.title }} untrue.*
{% endif %}

{% if page.index == "hitparada" %}
  ## [{{ page.title }}]({{ page.url }}) - {{ page.category }}
  {{ page.content | markdownify }}
  ***
  {% endif %}
{% endcomment %}
  {% endfor %}
