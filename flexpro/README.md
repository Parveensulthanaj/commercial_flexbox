# Ex02 Commercial Website
## Date:

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
```
flex.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Thalam | Handmade Indian Musical Instruments, Chennai</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Anton&family=Hind:wght@400;500;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="flex.css">
</head>
<body>

  <header class="site-header">
    <a href="#top" class="logo">Thalam</a>
    <nav>
      <ul class="nav-list">
        <li><a href="#instruments">Instruments</a></li>
        <li><a href="#workshop">Workshop</a></li>
        <li><a href="#visit">Visit</a></li>
        <li><a href="#enquire" class="btn btn-small">Book a trial</a></li>
      </ul>
    </nav>
  </header>

  <main id="top">

    <!-- HERO: giant headline row that wraps word by word -->
    <section class="hero">
      <h1 class="hero-title">
        <span>Made</span><span class="pill">by hand</span><span>in</span>
        <span class="pill pill-alt">Mylapore</span><span>for your</span><span class="pill">next</span><span>raga.</span>
      </h1>
      <div class="hero-side">
        <p>Veenas, flutes, mridangams and tanpuras built one at a time by third-generation craftsmen. Every instrument is tuned and played by a teacher before it ships.</p>
        <a href="#instruments" class="btn">Meet the instruments</a>
      </div>
    </section>

    <!-- INSTRUMENT PANELS: flex-grow expands the hovered or focused panel -->
    <section id="instruments" class="section">
      <h2>Pick one up. Literally.</h2>
      <p class="section-intro">Hover or tab through the panels to open them.</p>
      <div class="panels">
        <article class="panel p1" tabindex="0">
          <h3>Saraswati Veena</h3>
          <div class="panel-more">
            <p>Jackwood body, brass frets set by ear. Ships with a cover and spare strings.</p>
            <span class="price">from ₹68,000</span>
          </div>
        </article>
        <article class="panel p2" tabindex="0">
          <h3>Bamboo Flute</h3>
          <div class="panel-more">
            <p>Cured for two years before drilling. Available in 8 scales, A to G#.</p>
            <span class="price">from ₹2,400</span>
          </div>
        </article>
        <article class="panel p3" tabindex="0">
          <h3>Mridangam</h3>
          <div class="panel-more">
            <p>Jackfruit shell, goat-skin heads, pre-tuned to your pitch.</p>
            <span class="price">from ₹14,500</span>
          </div>
        </article>
        <article class="panel p4" tabindex="0">
          <h3>Tanpura</h3>
          <div class="panel-more">
            <p>Long-sustain gourd body with a clean jawari bridge.</p>
            <span class="price">from ₹22,000</span>
          </div>
        </article>
      </div>
    </section>

    <!-- WORKSHOP: a real sequence, so steps are numbered -->
    <section id="workshop" class="section section-dark">
      <h2>From a log to your living room</h2>
      <ol class="steps">
        <li class="step"><b>1</b><h3>Seasoning</h3><p>Wood rests 18 months before it is cut.</p></li>
        <li class="step"><b>2</b><h3>Carving</h3><p>One craftsman shapes one instrument start to finish.</p></li>
        <li class="step"><b>3</b><h3>Tuning</h3><p>A working musician plays and adjusts it.</p></li>
        <li class="step"><b>4</b><h3>Delivery</h3><p>Packed in a hard case, insured, 5 days across India.</p></li>
      </ol>
    </section>

    <!-- VISIT + ENQUIRY -->
    <section id="visit" class="section visit">
      <div class="visit-info">
        <h2>Come play before you buy</h2>
        <p>Our showroom is open Tuesday to Sunday, 10 am to 7 pm. Trial sessions last 30 minutes and are free.</p>
        <p>14 Kutchery Road, Mylapore, Chennai<br>+91 98765 43210</p>
      </div>
      <form id="enquire" class="enquire" action="#" method="post">
        <label>Your name <input type="text" name="name" required></label>
        <label>Phone <input type="tel" name="phone" required></label>
        <label>Instrument
          <select name="instrument">
            <option>Saraswati Veena</option>
            <option>Bamboo Flute</option>
            <option>Mridangam</option>
            <option>Tanpura</option>
          </select>
        </label>
        <button type="submit" class="btn">Book my trial</button>
      </form>
    </section>

  </main>

  <footer class="site-footer">
    <p>© 2026 Thalam Instruments, Chennai</p>
    <ul class="footer-links">
      <li><a href="#instruments">Instruments</a></li>
      <li><a href="#workshop">Workshop</a></li>
      <li><a href="#visit">Visit</a></li>
    </ul>
  </footer>

</body>
</html>


```

