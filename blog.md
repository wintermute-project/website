---
layout: page
title: Blog
permalink: /blog/
nav_order: 10
nav_display: 1
---

<div class="posts">

{% for post in site.posts %}
    <div class="post">
        <div class="post-img" style="float:left;">
            <a href="{{ post.url }}"><img src="{{ post.img }}" alt="{{ post.img-alt }}"/></a>
        </div>
        <div class="post-text" style="float:left">
            <div class="post-text-title"><a href="{{ post.url }}">{{ post.title }}</a></div>
            <div class="post-text-abstract">{{ post.excerpt }}</div>
        </div>
        <div style="clear: both"/>        
    
    </div>

{% endfor %}

</div>
