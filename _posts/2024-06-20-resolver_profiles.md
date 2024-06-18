---
layout: default
title:  "Simplify DNS management using Route 53 Profiles"
videoid: 
date:   2024-06-20 10:30:00 -0800
abstract: "Sharing and managing Route 53 resources and settings across your organization can quickly get complex and costly, as you scale to multiple VPCs and accounts. In this session of the Routing Loop, we will introduce Route 53 Profiles, a new capability that allows you to create a standard DNS configuration that may include one or more Route 53 private hosted zones, Route 53 Resolver DNS Firewall rule groups, and/or Resolver rules, and share the configuration across your VPCs and AWS accounts. Route 53 Profiles simplifies the management and association of Route 53 resources and settings across your organization, by enforcing a consistent configuration."
hosts: "Riggs"
guests: " Adhish Bhobe, Sr. Product Manager <br> Anusha Burla, Sr. Software Dev Engineer"
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
