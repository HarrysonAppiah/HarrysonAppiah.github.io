---

layout: page
title: Home
-----------

<style>
/* =========================================================
   Harrison Appiah — Homepage
   Designed to work with the existing Jekyll frame theme
   ========================================================= */

.homepage {
  max-width: 1100px;
  margin: 0 auto;
}

/* ---------- Hero ---------- */

.hero {
  display: grid;
  grid-template-columns: minmax(220px, 340px) 1fr;
  gap: clamp(2rem, 5vw, 4.5rem);
  align-items: center;
  padding: clamp(1rem, 3vw, 2rem) 0 3rem;
}

.hero-photo {
  text-align: center;
}

.hero-photo img {
  width: min(100%, 330px);
  aspect-ratio: 1 / 1;
  object-fit: cover;
  border-radius: 18px;
  display: block;
  margin: 0 auto;
  box-shadow: 0 8px 30px rgba(0, 0, 0, 0.12);
}

.hero-text h1 {
  margin: 0 0 0.35rem;
  font-size: clamp(2rem, 5vw, 3.25rem);
  line-height: 1.05;
  letter-spacing: -0.03em;
}

.hero-role {
  margin: 0 0 1.25rem;
  font-size: 1.05rem;
  font-weight: 600;
  opacity: 0.72;
}

.hero-intro {
  font-size: 1.08rem;
  line-height: 1.75;
  max-width: 720px;
  margin-bottom: 1.5rem;
}

.hero-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.7rem;
}

.hero-links a {
  display: inline-block;
  padding: 0.65rem 1rem;
  border: 1px solid currentColor;
  border-radius: 7px;
  text-decoration: none;
  font-size: 0.9rem;
  font-weight: 600;
  opacity: 0.85;
  transition: opacity 0.2s ease, transform 0.2s ease;
}

.hero-links a:hover {
  opacity: 1;
  transform: translateY(-2px);
}

/* ---------- Sections ---------- */

.home-section {
  padding: 2.5rem 0;
  border-top: 1px solid rgba(127, 127, 127, 0.25);
}

.home-section h2 {
  margin: 0 0 0.45rem;
  font-size: 1.55rem;
  letter-spacing: -0.02em;
}

.section-lead {
  margin: 0 0 1.7rem;
  max-width: 800px;
  line-height: 1.7;
  opacity: 0.78;
}

/* ---------- Research cards ---------- */

.research-grid {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 1rem;
}

.research-card {
  padding: 1.35rem;
  border: 1px solid rgba(127, 127, 127, 0.25);
  border-radius: 12px;
  background: rgba(127, 127, 127, 0.045);
}

.research-card h3 {
  margin: 0 0 0.55rem;
  font-size: 1.05rem;
}

.research-card p {
  margin: 0;
  line-height: 1.65;
  font-size: 0.94rem;
  opacity: 0.8;
}

/* ---------- Current research ---------- */

.current-research {
  font-size: 1.02rem;
  line-height: 1.8;
  max-width: 900px;
}

.current-research strong {
  font-weight: 700;
}

/* ---------- Expertise ---------- */

.expertise {
  display: flex;
  flex-wrap: wrap;
  gap: 0.55rem;
}

.expertise span {
  display: inline-block;
  padding: 0.5rem 0.75rem;
  border: 1px solid rgba(127, 127, 127, 0.28);
  border-radius: 999px;
  font-size: 0.82rem;
  line-height: 1;
  opacity: 0.82;
}

/* ---------- Closing section ---------- */

.home-closing {
  padding: 2.5rem 0 1rem;
  text-align: center;
}

.home-closing p {
  max-width: 760px;
  margin: 0 auto 1.25rem;
  line-height: 1.75;
  opacity: 0.78;
}

.home-closing a {
  font-weight: 600;
}

/* ---------- Responsive ---------- */

@media (max-width: 720px) {

  .hero {
    grid-template-columns: 1fr;
    text-align: center;
    gap: 1.75rem;
    padding-top: 0.5rem;
  }

  .hero-photo img {
    width: min(100%, 300px);
  }

  .hero-intro {
    font-size: 1rem;
  }

  .hero-links {
    justify-content: center;
  }

  .research-grid {
    grid-template-columns: 1fr;
  }

  .home-section {
    padding: 2rem 0;
  }

  .home-section h2 {
    font-size: 1.35rem;
  }
}
</style>

<div class="homepage">

  <!-- HERO -->

  <section class="hero">

