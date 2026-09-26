---
layout: default
title: Home
---

<div class="home-intro">

<div class="home-text">

## About the Lab

Our lab investigates fundamental and applied problems in mechanics, wave physics, and multiphysics systems.
We combine theoretical modeling, numerical simulation, advanced fabrication, and experimental characterization to develop new physical concepts and functional metamaterial systems.

<p>
<a href="mailto:your-email@example.com">Email</a> &nbsp;&nbsp;|&nbsp;&nbsp;
<a href="#">Google Scholar</a> &nbsp;&nbsp;|&nbsp;&nbsp;
<a href="#">ORCID</a>
</p>

</div>

<div class="home-photo">

<img src="/assets/images/profile.jpg" alt="Yi Chen">

</div>

</div>


## News

{% assign news = site.data.news | sort: "date" | reverse %}

{% for item in news limit:5 %}

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
