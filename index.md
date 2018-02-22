---
title: Modelica newsletters archive
layout: default
---

Hello world!

PLease contribute! See [submission guidelines](sg.html)


## Newsletters
here is the set of all collections:

  
  <section>
    <ul> 
{% for collection in site.collections %}

  {% assign name = collection.label %}
  {% unless name == "posts" %}
      
    {% for page in site.[name] %}
    {% if page.index %}
      <li><a href="{{ page.url }}">{{ page.title | markdownify }}</a> <BR /> {{ page.description }}</li>
    {% endif %}
    {% endfor %}
    </ul>
  </section>

{% endunless %}
{% endfor %}


## Archives

* [2015-01](archives/2015-01.html)
