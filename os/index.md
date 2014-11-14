---
layout: default
title: Operating Systems
---

<header>
  <nav>
    <a href="/">gregoryjscott</a> / os
  </nav>

  <h1>{{ page.title }}</h1>
</header>

<section markdown="1">
My projects run on these operating systems.
</section>

<section>
{% assign list = page.os | sort: 'projects_count' %}
{% for os in list reversed %}
  <h1><a href="{{ os.url }}">{{ os.title }}</a></h1>

  {% include links.md resource=os %}
{% endfor %}
</section>
