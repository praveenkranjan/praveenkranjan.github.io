---
layout: page
title: Safe Target Enclosing
description: a project with a background image and giscus comments
img: assets/img/3.jpg
importance: 2
category: Relational Maneuvering Guidance and Control
giscus_comments: true
---

We present a novel formation strategy for a leader-follower unmanned aerial vehicle (UAV) system, drawing inspiration from the behavior of human pilots. In our approach, the formation geometry is not restricted to remain fixed as the vehicles maneuver. This means that the position and orientation of the follower UAV in relation to the leader UAV can change while adhering to certain constraints. Our strategy aims to maintain a desired fixed relative distance between the follower and leader UAVs, allowing for variations in their orientation. This flexibility in orientation helps reduce control effort for the follower UAV and offers tactical advantages. We term this approach as a "flexible relational maneuvering scheme" since the follower UAV is not constrained to a predetermined set of feasible positions, as is typical in close-proximity two-ship formations in air-to-air combat. Our approach seeks to replicate the behavior of human pilots in UAVs by implementing anticipatory maneuvers when the leader UAV executes aggressive turns.

<div class="row justify-content-sm-center">
    <div class="col-sm-3 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/regionsofoper.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>    
</div>
<iframe width="540" height="420" src="https://www.youtube.com/embed/zmdImaB7bp0" title="Software-in-the-loop simulations with tuned autopilot" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<div class="caption">
    FBFM with different desired bearing angles. 
</div>
<div class ="row justify-content-sm-center">
    {% include figure.liquid loading="eager" path="assets/img/flex_form/flex_form_web_2.gif" title="example image" class="img-fluid rounded z-depth-1" %}
</div>
<div class="caption">
    FBFM Software in the Loop Simulation results. 
</div>
<div class ="row justify-content-sm-center">
    {% include figure.liquid loading="eager" path="assets/img/flex_form/flex_form_web_3.gif" title="example image" class="img-fluid rounded z-depth-1" %}
</div>
<div class="caption">
    FBFM Flight Experiments results. 
</div>
## Related Publications
<div class="publications">
  {% bibliography -f papers -q @*[key=new_2]* %}
  {% bibliography -f papers -q @*[key=new_2]* %}
</div>
