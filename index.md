---
layout: default
title: Home
---

<div class="hero-section">
    <h1>Hey, I'm Ashok! 👋</h1>
    <p>
        I'm a software engineer, AI enthusiast, and student. I love building things from scratch and writing about full-stack web development, AI, and my coding journey! 
    </p>
    <div class="hero-links">
        <a href="/about.html">👤 About Me</a>
        <a href="/projects.html">💻 Projects</a>
    </div>
</div>
---
<div class="posts-section">
    <h2>📝 Latest Posts</h2>
    <div class="latest-posts">
        {% for post in site.posts limit:5 %}
        <div class="post-item">
            <span class="post-date">{{ post.date | date: "%B %d" }}</span>
            <a href="{{ post.url }}">{{ post.title }}</a>
        </div>
        {% endfor %}
    </div>
    <div>
        <a href="/blog.html">View all posts →</a>
    </div>
</div>
---
<div class="projects-section">
    <h2>💻 Featured Projects</h2>
    <div class="project-wrapper">
        <a href="" target="_blank" class="project-card">
            <h3>📘 Try Jekyll</h3>
            <p>A custom developer blog built entirely from scratch without pre-made themes.</p>
        </a>
        <a href="#" class="project-card">
            <h3>🤖 TableSense AI</h3>
            <p>A web application project built for extracting structured data from PDF tables.</p>
        </a>
    </div>
</div>
