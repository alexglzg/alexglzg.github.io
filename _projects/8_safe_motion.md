---
layout: page
title: Safe Motion Planning and Control
description: Optimization-based planning and control with safety guarantees.
img: assets/img/projects/safe_asv.png
importance: 1
category: safe & fast motion planning
---

Different systems operate in environments where safety-critical solutions are required. That is the case for instance of ASVs operating in inland waterways, or AMRs in unstructured spaces, as they must deal with narrow environments where maneuverability is essential and complex. Model predictive control (MPC) has been widely used for motion planning and control, as it handles constraints while predicting the system's behavior. However, safety is typically enforced through distance constraints that only act once the predicted trajectory approaches an obstacle, and the complexity may explode with the number of obstacles or complex constraints. Control barrier functions (CBFs) guarantee safety by keeping the system within a safe set, but on their own they lack prediction. This project explores different ways of combining MPC and CBFs for safe motion planning and control, either using CBFs as a safety filter on the MPC solution, or as discrete-time CBF constraints within the MPC.

<div class="embed-responsive embed-responsive-16by9 mt-3">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/ogbfAdaSyIc" allowfullscreen></iframe>
</div>

<div class="embed-responsive embed-responsive-16by9 mt-3">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/MmQ3oSoCj54" allowfullscreen></iframe>
</div>

## Related Publications

{% bibliography --query @*[projects~=safe_motion] %}
