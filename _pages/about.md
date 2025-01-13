---
permalink: /
title: "Welcome"
excerpt: "Portfolio Website"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hello! This is Donghyeon Shin's website. Here, you will be able to review a brief portfolio and CV about me. 

<!-- <div class="content-container">
  <img src="images/20241115_161350(1).jpg" alt="profile">
</div> -->

I am a master student in AI Graduate School at GIST AI Data Science lab with [Prof. Sundong](https://sundong.kim/).


My primary research interests lie in leveraging large language models (LLMs) for natural language processing (NLP) and exploring reinforcement learning (RL). Currently, I am particularly focused on developing AI models aligned with human values. To achieve this, I am investigating methods to construct knowledge graphs from natural language and applying skill-based reinforcement learning approaches grounded in these graphs.

Below, I introduce the projects I worked on during my master’s program.


<!-- <div class="image-grid">
  <img src="images/diagonal-flip.gif" alt="diagonal flip">
  <img src="images/horizontal-align.gif" alt="horizontal align">
  <img src="images/tetris.gif" alt="tetris">
</div> -->


<hr style="height:1px; border:none; background-color:#e5e5e5;">

{% include base_path %}

# Publications
{% for post in site.publications reversed %}
  {% if post.type != "domestic-conference" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

# Domestic Conference
{% for post in site.publications reversed %}
  {% if post.type == "domestic-conference" %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}