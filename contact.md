---
layout: default
title: Contact
permalink: /contact/
---

<div class="page-content">
  <div class="wrapper">
    
    <div class="contact-hero">
      <h1 class="contact-title">Let's Connect</h1>
      <p class="contact-subtitle">Ready to collaborate, discuss game development, or explore opportunities? I'd love to hear from you!</p>
    </div>

    <div class="contact-grid">
      
      <div class="contact-info">
        <h2>Get In Touch</h2>
        <p>Whether you're interested in my work, have a project in mind, or just want to chat about game development and graphics programming, feel free to reach out through any of these channels:</p>
        
        <div class="contact-methods">
          <a href="mailto:contact@ralphwarrand.dev" class="contact-method">
            <div class="contact-icon">✉️</div>
            <div class="contact-details">
              <h3>Email</h3>
              <p>contact@ralphwarrand.dev</p>
              <span>Best for detailed discussions</span>
            </div>
          </a>
          
          <a href="https://linkedin.com/in/ralphwarrand" target="_blank" rel="noopener" class="contact-method">
            <div class="contact-icon">💼</div>
            <div class="contact-details">
              <h3>LinkedIn</h3>
              <p>linkedin.com/in/ralphwarrand</p>
              <span>Professional networking</span>
            </div>
          </a>
          
          <a href="https://github.com/ralphwarrand" target="_blank" rel="noopener" class="contact-method">
            <div class="contact-icon">💻</div>
            <div class="contact-details">
              <h3>GitHub</h3>
              <p>github.com/ralphwarrand</p>
              <span>Check out my code</span>
            </div>
          </a>
        </div>
      </div>

      <div class="contact-form-section">
        <h2>Quick Message</h2>
        <p>Prefer to send a message directly? Use the form below and I'll get back to you as soon as possible.</p>
        
        <form class="contact-form" action="https://formspree.io/f/xpzgkqpv" method="POST">
          <div class="form-group">
            <label for="name">Name</label>
            <input type="text" id="name" name="name" required>
          </div>
          
          <div class="form-group">
            <label for="email">Email</label>
            <input type="email" id="email" name="email" required>
          </div>
          
          <div class="form-group">
            <label for="subject">Subject</label>
            <select id="subject" name="subject" required>
              <option value="">Select a topic...</option>
              <option value="collaboration">Collaboration Opportunity</option>
              <option value="project">Project Discussion</option>
              <option value="internship">Internship/Job Opportunity</option>
              <option value="feedback">Portfolio Feedback</option>
              <option value="general">General Inquiry</option>
              <option value="other">Other</option>
            </select>
          </div>
          
          <div class="form-group">
            <label for="message">Message</label>
            <textarea id="message" name="message" rows="6" placeholder="Tell me about your project, question, or how we might work together..." required></textarea>
          </div>
          
          <button type="submit" class="submit-button">
            <span>Send Message</span>
            <span>🚀</span>
          </button>
        </form>
      </div>
      
    </div>

    <div class="contact-cta">
      <h2>About My Work</h2>
      <p>I'm currently focused on <strong>graphics programming</strong> and <strong>game engine development</strong>, with particular interests in:</p>
      <div class="interests-grid">
        <div class="interest-item">
          <h3>🎮 Game Development</h3>
          <p>Building interactive experiences with modern game engines and custom tools</p>
        </div>
        <div class="interest-item">
          <h3>🎨 Graphics Programming</h3>
          <p>DirectX 12, OpenGL, shader development, and rendering optimization</p>
        </div>
        <div class="interest-item">
          <h3>⚡ Performance Optimization</h3>
          <p>Low-level programming, memory management, and system architecture</p>
        </div>
        <div class="interest-item">
          <h3>🤝 Team Collaboration</h3>
          <p>Agile development, technical leadership, and cross-disciplinary communication</p>
        </div>
      </div>
    </div>

  </div>
</div>

<style>
.contact-hero {
  text-align: center;
  margin-bottom: 4rem;
  padding: 2rem 0;
}

.contact-title {
  font-size: 3rem;
  font-weight: 700;
  color: var(--text-primary);
  margin-bottom: 1rem;
  background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.contact-subtitle {
  font-size: 1.25rem;
  color: var(--text-secondary);
  max-width: 600px;
  margin: 0 auto;
  line-height: 1.6;
}

.contact-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 4rem;
  margin-bottom: 4rem;
}

