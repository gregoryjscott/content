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
{% assign list = page.projects | sort: 'begin_year' | sort: 'end_year', 'last' %}
{% for project in list reversed %}
  <h1><a href="{{ project.url }}">{{ project.title }}</a></h1>

  <p>
  <em>
    {{ project.role }},
    {{ project.begin_year }}
      {% unless project.begin_year == project.end_year %} -
        {% if project.end_year %}
          {{ project.end_year }}
        {% else %}
          present
        {% endif %}
      {% endunless %}
  </em>
  </p>

  {% include links.md resource=project %}
{% endfor %}
</section>
