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
      Chemist and materials/environmental researcher with a Ph.D. in Environmental Science (Material Chemistry) and an M.S. in Biomaterial Science (Chemistry). Research experience spans the chemical and materials valorization of municipal solid waste, solvent-targeted recovery of post-consumer plastics, polymer processing and biocomposites, biomass pyrolysis/biochar, and deep-eutectic-solvent conversion of lignocellulosic feedstocks to platform chemicals.
    </p>

    <p>
      Experienced in advanced chemical and materials characterization, laboratory method development, process optimization, and data-driven experimental research. Seeking a postdoctoral fellowship at the intersection of sustainable chemical manufacturing, circular materials, waste-derived feedstocks, and emerging conversion technologies.
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
  gap: 2.2rem;
  align-items: flex-start;
  max-width: 920px;
  margin: 2rem auto 3rem;
}

.about-photo {
  flex-shrink: 0;
  margin-top: 0.3rem;
}

.about-photo img {
  width: 240px;
  height: 240px;
  object-fit: cover;
  border-radius: 12px;
  display: block;
  box-shadow: 0 6px 18px rgba(0,0,0,0.3);
}

.about-text h1 {
  margin: 0 0 0.2rem;
  font-size: 1.85rem;
  font-weight: 700;
  color: #ffffff;
  line-height: 1.25;
}

.about-role {
  font-size: 0.95rem;
  color: #a0aec0;
  margin: 0 0 1.3rem;
}

.about-text p {
  font-size: 1.05rem;
  line-height: 1.7;
  color: #e2e8f0;
  margin-bottom: 1.1rem;
}

.about-links {
  margin-top: 1.6rem;
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
}

.about-links a:hover {
  border-bottom-color: #63b3ed;
}

@media (max-width: 700px) {
  .about-wrapper {
    flex-direction: column;
    align-items: center;
    text-align: center;
    gap: 1.5rem;
  }

  .about-photo {
    margin-top: 0;
  }

  .about-photo img {
    width: 210px;
    height: 210px;
  }
}
</style>
