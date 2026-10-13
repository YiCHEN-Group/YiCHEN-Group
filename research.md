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

<style>
.research-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 1.75rem;
  margin: 1.75rem 0;
}

.research-card {
  min-width: 0;
  overflow: hidden;
  border: 1px solid #e2e5e9;
  border-radius: 10px;
  background: var(--global-card-bg-color, #fff);
}

.research-card__image {
  overflow: hidden;
  aspect-ratio: 16 / 9;
  background: #f1f3f5;
}

.research-card__image img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.research-card__body {
  padding: 1.25rem 1.4rem 1.4rem;
}

.research-card__body h2 {
  margin-top: 0;
  font-size: 1.3rem;
  line-height: 1.35;
}

.research-card__body p {
  line-height: 1.6;
}

.research-card__body ul {
  margin-bottom: 0;
}

.research-card--placeholder {
  border: 2px dashed #c8cdd3;
  background: transparent;
}

.research-card__placeholder-visual {
  display: flex;
  align-items: center;
  justify-content: center;
  aspect-ratio: 16 / 9;
  background: #f7f8f9;
  color: #9aa1a9;
  font-size: 4rem;
  font-weight: 300;
}

.research-card__placeholder-visual span {
  line-height: 1;
}

@media (max-width: 700px) {
  .research-grid {
    grid-template-columns: 1fr;
    gap: 1.25rem;
  }
}
</style>
