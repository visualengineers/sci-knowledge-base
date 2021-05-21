---
layout: activity
title: Getting Started
description: getting started with SCI-KB
image: https://images.unsplash.com/photo-1513151233558-d860c5398176?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1950&q=80
image-credits: Photo by <a href="https://unsplash.com/@ninjason?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Jason Leung</a> on <a href="https://unsplash.com/s/photos/confetti?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>

# Insert the titles of all knowledge modules or interviews that belong to your activity 
# Due to YAML syntax, lists are needed for multiple entries, see https://docs.ansible.com/ansible/latest/reference_appendices/YAMLSyntax.html
terms: 
- example_term
- elastic-display
concepts: 
- example_concept
best-practices: 
- example_best-practice
interviews: 
- example_interview
links:
  - title: "Git-flow-Workflow"
    url: https://www.atlassian.com/de/git/tutorials/comparing-workflows/gitflow-workflow
  - title: "SCI-KB GitHub Repository"
    url: https://github.com/visualengineers/sci-knowledge-base
---

In this activity you will learn how the SCI-KB is organized, what features it has and how you can use them. If you want to share your own content, check out the sample templates and the additional links below.

<details markdown="1" open>
<summary><h3>What is SCI-KB?</h3></summary> 

The Shape-Changing Interfaces Knowledge Base (SCI-KB) originates from the research project [ZELASTO]({{ site.baseurl }}/2019/daten-zum-anfassen/) which explores the interaction with complex data using [Zoomable User Interfaces]({{ site.baseurl }}/terms/zoomable-user-interface) on [Elastic Displays]({{ site.baseurl }}/terms/elastic-display). We aim to spread recent knowledge on the research of [shape-changing interfaces]({{ site.baseurl }}/terms/shape-changing-interface) (SCI) both theoretically and practically. Modular knowledge items can be combined arbitrarily, e.g. to hold workshops. A [Workshop Builder]({{ site.baseurl }}/workshop-builder) provides assistance in finding an individual arrangement. The core of knowledge is supplemented by additional [resources]({{ site.baseurl }}/resources/) and structured by tags which reflect various topics in the interdisciplinary field of shape-changing interfaces.

### Topics

Browse [topics]({{ site.baseurl }}/topics) to discover knowledge items in one of the 4 essential topics related to the field of shape-changing interfaces. The topics can also be interpreted as states of development.

<div class="flex-start">
{% assign groups = site.best-practices | group_by: "category" | where_exp: "group", "group.name != 'example'" %}
{% for group in groups %}
<a class="capitalizeAll topic topic-{{ group.name | downcase | strip | replace:'user experience', 'user-experience'}}" href="{{ site.baseurl }}/{{ group.name | downcase | strip | replace:'user experience', 'user-experience' }}/">{{ group.name }}</a>
{% endfor %}
</div><br>

### Knowledge Modules

Depending on the type of knowledge they contain, smaller knowledge items are assigned one of the modules [Terms]({{ site.baseurl }}/terms), [Concept]({{ site.baseurl }}/concepts) or [Best Practices]({{ site.baseurl }}/best-practices/) (see picture). The modules each pervade the three conceptual levels “Learn”, “Apply” and “Contribute”. Thus, exploring items within a module provides an alternative path to the topic-based approach. 

![SCI-KB building blocks]({{ site.baseurl }}/assets/img/sci-kb-architecture.png)


**Term**. On the "Learn" level, each term explains a technical term for shape-changing interfaces, for example "Elastic Display". On the "Apply" level, examples show how the term is used in practice. The "Contribute" level invites users to modify or add terms.

**Concept**. In the style of a cheat sheet, each concept explains on the "Learn" level an application-independent principle that can be useful for the implementation of a shape-changing interface. This includes, for example, design guidelines, overviews of chart types and data types or a gesture catalogue for interaction with elastic displays. On the "Apply" level, a Concept provides workshop material. Analogous to a Term, a Concept can be modified or created at the "Contribute" level.

**Best Practice**. On the "Learn" level, a best practice explains a practical challenge that may arise in the design process of shape-changing interfaces, such as the choice of a suitable prototyping technology, and shows ways to overcome the challenge. On the "Apply" level, there are suggestions on how to train the solutions in a workshop using materials provided by the Concepts particularly. Workshop participants are invited to publish the results of their workshops on the "Contribute" level or to create their own best practice.

### Workshop Builder

With the [Workshop Builder]({{ site.baseurl }}/workshop-builder), modular workshops tailored to the custom needs can be composed from the knowledge items. Therefore, the starting point for a practical walkthrough through SCI-KB that is based on the context of the workshop and its objectives is suggested. The walktrough may be thematic, problem- or topic-oriented, a deep-dive into specific knowledge or explorative. [Start planning your workshop]({{ site.baseurl }}/workshop-builder).

</details>


<details markdown="1" open>
<summary><h3>How can I contribute?</h3></summary> 

Glad you want to join, it's quite easy. You only need a [GitHub](https://github.com/) account and should not be afraid of Markdown. Generally, you can add new knowledge modules or edit existing ones. In the desktop view of the SCI-KB you can see a link to edit the page directly on GitHub (top right corner). The easiest way is to copy code from existing pages, e.g. the example modules linked below. In the [GitHub repository of SCI-KB](https://github.com/visualengineers/sci-knowledge-base) you can also find detailed instructions on how to paste content in the existing style of the SCI-KB. 

</details>
