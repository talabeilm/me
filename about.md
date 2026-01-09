---
layout: default
title: About
permalink: /about/
---

<section class="about-page">
  <div class="container">
    <div class="about-hero">
      <div class="about-intro">
        <h1 class="page-title">Hello, I'm {{ site.title | default: 'Ademola Oladipo' }}</h1>
        <p class="lead-text">A photographer passionate about capturing authentic moments and telling stories through imagery.</p>
        <div class="about-cta">
          <a href="#contact" class="btn btn-primary">Get In Touch</a>
          <a href="{{ '/portfolio/' | relative_url }}" class="btn btn-outline">View My Work</a>
        </div>
      </div>
    </div>

    <div class="about-bio">
      <div class="bio-content">
        <h2>My Story</h2>
        <p>I'm a visual storyteller with a passion for capturing the beauty in everyday moments. My journey in photography began over a decade ago, and since then, I've dedicated myself to mastering the art of seeing and preserving meaningful moments.</p>
        
        <p>My approach combines technical expertise with emotional intuition, allowing me to create images that not only document but also evoke feeling and tell compelling stories. Whether working on personal projects or client commissions, I strive to bring authenticity and artistic vision to every frame.</p>

        <p>When I'm not behind the camera, you can find me exploring new locations, experimenting with different photographic techniques, or sharing my knowledge through workshops and writing.</p>
      </div>
      
      <div class="bio-highlights">
        <div class="highlight-item">
          <div class="highlight-number">8+</div>
          <div class="highlight-text">Years Experience</div>
        </div>
        <div class="highlight-item">
          <div class="highlight-number">200+</div>
          <div class="highlight-text">Projects Completed</div>
        </div>
        <div class="highlight-item">
          <div class="highlight-number">15+</div>
          <div class="highlight-text">Countries Explored</div>
        </div>
      </div>
    </div>

    <!-- Services Section -->
    <div class="about-services">
      <h2>Services & Specialties</h2>
      <div class="services-grid">
        <div class="service-card">
          <div class="service-icon">📷</div>
          <h3>Portrait Photography</h3>
          <p>Professional portrait sessions that capture personality and emotion in a natural, authentic way.</p>
        </div>
        
        <div class="service-card">
          <div class="service-icon">🏙️</div>
          <h3>Street Photography</h3>
          <p>Candid urban photography that documents life and tells stories of the city and its people.</p>
        </div>
        
        <div class="service-card">
          <div class="service-icon">🎨</div>
          <h3>Creative Projects</h3>
          <p>Conceptual and artistic photography projects that push creative boundaries and explore new ideas.</p>
        </div>
        
        <div class="service-card">
          <div class="service-icon">📖</div>
          <h3>Photo Workshops</h3>
          <p>Educational sessions and workshops to share photography techniques and creative approaches.</p>
        </div>
      </div>
    </div>

    <!-- Equipment Section -->
    <div class="about-equipment">
      <h2>My Toolkit</h2>
      <div class="equipment-grid">
        <div class="equipment-category">
          <h3>Cameras</h3>
          <ul>
            <li>Fujifilm X-T4</li>
            <li>Sony A7III</li>
            <li>Canon EOS R5</li>
          </ul>
        </div>
        
        <div class="equipment-category">
          <h3>Lenses</h3>
          <ul>
            <li>35mm f/1.4</li>
            <li>85mm f/1.8</li>
            <li>24-70mm f/2.8</li>
            <li>70-200mm f/2.8</li>
          </ul>
        </div>
        
        <div class="equipment-category">
          <h3>Software</h3>
          <ul>
            <li>Adobe Lightroom Classic</li>
            <li>Adobe Photoshop</li>
            <li>Capture One</li>
          </ul>
        </div>
      </div>
    </div>

    <!-- Testimonials Section -->
    <div class="about-testimonials">
      <h2>Kind Words</h2>
      <div class="testimonials-grid">
        <div class="testimonial-card">
          <div class="testimonial-text">
            "Working with {{ site.title | default: 'Your Name' }} was an incredible experience. The attention to detail and artistic vision brought our project to life in ways we never imagined."
          </div>
          <div class="testimonial-author">
            <strong>Sarah Johnson</strong>
            <span>Art Director</span>
          </div>
        </div>
        
        <div class="testimonial-card">
          <div class="testimonial-text">
            "The ability to capture genuine emotion and tell compelling stories through photography is truly remarkable. Every session feels unique and personal."
          </div>
          <div class="testimonial-author">
            <strong>Michael Chen</strong>
            <span>Magazine Editor</span>
          </div>
        </div>
      </div>
    </div>

    <!-- Contact CTA Section -->
    <div id="contact" class="about-contact">
      <div class="contact-cta">
        <h2>Let's Create Something Amazing Together</h2>
        <p>Interested in working together or have questions about my services? I'd love to hear from you.</p>
        <div class="cta-buttons">
          <a href="mailto:{{ site.email | default: 'your@email.com' }}" class="btn btn-primary">Send an Email</a>
          <a href="{{ site.instagram | default: '#' }}" class="btn btn-outline" target="_blank">Follow on Instagram</a>
        </div>
      </div>
    </div>
  </div>
