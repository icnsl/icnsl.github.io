---
title: "Publications"
permalink: /publications/
author_profile: false
hide_title: true
---
<div class="icnsl-showcase icnsl-showcase--publications">
<header class="icnsl-showcase__intro">
  <div class="icnsl-showcase__glyph" aria-hidden="true"><i class="fas fa-book-open"></i></div>
  <div class="icnsl-showcase__intro-copy">
    <div class="icnsl-showcase__eyebrow">Research Output</div>
    <p class="icnsl-showcase__lead">Peer-reviewed journal and conference publications </p>
    <div class="icnsl-showcase__tags" aria-label="Publication categories">
      <span>Journal Articles</span><span>Conference Papers</span>
    </div>
  </div>
</header>

<section class="icnsl-section" aria-labelledby="journal-papers-heading">
  <h2 id="journal-papers-heading" class="icnsl-section__heading">
    <span class="icnsl-section__icon" aria-hidden="true">📚</span>
    <span>Journal Papers</span>
  </h2>

<div class="pub-list icnsl-catalog-list icnsl-catalog-list--journal">

{% comment %}
새 저널 논문은 아래 journal_no 초기화 줄 다음에 추가하세요.
각 논문의 assign ... plus: 1 줄부터 pub-entry의 닫는 div까지 복사하고,
pub-citation 안의 논문 정보만 수정하면 됩니다.
초기화 줄(assign journal_no = 0)은 이 목록에 한 번만 둡니다.
{% endcomment %}
{% assign journal_no = 0 %}

{% assign journal_no = journal_no | plus: 1 %}
<div class="pub-entry" id="pub-j{{ journal_no }}">
  <div class="pub-no">[J{{ journal_no }}]</div>
  <div class="pub-citation">
    <strong>Jonghun Han</strong>, and Hongchan Kim*,
    “A Graph-Theoretic and Stochastic Analysis of BLE-Assisted Cooperative Wi-Fi Scanning,”<br>
    <em>Mathematics</em>, vol. 14, No. 17: 3214, Sep. 2026.
    <span class="pub-impact">(impact factor<span class="pub-metric-value">2.3</span>, SCIE top<span class="pub-metric-value pub-red">5.6%</span>)</span>
  </div>
</div>

{% assign journal_no = journal_no | plus: 1 %}
<div class="pub-entry" id="pub-j{{ journal_no }}">
  <div class="pub-no">[J{{ journal_no }}]</div>
  <div class="pub-citation">
    Jongyeon Park, Youngwook Son*, Kanghyun Lee, <strong>Jonghun Han</strong>, and Saewoong Bahk,
    “Demystifying Multi-Link Device Behavior and Performance under Network Saturation in Wi-Fi 7,”<br>
    <em>IEEE Transactions on Networking</em>, vol. 34, pp. 6632-6657, Jul. 2026.
    <span class="pub-impact">(impact factor<span class="pub-metric-value pub-red">5.3</span>, SCIE top<span class="pub-metric-value pub-red">16.1%</span>)</span>
  </div>
</div>

{% assign journal_no = journal_no | plus: 1 %}
<div class="pub-entry" id="pub-j{{ journal_no }}">
  <div class="pub-no">[J{{ journal_no }}]</div>
  <div class="pub-citation">
    Cheonyong Kim, Walid Saad, <strong>Jonghun Han*</strong>, Tao Yu, Kei Sakaguchi and Minchae Jung*,
    “Real-Time Task Scheduling with Fairness in Digital Twin Systems,”<br>
    <em>IEEE Internet of Things Journal</em>, vol. 12, no. 7, pp. 7846–7862, Apr. 2025.
    <span class="pub-impact">(impact factor<span class="pub-metric-value pub-red">8.2</span>, SCIE top<span class="pub-metric-value pub-red">3.4%</span>)</span>
  </div>
</div>

