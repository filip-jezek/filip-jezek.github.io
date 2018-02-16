We are building the WEB INDEX for current ISSUE!
V3.0

{% assign name = page.name %}
{% for page in site.[name] %}

{% unless page.index %} 
## [{{ page.title }}]({{ page.url }}) - {{ page.category }}
{{ page.content | markdownify }}
*This article is provided by {{ page.author }}*
Three or more...

---

Hyphens

***

Asterisks

___

Underscores

{% endunless %}
{% endfor %}
