---
title: Modelica newsletters archive
layout: default
---

Hello world!

here is the set of all collections:

{% for collection in site.collections %}

  {% assign name = collection.label %}
  {% unless name == "posts" %}
  
  <section>
    <h1>{{ name }}</h1>
    {% for page in site.[name] %}
    {% unless page.index %}
    <article>
      <h2>{{ page.title | markdownify }} ({{ page.category }})</h2>
      <p>{{ page.content | markdownify }}</p>
      <p>{{ page.authors | markdownify }}</p>
    </article>
    {% endunless %}
    {% endfor %}
    
  </section>

{% endunless %}
{% endfor %}

And then there are [submission guidelines](sg.html)