.contact-info h2,
.contact-form-section h2 {
  font-size: 1.75rem;
  font-weight: 600;
  color: var(--text-primary);
  margin-bottom: 1rem;
}

.contact-info p,
.contact-form-section p {
  color: var(--text-secondary);
  line-height: 1.6;
  margin-bottom: 2rem;
}

.contact-methods {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.contact-method {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 1.5rem;
  background: var(--bg-secondary);
  border: 1px solid var(--border-color);
  border-radius: var(--border-radius);
  text-decoration: none;
  color: var(--text-primary);
  transition: var(--transition);
}

.contact-method:hover {
  background: var(--primary-color);
  color: white;
  transform: translateY(-2px);
  box-shadow: var(--shadow-lg);
}

.contact-icon {
  font-size: 2rem;
  width: 3rem;
  height: 3rem;
  display: flex;
  align-items: center;
  justify-content: center;
  background: var(--bg-primary);
  border-radius: 50%;
  flex-shrink: 0;
}

.contact-method:hover .contact-icon {
  background: white;
}

.contact-details h3 {
  font-size: 1.125rem;
  font-weight: 600;
  margin: 0 0 0.25rem 0;
}

.contact-details p {
  font-size: 0.875rem;
  margin: 0 0 0.25rem 0;
  opacity: 0.8;
}

.contact-details span {
  font-size: 0.75rem;
  opacity: 0.6;
}

.contact-form {
  background: var(--bg-secondary);
  padding: 2rem;
  border-radius: var(--border-radius);
  border: 1px solid var(--border-color);
}

.form-group {
  margin-bottom: 1.5rem;
}

.form-group label {
  display: block;
  font-weight: 600;
  color: var(--text-primary);
  margin-bottom: 0.5rem;
}

.form-group input,
.form-group select,
.form-group textarea {
  width: 100%;
  padding: 0.75rem;
  border: 1px solid var(--border-color);
  border-radius: var(--border-radius);
  font-size: 1rem;
  transition: var(--transition);
  background: var(--bg-primary);
}

.form-group input:focus,
.form-group select:focus,
.form-group textarea:focus {
  outline: none;
  border-color: var(--primary-color);
  box-shadow: 0 0 0 3px rgba(37, 99, 235, 0.1);
}

.submit-button {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.75rem;
  width: 100%;
  background: linear-gradient(135deg, var(--primary-color), var(--primary-dark));
  color: white;
  border: none;
  padding: 1rem 2rem;
  border-radius: var(--border-radius);
  font-size: 1.125rem;
  font-weight: 600;
  cursor: pointer;
  transition: var(--transition);
}

.submit-button:hover {
  transform: translateY(-2px);
  box-shadow: var(--shadow-lg);
}

.contact-cta {
  background: linear-gradient(135deg, var(--bg-secondary) 0%, #e0e7ff 100%);
  padding: 3rem;
  border-radius: var(--border-radius);
  text-align: center;
}

.contact-cta h2 {
  font-size: 2rem;
  font-weight: 700;
  color: var(--text-primary);
  margin-bottom: 1rem;
}

.contact-cta > p {
  color: var(--text-secondary);
  font-size: 1.125rem;
  margin-bottom: 2rem;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
}

.interests-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}

.interest-item {
  background: var(--bg-primary);
  padding: 1.5rem;
  border-radius: var(--border-radius);
  border: 1px solid var(--border-color);
  text-align: left;
}

.interest-item h3 {
  font-size: 1.125rem;
  font-weight: 600;
  color: var(--text-primary);
  margin-bottom: 0.5rem;
}

.interest-item p {
  font-size: 0.875rem;
  line-height: 1.5;
  margin: 0;
}

@media (max-width: 768px) {
  .contact-title {
    font-size: 2.5rem;
  }
  
  .contact-grid {
    grid-template-columns: 1fr;
    gap: 2rem;
  }
  
  .contact-form {
    padding: 1.5rem;
  }
  
  .contact-cta {
    padding: 2rem;
  }
  
  .interests-grid {
    grid-template-columns: 1fr;
  }
}
</style>

