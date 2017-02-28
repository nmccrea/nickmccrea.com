---
layout:     page
permalink:  /blog/
style-id:   blog-index
title:      The Blog
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
  {% include post_preview.html %}
</li>

{% if forloop.last %}</ul>{% endif %}

{% endfor %}