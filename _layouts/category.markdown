---
layout: page
type: archive
---

<ul>
  {% assign sortednotes = site.notes | sort: 'date' | reverse %}
  {% for note in sortednotes %}
   {% if note.category == page.category %}
       <li>
        {% if note.status == "Done" %}
          <h4 style="color:green;margin:0;padding:0">[Done]
        {% elsif note.status == "WIP" %}
          <h4 style="color:orange;margin:0;padding:0">[In-Progress]
        {% else %}
          <h4 style="color:red;margin:0;padding:0">[Stale]
        {% endif %}
          <a href="{{ note.url }}">{{note.title }}</a></h4>
          <b>Short</b>: <i>{{ note.short }}</i><br>
          <b>Last update</b>: <i>{{ note.date | date: "%Y-%B-%d" }}</i>
        </li>
    {% endif % }
    {% endfor %}
    {% endfor %}
</ul>
