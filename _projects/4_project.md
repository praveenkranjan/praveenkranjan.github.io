---
layout: page
title: <h5>Autonomous Navigation and Control of Unmanned Vehicles</h5>
description: ""
img: assets/img/guide_ctrl/sta_sitl.gif
importance: 3
category: Robotics
---

The field of automatic guidance and control of unmanned systems is rapidly evolving, driven by advancements in artificial intelligence, sensor technology, and communication systems. This area encompasses a wide range of applications, from unmanned aerial vehicles (UAVs) to mobile manipulators, each requiring sophisticated control strategies to navigate complex environments effectively. This research aims to develop robust, adaptive guidance algorithms that ensure safety, efficiency, and flexibility in dynamic conditions. By leveraging methodologies such as Software in the Loop (SITL) and Hardware in the Loop (HITL) simulations, our work emphasizes the importance of rapid prototyping in optimizing control strategies. The integration of robust guidance mechanisms that account for factors such as autopilot lag and GPS-denied conditions ensures that unmanned systems can operate reliably and autonomously across diverse operational scenarios.

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;">Rapid prototyping of guidance algorithms for Unmanned aerial vehicles via Software in the Loop (SITL) and Hardware in the loop (HITL) simulations. Flight experiments were conducted on FVR-90, a fixed-wing vertical take-off and landing vehicle developed by L3Harris technologies. $$ a_1 $$ </span>

In this work, we focus on the rapid development and testing of guidance algorithms for Unmanned Aerial Vehicles (UAVs) using Software-in-the-Loop (SITL) and Hardware-in-the-Loop (HITL) simulations. SITL allows for the testing of guidance strategies in a simulated environment that replicates real-world conditions, enabling rapid prototyping without the risk and expense of live flight tests. HITL further validates the algorithms by integrating actual UAV hardware components into the simulation loop, providing more realistic feedback on performance under real-world constraints such as sensor delays, actuator limits, and environmental disturbances. Together, these approaches accelerate the development process, ensuring that UAV guidance algorithms are robust, reliable, and ready for deployment in field operations.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/flex_form_web_2.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Software-in-the-loop simulation used for testing the flexible formation guidance algorithms, ensuring readiness for real flight. 
        </div>
    </div>
</div>

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;"> Autonomous Control of Mobile Manipulators in GPS-Denied Conditions </span>

In GPS-denied environments, where traditional positioning systems are unavailable, guiding a mobile manipulator autonomously presents a unique challenge. This work focuses on developing robust navigation and control algorithms that enable mobile manipulators to operate efficiently in such environments. By leveraging onboard sensors, vision-based localization, and advanced state estimation techniques, we aim to ensure precise motion control and object manipulation without relying on external positioning systems. Our approach enables mobile robots to perform tasks such as pick-and-place operations, obstacle avoidance, and path planning in constrained, dynamic, and unstructured settings where GPS signals are unavailable.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/guide_ctrl/mob_mani.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Autonomous Mobile Manipulator operation without global position information.
        </div>
    </div>
</div>

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;">Robust guidance with Autopilot Lag Considerations</span>

In this work, we address the challenge of developing robust guidance strategies for unmanned aerial vehicles (UAVs) in the presence of autopilot lag. Autopilot lag, which introduces delays between control commands and the actual response of the UAV, can significantly impact flight performance and safety, particularly in dynamic environments. Our proposed guidance law is specifically designed to mitigate the effects of this lag, ensuring that the UAV maintains safe and reliable operation while pursuing its objectives. By incorporating lag-aware control mechanisms and ensuring robustness to various uncertainties, our approach allows for precise and stable flight even in the presence of significant delays, enabling UAVs to navigate complex scenarios with increased safety and performance.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/guide_ctrl/stline_autopilot.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Target moving in Straight line
        </div>
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/guide_ctrl/arb_autopilot.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Arbitrarily maneuvering target
        </div>
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
    Pursuer adapting for lag in autopilot dynamics to sucessfully enclose moving targets
</div>

## Related Publications

<div class="publications">
  {% bibliography -f papers -q @*[key=doi:10.2514/6.2024-0124]* %}
</div>
