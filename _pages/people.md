---
title: "👥 People"
permalink: /people/
author_profile: false
full_width: true
---

{% assign people = site.data.people %}

<nav class="people-subnav" aria-label="People sections">
  <a href="#faculty">Faculty <span>{{ people.faculty | size }}</span></a>
  <a href="#graduate-researchers">Graduate Researchers <span>{{ people.graduate_researchers | size }}</span></a>
  <a href="#undergraduate-researchers">Undergraduate Researchers <span>{{ people.undergraduate_researchers | size }}</span></a>
</nav>

<h2 id="faculty" class="people-heading">
  <span>Faculty</span>
  <span class="people-count">{{ people.faculty | size }}</span>
</h2>

<div class="faculty-list">
{% for member in people.faculty %}
  <article class="faculty-card">
    <div class="faculty-card__photo-wrap">
      <img class="faculty-card__photo" src="{{ member.photo | relative_url }}" alt="Portrait of {{ member.name }}" loading="eager" decoding="async">
    </div>

    <div class="faculty-card__content">
      <div class="faculty-card__identity">
        <h3 class="faculty-card__name">{{ member.name }}</h3>
        <div class="faculty-card__role">{{ member.role }}</div>
        <div class="faculty-card__affiliation">
          {{ member.department }}<br>
          {{ member.institution }}
        </div>
      </div>

      <div class="faculty-card__links" aria-label="Links for {{ member.name }}">
        {% if member.email %}<a href="mailto:{{ member.email }}"><i class="fas fa-envelope" aria-hidden="true"></i> Email</a>{% endif %}
        {% if member.scholar %}<a href="{{ member.scholar }}" target="_blank" rel="noopener noreferrer"><i class="ai ai-google-scholar" aria-hidden="true"></i> Google Scholar</a>{% endif %}
        {% if member.orcid %}<a href="{{ member.orcid }}" target="_blank" rel="noopener noreferrer"><i class="ai ai-orcid" aria-hidden="true"></i> ORCID</a>{% endif %}
        {% if member.linkedin %}<a href="{{ member.linkedin }}" target="_blank" rel="noopener noreferrer"><i class="fab fa-linkedin" aria-hidden="true"></i> LinkedIn</a>{% endif %}
      </div>

      <div class="faculty-card__bio">
        <div class="faculty-card__label">Biography</div>
        {% for paragraph in member.bio %}
          <p>{{ paragraph }}</p>
        {% endfor %}
      </div>

      {% if member.research_interests and member.research_interests.size > 0 %}
      <div class="faculty-card__interests">
        <div class="faculty-card__label">Research Interests</div>
        <div class="interest-tags">
          {% for interest in member.research_interests %}
            <span>{{ interest }}</span>
          {% endfor %}
        </div>
      </div>
      {% endif %}
    </div>
  </article>
{% endfor %}
</div>

<h2 id="graduate-researchers" class="people-heading">
  <span>Graduate Researchers</span>
  <span class="people-count">{{ people.graduate_researchers | size }}</span>
</h2>

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
<div class="people-empty">No graduate researchers are listed yet.</div>
{% endif %}

<h2 id="undergraduate-researchers" class="people-heading">
  <span>Undergraduate Researchers</span>
  <span class="people-count">{{ people.undergraduate_researchers | size }}</span>
</h2>

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
<div class="people-empty">No undergraduate researchers are listed yet.</div>
{% endif %}
