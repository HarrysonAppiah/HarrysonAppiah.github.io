---
layout: page
title: Home
---

<div class="about-wrapper">
  <div class="about-photo">
    <img src="{{ '/assets/rofile.jpeg' | relative_url }}" alt="Harrison Appiah" />
  </div>

  <div class="about-text">
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
</div>

<style>
.about-wrapper {
  display: flex;
  gap: 2.8rem;
  align-items: flex-start;
  max-width: 920px;
  margin: 2.5rem auto 3rem;
}

.about-photo {
  flex-shrink: 0;
}

.about-photo img {
  width: 300px;
  height: 300px;
  object-fit: cover;
  border-radius: 14px;
  display: block;
  box-shadow: 0 8px 24px rgba(0,0,0,0.35);
}

.about-text h1 {
  margin: 0 0 0.3rem;
  font-size: 2rem;
  font-weight: 700;
  color: #ffffff;
}

.about-role {
  font-size: 0.95rem;
  color: #a0aec0;
  margin: 0 0 1.4rem;
}

.about-text p {
  font-size: 1.02rem;
  line-height: 1.75;
  color: #e2e8f0;
  margin-bottom: 1.1rem;
}

.about-links {
  margin-top: 1.8rem;
  display: flex;
  gap: 1.4rem;
}

.about-links a {
  font-size: 0.95rem;
  font-weight: 600;
  text-decoration: none;
  color: #63b3ed;
  border-bottom: 2px solid transparent;
  padding-bottom: 2px;
  transition: border-color 0.2s;
}

.about-links a:hover {
  border-bottom-color: #63b3ed;
}

@media (max-width: 700px) {
  .about-wrapper {
    flex-direction: column;
    align-items: center;
    text-align: center;
    gap: 1.8rem;
  }

  .about-photo img {
    width: 240px;
    height: 240px;
  }
}
</style>
