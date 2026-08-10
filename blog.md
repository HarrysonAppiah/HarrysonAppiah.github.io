---
layout: default
title: "Beyond the Noise"
permalink: /blog/
---

<h2>Research Updates</h2>
<p style="max-width: 700px;">
A space for thinking out loud about society, culture, and the things that often go unnoticed. Through songs, poems, memes, stories, and everyday observations, I explore the contradictions, frustrations, and absurdities of modern life and the questions they leave us asking.

</p>

<hr>

{% for post in site.posts %}
  <div style="margin-bottom: 35px;">

    <h3 style="margin-bottom: 5px;">
      <a href="{{ post.url | relative_url }}" style="text-decoration: none;">
        {{ post.title }}
      </a>
    </h3>

    <div style="font-size: 14px; color: #555;">
      {{ post.date | date: "%B %d, %Y" }}
      {% if post.tags %}
        • 
        {% for tag in post.tags %}
          <span style="background:#f2f2f2; padding:2px 6px; margin-right:4px; border-radius:4px;">
            {{ tag }}
          </span>
        {% endfor %}
      {% endif %}
    </div>

    <p style="margin-top: 10px;">
      {{ post.excerpt }}
    </p>

    <div style="margin-top: 8px;">
      <a href="{{ post.url | relative_url }}">Read details →</a>
      {% if post.facebook %}
        | <a href="{{ post.facebook }}" target="_blank">View on Facebook →</a>
      {% endif %}
    </div>

  </div>

  <hr>

{% endfor %}
