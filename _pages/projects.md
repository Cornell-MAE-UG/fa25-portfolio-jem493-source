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

<div style="text-align: center; margin-top: 30px;">
    <h3>Other Works</h3>
    <a href="{{ '/assets/SystemsGroupProject.pdf' | relative_url }}" target="_blank">
        View Systems Group Project (PDF)
    </a>
</div>
