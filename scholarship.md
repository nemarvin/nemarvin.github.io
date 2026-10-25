
---
layout: page
title: "Scholarship"
---

<!-- Scholarship page: collapsible publication lists with Paper/Roboto styling. -->

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600;1,700&display=swap');

/* Style the existing Jekyll page, not an additional inset panel. */
html:has(.scholarship-page) body,
body:has(.scholarship-page) > article,
body:has(.scholarship-page) > article > header {
  background-color: #f4efe4 !important;
}

body:has(.scholarship-page) > article > header,
body:has(.scholarship-page) > article > header h1 {
  text-align: center !important;
  text-align-last: center !important;
}

body:has(.scholarship-page) > article > header h1,
body:has(.scholarship-page) > article > header h1 a {
  color: #332f2b !important;
  font-family: Roboto, "Helvetica Neue", Arial, sans-serif;
}

body:has(.scholarship-page) > article > header h1 {
  font-size: 1.5rem !important;
}

.scholarship-page {
  --scholarship-ink: #332f2b;
  --scholarship-muted: #746b62;
  --scholarship-rule: #8a2f2f;
  --scholarship-soft-rule: #d4c8b8;
  --scholarship-link: #7b2929;
  --scholarship-link-hover: #4f1717;

  box-sizing: border-box;
  max-width: none;
  margin: 0;
  padding: 0;
  background: transparent;
  color: var(--scholarship-ink);
  font-family: Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 18px;
  line-height: 1.68;
  text-align: left !important;
  text-align-last: auto !important;
}

.scholarship-page *,
.scholarship-page *::before,
.scholarship-page *::after {
  box-sizing: border-box;
}

/* Prevent inherited justification or centering. */
.scholarship-page p,
.scholarship-page .scholarship-item,
.scholarship-page .scholarship-item a,
.scholarship-page .scholarship-intro {
  text-align: left !important;
  text-align-last: auto !important;
}

/* Links */
.scholarship-page a,
.scholarship-page a:visited {
  color: var(--scholarship-link) !important;
  text-underline-offset: 0.12em;
}

.scholarship-page a:hover,
.scholarship-page a:focus {
  color: var(--scholarship-link-hover) !important;
  text-decoration-color: currentColor;
}

/* Introduction */
.scholarship-page .scholarship-intro {
  margin: 0 0 1.4rem;
  font-size: 0.92em;
}

/* Collapsible publication categories.
   Each full-width divider is exactly 2px thick.
   Borders occur only once between adjacent sections. */
.scholarship-page details.scholarship-group {
  margin: 0;
  border-top: 2px solid var(--scholarship-soft-rule);
  border-bottom: 0;
}

.scholarship-page details.scholarship-group:last-of-type {
  border-bottom: 2px solid var(--scholarship-soft-rule);
}

/* Section headings */
.scholarship-page details.scholarship-group > summary {
  display: block;
  position: relative;
  margin: 0;
  padding: 1.3rem 2.5rem 1.4rem 0;
  cursor: pointer;
  list-style: none;
  color: var(--scholarship-ink);
  font-family: Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 1.35rem;
  font-weight: 600;
  line-height: 1.25;
  text-align: left !important;
  text-align-last: left !important;
}

.scholarship-page details.scholarship-group > summary::-webkit-details-marker {
  display: none;
}

.scholarship-page details.scholarship-group > summary::marker {
  content: "";
}

/* Short burgundy accent line */
.scholarship-page details.scholarship-group > summary::after {
  content: "";
  display: block;
  width: 72px;
  height: 2px;
  margin: 0.7rem 0 0;
  background: var(--scholarship-rule);
}

/* Expand/collapse symbols */
.scholarship-page details.scholarship-group > summary::before {
  content: "+";
  position: absolute;
  right: 0.65rem;
  top: 1.3rem;
  color: var(--scholarship-link);
  font-size: 1.35rem;
  font-weight: 400;
}

.scholarship-page details.scholarship-group[open] > summary::before {
  content: "−";
}

.scholarship-page details.scholarship-group > summary:hover {
  color: var(--scholarship-link);
}

