---
layout: page
title: Publications
permalink: /publications/
years:
  - 2024
  - 2023
  - 2022
---

<ul style="list-style-type: none;">
  {% assign sortedpublications = site.publications | sort: 'date' | reverse %}
  {% for year in page.years %}
    <h3> {{ year }} </h3>
    {% for publication in sortedpublications %}
        {% capture pubyear %}{{ publication.date | date: "%Y" }}{% endcapture %}
        {% if publication.status == "Done" and  pubyear contains year %}
        <li style="margin-top: 20px; margin-bottom: 20px;">
          {{ publication.authors }} ({{ publication.date | date: "%Y %B" }})<br>
          <a href="{{ publication.url }}" style="color:#0089cf">{{ publication.title }}</a> <br>
          <i style="color:#868e96">{{ publication.conference }}</i> <br>
        </li>
        {% else %}
        {% endif %}
    {% endfor %}
  {% endfor %}
</ul>
