---
title: Modelica newsletters archive
layout: default
---

Hello world!

here is the set of all collections:

{% for collection in site.collections %}

  {% assign name = collection.label %}

  <section>
    <h1>{{ name }}</h1>

    {% for page in site.[name] %}
    {% unless page.index %}
    <article>
      <h2>{{ page.title | markdownify }} ({{ page.category }})</h2>
      <p>{{ page.content | markdownify }}</p>
      <p>{{ page.authors | markdownify }}</p>
    </article>
    {% endunlessf %}
    {% endfor %}
    
  </section>

{% endfor %}

And then there are [submission guidelines](sg.html)
