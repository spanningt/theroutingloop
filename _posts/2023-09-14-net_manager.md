---
layout: default
title:  "AWS Network Manger: Centralize management and monitoring of networking resource"
videoid: 1925430811
date:   2023-09-14 10:30:00 -0800
abstract: "In this session we will provide an overview of AWS Network Manager and discuss in detail how customers can leverage Network Manager for monitoring their Transit Gateways (TGWs). We will walk through a demo of how to register and visualize your TGWs in Network Manager as well as configure (TGW) events via Network Manager for monitoring/troubleshooting purposes. We will also cover how Route Analyzer can be utilized to perform an analysis of the routes in your transit gateway route tables. "
hosts: "Sidhartha Chauhan"
guests: "Ankush Goyal, Senior Technical Account Manager <br> Nishant Kumar, Senior Product Manager "
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
