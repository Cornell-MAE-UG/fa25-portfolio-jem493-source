---
layout: default
title: Jacob Miller - Portfolio
permalink: /projects/
---

<div class="gallery-container">
<div class="project-gallery">
    {% for project in site.projects %}
    <div class="gallery-item">
        <a href="{{ project.url | relative_url }}">
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" />
        <p>{{ project.title }}</p>
        </a>
    </div>
    {% endfor %}
</div>
</div>

<div style="text-align: center; margin-top: 40px;">
    <h3>MAE 3270 Final HW</h3>
    <a href="{{ '/assets/FPW.pdf' | relative_url }}" target="_blank" style="font-size: 1.2em; font-weight: bold;">
        Download FPW (PDF)
    </a>
</div>
