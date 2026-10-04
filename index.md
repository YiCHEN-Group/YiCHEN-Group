---
layout: default
title: Home
---

<div class="home-intro">

<div class="home-text">

<h2>About the Lab</h2>

Our lab combine theoretical modeling, numerical simulation, advanced fabrication, and experimental characterization to develop new physical concepts and functional metamaterial systems for addressing problems in mechanics, wave physics, and multiphysics systems.

<p>
<a href="mailto:your-email@example.com">Email</a> &nbsp;&nbsp;|&nbsp;&nbsp;
<a href="https://scholar.google.com/citations?user=dH3xIRcAAAAJ">Google Scholar</a> &nbsp;&nbsp;|&nbsp;&nbsp;
<a href="https://orcid.org/0000-0002-6614-976X">ORCID</a>
</p>

</div>

<div class="home-photo">

<!-- <img src="/assets/images/profile.jpg" alt="Yi Chen"> -->
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

<span>
{{ item.description }}
</span>

</div>

{% endfor %}
