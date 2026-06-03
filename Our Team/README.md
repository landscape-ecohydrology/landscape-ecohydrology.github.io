---
layout: page
title: Our Team
description: >
  Our current lab group!
hide_description: true
sitemap: false
permalink: /team/
---

<html>

<head>

<meta name="viewport" content="width=device-width, initial-scale=1">

```{=html}
<style>
html {
  box-sizing: border-box;
}
*, *:before, *:after {
  box-sizing: inherit;
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

/* The flip card container */
.flip-card {
  background-color: transparent;
  height: 420px; /* Increased height slightly */
  perspective: 1000px; /* 3D effect */
  cursor: pointer; /* Show it's clickable */
}

/* This container positions the front and back sides */
.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  transition: transform 0.8s;
  transform-style: preserve-3d;
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
}

/* Flip only when clicked */
.flip-card-inner.clicked {
  transform: rotateY(180deg);
}

/* Position the front and back sides */
.flip-card-front, .flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden; /* Safari */
  backface-visibility: hidden;
}

/* Style the front side */
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

/* Style the back side */
.flip-card-back {
  background-color: #f9f9f9;
  color: #333;
  transform: rotateY(180deg);
  padding: 20px;
  overflow-y: auto;
}

.title {
  color: grey;
  margin: 0 0 10px 0; /* Reduced margin */
}

.row:after {
  content: "";
  display: table;
  clear: both;
}

/* Add a prompt to let users know they can flip */
.flip-prompt {
  font-size: 12px;
  font-style: italic;
  margin-top: 5px;
  color: #666;
}

/* Visual indicator for flipped state */
.flip-card-inner.clicked .flip-card-back::after {
  content: "Click to flip back";
  position: absolute;
  bottom: 5px;
  right: 10px;
  font-size: 10px;
  color: #999;
  font-style: italic;
}
</style>
```

</head>

<body>

<h2>Meet The Team</h2>

<p>Click on a card to flip and see more details. Click again to flip back.</p>

<br>

::::: row
::: column
```         
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
```
:::

::: column
```         
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
      <p>Jack is a PhD student in the lab. He holds a bachelors degree in Environmental Science from the University of Notre Dame, where he studied limnology (the study of lakes) and conducted studies at a field station in Northern Wisconsin. Additionally, he spent time studying the effects of PFAS biomagnification within Lake Michigan prey fish. At UVA he studies the effects of nitrogen retention in wetlands, rivers and lakes. Outside the lab, Jack enjoys running, playing Mario Cart, and traveling to Montana to exploring the backcountry.</p>
    </div>
  </div>
</div>
```
:::
:::::

::::::: row
::: column
```         
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
```
:::

::::: row
::: column
```         
<div class="flip-card">
  <div class="flip-card-inner">
    <div class="flip-card-front">
      <img src="/assets/img/blog/team-michelle.png" alt="Jack">
      <h2>Michelle Nguyen</h2>
      <p class="title">MS Student</p>
    </div>
    <div class="flip-card-back">
      <h2>Michelle Nguyen</h2>
      <p class="title">MS Student</p>
      <p>I am an MS student in the lab, with my research focusing on modeling nitrogen legacies and predicting landscape-scale patterns of legacy nitrogen release. I have a bachelor's degree in computer science and environmental studies from Washington and Lee University. There, I conducted research on the erosion process of hydraulic plucking by using image processing to analyze dye dispersion in our homemade flume! I also did research at the Kansas Geological Survey, where I helped couple PyCHAMP, a Python-based hydrological model, with AquaCrop, a crop growth and water-use simulation tool, in order to enhance agricultural water management predictions. Outside of the lab, I enjoy hanging out with my two cats (Chair and Sofa) and my roommate's cat (Pingle), baking, and playing board games! </p>
    </div>
  </div>
</div>
```
:::

::: column
```         
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
```
:::
:::::

```{=html}
<script>
document.querySelectorAll('.flip-card').forEach(card => {
  const inner = card.querySelector('.flip-card-inner');
  
  card.addEventListener('click', function(e) {
    e.preventDefault();
    inner.classList.toggle('clicked');
  });
});
</script>
```

<h2>Lab Alumni!</h2>

<p>
-   Yamato Motai (Spring 2026). Undergraduate Researcher.
</p>
<p>
-   Olivia Smith (Fall 2025). Undergraduate Researcher.
</p>
<p>
-   Katie Glazier (Spring 2025). Undergraduate Researcher.
</p>
<p>
-   Owen Shaffer (Spring 2025). Distinguished Major Program Thesis. The outsized role of vulnerable wetlands in nitrogen cycling across the US in the context of changing Clean Water Act protections.
</p>

</body>

</html>
:::::::
