---
layout: page
title: "Digital Projects"
---

<!-- Digital Projects: Paper/Roboto styling matching Teaching Materials and Scholarship. -->

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600;1,700&display=swap');

/* Use the existing Jekyll page as the paper surface, with no extra inset frame. */
html:has(.digital-projects-page) body,
body:has(.digital-projects-page) > article,
body:has(.digital-projects-page) > article > header {
  background-color: #f4efe4 !important;
}
body:has(.digital-projects-page) > article > header,
body:has(.digital-projects-page) > article > header h1 {
  text-align: center !important;
  text-align-last: center !important;
}
body:has(.digital-projects-page) > article > header h1,
body:has(.digital-projects-page) > article > header h1 a {
  color: #332f2b !important;
  font-family: Roboto, "Helvetica Neue", Arial, sans-serif;
}
body:has(.digital-projects-page) > article > header h1 {
  font-size: 1.7rem !important;
}

.digital-projects-page {
  --project-ink: #332f2b;
  --project-muted: #746b62;
  --project-rule: #8a2f2f;
  --project-soft-rule: #d4c8b8;
  --project-link: #7b2929;
  --project-link-hover: #4f1717;

  box-sizing: border-box;
  max-width: none;
  padding: 0;
  margin: 0;
  color: var(--project-ink);
  background: transparent;
  font-family: Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 18px;
  line-height: 1.68;
  text-align: left !important;
  text-align-last: auto !important;
}
.digital-projects-page *,
.digital-projects-page *::before,
.digital-projects-page *::after { box-sizing: border-box; }

/* Prevent inherited justification (including on short paragraphs and list items). */
.digital-projects-page p,
.digital-projects-page ul,
.digital-projects-page li,
.digital-projects-page .project-body,
.digital-projects-page .project-body strong {
  text-align: left !important;
  text-align-last: auto !important;
}
.digital-projects-page a,
.digital-projects-page a:visited {
  color: var(--project-link) !important;
  text-underline-offset: 0.12em;
}
.digital-projects-page a:hover,
.digital-projects-page a:focus {
  color: var(--project-link-hover) !important;
  text-decoration-color: currentColor;
}

.digital-projects-page .project-intro {
  margin: 0 0 1.4rem;
  font-size: 0.92em;
}

/* The same restrained collapsible section treatment as Scholarship. */
.digital-projects-page details.project-group {
  margin: 0;
  border-bottom: 1px solid var(--project-soft-rule);
}
.digital-projects-page details.project-group:first-of-type {
  border-top: 1px solid var(--project-soft-rule);
}
.digital-projects-page details.project-group > summary {
  display: block;
  position: relative;
  margin: 0;
  padding: 1.3rem 2.5rem 1.4rem;
  cursor: pointer;
  list-style: none;
  color: var(--project-ink);
  font-family: Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 1.6rem;
  font-weight: 600;
  line-height: 1.3;
  text-align: center !important;
  text-align-last: center !important;
}
.digital-projects-page details.project-group > summary::-webkit-details-marker { display: none; }
.digital-projects-page details.project-group > summary::marker { content: ""; }
.digital-projects-page details.project-group > summary::after {
  content: "";
  display: block;
  width: 72px;
  height: 2px;
  margin: 0.7rem auto 0;
  background: var(--project-rule);
}
.digital-projects-page details.project-group > summary::before {
  content: "+";
  position: absolute;
  right: 0.65rem;
  top: 1.3rem;
  color: var(--project-link);
  font-size: 1.35rem;
  font-weight: 400;
}
.digital-projects-page details.project-group[open] > summary::before { content: "−"; }
.digital-projects-page details.project-group > summary:hover { color: var(--project-link); }
.digital-projects-page details.project-group > summary:focus-visible {
  outline: 2px solid var(--project-rule);
  outline-offset: -2px;
}
.digital-projects-page .project-body {
  padding: 0.35rem 0 1.5rem;
}
.digital-projects-page .project-body p {
  margin: 0 0 1rem;
  line-height: 1.65;
}
.digital-projects-page .project-body ul {
  padding-left: 1.5rem;
  margin: 0 0 1.15rem;
}
.digital-projects-page .project-body li {
  margin: 0.25rem 0;
  overflow-wrap: anywhere;
}
.digital-projects-page .project-body .project-links-label {
  margin-bottom: 0.2rem;
}
/* Show source images clearly, without forced cropping or mismatched oversized images. */
.digital-projects-page .project-images {
  display: flex;
  flex-wrap: wrap;
  align-items: flex-start;
  justify-content: flex-start;
  gap: 1rem;
  margin: 0 0 1.2rem;
}
.digital-projects-page .project-images img {
  display: block;
  width: auto;
  max-width: 100%;
  max-height: 300px;
  height: auto;
  object-fit: contain;
  object-position: left top;
}
.digital-projects-page .project-images--pair img {
  max-width: min(100%, 310px);
  max-height: 260px;
}
.digital-projects-page .project-interlude {
  width: 58%;
  max-width: 420px;
  margin: 2.4rem auto 2.65rem;
}
.digital-projects-page .project-interlude img {
  display: block;
  width: 100%;
  height: auto;
}
.digital-projects-page .project-back {
  margin: 2rem 0 0;
  font-size: 0.84em;
}
@media (max-width: 540px) {
  .digital-projects-page { font-size: 17px; line-height: 1.6; }
  body:has(.digital-projects-page) > article > header h1 { font-size: 1.55rem !important; }
  .digital-projects-page details.project-group > summary {
    font-size: 1.35rem;
    padding-left: 1.25rem;
    padding-right: 2.25rem;
  }
  .digital-projects-page .project-interlude { width: 78%; }
  .digital-projects-page .project-images img,
  .digital-projects-page .project-images--pair img { max-width: 100%; }
}
</style>

