---
layout: home
title: Home
---

<section class="hero-section">
  <div class="wrapper">
    <div class="hero-content">
      <h1 class="hero-title">Ralph Warrand</h1>
      <p class="hero-subtitle">Creative Media & Game Technologies Graduate | MSc Computer Science and Engineering Student |  Building the Future of Interactive Entertainment</p>
      <a href="#projects" class="hero-cta">
        <span>Explore My Journey</span>
        <span>↓</span>
      </a>
    </div>
  </div>
</section>

<div class="page-content">
  <div class="wrapper">
    
    <h2>About Me</h2>

    <p>I'm passionate about <strong>game development</strong>, with a particular interest in <strong>graphics programming</strong>. Throughout my studies at <strong>Breda University of Applied Sciences</strong>, I've been exploring various aspects of game development, from programming fundamentals to advanced rendering techniques.</p>

    <h3>My Focus Areas</h3>
    <ul>
      <li><strong>Graphics Programming</strong>: OpenGL, shader development</li>
      <li><strong>Game Engines</strong>: Unity, Unreal Engine, custom engine development</li>
      <li><strong>Programming Languages</strong>: C++, Python, Java, GLSL, HLSL</li>
      <li><strong>Specializations</strong>: Game engine architecture, gameplay programming, and graphics programming</li>
    </ul>

    <section id="projects" class="projects-section">
      <h2 class="section-title">My Learning Journey</h2>
      <p class="section-subtitle">Explore my projects and learning outcomes from my time at Breda University of Applied Sciences and Eindhoven University of Technology</p>
      
      <div class="projects-grid">
        {%- for project in site.projects reversed -%}
          <article class="project-card">
            <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
            <p class="project-period">{{ project.period }}</p>
            <div class="project-tags">
              {%- for tag in project.tags -%}
                <span class="tag">{{ tag }}</span>
              {%- endfor -%}
            </div>
            <p class="project-excerpt">{{ project.content | strip_html | truncatewords: 25 }}</p>
            <a href="{{ project.url | relative_url }}" class="read-more">Read More</a>
          </article>
        {%- endfor -%}
      </div>
    </section>

    <section class="cta-section">
      <h2>Let's Connect</h2>
      <p>Interested in my work or want to collaborate? I'd love to hear from you!</p>
      <a href="{{ 
'/contact/' | relative_url }}" class="cta-button">
        <span>Get In Touch</span>
        <span>✉️</span>
      </a>
    </section>

  </div>
</div>

