---
title: "Patents"
permalink: /patents/
author_profile: false
hide_title: true
---
{% comment %}
특허 목록을 먼저 렌더링하여 기존 자동 번호로 국가별 등록 건수를 집계합니다.
특허 항목을 추가하거나 삭제하면 상단 건수도 자동으로 갱신됩니다.
{% endcomment %}
{% capture patent_catalog %}
<section class="icnsl-section" aria-labelledby="us-patents-heading">
  <h2 id="us-patents-heading" class="icnsl-section__heading">
    <span class="icnsl-section__icon" aria-hidden="true">📜</span>
    <span>Patents (US, Granted)</span>
  </h2>

<div class="pub-list icnsl-catalog-list icnsl-catalog-list--patents icnsl-catalog-list--us">

{% comment %}
새 미국 특허는 아래 us_patent_no 초기화 줄 다음에 추가하세요.
각 특허의 assign ... plus: 1 줄부터 pub-entry의 닫는 div까지 복사하고,
pub-citation 안의 특허 정보만 수정하면 됩니다.
초기화 줄(assign us_patent_no = 0)은 이 목록에 한 번만 둡니다.
{% endcomment %}
{% assign us_patent_no = 0 %}

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.justia.com/patent/12756439" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,756,439 B2</a>,
    “Apparatus and method of uplink beamforming in wireless local area network system,”
    Eunsung Jeon, Chulho Chung, Jinmin Kim, Ravi Hiranand Gidvani, Myeongjin Kim, and <strong>Jonghun Han</strong>,
    2026.10.06.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.justia.com/patent/12719639" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,719,639 B2</a>,
    Method And Apparatus For Transmitting And Receiving Block ACK In Wireless Communication System Supporting Multi-link,”
    <strong>Jonghun Han</strong>, Chulho Chung, Seunghwan Oh, and Kyungik Cho,
    2026.08.25.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.justia.com/patent/12701614" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,701,614 B2</a>,
    “Apparatus for Channel Access in WLAN System and Operating Method of the Apparatus,”
    <strong>Jonghun Han</strong>, Saewoong Bahk, and Jongyeon Park,
    2026.08.04.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US12557141B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,557,141 B2</a>,
    “Methods, devices and systems for wireless communication using multi-link,”
    <strong>Jonghun Han</strong>, Chulho Chung, Myeongjin Kim, and Eunsung Jeon,
    2026.02.17.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US12537619B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,537,619 B2</a>,
    “Apparatus and method for wireless communication based on puncturing,”
    Chulho Chung, <strong>Jonghun Han</strong>, Myeongjin Kim, and Eunsung Jeon,
    2026.01.27.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.justia.com/patent/12526648" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,526,648 B2</a>,
    “Apparatus and method for channel sounding,”
    Eunsung Jeon, Myeongjin Kim, and <strong>Jonghun Han</strong>,
    2026.01.13.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US12445933B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,445,933 B2</a>,
    “Apparatus and method for multi-link based wireless communication,”
    <strong>Jonghun Han</strong>, Chulho Chung, Myeongjin Kim, and Eunsung Jeon,
    2025.10.14.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US12388606B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,388,606 B2</a>,
    “Apparatus and method for block acknowledgement within reduced duration,”
    <strong>Jonghun Han</strong>, Chulho Chung, Srinivas Kandala, Myeongjin Kim, and Eunsung Jeon,
    2025.08.12.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US12382497B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,382,497 B2</a>,
    “Device and method for wireless communication using multiple links,”
    <strong>Jonghun Han</strong>, Chulho Chung, Myeongjin Kim, and Eunsung Jeon,
    2025.08.05.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <span class="pub-red">(IEEE 802.11be 표준 채택)</span>
    <a class="patent-link" href="https://patents.google.com/patent/US12355706B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,355,706 B2</a>,
    “Apparatus and method for communication based on multi-resource unit in wireless local area network system,”
    Myeongjin Kim, Eunsung Jeon, Wookbong Lee, and <strong>Jonghun Han</strong>,
    2025.07.08.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US12301508B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,301,508 B2</a>,
    “Apparatus and method for communication based on multi-resource unit in wireless local area network system,”
    Myeongjin Kim, Eunsung Jeon, Wookbong Lee, and <strong>Jonghun Han</strong>,
    2025.04.30.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US12250589B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,250,589 B2</a>,
    “Apparatus and method for channel sounding,”
    Eunsung Jeon, Myeongjin Kim, Chulho Chung, and <strong>Jonghun Han</strong>,
    2025.03.11.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US12231190B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,231,190 B2</a>,
    “Apparatus and method for wireless communication based on enhanced null data packet announcement,”
    Eunsung Jeon, Wookbong Lee, Myeongjin Kim, Chulho Chung, and <strong>Jonghun Han</strong>,
    2025.01.29.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US12225451B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,225,451 B2</a>,
    “Apparatus and method for extended signal field,”
    Myeongjin Kim, Jinmin Kim, Wookbong Lee, Eunsung Jeon, Chulho Chung, and <strong>Jonghun Han</strong>,
    2025.02.11.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US12224817B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,224,817 B2</a>,
    “Apparatus and method of uplink beamforming in wireless local area network system,”
    Eunsung Jeon, Chulho Chung, Myeongjin Kim, and <strong>Jonghun Han</strong>,
    2025.02.11.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.justia.com/patent/12149394" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,149,394 B2</a>,
    “Apparatus and method for extended range communication,”
    Myeongjin Kim, Jinmin Kim, Eunsung Jeon, Wookbong Lee, Chulho Chung, and <strong>Jonghun Han</strong>,
    2024.11.19.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US12096475B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,096,475 B2</a>,
    “Apparatus and method for coordinated spatial reuse in wireless communication,”
    <strong>Jonghun Han</strong>, Chulho Chung, Myeongjin Kim, and Eunsung Jeon,
    2024.09.17.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US12082249B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,082,249 B2</a>,
    “Apparatus and method for coordinated spatial reuse in wireless communication,”
    <strong>Jonghun Han</strong>, Chulho Chung, Sharan Naribole, and Srinivas Kandala,
    2024.08.14.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US12058230B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#12,058,230 B2</a>,
    “Apparatus and method for signaling expansion in wireless local area network system,”
    <strong>Jonghun Han</strong> and Chulho Chung,
    2024.08.06.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US11984985B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#11,984,985 B2</a>,
    “Method of performing wireless communication, wireless transmission device and wireless reception device performing the same,”
    <strong>Jonghun Han</strong> and Chulho Chung,
    2024.05.14.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US11979866B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#11,979,866 B2</a>,
    “Apparatus and method for channel sounding based on aggregated physical protocol data unit,”
    Eunsung Jeon, Wookbong Lee, Myeongjin Kim, Chulho Chung, and <strong>Jonghun Han</strong>,
    2024.05.07.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US11595994B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#11,595,994 B2</a>,
    “Apparatus and method for coordinated spatial reuse in wireless communication,”
    <strong>Jonghun Han</strong>, Chulho Chung, Sharan Naribole, and Srinivas Kandala,
    2023.02.28.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.justia.com/patent/11387877" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#11,387,877 B2</a>,
    “Device and method using adaptive codebook for dual beamforming feedback and wireless communication system including the same,”
    Eunsung Jeon, Wookbong Lee, Myeongjin Kim, and <strong>Jonghun Han</strong>,
    2022.07.12.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US11381366B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#11,381,366 B2</a>,
    “Wireless communication devices for transmitting data using spatial reuse and data communication methods using the same,”
    <strong>Jonghun Han</strong>, Young-Wook Son, Sung-Hyun Choi, Seong-Won Kim, and Kang-hyun Lee,
    2022.07.05.
  </div>
