---
layout: page
title: About SCI-KB
permalink: /
---



# {{ page.title }}

The Shape-Changing Interfaces Knowledge Base (SCI-KB) originates from the research project [ZELASTO]({{ site.baseurl }}/2019/daten-zum-anfassen/) which explores the interaction with complex data using [Zoomable User Interfaces]({{ site.baseurl }}/terms/zoomable-user-interface) on [Elastic Displays]({{ site.baseurl }}/terms/elastic-display). We aim to spread recent knowledge on the research of [shape-changing interfaces]({{ site.baseurl }}/terms/shape-changing-interface) (SCI) both theoretically and practically. Modular knowledge items can be combined arbitrarily, e.g. to hold workshops. A [Workshop Builder]({{ site.baseurl }}/workshop-builder) provides assistance in finding an individual arrangement. The core of knowledge is supplemented by additional [resources]({{ site.baseurl }}/resources/) and structured by tags which reflect various topics in the interdisciplinary field of shape-changing interfaces.

![EFRE Logo]({{ site.baseurl }}/assets/img/efre-logo.jpg){: #efre-logo }

<details markdown="1" open>
<summary><h3>Topics</h3></summary> 

Browse [topics]({{ site.baseurl }}/topics) to discover knowledge items in one of the 4 essential topics related to the field of shape-changing interfaces. The topics can also be interpreted as states of development.

<div class="flex-start">
{% assign groups = site.best-practices | group_by: "category" %}
{% for group in groups %}
<a class="capitalizeAll topic topic-{{ group.name | downcase | strip | replace:'user experience', 'user-experience'}}" href="{{ site.baseurl }}/{{ group.name | downcase | strip | replace:'user experience', 'user-experience' }}/">{{ group.name }}</a>
{% endfor %}
</div><br>

</details>

<details markdown="1" open>
<summary><h3>Knowledge Modules</h3></summary> 

Depending on the type of knowledge they contain, smaller knowledge items are assigned one of the modules [Terms]({{ site.baseurl }}/terms), [Concept]({{ site.baseurl }}/concepts) or [Best Practices]({{ site.baseurl }}/best-practices/) (see picture). The modules each pervade the three conceptual levels “Learn”, “Apply” and “Contribute”. Thus, exploring items within a module provides an alternative path to the topic-based approach. 

![SCI-KB building blocks]({{ site.baseurl }}/assets/img/sci-kb-architecture.png)


**Term**. On the "Learn" level, each term explains a technical term for shape-changing interfaces, for example "Elastic Display". On the "Apply" level, examples show how the term is used in practice. The "Contribute" level invites users to modify or add terms.

**Concept**. In the style of a cheat sheet, each concept explains on the "Learn" level an application-independent principle that can be useful for the implementation of a shape-changing interface. This includes, for example, design guidelines, overviews of chart types and data types or a gesture catalogue for interaction with elastic displays. On the "Apply" level, a Concept provides workshop material. Analogous to a Term, a Concept can be modified or created at the "Contribute" level.

**Best Practice**. On the "Learn" level, a best practice explains a practical challenge that may arise in the design process of shape-changing interfaces, such as the choice of a suitable prototyping technology, and shows ways to overcome the challenge. On the "Apply" level, there are suggestions on how to train the solutions in a workshop using materials provided by the Concepts particularly. Workshop participants are invited to publish the results of their workshops on the "Contribute" level or to create their own best practice.

</details>

<details markdown="1" open>
<summary><h3>Workshop Builder</h3></summary> 

With the [Workshop Builder]({{ site.baseurl }}/workshop-builder), modular workshops tailored to the custom needs can be composed from the knowledge items. Therefore, the starting point for a practical walkthrough through SCI-KB that is based on the context of the workshop and its objectives is suggested. The walktrough may be thematic, problem- or topic-oriented, a deep-dive into specific knowledge or explorative. [Start planning your workshop]({{ site.baseurl }}/workshop-builder).

</details>

### Support

If you need help, please don't hesitate to [open an issue](https://www.github.com/{{ site.github_repo }}/issues).


