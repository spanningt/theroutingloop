---
layout: default
title:  "Introduction to NetDevSecOps"
videoid: 
date:   2023-04-13 10:30:00 -0800
abstract: "In this session, come learn about the concept of NetDevSecOps and the key considerations that are required to be kept in mind when operating at scale. We will cover the architectural patterns, services and features, learnings that can be leveraged by you and an end-to-end demonstration of NetDevSecOps in practice"
hosts: "Sidhartha Chauhan"
guests: Shiva Vaidyanathan, Principal Cloud Architect "
---
{{ page.date | date: "%-d %B %Y" }}

<h1> {{ page.title}} </h1>

<p><b> Hosts: </b> <br> {{ page.hosts }}  </p>
<p><b> Guests: </b> <br> {{ page.guests }}  </p>
<p> <b> Abstract: </b> <br> {{page.abstract}} </p>



{% capture nowunix %}{{'now' | date: '%s'}}{% endcapture %}
{% capture posttime %}{{page.date | date: '%s'}}{% endcapture %}
{% if posttime < nowunix %}   
<div class="video-container">
    <iframe src="https://player.twitch.tv/?video={{ page.videoid }}&parent=www.theroutingloop.net&parent=127.0.0.1&autoplay=false" height="315" width="560" allowfullscreen="" frameborder="0">
    </iframe>
</div>
 
{% else %}
<p>Session hasn't started. Join live on <b>{{ page.date | date: "%-d %B %Y" }} at 10:30AM PST / 1:30PM EST / 6:30PM GMT  </b><p>
<div class="video-container">
    <iframe src="https://player.twitch.tv/?channel=aws&parent=www.theroutingloop.net&parent=127.0.0.1&autoplay=false" height="315" width="560" allowfullscreen="" frameborder="0">
    </iframe>
</div>
{% endif %}


{% if page.videoid == null %}
<b> Video on demand will become available soon after the livestream </b>
{% endif %}
