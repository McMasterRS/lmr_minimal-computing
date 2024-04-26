---
layout: page
title: Locations
permalink: /locations/
---


<ul id="locations-list">
{% for location in site.data.locations %}
<div class="location-box">
    <p>{{ location.city | split: ', ' | city }},</p>
    <p>{{ location.province | split: ', ' | province }}</p>
    <p>{{ location.postal }}</p>
</div>
{% endfor %}
</ul>