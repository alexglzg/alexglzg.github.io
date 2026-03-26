---
layout: page
title: Safe Distributed Motion Planning
description: Distributed motion planning for multi-agent systems with safety guarantees.
img: assets/img/projects/maglev.png
importance: 2
category: research
---

Multi-agent systems are useful for diverse industries and domains, as they can extend the capability of single-agent systems. To develop autonomous multi-agent systems, motion planning remains a challenge. Centralized solutions can solve for safe and even optimal motions for multiple agents, but they suffer as the number of agents grow, becoming intractable. Distributed solutions can help to overcome this issue, decoupling the complexity of the problem. Nevertheless, it is important to not sacrifice safety of the system for the sake of efficiency. How can we guarantee safe performance, while still achieving a certain level of performance?

<div class="embed-responsive embed-responsive-16by9 mt-3">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/5H8QRz0ndy4" allowfullscreen></iframe>
</div>

## Related Publications

{% bibliography --query @*[project=admm] %}