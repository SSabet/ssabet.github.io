---
layout: archive
title: "The Macro Notebooks"
permalink: /notebooks/
author_profile: true
entries_layout: grid
---
{% include base_path %}

<div id="notebooks-grid">
    {% assign items = site.notebooks | sort: 'date' %}
    {% for post in items %}
    {% include archive-single.html type="grid" show_meta=false %}
    {% endfor %}
</div>
