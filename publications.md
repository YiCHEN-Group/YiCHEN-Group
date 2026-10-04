---
layout: default
title: Publications
---

# Publications

{% assign publications = site.data.publications | sort: "year" | reverse %}

{% assign current_year = "" %}

{% for paper in publications %}

{% if paper.year != current_year %}

## {{ paper.year }}

{% assign current_year = paper.year %}

{% endif %}

<div class="publication">

<p>
<strong>{{ paper.title }}</strong>
</p>

<p>
{{ paper.authors }}
</p>

<p>
<em>{{ paper.journal }}</em>, <strong>{{ paper.volumes }}</strong>, {{ paper.pages | split: '-' | first }} ({{ paper.year }}).
{% if paper.doi %}
<a href="{{ paper.doi }}" target="_blank">[DOI]</a>
{% endif %}
</p>

</div>

{% endfor %}
