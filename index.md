---
layout: page
title: Brock Boland
tagline: iOS, Drupal, Chicago
---
{% include JB/setup %}

{% for post in site.posts limit:10 %}
<div class="row-fluid">
  <div class="span12">
	<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <div class="date">
      <span>{{ post.date | date_to_long_string }}</span>
    </div>
    <div class="content">
      {{ post.content }}
    </div>
  </div>
</div>
{% endfor %}
