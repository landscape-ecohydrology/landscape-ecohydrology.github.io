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

/* Do the horizontal flip when hovering */
.flip-card:hover .flip-card-inner {
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
</style>
</head>
<body>
<h2>Meet The Team</h2>
<p>Hover or click on a card to learn more about our team members.</p>
<br>

<div class="row">
  <div class="column">
    <div class="flip-card">
      <div class="flip-card-inner">
        <div class="flip-card-front">
          <img src="/assets/img/blog/team-tolentino2.jpg" alt="Meara">
          <h2>Meara Tolentino</h2>
          <p class="title">PhD Student</p>
        </div>
        <div class="flip-card-back">
          <h2>Meara Tolentino</h2>
          <p class="title">PhD Student</p>
          <p>Meara is a PhD student in the lab studying carbon dynamics across the terrestrial-coastal continuum.</p>
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
          <p class="title">MS Student</p>
        </div>
        <div class="flip-card-back">
          <h2>Jack Boyle</h2>
          <p class="title">MS Student</p>
          <p>Jack is a MS student in the lab. He holds a bachelors degree in Environmental Science from the University of Notre Dame, where he studied limnology (the study of lakes) and conducted studies at a field station in Northern Wisconsin. Additionally, he spent time studying the effects of PFAS biomagnification within Lake Michigan prey fish. At UVA he studies the effects of nitrogen retention in wetlands, rivers and lakes. Outside the lab, Jack enjoys running, playing Mario Cart, and traveling to Montana to exploring the backcountry.</p>
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
          <img src="/assets/img/blog/team-shaffer.png" alt="Owen">
          <h2>Owen Shaffer</h2>
          <p class="title">Undergrad DMP Thesis</p>
        </div>
        <div class="flip-card-back">
          <h2>Owen Shaffer</h2>
          <p class="title">Undergrad DMP Thesis</p>
          <p>Quantifying the effects of Clean Water Act regulations on wetlands and water quality.</p>
        </div>
      </div>
    </div>
  </div>
  
  <div class="column">
    <div class="flip-card">
      <div class="flip-card-inner">
        <div class="flip-card-front">
          <img src="" alt="Katie" style="background-color: #eee;">
          <h2>Katie Glazier</h2>
          <p class="title">Undergraduate Research Assistant</p>
        </div>
        <div class="flip-card-back">
          <h2>Katie Glazier</h2>
          <p class="title">Undergraduate Research Assistant</p>
          <p>Some text that describes me lorem ipsum ipsum lorem.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<!-- Add JavaScript for click/tap functionality -->
<script>
  // Add click/tap functionality for mobile users
  document.querySelectorAll('.flip-card').forEach(card => {
    card.addEventListener('click', function() {
      this.querySelector('.flip-card-inner').classList.toggle('flipped');
    });
  });
</script>

<style>
  /* Add this to your existing CSS */
  .flipped {
    transform: rotateY(180deg);
  }
</style>
</body>
</html>



## Lab Alumni!

-   Owen Shaffer (Spring 2025). Distinguished Major Program Thesis. The outsized role of vulnerable wetlands in 
nitrogen cycling across the US in the context of changing Clean Water Act protections.
 