</section>

<style>
.about-page {
  padding: 120px 0 80px;
}

/* Hero Section (centered without image) */
.about-hero {
  text-align: center;
  margin-bottom: 6rem;
  max-width: 800px;
  margin-left: auto;
  margin-right: auto;
}

.about-intro .page-title {
  font-size: 3.5rem;
  font-weight: 300;
  margin-bottom: 1.5rem;
  letter-spacing: -0.02em;
  line-height: 1.2;
}

.lead-text {
  font-size: 1.375rem;
  line-height: 1.7;
  color: var(--secondary-color);
  margin-bottom: 2.5rem;
  font-weight: 300;
}

.about-cta {
  display: flex;
  gap: 1rem;
  justify-content: center;
  flex-wrap: wrap;
}

/* Bio Section */
.about-bio {
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: 4rem;
  margin-bottom: 6rem;
  padding: 3rem 0;
  border-top: 1px solid var(--border-color);
  border-bottom: 1px solid var(--border-color);
}

.bio-content h2 {
  font-size: 2rem;
  font-weight: 300;
  margin-bottom: 2rem;
  color: var(--primary-color);
}

.bio-content p {
  font-size: 1.125rem;
  line-height: 1.8;
  margin-bottom: 1.5rem;
  color: var(--text-color);
}

.bio-highlights {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  justify-content: center;
}

.highlight-item {
  text-align: center;
  padding: 1.5rem;
  background: var(--light-gray);
  border-radius: 8px;
}

.highlight-number {
  font-size: 2.5rem;
  font-weight: 300;
  color: var(--accent-color);
  margin-bottom: 0.5rem;
}

.highlight-text {
  font-size: 0.875rem;
  color: var(--secondary-color);
  text-transform: uppercase;
  letter-spacing: 0.5px;
}

/* Services Section */
.about-services {
  margin-bottom: 6rem;
}

.about-services h2 {
  text-align: center;
  font-size: 2.5rem;
  font-weight: 300;
  margin-bottom: 3rem;
}

.services-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

.service-card {
  background: white;
  padding: 2.5rem 2rem;
  border-radius: 12px;
  text-align: center;
  border: 1px solid var(--border-color);
  transition: all 0.3s ease;
}

.service-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
  border-color: var(--accent-color);
}

.service-icon {
  font-size: 3rem;
  margin-bottom: 1.5rem;
}

.service-card h3 {
  font-size: 1.25rem;
  font-weight: 500;
  margin-bottom: 1rem;
  color: var(--primary-color);
}

