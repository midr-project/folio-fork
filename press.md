---
layout: page
title: press
permalink: /press/
---

  <ul style="margin-left: 30px;">
      {% for item in site.data.press %}
        <li>
          <p class="press-item"><strong>{{ item.title }}</strong>, {{ item.where }}, {{ item.date | date: '%B %-d %Y' }}, <a class="press-item" href="{{ item.original-url }}" target="_blank"><strong>URL</strong></a></p>
        </li>
      {% endfor %}
  </ul>