</div>

{% assign us_patent_no = us_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-p{{ us_patent_no }}">
  <div class="pub-no">[P{{ us_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/US8260270B2/en" target="_blank" rel="noopener noreferrer" title="Read the full patent text (opens in a new tab)">US#8,260,270 B2</a>,
    “Femto BS for reducing inter-cell interference and method for transmitting signal using the same,”
    Sung Guk Yoon, <strong>Jonghun Han</strong>, Sae Woong Bahk, Young Han Kim, and Ik Hyeon Kim,
    2012.09.04.
  </div>
</div>

</div>
</section>

<section class="icnsl-section" aria-labelledby="kr-patents-heading">
  <h2 id="kr-patents-heading" class="icnsl-section__heading">
    <span class="icnsl-section__icon" aria-hidden="true">🧾</span>
    <span>Patents (KR, Granted)</span>
  </h2>

<div class="pub-list icnsl-catalog-list icnsl-catalog-list--patents icnsl-catalog-list--kr">

{% comment %}
새 한국 특허는 아래 kr_patent_no 초기화 줄 다음에 추가하세요.
각 특허의 assign ... plus: 1 줄부터 pub-entry의 닫는 div까지 복사하고,
pub-citation 안의 특허 정보만 수정하면 됩니다.
초기화 줄(assign kr_patent_no = 0)은 이 목록에 한 번만 둡니다.
{% endcomment %}
{% assign kr_patent_no = 0 %}

{% assign kr_patent_no = kr_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-pk{{ kr_patent_no }}">
  <div class="pub-no">[PK{{ kr_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/KR102992232B1/ko" target="_blank" rel="noopener noreferrer" title="특허 원문 보기 (새 탭에서 열림)">KR#10-2992232</a>,
    “WLAN 시스템에서 상향링크 빔포밍을 위한 장치 및 방법,”
    Eunsung Jeon, Chulho Chung, Myeongjin Kim, and <strong>Jonghun Han</strong>,
    2026.07.16.
  </div>
</div>

{% assign kr_patent_no = kr_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-pk{{ kr_patent_no }}">
  <div class="pub-no">[PK{{ kr_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/KR102976771B1/ko" target="_blank" rel="noopener noreferrer" title="특허 원문 보기 (새 탭에서 열림)">KR#10-2976771</a>,
    “시 민감 네트워크 패킷의 무선 송수신 시 데이터 송수신 방법 및 장치,”
    Ilmu Byun, <strong>Jonghun Han</strong>, Youngju Kim, Sungsoo Park, and Yong-ki Yoon,
    2026.06.09.
  </div>
</div>

{% assign kr_patent_no = kr_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-pk{{ kr_patent_no }}">
  <div class="pub-no">[PK{{ kr_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/KR102976784B1/ko" target="_blank" rel="noopener noreferrer" title="특허 원문 보기 (새 탭에서 열림)">KR#10-2976784</a>,
    “시 민감 네트워크 패킷의 무선 송수신을 위한 무선 플로우 해지 방법 및 장치,”
    Ilmu Byun, <strong>Jonghun Han</strong>, Youngju Kim, Sungsoo Park, and Yong-ki Yoon,
    2026.06.09.
  </div>
</div>

{% assign kr_patent_no = kr_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-pk{{ kr_patent_no }}">
  <div class="pub-no">[PK{{ kr_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/KR102894598B1/ko" target="_blank" rel="noopener noreferrer" title="특허 원문 보기 (새 탭에서 열림)">KR#10-2894598</a>,
    “고장 방지 기능을 갖는 멀티-억세스 에지 컴퓨팅 시스템 및 이의 고장 방지 방법,”
    Seongho Kwon, Ilmu Byun, Youngju Kim, Sungsoo Park, and <strong>Jonghun Han</strong>,
    2025.11.28.
  </div>
</div>

{% assign kr_patent_no = kr_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-pk{{ kr_patent_no }}">
  <div class="pub-no">[PK{{ kr_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/KR102846763B1/ko" target="_blank" rel="noopener noreferrer" title="특허 원문 보기 (새 탭에서 열림)">KR#10-2846763</a>,
    “듀얼 빔포밍 피드백을 위한 적응적 코드북을 이용하는 장치, 방법 및 이를 포함하는 무선 통신 시스템,”
    Eunsung Jeon, Wookbong Lee, Myeongjin Kim, and <strong>Jonghun Han</strong>,
    2025.08.14.
  </div>
</div>

{% assign kr_patent_no = kr_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-pk{{ kr_patent_no }}">
  <div class="pub-no">[PK{{ kr_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/KR102755897B1/ko" target="_blank" rel="noopener noreferrer" title="특허 원문 보기 (새 탭에서 열림)">KR#10-2755897</a>,
    “EDCA 파라미터를 동적으로 조절하는 방법 및 장치,”
    <strong>Jonghun Han</strong>, Jung-tai Kim, and Yong-ki Yoon,
    2025.01.13.
  </div>
</div>

{% assign kr_patent_no = kr_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-pk{{ kr_patent_no }}">
  <div class="pub-no">[PK{{ kr_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/KR102572878B1/ko" target="_blank" rel="noopener noreferrer" title="특허 원문 보기 (새 탭에서 열림)">KR#10-2572878</a>,
    “공간 재사용을 이용하여 데이터를 전송하는 무선 통신 장치 및 이를 이용한 데이터 통신 방법,”
    <strong>Jonghun Han</strong>, Young-Wook Son, Sung-Hyun Choi, Seong-Won Kim, and Kang-Hyun Lee,
    2023.08.30.
  </div>
</div>

{% assign kr_patent_no = kr_patent_no | plus: 1 %}
<div class="pub-entry" id="pub-pk{{ kr_patent_no }}">
  <div class="pub-no">[PK{{ kr_patent_no }}]</div>
  <div class="pub-citation">
    <a class="patent-link" href="https://patents.google.com/patent/KR101168635B1/ko" target="_blank" rel="noopener noreferrer" title="특허 원문 보기 (새 탭에서 열림)">KR#10-1168635</a>,
    “셀간 간섭 감소를 위한 펨토 기지국 및 이를 이용한 신호 전송 방법,”
    Sae Woong Bahk, Sung Guk Yoon, <strong>Jonghun Han</strong>, Young Han Kim, and Ik Hyeon Kim,
    2012.07.25.
  </div>
</div>

</div>
</section>
{% endcapture %}

<div class="icnsl-showcase icnsl-showcase--patents">
<header class="icnsl-showcase__intro">
  <div class="icnsl-showcase__glyph" aria-hidden="true"><i class="fas fa-certificate"></i></div>
  <div class="icnsl-showcase__intro-copy">
    <div class="icnsl-showcase__eyebrow">Intellectual Property</div>
    <p class="icnsl-showcase__lead">Granted patents covering wireless communication, multi-link operation, channel access, and network systems.</p>
    <div class="icnsl-showcase__tags" aria-label="Granted patent counts">
      <span>United States · {{ us_patent_no }} granted</span><span>Republic of Korea · {{ kr_patent_no }} granted</span><span>Total · {{ us_patent_no | plus: kr_patent_no }} granted</span>
    </div>
  </div>
</header>

{{ patent_catalog }}
</div>

