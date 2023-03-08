---
layout: default
title:  "Advanced VPC design, and Application Architectures"
videoid: 1747798356
date:   2023-02-23 10:30:00 -0800
abstract: "Jamie and Matt cover advanced VPC architectures and basics of VPC networking."
hosts: "Jamie Wenzel, Matt Lehwess"
guests: ""
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
