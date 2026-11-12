---
layout: lab
title: "Research"
permalink: /research/
description: "Research on performance, system design, and learning across communication networks, edge computing and AI, and quantum information."
---

We study how information and decisions shape one another in classical and quantum systems under constraints and uncertainty.<span id="open-questions"></span>

<section class="research-part" aria-labelledby="research-questions" markdown="1">

<header class="research-part__heading">
  <h2 id="research-questions"><span class="research-part__number" aria-hidden="true">01</span> Research Questions</h2>
</header>

<div class="research-subsections" markdown="1">

<section class="research-subsection research-theme" markdown="1">

### Performance Limits and Trade-offs
{: #limits}

*What can systems achieve?*<span id="dt-credibility"></span>

<figure class="research-theme__figure">
  <img src="{{ '/assets/images/research-limits.svg' | relative_url }}?v={{ site.time | date: '%Y%m%d%H%M%S' }}" width="480" height="260" loading="lazy" alt="Conceptual achievable performance region, feasible operating points, and an upper bound as the resource budget changes.">
</figure>

We study how physical constraints, limited resources, and uncertainty shape performance. Our work examines trade-offs among reliability, security, latency, accuracy, and energy use, and develops performance bounds and algorithmic guarantees under explicit assumptions.

</section>

<section class="research-subsection research-theme" markdown="1">

### System Design and Resource Management
{: #networks}

*How should systems be designed and resources allocated?*<span id="dt-synchronization"></span><span id="dt-resources"></span>

<figure class="research-theme__figure">
  <img src="{{ '/assets/images/research-resources.svg' | relative_url }}?v={{ site.time | date: '%Y%m%d%H%M%S' }}" width="480" height="260" loading="lazy" alt="Workload placement across devices, edge, and shared computing resources, with bandwidth, compute, and energy allocation.">
</figure>

We design systems that coordinate communication, computation, and sensing. Topics include resource allocation, task offloading, workload placement, and carbon-aware operation across devices, edge servers, and networked infrastructure.

</section>

<section class="research-subsection research-theme" markdown="1">

### Learning and Decision-Making
{: #decisions}

*How should systems learn and act under uncertainty?*<span id="dt-decisions"></span>

<figure class="research-theme__figure">
  <img src="{{ '/assets/images/research-decisions.svg' | relative_url }}?v={{ site.time | date: '%Y%m%d%H%M%S' }}" width="480" height="260" loading="lazy" alt="An observe, decide, and act loop with a selected action and feedback updates under limited or delayed information.">
</figure>

We develop learning and optimization methods for decision-making with incomplete information in changing environments. Bandit methods, reinforcement learning, and game theory help systems adapt to feedback and coordinate their actions. Applications of interest include public-sector decision support.

</section>

</div>

</section>

<section class="research-part" aria-labelledby="domains" markdown="1">

<header class="research-part__heading">
  <h2 id="domains"><span class="research-part__number" aria-hidden="true">02</span> Research Domains</h2>
</header>

<div class="research-subsections" markdown="1">

<section class="research-subsection research-domain" markdown="1">

### Communication Networks

We design communication systems that balance security, reliability, fairness, and resource use under mobility and imperfect information. Our [ISAC-enhanced symbiotic radio]({{ '/publications/#secure-symbiotic-radio' | relative_url }}) research connects sensing with beamforming for secure communication, while [multi-UAV data collection]({{ '/publications/#multi-uav-data-collection' | relative_url }}) addresses covertness and fairness. Related settings include terrestrial, UAV, and satellite networks.

</section>

<section class="research-subsection research-domain" markdown="1">

### Edge Computing and Physical AI
{: #edge-ai}

We connect two complementary directions:

- **AI for Edge Computing:** learning-based decisions for offloading, capacity planning, and resource allocation. Our [multi-agent reinforcement learning research]({{ '/publications/#marl-capacity-planning' | relative_url }}) addresses vehicular fog computing. We also explore carbon-aware workload placement and scheduling.
- **Edge Computing for AI:** communication and computing systems for efficient inference. [CORAL]({{ '/publications/#coral' | relative_url }}) adapts hardware configurations to meet inference throughput targets and power budgets, while [edge video analytics]({{ '/publications/#edge-video-analytics' | relative_url }}) examines accuracy–latency trade-offs. Current work extends to efficient robot-policy execution and world models.

<span id="digital-twins"></span>Within Physical AI, we study **model construction for digital twins**. [Video2URDF]({{ '/research/video2urdf/' | relative_url }}) builds articulated simulation models from video and checks their motion against recorded observations.

</section>

<section class="research-subsection research-domain" markdown="1">

### Quantum Information Systems

We study the performance limits and design of quantum communication, sensing, and algorithms under noise and resource constraints. In quantum communication, our interests include the quantum switch, which coherently controls channel order, and security in quantum key distribution (QKD). Our [quantum bandit research]({{ '/publications/#quantum-bandit' | relative_url }}) examines amplitude amplification for exploration in adversarial bandit settings, connecting quantum algorithms with sequential learning and decision-making.

</section>

</div>

</section>

<section class="research-part" aria-labelledby="projects" markdown="1">

<header class="research-part__heading">
  <h2 id="projects"><span class="research-part__number" aria-hidden="true">03</span> Ongoing Research</h2>
</header>

<div class="research-subsections ongoing-projects">
  <article class="research-subsection ongoing-project" id="dt-models">
    <h3><a href="{{ '/research/video2urdf/' | relative_url }}">Model Construction for Digital Twins (Video2URDF)</a></h3>
    <p class="ongoing-project__member">Led by <a href="{{ '/people/#member-joshua-austin-kim' | relative_url }}">Joshua Austin Kim</a></p>
    <p>Constructing articulated models from video for robotics simulation and checking their motion against observations.</p>
  </article>
  <article class="research-subsection ongoing-project">
    <h3>AI Pilots for Aircraft Pursuit</h3>
    <p class="ongoing-project__member">Led by <a href="{{ '/people/#member-joshua-austin-kim' | relative_url }}">Joshua Austin Kim</a></p>
    <p>Reinforcement learning for autonomous agents in simulated aircraft-pursuit tasks.</p>
  </article>
  <article class="research-subsection ongoing-project">
    <h3><a href="{{ '/research/edge-inference/' | relative_url }}">World Models and Edge Inference for Physical AI</a></h3>
    <p class="ongoing-project__member">Led by <a href="{{ '/people/#member-kim-jh' | relative_url }}">Jungha Kim</a></p>
    <p>Studying world models and optimizing robot-policy execution latency on edge devices.</p>
  </article>
</div>

</section>
