---
layout: lab
title: "Research"
permalink: /research/
description: "Communication networks, edge computing and AI systems, and quantum information systems: performance analysis, resource management, and learning and decision algorithms."
---

Our research spans **communication networks**, **edge computing and AI systems**, and **quantum information systems**. We study how physical constraints, limited resources, and uncertainty affect what systems can achieve and how they should be designed and operated. Mathematical modeling and analysis guide our algorithms; simulation, measurement, and system implementation help us evaluate them.

Across these domains, our work is organized around three connected questions about performance, system design, and decision-making.

<section class="research-theme" markdown="1">

## Performance Limits and Trade-offs
{: #limits}

*What is achievable, and what performance can be guaranteed?*

<figure class="research-theme__figure">
  <img src="{{ '/assets/images/research-limits.svg' | relative_url }}?v={{ site.time | date: '%Y%m%d%H%M%S' }}" width="480" height="260" loading="lazy" alt="Conceptual achievable performance region, feasible operating points, and an upper bound as the resource budget changes.">
</figure>

We characterize performance limits and trade-offs in communication, computation, and sensing. Topics include reliability and security, latency and inference accuracy, throughput and power consumption, and the cost of acquiring information. Where the model permits, we derive analytical bounds and algorithmic performance guarantees.

In wireless networks, this includes the effects of interference, mobility, and imperfect channel information on secure and reliable communication. In edge AI systems, we examine how networking and hardware settings shape inference performance and resource use, as in our [deep video analytics]({{ '/publications/#edge-video-analytics' | relative_url }}) and [CORAL]({{ '/publications/#coral' | relative_url }}) studies.

Our quantum information research includes quantum algorithms, the quantum switch, quantum key distribution (QKD), and quantum sensing. We investigate the roles of noise, measurement, and available quantum resources in the performance of these systems.

</section>

<section class="research-theme" markdown="1">

## System Design and Resource Management
{: #networks}

*How should systems be configured and resources shared?*

<figure class="research-theme__figure">
  <img src="{{ '/assets/images/research-resources.svg' | relative_url }}?v={{ site.time | date: '%Y%m%d%H%M%S' }}" width="480" height="260" loading="lazy" alt="Workload placement across devices, edge, and shared computing resources, with bandwidth, compute, and energy allocation.">
</figure>

In **communication networks**, we study spectrum sharing, interference management, symbiotic radio and backscatter, integrated sensing and communication (ISAC), and UAV and satellite communications. Our work on [secure symbiotic radio]({{ '/publications/#secure-symbiotic-radio' | relative_url }}), for example, connects passive localization with beamforming design. Our [multi-UAV data collection]({{ '/publications/#multi-uav-data-collection' | relative_url }}) research addresses covertness, reliability, and fairness under imperfect channel information.

In **edge computing and AI systems**, we study task offloading, capacity planning, workload placement, and runtime resource management. [Air-ground collaborative offloading]({{ '/publications/#air-ground-offloading' | relative_url }}) connects mobile computing resources with communication networks. This direction also extends to carbon-aware edge computing, including how workloads should be placed and scheduled across devices while accounting for performance, energy use, and carbon emissions.

</section>

<section class="research-theme" markdown="1">

## Learning and Decision-Making
{: #decisions}

*How should systems act when their environment is not fully known?*

<figure class="research-theme__figure">
  <img src="{{ '/assets/images/research-decisions.svg' | relative_url }}?v={{ site.time | date: '%Y%m%d%H%M%S' }}" width="480" height="260" loading="lazy" alt="An observe, decide, and act loop with a selected action and feedback updates under limited or delayed information.">
</figure>

We develop learning and optimization methods for sequential and distributed decisions. Bandit methods, reinforcement learning, game theory, and optimization help us address partial or delayed feedback, changing environments, and coordination among network participants. We also study algorithmic guarantees, including regret bounds that compare cumulative performance with a specified benchmark under explicit assumptions.

Our edge research connects two complementary directions:

- **AI for Edge Computing:** learning-based resource management, offloading decisions, and computing capacity planning, including [multi-agent reinforcement learning for vehicular fog computing]({{ '/publications/#marl-capacity-planning' | relative_url }}).
- **Edge Computing for AI:** communication and computing systems that support efficient AI inference. Examples include adapting video transmission to balance inference accuracy and latency, and tuning device resources to meet throughput and power targets in CORAL. Current work also targets low-latency robot-policy execution for Physical AI.

We examine both the benefit of new information and the communication, computation, and observation effort required to acquire and use it.

</section>

## Ongoing Research
{: #projects}

<div class="ongoing-projects">
  <article class="ongoing-project">
    <h3>AI Pilots for Aircraft Pursuit</h3>
    <p class="ongoing-project__member">Led by <a href="{{ '/people/#member-kim-seonghyeon' | relative_url }}">Seonghyeon Kim</a></p>
    <p>Reinforcement learning for AI pilot agents in simulated aircraft-pursuit tasks.</p>
  </article>
  <article class="ongoing-project">
    <h3>World Models and Edge Inference for Physical AI</h3>
    <p class="ongoing-project__member">Led by <a href="{{ '/people/#member-kim-jh' | relative_url }}">Jungha Kim</a></p>
    <p>Research on omnimodal world models for Physical AI, alongside efficient robot-policy execution on edge devices.</p>
    <p>A systems study targets dual-camera policy execution on Jetson Orin Nano 8GB, with SO-ARM101 as the evaluation platform. It aims to reduce sensor-to-command latency while verifying numerical agreement and input freshness. Evaluation against PyTorch and TensorRT-based baselines will assess robot responsiveness, the contribution of runtime and GPU kernel optimizations, and power-mode effects.</p>
  </article>
</div>

---

[Explore our publications]({{ '/publications/' | relative_url }})
