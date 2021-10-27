---
layout: page
title: Topics
permalink: /topics/
---

# {{ page.title }}

Topics describe 4 essential topics related to the field of shape-changing interfaces. The topics can also be interpreted as states of development.

<!-- topic previews (link and desciption) -->

{% assign topics = site.pages | where: "layout", "topic" %}

<ul class="plain tile">

{% for item in topics %}

{% assign terms = site.terms | where: "category", item.title %}
{% assign concepts = site.concepts | where: "category", item.title %}
{% assign best-practices = site.best-practices | where: "category", item.title %}

<li>
<a class="capitalizeAll topic topic-{{ item.title | downcase | strip | replace:'user experience', 'user-experience'}}" href="{{ site.baseurl }}/{{ item.title | downcase | strip | replace:'user experience', 'user-experience' }}/">{{ item.title}}</a>
<p class="margin-top">{{ item.description }}</p>
<p class="counts topic-{{ item.title | downcase | strip | replace:'user experience', 'user-experience'}}">{{ terms.size }} Terms / {{concepts.size }} Concepts / {{ best-practices.size }} Best Practices</p>
</li>

{% endfor %}

</ul>

<hr>
<br>
<p>Browse <a href="{{site.baseurl}}/knowledge-modules">knowledge modules</a> instead.</p>




