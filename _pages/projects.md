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

    <embed src="assets/FPW.pdf" type="application/pdf" width="100%" height="800px" />

<p>
<a href="assets/FPW.pdf" target="_blank">IF PDF VIEW IS NOT WORKING, CLICK HERE TO DOWNLOAD MAE 3270 FINAL HW.</a>
</p>
</div>
