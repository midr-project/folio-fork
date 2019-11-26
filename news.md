---
layout: page
title: news
permalink: /news/
---

<div class="news-grid" style="padding-top: 25px; display: grid; column-gap: 16px; grid-template-columns: fit-content(250px) auto;">
  {% for new in site.news reversed %}
    <div style="grid-column-start: 1;grid-column-end: 2;">
        <strong>{{ new.date | date: '%B, %Y' }}</strong>
    </div>
    <div style="grid-column-start: 2;grid-column-end: 3; ">
        {{ new.description }}
    </div>
  {% endfor %}
</div>
