---
layout: default
permalink: /upcoming/
---

## Upcoming episodes

<ul>
  {% for post in site.posts %}
    {% capture nowunix %}{{'now' | date: '%s'}}{% endcapture %}
    {% capture posttime %}{{post.date | date: '%s'}}{% endcapture %}
    {% if posttime > nowunix %}
      <li>
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        {{ post.excerpt }}

      </li>
      {% endif %}
  {% endfor %}
</ul>
