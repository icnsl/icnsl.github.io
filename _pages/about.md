---
permalink: /
title: "🏠 Home"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
<div class="home-notice-title">
  <strong>📌 Notice:</strong> 연구/학업/대학생활 등 면담이 필요한 경우, 메일로 연락주세요. 
</div>

## 📢 Recent News (최근 소식)

<div class="news-list">

<div class="news-entry">  
  <div class="news-text">
    <strong>[2026.07]</strong> Our work, "Demystifying Multi-Link Device Behavior and Performance under Network Saturation in Wi-Fi 7", has been accepted to <em>IEEE Transactions on Networking</em>.
  </div>
</div>

<div class="news-entry">  
  <div class="news-text">
    <strong>[2026.06]</strong> Website renewal! Yay! 홈페이지를 리뉴얼 했습니다 😺
  </div>
</div>

<div class="news-entry">
  <div class="news-text">
    <strong>[2025.04]</strong> Our paper titled “Real-Time Task Scheduling With Fairness in Digital Twin Systems” has been published in the <em>IEEE Internet of Things Journal</em>.
  </div>
</div>

<div class="news-entry">
  <div class="news-text">
    <strong>[2025.03]</strong> I was appointed as an Assistant Professor in the Department of Artificial Intelligence and Information Technology at Sejong University.
  </div>
</div>

</div>

## 🔬 Research Areas

<div class="research-card-grid">
{% for area in site.data.research.areas %}
  <article class="research-card">
    <div class="research-card__image">
      <img src="{{ area.image | relative_url }}" alt="{{ area.alt }}" loading="lazy" decoding="async">
    </div>
    <div class="research-card__body">
      <div class="research-card__kicker">{{ area.kicker }}</div>
      <h3 class="research-card__title">{{ area.title }}</h3>
      <p class="research-card__description">{{ area.description }}</p>
      {% if area.publications and area.publications.size > 0 %}
      <div class="research-card__refs" aria-label="Representative publications">
        <span>Representative work</span>
        {% for publication in area.publications %}
          <a href="{{ publication.url | relative_url }}">{{ publication.label }}</a>
        {% endfor %}
      </div>
      {% endif %}
    </div>
  </article>
{% endfor %}
</div>
