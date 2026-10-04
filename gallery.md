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
    <img src="{{ '/assets/lab/h1.jpg' | relative_url }}" alt="Description of image 1">
    <div class="lab-caption">
      <h3>Solvent-based Plastic Recovery</h3>
      <p>Processing municipal solid waste streams to extract and recover post-consumer plastics using solvent-targeted methods.</p>
    </div>
  </div>

  <!-- Image 2 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/lab2.jpg' | relative_url }}" alt="Description of image 2">
    <div class="lab-caption">
      <h3>Biomass Pyrolysis Setup</h3>
      <p>Experimental setup for catalytic fast pyrolysis and biochar production from lignocellulosic feedstocks.</p>
    </div>
  </div>

  <!-- Image 3 -->
  <div class="lab-item">
   <img src="{{ '/assets/lab/h3.jpeg' | relative_url }}" alt="Solvent-based Plastic Recovery">
    <div class="lab-caption">
      <h3>Deep Eutectic Solvent Synthesis</h3>
      <p>Preparation and evaluation of deep eutectic solvents for xylan-to-furfural conversion.</p>
    </div>
  </div>

  <!-- Image 4 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/lab4.jpg' | relative_url }}" alt="Description of image 4">
    <div class="lab-caption">
      <h3>Materials Characterization</h3>
      <p>Using thermal analysis (DSC/TGA), spectroscopy, and microscopy to evaluate structure–property relationships of recovered polymers and biocomposites.</p>
    </div>
  </div>

  <!-- Image 5 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/lab5.jpg' | relative_url }}" alt="Description of image 5">
    <div class="lab-caption">
      <h3>Polymer Processing</h3>
      <p>Melt extrusion and cast-film processing of waste-derived and bio-based polymer systems.</p>
    </div>
  </div>

  <!-- Image 6 -->
  <div class="lab-item">
    <img src="{{ '/assets/lab/lab6.jpg' | relative_url }}" alt="Description of image 6">
    <div class="lab-caption">
      <h3>Laboratory Research Environment</h3>
      <p>Day-to-day experimental work in the Renewable Materials Laboratory at the University of Idaho.</p>
    </div>
  </div>

</div>

<style>
.lab-intro {
  max-width: 780px;
  margin: 0 auto 2.5rem;
  text-align: center;
  color: #000000;          /* Black */
  font-size: 1.05rem;
  line-height: 1.6;
}

.lab-gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 2rem;
  max-width: 1100px;
  margin: 0 auto 3rem;
}

.lab-item {
  background: #fff;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 16px rgba(0,0,0,0.08);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.lab-item:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 24px rgba(0,0,0,0.12);
}

.lab-item img {
  width: 100%;
  height: 240px;
  object-fit: cover;
  display: block;
}

.lab-caption {
  padding: 1.2rem 1.4rem 1.5rem;
}

.lab-caption h3 {
  margin: 0 0 0.5rem;
  font-size: 1.15rem;
  color: #111;
  font-weight: 600;
}

.lab-caption p {
  margin: 0;
  font-size: 0.95rem;
  line-height: 1.55;
  color: #000000;          /* Black */
}

@media (max-width: 700px) {
  .lab-gallery {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }
  
  .lab-item img {
    height: 220px;
  }
}
</style>
