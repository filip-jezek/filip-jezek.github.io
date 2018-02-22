---
title: Modelica newsletters archive
layout: default
---

Hello world!

PLease contribute! See [submission guidelines](sg.html)


## Newsletters
here is the set of all collections:

{% for collection in site.collections %}

  {% assign name = collection.label %}
  {% unless name == "posts" %}
  
  <section>
    <ul> 
    <h3>{{ name }}</h1>
    {% for page in site.[name] %}
    {% if page.index %}
    <li>[{{ page.title | markdownify }}](page.url) <BR /> {{ page.description }}</li>
    {% endif %}
    {% endfor %}
    </ul>
  </section>

{% endunless %}
{% endfor %}

## Archives
* [2015-01](archives/2015-01.html)
