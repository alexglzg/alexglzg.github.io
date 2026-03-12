---
layout: page
title: Safe Motion Planning and Control
description: Optimization-based planning and control with safety guarantees.
img: assets/img/projects/safe_asv.png
importance: 1
category: research
---

ASVs operating in inland waterways must deal with narrow environments where maneuverability is essential and complex. Model predictive control (MPC) has been widely used for motion planning and control, but it does not provide any formal safety guarantees and the complexity may explode with the number of obstacles or complex constraints. Control barrier functions (CBFs) have been proposed to formally guarantee safety. Thus, designing hybrid frameworks combining MPC and CBFs is a promising way to achieve safety, both against enviornmental disturbances and throguh narrow channels.

<div class="embed-responsive embed-responsive-16by9 mt-3">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/ogbfAdaSyIc" allowfullscreen></iframe>
</div>

## Related Publications

{% bibliography --query @*[project=safe_asv] %}