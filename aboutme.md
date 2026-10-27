---
layout: page
title: "About Me"
---

<!-- About Me: same seamless Paper palette and Roboto typography as Teaching Materials. -->

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,400;0,500;0,600;0,700;1,400;1,500;1,600;1,700&display=swap');

/* Match the existing Jekyll page surface to the Teaching Materials paper color.
   No additional inner panel; the outer site shell stays unchanged. */
html:has(.about-page) body,
body:has(.about-page) > article,
body:has(.about-page) > article > header {
  background-color: #f4efe4 !important;
}

/* Jekyll generates the "About Me" heading outside .about-page. */
body:has(.about-page) > article > header,
body:has(.about-page) > article > header h1 {
  text-align: center !important;
  text-align-last: center !important;
}
body:has(.about-page) > article > header h1,
body:has(.about-page) > article > header h1 a {
  color: #332f2b !important;
  font-family: Roboto, "Helvetica Neue", Arial, sans-serif;
}
body:has(.about-page) > article > header h1 {
  font-size: 1.7rem !important;
}

.about-page {
  --about-ink: #332f2b;
  --about-muted: #746b62;
  --about-link: #7b2929;
  --about-link-hover: #4f1717;

  max-width: none;
  margin: 0;
  padding: 0;
  background: transparent;
  color: var(--about-ink);
  font-family: Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 18px;
  line-height: 1.68;
  text-align: left !important;
  text-align-last: auto !important;
}

.about-page p {
  margin: 0 0 1.15em;
  color: var(--about-ink);
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
  text-align: left !important;
  text-align-last: auto !important;
  word-spacing: normal;
}

.about-page a,
.about-page a:visited {
  color: var(--about-link) !important;
  text-underline-offset: 0.12em;
}
.about-page a:hover,
.about-page a:focus {
  color: var(--about-link-hover) !important;
}

/* Preserve the original floated-image composition. */
.about-page .about-portrait {
  display: block;
  float: left;
  width: 20%;
  max-width: 170px;
  height: auto;
  margin: 0 1.5rem 1.25rem 0;
}
.about-page .about-harbor {
  display: block;
  float: right;
  width: 35%;
  height: auto;
  margin: 0.25rem 0 1rem 1.5rem;
}
.about-page::after {
  content: "";
  display: block;
  clear: both;
}

@media (max-width: 540px) {
  .about-page {
    font-size: 17px;
    line-height: 1.6;
  }
  body:has(.about-page) > article > header h1 {
    font-size: 1.55rem !important;
  }
  .about-page .about-portrait {
    width: 32%;
    max-width: 140px;
    margin-right: 1rem;
  }
  .about-page .about-harbor {
    width: 43%;
    margin-left: 1rem;
  }
}
</style>

<div class="about-page">

<img class="about-portrait" src="{{ site.baseurl }}/me24_2.png" alt="Nathan E. Marvin">

<p>I am a social and cultural historian of the French colonial world, working comparatively across Creole spaces in Africa’s Indian Ocean islands, North America, and the Caribbean. My research and teaching focus on places (and people) considered “marginal” to the histories of empires. Their histories are often especially revealing of how empires were made and sustained, and what endured after one was swapped for another.</p>

<p>My first book follows the shifting politics of race on Réunion Island in the Indian Ocean, showing how a colony treated as peripheral to the French and Haitian Revolutions was in fact deeply implicated in the transformations they set in motion. My work on the memoirs of a globetrotting sailor from Mauritius, a neighboring French island, explores what it meant to call oneself “Creole” in a maritime world remade by those revolutions, even after his home fell under British rule. My second book project documents the scope and scale of an understudied phenomenon across the French colonial world: slaveholding by Catholic orders and congregations. Beyond reconstructing the daily lives and resistance strategies of the thousands who labored on missionary-run plantations in the latter third of the eighteenth century, the project examines their relationships with the clergy who enslaved them and traces what happened to them when revolutionary governments declared them “national property.”</p>

<img class="about-harbor" src="{{ site.baseurl }}/portsmouthharbor_2.gif" alt="Portsmouth Harbor, New Hampshire–Maine">

<p>I teach history at the University of Arkansas at Little Rock (a region whose own Creole history is often overlooked). I work with students to explore the survival of Francophone culture in early Arkansas through successive French, Spanish, and U.S. regimes, as well as how the legacies of that world—and of the families of diverse origins who shaped it—remain embedded in many of our state's place names. We use archival research to connect the local to the global and bring our findings, and the new questions they raise, to audiences beyond the classroom. Doing history “from the margins,” whether geographical or social, does more than enrich our scholarship; it can help us rethink how the past figures in the stories we tell about our communities.</p>

<p>I live and work in beautiful Central Arkansas. I am originally from the Piscataqua River region, between coastal New Hampshire and southern Maine, where I first discovered the power of history to foster a more meaningful sense of place.</p>

</div>
