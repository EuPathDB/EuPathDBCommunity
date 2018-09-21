---
layout: page
title: Our Staff
---

{% for staff_member in site.staff_members %}
  <h2>{{ staff_member.name }} - {{ staff_member.position }}</h2>
  <p>{{ staff_member.content | markdownify }}</p>
  <img src="{{ staff_member.image_path }}" width="300" height="300"/>
{% endfor %}
