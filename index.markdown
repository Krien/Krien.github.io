---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
list_title: ' '
years:
  - 2024
  - 2023
---


<h2> Selected Publications </h2>
<h3><a href="./publications" style="color:#0089cf"> Click here to see all publications</a></h3>
<ul style="list-style-type: none;">
  {% assign sortedpublications = site.publications | sort: 'date' | reverse %}
  {% for year in page.years %}
    <h3> {{ year }} </h3>
    {% for publication in sortedpublications %}
        {% capture pubyear %}{{ publication.date | date: "%Y" }}{% endcapture %}
        {% if publication.status == "Done" and pubyear contains year and (publication.type == "conference" or publication.type == "workshop") and publication.selected  %}
            <li style="margin-top: 10px; margin-bottom: 10px;">
            {{ publication.authors }} ({{ publication.date | date: "%Y %B" }})<br>
            <a href="{{ publication.url }}" style="color:#0089cf">{{ publication.title }}</a> <br>
            <i style="color:#868e96">{{ publication.conference }}</i> <br>
            </li>
        {% endif %}
    {% endfor %}
  {% endfor %}
</ul>

<h2> Teaching and Supervision </h2>

I am looking for students to supervise that are interested in storage systems. I have topics regarding performance analysis, QoS tracing and LSM-trees.

I am a teaching assistant for (coordinating roles):
<ul>
    <li> <a href="https://research.vu.nl/en/courses/systems-seminar-2"> System Seminar (MSc)</a>: Teaching students how to read <i>and</i> review systems papers and how to run/evaluate systems artifacts; 2022--</li>
    <li> <a href="https://atlarge-research.com/courses/storage-systems-vu/"> Storage Systems (MSc)</a>: Teaching students how to design, implement and evaluate storage systems (they implement an FTL, GC algorithm and FS); 2023</li>
    <li> <a href="https://research.vu.nl/en/courses/advanced-network-programming-2"> Advanced Network Programming (BSc)</a>: Teaching students how to design, implement and evaluate network stacks (among others they implement ICMP and TCP in user-space); 2023--</li>
</ul>
