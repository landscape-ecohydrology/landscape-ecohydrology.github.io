```html
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
</style>

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
          <img src="/assets/img/blog/team-michelle.png" alt="Michelle">
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

I would also remove these tags from the page:

<html>
<head>
<body>
</body>
</html>

Because your layout already supplies those. In a Jekyll page, you usually only need the YAML front matter plus the page content. The biggest issue, though, is the Quarto syntax showing up literally.

that's mainly fixed, but now the pushed site has one last trailing 

html at the top


Yes — that means there is still an opening Markdown code fence left in the file:

```html

It is likely sitting immediately after your YAML front matter, maybe right before the <style> tag or <h2>Meet The Team</h2> section.

Remove this line entirely:

```html

Also search the file for any remaining triple backticks:


For this page, you should have **zero** triple-backtick fences around the HTML/CSS/JS. GitHub Pages/Jekyll should receive the HTML directly, not as a Markdown code block.

So the top of the file should look like this:

```markdown
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
...
</style>

<h2>Meet The Team</h2>

Not this:

---
layout: page
title: Our Team
...
---

```html
<style>
...
</style>

The leftover fence is probably from replacing:

```{=html}

with:

```html

But for Jekyll, you want to delete the whole fence, not rename it. The original uploaded page had these code-fence wrappers around the CSS/JS, which caused the raw syntax to print on the page.

great, I want to add a PI section ABOVE the flipping cards, where i want a static biography and picture (probably need the picture to be square to match everything). give me a template and tell me where to put it. Presumably I want it above the Meet the Team header

Yes — put the PI section above this line:

<h2>Meet The Team</h2>

The clean structure should be:

<style>
/* existing style block */

/* add PI styles here */
</style>

<!-- PI section goes here -->

<h2>Meet The Team</h2>

<p>Click on a card to flip and see more details. Click again to flip back.</p>

Add this CSS inside your existing <style> block, near the other card/row styles:

/* PI biography section */
.pi-section {
  display: flex;
  align-items: flex-start;
  gap: 30px;
  margin: 30px 0 50px 0;
  padding: 25px;
  background-color: #f9f9f9;
  color: #333;
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
}

.pi-photo {
  width: 220px;
  height: 220px;
  object-fit: cover;
  flex-shrink: 0;
}

.pi-bio {
  flex: 1;
}

.pi-bio h2 {
  margin-top: 0;
  margin-bottom: 5px;
  color: #111;
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
    flex-direction: column;
  }

  .pi-photo {
    width: 100%;
    height: auto;
    aspect-ratio: 1 / 1;
  }
}

Then put this HTML immediately above <h2>Meet The Team</h2>:

<div class="pi-section">
  <img src="/assets/img/blog/your-pi-photo.jpg" alt="Frederick Cheng" class="pi-photo">

  <div class="pi-bio">
    <h2>Frederick Cheng</h2>
    <p class="title">Principal Investigator</p>

    <p>
      I am an Assistant Professor in the Department of Environmental Sciences at the University of Virginia. My research focuses on watershed hydrology, biogeochemistry, water quality, and ecosystem restoration, with a particular interest in how wetlands and other landscape features regulate water, carbon, and nutrient dynamics.
    </p>

    <p>
      Our lab combines field observations, environmental data synthesis, geospatial analysis, remote sensing, and process-based and statistical modeling to understand how hydrologic and biogeochemical processes scale from local ecosystems to watersheds and regions.
    </p>

    <p>
      I am especially interested in mentoring students who want to work across disciplinary boundaries, combining environmental science, data analysis, and modeling to address applied water and ecosystem challenges.
    </p>
  </div>
</div>

So the relevant section of the page would become:

<div class="pi-section">
  <img src="/assets/img/blog/your-pi-photo.jpg" alt="Frederick Cheng" class="pi-photo">

  <div class="pi-bio">
    <h2>Frederick Cheng</h2>
    <p class="title">Principal Investigator</p>

    <p>
      I am an Assistant Professor in the Department of Environmental Sciences at the University of Virginia. My research focuses on watershed hydrology, biogeochemistry, water quality, and ecosystem restoration, with a particular interest in how wetlands and other landscape features regulate water, carbon, and nutrient dynamics.
    </p>

    <p>
      Our lab combines field observations, environmental data synthesis, geospatial analysis, remote sensing, and process-based and statistical modeling to understand how hydrologic and biogeochemical processes scale from local ecosystems to watersheds and regions.
    </p>

    <p>
      I am especially interested in mentoring students who want to work across disciplinary boundaries, combining environmental science, data analysis, and modeling to address applied water and ecosystem challenges.
    </p>
  </div>
</div>

<h2>Meet The Team</h2>

<p>Click on a card to flip and see more details. Click again to flip back.</p>

For the image, upload a square or near-square photo to something like:

/assets/img/blog/team-cheng.jpg

Then update this line:

<img src="/assets/img/blog/team-cheng.jpg" alt="Frederick Cheng" class="pi-photo">

The CSS will force it into a square using width, height, and object-fit: cover, so the source image does not have to be perfectly square, but a square crop will give you the most control.

i don't want it to flip, does this code do that? THe PI section can be static and take up the width of the two student boxes

Yes — the PI code I gave is static. It does not include flip-card, flip-card-inner, or the click JavaScript, so it will not flip.

To make it take up the same total width as the two student cards, use a full-width static section above the student-card grid. I would slightly revise the CSS so it aligns with the left/right edges of the two-card layout.

Add this inside your existing <style> block:

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
  color: #111;
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
    flex-direction: column;
    margin-left: 15px;
    margin-right: 15px;
  }

  .pi-photo {
    width: 100%;
    height: auto;
    aspect-ratio: 1 / 1;
  }
}

Then place this above:

<h2>Meet The Team</h2>

Use this template:

<div class="pi-section">
  <img src="/assets/img/blog/team-cheng.jpg" alt="Frederick Cheng" class="pi-photo">

  <div class="pi-bio">
    <h2>Frederick Cheng</h2>
    <p class="title">Principal Investigator</p>

    <p>
      I am an Assistant Professor in the Department of Environmental Sciences at the University of Virginia. My research focuses on watershed hydrology, biogeochemistry, water quality, and ecosystem restoration, with a particular interest in how wetlands and other landscape features regulate water, carbon, and nutrient dynamics.
    </p>

    <p>
      Our lab combines field observations, environmental data synthesis, geospatial analysis, remote sensing, and process-based and statistical modeling to understand how hydrologic and biogeochemical processes scale from local ecosystems to watersheds and regions.
    </p>
  </div>
</div>

So the page order should be:

<!-- PI section -->
<div class="pi-section">
  ...
</div>

<!-- Student/team section -->
<h2>Meet The Team</h2>

<p>Click on a card to flip and see more details. Click again to flip back.</p>

<br>

<div class="row">
  ...
</div>

The key details are:

<div class="pi-section">

not:

<div class="flip-card">

As long as the PI section does not use the flip-card class, the click-to-flip script will ignore it.

something went wrong.

I also don't need the PI section to be in white

The screenshot suggests two separate issues:

    The PI image path is wrong, so the browser is showing the alt text, “Frederick Cheng,” instead of the image.

    Some HTML tags are being printed as text, especially </p> and </div>. That usually means there is still a code fence, escaped HTML, or malformed copy/paste around the PI section.

For the PI section, use this cleaner version. It is static, not white, and spans the width of the two student cards.
1. Add this CSS inside your existing <style> block

/* PI biography section: static, full-width, no white card */
.pi-section {
  display: flex;
  align-items: flex-start;
  gap: 30px;
  margin: 30px 15px 50px 15px;
  padding: 0;
  background-color: transparent;
  color: inherit;
}

.pi-photo {
  width: 260px;
  height: 260px;
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
    flex-direction: column;
    margin-left: 15px;
    margin-right: 15px;
  }

  .pi-photo {
    width: 100%;
    height: auto;
    aspect-ratio: 1 / 1;
  }
}

2. Put this immediately above Meet The Team

Put it above this line:

<h2>Meet The Team</h2>

Use this:

<div class="pi-section">
  <img src="/assets/img/blog/team-cheng.jpg" alt="Frederick Cheng" class="pi-photo">

  <div class="pi-bio">
    <h2>Dr. Frederick Cheng</h2>
    <p class="title">Principal Investigator</p>

    <p>
      I am an assistant professor in critical zone hydrology in the Department of Environmental Sciences at the University of Virginia. I was previously a postdoctoral researcher in the Department of Ecosystem Science and Sustainability at Colorado State University.
    </p>

    <p>
      My research interests lie in the sustainable management of our water resources by exploring the interactions between hydrological and biogeochemical processes across different scales. Topics of particular interest include modeling groundwater-surface water interactions, ecohydrological modeling across scales, and contaminant fate in watersheds.
    </p>

    <p>
      Outside of the lab, I enjoy competitive ballroom dancing, bouldering, and all sorts of board games!
    </p>
  </div>
</div>

<h2>Meet The Team</h2>

3. Fix the image path

Right now, this line is probably pointing to a file that does not exist:

<img src="/assets/img/blog/team-cheng.jpg" alt="Frederick Cheng" class="pi-photo">

Make sure the image is actually uploaded to:

/assets/img/blog/team-cheng.jpg

If your file is named something else, update the src. For example:

<img src="/assets/img/blog/frederick-cheng.png" alt="Frederick Cheng" class="pi-photo">

4. Important: remove any literal closing tags

In your screenshot, I can see things like:

</p>
</div> </div>

Those should not be visible on the website. Make sure you did not paste them as text with escaped characters like:

&lt;/p&gt;
&lt;/div&gt;

Also make sure there are no triple backticks around this section:

```html
...
```

For this page, the PI section should be plain HTML directly in the file, not inside a code block.

Pasted text(6).txt
Document
can you just edit the following


I edited the page and saved a corrected version here:

The main bug was this unclosed link in the PI bio:

<a href="https://www.colostate.edu/">Colorado State University.

It needed to be:

<a href="https://www.colostate.edu/">Colorado State University</a>.

Because that <a> tag was never closed, the rest of the page became part of the link, which explains the underlined text and strange rendering. I also changed the PI section so it is transparent rather than a white card, while keeping it static and full-width above the flipping student cards.

it's getting there, but I still have a white box

Yes — that white box is coming from the .pi-section CSS. Your live site is still using this older version:

.pi-section {
  ...
  padding: 25px;
  background-color: #f9f9f9;
  color: #333;
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
}

Replace the whole .pi-section block with this:

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

Also replace this block:

.pi-bio h2 {
  margin-top: 0;
  margin-bottom: 5px;
  color: #111;
}

with:

.pi-bio h2 {
  margin-top: 0;
  margin-bottom: 5px;
}

That will remove the forced black text and let the heading inherit your site’s normal theme color.

So the full PI CSS should be:

/* PI biography section: static, full-width */
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
  width: 260px;
  height: 260px;
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

One more thing: your screenshot still shows the links underlining huge chunks of text. That means the unclosed Colorado State link may still be present on the live version. Make sure this line is exactly:

at <a href="https://www.colostate.edu/">Colorado State University</a>.

not:

at the <a href="https://www.colostate.edu/">Colorado State University.

After those two changes, the PI section should sit directly on the dark page background, without the white card.

Pasted text(7).txt
Document
it still looks like the pi section stays white in dark mode. is there a way for that to be responsive, and the text adjusts accordingly (example the Meet the Team header changes font colour)

Yes. The problem is that your normal .pi-section still has a forced white background:

background-color: #f9f9f9;
color: #333;

and your transparent version is only inside the small-screen media query, so it only applies when the screen is under 650 px wide. In the uploaded file, that transparent styling is nested under @media screen and (max-width: 650px), so desktop dark mode still gets the white card.

I edited the file so the PI section is transparent and inherits the theme colors on desktop and mobile:

The key replacement is this CSS:

/* PI biography section: static, full-width, theme-responsive */
.pi-section {
  display: flex;
  align-items: flex-start;
  gap: 30px;
  margin: 30px 15px 50px 15px;
  padding: 0;
  background: transparent;
  color: inherit;
  box-shadow: none;
}

.pi-photo {
  width: 260px;
  height: 260px;
  object-fit: cover;
  flex-shrink: 0;
}

.pi-bio {
  flex: 1;
  color: inherit;
}

.pi-bio h2 {
  margin-top: 0;
  margin-bottom: 5px;
  color: inherit;
}

.pi-bio .title {
  color: inherit;
  opacity: 0.7;
  margin-bottom: 15px;
}

.pi-bio p {
  margin-bottom: 12px;
  color: inherit;
}

I also cleaned up this line, which had awkward punctuation and spacing:

<a href="https://evsc.as.virginia.edu/">Department of Environmental Sciences at the University of Virginia.</a>I was previously...

to:

<a href="https://evsc.as.virginia.edu/">Department of Environmental Sciences at the University of Virginia</a>.
I was previously...


one last thing:

I think I wan to align the picture with the main text, and have the name and title left justified. How do i do that

Yes — right now the text column starts at the top, so the name/title are aligned with the top of the photo. To align the photo with the main biography text, make the PI section a small grid: left column = image, right column = name/title + bio, with the photo starting on the same row as the bio paragraph.

Replace your PI CSS with this:

/* PI biography section: static, full-width, theme-responsive */
.pi-section {
  display: grid;
  grid-template-columns: 260px 1fr;
  grid-template-areas:
    "empty heading"
    "photo bio";
  column-gap: 30px;
  row-gap: 20px;
  margin: 30px 15px 50px 15px;
  padding: 0;
  background: transparent;
  color: inherit;
  box-shadow: none;
}

.pi-photo {
  grid-area: photo;
  width: 260px;
  height: 260px;
  object-fit: cover;
}

.pi-bio {
  display: contents;
  color: inherit;
}

.pi-heading {
  grid-area: heading;
  text-align: left;
}

.pi-heading h2 {
  margin-top: 0;
  margin-bottom: 5px;
  color: inherit;
}

.pi-heading .title {
  color: inherit;
  opacity: 0.7;
  margin-bottom: 0;
}

.pi-text {
  grid-area: bio;
  color: inherit;
}

.pi-text p {
  margin-top: 0;
  margin-bottom: 12px;
  color: inherit;
}

/* Stack PI photo and bio on smaller screens */
@media screen and (max-width: 650px) {
  .pi-section {
    display: block;
    margin-left: 15px;
    margin-right: 15px;
  }

  .pi-photo {
    width: 100%;
    height: auto;
    aspect-ratio: 1 / 1;
    margin-bottom: 20px;
  }

  .pi-heading {
    margin-bottom: 15px;
  }
}

Then change the PI HTML to this structure:

<div class="pi-section">
  <img src="/assets/img/blog/1456936992.png" alt="Frederick Cheng" class="pi-photo">

  <div class="pi-bio">
    <div class="pi-heading">
      <h2>Dr. Frederick Cheng</h2>
      <p class="title">Principal Investigator</p>
    </div>

    <div class="pi-text">
      <p>
        I am an assistant professor in critical zone hydrology in the
        <a href="https://evsc.as.virginia.edu/">Department of Environmental Sciences at the University of Virginia</a>.
        I was previously a postdoctoral researcher in the Department of Ecosystem Science and Sustainability at
        Colorado State University.
      </p>

      <p>
        My research interests lie in the sustainable management of water resources by exploring interactions between
        hydrological and biogeochemical processes across scales. Topics of particular interest include modeling
        groundwater-surface water interactions, ecohydrological modeling across scales, and contaminant fate in watersheds.
      </p>

      <p>
        Outside of the lab, I enjoy competitive ballroom dancing, bouldering, and all sorts of board games!
      </p>
    </div>
  </div>
</div>

That will give you this layout:

                 Dr. Frederick Cheng
                 Principal Investigator

[ PI photo ]     I am an assistant professor...
[          ]     My research interests...
[          ]     Outside of the lab...

The important change is that the name/title are now in their own .pi-heading block, while the photo and biography text align beneath it.

i want the name and title to be left aligned with the left side of the photo

Got it. Then you want a two-column layout, where the entire left column contains the name/title above the photo, and the right column contains the biography text.

Use this structure:

Dr. Frederick Cheng        Bio paragraph 1...
Principal Investigator     Bio paragraph 2...

[ PI photo ]               Bio paragraph 3...

Replace your PI CSS with this:

/* PI biography section: static, full-width, theme-responsive */
.pi-section {
  display: grid;
  grid-template-columns: 260px 1fr;
  column-gap: 30px;
  margin: 30px 15px 50px 15px;
  padding: 0;
  background: transparent;
  color: inherit;
  box-shadow: none;
}

.pi-left {
  color: inherit;
}

.pi-left h2 {
  margin-top: 0;
  margin-bottom: 5px;
  color: inherit;
}

.pi-left .title {
  color: inherit;
  opacity: 0.7;
  margin-bottom: 20px;
}

.pi-photo {
  width: 260px;
  height: 260px;
  object-fit: cover;
  display: block;
}

.pi-bio {
  color: inherit;
}

.pi-bio p {
  margin-top: 0;
  margin-bottom: 12px;
  color: inherit;
}

/* Stack PI section on smaller screens */
@media screen and (max-width: 650px) {
  .pi-section {
    display: block;
    margin-left: 15px;
    margin-right: 15px;
  }

  .pi-left {
    margin-bottom: 20px;
  }

  .pi-photo {
    width: 100%;
    height: auto;
    aspect-ratio: 1 / 1;
  }
}

Then replace your PI HTML with this:

The key change is that h2, .title, and img all live inside:

<div class="pi-left">

That makes the name and title align with the left edge of the photo.

can you give me the code for the whole page to copy and paste

Here is the full page code to copy and paste. I kept the PI section static, theme-responsive, and arranged so the name/title align with the left side of the photo. I also preserved your flipping student cards and alumni section from the uploaded page.

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

/* The flip card container */
.flip-card {
  background-color: transparent;
  height: 420px;
  perspective: 1000px;
  cursor: pointer;
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
.flip-card-front,
.flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden;
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
  margin: 0 0 10px 0;
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

/* PI biography section: static, full-width, theme-responsive */
.pi-section {
  display: grid;
  grid-template-columns: 260px 1fr;
  column-gap: 30px;
  margin: 30px 15px 50px 15px;
  padding: 0;
  background: transparent;
  color: inherit;
  box-shadow: none;
}

.pi-left {
  color: inherit;
}

.pi-left h2 {
  margin-top: 0;
  margin-bottom: 5px;
  color: inherit;
}

.pi-left .title {
  color: inherit;
  opacity: 0.7;
  margin-bottom: 20px;
}

.pi-photo {
  width: 260px;
  height: 260px;
  object-fit: cover;
  display: block;
}

.pi-bio {
  color: inherit;
}

.pi-bio p {
  margin-top: 0;
  margin-bottom: 12px;
  color: inherit;
}

/* Stack PI section on smaller screens */
@media screen and (max-width: 650px) {
  .pi-section {
    display: block;
    margin-left: 15px;
    margin-right: 15px;
  }

  .pi-left {
    margin-bottom: 20px;
  }

  .pi-photo {
    width: 100%;
    height: auto;
    aspect-ratio: 1 / 1;
  }
}

</style>

<div class="pi-section">

  <div class="pi-left">
    <h2>Dr. Frederick Cheng</h2>
    <p class="title">Principal Investigator</p>

    <img src="/assets/img/blog/1456936992.png" alt="Frederick Cheng" class="pi-photo">
  </div>

  <div class="pi-bio">
    <p>
      I am an assistant professor in critical zone hydrology in the
      <a href="https://evsc.as.virginia.edu/">Department of Environmental Sciences at the University of Virginia</a>.
      I was previously a postdoctoral researcher in the Department of Ecosystem Science and Sustainability at
      Colorado State University.
    </p>

    <p>
      My research interests lie in the sustainable management of water resources by exploring interactions between
      hydrological and biogeochemical processes across scales. Topics of particular interest include modeling
      groundwater-surface water interactions, ecohydrological modeling across scales, and contaminant fate in watersheds.
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
          <p>Jack is a PhD student in the lab. He holds a bachelor's degree in Environmental Science from the University of Notre Dame, where he studied limnology and conducted studies at a field station in Northern Wisconsin. Additionally, he spent time studying the effects of PFAS biomagnification within Lake Michigan prey fish. At UVA, he studies nitrogen retention in wetlands, rivers, and lakes. Outside the lab, Jack enjoys running, playing Mario Kart, and traveling to Montana to explore the backcountry.</p>
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


1Password menu is available. Press down arrow to select.