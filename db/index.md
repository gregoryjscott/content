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
{% for item in page.items %}
  <h1>{{ item.title }}</h1>

  {% include links-ul.html data=item %}
{% endfor %}
</section>
