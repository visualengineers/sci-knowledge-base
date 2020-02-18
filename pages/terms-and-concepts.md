---
layout: page
title: Terms and Concepts
permalink: /terms-and-concepts/
---

# <i class="fa fa-book-open"></i> Terms and Concepts

Find detailed explanation about vocabulary and concepts of elastic displays.

### Terms
<ul>{% for term in site.terms %} 
    <li><a href="{{ term.url }}" alt="{{ term.description }}">{{ term.title }}</a></li>  
{% endfor %}
</ul>

### Concepts
<ul>{% for concept in site.concepts %} 
    <li><a href="{{ concept.url }}" alt="{{ concept.description }}">{{ concept.title }}</a></li>  
{% endfor %}
</ul>


<div class="section-index">
    <hr class="panel-line">
    {% for post in site.docs  %}        
    <div class="entry">
    <h5><a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h5>
    <p>{{ post.description }}</p>
    </div>{% endfor %}
</div>
