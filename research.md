---
layout: default
title: Research
---

# Research

<div class="research-grid">

  <article class="research-card">
    <a class="research-card__image" href="{{ '/research/nonlocal-metamaterials/' | relative_url }}">
      <img src="{{ '/assets/images/Research_01.jpg' | relative_url }}"
           alt="Nonlocal metamaterials and beyond-nearest-neighbor interactions">
    </a>
    <div class="research-card__body">
      <h2>1. Nonlocal Metamaterials</h2>
      <p>We investigate how interactions beyond nearest neighbors can be engineered to control static mechanical responses and wave propagation. This approach enables unusual dispersion relations, including roton-like bands, and new ways to implement nonlocal interactions across physical systems.</p>
      <ul>
        <li>Beyond-nearest-neighbor interactions and nonlocal elasticity</li>
        <li>Dispersion engineering and roton-like dispersion relations</li>
        <li>Anomalous static responses</li>
        <li>Nonlocal interaction engineering across physical systems</li>
      </ul>
    </div>
  </article>

  <article class="research-card">
    <a class="research-card__image" href="{{ '/research/advanced-mechanics-waves/' | relative_url }}">
      <img src="{{ '/assets/images/Research_02.jpg' | relative_url }}"
           alt="Advanced mechanics and wave physics in architected materials">
    </a>
    <div class="research-card__body">
      <h2>2. Advanced Mechanics and Wave Physics</h2>
      <p>We explore how material architecture and constitutive behavior determine the mechanical properties and collective dynamics of structured materials. Our work examines extremal elasticity, chiral and micropolar mechanics, and mechanical lattices with floppy modes and topological properties.</p>
      <ul>
        <li>Extremal elasticity and pentamode metamaterials</li>
        <li>Chiral mechanics and micropolar elasticity</li>
        <li>Maxwell lattices, floppy modes, and topological mechanics</li>
      </ul>
    </div>
  </article>

  <article class="research-card">
    <a class="research-card__image" href="{{ '/research/functional-metamaterials/' | relative_url }}">
      <img src="{{ '/assets/images/Research_03.jpg' | relative_url }}"
           alt="Functional metamaterials for acoustic cloaking and underwater sound insulation">
    </a>
    <div class="research-card__body">
      <h2>3. Functional Metamaterials and Applications</h2>
      <p>We design metamaterials to achieve functions that are difficult to realize with conventional materials. Examples include pentamode-based cloaking and underwater sound insulation, supported by inverse-design strategies for prescribed material responses.</p>
      <ul>
        <li>Pentamode cloaking for underwater acoustics</li>
        <li>Pentamode metamaterials for underwater sound insulation</li>
        <li>Inverse design of functional metamaterials</li>
      </ul>
    </div>
  </article>

  <article class="research-card research-card--placeholder" aria-label="Future research direction placeholder">
    <div class="research-card__placeholder-visual" aria-hidden="true">
      <span>+</span>
    </div>
    <div class="research-card__body">
      <h2>Future Research Directions</h2>
      <p>This space is reserved for an emerging research direction. A new topic, figure, and short description can be added here as the group's research develops.</p>
    </div>
  </article>

</div>

<style>
.research-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 2rem;
  margin: 2rem 0;
}

.research-card {
  min-width: 0;
  overflow: hidden;
  border: 1px solid #e2e5e9;
  border-radius: 10px;
  background: var(--global-card-bg-color, #fff);
}

.research-card__image {
  display: block;
  overflow: hidden;
  aspect-ratio: 16 / 9;
  background: #f1f3f5;
}

.research-card__image img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.25s ease;
}

.research-card__image:hover img {
  transform: scale(1.03);
}

.research-card__body {
  padding: 1.25rem 1.4rem 1.4rem;
}

.research-card__body h2 {
  margin-top: 0;
  font-size: 1.35rem;
}

.research-card__body p {
  margin-bottom: 1rem;
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
  display: block;
  line-height: 1;
}

@media (max-width: 700px) {
  .research-grid {
    grid-template-columns: 1fr;
    gap: 1.25rem;
  }
}
</style>
