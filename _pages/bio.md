<!-- ---
permalink: /
title: ""
excerpt: ""
author_profile: true
---
<h1>Liu Junming</h1>
{% if page.author_profile or layout.author_profile or page.sidebar %}
  <div class="my-bio">
  {% if page.author_profile or layout.author_profile %}{% include author-profile.html %}{% endif %}
  {% if page.sidebar %}
    {% for s in page.sidebar %}
      {% if s.image %}
        <img src= "{{ s.image }}" alt="{% if s.image_alt %}{{ s.image_alt }}{% endif %}">
      {% endif %}
      {% if s.title %}<h3>{{ s.title }}</h3>{% endif %}
      {% if s.text %}{{ s.text | markdownify }}{% endif %}
    {% endfor %}
  {% endif %}
  </div>
{% endif %} -->