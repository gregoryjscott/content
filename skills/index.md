---
layout: default
---

<header>
<nav>
<a href="/">gregoryjscott</a> / skills
</nav>

<h1>{{ page.title }}</h1>
</header>

<article markdown="1">
If you're looking for a specific set of technical skills then you've came to the right place. You can browse my work by skill such as language, database, or operating system. Everything is cross-referenced with hyperlinks so knock yourself out.
</article>

<a class="button" href="{{ page._links.languages.href }}">{{ page._links.languages.title }}</a>
<a class="button" href="{{ page._links.db.href }}">{{ page._links.db.title }}</a>
<a class="button" href="{{ page._links.os.href }}">{{ page._links.os.title }}</a>

<article markdown="1">
Don't see the particular skills you have in mind? No worries - learning new skills is my best skill.
</article>

# Find out more about me.

<a class="button" href="/work/">Check out my work.</a>
<a class="button" href="/services/">Learn what I can do for you.</a>

<section markdown="1">
{% include get-started.md %}
</section>
