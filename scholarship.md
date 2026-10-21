---
layout: page
title: "Scholarship"
---

<!-- Scholarship page: matched to Teaching Materials (Paper palette, Roboto, seamless Jekyll shell). -->

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600;1,700&display=swap');

/* Use the existing Jekyll page as the paper surface, not an inset panel. */
html:has(.scholarship-page) body,
body:has(.scholarship-page) > article,
body:has(.scholarship-page) > article > header {
  background-color: #f4efe4 !important;
}

/* Center the Jekyll-generated page title without altering the navigation bar. */
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
  font-size: 1.7rem !important;
}

.scholarship-page {
  --scholarship-paper: #f4efe4;
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

/* All body text and entry titles remain flush left, never justified. */
.scholarship-page p,
.scholarship-page h3,
.scholarship-page h4,
.scholarship-page article,
.scholarship-page section,
.scholarship-page .scholarship-entry > div,
.scholarship-page a {
  text-align: left !important;
  text-align-last: auto !important;
}

.scholarship-page *,
.scholarship-page *::before,
.scholarship-page *::after {
  box-sizing: border-box;
}

/* The same centered small headings and burgundy rules as Teaching Materials. */
.scholarship-page h2 {
  margin: 0 0 1.65rem;
  padding: 0;
  border: 0 !important;
  color: var(--scholarship-ink);
  font-family: Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 1.6rem;
  font-weight: 600;
  line-height: 1.25;
  text-align: center !important;
  text-align-last: center !important;
}
.scholarship-page h2::after {
  content: "";
  display: block;
  width: 72px;
  height: 2px;
  margin: 0.7rem auto 0;
  background: var(--scholarship-rule);
}

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

.scholarship-page .scholarship-intro {
  margin: 0 0 2.7rem;
  font-size: 0.92em;
}

.scholarship-page .scholarship-section {
  margin-bottom: 2.35rem;
}

/* Exactly the Teaching Materials grid and card spacing. */
.scholarship-page .scholarship-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(min(100%, 330px), 1fr));
  column-gap: 1.8rem;
}
.scholarship-page .scholarship-entry {
  display: grid;
  grid-template-columns: 100px minmax(0, 1fr);
  gap: 0.95rem;
  align-items: start;
  padding: 1.35rem 0;
  border-bottom: 1px solid var(--scholarship-soft-rule);
}
.scholarship-page .scholarship-entry img {
  display: block;
  width: 100%;
  height: auto;
  max-height: 165px;
  object-fit: contain;
  object-position: top left;
}
.scholarship-page .scholarship-entry p {
  margin: 0 0 0.55rem;
  font-size: 0.88em;
  line-height: 1.5;
}
.scholarship-page .scholarship-entry p:first-child {
  font-size: 0.97em;
  line-height: 1.4;
}
.scholarship-page .scholarship-entry p:last-child {
  margin-bottom: 0;
}

/* Keep the original interactive Calaméo preview usable and legible. */
.scholarship-page .scholarship-entry--embed {
  grid-column: 1 / -1;
  grid-template-columns: minmax(0, 300px) minmax(0, 1fr);
  gap: 1.25rem;
}
.scholarship-page .scholarship-entry--embed iframe {
  display: block;
  width: 300px;
  max-width: 100%;
  height: 260px;
  border: 0;
}

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

.scholarship-page .scholarship-back {
  margin: 2rem 0 0;
  font-size: 0.84em;
}

@media (max-width: 650px) {
  .scholarship-page .scholarship-entry--embed {
    grid-template-columns: minmax(0, 1fr);
  }
}
@media (max-width: 540px) {
  .scholarship-page {
    font-size: 17px;
    line-height: 1.6;
  }
  .scholarship-page h2 {
    font-size: 1.4rem;
  }
  body:has(.scholarship-page) > article > header h1 {
    font-size: 1.55rem !important;
  }
  .scholarship-page .scholarship-entry {
    grid-template-columns: 86px minmax(0, 1fr);
    gap: 0.8rem;
  }
  .scholarship-page .scholarship-entry--embed {
    grid-template-columns: minmax(0, 1fr);
  }
  .scholarship-page .scholarship-interlude {
    width: 78%;
  }
}
</style>

