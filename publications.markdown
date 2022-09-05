---
layout: page
title: Publications
permalink: /publications/
---


<ul>
  {% assign sortedpublications = site.publications | sort: 'date' | reverse %}
  {% for publication in sortedpublications %}
    <li>
      {% if publication.status == "Done" %}
      <h3 style="color:green">[Done]
      {% else %}
      <h3 style="color:orange">[In-Progress]
      {% endif %}
      <a href="{{ publication.url }}">{{ publication.title }}</a></h3>
      <b> {{ publication.date | date: "%Y %B" }} - {{ publication.authors }}:</b><br> 
      <i>{{ publication.short }}</i>
    </li>
  {% endfor %}
</ul>
