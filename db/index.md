---
layout: default
title: Databases
---

<header>
  <nav>
    <a href="/">gregoryjscott</a> / db
  </nav>

  <h1>{{ page.title }}</h1>
</header>

<section markdown="1">
My projects use these databases.
</section>

<section>
{% assign list = page.db | sort: 'projects_count' %}
{% for db in list reversed %}
  <h1><a href="{{ db.url }}">{{ db.title }}</a></h1>

  {% include links.md resource=db%}
{% endfor %}
</section>
