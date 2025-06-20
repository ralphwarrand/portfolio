---
layout: home
title: Home
---

<section class="hero-section">
  <div class="wrapper">
    <div class="hero-content">
      <h1 class="hero-title">Ralph Warrand</h1>
      <p class="hero-subtitle">Creative Media & Game Technologies Student | Graphics Programming Enthusiast | Building the Future of Interactive Entertainment</p>
      <a href="#projects" class="hero-cta">
        <span>Explore My Journey</span>
        <span>↓</span>
      </a>
    </div>
  </div>
</section>

<div class="page-content">
  <div class="wrapper">
    
    ## About Me

    I'm passionate about **game development**, with a particular interest in **graphics programming**. Throughout my studies at **Breda University of Applied Sciences**, I've been exploring various aspects of game development, from programming fundamentals to advanced rendering techniques.

    ### My Focus Areas
    - **Graphics Programming**: DirectX 12, OpenGL, shader development
    - **Game Engines**: Unity, Unreal Engine, custom engine development  
    - **Programming Languages**: C++, C#, HLSL
    - **Specializations**: Rendering systems, game architecture, performance optimization

    ---

    <section id="projects" class="projects-section">
      <h2 class="section-title">My Learning Journey</h2>
      <p class="section-subtitle">Explore my projects and learning outcomes from Year 2 at Breda University of Applied Sciences</p>
      
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
      <a href="{{ '/contact/' | relative_url }}" class="cta-button">
        <span>Get In Touch</span>
        <span>✉️</span>
      </a>
    </section>

  </div>
</div>

