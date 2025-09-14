---
layout: archive
title: "The Macro Notebooks"
permalink: /notebooks/
author_profile: true
entries_layout: grid
---
<div class="nb-intro" markdown="1">
This page contains links to interactive notebooks that I created for (beginning) graduate Macroeconomics course at the LSE (EC413), 2023-2024, with [Matthias Doepke](https://mdoepke.github.io/index.html) and [Silvana Tenreyro](https://personal.lse.ac.uk/tenreyro/) as lecturers. My students found them extremely useful. Built using the [Pluto](https://github.com/fonsp/Pluto.jl) and [PlutoUI](https://github.com/JuliaPluto/PlutoUI.jl) packages of Julia ecosystem, these are mainly meant to help students visualise the models and build intuition by enabling them to do comparative statics (and dynamics) simply by dragging a slider! No knowledge of Julia is required, but interested students can reveal the underlying code and use it as a basic intro to Julia and numerical methods in Macroeconomics.

- To see the full notebooks, dockerised on [Binder](https://mybinder.org/), click on the teaser images, or open the notebook page and click on the link for the full notebook. (takes few minutes to load, look at the status button at the bottom right)
- To see a preview (no interactivity), load the static notebooks.
- There are few half-complete notebooks, related to business fluctuations and monetary economics, as well as some underlying mathematical concepts such as contraction mapping. Stay tuned for updates!
- Don't hesitate to reach out if you have feedback on the content, or need some advice on implementing something similar for your course!
</div>
<br>

{% include base_path %}


<div id="notebooks-grid">
    {% assign items = site.notebooks | sort: 'date' %}
    {% for post in items %}
    {% include archive-single.html type="grid" show_meta=false %}
    {% endfor %}
</div>
