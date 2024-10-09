---
layout: page
title: Multi-Vehicle Motion Planning for Relational Maneuvering
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
    Fixed Bearing Angle Formation Maneuvering (FBFM), where the follower maintains fixed distance and fixed bearing angle from the leader.
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-5 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/flex_form_web_4.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            The follower adjusts to the leader's maneuvers by either expanding its path or cutting inside the leader's trajectory when needed.
        </div>
    </div>
    <div class="col-sm-7 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/flex_form_web_3.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Validation of guidance approach on fixed wing UAV, for arbitararily moving target.
        </div>
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
    The FBFM scheme enables the follower to adapt to the leader's maneuvers, ensuring it maintains a tactical advantage by consistently staying behind the leader.
</div>

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;">Leader-Follower Ring Formation Control</span>

In this approach, the followers organize themselves along a virtual ring around the leader, adjusting their positions based on the leader's movement. This method allows the followers to adapt to various maneuvers of the leader, whether moving in a straight line or executing complex turns, while maintaining safe distances and formation stability. The flexibility of this control system makes it particularly suited for dynamic environments and tactical operations, ensuring that the formation remains robust despite changes in movement or external disturbances.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/eng_form.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/engagement_geom.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
    A virtual ring behind the leader represents the allowable positions for the follower to maintain formation.
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/ringform_stline.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Leader moving in straight line. The followers settle at different positions on the ring based on their initial conditions.
        </div>
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/ringform_loit.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Leader executing loiter maneuver. The followers starting from different initial positions all converge to the same point on the virtual ring, which corresponds to the minimum speed required to maintain the formation.
        </div>
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
    The follower converges to a point on the virtual ring to maintain formation. This simulation results demonstrate the flexibility provided by approach to the follower in maintaining formation, adapting to the leader's maneuvers.
</div>

## Related Publications

<div class="publications">
  {% bibliography -f papers -q @*[key=new_3]* %}
  {% bibliography -f papers -q @*[key=new_1]* %}
  {% bibliography -f papers -q @*[key=10.2514/1.G007057]* %}
  {% bibliography -f papers -q @*[key=10.2514/6.2022-2217]* %}
</div>
