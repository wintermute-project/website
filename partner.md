---
layout: page
title: Partner
permalink: /partner/
nav_order: 30
nav_display: 1
---

<ul class="partners">

{% for partner in site.data.partners %}
    <li>
        <a href="{{partner.url}}"><img src="{{partner.logo}}" alt="{{partner.logo-alt}}" /></a>
        {{partner.name}}<br>
        <a href="{{partner.url}}">{{partner.url | replace: "http://", "" | replace: "https://", ""}}</a>
    </li>
{% endfor %}

</ul>
