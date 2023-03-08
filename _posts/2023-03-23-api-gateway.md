---
layout: default
title:  "Networking with AWS API Gateway"
videoid:
date:   2023-03-23 10:30:00 -0800
abstract: "We'll go over the networking aspects of AWS API Gateway service. This includes executing the API (from 
the Internet or privately from other VPCs) as well as backend integrations."
hosts: "Tom Adamski"
guests: "Giedrius Praspaliauskas, Senior Solutions Architect specializing in Serverless"
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
    <iframe src="https://player.twitch.tv/?video={{ page.videoid }}&parent=pages.tomadamski.net&parent=127.0.0.1&autoplay=false" height="315" width="560" allowfullscreen="" frameborder="0">
    </iframe>
</div>
 
{% else %}
<p>Session hasn't started. Join live on <b>{{ page.date | date: "%-d %B %Y" }} at 10:30AM PST </b><p>
<div class="video-container">
    <iframe src="https://player.twitch.tv/?channel=aws&parent=pages.tomadamski.net&parent=127.0.0.1&autoplay=false" height="315" width="560" allowfullscreen="" frameborder="0">
    </iframe>
</div>
{% endif %}


{% if page.videoid == null %}
<b> Video on demand will become avaialble soon after livestream </b>
{% endif %}
