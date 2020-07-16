---
layout: page
title: Shape-changing Interfaces Knowledge Base
permalink: /
---

# About SCI-KB

The Shape-Changing Interfaces Knowledge Base (SCI-KB) originates from the research project [ZELASTO]({{ site.baseurl }}/2019/daten-zum-anfassen/) which explores the interaction with complex data using [Zoomable User Interfaces]({{ site.baseurl }}/terms/zoomable-user-interface) on [Elastic Displays]({{ site.baseurl }}/terms/elastic-display). We aim to spread recent knowledge on the research of [shape-changing interfaces]({{ site.baseurl }}/terms/shape-changing-interface) (SCI) both theoretically and practically.  SCI-KB’s heart is a deeply interwoven 3-level-architecture of knowledge modules about shape-changing interfaces. A [Workshop Builder]({{ site.baseurl }}/workshop-builder) provides assistance in finding an arrangement of the knowledge items tailored to individual needs in order to hold a customized workshop. The core is supplemented by additional [resources]({{ site.baseurl }}/resources/) such as paper references, links and media content and thematically structured by means of tags on the meta-level.

![SCI-KB building blocks]({{ site.baseurl }}/assets/img/sci-kb-architecture.png)

### Modules

The knowledge modules items [Terms]({{ site.baseurl }}/terms-and-concepts/#terms), [Concept]({{ site.baseurl }}/terms-and-concepts/#concepts) and [Best Practices]({{ site.baseurl }}/best-practices/) can be arranged in any combination and pervade each of the three conceptual levels “Learn”, “Apply” and “Contribute”. Modules and levels of knowledge are inspired by [Bloom’s taxonomy of educational objectives](). Similarly, we also address factual knowledge on the lower levels (Learn, Terms, Concepts) and procedural knowledge on the higher levels (Contribute, Apply, Best Practices).

**Term**. On the "Learn" level, each term explains a technical term for shape-changing interfaces, for example "Elastic Display". On the "Apply" level, examples show how the term is used in practice. The "Contribute" level invites users to modify or add terms.

**Concept**. In the style of a cheat sheet, each concept explains on the "Learn" level an application-independent principle that can be useful for the implementation of a shape-changing interface. This includes, for example, design guidelines, overviews of chart types and data types or a gesture catalogue for interaction with elastic displays. On the "Apply" level, a Concept provides workshop material. Analogous to a Term, a Concept can be modified or created at the "Contribute" level.

**Best Practice**. On the "Learn" level, a best practice explains a practical challenge that may arise in the design process of shape-changing interfaces, such as the choice of a suitable prototyping technology, and shows ways to overcome the challenge. On the "Apply" level, there are suggestions on how to train the solutions in a workshop using materials provided by the Concepts particularly. Workshop participants are invited to publish the results of their workshops on the "Contribute" level or to create their own best practice.

### Topics
With the help of the supervised tag structure, knowledge items are grouped in the four thematic areas proposed by Alexander et al. for the classification of the research field on shape-changing interfaces (technological, behavioural, design and societal) \cite{10.1145/3173574.3173873}. In this way, a thematic access to the knowledge base is created. This division both separates disciplines within the field from each other and reflects successive stages of implementation. As a small difference, we have therefore renamed the category "behavioural" into "User Experience" to emphasize the steps of development.

<div class="flex-start">
{% assign groups = site.best-practices | group_by: "category" %}
{% for group in groups %}
<a class="capitalizeAll topic topic-{{ group.name | downcase | strip | replace:'user experience', 'user-experience'}}" href="{{ site.baseurl }}/{{ group.name | downcase | strip | replace:'user experience', 'user-experience' }}/">{{ group.name }}</a>
{% endfor %}
</div><br>

### Workshop Builder

With the [Workshop Builder]({{ site.baseurl }}/workshop-builder), you can find assistance in finding an arrangement of knowledge items, using them as building  blocks to conduct a workshop that is tailored to your individual needs. Based on the information you provide about the goal and context of the workshop, it will suggest suitable tools and your the starting point for a practical walk-through through SCI-KB. To match your needs, the walk-trough may be thematic, problem- or topic-oriented, a deep-dive into specific knowledge or explorative.

### Support

If you need help, please don't hesitate to [open an issue](https://www.github.com/{{ site.github_repo }}/issues).

![EFRE Logo]({{ site.baseurl }}/assets/img/efre-logo.jpg){: #efre-logo }
