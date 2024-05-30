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

<h2> Publications </h2>

<ul style="list-style: none; padding-left: 0;display:table-row;">
  {% assign sortedpublications = site.publications | sort: 'date' | reverse %}
  {% for year in page.years %}
    <h3> {{ year }} </h3>
    <ul style="list-style-type: none;">
    {% for publication in sortedpublications %}
        {% capture pubyear %}{{ publication.date | date: "%Y" }}{% endcapture %}
        {% if publication.status == "Done" and  pubyear contains year %}
        <li style="margin-top: 20px; margin-bottom: 20px;">
          {{ publication.authors }} ({{ publication.date | date: "%Y %B" }}) {{ publication.other }}
          <br>
          <a href="{{ publication.url }}" style="color:#0089cf">{{ publication.title }}</a> 
          <br>
          <i style="color:#868e96">{{ publication.conference }}</i> <br>
        </li>
        {% else %}
        {% endif %}
    {% endfor %}
    </ul>
  {% endfor %}
</ul>

<h2> Talks </h2>

<ul style="list-style: none; padding-left: 0;display:table-row;">

<h4> Conference </h4>
<ul style="list-style-type: none;">

  <li style="margin-top: 0px; margin-bottom: 20px;">
    Krijn Doekemeijer, Zebin Ren, Nick Tehrany, Animesh Trivedi (2024 April)<br>
    <a href="{{ site.url }}/downloads/talk_zwal_2024.pdf" style="color:#0089cf">Talk - ZWAL: Rethinking Write-ahead Logs for ZNS SSDs with Zone Appends</a><br>
    <i style="color:#868e96">4th Workshop on Challenges and Opportunities of Efficient and Performant Storage Systems (CHEOPS'24) at EuroSys 2024, Athens, Greece</i> <br>
  </li>

  <li style="margin-top: 0px; margin-bottom: 20px;">
    Krijn Doekemeijer, Nick Tehrany, Balakrishnan Chandrasekaran, Matias Bjørling, Animesh Trivedi (2023 November)<br>
    <a href="{{ site.url }}/downloads/talk_cluster_2023.pdf" style="color:#0089cf">Talk - Performance Characterization of NVMe Flash Devices with Zoned Namespaces (ZNS)</a><br>
    <i style="color:#868e96">IEEE CLUSTER'23, Santa Fe, NM, USA</i> <br>
  </li>
</ul>

<h4> Dutch Venues </h4>
<ul style="list-style-type: none;">

  <li style="margin-top: 0px; margin-bottom: 20px;">
    Krijn Doekemeijer, Zebin Ren, Nick Tehrany, Animesh Trivedi (2024 May)<br>
    <a href="{{ site.url }}/downloads/talk_compsys_2024.pdf" style="color:#0089cf">Talk - ZWAL: Rethinking Write-ahead Logs for ZNS SSDs with Zone Appends</a><br>
    <i style="color:#868e96">CompSys'24, Sint michielsgestel, The Netherlands</i> <br>
  </li>

  <li style="margin-top: 20px; margin-bottom: 20px;">
    Krijn Doekemeijer, Nick Tehrany, Balakrishnan Chandrasekaran, Animesh Trivedi (2024 April)<br>
    <a href="{{ site.url }}/downloads/poster_ictopen_2024.pdf" style="color:#0089cf">Poster - Performance Characterization of NVMe Devices with Zoned Namespaces (ZNS)</a><br>
    <i style="color:#868e96">ICT.OPEN'24, Utrecht, The Netherlands</i> <br>
  </li>

  <li style="margin-top: 20px; margin-bottom: 20px;">
    Krijn Doekemeijer, Animesh Trivedi (2023 June)<br>
    <a href="{{ site.url }}/downloads/talk_compsys_2023.pdf" style="color:#0089cf">Talk - TropoDB: Design, Implementation and Evaluation of a KV-Store for Zoned Namespace SSDs</a><br>
    <i style="color:#868e96">CompSys'23, Soesterberg, The Netherlands</i> <br>
  </li>

  <li style="margin-top: 20px; margin-bottom: 20px;">
    Krijn Doekemeijer, Animesh Trivedi (2023 April)<br>
    <a href="{{ site.url }}/downloads/poster_ictopen_2023.pdf" style="color:#0089cf">Poster - TropoDB: Design, Implementation and Evaluation of a KV-Store for Zoned Namespace Devices</a><br>
    <i style="color:#868e96">ICT.OPEN'23, Utrecht, The Netherlands</i> <br>
  </li>
</ul>
</ul>
