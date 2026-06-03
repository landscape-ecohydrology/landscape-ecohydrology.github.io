---
layout: page
title: Our Team
description: >
  Our current lab group!
hide_description: true
sitemap: false
permalink: /team/
---

<style>
html {
  box-sizing: border-box;
}
*, *:before, *:after {
  box-sizing: inherit;
}

.row:after {
  content: "";
  display: table;
  clear: both;
}

.column {
  float: left;
  width: 50%;
  margin-bottom: 30px;
  padding: 0 15px;
}

@media screen and (max-width: 650px) {
  .column {
    width: 100%;
    display: block;
  }
}

.flip-card {
  background-color: transparent;
  height: 420px;
  perspective: 1000px;
  cursor: pointer;
}

.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  transition: transform 0.8s;
  transform-style: preserve-3d;
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
}

.flip-card-inner.clicked {
  transform: rotateY(180deg);
}

.flip-card-front, .flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
}

.flip-card-front {
  background-color: #fff;
  color: black;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  padding-bottom: 15px;
}

.flip-card-front img {
  width: 100%;
  height: 300px;
  object-fit: cover;
}

.flip-card-front h2 {
  margin: 10px 0 5px;
}

.flip-card-back {
  background-color: #f9f9f9;
  color: #333;
  transform: rotateY(180deg);
  padding: 20px;
  overflow-y: auto;
}

.title {
  color: grey;
  margin: 0 0 10px 0;
}

.flip-card-inner.clicked .flip-card-back::after {
  content: "Click to flip back";
  position: absolute;
  bottom: 5px;
  right: 10px;
  font-size: 10px;
  color: #999;
  font-style: italic;
}

/* PI biography section: static, full-width */
.pi-section {
  display: flex;
  align-items: flex-start;
  gap: 30px;
  margin: 30px 15px 50px 15px;
  padding: 25px;
  background-color: #f9f9f9;
  color: #333;
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
}

.pi-photo {
  width: 240px;
  height: 240px;
  object-fit: cover;
  flex-shrink: 0;
}

.pi-bio {
  flex: 1;
}

.pi-bio h2 {
  margin-top: 0;
  margin-bottom: 5px;
}

.pi-bio .title {
  color: grey;
  margin-bottom: 15px;
}

.pi-bio p {
  margin-bottom: 12px;
}

/* Stack PI photo and bio on smaller screens */
@media screen and (max-width: 650px) {
  .pi-section {
    display: flex;
    align-items: flex-start;
    gap: 30px;
    margin: 30px 15px 50px 15px;
    padding: 0;
    background-color: transparent;
    color: inherit;
    box-shadow: none;
  }

  .pi-photo {
    width: 100%;
    height: auto;
    aspect-ratio: 1 / 1;
  }
}

</style>

<div class="pi-section">
  <img src="/assets/img/blog/1456936992.png" alt="Frederick Cheng" class="pi-photo">

  <div class="pi-bio">
    <h2>Dr. Frederick Cheng</h2>
    <p class="title">Principal Investigator</p>

    <p>
      I am an assistant professor in critical zone hydrology in the <a href="https://evsc.as.virginia.edu/">Department of Environmental Sciences at the University of Virginia</a>. I was previously a postdoctoral researcher in the <a href="https://warnercnr.colostate.edu/ess/">Department of Ecosystem Science and Sustainability</a> at the <a href="https://www.colostate.edu/">Colorado State University</a>.
    </p>
    <p>
      My research interest lies in the sustainable management of our water resources by exploring the interactions between hydrological and biogeochemical processes across different scales. Topics of particular interest are: modelling groundwater-surface water interactions, ecohydrological modelling across scales, contaminant fate in watersheds.
    </p>
    <p>
      Outside of the lab, I enjoy competitive ballroom dancing, bouldering, and all sorts of board games! 
    </p>
  </div>
</div>

<h2>Meet The Team</h2>

<p>Click on a card to flip and see more details. Click again to flip back.</p>

<br>