{% assign journal_no = journal_no | plus: 1 %}
<div class="pub-entry" id="pub-j{{ journal_no }}">
  <div class="pub-no">[J{{ journal_no }}]</div>
  <div class="pub-citation">
    Jongyeon Park, <strong>Jonghun Han*</strong>, and Saewoong Bahk*,
    “Adaptive Multi-Link Channel Access Under Cross-Link Interference in Next-Generation WLANs,”<br>
    <em>IEEE Internet of Things Journal</em>, vol. 11, no. 14, pp. 24685–24697, Jul. 2024.
    <span class="pub-impact">(impact factor<span class="pub-metric-value pub-red">8.2</span>, SCIE top<span class="pub-metric-value pub-red">3.4%</span>)</span>
  </div>
</div>

{% assign journal_no = journal_no | plus: 1 %}
<div class="pub-entry" id="pub-j{{ journal_no }}">
  <div class="pub-no">[J{{ journal_no }}]</div>
  <div class="pub-citation">
    Minchae Jung, and <strong>Jonghun Han*</strong>, 
    “Adaptive Packet Tuning for Energy Efficient Communication in Underlay CSMA/CA Networks,”<br>
    <em>IEEE Access</em>, vol. 11, pp. 95989-95998, Aug. 2023.
    <span class="pub-impact">(impact factor<span class="pub-metric-value">3.9</span>, SCIE top<span class="pub-metric-value">36.2%</span>)</span>
  </div>
</div>

{% assign journal_no = journal_no | plus: 1 %}
<div class="pub-entry" id="pub-j{{ journal_no }}">
  <div class="pub-no">[J{{ journal_no }}]</div>
  <div class="pub-citation">
    <strong>Jonghun Han</strong>, Changhee Joo, and Saewoong Bahk*,
    “Resource Sharing in Dual-Stack Devices: Opportunistic Bluetooth Transmissions in WLAN Busy Periods,”<br>
    <em>IEEE Transactions on Mobile Computing</em>, vol. 17, no. 10, pp. 2396–2407, Oct. 2018.
    <span class="pub-impact">(impact factor<span class="pub-metric-value">4.098</span>, SCIE top<span class="pub-metric-value pub-red">9.1%</span>)</span>
  </div>
</div>

</div>
</section>

<section class="icnsl-section" aria-labelledby="conference-papers-heading">
  <h2 id="conference-papers-heading" class="icnsl-section__heading">
    <span class="icnsl-section__icon" aria-hidden="true">🛰️</span>
    <span>Conference Papers</span>
  </h2>

<div class="pub-list icnsl-catalog-list icnsl-catalog-list--conference">

{% comment %}
새 학회 논문은 아래 conference_no 초기화 줄 다음에 추가하세요.
각 논문의 assign ... plus: 1 줄부터 pub-entry의 닫는 div까지 복사하고,
pub-citation 안의 논문 정보만 수정하면 됩니다.
초기화 줄(assign conference_no = 0)은 이 목록에 한 번만 둡니다.
{% endcomment %}
{% assign conference_no = 0 %}

{% assign conference_no = conference_no | plus: 1 %}
<div class="pub-entry" id="pub-c{{ conference_no }}">
  <div class="pub-no">[C{{ conference_no }}]</div>
  <div class="pub-citation">
    Seonho Jang, Jongseo Lee, <strong>Jonghun Han</strong>, and Minchae Jung,
    “Optimization of Update Period in Digital Twin Systems,”<br>
    in <em>International Conference on Ubiquitous and Future Networks (ICUFN)</em> 2025,
    Lisbon, Portugal, Jul. 8–11, 2025.
  </div>
</div>

{% assign conference_no = conference_no | plus: 1 %}
<div class="pub-entry" id="pub-c{{ conference_no }}">
  <div class="pub-no">[C{{ conference_no }}]</div>
  <div class="pub-citation">
    Subin Choi, Hongjae Jeong, <strong>Jonghun Han</strong>, and Minchae Jung,
    “Optimal Inference Task Length for Minimizing Synchronization Error in Digital Twin Systems,”<br>
    in <em>International Conference on Ubiquitous and Future Networks (ICUFN)</em> 2025,
    Lisbon, Portugal, Jul. 8–11, 2025.
  </div>
