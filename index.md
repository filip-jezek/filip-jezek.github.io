---
title: Modelica newsletters archive
layout: default
---

Hello world!

PLease contribute! See [submission guidelines](sg.html)


## Newsletters
here is the sorted set of all collections:

  
  <section>
    <ul> 
{% assign sorted = (site.collections | sort: 'date') | reverse %}
         
{% for collection in sorted %}

  {% assign name = collection.label %}
  {% unless name == "posts" %}
      
    {% for page in site.[name] %}
    {% if page.name == name %}
      <li><a href="{{ page.url }}">{{ page.title }}</a><BR />{{ page.description }}</li>
    {% endif %}
    {% endfor %}
{% endunless %}
{% endfor %}    
    </ul>
  </section>


## Archives

* [2015-01](archives/2015-01.html)
