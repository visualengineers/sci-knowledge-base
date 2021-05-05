---
layout: page
title: Concepts
permalink: /concepts/
description: Concepts assist you in the development of any kind of shape-changing interface by giving you an overview over different techniques or explaning a transferable method. Additionally, concepts may provide workshop material.
---

# {{ page.title }}

{{ page.description }} 
Feel free to share your own knowledge!  

---------------
{% assign groups = site.concepts | group_by: "category" | where_exp: "group", "group.name != 'example'" %}

{% for group in groups %}
<a class="capitalizeAll capitalizeAll topic topic-{{ group.name | downcase | strip | replace:'user experience', 'user-experience'}}" href="{{ site.baseurl }}/{{ group.name | downcase | strip | replace:'user experience', 'user-experience' }}/">{{ group.name }}</a> 

<ul class="tile">
{% for item in group.items %}
<li>
    <a href="{{ item.url | prepend: site.baseurl }}" alt="{{ item.description }}">
            {% if item.image %}
                <img src="{{ item.image }}">
            {% else %}
                <img src="https://images.unsplash.com/photo-1566041510639-8d95a2490bfb?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=626&q=80">
            {% endif %}
          <span>{{ item.title }}</span>
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

<br>
<p>Are you facing a tricky challenge or looking for practical applications? See the collection of <a href="{{site.baseurl}}/best-practices">Best Practices</a>.</p>