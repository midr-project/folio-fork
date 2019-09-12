---
layout: page
title: team
permalink: /team/
---

{% for person in site.team %}
<div class="project">
    <div class="thumbnail">
        <a href="{{ person.link }}" target="_blank">
        {% if person.img %}
        <img class="thumbnail" src="{{ person.img }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}
        <span>
            <h1>{{ person.title }}</h1>
            <br/>
            <p>{{ person.description }}</p>
        </span>
        </a>
    </div>
</div>
{% endfor %}
