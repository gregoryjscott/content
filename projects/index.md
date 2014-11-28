---
layout: default
title: Projects
---

<header>
  <nav>
    <a href="/">gregoryjscott</a> / projects
  </nav>

  <h1>{{ page.title }}</h1>
</header>

<section markdown="1">
These are most of my current and past projects. Projects can also be explored by skill such as [language](/languages), [operating system](/os), or [database](/db).
</section>

<section>
{% for item in page.items %}
  <h1>{{ item.title }}</h1>

  <p><em>{{ item.subtitle }}</em></p>

  {% include links.md resource=item %}
{% endfor %}
</section>
