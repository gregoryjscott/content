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
{% for item in page.items %}
  <h1>{{ item.title }}</h1>

  {% include links-ul.md data=item %}
{% endfor %}
</section>
