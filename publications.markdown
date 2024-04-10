---
layout: page
title: Publications
permalink: /publications/
years:
  - 2024
  - 2023
  - 2022
---
<link rel="icon" href="{{ "./favicon-32x32.png" | relative_url }}" type="image/x-icon">

<ul style="list-style: none; padding-left: 0;display:table-row;">
  {% assign sortedpublications = site.publications | sort: 'date' | reverse %}
  {% for year in page.years %}
    <h3> {{ year }} </h3>
    <ul style="list-style-type: none;">
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
    </ul>
  {% endfor %}
</ul>
