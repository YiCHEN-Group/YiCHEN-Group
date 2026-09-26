---
layout: default
title: Team
---

# Team

## Principal Investigator

{% for person in site.data.team %}
{% if person.position == "Principal Investigator" %}

<div class="card">

{% if person.photo %}
<img src="{{ person.photo }}"
     style="width:160px;height:160px;object-fit:cover;">
{% endif %}

<h3>
{{ person.name }}
</h3>

<p>
<strong>{{ person.position }}</strong>
</p>

<p>
{{ person.research }}
</p>

{% if person.email %}
<p>
Email:
<a href="mailto:{{ person.email }}">
{{ person.email }}
</a>
</p>
{% endif %}

</div>

{% endif %}
{% endfor %}


## Researchers and Students

{% for person in site.data.team %}
{% unless person.position == "Principal Investigator" %}

<div class="card">

{% if person.photo %}
<img src="{{ person.photo }}"
     style="width:140px;height:140px;object-fit:cover;">
{% endif %}

<h3>
{{ person.name }}
</h3>

<p>
<strong>{{ person.position }}</strong>
</p>

<p>
{{ person.research }}
</p>

</div>

{% endunless %}
{% endfor %}
