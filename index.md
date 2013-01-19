---
layout: page
title: Welcome!
tagline: ""
---
{% include JB/setup %}
<div class="row">
<div class="span9">
<p>
	Welcome to my homepage! I finally decided to set up a web presence. After doing some research on how to go about this, I settled on Jekyll, Jekyll-Bootstrap on Github pages.
</p>
</div>
<div class="span3">
	<img src="{{ ASSET_PATH }}images/Profile.jpg">
</div>


<h3>Posts</h3>

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
</div>