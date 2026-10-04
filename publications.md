---
layout: default
title: Publications
---

# Publications

<p class="publication-notice" style="font-size: 0.9em; color: #666; margin-bottom: 2rem;">
  <em>* Corresponding authors &nbsp;&nbsp;|&nbsp;&nbsp; † Equal contributions</em>
</p>

{% assign publications = site.data.publications | sort: "year" | reverse %}

{% assign current_year = "" %}

{% for paper in publications %}

{% if paper.year != current_year %}

## {{ paper.year }}

{% assign current_year = paper.year %}

{% endif %}

<div class="publication">
    <p>
        <strong>{{ paper.title }}</strong>, <em>{{ paper.journal }}</em>, <strong>{{ paper.volumes }}</strong>, {{ paper.pages | split: '-' | first }} ({{ paper.year }}).
        {% if paper.doi %}
        <a href="{{ paper.doi }}" target="_blank">[DOI]</a>
        {% endif %}<br>
        {{ paper.authors }}<br>
    </p>
</div>

{% endfor %}
