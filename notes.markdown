---
layout: page
title: Notes
permalink: /notes/
---
<link rel="icon" href="{{ "./favicon-32x32.png" | relative_url }}" type="image/x-icon">

<ul>
  {% for category in site.categories %}
        <li>
          <h3 style="padding:0;margin:0"><a href="{{ category.url }}">{{category.title }}</a></h3>
          <b>Description</b>: <i>{{ category.description }}</i><br>
        </li>
    {% endfor %}
</ul>
