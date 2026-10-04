---
layout: page
title: Lab Gallery
permalink: /lab/
---

<div class="lab-intro">
  <p>
    A selection of photographs from my research activities in the laboratory — 
    covering municipal solid waste processing, polymer recovery, biomass conversion, 
    and materials characterization.
  </p>
</div>

<div class="lab-gallery">

  <!-- Image 1 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/h1.jpeg' | relative_url }}" alt="Solvent-based Plastic Recovery" onclick="openLightbox(this)">
    <div class="lab-caption">
      <h3>Solvent-based Plastic Recovery</h3>
      <p> Processing municipal solid waste streams to extract and recover post-consumer plastics using solvent-targeted methods.</p>
    </div>
  </div>

  <!-- Image 2 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/h2.jpeg' | relative_url }}" alt="Biomass Pyrolysis Setup" onclick="openLightbox(this)">
    <div class="lab-caption">
      <h3> some fun time</h3>
      <p> Who said lab work can't be fun? </p>
    </div>
  </div>

  <!-- Image 3 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/h3.jpg' | relative_url }}" alt="some reflections" onclick="openLightbox(this)">
    <div class="lab-caption">
      <h3>The final caption</h3>
      <p>My research group.</p>
    </div>
  </div>

  <!-- Image 4 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/h4.jpeg' | relative_url }}" alt="Materials Characterization" onclick="openLightbox(this)">
    <div class="lab-caption">
      <h3>Materials Characterization</h3>
      <p>Using GC-MS to analyze plasticizers in extracted plastic.</p>
    </div>
  </div>

  <!-- Image 5 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/h5.jpeg' | relative_url }}" alt="Polymer Processing" onclick="openLightbox(this)">
    <div class="lab-caption">
      <h3>Polymer Processing</h3>
      <p>Melt extrusion and cast-film processing of waste-derived and bio-based polymer systems.</p>
    </div>
  </div>

  <!-- Image 6 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/lab6.jpg' | relative_url }}" alt="Laboratory Research Environment" onclick="openLightbox(this)">
    <div class="lab-caption">
      <h3>Laboratory Research Environment</h3>
      <p>Day-to-day experimental work in the Renewable Materials Laboratory at the University of Idaho.</p>
    </div>
  </div>

</div>

<!-- Lightbox -->
<div id="lightbox" onclick="closeLightbox()">
  <img id="lightbox-img" src="" alt="Enlarged view">
</div>

<style>
.lab-intro {
  max-width: 780px;
  margin: 0 auto 2.5rem;
  text-align: center;
  color: #000;
  font-size: 1.05rem;
  line-height: 1.6;
}

.lab-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.8rem;
  max-width: 1100px;
  margin: 0 auto 3rem;
}

.lab-item {
  background: #fff;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 14px rgba(0,0,0,0.08);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  display: flex;
  flex-direction: column;
}

.lab-item:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 22px rgba(0,0,0,0.12);
}

.lab-item img {
  width: 100%;
  height: 260px;               /* taller image area */
  object-fit: cover;
  display: block;
  cursor: pointer;
  transition: opacity 0.2s;
}

.lab-item img:hover {
  opacity: 0.92;
}

.lab-caption {
  padding: 0.9rem 1.2rem 1.1rem;  /* more compact */
}

.lab-caption h3 {
  margin: 0 0 0.35rem;
  font-size: 1.08rem;
  color: #111;
  font-weight: 600;
}

.lab-caption p {
  margin: 0;
  font-size: 0.9rem;
  line-height: 1.45;
  color: #000;
}

/* Lightbox */
#lightbox {
  display: none;
  position: fixed;
  z-index: 9999;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0,0,0,0.9);
  justify-content: center;
  align-items: center;
  cursor: zoom-out;
}

#lightbox-img {
  max-width: 90%;
  max-height: 90%;
  border-radius: 8px;
  box-shadow: 0 0 30px rgba(0,0,0,0.5);
}

@media (max-width: 700px) {
  .lab-gallery {
    grid-template-columns: 1fr;
  }
  .lab-item img {
    height: 240px;
  }
}
</style>

<script>
  function openLightbox(img) {
    const lightbox = document.getElementById('lightbox');
    const lightboxImg = document.getElementById('lightbox-img');
    lightboxImg.src = img.src;
    lightbox.style.display = 'flex';
  }

  function closeLightbox() {
    document.getElementById('lightbox').style.display = 'none';
  }

  // Close with Escape key
  document.addEventListener('keydown', function(e) {
    if (e.key === 'Escape') closeLightbox();
  });
</script>
