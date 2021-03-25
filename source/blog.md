---
html_title: Blog
layout:     page
permalink:  /blog/
style-id:   blog-index
title:      Stuff I Wrote
---

{% for post in site.posts %}

{% assign post_year = post.date | date: "%Y" %}
{% if post_year != list_year %}
  {% unless forloop.first %}</ul>{% endunless %}
  {% assign list_year = post_year %}
  <h4 id="year-{{ list_year }}" class="year">{{ post_year }}</h4>
  <ul class="post-list">
{% endif %}

<li>
  {% include post-preview.html post=post elements="date title" %}
</li>

{% if forloop.last %}</ul>{% endif %}

{% endfor %}

<!-- Offsite Articles -->
<h4>Articles for the Toptal Engineering Blog</h4>
<ul class="post-list">
  <li>
    <div class="post-preview">
    <a target="_blank" href="https://www.toptal.com/machine-learning/machine-learning-theory-an-introductory-primer#obtain-only-eye-opening-engineers">
      <p class="post-title">Machine Learning Tutorial</p>
    </a>
    </div>
  </li>

  <li>
    <div class="post-preview">
    <a target="_blank" href="https://www.toptal.com/robotics/programming-a-robot-an-introductory-tutorial#obtain-only-eye-opening-engineers">
      <p class="post-title">Robot Programming Tutorial</p>
    </a>
    </div>
  </li>
</ul>
