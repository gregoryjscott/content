---
layout: default
title: Languages
---

<header>
  <nav>
    <a href="/">gregoryjscott</a> / languages
  </nav>

  <h1>{{ page.title }}</h1>
</header>

<section markdown="1">
My projects use these programming languages.
</section>

<section>
{% for item in page.items %}
  <h1>{{ item.title }}</h1>

  {% include links.md resource=item %}
{% endfor %}
</section>
