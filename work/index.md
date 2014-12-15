---
layout: default
---

<header>
<nav>
<a href="/">gregoryjscott</a> / work
</nav>

<h1>{{ page.title }}</h1>
</header>

<article markdown="1">
I've programmed PCs, Macs, mainframes, hand-held range finders, GPS devices, a laser mounted to single-engine plane, smartphones, tablets, calculators, and B-1 Bombers. I have been fortunate to work with teams of amazingly talented people on these exciting and challenging projects.

Feel free to browse through my projects or look over my resume.
</article>

<a class="button" href="{{ page._links.projects.href }}">{{ page._links.projects.title }}</a>
<a class="button" href="{{ page._links.resume.href }}">{{ page._links.resume.title }}</a>

## Show me some code!

<article markdown="1">
You bet. The source code for all my open source projects is on GitHub.
</article>

<a class="button" href="{{ page._links.code.href }}">{{ page._links.code.title }}</a>

# Find out more about me.

<a class="button" href="/skills/">Explore my skills.</a>
<a class="button" href="/services/">Learn what I can do for you.</a>

<section markdown="1">
{% include get-started.md %}
</section>
