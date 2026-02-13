---
layout: default
title: Home
---

<!-- Hero Section -->
<section class="hero">
    <div class="hero-content">
        <div class="hero-label">AI Researcher & Builder</div>
        <h1>Edo Cohen-Karlik</h1>
        <p class="hero-bio">
            I work at the intersection of rigorous research and real-world products—teaching machines to argue, generating novel drug candidates, and shaping AI strategy. Currently VP of AI at a stealth startup, driven by the belief that the most impactful AI work happens where research meets implementation.
        </p>
        <div class="hero-links">
            <a href="mailto:edocohen@mail.tau.ac.il" class="hero-link">
                <span>Email</span>
            </a>
            <a href="https://www.linkedin.com/in/edo-cohen" target="_blank" class="hero-link">
                <span>LinkedIn</span>
            </a>
            <a href="https://scholar.google.com/citations?hl=en&user=uLBSdVQAAAAJ" target="_blank" class="hero-link">
                <span>Google Scholar</span>
            </a>
        </div>
    </div>
    <div class="scroll-indicator">
        <span class="scroll-text">Explore</span>
        <div class="scroll-line"></div>
    </div>
</section>

<!-- Publications Section -->
<section id="publications">
    <div class="container">
        <div class="section-header reveal">
            <div class="section-number">01</div>
            <h2>Research Publications</h2>
        </div>

        <div class="publications-grid">
            {% for pub in site.data.publications %}
            <article class="publication reveal">
                <div class="pub-year">{{ pub.year }}</div>
                <h3 class="pub-title">
                    <a href="{{ pub.url }}" target="_blank">{{ pub.title }}</a>
                </h3>
                <p class="pub-authors">
                    {{ pub.authors }}
                </p>
                <p class="pub-venue">{{ pub.venue }}</p>
            </article>
            {% endfor %}
        </div>
    </div>
</section>

<!-- Teaching Section -->
<section id="teaching">
    <div class="container">
        <div class="section-header reveal">
            <div class="section-number">02</div>
            <h2>Teaching</h2>
        </div>

        <div class="teaching-grid">
            {% for course in site.data.teaching %}
            <div class="teaching-card reveal">
                <h3 class="teaching-title">{{ course.name }}</h3>
                <p class="teaching-years">{{ course.years }}</p>
            </div>
            {% endfor %}
        </div>
    </div>
</section>

<!-- Footer -->
<footer>
    <div class="container">
        <div class="footer-content">
            <h2 class="footer-title">Get in Touch</h2>
            <div class="footer-links">
                <a href="mailto:edocohen@mail.tau.ac.il" class="footer-link">Email</a>
                <a href="https://www.linkedin.com/in/edo-cohen" target="_blank" class="footer-link">LinkedIn</a>
                <a href="https://scholar.google.com/citations?hl=en&user=uLBSdVQAAAAJ" target="_blank" class="footer-link">Google Scholar</a>
            </div>
            <p class="footer-note">© 2026 Edo Cohen-Karlik</p>
        </div>
    </div>
</footer>
