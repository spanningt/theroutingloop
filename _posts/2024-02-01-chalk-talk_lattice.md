---
layout: default
title:  "re:Invent 2023 Chalk Talk - Connecting and securing services with Amazon VPC Lattice"
videoid: 
date:   2024-02-01 10:30:00 -0800
abstract: "Amazon VPC Lattice helps you connect your applications and services securely and simplifies the way microservices communicate in a multi-account and multi-virtual private cloud (VPC) environment. In this chalk talk, learn how you can connect your Amazon EC2, Amazon EKS, Amazon ECS, or AWS Lambda microservices whether they are on AWS or on premises. Explore common use cases like multiple account/VPC connectivity, service-to-service authentication and authorization, load balancing, blue-green/canary deployments, and more. Bring your questions."
hosts: "Riggs Goodman III"
guests: "Justin Davies, Principal Product Manager <br> Satish Katpally, Principal Networking Specialist <br> Jamie Wenzel, Principal Solutions Architect ELB"
---
<div class="content-area">
  <span class="date">{{ page.date | date: "%-d %B %Y" }}</span>

  <h1>{{ page.title }}</h1>

  <p><b>Hosts:</b><br>{{ page.hosts }}</p>
  <p><b>Guests:</b><br>{{ page.guests }}</p>
  <div class="abstract">
    <b>Abstract:</b><br>{{ page.abstract }}
  </div>

  {% capture nowunix %}{{'now' | date: '%s'}}{% endcapture %}
  {% capture posttime %}{{page.date | date: '%s'}}{% endcapture %}
  {% if posttime < nowunix %}   
    <div class="video-container">
      <iframe src="https://player.twitch.tv/?video={{ page.videoid }}&parent=www.theroutingloop.net&parent=127.0.0.1&autoplay=false" height="315" width="560" allowfullscreen="" frameborder="0"></iframe>
    </div>
    <a href="https://pulse.aws/survey/6ONETCNV" class="button">Session Feedback/Content Suggestions</a>
  {% else %}
    <p>Session hasn't started. Join live on <b>{{ page.date | date: "%-d %B %Y" }} at 10:30AM PST / 1:30PM EST / 6:30PM GMT</b></p>
    <div class="video-container">
      <iframe src="https://player.twitch.tv/?channel=aws&parent=www.theroutingloop.net&parent=127.0.0.1&autoplay=false" height="315" width="560" allowfullscreen="" frameborder="0"></iframe>
    </div>
  {% endif %}

  {% if page.videoid == null %}
    <b>Video on demand will become available soon after the livestream</b>
  {% endif %}
</div>
