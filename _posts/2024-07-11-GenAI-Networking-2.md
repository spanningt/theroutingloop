---
layout: default
title:  "Supercharge Your Network Engineering: Harnessing GenAI Tools for Enhanced Productivity"
videoid: 
date:   2024-07-11 10:30:00 -0800
abstract: "Discover how generative AI is revolutionizing the daily work of network engineers. Tune in to learn how to leverage cutting-edge AI assistants to boost your productivity and streamline complex tasks such as: <br><br> 1) RAG-Powered Knowledge Basics: Enhancing your troubleshooting with AI that understands network contexts. <br> 2) Amazon Bedrock Agents: Creating your personal AI network assistant for faster problem solving. <br> 3) Amazon Q Developer: Accelerating NetDevOps workflows and automating code generation."
hosts: "Jamie"
guests: " Du'An Lightfoot, Sr. Developer Advocate <br> Sid Chauhan, Principal Solutions Architect"
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