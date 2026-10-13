---
layout: default
title: Research
permalink: /research/
---

# Research

Our research connects the engineering of material interactions with the discovery of unconventional mechanical and wave phenomena, and their use in functional metamaterial designs.

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

  <article class="research-card research-card--placeholder">
    <div class="research-card__placeholder-visual" aria-hidden="true">
      <span>+</span>
    </div>
    <div class="research-card__body">
      <h2>Future Research Directions</h2>
      <p>This space is reserved for an emerging research direction. A new topic, figure, and description can be added here as the group's research develops.</p>
    </div>
  </article>
</div>
