---
layout: default
title: Courses
---

# Courses

{% assign courses = site.data.courses
   | sort: "year"
   | reverse %}

{% for course in courses %}

<div class="card">

<h3>
{{ course.title }}
</h3>

<p>
<strong>
{{ course.year }}
</strong>
|
{{ course.semester }}
</p>

<p>
{{ course.description }}
</p>

</div>

{% endfor %}
