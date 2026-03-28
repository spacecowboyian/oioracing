---
layout: default
title: 2025 Race Results
---

<h1 class="h2 mb-4">2025 Race Results</h1>
<ul class="list-group">
  {% assign events = site.pages | where_exp: "p", "p.dir == '/raceresults/2025/'" | sort: "date" %}
  {% for event in events %}
  {% unless event.name == 'index.md' %}
  <li class="list-group-item">
    <a href="{{ event.url | relative_url }}" class="text-decoration-none">
      {{ event.title }}
    </a>
  </li>
  {% endunless %}
  {% endfor %}
</ul>
