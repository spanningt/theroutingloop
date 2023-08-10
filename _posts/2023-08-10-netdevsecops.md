---
layout: default
title:  "NetDevSecOps, and why it matters"
videoid: 1895319554
date:   2023-08-10 10:30:00 -0800
abstract: "Organizations are moving from traditional monolithic data center networks to an agile application programming interface (API)-driven cloud network. As a result, customers are looking for a secure and automated way to make changes to their cloud network infrastructure. In this session we will cover the modern practices of NetDevSecOps in AWS and how it will benefit organizations to build, configure and manage networks. You will see a live demo on how to inject network security and compliance as part of CI/CD pipelines and perform automated vulnerability management in networking at scale. You will leave this session understanding how to confidently release changes to your network infrastructure while maintaining the highest levels of security, auditing and compliance."
hosts: "Sidhartha Chauhan"
guests: "Shiva Vaidyanathan, Principal Cloud Architect"
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
