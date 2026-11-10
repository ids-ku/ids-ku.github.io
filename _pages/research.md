---
layout: lab
title: "Research"
permalink: /research/
description: "Performance, resource management, and decisions across digital twins, Physical AI, networked systems, and quantum information."
---

Our research spans **communication networks**, **edge computing and AI systems**, and **quantum information systems**. We study how physical constraints, limited resources, and uncertainty affect what systems can achieve and how they should be designed and operated. Mathematical modeling and analysis guide our algorithms; simulation, measurement, and system implementation help us evaluate them.

Across these domains, our work is organized around three connected questions about performance, system design, and decision-making. [Digital twins]({{ '/research/#digital-twins' | relative_url }}) provide a concrete research direction connecting observations, models, and decisions.

<section class="research-theme" markdown="1">

## Performance Limits and Trade-offs
{: #limits}

*What is achievable, and what performance can be guaranteed?*

<figure class="research-theme__figure">
  <img src="{{ '/assets/images/research-limits.svg' | relative_url }}?v={{ site.time | date: '%Y%m%d%H%M%S' }}" width="480" height="260" loading="lazy" alt="Conceptual achievable performance region, feasible operating points, and an upper bound as the resource budget changes.">
</figure>

We characterize performance limits and trade-offs in communication, computation, and sensing. Topics include reliability and security, latency and inference accuracy, throughput and power consumption, and the cost of acquiring information. Where the model permits, we derive analytical bounds and algorithmic performance guarantees. For [digital twins]({{ '/research/#dt-credibility' | relative_url }}), we aim to understand how model error, observation delay, and resource budgets affect prediction and decision quality.

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

In **edge computing and AI systems**, we study task offloading, capacity planning, workload placement, and runtime resource management. [Air-ground collaborative offloading]({{ '/publications/#air-ground-offloading' | relative_url }}) connects mobile computing resources with communication networks. This direction also extends to carbon-aware edge computing, including how workloads should be placed and scheduled across devices while accounting for performance, energy use, and carbon emissions. Our [digital twin questions]({{ '/research/#dt-resources' | relative_url }}) connect these resource decisions to model fidelity, update frequency, and execution time.

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
- **Edge Computing for AI:** communication and computing systems that support efficient AI inference. Examples include adapting video transmission to balance inference accuracy and latency, and tuning device resources to meet throughput and power targets in CORAL. Current work targets efficient robot policy execution for **Physical AI** through runtime and GPU kernel optimization under memory, power, and response-time constraints.

We also study **quantum learning and decision algorithms**. Our [quantum bandit research]({{ '/publications/#quantum-bandit' | relative_url }}) examines amplitude amplification for exploration in adversarial bandit settings.

We are exploring **AI for Public-Sector Decision Support** as an emerging direction in public-sector AI transformation (AX). Our interests include prediction, resource allocation, scheduling, and replanning under uncertainty and operational constraints, with human oversight.

We examine both the benefit of new information and the communication, computation, and observation effort required to acquire and use it. In [digital twins]({{ '/research/#dt-decisions' | relative_url }}), this leads to a feedback loop: decisions affect system behavior and the observations available for subsequent learning.

</section>

## Ongoing Research
{: #projects}

<div class="ongoing-projects">
  <article class="ongoing-project">
    <h3><a href="{{ '/research/video2urdf/' | relative_url }}">Video2URDF: Visual Reconstruction for Robotics Simulation</a></h3>
    <p class="ongoing-project__member">Led by <a href="{{ '/people/#member-joshua-austin-kim' | relative_url }}">Joshua Austin Kim</a></p>
    <p>Reconstructing articulated objects from phone video, with an agent that connects segmentation, joint estimation, and simulation replay. Selected as a Top Finalist in the Indie Developer Track of the Meta Global AI Developer Hackathon 2026. <a href="{{ '/research/video2urdf/' | relative_url }}">Project and judges' feedback</a>.</p>
  </article>
  <article class="ongoing-project">
    <h3>AI Pilots for Aircraft Pursuit</h3>
    <p class="ongoing-project__member">Led by <a href="{{ '/people/#member-joshua-austin-kim' | relative_url }}">Joshua Austin Kim</a></p>
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

## Digital Twins: From Observations to Decisions
{: #digital-twins}

<span id="open-questions"></span>

We are developing a research direction in **digital twins for Physical AI and networked systems**. Five questions connect model construction, observation, prediction, resource management, and action. They apply to robotics and computing infrastructure and draw on our three research themes.

### 1. Models from Observations
{: #dt-models}

*How can limited observations produce simulation models whose structure and behavior can be checked against evidence?*

**Current work:** [Video2URDF]({{ '/research/video2urdf/' | relative_url }}) addresses articulated model construction and motion replay checks. Further questions concern identifying dynamic parameters and validating models against independent measurements.

### 2. State Estimation and Synchronization
{: #dt-synchronization}

*What should be sensed and updated, and when, to keep a twin useful as the physical system changes?*

**Open direction:** estimate hidden states and update states and parameters despite noise, delay, or missing data. The update frequency should match the decision being supported.

### 3. Prediction and Model Credibility
{: #dt-credibility}

*When can a twin's predictions be trusted, and how can we detect when the model needs to change?*

**Open direction:** quantify uncertainty, detect model drift, and validate predictions on held-out operating conditions or independent measurements. Agreement with a recorded video is one part of this evaluation.

### 4. Efficient Execution and Resource Management
{: #dt-resources}

*How should sensing, communication, inference, and simulation share limited computing, memory, and energy budgets?*

**Related foundation:** [Jungha's edge inference research]({{ '/people/#member-kim-jh' | relative_url }}) and [CORAL]({{ '/publications/#coral' | relative_url }}) concern efficient execution. Further questions address model fidelity, update rates, computation placement, and end-to-end latency, energy use, and carbon emissions.

### 5. Decisions with Imperfect Models
{: #dt-decisions}

*How should a system act when its twin is incomplete, delayed, or uncertain?*

**Open direction:** evaluate decisions under model error and operational constraints, determine when more observations are worthwhile, and design fallback policies. Actions also affect the information available for subsequent learning.

Interoperable interfaces, traceable data and model versions, and secure updates are shared design questions across this direction.

Our broader research also asks when quantum resources outperform classical baselines and how prediction and optimization can support public-sector decisions with human oversight.

Background: [NIST on model credibility](https://www.nist.gov/publications/credibility-consideration-digital-twins-manufacturing) · [NIST on digital twin integration](https://www.nist.gov/programs-projects/digital-twins-advanced-manufacturing) · [Definition and validation scope](https://www.gov.uk/government/publications/digital-twin-definition/digital-twin-official).

Interested in these or related questions? Please visit our [Contact]({{ '/contact/' | relative_url }}) page.
