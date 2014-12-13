---
layout: default
title: Databases
_links:
  email:
    title: Email me.
    href: mailto:me@gregoryjscott.com
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
  <h1><a href="{{ item.url }}">{{ item.title }}</a></h1>

  <p>{{ item.desc }}</p>

  {% include links-ul.html data=item %}
{% endfor %}
</section>

<hr>

<section markdown="1">
{% include get-started.md email=page._links.email %}
</section>
