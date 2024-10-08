---
layout: page
title: <h4>Distributed Multi-agent Systems and Controls</h4>
description: ""
img: assets/img/safe_enc/self_org.gif
importance: 1
category: Relational Maneuvering Guidance and Control
---

In the field of autonomous systems, multi-vehicle coordination is crucial for achieving complex missions involving UAVs. My research focuses on developing flexible and safe motion planning strategies for relational maneuvering, where multiple UAVs operate in coordination to maintain specific formations and adapt to dynamic mission requirements. By integrating safety constraints with flexible control mechanisms, I aim to enhance UAV performance in tasks such as target tracking, formation flying, and area coverage. These approaches allow UAVs to navigate safely while responding to unpredictable changes in the environment, ensuring reliable and robust operations in real-world scenarios.

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;">Self-organising Multi-agent Target enclosing</span>

Inspired by the behavior of human pilots, we present a novel formation strategy for a leader-follower unmanned aerial vehicle (UAV) system where the formation geometry is not restricted to remain fixed as the vehicles maneuver. This means that the position and orientation of the follower UAV in relation to the leader UAV can change while adhering to certain constraints. Our strategy aims to maintain a desired fixed relative distance between the follower and leader UAVs, allowing for variations in their orientation. This flexibility in orientation helps reduce control effort for the follower UAV and offers tactical advantages. We term this approach a "flexible relational maneuvering scheme" since the follower UAV is not constrained to a predetermined set of feasible positions, as is typical in close-proximity two-ship formations in air-to-air combat. Our approach seeks to replicate the behavior of human pilots in UAVs by implementing anticipatory maneuvers when the leader UAV executes aggressive turns.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/self_org_f1.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/self_org_f2.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/self_org_f3.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/self_org.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
    Autonomous organization of multiple pursuers on the enclosing shape around the target
</div>

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;">Safe And Flexible Target-Enclosing</span>

In this work, we focuses on developing advanced guidance strategies for unmanned aerial vehicles (UAVs) to safely enclose moving targets in three-dimensional space. Our approach prioritizes both safety and flexibility, allowing UAVs to maintain optimal distance while adapting to dynamic environments. By leveraging nonholonomic constraints and innovative control techniques, we ensure collision avoidance and robust performance, even in challenging scenarios. This solution is designed to handle complex target maneuvers, offering reliable and resilient UAV operations in real-time applications.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/inertialengagement.png" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Pursuer-Target Engagement Geometry
        </div>
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/regionsofoper.png" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Safe region for pursuer motion offering mutliple stable enclosing trajectories around the target
        </div>
    </div>
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/safe_enc_sta_r3.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Stationary Target
        </div>
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/safe_enc_stline_r3.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Target Moving in straight line
        </div>
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
   The pursuer adapts between stable enclosing trajectories as needed, ensuring robustness against uncertainties such as modeling inaccuracies, measurement errors, and external disturbances.
</div>

## Related Publications

<div class="publications">
  {% bibliography -f papers -q @*[key=new_2]* %}
  {% bibliography -f papers -q @*[key=new_2]* %}  
</div>
