---
layout: default
permalink: /past/
---

## Episode Search

{% include search-form.html %}


----


## Previous episodes

<ul>
  {% for post in site.posts %}
    {% capture nowunix %}{{'now' | date: '%s'}}{% endcapture %}
    {% capture posttime %}{{post.date | date: '%s'}}{% endcapture %}
    {% if posttime < nowunix %}
      <li>
        <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
        <b>{{ post.date | date: "%-d %B %Y" }}</b><br>
        Host(s): {{ post.hosts}}

      </li>
      {% endif %}
  {% endfor %}
</ul>
