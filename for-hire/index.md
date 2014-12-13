---
layout: default
---

<header>
<nav>
<a href="/">gregoryjscott</a> / for-hire
</nav>

<h1>{{ page.title }}</h1>
</header>

<article markdown="1">
Technology moves so fast. Change is exciting, but it can also be scary. We can't stop it, so our only choice is to embrace it. Fortunately, it turns out that change isn't so scary if you prepare for it. In fact, it can even be fun!

**I've helped schools, governments, and businesses** of all kinds build systems that work _and_ change over time. Technology systems are either improving or dying - that's how technology evolves.

In this world filled with technology, chances are good that you're dealing with technology problems at your place of work. Perhaps **I can help you**.
</article>

# Check out my work.

<article markdown="1">
My career has been filled with challenging projects, engaged clients, great companies, and awesome teammates. I've been very fortunate. Feel free to browse through my projects or look over my resume.
</article>

<a class="button" href="{{ page._links.projects.href }}">{{ page._links.projects.title }}</a>
<a class="button" href="{{ page._links.resume.href }}">{{ page._links.resume.title }}</a>

## Show me some code!

<article markdown="1">
You bet. The source code for all my open source projects is on GitHub. If you find anything that looks incorrect then please send me a pull request. I'm always grateful for contributions.
</article>

<a class="button" href="{{ page._links.oss.href }}">{{ page._links.oss.title }}</a>

# Explore my skills.

<article markdown="1">
Want technical details? I've got you covered. You can browse my work by skill such as language, database, or operating system. Everything is cross-referenced with hyperlinks so knock yourself out.
</article>

<a class="button" href="{{ page._links.languages.href }}">{{ page._links.languages.title }}</a>
<a class="button" href="{{ page._links.db.href }}">{{ page._links.db.title }}</a>
<a class="button" href="{{ page._links.os.href }}">{{ page._links.os.title }}</a>

<section markdown="1">
{% include get-started.md email=page._links.email %}
</section>
