---
title: "📞 Contact"
permalink: /contact/
author_profile: true
---

<style>
/* Contact page title style */
.page__title {
  padding-bottom: 0.45em;
  border-bottom: 1px solid var(--global-border-color);
  letter-spacing: 0.06em;
}

.page__title::before {
  content: none !important;
}

/* Contact page layout */
.page__content .contact-list {
  max-width: 920px;
  width: 100%;
  margin: 1.6rem 0 2.2rem;
}

.page__content .contact-row {
  display: grid;
  grid-template-columns: 2.25rem minmax(0, 1fr);
  column-gap: 0.85rem;
  align-items: start;

  margin: 0 0 1.35rem;
  line-height: 1.55;
}

.page__content .contact-icon {
  width: 2.1rem;
  min-height: 2.1rem;

  display: flex;
  align-items: center;
  justify-content: center;

  font-size: 1.25rem;
  color: var(--global-text-color);
}

.page__content .contact-text {
  font-size: 1.08em;
  line-height: 1.55;
  color: var(--global-text-color);
}

/* Location block */
.page__content .contact-location-list {
  width: 100%;
  margin-top: 0.1rem;
}

.page__content .contact-location-row {
  display: grid;
  grid-template-columns: 8.8rem minmax(0, 1fr);
  column-gap: 1rem;
  align-items: baseline;

  margin: 0 0 0.55rem;
  line-height: 1.55;
}

.page__content .contact-location-row:last-child {
  margin-bottom: 0;
}

.page__content .contact-location-label {
  font-weight: 800;
  white-space: nowrap;
  color: var(--global-text-color);
}

.page__content .contact-location-text {
  color: var(--global-text-color);
}

.page__content .contact-address {
  white-space: normal;
}

/* Google map block */
.page__content .contact-map {
  position: relative;

  max-width: 920px;
  width: 100%;

  margin: 2rem 0 2.5rem;
  overflow: hidden;

  border-radius: 0.45rem;
  background: rgba(255, 255, 255, 0.035);
  box-shadow: 0 1px 6px rgba(0, 0, 0, 0.18);
}

.page__content .contact-map iframe {
  display: block;
  width: 100%;
  height: 430px;
  border: 0;
}

/* Button on the map */
.page__content .contact-map-link {
  position: absolute;
  top: 0.85rem;
  left: 0.85rem;
  z-index: 5;

  padding: 0.55rem 0.75rem;

  border-radius: 0.25rem;
  background: #ffffff;
  color: #1a73e8 !important;

  font-size: 0.88em;
  font-weight: 700;
  line-height: 1;

  text-decoration: none !important;
  box-shadow: 0 1px 4px rgba(0, 0, 0, 0.22);
}

.page__content .contact-map-link:hover {
  text-decoration: none !important;
  background: #f7f7f7;
}

.page__content .contact-map-link i {
  margin-left: 0.25rem;
  font-size: 0.82em;
}

/* Mobile layout */
@media (max-width: 600px) {
  .page__content .contact-row {
    grid-template-columns: 1.9rem minmax(0, 1fr);
    column-gap: 0.65rem;
    margin-bottom: 1.2rem;
  }

  .page__content .contact-icon {
    width: 1.8rem;
    min-height: 1.8rem;
    font-size: 1.05rem;
  }

  .page__content .contact-text {
    font-size: 1em;
  }

  .page__content .contact-location-row {
    grid-template-columns: 1fr;
    row-gap: 0.05rem;
    margin-bottom: 0.75rem;
  }

  .page__content .contact-location-label {
    margin-bottom: 0.05rem;
  }

  .page__content .contact-map iframe {
    height: 340px;
  }

  .page__content .contact-map-link {
    top: 0.65rem;
    left: 0.65rem;
    font-size: 0.82em;
  }
}
</style>

<div class="contact-list">

<div class="contact-row">
  <div class="contact-icon">
    <i class="fas fa-at"></i>
  </div>
  <div class="contact-text">
    jhan at sejong dot ac dot kr
  </div>
</div>

<div class="contact-row">
  <div class="contact-icon">
    <i class="fas fa-map-marker-alt"></i>
  </div>

  <div class="contact-text">

    <div class="contact-location-list">

      <div class="contact-location-row">
        <div class="contact-location-label">Faculty Office</div>
        <div class="contact-location-text">Room 704, Daeyang AI Center</div>
      </div>

      <div class="contact-location-row">
        <div class="contact-location-label">Student Lab</div>
        <div class="contact-location-text">Room XXX, Daeyang AI Center</div>
      </div>

      <div class="contact-location-row">
        <div class="contact-location-label">Address</div>
        <div class="contact-location-text contact-address">
          209, Neungdong-ro, Gwangjin-gu, Seoul 05006, South Korea (Sejong University)
        </div>
      </div>

    </div>

  </div>
</div>

</div>

<div class="contact-map">
  <a class="contact-map-link" href="https://maps.app.goo.gl/btpSMxDUDCLdNDNW8" target="_blank" rel="noopener noreferrer">
    Open in Google Maps <i class="fas fa-external-link-alt"></i>
  </a>

  <iframe
    src="https://www.google.com/maps?q=Daeyang%20AI%20Center%2C%20Sejong%20University%2C%20Seoul%2C%20South%20Korea&amp;output=embed"
    width="100%"
    height="430"
    style="border:0;"
    allowfullscreen=""
    loading="lazy"
    referrerpolicy="no-referrer-when-downgrade">
  </iframe>
</div>
