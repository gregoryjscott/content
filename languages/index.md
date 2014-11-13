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
{% assign list = page.languages | sort: 'projects_count' %}
{% for language in list reversed %}
  <h1>{{ language.title }}</h1>

  {% include links.md resource=language %}
{% endfor %}
</section>
