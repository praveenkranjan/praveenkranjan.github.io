---
layout: page
title: <h5>Multi-Vehicle Motion Planning for Relational Maneuvering</h5>
description: #
img: assets/img/flex_form/flex_form_web_1.gif
importance: 1
category: Relational Maneuvering Guidance and Control
---

In the field of autonomous systems, multi-vehicle coordination is crucial for achieving complex missions involving UAVs. My research focuses on developing flexible and safe motion planning strategies for relational maneuvering, where multiple UAVs operate in coordination to maintain specific formations and adapt to dynamic mission requirements. By integrating safety constraints with flexible control mechanisms, I aim to enhance UAV performance in tasks such as target tracking, formation flying, and area coverage. These approaches allow UAVs to navigate safely while responding to unpredictable changes in the environment, ensuring reliable and robust operations in real-world scenarios.

## Flexible Leader-Follower formation control

Inspired by the behavior of human pilots we present a novel formation strategy for a leader-follower unmanned aerial vehicle (UAV) system where the formation geometry is not restricted to remain fixed as the vehicles maneuver. This means that the position and orientation of the follower UAV in relation to the leader UAV can change while adhering to certain constraints. Our strategy aims to maintain a desired fixed relative distance between the follower and leader UAVs, allowing for variations in their orientation. This flexibility in orientation helps reduce control effort for the follower UAV and offers tactical advantages. We term this approach as a "flexible relational maneuvering scheme" since the follower UAV is not constrained to a predetermined set of feasible positions, as is typical in close-proximity two-ship formations in air-to-air combat. Our approach seeks to replicate the behavior of human pilots in UAVs by implementing anticipatory maneuvers when the leader UAV executes aggressive turns.

<div class="row justify-content-sm-center">
    {% include figure.liquid path="assets/img/flex_form/flex_form_web_1.gif" title="example image" class="img-fluid rounded z-depth-1" style="max-width: auto; height: 1px;" %}
    <div class="caption">
         Schematic of Leader follower engagement geometry.
    </div>
</div>
<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/flex_form_web_4.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    FBFM  
</div>
## Energy-efficient Ring Formation Control
## Related Publications
<div class="publications">
  {% bibliography -f papers -q @*[key=new_2]* %}
  {% bibliography -f papers -q @*[key=new_2]* %}
</div>
