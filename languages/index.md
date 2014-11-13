---
layout: default
title: Languages
---

<header>
  <nav>
    <a href="/">gregoryjscott</a> / {{ page.key }}
  </nav>

  <h1>{{ page.title }}</h1>
</header>

<section markdown="1">
I've written programs using the following programming languages. Each languages lists the projects that used the language.

I like to learn new languages! I also like using the best tool for the job. Having the ability to use (and fork if necessary) Ruby gems, JavaScript npm modules, Python pip packages, and C# NuGet packages to solve problems is very powerful.
</section>

<section>
{% assign list = page.languages | sort: 'projects_count' %}
{% for language in list reversed %}
  <h1><a href="{{ language.url }}">{{ language.title }}</a></h1>

  {% if language.todo %} *NEEDS WORK* {% endif %}

  <p>{{ language.desc }}</p>

  {% include links.md resource=language %}
{% endfor %}
</section>
