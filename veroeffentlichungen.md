---
layout: page
title: Veröffentlichungen
permalink: /veroeffentlichungen/
nav_order: 20
nav_display: 0
---

<ul class="publications">

{% for pub in site.data.publications %}
    <li>{{pub.authors}}<br/><em>{{pub.title}}</em><br/>{{pub.conf}}, {{pub.year}}</li>
{% endfor %}

</ul>