```
flex.css
/* ===== Thalam: creative Flexbox commercial website ===== */

:root {
  --peacock: #0b4f6c;
  --marigold: #ff9f1c;
  --rose: #e5446d;
  --ink: #101820;
  --paper: #ffffff;
  --mist: #eef3f5;
  --muted: #53636b;
}

* { box-sizing: border-box; margin: 0; padding: 0; }
html { scroll-behavior: smooth; }

body {
  font-family: "Hind", system-ui, sans-serif;
  color: var(--ink);
  background: var(--mist);
  line-height: 1.6;
  display: flex;               /* sticky-footer layout */
  flex-direction: column;
  min-height: 100vh;
}
main { flex: 1; }

h1, h2, h3, .logo, .price { font-family: "Anton", Impact, sans-serif; font-weight: 400; letter-spacing: 0.01em; line-height: 1.05; }
a { color: inherit; text-decoration: none; }
ul, ol { list-style: none; }

a:focus-visible, button:focus-visible, input:focus-visible,
select:focus-visible, .panel:focus-visible { outline: 3px solid var(--marigold); outline-offset: 3px; }

/* ===== Buttons ===== */
.btn {
  display: inline-flex; align-items: center; justify-content: center;
  padding: 0.9rem 1.8rem;
  background: var(--marigold); color: var(--ink);
  font: 600 1rem "Hind", sans-serif;
  border: 2px solid var(--ink); border-radius: 999px; cursor: pointer;
}
.btn:hover { background: var(--ink); color: var(--marigold); }
.btn-small { padding: 0.45rem 1.1rem; font-size: 0.95rem; }

/* ===== Header ===== */
.site-header {
  display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 1rem;
  padding: 1rem 5%;
  background: var(--paper);
  border-bottom: 3px solid var(--ink);
  position: sticky; top: 0; z-index: 10;
}
.logo { font-size: 2rem; color: var(--peacock); }
.nav-list { display: flex; align-items: center; gap: 1.75rem; font-weight: 500; }
.nav-list a:not(.btn):hover { color: var(--rose); }

/* ===== Hero: wrapping flex row of words and pills ===== */
.hero {
  display: flex; flex-wrap: wrap; align-items: flex-end; justify-content: space-between;
  gap: 2.5rem;
  padding: 4rem 5%;
}
.hero-title {
  flex: 1 1 560px;
  display: flex; flex-wrap: wrap; align-items: center;
  gap: 0.15em 0.3em;
  font-size: clamp(3rem, 8.5vw, 7rem);
  text-transform: uppercase;
}
.pill {
  display: inline-flex; align-items: center;
  padding: 0 0.3em;
  background: var(--marigold);
  border: 3px solid var(--ink);
  border-radius: 999px;
  transform: rotate(-2deg);
}
.pill-alt { background: var(--rose); color: var(--paper); transform: rotate(2deg); }
.hero-side { flex: 0 1 340px; display: flex; flex-direction: column; align-items: flex-start; gap: 1.25rem; }
.hero-side p { color: var(--muted); font-size: 1.1rem; }

/* ===== Sections ===== */
.section { padding: 4.5rem 5%; }
.section h2 { font-size: clamp(2rem, 4.5vw, 3.2rem); text-transform: uppercase; }
.section-intro { color: var(--muted); margin-top: 0.5rem; }

/* ===== Expanding panels (the main Flexbox showpiece) ===== */
.panels {
  display: flex;
  gap: 0.75rem;
  height: 440px;
  margin-top: 2rem;
}
.panel {
  flex: 1;                                   /* all panels start equal */
  min-width: 0;
  display: flex; flex-direction: column; justify-content: flex-end; gap: 0.75rem;
  padding: 1.25rem;
  border: 3px solid var(--ink);
  border-radius: 20px;
  color: var(--paper);
  overflow: hidden;
  cursor: pointer;
  transition: flex-grow 0.5s ease;
}
.panel:hover, .panel:focus-visible, .panel:focus-within { flex-grow: 4; }  /* hovered panel takes 4x space */
.panel h3 { font-size: 1.7rem; text-transform: uppercase; }

.panel-more {
  display: flex; flex-direction: column; gap: 0.5rem;
  max-height: 0; opacity: 0; overflow: hidden;
  transition: max-height 0.4s ease, opacity 0.4s ease;
}
.panel:hover .panel-more, .panel:focus-visible .panel-more { max-height: 200px; opacity: 1; }
.panel-more .price { font-size: 1.5rem; color: var(--marigold); }

.p1 { background: var(--peacock); }
.p2 { background: var(--rose); }
.p3 { background: #6a3d9a; }
.p4 { background: #1b7f5c; }

/* ===== Workshop steps ===== */
.section-dark { background: var(--ink); color: var(--paper); }
.section-dark h2 { color: var(--marigold); }
.steps { display: flex; flex-wrap: wrap; gap: 1.5rem; margin-top: 2rem; }
.step {
  flex: 1 1 220px;
  display: flex; flex-direction: column; gap: 0.5rem;
  padding: 1.25rem;
  border: 2px solid #33414c;
  border-radius: 16px;
}
.step b {
  display: flex; align-items: center; justify-content: center;
  width: 2.4rem; height: 2.4rem;
  background: var(--marigold); color: var(--ink);
  border-radius: 50%;
  font-family: "Anton", sans-serif; font-weight: 400;
}
.step h3 { font-size: 1.4rem; text-transform: uppercase; }
.step p { color: #b7c4cc; }
/* staggered heights using align-self on a row container */
.step:nth-child(even) { margin-top: 1.5rem; }

/* ===== Visit and enquiry ===== */
.visit { display: flex; flex-wrap: wrap; gap: 3rem; background: var(--paper); }
.visit-info { flex: 1 1 300px; display: flex; flex-direction: column; gap: 1rem; }
.enquire {
  flex: 1 1 340px;
  display: flex; flex-direction: column; gap: 1rem;
  padding: 1.75rem;
  background: var(--mist);
  border: 3px solid var(--ink);
  border-radius: 20px;
}
.enquire label { display: flex; flex-direction: column; gap: 0.3rem; font-weight: 600; }
.enquire input, .enquire select {
  padding: 0.75rem; font: inherit;
  border: 2px solid var(--ink); border-radius: 10px; background: var(--paper);
}
.enquire .btn { align-self: flex-start; }

/* ===== Footer ===== */
.site-footer {
  display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 1rem;
  padding: 1.5rem 5%;
  background: var(--peacock); color: var(--paper);
}
.footer-links { display: flex; gap: 1.5rem; }
.footer-links a:hover { color: var(--marigold); }

/* ===== Mobile: panels stack, tap to open ===== */
@media (max-width: 768px) {
  .site-header { flex-direction: column; }
  .nav-list { flex-wrap: wrap; justify-content: center; gap: 1rem; }
  .panels { flex-direction: column; height: 560px; }
  .panel { flex: 1; }
  .panel:hover, .panel:focus-visible, .panel:focus-within { flex-grow: 3; }
  .step:nth-child(even) { margin-top: 0; }
  .site-footer { flex-direction: column; text-align: center; }
}

@media (prefers-reduced-motion: reduce) {
  html { scroll-behavior: auto; }
  .panel, .panel-more { transition: none; }
}

```

## OUTPUT


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
