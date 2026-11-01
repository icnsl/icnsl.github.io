---
permalink: /
title: "Home"
author_profile: false
hide_title: true
redirect_from:
  - /about/
  - /about.html
---
<div class="icnsl-showcase icnsl-showcase--home">
<header class="icnsl-showcase__intro" aria-labelledby="home-lab-title">
  <div class="icnsl-showcase__glyph" aria-hidden="true"><i class="fas fa-network-wired"></i></div>
  <div class="icnsl-showcase__intro-copy">
    <div class="icnsl-showcase__eyebrow">ICNSL</div>
    <h1 id="home-lab-title" class="icnsl-showcase__lead">Intelligent Communications and Networked Systems Laboratory</h1>
    <div class="icnsl-showcase__tags" aria-label="Laboratory research themes">
      <span>Wireless Communications</span><span>Intelligent Networks</span><span>Positioning &amp; Digital Twins</span>
    </div>
  </div>
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
      <div class="notice-email">
        <button class="notice-email__toggle" type="button" data-email-codes="x.z.16.11.b.1k.1a.x.10.11.18.2t.16.14.2t.w.1l" aria-expanded="false" aria-controls="home-notice-email-details" hidden>이메일 확인 / Show email</button>
        <div class="notice-email__details" id="home-notice-email-details" aria-live="polite" hidden></div>
        <a class="notice-email__fallback" href="{{ '/contact/' | relative_url }}">이메일 연락처 / Email contact</a>
      </div>
    </div>
  </div>
</section>

<section class="home-section home-section--news" aria-labelledby="home-news-heading">
  <h2 id="home-news-heading">📢 Recent News</h2>

   <div class="home-section__list">
    <div class="home-section__entry">
      <div class="home-section__text"> 
        <strong>[2026.09]</strong> Our paper, “A Graph-Theoretic and Stochastic Analysis of BLE-Assisted Cooperative Wi-Fi Scanning,” has been published in <em>Mathematics</em>.
      </div>
    </div>
     
    <div class="home-section__entry">
      <div class="home-section__text">
        <strong>[2026.08]</strong> 지능정보융합학과 최세현 학생이 학부연구생으로 연구실에 합류하게 되었습니다. 환영합니다!. We are pleased to welcome Sehyun Choi, a student in the Department of Artificial Intelligence and Information Technology, to our lab as an undergraduate researcher. 👍
      </div>
    </div>
    
    <div class="home-section__entry">
      <div class="home-section__text">
        <strong>[2026.07]</strong> Our work, "Demystifying Multi&#8209;Link Device Behavior and Performance under Network Saturation in Wi&#8209;Fi&nbsp;7", has been published in the <em>IEEE Transactions on Networking</em>.
      </div>
    </div>

    <div class="home-section__entry">
      <div class="home-section__text">
        <strong>[2026.06]</strong> Website renewal! Yay! 홈페이지를 리뉴얼 했습니다 😺
      </div>
    </div>

    <div class="home-section__entry">
      <div class="home-section__text">
        <strong>[2025.04]</strong> Our paper titled “Real&#8209;Time Task Scheduling With Fairness in Digital Twin Systems” has been published in the <em>IEEE Internet of Things Journal</em>.
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
      <a class="research-card__image" href="{{ area.image_full | default: area.image | relative_url }}" target="_blank" rel="noopener" aria-label="Enlarge diagram: {{ area.title | escape }}">
        <img src="{{ area.image | relative_url }}" alt="{{ area.alt | escape }}" width="1536" height="1024" loading="lazy" decoding="async">
        <span class="research-card__zoom-hint" aria-hidden="true"><svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.7"><circle cx="10" cy="10" r="6.5"/><path d="m15 15 6 6M10 7v6M7 10h6"/></svg>View larger</span>
      </a>
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
</div>


