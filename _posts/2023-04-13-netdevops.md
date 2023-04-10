---
layout: default
title:  "TBC - Last minute speaker change"
videoid: 
date:   2023-04-13 10:30:00 -0800
abstract: "Details of the session will be confirmed soon"
hosts: "Sidhartha Chauhan"
guests:
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
