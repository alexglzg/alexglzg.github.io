---
layout: page
title: Robust Control of Autonomous Surface Vessels
description: Adaptive sliding mode control for autonomous surface vessels under environmental disturbances
img: assets/img/publication_preview/AITSMC.gif
importance: 1
category: research
---

Autonomous Surface Vehicles (ASVs) operate in complex environments subject to external disturbances from wind, waves, and currents. Furthermore, mathematical model discrepancies to the real system, such as unmodeled dynamics or parameter inaccuracies, induce uncertainty. Thus, robust control techniques are required to overcome disturbances and uncertainty, increasing safety, efficiency, and accuracy.

{% include video.liquid path="https://www.youtube.com/embed/G_6aAegapG8" class="img-fluid rounded z-depth-1" %}

<div class="row mt-3">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/publication_preview/AITSMC.gif" title="ASV trajectory tracking" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

## Related Publications

{% bibliography --query @*[keywords=robust_asv] %}
