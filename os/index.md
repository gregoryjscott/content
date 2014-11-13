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
I've written programs that run on the following operating systems. Each operating system lists the projects that were deployed to, and/or tested on, the operating system.
</section>

<section>
{% assign list = page.os | sort: 'projects_count' %}
{% for os in list reversed %}
  <h1><a href="{{ os.url }}">{{ os.title }}</a></h1>

  {% include links.md resource=os %}
{% endfor %}
</section>
