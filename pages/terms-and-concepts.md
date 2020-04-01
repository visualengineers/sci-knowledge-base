---
layout: page
title: Terms and Concepts
permalink: /terms-and-concepts/
---

# <i class="fa fa-book-open"></i> Terms and Concepts

Explore the vocabulary of shape-changing interfaces and its application. Feel free to share your own knowledge!  

- _Each **term** explains a technical term for shape-changing interfaces and provides examples to illustrate how its used in practice.  
- _Just like of a cheat sheet, each **concept** explains an application-independent principle (such as design guidelines) that are useful for the implementation of a shape-changing interface. Additionally, a Concept provides material to hold your own workshop.

### Terms
<ul>{% for term in site.terms %} 
    <li><a href="{{ term.url | prepend: site.baseurl }}" alt="{{ term.description }}">{{ term.title }}</a></li>  
{% endfor %}
</ul>

### Concepts
<ul>{% for concept in site.concepts %} 
    <li><a href="{{ concept.url | prepend: site.baseurl }}" alt="{{ concept.description }}">{{ concept.title }}</a></li>  
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
