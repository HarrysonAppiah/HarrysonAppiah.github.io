---
layout: page
title: Home
---
---

<div class="about-wrapper">
  <div class="about-photo">
    <img src="{{ '/assets/rofile.jpeg' | relative_url }}" alt="Harrison Appiah" />

  <div class="about-text">
    <h1>Harrison Appiah</h1>
    <p class="about-role">PhD &mdash; University of Idaho | Material & Environmental Science</p>

    <p>
      I am a researcher with a deep interest in biomaterials science and  waste valorization — and a technical foundation that spans green chemistry, analytical chemistry, wet chemistry, printed circuit board chemistry, and semiconductor fabrication. My work sits at the intersection of biomass valorization and sustainable materials, exploring how agricultural residues, municipal solid waste, and end-of-life plastics can be transformed into useful fuels, chemicals, and packaging materials.
    </p>

    <p>
      My research spans catalytic fast pyrolysis, deep eutectic solvent systems for furfural synthesis, solvent-based plastic recovery, and the development of lignin- and xylan-derived bioproducts. This work is grounded in rigorous analytical and wet chemistry practice — the same discipline that informs my experience with semiconductor fabrication processes and the precise chemical control demanded by printed circuit board manufacturing. A common thread runs through all of it: the conviction that a circular economy is not just an aspiration but an engineering problem — one that can be solved with the right chemistry and process design.
    </p>

    <p>
      What drives me is the global urgency of waste. Millions of tons of biomass, plastics, and municipal solid waste are generated every year with little recovery. My background in high-precision chemical systems — from semiconductor-grade processes to PCB fabrication chemistry — gives me a distinct perspective on how tightly controlled industrial chemistries can be reimagined and redirected toward sustainable ends. I find it deeply motivating to work on systems that close those loops, recovering materials, generating energy, and reducing environmental burden all at once..
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
  gap: 2.5rem;
  align-items: flex-start;
  max-width: 820px;
  margin-top: 1.5rem;
}

.about-photo img {
  width: 360px;
  height: 360px;
  object-fit: cover;
  border-radius: 12px;
  display: block;
  flex-shrink: 0;
  border: 3px solid rgba(255, 255, 255, 0.3);
}

.about-text h1 {
  margin: 0 0 0.15rem;
  font-size: 1.6rem;
  color: #ffffff;
}

.about-role {
  font-size: 0.9rem;
  color: rgba(255, 255, 255, 0.7);
  margin: 0 0 1.25rem;
}

.about-text p {
  font-size: 0.975rem;
  line-height: 1.8;
  color: rgba(255, 255, 255, 0.9);
  margin-bottom: 1rem;
}

.about-links {
  margin-top: 1.5rem;
  display: flex;
  gap: 1rem;
}

.about-links a {
  font-size: 0.875rem;
  font-weight: 600;
  text-decoration: none;
  color: #ffffff;
  border-bottom: 2px solid rgba(255, 255, 255, 0.5);
  padding-bottom: 2px;
}

.about-links a:hover {
  border-bottom-color: #ffffff;
}

@media (max-width: 600px) {
  .about-wrapper {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }
 .about-photo img {
  width: 500px;
  height: 360px;
  object-fit: cover;
  border-radius: 12px;
  display: block;
  flex-shrink: 0;
  border: 3px solid rgba(255, 255, 255, 0.3);
}
  }
}
  </style>



  <div style="margin-top: 15px;">
    {% for item in site.external %}
      <a href="{{ item.url }}" style="margin: 0 10px; text-decoration: none;">
        {{ item.title }}
      </a>
    {% endfor %}
  </div>





<hr>

<section class="recent-posts">
  <h2>Monday Musings</h2>

  {% for post in site.posts limit:5 %}
    <article class="post-preview">
      <h3>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>

      <p class="post-date">
        {{ post.date | date: "%B %-d, %Y" }}
      </p>

      <div class="post-excerpt">
        {{ post.excerpt }}
      </div>

      <a class="read-more" href="{{ post.url | relative_url }}">
        Read More →
      </a>
    </article>
  {% endfor %}
</section>

<style>
.recent-posts {
  max-width: 820px;
  margin: 3rem auto;
}

.recent-posts h2 {
  margin-bottom: 2rem;
  color: #ffffff;
}

.post-preview {
  margin-bottom: 3rem;
}

.post-preview h3 {
  margin-bottom: 0.25rem;
}

.post-preview h3 a {
  color: #ffffff;
  text-decoration: none;
}

.post-preview h3 a:hover {
  text-decoration: underline;
}

.post-date {
  font-size: 0.85rem;
  color: rgba(255, 255, 255, 0.6);
}

.post-excerpt {
  line-height: 1.8;
  color: rgba(255, 255, 255, 0.9);
}

.read-more {
  display: inline-block;
  margin-top: 0.5rem;
  color: #ffffff;
  font-weight: 600;
  text-decoration: none;
  border-bottom: 2px solid rgba(255, 255, 255, 0.5);
  padding-bottom: 2px;
}

.read-more:hover {
  border-bottom-color: #ffffff;
}
</style>



  
</div>