<div class="row">

  <div class="column">
    <div class="flip-card">
      <div class="flip-card-inner">
        <div class="flip-card-front">
          <img src="/assets/img/blog/team-tolentino2.jpg" alt="Meara">
          <h2>M. Tolentino</h2>
          <p class="title">PhD Student</p>
        </div>
        <div class="flip-card-back">
          <h2>M. Tolentino</h2>
          <p class="title">PhD Student</p>
          <p>My research focuses on understanding carbon dynamics across ecosystems, with an emphasis on the terrestrial–aquatic interface. I have a Bachelor's degree in the physical sciences and a Master’s in Environmental Science. My graduate work used satellite remote sensing to examine how ocean frontal features influence fishing activity in marine waters. I later contributed to oceanographic research, including hydroacoustic surveys to estimate single fish species biomass. Currently, I am a PhD student in the lab studying organic carbon across the terrestrial–coastal continuum, using remote sensing and modeling to explore coastal wetland processes. Outside of research, I enjoy strength training, cooking & baking, badminton, and hiking.</p>
        </div>
      </div>
    </div>
  </div>

  <div class="column">
    <div class="flip-card">
      <div class="flip-card-inner">
        <div class="flip-card-front">
          <img src="/assets/img/blog/team-boyle.png" alt="Jack">
          <h2>Jack Boyle</h2>
          <p class="title">PhD Student</p>
        </div>
        <div class="flip-card-back">
          <h2>Jack Boyle</h2>
          <p class="title">PhD Student</p>
          <p>Jack is a PhD student in the lab. He holds a bachelors degree in Environmental Science from the University of Notre Dame, where he studied limnology and conducted studies at a field station in Northern Wisconsin. Additionally, he spent time studying the effects of PFAS biomagnification within Lake Michigan prey fish. At UVA he studies the effects of nitrogen retention in wetlands, rivers and lakes. Outside the lab, Jack enjoys running, playing Mario Kart, and traveling to Montana to explore the backcountry.</p>
        </div>
      </div>
    </div>
  </div>

</div>

<div class="row">

  <div class="column">
    <div class="flip-card">
      <div class="flip-card-inner">
        <div class="flip-card-front">
          <img src="/assets/img/blog/anon.webp" alt="placeholder">
          <h2>Lucas Raymond</h2>
          <p class="title">PhD Student</p>
        </div>
        <div class="flip-card-back">
          <h2>Lucas Raymond</h2>
          <p class="title">PhD Student</p>
          <p>Under Construction!</p>
        </div>
      </div>
    </div>
  </div>

  <div class="column">
    <div class="flip-card">
      <div class="flip-card-inner">
        <div class="flip-card-front">
          <img src="/assets/img/blog/team-michelle.jpeg" alt="Michelle">
          <h2>Michelle Nguyen</h2>
          <p class="title">MS Student</p>
        </div>
        <div class="flip-card-back">
          <h2>Michelle Nguyen</h2>
          <p class="title">MS Student</p>
          <p>I am an MS student in the lab, with my research focusing on modeling nitrogen legacies and predicting landscape-scale patterns of legacy nitrogen release. I have a bachelor's degree in computer science and environmental studies from Washington and Lee University. There, I conducted research on the erosion process of hydraulic plucking by using image processing to analyze dye dispersion in our homemade flume. I also did research at the Kansas Geological Survey, where I helped couple PyCHAMP, a Python-based hydrological model, with AquaCrop, a crop growth and water-use simulation tool, in order to enhance agricultural water management predictions. Outside of the lab, I enjoy hanging out with my two cats, Chair and Sofa, and my roommate's cat, Pingle, baking, and playing board games!</p>
        </div>
      </div>
    </div>
  </div>

</div>

<div class="row">

  <div class="column">
    <div class="flip-card">
      <div class="flip-card-inner">
        <div class="flip-card-front">
          <img src="/assets/img/blog/anon.webp" alt="placeholder">
          <h2>Could be you!</h2>
          <p class="title">Undergraduate Research Assistant</p>
        </div>
        <div class="flip-card-back">
          <h2>Could be you!</h2>
          <p class="title">Undergraduate Research Assistant</p>
          <p>Please reach out if you're an undergraduate student at UVA and are interested in being a research assistant!</p>
        </div>
      </div>
    </div>
  </div>

</div>

<script>
document.querySelectorAll('.flip-card').forEach(card => {
  const inner = card.querySelector('.flip-card-inner');

  card.addEventListener('click', function(e) {
    e.preventDefault();
    inner.classList.toggle('clicked');
  });
});
</script>

<h2>Lab Alumni!</h2>

<ul>
  <li>Yamato Motai (Spring 2026). Undergraduate Researcher.</li>
  <li>Olivia Smith (Fall 2025). Undergraduate Researcher.</li>
  <li>Katie Glazier (Spring 2025). Undergraduate Researcher.</li>
  <li>Owen Shaffer (Spring 2025). Distinguished Major Program Thesis. The outsized role of vulnerable wetlands in nitrogen cycling across the US in the context of changing Clean Water Act protections.</li>
</ul>
