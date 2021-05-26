---
layout: page
title: Knowledge Modules
permalink: /knowledge-modules/
---

# {{ page.title }}

Here you can find an all terms, concepts, and best practices in SCI-KB at a glance. You can also browse them [by topic]({{ site.baseurl}}/topics).

{% assign terms = site.terms %}
{% assign concepts = site.concepts %}
{% assign best-practices = site.best-practices %}


<!-- terms -->
<details markdown="1" open>
<summary><h3>Terms</h3></summary> 

<ul class="plain column">
{% for item in terms %}
<li>
    <a href="{{ item.url | prepend: site.baseurl }}">{{ item.title }}</a>
</li>
{%endfor%}
</ul>

</details>

<!-- concepts -->
<details markdown="1" open>
<summary><h3>Concepts</h3></summary> 

<ul class="tile">
        {% for item in concepts %}
        <li>
            <a href="{{ item.url | prepend: site.baseurl }}">
                {% if item.image %}
                    <img src="{{ item.image }}" />
                {% else %}
                    <img src="https://images.unsplash.com/photo-1566041510639-8d95a2490bfb?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=626&q=80">
                {% endif %}
                <h5>{{ item.title }}</h5>
            </a>
        </li> 
        {%endfor%}
</ul>

</details>

<!-- best practices -->
<details markdown="1" open>
<summary><h3>Best Practices</h3></summary> 

<ul class="tile">
        {% for item in best-practices %}
        <li>
            <a href="{{ item.url | prepend: site.baseurl }}">
                {% if item.image %}
                    <img src="{{ item.image }}" />
                {% else %}
                    <img src="https://images.unsplash.com/photo-1566041510639-8d95a2490bfb?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=626&q=80">
                {% endif %}
                <h5>{{ item.title }}</h5>
            </a>
        </li> 
        {%endfor%}
</ul>

</details>

<hr>
<br>
<p>Browse <a href="{{site.baseurl}}/topics">by topic</a> instead.</p>





