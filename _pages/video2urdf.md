---
layout: lab
title: "Video2URDF"
permalink: /research/video2urdf/
description: "Joshua Austin Kim's Video2URDF: Top Finalist in the Indie Developer Track of the Meta Global AI Developer Hackathon 2026."
---

**From phone video to articulated models for robotics simulation**

Developed by [Joshua Austin Kim]({{ '/people/#member-joshua-austin-kim' | relative_url }}), Video2URDF was selected as a **Top Finalist in the Indie Developer Track** and awarded **US$25,000** at the Meta Global AI Developer Hackathon on November 9, 2026. The organizers reported 20,000 participants and 5,367 submitted projects across both tracks; Video2URDF was one of five finalists selected in its track.

[Project and interactive demos](https://sunghyunc.github.io/video2urdf/) · [Code](https://github.com/SungHyunC/video2urdf) · [Final presentation and judges' feedback](https://vimeo.com/1245287583) · [Award announcement](https://vimeo.com/1245287584)

## Watch the demo

<figure class="project-video">
  <video controls playsinline preload="metadata" width="960" height="540" aria-label="Video2URDF project demonstration">
    <source src="https://sunghyunc.github.io/video2urdf/demo.mp4" type="video/mp4">
    <a href="https://sunghyunc.github.io/video2urdf/demo.mp4">Watch the Video2URDF demo</a>.
  </video>
  <figcaption>The developer's 3-minute demonstration: object video, reconstruction, simulation replay, and robot interaction. <a href="https://youtu.be/aK_csSIU24c">Watch on YouTube</a> · <a href="https://sunghyunc.github.io/video2urdf/demo.mp4">Open video</a>.</figcaption>
</figure>

## What it does

Robots need models of how objects move: where a laptop lid hinges, how far a drawer slides, or how a lamp's joints connect. Building these simulation assets by hand takes time.

Video2URDF estimates an object's parts, geometry, and joint motion from a short video and exports **URDF and MJCF**, formats used in robotics simulation. A Muse Spark agent prompts SAM 3.1 to segment and track parts, chooses fitting tools, and inspects the result. A MuJoCo replay is compared with the source video so that discrepancies can trigger another round of segmentation, tracking, or joint fitting.

## Why it matters

The central contribution is a **feedback loop between reconstruction and verification**. A proposed model must explain observed motion. This creates a practical route from everyday recordings to reusable simulation assets and test cases for Physical AI.

The project includes comparisons with direct model prompting, benchmark evaluations, and documented failure cases. It also distinguishes properties estimated from visual observations from those supplied by model priors. Replay agreement checks consistency with the footage; it does not establish every physical parameter independently. The robot-manipulation demonstrations run in simulation.

## What the judges highlighted

In the recorded final discussion (**09:20–11:44**), judges highlighted three strengths:

- **Combining models for a new task:** reasoning and segmentation models were connected to build articulated assets for embodied AI.
- **Useful data for the community:** the approach could make it easier to create robot-learning data and new benchmarks.
- **Checking motion against evidence:** using SAM and video to validate the joints made the reconstruction testable.

They also raised a critical question: **which properties are measured from the video, and which are recalled or inferred from the model's prior knowledge?** This distinction matters when a plausible reconstruction will be used to train or evaluate a robot.

The presentation runs from approximately **06:13 to 09:09** in the [closing show](https://vimeo.com/1245287583). The Indie Developer Track results are announced at approximately **02:23–02:51** in the [awards video](https://vimeo.com/1245287584).

[Technical approach](https://github.com/SungHyunC/video2urdf/blob/master/docs/HOW_IT_WORKS.md) · [Evaluation and limitations](https://github.com/SungHyunC/video2urdf/blob/master/docs/RESULTS.md) · [About the hackathon](https://dev.meta.ai/events/global-hackathon)
