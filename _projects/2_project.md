---
layout: page
title: "Multi-agent Systems and Control"
description: "Research on flexible and safe motion planning strategies for relational maneuvering using UAVs."
img: assets/img/safe_enc/self_org_f3.gif
importance: 2
category: "Relational Maneuvering Guidance and Control"
---

In the field of autonomous systems, multi-vehicle coordination is crucial for achieving complex missions involving UAVs. My research focuses on developing flexible and safe motion planning strategies for relational maneuvering, where multiple UAVs operate in coordination to maintain specific formations and adapt to dynamic mission requirements. By integrating safety constraints with flexible control mechanisms, I aim to enhance UAV performance in tasks such as target tracking, formation flying, and area coverage. These approaches allow UAVs to navigate safely while responding to unpredictable changes in the environment, ensuring reliable and robust operations in real-world scenarios.

<hr> <!-- Adding a line to separate sections -->

### Self-organising for multi-agent systems.

This paper introduces an approach to address the target enclosing problem using non-holonomic multiagent systems, where agents self-organize on the enclosing shape around a fixed target. In our approach, agents independently move toward the desired enclosing geometry when apart and activate the collision avoidance mechanism when a collision is imminent, thereby guaranteeing inter-agent safety. Our approach combines global enclosing behavior and local collision avoidance mechanisms by devising a special potential function and sliding manifold. We rigorously show that an agent does not need to ensure safety with every other agent and put forth a concept of the nearest colliding agent (for any arbitrary agent) with whom ensuring safety is sufficient to avoid collisions in the entire swarm. The proposed control eliminates the need for a fixed or pre-established agent arrangement around the target and requires only relative information between an agent and the target. This makes our design particularly appealing for scenarios with limited global information, hence significantly reducing communication requirements. We finally present simulation results to vindicate the efficacy of the proposed method.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/self_org_f1.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/self_org_f2.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
    Collision free Behaviour of pursuer autonomously organising on the desired orbit of desired proximity.
</div>

<hr> <!-- Adding a line to separate sections -->

### Safety and flexibility in Target Enclosing.
This paper focuses on developing an energy-efficient control algorithm for a type of leader-follower aircraft formation, namely, ring formation, where the follower seeks to track a virtual circle, also called a ring, whose center is behind the leader along the leader's heading direction. Enabling this type of ring formation allows the follower to maintain a certain geometric configuration with respect to the leader, but not a rigid structure that is often hard for the follower to maintain in, e.g., turning maneuvers. Meanwhile, the flexibility in a ring formation lies in the fact that the follower can stay on any point on the ring, thus helping save thrust-related energy consumption and addressing inherent physical constraints. Towards this objective, we develop a new controller using the backstepping technique and use nonlinear dynamic programming to address the control input constraints. First, we show that the minimum speed point on the ring can yield the lowest energy consumption. We then provide a specific control design based on backstepping for the follower to track the minimum speed point on the ring. To address the physical input constraints, we propose to use nonlinear dynamic programming to optimize the control inputs subject to control saturation. Finally, we present simulation results to demonstrate the effectiveness of the proposed approach in saving energy and addressing control input constraints.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/eng_form.png" title="example image" class="img-fluid rounded z-depth-1" %}
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
  {% bibliography -f papers -q @*[key=new_2]* %}
</div>
