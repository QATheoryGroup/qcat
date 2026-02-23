---
layout: page
title: Quantum Computing Applications & Theory
sitemap: false
permalink: /
carousels:
  - images: 
    - image: /images/carousel/1.PNG
    - image: /images/carousel/2.PNG
    - image: /images/carousel/1.PNG
    - image: /images/carousel/2.PNG
---

We are a theoretical quantum computing research group at the University of Queensland in Brisbane, Australia. 

Led by [Dr. Riddhi Gupta](https://smp.uq.edu.au/profile/16165/riddhi-gupta) and [Associate Professor Sally Shrapnel](https://about.uq.edu.au/experts/16630), our work focusses on clarifying regimes we expect quantum computing to be useful.

<div id="carouselExample" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    {% for img in page.carousels[0].images %}
      <div class="carousel-item {% if forloop.first %}active{% endif %}">
        <img src="{{ img.image }}" class="d-block w-100" alt="">
      </div>
    {% endfor %}
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
    <span class="carousel-control-prev-icon"></span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
    <span class="carousel-control-next-icon"></span>
  </button>
</div>

Our work explores potential applications for quantum computing in the nascent fault-tolerant regime. As examples, these potential applications include quantum simulations for molecular interactions in chemistry; preparing resource states for fault-tolerant quantum computing, and quantum machine learning.

Mitigating the impact of noise on quantum computers remains a persistent challenge. 

Our team works closely with industry partners to develop application-specific protocols in quantum noise characterization and control, quantum error mitigation and quantum error correction. 

We aim to bridge the gap between fundamental quantum theory and practical quantum technologies. Whether you are a student, researcher, or collaborator, we invite you to [explore our work](https://qatheorygroup.github.io/qcat/research) or [talk to us](riddhi.gupta@uq.edu.au).

We are currently hiring at all levels: students (Honours, Masters, Ph.D) and postdoctoral candidates. Our work is partly supported by [Queensland Digital Health Center](https://chsr.centre.uq.edu.au/research/queensland-digital-health-centre), the [Queensland Decarbonization Alliance](https://www.qubic.au/queensland-quantum-decarbonisation-alliance/) and [NCMAS](https://my.nci.org.au/mancini/ncmas/2026/).

<figure>
  <img src="https://raw.githubusercontent.com/QATheoryGroup/qcat/main/images/logos/UQ-300x300.png" style="width: 130px">
  <img src="https://raw.githubusercontent.com/QATheoryGroup/qcat/main/images/logos/QUBIC-Logo.svg" style="width: 130px">
</figure>
