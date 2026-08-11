---
title: "People"
permalink: /people/
author_profile: false
hide_title: true
---

{% assign people = site.data.people %}

<section class="people-section people-section--faculty">
  <h2 id="faculty" class="people-heading">Faculty</h2>

  <div class="faculty-list">
  {% for member in people.faculty %}
    <article class="faculty-card">
      <div class="faculty-card__photo-wrap">
        <img class="faculty-card__photo" src="{{ member.photo | relative_url }}" alt="Portrait of {{ member.name }}" loading="eager" decoding="async">
      </div>

      <header class="faculty-card__identity">
        <h3 class="faculty-card__name">{{ member.name }}</h3>
        <div class="faculty-card__role">{{ member.role }}</div>
        <div class="faculty-card__affiliation">
          {{ member.department }}<br>
          {{ member.institution }}
        </div>
      </header>

      <details class="faculty-card__bio">
        <summary class="faculty-card__bio-toggle">Biography</summary>
        <div class="faculty-card__bio-content">
          {% for paragraph in member.bio %}
            <p>{{ paragraph }}</p>
          {% endfor %}
        </div>
      </details>

      <nav class="faculty-card__links" aria-label="External links for {{ member.name }}">
        {% if member.email %}
          <a href="mailto:{{ member.email }}">
            <i class="fas fa-fw fa-envelope icon-pad-right" aria-hidden="true"></i>
            <span>Email</span>
          </a>
        {% endif %}
        {% if member.scholar %}
          <a href="{{ member.scholar }}" target="_blank" rel="noopener noreferrer">
            <i class="ai ai-google-scholar ai-fw icon-pad-right" aria-hidden="true"></i>
            <span>Google Scholar</span>
          </a>
        {% endif %}
        {% if member.orcid %}
          <a href="{{ member.orcid }}" target="_blank" rel="noopener noreferrer">
            <i class="ai ai-orcid ai-fw icon-pad-right" aria-hidden="true"></i>
            <span>ORCID</span>
          </a>
        {% endif %}
        {% if member.researchgate %}
          <a href="{{ member.researchgate }}" target="_blank" rel="noopener noreferrer">
            <i class="fab fa-fw fa-researchgate icon-pad-right" aria-hidden="true"></i>
            <span>ResearchGate</span>
          </a>
        {% endif %}
        {% if member.linkedin %}
          <a href="{{ member.linkedin }}" target="_blank" rel="noopener noreferrer">
            <i class="fab fa-fw fa-linkedin icon-pad-right" aria-hidden="true"></i>
            <span>LinkedIn</span>
          </a>
        {% endif %}
      </nav>
    </article>
  {% endfor %}
  </div>
</section>

<section class="people-section">
  <h2 id="graduate-researchers" class="people-heading">Graduate Researchers</h2>

  {% if people.graduate_researchers.size > 0 %}
  <div class="member-grid">
  {% for member in people.graduate_researchers %}
    <article class="member-card">
      {% if member.photo %}
        <img class="member-card__photo" src="{{ member.photo | relative_url }}" alt="Portrait of {{ member.name }}" loading="lazy" decoding="async">
      {% else %}
        <div class="member-card__placeholder" aria-hidden="true">PHOTO</div>
      {% endif %}

      <div class="member-card__content">
        <h3>{{ member.name }}</h3>
        {% if member.program %}<div class="member-card__program">{{ member.program }}</div>{% endif %}
        {% if member.period %}<div class="member-card__period">{{ member.period }}</div>{% endif %}
        {% if member.research %}<p>{{ member.research }}</p>{% endif %}
        <div class="member-card__links">
          {% if member.email %}<a href="mailto:{{ member.email }}">Email</a>{% endif %}
          {% if member.linkedin %}<a href="{{ member.linkedin }}" target="_blank" rel="noopener noreferrer">LinkedIn</a>{% endif %}
        </div>
      </div>
    </article>
  {% endfor %}
  </div>
  {% else %}
  <div class="people-empty">Graduate researcher profiles will be added here.</div>
  {% endif %}
</section>

<section class="people-section">
  <h2 id="undergraduate-researchers" class="people-heading">Undergraduate Researchers</h2>

  {% if people.undergraduate_researchers.size > 0 %}
  <div class="member-grid">
  {% for member in people.undergraduate_researchers %}
    <article class="member-card">
      {% if member.photo %}
        <img class="member-card__photo" src="{{ member.photo | relative_url }}" alt="Portrait of {{ member.name }}" loading="lazy" decoding="async">
      {% else %}
        <div class="member-card__placeholder" aria-hidden="true">PHOTO</div>
      {% endif %}

      <div class="member-card__content">
        <h3>{{ member.name }}</h3>
        {% if member.program %}<div class="member-card__program">{{ member.program }}</div>{% endif %}
        {% if member.period %}<div class="member-card__period">{{ member.period }}</div>{% endif %}
        {% if member.research %}<p>{{ member.research }}</p>{% endif %}
        <div class="member-card__links">
          {% if member.email %}<a href="mailto:{{ member.email }}">Email</a>{% endif %}
          {% if member.linkedin %}<a href="{{ member.linkedin }}" target="_blank" rel="noopener noreferrer">LinkedIn</a>{% endif %}
        </div>
      </div>
    </article>
  {% endfor %}
  </div>
  {% else %}
  <div class="people-empty">Undergraduate researcher profiles will be added here.</div>
  {% endif %}
</section>
