---
layout: page
title: "Teaching"
---

<!-- Teaching page: seamless Arkansas Créole Paper palette within the existing Jekyll shell. -->

<style>
/*
  In this site's Jekyll layout, the page heading sits OUTSIDE .teaching-page.
  Color the existing page rather than introducing an inset paper-colored panel.
  The selectors below activate ONLY on a page containing .teaching-page.
  The theme's dark outer surround and navigation structure are retained.
*/
html:has(.teaching-page) body,
body:has(.teaching-page) > article,
body:has(.teaching-page) > article > header {
  background-color: #f4efe4 !important;
}

/* Align the Jekyll-generated page title with the content below. */
body:has(.teaching-page) > article > header,
body:has(.teaching-page) > article > header h1 {
  text-align: left !important;
  text-align-last: auto !important;
}
body:has(.teaching-page) > article > header h1,
body:has(.teaching-page) > article > header h1 a {
  color: #332f2b !important;
  font-family: Georgia, "Times New Roman", serif;
}

.teaching-page {
  --teaching-paper: #f4efe4;
  --teaching-ink: #332f2b;
  --teaching-muted: #746b62;
  --teaching-rule: #8a2f2f;
  --teaching-soft-rule: #d4c8b8;
  --teaching-link: #7b2929;
  --teaching-link-hover: #4f1717;

  /* No nested panel or second level of padding/framing. */
  box-sizing: border-box;
  max-width: none;
  margin: 0;
  padding: 0;
  background: transparent;
  color: var(--teaching-ink);
  font-family: Georgia, "Times New Roman", serif;
  font-size: 18px;
  line-height: 1.68;

  text-align: left !important;
  text-align-last: auto !important;
}

/* Override site-wide justification at every level, including short snippets. */
.teaching-page h2,
.teaching-page h3,
.teaching-page h4,
.teaching-page p,
.teaching-page article,
.teaching-page section,
.teaching-page .teaching-course > div,
.teaching-page a {
  text-align: left !important;
  text-align-last: auto !important;
}

.teaching-page *, .teaching-page *::before, .teaching-page *::after {
  box-sizing: border-box;
}

.teaching-page h2 {
  margin: 0 0 1.65rem;
  padding: 0;
  border: 0 !important;
  color: var(--teaching-ink);
  font-family: Georgia, "Times New Roman", serif;
  font-size: 1.8rem;
  font-weight: 600;
  line-height: 1.25;
}

.teaching-page h2::after {
  content: "";
  display: block;
  width: 72px;
  height: 2px;
  margin-top: 0.7rem;
  background: var(--teaching-rule);
}

.teaching-page a,
.teaching-page a:visited {
  color: var(--teaching-link) !important;
  text-underline-offset: 0.12em;
}

.teaching-page a:hover,
.teaching-page a:focus {
  color: var(--teaching-link-hover) !important;
  text-decoration-color: currentColor;
}

.teaching-page .teaching-feature,
.teaching-page .teaching-course,
.teaching-page .teaching-resource {
  border-bottom: 1px solid var(--teaching-soft-rule);
}

.teaching-page .teaching-feature {
  padding: 0.3rem 0 1.25rem;
  margin-bottom: 1.15rem;
}

.teaching-page .teaching-feature p,
.teaching-page .teaching-resource p {
  margin: 0 0 0.7rem;
}

.teaching-page .teaching-feature p:last-child,
.teaching-page .teaching-resource p:last-child,
.teaching-page .teaching-course p:last-child {
  margin-bottom: 0;
}

.teaching-page .teaching-course-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(min(100%, 330px), 1fr));
  column-gap: 1.8rem;
}

.teaching-page .teaching-course {
  display: grid;
  grid-template-columns: 100px minmax(0, 1fr);
  gap: 0.95rem;
  align-items: start;
  padding: 1.35rem 0;
}

.teaching-page .teaching-course img {
  display: block;
  width: 100%;
  height: auto;
  max-height: 165px;
  object-fit: contain;
  object-position: top left;
}

