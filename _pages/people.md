---
layout: archive
title: "Group Members"
permalink: /people/
author_profile: true
---

{% for person in site.people %}
  <div class="person-card">
    {% if person.image %}
      <img src="{{ person.image }}" alt="{{ person.name }}" style="width:150px; border-radius:50%">
    {% endif %}
    <h2>{{ person.name }}</h2>
    <p><strong>{{ person.position }}</strong></p>
    <p>{{ person.content | markdownify }}</p>
  </div>
{% endfor %}
