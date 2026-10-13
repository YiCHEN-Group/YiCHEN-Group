---
layout: default
title: Research
---

# Research

<div class="research-grid">
{% for direction in site.data.research %}
  <article class="research-card">
    <div class="research-card__image">
      <img src="{{ direction.image | relative_url }}"
           alt="{{ direction.image_alt }}"
           loading="lazy">
    </div>
    <div class="research-card__body">
      <h2>{{ forloop.index }}. {{ direction.title }}</h2>
      <p>{{ direction.description }}</p>
      <ul>
      {% for topic in direction.topics %}
        <li>{{ topic }}</li>
      {% endfor %}
      </ul>
    </div>
  </article>
{% endfor %}
