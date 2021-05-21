---
layout: page
title: Activities
permalink: /activities/
description: Activities are collections of terms, concepts, and best practices on a specific issue or question. Example activities include Getting Started With SCI-KB, Elastic Display in Historical Context, or Prototyping Approaches.
---

# {{ page.title }}

{{ page.description }} 

---------------
{% assign activities = site.activities %}

<ul class="tile">
{% for activity in activities %}
<li>
    <a href="{{ activity.url | prepend: site.baseurl }}" alt="{{ activity.description }}">
            {% if activity.image %}
                <img src="{{ activity.image }}">
            {% else %}
                <img src="https://images.unsplash.com/photo-1566041510639-8d95a2490bfb?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=626&q=80">
            {% endif %}
            <span>{{ activity.title }}</span>
            <p class="counts topic-{{ item.title | downcase | strip | replace:'user experience', 'user-experience'}}">
            {{ activity.terms.size }} Terms / {{activity.concepts.size }} Concepts / {{ activity.best-practices.size }} Best Practices / {{ activity.interviews.size }} Interviews</p>
      </a>
</li>
{%endfor%}
</ul>

<div class="section-index">
    <hr class="panel-line">
    {% for post in site.docs  %}        
    <div class="entry">
    <h5><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h5>
    <p>{{ post.description }}</p>
    </div>{% endfor %}
</div>

<br>
<p>Don't know where to start? Try out <a href="{{site.baseurl}}/activities/getting-started">Getting Started With SCI-KB</a>.</p>