---
layout: page
title: Terms
permalink: /terms/
description: Terms each explain a technical term and illustrate it with practical examples. They primarily serve the level of factual knowledge by providing background knowledge to develop practical applications with shape-changing interfaces.
---

# {{ page.title }}

{{ page.description }} 
Feel free to share your own knowledge!  

{% assign groups = site.terms | group_by: "category" | where_exp: "group", "group.name != 'example'" %}

{% for group in groups %}
<a class="capitalizeAll capitalizeAll topic topic-{{ group.name | downcase | strip | replace:'user experience', 'user-experience'}}" href="{{ site.baseurl }}/{{ group.name | downcase | strip | replace:'user experience', 'user-experience' }}/">{{ group.name }}</a> 

<ul class="plain column">
{% for item in group.items %}
<li>
    <a href="{{ item.url | prepend: site.baseurl }}">{{ item.title }}</a>
</li>
{%endfor%}
</ul>

{%endfor%}

<div class="section-index">
    <hr class="panel-line">
    {% for post in site.docs  %}        
    <div class="entry">
    <h5><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h5>
    <p>{{ post.description }}</p>
    </div>{% endfor %}
</div>

<br>
<p>Are you facing a tricky challenge or looking for practical applications? See the collection of <a href="{{site.baseurl}}/best-practices">Best Practices</a>.</p>