.scholarship-page details.scholarship-group > summary:focus-visible {
  outline: 2px solid var(--scholarship-rule);
  outline-offset: -2px;
}

/* Single-column publication lists */
.scholarship-page .scholarship-list {
  padding: 0.15rem 0 1.4rem;
}

.scholarship-page .scholarship-item {
  margin: 0;
  padding: 1.15rem 0;
  border-bottom: 1px solid var(--scholarship-soft-rule);
}

.scholarship-page .scholarship-item:last-child {
  border-bottom: 0;
}

/* Publication images */
.scholarship-page .scholarship-item img {
  display: block;
  width: 200px;
  max-width: 100%;
  height: auto;
  margin: 0 0 0.45rem;
}

/* Publication text */
.scholarship-page .scholarship-item p {
  margin: 0 0 0.5rem;
  font-size: 0.95em;
  line-height: 1.55;
}

.scholarship-page .scholarship-item p:last-child {
  margin-bottom: 0;
}

/* Embedded publication */
.scholarship-page .scholarship-item iframe {
  display: block;
  width: 300px;
  max-width: 100%;
  height: 260px;
  margin-bottom: 0.45rem;
  border: 0;
}

/* Decorative image */
.scholarship-page .scholarship-interlude {
  width: 58%;
  max-width: 420px;
  margin: 2.4rem auto 2.65rem;
}

.scholarship-page .scholarship-interlude img {
  display: block;
  width: 100%;
  height: auto;
}

/* Back to top */
.scholarship-page .scholarship-back {
  margin: 2rem 0 0;
  font-size: 0.84em;
}

/* Mobile styling */
@media (max-width: 540px) {
  .scholarship-page {
    font-size: 17px;
    line-height: 1.6;
  }

  body:has(.scholarship-page) > article > header h1 {
    font-size: 1.35rem !important;
  }

  .scholarship-page details.scholarship-group > summary {
    font-size: 1.25rem;
  }

  .scholarship-page .scholarship-interlude {
    width: 78%;
  }
}
</style>

