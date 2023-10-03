---
layout: default
title:  "Insights into Internet woes and application performance using CloudWatch Internet Monitor"
videoid: 
date:   2023-10-19 10:30:00 -0800
abstract: "Organizations looking to provide superior digital experiences to their users need to monitor these digital experiences proactively. In this session, you will learn more about Amazon CloudWatch Internet Monitor capabilities and roadmap that help you continuously monitor internet performance metrics, such as availability and performance between your AWS-hosted applications and application end users. Explore how you can visualize impact, pinpoint the geographic locations and providers that are impacted, and take actions as an application developer or network engineer to improve your end users’ network experience."
hosts: "Alexandra Huides"
guests: "Subbu Mahadevan, Senior Manager, Technical Product Management, Network Availability"
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
