---
layout: page
title: <h4>Multi-Vehicle Motion Planning for Relational Maneuvering</h4>
description: ""
img: assets/img/flex_form/flex_form_web_1.gif
importance: 1
category: Relational Maneuvering Guidance and Control
---

In the field of autonomous systems, multi-vehicle coordination is crucial for achieving complex missions involving UAVs. My research focuses on developing flexible and safe motion planning strategies for relational maneuvering, where multiple UAVs operate in coordination to maintain specific formations and adapt to dynamic mission requirements. By integrating safety constraints with flexible control mechanisms, I aim to enhance UAV performance in tasks such as target tracking, formation flying, and area coverage. These approaches allow UAVs to navigate safely while responding to unpredictable changes in the environment, ensuring reliable and robust operations in real-world scenarios.

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;">Flexible Leader-Follower Formation Control</span>

Inspired by the behavior of human pilots, we present a novel formation strategy for a leader-follower unmanned aerial vehicle (UAV) system where the formation geometry is not restricted to remain fixed as the vehicles maneuver. This means that the position and orientation of the follower UAV in relation to the leader UAV can change while adhering to certain constraints. Our strategy aims to maintain a desired fixed relative distance between the follower and leader UAVs, allowing for variations in their orientation. This flexibility in orientation helps reduce control effort for the follower UAV and offers tactical advantages. We term this approach a "flexible relational maneuvering scheme" since the follower UAV is not constrained to a predetermined set of feasible positions, as is typical in close-proximity two-ship formations in air-to-air combat. Our approach seeks to replicate the behavior of human pilots in UAVs by implementing anticipatory maneuvers when the leader UAV executes aggressive turns.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/flexible_form.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
    Fixed Bearing Angle Formation Maneuvering (FBFM)
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/flex_form_web_4.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
    FBFM Follower Behavior
</div>

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;">Energy-Efficient Ring Formation Control</span>

This paper focuses on developing an energy-efficient control algorithm for a type of leader-follower aircraft formation, namely, ring formation, where the follower seeks to track a virtual circle, also called a ring, whose center is behind the leader along the leader's heading direction. Enabling this type of ring formation allows the follower to maintain a certain geometric configuration with respect to the leader, but not a rigid structure that is often hard for the follower to maintain in, e.g., turning maneuvers. Meanwhile, the flexibility in a ring formation lies in the fact that the follower can stay on any point on the ring, thus helping save thrust-related energy consumption and addressing inherent physical constraints. Towards this objective, we develop a new controller using the backstepping technique and use nonlinear dynamic programming to address the control input constraints. First, we show that the minimum speed point on the ring can yield the lowest energy consumption. We then provide a specific control design based on backstepping for the follower to track the minimum speed point on the ring. To address the physical input constraints, we propose to use nonlinear dynamic programming to optimize the control inputs subject to control saturation. Finally, we present simulation results to demonstrate the effectiveness of the proposed approach in saving energy and addressing control input constraints.

<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/eng_form.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/engagement_geom.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
    Fixed Bearing Angle Formation Maneuvering (FBFM)
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/engagement_geom.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
    FBFM Follower Behavior
</div>

## Related Publications

<div class="publications">
  {% bibliography -f papers -q @*[key=new_3]* %}
  {% bibliography -f papers -q @*[key=new_1]* %}
  {% bibliography -f papers -q @*[key=10.2514/1.G007057]* %}
  {% bibliography -f papers -q @*[key=10.2514/6.2022-2217]* %}
</div>
