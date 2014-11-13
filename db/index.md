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
I've written programs that used the following databases. Each database lists the projects that used the database.

</section>

<section>
{% assign list = page.db | sort: 'projects_count' %}
{% for db in list reversed %}
  <h1><a href="{{ db.url }}">{{ db.title }}</a></h1>

  {% include links.md resource=db%}
{% endfor %}
</section>
