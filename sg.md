---
title: Submission guidelines
layout: default
---

Hello world!

We do propose the following categories:
-  MA
-  Meetings
-  Vendor
-  Education
-  Library

here is the set of all categories:

{% for collection in site.collections %}

  {% assign name = collection.label %}

  <section>
    <h1>{{ name }}</h1>
    {% for page in site.[name] %}
  <p><a href="{{page.url}}")>{{ page.title }}</a> - {{ page.category}}</p>
    {% endfor %}
    
  </section>

{% endfor %}
