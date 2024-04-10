---
layout: page
title: Awards
permalink: /awards/
---
<link rel="icon" href="{{ "./favicon-32x32.png" | relative_url }}" type="image/x-icon">

<ul>
  {% assign sortedawards = site.awards | sort: 'date' | reverse %}
  {% for award in sortedawards %}
    <li>
      <h3><a href="{{ award.url }}">{{ award.title }}</a></h3>
      <b> {{ award.date | date: "%Y %B" }} </b><br>
      <i>{{ award.short }}</i>
    </li>
  {% endfor %}
</ul>
