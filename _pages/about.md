---
permalink: /
title: "Home"
author_profile: false
hide_title: true
redirect_from:
  - /about/
  - /about.html
---
<header class="home-lab-hero" aria-labelledby="home-lab-title">
  <div class="home-lab-hero__accent" aria-hidden="true">
    <span></span><span></span><span></span>
  </div>
  <h1 id="home-lab-title" class="home-lab-hero__title">Intelligent Communications and Networked Systems Laboratory</h1>
</header>

<section class="home-section home-section--notice" aria-labelledby="home-notice-heading">
  <h2 id="home-notice-heading">📌 Notice</h2>

  <div class="home-section__list">
    <div class="home-section__entry home-section__entry--notice">
      <div class="home-section__text" lang="ko">
        연구, 학업, 진로·미래 또는 개인적인 고민에 관해 면담이 필요한 경우, 메일로 연락주세요.
      </div>
      <div class="home-section__translation" lang="en">
        If you would like to discuss research, academics, career or future plans, or personal concerns, please contact me by email.
      </div>
    </div>
  </div>
</section>

<section class="home-section home-section--news" aria-labelledby="home-news-heading">
  <h2 id="home-news-heading">📢 Recent News</h2>

  <div class="home-section__list">
    <div class="home-section__entry">
      <div class="home-section__text">
        <strong>[2026.07]</strong> Our work, "Demystifying Multi-Link Device Behavior and Performance under Network Saturation in Wi-Fi 7", has been accepted to <em>IEEE Transactions on Networking</em>.
      </div>
    </div>

    <div class="home-section__entry">
      <div class="home-section__text">
        <strong>[2026.06]</strong> Website renewal! Yay! 홈페이지를 리뉴얼 했습니다 😺
      </div>
    </div>

    <div class="home-section__entry">
      <div class="home-section__text">
        <strong>[2025.04]</strong> Our paper titled “Real-Time Task Scheduling With Fairness in Digital Twin Systems” has been published in the <em>IEEE Internet of Things Journal</em>.
      </div>
    </div>

    <div class="home-section__entry">
      <div class="home-section__text">
        <strong>[2025.03]</strong> I was appointed as an Assistant Professor in the Department of Artificial Intelligence and Information Technology at Sejong University.
      </div>
    </div>
  </div>
</section>

<section class="home-section home-section--research" aria-labelledby="home-research-heading">
  <h2 id="home-research-heading">🔬 Research Areas</h2>


  <div class="research-card-grid">
  {% for area in site.data.research.areas %}
    <article class="research-card">
      <div class="research-card__image">
        <img src="{{ area.image | relative_url }}" alt="{{ area.alt }}" loading="lazy" decoding="async">
      </div>
      <div class="research-card__body">
        <div class="research-card__kicker">{{ area.kicker }}</div>
        <h3 class="research-card__title{% if area.title_style %} research-card__title--{{ area.title_style }}{% endif %}">{{ area.title }}</h3>
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
</section>
