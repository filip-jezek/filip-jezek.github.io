---
title: Modelica newsletters archive
layout: default
---

Hello world!

here is the set of all collections:

{% for issue in site.collections %}
  <li>
    <h6 class="post-meta">Issue {{ issue.name }} &mdash; {{ issue.date | date: "%b %-d, %Y" }}</h6>

    <h2>
      {{ issue.title }}
    </h2>
  </li>
{% endfor %}
