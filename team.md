---
layout: page
title: team
permalink: /team/
---

{% for person in site.team %}
<div class="team">
    <div class="thumbnail">
        <a href="{{ person.link }}" target="_blank">
        {% if person.img %}
        <img class="thumbnail" src="{{ person.img }}"/>
        {% else %}
        {% endif %}
        <span>
            <h1>{{ person.title }}</h1>
            <br/>
            <p>{{ person.description }}</p>
        </span>
        </a>
    </div>
    <h1 style="margin-top: 5px;">{{ person.title }}</h1>
    <p style="margin-top: 5px;">{{ person.role }}</p>
</div>
{% endfor %}
