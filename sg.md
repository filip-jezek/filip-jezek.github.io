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
      <p>[{{ page.title }}]({{page.url}}) - {{ page.category}}</p>
    {% endfor %}
    
  </section>

{% endfor %}
