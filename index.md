---
layout: default
title: Home
---

<div class="home-intro">

  <div class="home-text">
    <h2>Metamaterials: Mechanics, Waves, and Beyond</h2>

	<p class="about-intro">	
Our research focuses on mechanical and acoustic metamaterials, aiming to discover and realize physical behaviors beyond those of conventional materials. By engineering nonlocal interactions, structural architectures, and constitutive properties, we develop new strategies for controlling mechanical responses, wave propagation, and dispersion. Combining theoretical modeling, numerical simulations, and experimental investigations, we explore fundamental physical phenomena and translate our findings into functional metamaterial designs. Beyond mechanics and acoustics, we also explore how these principles can be extended to transport phenomena, including thermal and electrical transport and fluid flow.
	</p>
    <p>
      <a href="mailto:yi.chen@bit.edu.cn">Email</a> &nbsp;&nbsp;|&nbsp;&nbsp;
      <a href="https://scholar.google.com/citations?user=dH3xIRcAAAAJ">Google Scholar</a> &nbsp;&nbsp;|&nbsp;&nbsp;
      <a href="https://orcid.org/0000-0002-6614-976X">ORCID</a>
    </p>
  </div>

  <div class="home-photo">
    <!-- <img src="{{ '/assets/images/profile.jpg' | relative_url }}" alt="Yi Chen"> -->
  </div>

</div>

## News
{% assign news = site.data.news | sort: "date" | reverse %}

{% for item in news limit:10 %}
<div class="news-item">
  <strong>{{ item.date }}</strong>
  &nbsp;&nbsp;
  {{ item.title }}
  <br>
  <span>{{ item.description }}</span>
</div>
{% endfor %}

## Research
<div class="home-research-grid">
{% for direction in site.data.research %}
  <a class="home-research-card" href="{{ '/research' | relative_url }}">
    <img src="{{ direction.image | relative_url }}"
         alt="{{ direction.image_alt }}"
         loading="lazy">
    <div class="home-research-card__body">
      <h3>{{ direction.title }}</h3>
      <p>{{ direction.description | strip_html | truncatewords: 25 }}</p>
      <span class="home-research-link">Explore research →</span>
    </div>
  </a>
{% endfor %}
</div>

<p class="home-research-more">
  <a href="{{ '/research' | relative_url }}">View all research directions →</a>
</p>
