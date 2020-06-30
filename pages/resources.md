---
layout: page
title: Resources
permalink: /resources/
---

# Resources
additional resources related to the research on Elastic Displays

<details markdown="1" open>
<summary><h3>References</h3></summary> 

{% assign references = site.data.references | sort: "author" %}
<ul>
{% for reference in references %}
{% assign index = forloop.index %}
<li>
    [{{ index }}] {{ reference.author }}{% if reference.date %} ({{ reference.date}}) }{% elsif reference.year %} ({{ reference.year}}){% endif %}. <a href="{{ reference.url }}">{{ reference.title }}</a>.{% if reference.in %} In: {{ reference.in}}. {% endif %} {{ reference.url }}
</li>
{% endfor %}
</ul>

</details>

<details markdown="1" open>
<summary><h3>Links</h3></summary> 

{% assign links = site.data.links | sort: "title" %}
<ul>
{% for link in links %}
<li>
    <a href="{{ link.url }}">{{ link.title }}</a>{% if link.src %}, {{ link.src}} {% endif %}. {{ link.url }}
</li>
{% endfor %}
</ul>

</details>

