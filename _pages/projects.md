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

<object data="{{ '/assets/FPW.pdf' | relative_url }}" type="application/pdf" width="100%" height="800px">
    <p>Unable to display PDF file. <a href="{{ '/assets/FPW.pdf' | relative_url }}">Download</a> instead.</p>
</object>