<div class="scholarship-page">

  <p class="scholarship-intro">
    For a full list, see my
    <a href="https://scholar.google.com/citations?user=8jtmeYUAAAAJ&amp;hl=en">Google Scholar profile</a>.
  </p>

  <!-- ARTICLES AND BOOK CHAPTERS -->
  <details class="scholarship-group">
    <summary>Articles &amp; Book Chapters</summary>
    <div class="scholarship-list">

      <div class="scholarship-item">
        <img src="{{ site.baseurl }}/pub5.png"
             alt="The 'Ambroise Affair'"
             loading="lazy">
        <p>
          <strong>
            <a href="https://drive.google.com/file/d/13HDaWQDQkAgnthVORFdYn4tqqhlsAguF/view?usp=sharing">The 'Ambroise Affair'...</a>
          </strong>
        </p>
      </div>

      <div class="scholarship-item">
        <img src="{{ site.baseurl }}/pub2.png"
             alt="Gender, Family, and Social Control"
             loading="lazy">
        <p>
          <strong>
            <a href="https://drive.google.com/file/d/1wrS2phtMkgjha5g6sPnsUbgIQzGT8S3Z/view?usp=sharing">Gender, Family, and Social Control...</a>
          </strong>
        </p>
      </div>

      <div class="scholarship-item">
        <img src="{{ site.baseurl }}/pub3.png"
             alt="‘Free and Naturalized Frenchwomen’"
             loading="lazy">
        <p>
          <strong>
            <a href="https://drive.google.com/file/d/1ro_OSNdbyXvhlbsgDIOxa0Bu_vPYurnD/view?usp=sharing">‘Free and Naturalized Frenchwomen’...</a>
          </strong>
        </p>
      </div>

      <div class="scholarship-item">
        <img src="{{ site.baseurl }}/pub7.png"
             alt="‘A Thousand Prejudices’"
             loading="lazy">
        <p>
          <strong>
            <a href="https://drive.google.com/file/d/11tlLSyZsk0CGviQG3r8ItdsuyUudYvXS/view?usp=sharing">‘A Thousand Prejudices’...</a>
          </strong>
        </p>
      </div>

    </div>
  </details>

  <!-- ESSAYS -->
  <details class="scholarship-group">
    <summary>Essays</summary>
    <div class="scholarship-list">

      <div class="scholarship-item">
        <img src="{{ site.baseurl }}/pub0.png"
             alt="Gender in Slave and Post-Emancipation Societies"
             loading="lazy">
        <p>
          <strong>
            <a href="https://doi.org/10.4000/11oa3">Gender in Slave and Post-Emancipation...</a>
          </strong>
        </p>
      </div>

      <div class="scholarship-item">
        <img src="{{ site.baseurl }}/pub4.png"
             alt="France and its Empire in the Indian Ocean"
             loading="lazy">
        <p>
          <strong>
            <a href="https://drive.google.com/file/d/1E-aXR8FHurDIJGhWrcERDPEunQA0EhkR/view?usp=sharing">France and its Empire in the Indian Ocean...</a>
          </strong>
        </p>
      </div>

      <div class="scholarship-item">
        <img src="{{ site.baseurl }}/pub6.png"
             alt="Instructions du Ministère de la Marine"
             loading="lazy">
        <p>
          <strong>
            <a href="https://www.cairn.info/revue-outre-mers-2015-2-page-285.htm">Instructions du Ministère de la Marine...</a>
          </strong>
        </p>
      </div>

    </div>
  </details>

  <!-- DISSERTATION -->
  <details class="scholarship-group">
    <summary>Dissertation</summary>
    <div class="scholarship-list">

      <div class="scholarship-item">
        <p>
          <strong>
            <a href="https://drive.google.com/file/d/1ywHXi5mUUO-OqxAZwqNq_DLvdJ8_UHwt/view?usp=sharing">Ph.D. Dissertation</a>
          </strong>
        </p>
      </div>

    </div>
  </details>

  <!-- PUBLIC SCHOLARSHIP -->
  <details class="scholarship-group">
    <summary>Public Scholarship</summary>
    <div class="scholarship-list">

      <div class="scholarship-item">
        <img src="{{ site.baseurl }}/pub1.png"
             alt="Église, État, et Esclavage"
             loading="lazy">
        <p>
          <strong>
            <a href="https://www.portail-esclavage-reunion.fr/documentaires/l-esclavage/leglise-et-lesclavage/eglise-etat-et-esclavage-les-familles-vendues-comme-biens-nationaux-a-lile-de-la-reunion-pendant-la-revolution-francaise/">Église, État, et Esclavage...</a>
          </strong>
        </p>
      </div>

      <div class="scholarship-item">
        <img src="{{ site.baseurl }}/pub0.jpg"
             alt="Looking for 'Petit Jean'"
             loading="lazy">
        <p>
          <strong>
            <a href="https://64parishes.org/looking-for-petit-jean">Looking for 'Petit Jean'...</a>
          </strong>
        </p>
      </div>

      <div class="scholarship-item">
        <iframe
          src="https://v.calameo.com/?bkcode=00522093399f6cf3724ae&amp;mode=mini&amp;showsharemenu=false&amp;clickto=view&amp;clicktarget=_blank"
          width="300"
          height="260"
          title="Digital Publication"
          loading="lazy"
          allowfullscreen>
        </iframe>
        <p>
          <strong>
            <a href="https://www.portail-esclavage-reunion.fr/dossiers-documentaires/laffaire-abby-guy-le-combat-dune-femme-pour-la-liberte-dans-le-sud-des-etats-unis-exposition-musee-de-villele/">“L’affaire Abby Guy : Le combat d’une femme pour la liberté dans le Sud des États-Unis”</a>
          </strong>
        </p>
      </div>

    </div>
  </details>

  <!-- DECORATIVE IMAGE -->
  <div class="scholarship-interlude">
    <img src="{{ site.baseurl }}/3bassins.gif"
         alt="3 Bassins"
         loading="lazy">
  </div>

  <!-- BACK TO TOP -->
  <p class="scholarship-back">
    <a href="#">Back to Top</a>
  </p>

</div>
