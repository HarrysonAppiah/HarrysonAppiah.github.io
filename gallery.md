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
    <img src="{{ '/assets/lab/h1.jpeg' | relative_url }}" alt="Solvent-based Plastic Recovery" onclick="openLightbox(0)">
    <div class="lab-caption">
      <h3>Solvent-based Plastic Recovery</h3>
      <p>Processing municipal solid waste streams to extract and recover post-consumer plastics using solvent-targeted methods.</p>
    </div>
  </div>

  <!-- Image 2 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/h2.jpeg' | relative_url }}" alt="some fun time" onclick="openLightbox(1)">
    <div class="lab-caption">
      <h3>some fun time</h3>
      <p>Who said lab work can't be fun?</p>
    </div>
  </div>

  <!-- Image 3 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/h3.jpeg' | relative_url }}" alt="some reflections" onclick="openLightbox(2)">
    <div class="lab-caption">
      <h3>The final caption</h3>
      <p>My research group.</p>
    </div>
  </div>

  <!-- Image 4 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/h4.jpeg' | relative_url }}" alt="Materials Characterization" onclick="openLightbox(3)">
    <div class="lab-caption">
      <h3>Materials Characterization</h3>
      <p>Using GC-MS to analyze plasticizers in extracted plastic.</p>
    </div>
  </div>

  <!-- Image 5 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/h5.jpeg' | relative_url }}" alt="Polymer Processing" onclick="openLightbox(4)">
    <div class="lab-caption">
      <h3>Polymer Processing</h3>
      <p>Melt extrusion and cast-film processing of waste-derived and bio-based polymer systems.</p>
    </div>
  </div>

  <!-- Image 6 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/h6.jpeg' | relative_url }}" alt="Laboratory Research Environment" onclick="openLightbox(5)">
    <div class="lab-caption">
      <h3>The Lab and Research in a nutshell</h3>
      <p>Day-to-day experimental work in the Renewable Materials Laboratory at the University of Idaho.</p>
    </div>
  </div>

</div>

<!-- Lightbox -->
<div id="lightbox">
  <span class="lightbox-close" onclick="closeLightbox()">×</span>
  <span class="lightbox-prev" onclick="changeImage(-1)">‹</span>
  <img id="lightbox-img" src="" alt="Enlarged view">
  <span class="lightbox-next" onclick="changeImage(1)">›</span>
</div>

<style>
.lab-intro {
  max-width: 780px;
  margin: 0 auto 2.5rem;
  text-align: center;
  color: inherit;
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
  height: 260px;
  object-fit: cover;
  display: block;
  cursor: pointer;
  transition: opacity 0.2s;
}

.lab-item img:hover {
  opacity: 0.92;
}

.lab-caption {
  padding: 0.9rem 1.2rem 1.1rem;
}

.lab-caption h3 {
  margin: 0 0 0.35rem;
  font-size: 1.08rem;
  color: #111111;
  font-weight: 600;
}

.lab-caption p {
  margin: 0;
  font-size: 0.9rem;
  line-height: 1.45;
  color: #222222;
}

html.dark-mode .lab-caption h3,
html.dark-mode .lab-caption p {
  color: #e2e8f0 !important;
}

html.dark-mode .lab-item {
  background: #1e1e1e !important;
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
  background: rgba(0,0,0,0.92);
  justify-content: center;
  align-items: center;
}

#lightbox-img {
  max-width: 85%;
  max-height: 85%;
  border-radius: 8px;
  box-shadow: 0 0 30px rgba(0,0,0,0.5);
  user-select: none;
}

.lightbox-close {
  position: absolute;
  top: 18px;
  right: 28px;
  color: white;
  font-size: 2.8rem;
  cursor: pointer;
  z-index: 10000;
  line-height: 1;
  opacity: 0.9;
}

.lightbox-prev,
.lightbox-next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  color: white;
  font-size: 3.5rem;
  cursor: pointer;
  padding: 0 18px;
  user-select: none;
  z-index: 10000;
  opacity: 0.85;
}

.lightbox-prev:hover,
.lightbox-next:hover,
.lightbox-close:hover {
  opacity: 1;
}

.lightbox-prev { left: 8px; }
.lightbox-next { right: 8px; }

@media (max-width: 700px) {
  .lab-gallery {
    grid-template-columns: 1fr;
  }
  .lab-item img {
    height: 240px;
  }
  .lightbox-prev, .lightbox-next {
    font-size: 2.6rem;
  }
}
</style>

<script>
  const galleryImages = [
    "{{ '/assets/lab/h1.jpeg' | relative_url }}",
    "{{ '/assets/lab/h2.jpeg' | relative_url }}",
    "{{ '/assets/lab/h3.jpeg' | relative_url }}",
    "{{ '/assets/lab/h4.jpeg' | relative_url }}",
    "{{ '/assets/lab/h5.jpeg' | relative_url }}",
    "{{ '/assets/lab/h6.jpeg' | relative_url }}"
  ];

  let currentIndex = 0;

  function openLightbox(index) {
    currentIndex = index;
    document.getElementById('lightbox-img').src = galleryImages[currentIndex];
    document.getElementById('lightbox').style.display = 'flex';
  }

  function closeLightbox() {
    document.getElementById('lightbox').style.display = 'none';
  }

  function changeImage(direction) {
    currentIndex += direction;
    if (currentIndex < 0) currentIndex = galleryImages.length - 1;
    if (currentIndex >= galleryImages.length) currentIndex = 0;
    document.getElementById('lightbox-img').src = galleryImages[currentIndex];
  }

  // Keyboard navigation
  document.addEventListener('keydown', function(e) {
    const lightbox = document.getElementById('lightbox');
    if (lightbox.style.display !== 'flex') return;

    if (e.key === 'Escape') closeLightbox();
    if (e.key === 'ArrowRight') changeImage(1);
    if (e.key === 'ArrowLeft') changeImage(-1);
  });

  // Close when clicking the dark background
  document.getElementById('lightbox').addEventListener('click', function(e) {
    if (e.target === this) closeLightbox();
  });
</script>