</div>

{% assign conference_no = conference_no | plus: 1 %}
<div class="pub-entry" id="pub-c{{ conference_no }}">
  <div class="pub-no">[C{{ conference_no }}]</div>
  <div class="pub-citation">
    <strong>Jonghun Han</strong>, Joonsuk Kim, Changhee Joo, and Saewoong Bahk,
    “SplitScan: Sharing Wi-Fi Scan Information through Bluetooth Low Energy,”<br>
    in <em>IEEE Vehicular Technology Conference (VTC) 2019-Spring</em>,
    Honolulu, USA, Sep. 22–25, 2019.
  </div>
</div>

{% assign conference_no = conference_no | plus: 1 %}
<div class="pub-entry" id="pub-c{{ conference_no }}">
  <div class="pub-no">[C{{ conference_no }}]</div>
  <div class="pub-citation">
    Taeseop Lee, <strong>Jonghun Han</strong>, Myung-Sup Lee, Hyung-Sin Kim, and Saewoong Bahk,
    “cABLE: Connection Interval Adaptation for BLE in Dynamic Wireless Environments,”<br>
    in <em>IEEE International Conference on Sensing, Communication, and Networking (SECON)</em> 2017,
    San Diego, USA, June 12–14, 2017.
  </div>
</div>

{% assign conference_no = conference_no | plus: 1 %}
<div class="pub-entry" id="pub-c{{ conference_no }}">
  <div class="pub-no">[C{{ conference_no }}]</div>
  <div class="pub-citation">
    Wonbin Park, <strong>Jonghun Han</strong>, Seowoo Jang, and Saewoong Bahk,
    “OAU: Opportunistic Antenna Utilization for Wi-Fi and Bluetooth Coexistence,”<br>
    in <em>IEEE Global Communication Conference (GLOBECOM)</em> 2016,
    Washington, DC, USA, Dec. 4–8, 2016.
  </div>
</div>

{% assign conference_no = conference_no | plus: 1 %}
<div class="pub-entry" id="pub-c{{ conference_no }}">
  <div class="pub-no">[C{{ conference_no }}]</div>
  <div class="pub-citation">
    Sung-Guk Yoon, <strong>Jonghun Han</strong>, and Saewoong Bahk,
    “Low-Duty Mode Operation of Femto Base Stations in a Densely Deployed Network Environment,”<br>
    in <em>International Symposium on Personal, Indoor and Mobile Radio Communications (PIMRC)</em> 2012,
    Sydney, Australia, Sep. 9–12, 2012.
  </div>
</div>

{% assign conference_no = conference_no | plus: 1 %}
<div class="pub-entry" id="pub-c{{ conference_no }}">
  <div class="pub-no">[C{{ conference_no }}]</div>
  <div class="pub-citation">
    <strong>Jonghun Han</strong> and Saewoong Bahk,
    “Low-Duty Mode Operation of Femto Base Stations in a Densely Deployed Network Environment,”<br>
    in <em>IEEE VTS Asia Pacific Wireless Communications Symposium (APWCS)</em> 2012,
    Kyoto, Japan, Aug. 23–24, 2012.
  </div>
</div>

{% assign conference_no = conference_no | plus: 1 %}
<div class="pub-entry" id="pub-c{{ conference_no }}">
  <div class="pub-no">[C{{ conference_no }}]</div>
  <div class="pub-citation">
    Nalin Chakoo, <strong>Jonghun Han</strong>, and Saewoong Bahk,
    “Context-Aware Ontological Schemes for Multimedia Personalization,”<br>
    in <em>International Conference on ICT Convergence (ICTC)</em> 2011,
    Seoul, Korea, Sep. 28–30, 2011.
  </div>
</div>

</div>
</section>
</div>
