---
layout: lab
title: "Research"
permalink: /research/
description: "Research on performance, system design, and learning across communication networks, edge computing and AI, and quantum information."
---

We study how information and decisions shape one another in classical and quantum systems under constraints and uncertainty. Three questions guide our work.<span id="open-questions"></span>

<section class="research-theme" markdown="1">

## Performance Limits and Trade-offs
{: #limits}

*What can systems achieve?*<span id="dt-credibility"></span>

<figure class="research-theme__figure">
  <img src="{{ '/assets/images/research-limits.svg' | relative_url }}?v={{ site.time | date: '%Y%m%d%H%M%S' }}" width="480" height="260" loading="lazy" alt="Conceptual achievable performance region, feasible operating points, and an upper bound as the resource budget changes.">
</figure>

We study how physical constraints, limited resources, and uncertainty shape performance. Our work examines trade-offs among reliability, security, latency, accuracy, and energy use, and develops performance bounds and algorithmic guarantees under explicit assumptions.

</section>

<section class="research-theme" markdown="1">

## System Design and Resource Management
{: #networks}

*How should resources be used?*<span id="dt-synchronization"></span><span id="dt-resources"></span>

<figure class="research-theme__figure">
  <img src="{{ '/assets/images/research-resources.svg' | relative_url }}?v={{ site.time | date: '%Y%m%d%H%M%S' }}" width="480" height="260" loading="lazy" alt="Workload placement across devices, edge, and shared computing resources, with bandwidth, compute, and energy allocation.">
</figure>

We design systems that coordinate communication, computation, and sensing. Topics include resource allocation, task offloading, workload placement, and carbon-aware operation across devices, edge servers, and networked infrastructure.

</section>

<section class="research-theme" markdown="1">

## Learning and Decision-Making
{: #decisions}

*How should systems learn and act?*<span id="dt-decisions"></span>

<figure class="research-theme__figure">
  <img src="{{ '/assets/images/research-decisions.svg' | relative_url }}?v={{ site.time | date: '%Y%m%d%H%M%S' }}" width="480" height="260" loading="lazy" alt="An observe, decide, and act loop with a selected action and feedback updates under limited or delayed information.">
</figure>

We develop learning and optimization methods for decisions with incomplete information and changing environments. Bandit methods, reinforcement learning, and game theory help systems adapt to feedback and coordinate their actions. We also explore these methods for public-sector decision support.

</section>

## Research Domains
{: #domains}

### Communication Networks

Secure and efficient communication in terrestrial, UAV, and satellite networks, including symbiotic radio and integrated sensing and communication.

### Edge Computing and Physical AI
{: #edge-ai}

<span id="digital-twins"></span>AI for resource management and efficient systems for AI inference. Topics include robot-policy execution, world models, and model construction for digital twins.

### Quantum Information Systems

Quantum algorithms, communication, sensing, and learning under noise and resource constraints, including the quantum switch and quantum key distribution.

## Ongoing Research
{: #projects}

<div class="ongoing-projects">
  <article class="ongoing-project" id="dt-models">
    <h3><a href="{{ '/research/video2urdf/' | relative_url }}">Video2URDF</a></h3>
    <p class="ongoing-project__member">Led by <a href="{{ '/people/#member-joshua-austin-kim' | relative_url }}">Joshua Austin Kim</a></p>
    <p>Constructing articulated models from video for robotics simulation and checking their motion against observations.</p>
  </article>
  <article class="ongoing-project">
    <h3>AI Pilots for Aircraft Pursuit</h3>
    <p class="ongoing-project__member">Led by <a href="{{ '/people/#member-joshua-austin-kim' | relative_url }}">Joshua Austin Kim</a></p>
    <p>Reinforcement learning for autonomous agents in simulated aircraft-pursuit tasks.</p>
  </article>
  <article class="ongoing-project">
    <h3><a href="{{ '/research/edge-inference/' | relative_url }}">World Models and Edge Inference for Physical AI</a></h3>
    <p class="ongoing-project__member">Led by <a href="{{ '/people/#member-kim-jh' | relative_url }}">Jungha Kim</a></p>
    <p>World models and efficient robot-policy execution on edge devices.</p>
  </article>
</div>

Interested in these or related questions? Please visit our [Contact]({{ '/contact/' | relative_url }}) page.
