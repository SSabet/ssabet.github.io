---
layout: archive
title: "The Macro Notebooks"
permalink: /notebooks/
author_profile: true
entries_layout: grid
---
This page contains links to interactive notebooks that I created for (beginning) graduate Macroeconomics course at the LSE (EC413), 2023-2024, with Matthias Doepke and Silvana Tenreyro as lecturers. My students found them extremely useful. Built using the Pluto and PlutoUI packages of Julia ecosystem, these are meant to help students visualise the models, and help them building intuition by enabling them to  do comparative statics (and dynamics) simply by dragging a slider! Interest students can use also reveal the underlying code and use it as a basic intro to Julia and numerical methods in Macroeconomics.

- To see the full notebooks, click on the teaser images, or open the notebook page and click on the link for the full notebook. (takes few minutes to load, look at the status button at the bottom right)
- To see a preview (no interactivity), load the static notebooks.
- There are few half-complete notebooks, aimed at visualising models of business fluctuations and monetary economics, as well as some underlying mathematical concepts such as contraction mapping
- Don't hesitate to reach out if you have feedback on the content, or need some advice on implementing something similar for your course!

{% include base_path %}

<div id="notebooks-grid">
    {% assign items = site.notebooks | sort: 'date' %}
    {% for post in items %}
    {% include archive-single.html type="grid" show_meta=false %}
    {% endfor %}
</div>