.teaching-page .teaching-course p {
  margin: 0 0 0.55rem;
  font-size: 0.88em;
  line-height: 1.5;
}

.teaching-page .teaching-course p:first-child {
  font-size: 0.97em;
  line-height: 1.4;
}

.teaching-page .teaching-resource {
  padding: 1rem 0;
}

.teaching-page .teaching-interlude {
  width: 58%;
  max-width: 420px;
  margin: 2.4rem auto 2.65rem;
}

.teaching-page .teaching-interlude img {
  display: block;
  width: 100%;
  height: auto;
}

.teaching-page .teaching-section {
  margin-bottom: 2.2rem;
}

.teaching-page > p:last-child {
  margin: 2rem 0 0;
  font-size: 0.84em;
}

@media (max-width: 540px) {
  .teaching-page {
    font-size: 17px;
    line-height: 1.6;
  }

  .teaching-page h2 {
    font-size: 1.55rem;
  }

  .teaching-page .teaching-course {
    grid-template-columns: 86px minmax(0, 1fr);
    gap: 0.8rem;
  }

  .teaching-page .teaching-interlude {
    width: 78%;
  }
}
</style>

<div class="teaching-page">

  <section class="teaching-section" aria-labelledby="teaching-oer">
    <h2 id="teaching-oer">Open Educational Resources</h2>

    <article class="teaching-feature">
      <p><strong><em>Freedom Deferred: Slavery, Resistance, &amp; the Politics of Race in France’s Indian Ocean Colonies During the Age of Revolution</em></strong></p>
      <p>An open-access documentary reader on slavery, resistance, race, and revolution in the French Indian Ocean world. The collection brings together translated primary sources with historical introductions, annotations, images, and maps for use in undergraduate and graduate courses.</p>
      <p><strong><a href="https://nemarvin.github.io/textio/">Open <em>Freedom Deferred</em>...</a></strong></p>
    </article>

    <article class="teaching-feature">
      <p><strong><em>Arkansas Créole: Rediscovering a Lost Vernacular Landscape</em></strong></p>
      <p>An open educational resource exploring the French and Creole histories embedded in Arkansas’s landscape. Through maps, primary sources, images, and local histories, the project traces place names, migration, Indigenous and colonial encounters, and the persistence of Creole communities and cultural landscapes.</p>
      <p><strong><a href="https://nemarvin.github.io/arkansas-creole/">Open <em>Arkansas Créole</em>...</a></strong></p>
    </article>

    <div class="teaching-interlude">
      <img src="{{ site.baseurl }}/montstmichel.gif"
           alt="Mont Saint-Michel animated footer">
    </div>
  </section>

  <section class="teaching-section" aria-labelledby="teaching-syllabi">
    <h2 id="teaching-syllabi">Course Syllabi</h2>

    <div class="teaching-course-grid">

      <article class="teaching-course">
        <img src="{{ site.baseurl }}/TeachWorldHistFTF.png" alt="Tabardin manuscript illustration" loading="lazy">
        <div>
          <p><strong>World History from 1500 (in person)</strong></p>
          <p>Detail from the illustrated manuscript, <em>La Vie ou aventures de J.-B. Tabardin</em>, ca. 1805, housed in the Carnegie Library of Curepipe, Mauritius. Memoirs of a Creole privateer. Original translation used as a primary source with students.</p>
          <p><strong><a href="https://docs.google.com/document/d/1fePnBlo6BaXp4tC4P-dX8siCCeHUv5IF/preview">View syllabus...</a></strong></p>
        </div>
      </article>

      <article class="teaching-course">
        <img src="{{ site.baseurl }}/TeachWorldHistOnline.png" alt="Haitian stamp with the Unknown Maroon" loading="lazy">
        <div>
          <p><strong>World History from 1500 (asynchronous)</strong></p>
          <p>Haitian postage stamps depicting “the Unknown Maroon,” symbol of resistance to slavery. The Haitian Revolution features prominently in this course.</p>
          <p><strong><a href="https://docs.google.com/document/d/1hhxoUAdHtz3dNuMagoWacLXGb1Mez3QQCwYnhBW9MVY/preview?tab=t.0">View syllabus...</a></strong></p>
        </div>
      </article>

      <article class="teaching-course">
        <img src="{{ site.baseurl }}/TeachFrencHist.png" alt="Josephine Baker Pantheon photo" loading="lazy">
        <div>
          <p><strong>Modern France from 1750</strong></p>
          <p>Photograph from the Pantheonization of Josephine Baker (30 Nov. 2021). Baker’s life and legacy are explored in depth in the course.</p>
          <p><strong><a href="https://docs.google.com/document/d/1g6miJ6b75h02qdgefYWlurPEkbpXHWox-bQUr9kdH1Q/preview">View syllabus (v1)...</a></strong><br>
          <strong><a href="https://docs.google.com/document/d/14ygltrpqJUv1XieKAHX0A7mDH2qUUAVB/preview">View syllabus (v2)...</a></strong></p>
        </div>
      </article>

      <article class="teaching-course">
        <img src="{{ site.baseurl }}/TeachModernEuro.png" alt="Still from Visconti’s Senso" loading="lazy">
        <div>
          <p><strong>Modern Europe</strong></p>
          <p>Still from <em>Senso</em> (1954), film by Luchino Visconti. Film, opera, and propaganda posters are analyzed in this course.</p>
          <p><strong><a href="https://docs.google.com/document/d/1AmCxEgQUcqxwUjT3YtKEfo3fPuFenxel/preview">View syllabus...</a></strong></p>
        </div>
      </article>

      <article class="teaching-course">
        <img src="{{ site.baseurl }}/TeachAtlanticWorld.png" alt="Atlantic History word cloud" loading="lazy">
        <div>
          <p><strong>Atlantic World and Beyond</strong></p>
          <p>Word cloud from a text-mining exercise based on the Oxford Bibliographies in Atlantic History. One of the goals of the course is to critically interrogate Atlantic Studies as a field.</p>
          <p><strong><a href="https://docs.google.com/document/d/14nkCsZx6Kncmx62_e2okoq5_UxqVm3pu/preview">View syllabus...</a></strong></p>
        </div>
      </article>

      <article class="teaching-course">
        <img src="{{ site.baseurl }}/plumbayou.jpg" alt="Headstones of French-speaking families in Old St. Mary’s Cemetery beside historic Catholic church in Plum Bayou, Arkansas" loading="lazy">
        <div>
          <p><strong>Creole South</strong></p>
          <p>The course traces Creole histories across North America, the Caribbean, and beyond, connecting local to global stories.</p>
          <p><strong><a href="https://docs.google.com/document/d/13r3C5urg4DUOiR_BnhCfQzbiOldEMCkM/edit?usp=sharing&amp;ouid=112037445374503169151&amp;rtpof=true&amp;sd=true">View syllabus...</a></strong></p>
        </div>
      </article>

      <article class="teaching-course">
        <img src="{{ site.baseurl }}/TeachRevsWorld.png" alt="French Revolution in Assassin's Creed" loading="lazy">
        <div>
          <p><strong>Revolutions in World History</strong></p>
          <p>Screenshot from <em>Assassin’s Creed: Unity</em>. Students analyze game videos and cutscenes as part of their engagement with revolutionary history and popular memory.</p>
          <p><strong><a href="https://docs.google.com/document/d/1WkrzMls7drYKM8t-_WDqJt2sfxVG8XL53zwjI-y6Y7o/preview">View syllabus...</a></strong></p>
        </div>
      </article>

      <article class="teaching-course">
        <img src="{{ site.baseurl }}/TeachSemRace.png" alt="Bowen Law Library image" loading="lazy">
        <div>
          <p><strong>Global Perspectives on Race</strong></p>
          <p>Photograph from inside the Bowen Law Library’s special collections. Students examine original paperwork from the race-based freedom lawsuit of Abby Guy (1850s, Arkansas).</p>
          <p><strong><a href="https://docs.google.com/document/d/1qI3VulFpNQr1wsPlxu8YOW3VgEVPoFOx/preview">View syllabus...</a></strong></p>
        </div>
      </article>

      <article class="teaching-course">
        <img src="{{ site.baseurl }}/TeachHistUndergradMethods.png" alt="Boston Athenaeum interior" loading="lazy">
        <div>
          <p><strong>Historian’s Craft (Undergraduate Methods)</strong></p>
          <p>Interior of the Boston Athenaeum private library (photo by instructor). Students explore critical approaches to archives and historical method.</p>
          <p><strong><a href="https://docs.google.com/document/d/1p-3HZ_d7Tx7nQX9UHappycZKM5oANXx1/preview">View syllabus...</a></strong></p>
        </div>
      </article>

      <article class="teaching-course">
        <img src="{{ site.baseurl }}/TeachHistMethodsGrad.png" alt="1793 document from Réunion" loading="lazy">
        <div>
          <p><strong>Historical Methods (Graduate)</strong></p>
          <p>Archival document from Réunion Island (1793) related to the “Ambroise Affaire,” which students study in depth in this graduate seminar.</p>
          <p><strong><a href="https://docs.google.com/document/d/1wAJgaCgIgv1O2BHGSLWh-g3WLSV8gDv-/preview">View syllabus...</a></strong></p>
        </div>
      </article>

      <article class="teaching-course">
        <img src="{{ site.baseurl }}/TeachHaitianRev.png" alt="Map of Haitian Revolution diaspora impact" loading="lazy">
        <div>
          <p><strong>Haitian Revolution in World History</strong></p>
          <p>Original map depicting sites impacted by the Haitian Revolution in North America — including inspired revolts and refugee settlement. The global repercussions of the revolution are central to this course.</p>
          <p><strong><a href="https://docs.google.com/document/d/1_dFZoTgSPifFJswXEmFPguYMD86tAD0D/preview">View syllabus...</a></strong></p>
        </div>
      </article>

    </div>

    <div class="teaching-interlude">
      <img src="{{ site.baseurl }}/nolafog.gif"
           alt="New Orleans fog animated footer">
    </div>
  </section>

  <section class="teaching-section" aria-labelledby="teaching-resources">
    <h2 id="teaching-resources">Additional Teaching Resources</h2>

    <article class="teaching-resource">
      <p><strong>Mother Lange: A Haitian-American Educator</strong></p>
      <p>StoryMap highlighting the life and legacy of Mother Mary Lange, founder of the Oblate Sisters of Providence in Baltimore. Integrates spatial history, biography, and Black Catholic history.</p>
      <p><strong><a href="https://storymaps.arcgis.com/stories/6d7e71f256ab4debae028fb5b633bdbd">View digital storytelling project...</a></strong></p>
    </article>

    <article class="teaching-resource">
      <p><strong>A Colonial “Return of Martin Guerre”?</strong></p>
      <p>In this methods course exercise, students analyze testimony in a colonial identity theft case. Inspired by Natalie Zemon Davis’s classic microhistory.</p>
      <p><strong><a href="https://docs.google.com/document/d/1UW6d3K77pzmF_aZJLdBuh1gwqzq8VWRb/preview">View exercise...</a></strong></p>
    </article>

    <article class="teaching-resource">
      <p><strong>Student Digital History Resource Guide</strong></p>
      <p>A curated and frequently updated set of tools, platforms, and archives to support students exploring digital history methods and public scholarship.</p>
      <p><strong><a href="https://docs.google.com/document/d/1JjWOqs-UMzJ3lkysWkx5klx43iV54Tzx40Zli73fbvw/preview">View resource list...</a></strong></p>
    </article>

    <div class="teaching-interlude">
      <img src="{{ site.baseurl }}/littlerock.gif"
           alt="Little Rock animated footer">
    </div>
  </section>

  <p><a href="#">Back to Top</a></p>

</div>
