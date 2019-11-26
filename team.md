---
layout: page
title: team
permalink: /team/
---
<div class="team-container-outer">
<div class="team-container">
{% for person in site.team %}
<div class="team-photos">
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
    <h1 class="p-name" style="margin-top: 5px;">{{ person.title }}</h1>
    <p style="margin-top: 5px;">{{ person.role }}</p>
</div>
{% endfor %}
</div>
</div>
<br>
<header class="post-header">
    <h1 class="post-title">past</h1>
    <h5 class="post-description"></h5>
  </header>
<div class="team-container-outer">
<div class="team-container-2">
{% for person in site.past %}
<div class="team-photos">
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
    <h1 class="p-name"  style="margin-top: 5px;">{{ person.title }}</h1>
    <p style="margin-top: 5px;">{{ person.role }}</p>
</div>
{% endfor %}
</div>
</div>
<br>