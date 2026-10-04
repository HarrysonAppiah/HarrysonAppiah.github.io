---
layout: page
title: Home
---

<div class="about-wrapper">
  <img class="about-photo" src="{{ '/assets/rofile.jpeg' | relative_url }}" alt="Harrison Appiah" />

  <h1>Harrison Appiah</h1>
  <p class="about-role">PhD — University of Idaho | Material & Environmental Science</p>

  <p>
    I am a researcher with a deep interest in biomaterials science and waste valorization — and a technical foundation that spans green chemistry, analytical chemistry, wet chemistry, printed circuit board chemistry, and semiconductor fabrication. My work sits at the intersection of biomass valorization and sustainable materials, exploring how agricultural residues, municipal solid waste, and end-of-life plastics can be transformed into useful fuels, chemicals, and packaging materials.
  </p>

  <p>
    My research spans catalytic fast pyrolysis, deep eutectic solvent systems for furfural synthesis, solvent-based plastic recovery, and the development of lignin- and xylan-derived bioproducts. This work is grounded in rigorous analytical and wet chemistry practice — the same discipline that informs my experience with semiconductor fabrication processes and the precise chemical control demanded by printed circuit board manufacturing. A common thread runs through all of it: the conviction that a circular economy is not just an aspiration but an engineering problem — one that can be solved with the right chemistry and process design.
  </p>

  <p>
    What drives me is the global urgency of waste. Millions of tons of biomass, plastics, and municipal solid waste are generated every year with little recovery. My background in high-precision chemical systems — from semiconductor-grade processes to PCB fabrication chemistry — gives me a distinct perspective on how tightly controlled industrial chemistries can be reimagined and redirected toward sustainable ends. I find it deeply motivating to work on systems that close those loops, recovering materials, generating energy, and reducing environmental burden all at once.
  </p>

  <p>
    Looking ahead, I am eager to bring this work into industry R&D, where I can help scale sustainable technologies and embed circular economy principles into real-world manufacturing and materials pipelines — drawing on both my sustainable chemistry research and my hands-on expertise in advanced fabrication and analytical systems.
  </p>

  <div class="about-links">
    <a href="{{ '/publications/' | relative_url }}">Publications</a>
    <a href="{{ '/research/' | relative_url }}">Research</a>
  </div>
</div>

<style>
.about-wrapper {
  max-width: 900px;
  margin: 2rem auto 3rem;
  overflow: hidden;
}

.about-photo {
  float: left;
  width: 240px;
  height: 240px;
  object-fit: cover;
  border-radius: 12px;
  margin: 0 1.8rem 1rem 0;
  box-shadow: 0 6px 18px rgba(0,0,0,0.15);
}

.about-wrapper h1 {
  margin: 0 0 0.25rem;
  font-size: 1.9rem;
  font-weight: 700;
  color: #111111;
  line-height: 1.25;
}

.about-role {
  font-size: 0.95rem;
  color: #333333;
  margin: 0 0 1.2rem;
}

.about-wrapper p {
  font-size: 1.05rem;
  line-height: 1.7;
  color: #222222;
  margin-bottom: 1.1rem;
}

.about-links {
  margin-top: 1.6rem;
  clear: both;
  display: flex;
  gap: 1.4rem;
}

.about-links a {
  font-size: 0.95rem;
  font-weight: 600;
  text-decoration: none;
  color: #1a56db;
  border-bottom: 2px solid transparent;
  padding-bottom: 2px;
}

.about-links a:hover {
  border-bottom-color: #1a56db;
}

@media (max-width: 650px) {
  .about-photo {
    float: none;
    display: block;
    margin: 0 auto 1.5rem;
    width: 210px;
    height: 210px;
  }

  .about-wrapper {
    text-align: center;
  }

  .about-links {
    justify-content: center;
  }
}
</style>
