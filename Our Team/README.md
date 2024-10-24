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
  width: 33.3%;
  margin-bottom: 16px;
  padding: 0 8px;
}

@media screen and (max-width: 650px) {
  .column {
    width: 100%;
    display: block;
  }
}

.card {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  min-height: 400px; /* Set a minimum height for the card */
  max-height: 500px; /* Set a maximum height */
  display: flex;
  flex-direction: column;
  overflow: auto; /* Hide overflow if it exceeds max height */
}

.container {
  padding: 0 16px;
}

.container::after, .row::after {
  content: "";
  clear: both;
  display: table;
}

.title {
  color: grey;
}

.button {
  border: none;
  outline: 0;
  display: inline-block;
  padding: 8px;
  color: white;
  background-color: #000;
  text-align: center;
  cursor: pointer;
  width: 100%;
}

.button:hover {
  background-color: #555;
}
</style>
</head>
<body>

<h2>Meet The Team</h2>
<br>


<div class="row">
  <div class="column">
    <div class="card">
      <img src="/assets/img/blog/team-tolentino.jpg" alt="Meara" style="width:100%">
      <div class="container">
        <h2>Meara Tolentino</h2>
        <p class="title">PhD Student</p>
        <p>Meara is a PhD student in the lab studying X, Y, Z.</p>
      </div>
    </div>
  </div>

  <div class="column">
    <div class="card">
      <img src="/assets/img/blog/team-boyle.png" alt="Jack" style="width:100%">
      <div class="container">
        <h2>Jack Boyle</h2>
        <p class="title">MS Student</p>
        <p>Jack is a MS student in the lab. He holds a bachelors degree in Environmental Science from the University of Notre Dame, where he studied limnology (the study of lakes) and conducted studies at a field station in Northern Wisconsin. Additionally, he spent time studying the effects of PFAS biomagnification within Lake Michigan prey fish. At UVA he studies the effects of nitrogen retention in wetlands, rivers and lakes. Outside the lab, Jack enjoys running, playing Mario Cart, and traveling to Montana to exploring the backcountry.</p>
      </div>
    </div>
  </div>
  
  <div class="column">
    <div class="card">
      <img src="/w3images/team3.png" alt="Owen" style="width:100%">
      <div class="container">
        <h2>Owen Shaffer</h2>
        <p class="title">Undergrad DMP Thesis</p>
        <p>Some text that describes me lorem ipsum ipsum lorem.</p>
      </div>
    </div>
  </div>
  
  <div class="row">
  <div class="column">
    <div class="card">
      <img src="" alt="Katie" style="width:100%">
      <div class="container">
        <h2>Katie Glathier</h2>
        <p class="title">Undergraduate Research Assistant</p>
        <p>Some text that describes me lorem ipsum ipsum lorem.</p>
      </div>
    </div>
  </div>
  
</div>

</body>
</html>

