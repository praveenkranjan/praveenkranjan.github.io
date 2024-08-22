---
layout: page
title: Safe Target Enclosing
description: a project with a background image and giscus comments
img: assets/img/3.jpg
importance: 2
category: Relational Maneuvering Guidance and Control
giscus_comments: true
---

We present a novel formation strategy for a leader-follower unmanned aerial vehicle (UAV) system, drawing inspiration from the behavior of human pilots. In our approach, the formation geometry is not restricted to remain fixed as the vehicles maneuver. This means that the position and orientaower UAV in relation to the leader UAV can change while adhering to certain constraints. Our strategy aims to maintain a desired fixed relative distance between the follower and leader UAVs, allowing for variations in their orientation. This flexibility in orientation helps reduce control effort for the follower UAV and offers tactical advantages. We term this approach as a "flexible relational maneuvering scheme" since the follower UAV is not constrained to a predetermined set of feasible positions, as is typical in close-proximity two-ship formations in air-to-air combat. Our approach seeks to replicate the behavior of human pilots in UAVs by implementing anticipatory maneuvers when the leader UAV executes aggressive turns.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/regionsofoper_vid.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>    
</div>
<div class="caption">
    Safe Region for Pursuer movement while enclosing the Target. 
</div>
<div class="row justify-content-sm-center">
    <iframe width="720" height="540" align="center" src="https://www.youtube.com/embed/zmdImaB7bp0" title="Software-in-the-loop simulations with tuned autopilot" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
<div class="caption">
    Safe Target enclosing quadrotor Software-In-the-loop simulation results 
</div>
## Related Publications
<div class="publications">
  {% bibliography -f papers -q @*[key=new_2]* %}
  {% bibliography -f papers -q @*[key=doi:10.2514/6.2024-0124]* %}
</div>