<div class="scholarship-page">

  <p class="scholarship-intro">For a full list, see my <a href="https://scholar.google.com/citations?user=8jtmeYUAAAAJ&amp;hl=en">Google Scholar profile</a>.</p>

  <section class="scholarship-section" aria-labelledby="scholarship-articles">
    <h2 id="scholarship-articles">Articles &amp; Book Chapters</h2>
    <div class="scholarship-grid">

      <article class="scholarship-entry">
        <img src="{{ site.baseurl }}/pub5.png" alt="The 'Ambroise Affair'" loading="lazy">
        <div>
          <p><strong><a href="https://drive.google.com/file/d/13HDaWQDQkAgnthVORFdYn4tqqhlsAguF/view?usp=sharing">The 'Ambroise Affair'...</a></strong></p>
        </div>
      </article>

      <article class="scholarship-entry">
        <img src="{{ site.baseurl }}/pub2.png" alt="Gender, Family, and Social Control" loading="lazy">
        <div>
          <p><strong><a href="https://drive.google.com/file/d/1wrS2phtMkgjha5g6sPnsUbgIQzGT8S3Z/view?usp=sharing">Gender, Family, and Social Control...</a></strong></p>
        </div>
      </article>

      <article class="scholarship-entry">
        <img src="{{ site.baseurl }}/pub3.png" alt="‘Free and Naturalized Frenchwomen’" loading="lazy">
        <div>
          <p><strong><a href="https://drive.google.com/file/d/1ro_OSNdbyXvhlbsgDIOxa0Bu_vPYurnD/view?usp=sharing">‘Free and Naturalized Frenchwomen’...</a></strong></p>
        </div>
      </article>

      <article class="scholarship-entry">
        <img src="{{ site.baseurl }}/pub7.png" alt="‘A Thousand Prejudices’" loading="lazy">
        <div>
          <p><strong><a href="https://drive.google.com/file/d/11tlLSyZsk0CGviQG3r8ItdsuyUudYvXS/view?usp=sharing">‘A Thousand Prejudices’...</a></strong></p>
        </div>
      </article>

    </div>
  </section>

  <section class="scholarship-section" aria-labelledby="scholarship-essays">
    <h2 id="scholarship-essays">Essays</h2>
    <div class="scholarship-grid">

      <article class="scholarship-entry">
        <img src="{{ site.baseurl }}/pub0.png" alt="Gender in Slave and Post-Emancipation Societies" loading="lazy">
        <div>
          <p><strong><a href="https://doi.org/10.4000/11oa3">Gender in Slave and Post-Emancipation...</a></strong></p>
        </div>
      </article>

      <article class="scholarship-entry">
        <img src="{{ site.baseurl }}/pub4.png" alt="France and its Empire in the Indian Ocean" loading="lazy">
        <div>
          <p><strong><a href="https://drive.google.com/file/d/1E-aXR8FHurDIJGhWrcERDPEunQA0EhkR/view?usp=sharing">France and its Empire in the Indian Ocean...</a></strong></p>
        </div>
      </article>

      <article class="scholarship-entry">
        <img src="{{ site.baseurl }}/pub6.png" alt="Instructions du Ministère de la Marine" loading="lazy">
        <div>
          <p><strong><a href="https://www.cairn.info/revue-outre-mers-2015-2-page-285.htm">Instructions du Ministère de la Marine...</a></strong></p>
        </div>
      </article>

    </div>
  </section>

  <section class="scholarship-section" aria-labelledby="scholarship-public">
    <h2 id="scholarship-public">Public Scholarship</h2>
    <div class="scholarship-grid">

      <article class="scholarship-entry">
        <img src="{{ site.baseurl }}/pub1.png" alt="Église, État, et Esclavage" loading="lazy">
        <div>
          <p><strong><a href="https://www.portail-esclavage-reunion.fr/documentaires/l-esclavage/leglise-et-lesclavage/eglise-etat-et-esclavage-les-familles-vendues-comme-biens-nationaux-a-lile-de-la-reunion-pendant-la-revolution-francaise/">Église, État, et Esclavage...</a></strong></p>
        </div>
      </article>

      <article class="scholarship-entry">
        <img src="{{ site.baseurl }}/pub0.jpg" alt="Looking for 'Petit Jean'" loading="lazy">
        <div>
          <p><strong><a href="https://64parishes.org/looking-for-petit-jean">Looking for 'Petit Jean'...</a></strong></p>
        </div>
      </article>

      <article class="scholarship-entry scholarship-entry--embed">
        <iframe
          src="https://v.calameo.com/?bkcode=00522093399f6cf3724ae&amp;mode=mini&amp;showsharemenu=false&amp;clickto=view&amp;clicktarget=_blank"
          width="300"
          height="260"
          title="Digital Publication"
          loading="lazy"
          allowfullscreen>
        </iframe>
        <div>
          <p><strong><a href="https://www.portail-esclavage-reunion.fr/dossiers-documentaires/laffaire-abby-guy-le-combat-dune-femme-pour-la-liberte-dans-le-sud-des-etats-unis-exposition-musee-de-villele/">“L’affaire Abby Guy : Le combat d’une femme pour la liberté dans le Sud des États-Unis”</a></strong></p>
        </div>
      </article>

    </div>
  </section>

  <div class="scholarship-interlude">
    <img src="{{ site.baseurl }}/3bassins.gif" alt="3 Bassins" loading="lazy">
  </div>

  <p class="scholarship-back"><a href="#">Back to Top</a></p>

</div>
