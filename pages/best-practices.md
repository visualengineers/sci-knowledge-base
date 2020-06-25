---
layout: page
title: Best Practices
permalink: /best-practices/
---

# Best Practices

Best Practices cover practical challenges that may arise during the design process of shape-changing interfaces. To help you get started they are grouped into 4 major topics: <a href="{{site.baseurl }}/technology">Technology</a>, <a href="{{site.baseurl }}/ux">User Experience</a>, <a href="{{site.baseurl }}/design">Design</a> and <a href="{{site.baseurl }}/society">Society</a>. 

Read about a specific challenge and why it is important and what ways you have to overcome it. Additional workshop instructions help you to quickly train your aquired knowledge in practice. You are invited to publish the results of your workshops or to create your own best practice.

### Topics

{% assign groups = site.best-practices | group_by: "category" %}

{% for group in groups %}
<a href="{{ site.baseurl }}/{{ group.name | downcase | strip | replace:'user experience', 'ux' }}/">{{ group.name | replace:'UX', 'User Experience'}}</a>
{: .topic .topic-{{ group.name | downcase | strip | replace:'user experience', 'ux'}}}

<ul class="tile">
{% for item in group.items %}
<li>
    <a href="{{ item.url | prepend: site.baseurl }}">
        <img src="{{ item.image }} /">
        <h5>{{ item.title }}</h5>
    </a>
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
