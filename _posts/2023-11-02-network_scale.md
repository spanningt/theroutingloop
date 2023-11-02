---
layout: default
title:  "Designing AWS networks for growth and scale "
videoid: 
date:   2023-11-02 10:30:00 -0800
abstract: "As companies grow, their AWS network architectures need to evolve to accommodate increasing traffic, security needs, and complexity. This session will provide strategies and best practices for designing scalable, secure, and highly available AWS networks. We will discuss how to design VPCs, subnets, route tables, security groups, and other components to allow for future growth. Topics will include choosing the right VPC topology, connecting VPCs and hybrid networks with AWS Transit Gateway, AWS Cloud WAN, building hub-and-spoke models, and integrating network security tools. Attendees will learn how to assess current workloads and plan network changes to support growth over time. The session will cover options for scaling up network capacity, segmenting resources, and automating network management tasks. Architects, network administrators, and cloud practitioners looking to design future-ready AWS networks that can evolve smoothly will find practical takeaways."
hosts: "Sidhartha Chauhan & Tom Adamski"
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
