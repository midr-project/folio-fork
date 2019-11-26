---
layout: page
title: publications
permalink: /publications/
---

<ul class="post-list">
{% for pub in site.publications reversed %}
<li>
<div class="publication-grid-container">
<div class="publication-grid-img">
<div class="publication-thumbnail">
<img src="{{ pub.img }}"/>
</div>
</div>
<div class="publication-grid-body">
<h4>
<a class="poem-title" href="{{ pub.link }}" target="_blank">{{ pub.title }}</a>
</h4>
{% if pub.description %}
<p class="post-description" style="text-align: justify; padding: 10px;">{{ pub.description }}</p>
<p class="post-meta-important" style="text-align: left; ">{{ pub.authors }}</p>
<p class="post-meta" style="text-align: left; ">{{ pub.venue }}</p>
{% else %}
<p class="post-meta-important" style="text-align: left; padding-top: 5px;">{{ pub.authors }}</p>
<p class="post-meta" style="text-align: left; ">{{ pub.venue }}</p>
<p class="post-meta" style="text-align: left; ">[ <a style="color: #282828;" class="poem-title" href="{{ pub.link }}" target="_blank"><i class="fa fa-file-pdf-o" aria-hidden="true"></i> pdf </a> ] 
</p>
</div>
</div>
{% endif %}
</li>
{% endfor %}
</ul>