---
layout: page
title: Home
id: home
permalink: /
---

# Hi and welcome!

## I'm [[cbt|Charlie]]. This blog is meant as a place for me to think out loud, ponder with friends, and build an archive of personal knowledge.

If you're curious about the conceptual underpinnings of this blog, check out my note about the phenomenon of [[Digital Gardens]]. The basic gist is:
- notes are not organized chronologically
- many of the notes you find may be incomplete
- you can use links within the notes to navigate to other notes

If you're looking for a specific (or a non-specific) note, check below:

# Map of the garden so far:
<div class="key">
<b>Key:</b><div class="seedy chonk"><span class="key-label">Seeds</span></div>
<div class="greenie chonk"><span class="key-label">Sprouts</span></div>
<div class="fruity chonk"><span class="key-label">Fruit</span></div>
</div> 

{% include notes_graph.html %}

<!-- # Notes I've worked on recently: -->
<!-- <div>
{% capture now_time %} {{'now' | date: "%s"}} {% endcapture %}
{% assign now_time_no = now_time | minus: 604800 %}
{% assign notes = site.notes | sort: "last_modified_at" | reverse %}
{% for note in notes %}
{% capture note_time %} {{note.last_modified_at | date: "%s"}} {% endcapture %}
{% assign note_time_no = note_time | plus: 0 %}
{% if note_time_no <= now_time_no %}
	{% break %}
{% else %}
 <a href="{{note.url}}" class="internal-link">{{note.title}}</a> <span style="color: grey"> - {{note.last_modified_at | date: "%b %d"}}</span><br>
{% endif %}
{% endfor %}
</div> -->

<!-- <div>
{% assign notes = site.notes | sort: "last_modified_at" | reverse %}
{% for note in notes %}
<a href="{{note.url}}" class="internal-link">{{note.title}}</a> <span style="color: grey"> - {{note.last_modified_at | date: "%b %d"}}</span><br>
{% endfor %}
</div> -->

<!-- <style>
  .wrapper {
    max-width: 46em;
  }
  .bord-it-up {
  	border-style: solid;
  	border-width: 2px;
  	border-color: #941c2f;
  }
</style> -->