```
<div class="hero-photo">
  <img
    src="{{ '/assets/rofile.jpeg' | relative_url }}"
    alt="Harrison Appiah"
  />
</div>

<div class="hero-text">

  <h1>Harrison Appiah</h1>

  <p class="hero-role">
    PhD Researcher · Materials &amp; Environmental Science
  </p>

  <p class="hero-intro">
    I am a materials and environmental scientist working at the
    intersection of <strong>sustainable chemistry, waste valorization,
    materials characterization, and chemical process development.</strong>
    My research focuses on transforming heterogeneous waste streams
    into useful materials, chemicals, and energy while developing the
    analytical and process understanding needed for scalable applications.
  </p>

  <div class="hero-links">
    <a href="{{ '/research/' | relative_url }}">Research</a>
    <a href="{{ '/publications/' | relative_url }}">Publications</a>
    <a href="{{ '/resume/' | relative_url }}">Resume</a>
  </div>

</div>
```

  </section>

  <!-- RESEARCH -->

  <section class="home-section">

```
<h2>Research Focus</h2>

<p class="section-lead">
  My work combines experimental chemistry, materials science, analytical
  characterization, and process optimization to address challenges in
  resource recovery and sustainable chemical manufacturing.
</p>

<div class="research-grid">

  <div class="research-card">
    <h3>Waste &amp; Polymer Valorization</h3>
    <p>
      Solvent-based recovery and characterization of polymers from
      municipal solid waste and end-of-life plastics, with emphasis on
      purification, processing, and materials performance.
    </p>
  </div>

  <div class="research-card">
    <h3>Biomass &amp; Bioproducts</h3>
    <p>
      Conversion of lignocellulosic and biomass-derived feedstocks into
      biochar, platform chemicals, and value-added products through
      thermochemical and chemical conversion pathways.
    </p>
  </div>

  <div class="research-card">
    <h3>Chemical Conversion &amp; Catalysis</h3>
    <p>
      Development of chemical and potentially electrified or catalytic
      strategies for converting heterogeneous waste-derived feedstocks
      into useful chemicals and functional materials.
    </p>
  </div>

  <div class="research-card">
    <h3>Materials &amp; Chemical Analysis</h3>
    <p>
      Application of chromatographic, spectroscopic, thermal, rheological,
      and microscopic techniques to understand composition, structure,
      processing behavior, and material performance.
    </p>
  </div>

</div>
```

  </section>

  <!-- CURRENT RESEARCH -->

  <section class="home-section">

```
<h2>Current Research Direction</h2>

<p class="current-research">
  My current research direction is centered on developing
  <strong>sustainable and potentially electrified or catalytic
  chemical-conversion strategies for heterogeneous waste-derived
  feedstocks.</strong>
  This builds on established expertise in plastic recovery, polymer
  characterization, biomass conversion, and process optimization while
  expanding toward next-generation sustainable chemical manufacturing.
</p>

<p class="current-research">
  A major theme of this work is connecting <strong>feedstock chemistry,
  reaction pathways, analytical characterization, and process
  performance</strong> so that laboratory-scale discoveries can ultimately
  inform practical materials and chemical-processing systems.
</p>
```

  </section>

  <!-- TECHNICAL EXPERTISE -->

  <section class="home-section">

```
<h2>Analytical &amp; Experimental Expertise</h2>

<p class="section-lead">
  My experimental background spans chemical analysis, materials
  characterization, wet chemistry, polymer processing, and thermal analysis.
</p>

<div class="expertise">
  <span>GC-MS</span>
  <span>GC</span>
  <span>HPLC / UHPLC</span>
  <span>FTIR</span>
  <span>UV-Vis</span>
  <span>Py-GC-MS</span>
  <span>DSC</span>
  <span>TGA</span>
  <span>DMA</span>
  <span>TMA</span>
  <span>Rheology</span>
  <span>BET</span>
  <span>XRD</span>
  <span>SEM</span>
  <span>Wet Chemistry</span>
  <span>Polymer Characterization</span>
  <span>Process Optimization</span>
</div>
```

  </section>

  <!-- INDUSTRY / CAREER DIRECTION -->

  <section class="home-section">

```
<h2>Research to Application</h2>

<p class="current-research">
  I am interested in research and development environments where
  chemistry, materials science, analytical science, and manufacturing
  intersect — including <strong>sustainable chemical manufacturing,
  advanced materials, semiconductor and electronics manufacturing,
  national laboratory research, and aerospace-related technologies.</strong>
</p>
```

  </section>

  <!-- CLOSING -->

  <section class="home-closing">

```
<p>
  Explore my research, publications, and professional background to learn
  more about my work and current research interests.
</p>

<p>
  <a href="{{ '/research/' | relative_url }}">Explore Research →</a>
</p>
```

  </section>

</div>
