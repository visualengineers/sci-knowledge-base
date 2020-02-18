---
layout: page
title: Best Practices
permalink: /best-practices/
---

# Best Practices

Best Practices cover current challenges in research on elastic displays in the 4 major topics <a href="{{site.baseurl }}/technology">technology</a>, <a href="{{site.baseurl }}/ux">UX</a>, <a href="{{site.baseurl }}/design">design</a> and <a href="{{site.baseurl }}/society">society</a>. Read about a specific **challenge** and why it is important, what **options** you have to face it and discover **examples** of existing solutions. Additional **workshop** instructions help you to quickly apply your aquired knowledge in practice.

### Topics

{% assign groups = site.best-practices | group_by: "category" %}

{% for group in groups %}
<a href="/{{ group.name | downcase | strip | replace:'user experience', 'ux' }}/">{{ group.name | replace:'UX', 'User Experience'}}</a>
{: .topic .topic-{{ group.name | downcase | strip | replace:'user experience', 'ux'}}}

<ul>
{% for item in group.items %}
<li><a href="{{ item.url }}">{{ item.title }}</a></li>
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
