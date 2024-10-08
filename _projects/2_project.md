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

In this paper, we address the problem of enclosing an arbitrarily moving target in three dimensions by a single pursuer, which is an unmanned aerial vehicle (UAV), for maximum coverage while also ensuring the pursuer’s safety by preventing collisions with the target. The proposed guidance strategy steers the pursuer to a safe region of space surrounding the target, allowing it to maintain a certain distance from the latter while offering greater flexibility in positioning and converging to any orbit within this safe zone. Our approach is distinguished by the use of nonholonomic constraints to model vehicles with accelerations serving as control inputs and coupled engagement kinematics to craft the pursuer’s guidance law meticulously. Furthermore, we leverage the concept of the Lyapunov Barrier Function as a powerful tool to constrain the distance between the pursuer and the target within asymmetric bounds, thereby ensuring the pursuer’s safety within the predefined region. To validate the efficacy and robustness of our algorithm, we conduct experimental tests by implementing a high-fidelity quadrotor model within Software-in-the-loop (SITL) simulations, encompassing various challenging target maneuver scenarios. The results obtained showcase the resilience of the proposed guidance law, effectively handling arbitrarily maneuvering targets, vehicle/autopilot dynamics, and external disturbances. Our method consistently delivers stable global enclosing behaviors, even in response to aggressive target maneuvers, and requires only relative information for successful execution.

<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/regionsofoper.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
    Safe region for pursuer motion while enclosing the target
</div>

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/safe_enc_v1.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
    The pursuer encloses the target switching between stable enclosing trajectories offering robustness to uncertainty 
</div>

## Related Publications

<div class="publications">
  {% bibliography -f papers -q @*[key=new_2]* %}
  {% bibliography -f papers -q @*[key=new_2]* %}  
</div>
