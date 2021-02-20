---
layout: page
title: Navigating the Garden
permalink: /nav
---

> You've found a little secret!

# Notes organized by done-ness

<hr>

## Seeds - the very starts of ideas

<div>
	{% for note in site.notes %}
		{% if note.status == "seed" %}
			🌱 <a href="{{note.url}}" class="internal-link">{{note.title}}</a><br>
		{% endif %}
	{% endfor %}
</div>

## Growing - WIPs

<div>
	{% for note in site.notes %}
		{% if note.status == "growing" %}
			🌿 <a href="{{note.url}}" class="internal-link">{{note.title}}</a><br>
		{% endif %}
	{% endfor %}
</div>

## Fruit - "finished" notes

<div>
	{% for note in site.notes %}
		{% if note.status == "fruit" %}
			🍊 <a href="{{note.url}}" class="internal-link">{{note.title}}</a><br>
		{% endif %}
	{% endfor %}
</div>

## Branches - ever growing

<div>
	{% for note in site.notes %}
		{% if note.status == "branch" %}
			🌳 <a href="{{note.url}}" class="internal-link">{{note.title}}</a><br>
		{% endif %}
	{% endfor %}
</div>

## Flowers - small finished notes

<div>
	{% for note in site.notes %}
		{% if note.status == "flower" %}
			🌸 <a href="{{note.url}}" class="internal-link">{{note.title}}</a><br>
		{% endif %}
	{% endfor %}
</div>