<div class="digital-projects-page">
  <p class="project-intro">Digital history projects in progress. Updates posted here.</p>

  <details class="project-group">
    <summary>Arkansas Créole: Recovering a Lost Vernacular Landscape</summary>
    <div class="project-body">
      <div class="project-images">
        <img src="{{ site.baseurl }}/image1.png" alt="Screenshot of Arkansas Creole Map" loading="lazy">
      </div>
      <p>Map App Companion to <em>Arkansas Créole</em>. Click the points on the map to reveal the stories behind the place names.</p>
      <ul>
        <li><strong>Layers:</strong> Toggle layers via the "Layers" button.</li>
        <li><strong>Info:</strong> Click map points for information pop-ups on the left.</li>
        <li><strong>Search:</strong> Search the database of historic names, or locate contemporary geographical features using the search function.</li>
      </ul>
      <p>The “French period” of Arkansas history has long been romanticized, whitewashed, or altogether dismissed as inconsequential. This digital history project shines light on the contributions to Arkansas’s culture and geography made by French-speaking people of European, Indigenous, and African descent who lived alongside the Ogahpah Nation under French, Spanish, and early U.S. rule. The accompanying map seeks to recover the stories of the people behind the names of many of the state's settlements, mountains, bayous, and streams.</p>
      <p class="project-links-label"><strong>Explore:</strong></p>
      <ul>
        <li><a href="https://www.arcgis.com/apps/instant/sidebar/index.html?appid=274918c16c384b2eae7ead967f951336">Map App</a></li>
        <li><a href="https://docs.google.com/spreadsheets/d/1KzCWSWgVIp_LNtOnzIFhbCU2DXkO-W9oFn4q6WbL3CY/preview">Dataset</a></li>
        <li><a href="https://arcg.is/1izPe01">Digital Guide (ESRI StoryMap Version)</a></li>
        <li><a href="https://nemarvin.github.io/arkansas-creole">Digital Guide (Open Source Markdown Version)</a></li>
        <li><a href="https://youtu.be/StffuOwZWGc?si=Gibl8l_xagVG6A-M">Video Introduction</a></li>
      </ul>
    </div>
  </details>

  <details class="project-group">
    <summary>Enslaved by the Church, Sold for the Republic</summary>
    <div class="project-body">
      <div class="project-images project-images--pair">
        <img src="{{ site.baseurl }}/image3.png" alt="Victims of 1793, Reunion Island - screenshot 1" loading="lazy">
        <img src="{{ site.baseurl }}/image5.png" alt="Victims of 1793, Reunion Island - screenshot 2" loading="lazy">
      </div>
      <p>When French revolutionaries seized the assets of the Catholic Church as "national property," the thousands of men, women, and children enslaved by missionary organizations across the colonial empire were not spared. This digital narrative traces their stories of survival and resistance through a close reading of the documents drawn up to facilitate their re-enslavement. It features a first-of-its-kind interactive atlas that maps all sites of slaveholding by Roman Catholic orders and congregations in the French colonial world and beyond.</p>
      <p class="project-links-label"><strong>Explore:</strong></p>
      <ul>
        <li><a href="https://nemarvin.github.io/church-slavery-atlas/">Map: Church and Slavery Atlas (18th c.)</a></li>
        <li><a href="https://github.com/nemarvin/church-slavery-atlas/blob/main/french_clergy.csv">Dataset: French Colonial Clergy Slaveholding</a></li>
        <li><a href="https://github.com/nemarvin/church-slavery-atlas/blob/main/world_eccl.csv">Dataset: Global Ecclesiastical Slaveholding</a></li>
        <li><a href="https://arcg.is/14Liv82">Map: French Missions Worldwide (1782)</a></li>
        <li><a href="https://storymaps.arcgis.com/stories/68ea1822adba48acadb2848f40b29048">StoryMap Narrative (English)</a></li>
        <li><a href="https://storymaps.arcgis.com/stories/08351cc5814c4d6e9d1672145575b422">StoryMap Narrative (Français)</a></li>
        <li><a href="https://arcg.is/1SKG4u0">StoryMap Detail ("Les Ventes / 1793")</a></li>
      </ul>
    </div>
  </details>

  <details class="project-group">
    <summary>This Unalterable Friendship: New England Merchants in the French Indian Ocean Islands</summary>
    <div class="project-body">
      <div class="project-images project-images--pair">
        <img src="{{ site.baseurl }}/image6.png" alt="Port Louis map screenshot 1" loading="lazy">
        <img src="{{ site.baseurl }}/image2.png" alt="Port Louis map screenshot 2" loading="lazy">
      </div>
      <p>Between 1786 and 1810, Boston was the leading point of origin for ships calling at Port Louis, Mauritius; this map-based overview explores why this distant French island port attracted so many Yankee captains—showing how the French free trade zone, the establishment of a U.S. consulate in 1794, a desire to bypass British markets, and a shared interest in preserving slavery in the Indian Ocean solidified a transoceanic connection between American merchants and Mascarene planters, and how, in the wake of the Haitian Revolution and France’s 1794 Abolition Decree, those same merchants supported a 1796 coup that expelled French commissioners enforcing emancipation (research supported by a Boston Athenæum Library Fellowship from ASECS).</p>
      <p class="project-links-label"><strong>Explore:</strong></p>
      <ul>
        <li><a href="https://storymaps.arcgis.com/stories/5a50f7f5c7824506a3256a0e8b496dcf">This Unalterable Friendship</a></li>
      </ul>
    </div>
  </details>

  <details class="project-group">
    <summary>Creoles Far From Our Native Place: Mapping the Global Peregrinations of Jean-Baptiste Tabardin</summary>
    <div class="project-body">
      <div class="project-images">
        <img src="{{ site.baseurl }}/image4.png" alt="Tabardin Project Screenshot" loading="lazy">
      </div>
      <p>Jean-Baptiste Tabardin, born to an enslaved mother in Mauritius, left behind a remarkable illustrated manuscript chronicling his voyages across the Indian and Atlantic Oceans during the French Revolutionary Wars. Today, "The Life and Adventures of J. B. Tabardin" (c. 1811) is preserved in the manuscript collections of Mauritius’s Carnegie Library. After twelve youthful years as a tailor, steward, and privateer turned prisoner of war, Tabardin reflected on love and masculinity, war and politics, race and religion, and the meaning of life itself.</p>
      <p class="project-links-label"><strong>Explore:</strong></p>
      <ul>
        <li><a href="https://storymaps.arcgis.com/stories/a4727bb429634c28a27c7b217e345419">Creoles Far From Our Land</a></li>
      </ul>
    </div>
  </details>

  <div class="project-interlude">
    <img src="{{ site.baseurl }}/caen2.gif" alt="Garden at the Abbaye-aux-Hommes, Caen, Normandy" loading="lazy">
  </div>

  <p class="project-back"><a href="#">Back to Top</a></p>
</div>
