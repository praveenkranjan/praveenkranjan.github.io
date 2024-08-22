---
layout: page
title: Safe Target Enclosing
description: a project with a background image
img: assets/img/flex_form/flex_form_web_1.gif
importance: 2
category: Relational Maneuvering Guidance and Control
---

In this paper, we address the problem of enclosing an arbitrarily moving target in three dimensions by a single pursuer, which is an unmanned aerial vehicle (UAV), for maximum coverage while also ensuring the pursuer’s safety by preventing collisions with the target. The proposed guidance strategy steers the pursuer to a safe region of space surrounding the target, allowing it to maintain a certain distance from the latter while offering greater flexibility in positioning and converging to any orbit within this safe zone. Our approach is distinguished by the use of nonholonomic constraints to model vehicles with accelerations serving as control inputs and coupled engagement kinematics to craft the pursuer’s guidance law meticulously. Furthermore, we leverage the concept of the Lyapunov Barrier Function as a powerful tool to constrain the distance between the pursuer and the target within asymmetric bounds, thereby ensuring the pursuer’s safety within the predefined region. To validate the efficacy and robustness of our algorithm, we conduct experimental tests by implementing a high-fidelity quadrotor model within Software-in-the-loop (SITL) simulations, encompassing various challenging target maneuver scenarios. The results obtained showcase the resilience of the proposed guidance law, effectively handling
arbitrarily maneuvering targets, vehicle/autopilot dynamics, and external disturbances. Our method consistently delivers stable global enclosing behaviors, even in response to aggressive target maneuvers, and requires only relative information for successful execution.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/inertialengagement.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/losengagement.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/regionsofoper_vid.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row justify-content-sm-center">
    <iframe width="720" height="540" src="https://www.youtube.com/embed/zmdImaB7bp0" title="Software-in-the-loop simulations with tuned autopilot" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</div>
<div class="caption">
    Target enclosing   
</div>
## Related Publications
<div class="publications">
  {% bibliography -f papers -q @*[key=new_4]* %}  
</div>
