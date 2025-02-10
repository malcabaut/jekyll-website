---
layout: default
title: Equipo
---

# Nuestro Equipo

{% for member in site.team %}
  <div class="team-member">
    <img src="{{ member.photo | relative_url }}" alt="{{ member.name }}">
    <h2>{{ member.name }}</h2>
    <p>{{ member.position }}</p>
    <a href="{{ member.cv | relative_url }}" target="_blank">Ver CV</a>
  </div>
{% endfor %}

