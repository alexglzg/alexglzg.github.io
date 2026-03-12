---
layout: page
title: Fast Motion Planning in Highly Structured Environments
description: Exploiting environment structure to develop efficient motion planners.
img: assets/img/projects/arena.jpg
importance: 1
category: research
---

For industries where robots operate in structured environments, such as factory floors, warehouses, terminals, hospitals, smart farms, and green houses, conventional motion planners may be slow or degrade with the map scale or application requirements. For non-holonomic robots, for instance, grid-based planners scale with the map size or resolution, and have an increased complexity to satisfy the kinematic constraints. However, these structured environments exhibit geometric patterns which can be exploited to offload the motion planner complexity. This project investigates how to create structure abstractions, and use them to develop efficient motion planners.

<div class="embed-responsive embed-responsive-16by9 mt-3">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/zJpmJpMFQuI" allowfullscreen></iframe>
</div>

## Related Publications

{% bibliography --query @*[project=arena] %}