.service-card p {
  color: var(--secondary-color);
  line-height: 1.6;
}

/* Equipment Section */
.about-equipment {
  margin-bottom: 6rem;
}

.about-equipment h2 {
  text-align: center;
  font-size: 2.5rem;
  font-weight: 300;
  margin-bottom: 3rem;
}

.equipment-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
}

.equipment-category {
  background: var(--light-gray);
  padding: 2rem;
  border-radius: 8px;
}

.equipment-category h3 {
  font-size: 1.25rem;
  font-weight: 500;
  margin-bottom: 1.5rem;
  color: var(--primary-color);
  text-align: center;
}

.equipment-category ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.equipment-category li {
  padding: 0.75rem 0;
  border-bottom: 1px solid var(--border-color);
  text-align: center;
  color: var(--text-color);
}

.equipment-category li:last-child {
  border-bottom: none;
}

/* Testimonials Section */
.about-testimonials {
  margin-bottom: 6rem;
}

.about-testimonials h2 {
  text-align: center;
  font-size: 2.5rem;
  font-weight: 300;
  margin-bottom: 3rem;
}

.testimonials-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 2rem;
}

.testimonial-card {
  background: white;
  padding: 2.5rem;
  border-radius: 12px;
  border: 1px solid var(--border-color);
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
}

.testimonial-text {
  font-size: 1.125rem;
  line-height: 1.7;
  color: var(--text-color);
  margin-bottom: 2rem;
  font-style: italic;
  position: relative;
}

.testimonial-text::before {
  content: '"';
  font-size: 4rem;
  color: var(--accent-color);
  position: absolute;
  top: -1rem;
  left: -1rem;
  opacity: 0.3;
  font-family: serif;
}

.testimonial-author {
  text-align: right;
}

.testimonial-author strong {
  display: block;
  color: var(--primary-color);
  margin-bottom: 0.25rem;
}

.testimonial-author span {
  color: var(--secondary-color);
  font-size: 0.875rem;
}

/* Contact CTA Section */
.about-contact {
  background: var(--light-gray);
  padding: 4rem 2rem;
  border-radius: 12px;
  text-align: center;
}

.contact-cta h2 {
  font-size: 2.25rem;
  font-weight: 300;
  margin-bottom: 1.5rem;
  color: var(--primary-color);
}

.contact-cta p {
  font-size: 1.125rem;
  color: var(--secondary-color);
  margin-bottom: 2.5rem;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
}

.cta-buttons {
  display: flex;
  gap: 1rem;
  justify-content: center;
  flex-wrap: wrap;
}

/* Responsive Design */
@media (max-width: 968px) {
  .about-bio {
    grid-template-columns: 1fr;
    gap: 3rem;
  }
  
  .bio-highlights {
    flex-direction: row;
    justify-content: space-around;
  }
}

@media (max-width: 768px) {
  .about-page {
    padding: 100px 0 60px;
  }
  
  .about-intro .page-title {
    font-size: 2.5rem;
  }
  
  .lead-text {
    font-size: 1.25rem;
  }
  
  .about-cta,
  .cta-buttons {
    flex-direction: column;
    align-items: center;
  }
  
  .services-grid,
  .testimonials-grid {
    grid-template-columns: 1fr;
  }
  
  .bio-highlights {
    flex-direction: column;
  }
  
  .equipment-grid {
    grid-template-columns: 1fr;
  }
}

@media (max-width: 480px) {
  .about-intro .page-title {
    font-size: 2rem;
  }
  
  .about-services h2,
  .about-equipment h2,
  .about-testimonials h2 {
    font-size: 2rem;
  }
  
  .service-card,
  .testimonial-card {
    padding: 2rem 1.5rem;
  }
  
  .contact-cta h2 {
    font-size: 1.75rem;
  }
  
  .highlight-item {
    padding: 1rem;
  }
  
  .highlight-number {
    font-size: 2rem;
  }
}
</style>