---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
list_title: ' '
years:
  - 2024
  - 2023
---
<link rel="icon" href="{{ "./favicon-32x32.png" | relative_url }}" type="image/x-icon">

<h2> Bio </h2>
I am a PhD student in Computer Science at the <a href="https://www.vu.nl/en">Vrije Universiteit Amsterdam (VU)</a> and part of the Massivizing Computer Systems group ([AtLarge](https://atlarge-research.com/kdoekemeijer/)).
I am also a part of [StoNet-research](https://stonet-research.github.io/). My research area is scheduling storage and networked systems.

<h2> Selected Publications </h2>
<h3>Click <a href="./publications" style="color:#0089cf"> here </a> to see all publications</h3>
<ul style="list-style: none; padding-left: 0;display:table-row;">
  {% assign sortedpublications = site.publications | sort: 'date' | reverse %}
  {% for year in page.years %}
    <ul style="list-style-type: none;">
    {% for publication in sortedpublications %}
        {% capture pubyear %}{{ publication.date | date: "%Y" }}{% endcapture %}
        {% if publication.status == "Done" and pubyear contains year and publication.selected %}
            <li style="margin-top: 10px; margin-bottom: 10px;">
                <b><a href="{{ publication.pdf }}" style="color:#0089cf">{{ publication.title }}</a></b> <br>
                {% for author in publication.authors %}
                  {% if author == "Krijn Doekemeijer" %}
                    <u>{{ author -}}</u>{% unless forloop.last -%},{% endunless %}
                  {% else %}
                    {{ author -}}{% unless forloop.last -%},{% endunless %}
                  {% endif %}
                {% endfor %}
                ({{ publication.date | date: "%Y %B" }}) <br>
                <i style="color:#868e96">{{ publication.conference }}</i> <br>
                {% if publication.other != "" %}
                  <b> {{ publication.other }} </b><br>
                {% endif %}
                <div style="word-space: 10px;">
                  {% if publication.pdf %}
                    <a href="{{ publication.pdf }}" style="color:#009988">PDF</a>
                  {% endif %}
                  {% if publication.code %}
                    <a href="{{ publication.code }}" style="color:#009988">Code</a>
                  {% endif %}
                  <a href="{{ publication.url }}" style="color:#009988">More</a>
                </div>
            </li>
        {% endif %}
    {% endfor %}
    </ul>
  {% endfor %}
</ul>
