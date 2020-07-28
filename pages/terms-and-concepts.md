---
layout: page
title: Terms & Concepts
permalink: /terms-and-concepts/
---

# Terms & Concepts

The terms and concepts primarily serve the level of factual knowledge by providing background knowledge to develop practical applications with shape-changing interfaces. Feel free to share your own knowledge!  

### Terms
The terms each explain a technical term and illustrate it with practical examples.
<ul class="plain column">{% for term in site.terms %} 
    <li><a href="{{ term.url | prepend: site.baseurl }}" alt="{{ term.description }}">{{ term.title }}</a></li>  
{% endfor %}
</ul>

### Concepts
Concepts assist you in the development of any kind of shape-changing interface by giving you an overview over different techniques or explaning a transferable method. Additionally, they may provide workshop material.

<ul class="tile">{% for concept in site.concepts %} 
    <li>
      <a href="{{ concept.url | prepend: site.baseurl }}" alt="{{ concept.description }}">
            {% if concept.image %}
                <img src="{{ concept.image }}">
            {% else %}
                <img src="https://images.unsplash.com/photo-1566041510639-8d95a2490bfb?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=626&q=80">
            {% endif %}

          <span>{{ concept.title }}</span>
      </a>
  </li>
   <!-- <li><a href="{{ concept.url | prepend: site.baseurl }}" alt="{{ concept.description }}">{{ concept.title }}</a></li>  -->
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

<br>
<p>Are you facing a tricky challenge or looking for practical applications? See the collection of <a href="{{site.baseurl}}/best-practices">Best Practices</a>.</p>