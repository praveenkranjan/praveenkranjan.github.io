---
layout: page
title: "Design and Development of Unmanned Aerial Vehicles"
description: ""
img: "assets/img/uavdesign/heliautorotate.gif"
importance: 5
category: "Flight Dynamics Modelling"
---

The design and development of UAVs involve integrating advanced aerodynamics, control systems, and sensor technology to ensure stability, efficiency, and adaptability in various flight conditions. This project explores both theoretical and practical aspects of UAV development, focusing on creating vehicles that can perform reliably in complex, dynamic environments. By leveraging modern modeling and control techniques, we aim to push the boundaries of UAV performance, especially for vertical takeoff and landing (VTOL) aircraft and small UAVs.

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;">Frequency Domain System Identification for Small UAVs</span>

In this work, we focus on the rapid development and testing of guidance algorithms for Unmanned Aerial Vehicles (UAVs) using Software-in-the-Loop (SITL) and Hardware-in-the-Loop (HITL) simulations. SITL allows for the testing of guidance strategies in a simulated environment that replicates real-world conditions, enabling rapid prototyping without the risk and expense of live flight tests. HITL further validates the algorithms by integrating actual UAV hardware components into the simulation loop, providing more realistic feedback on performance under real-world constraints such as sensor delays, actuator limits, and environmental disturbances. Together, these approaches accelerate the development process, ensuring that UAV guidance algorithms are robust, reliable, and ready for deployment in field operations.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/uavdesign/helifrequencysweep.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Flight data with multi-frequency input.
        </div>
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/uavdesign/heliautorotate.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Helicopter Autorotation Data Collection.
        </div>
    </div>
</div>
<div class="caption" style="font-style: italic; font-size: 14px; text-align: center;">
    Collecting flight data on helicopter UAV "TREX-ALign 700"
</div>

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;">Physics-based Flight Dynamics Modelling</span>

In this work, we develop and test guidance algorithms for UAVs using Software-in-the-Loop (SITL) and Hardware-in-the-Loop (HITL) simulations. SITL allows for the testing of guidance strategies in a simulated environment that replicates real-world conditions, enabling rapid prototyping without the risk and expense of live flight tests. HITL further validates the algorithms by integrating actual UAV hardware components into the simulation loop, providing more realistic feedback on performance under real-world constraints such as sensor delays, actuator limits, and environmental disturbances. These approaches ensure that UAV guidance algorithms are robust, reliable, and ready for deployment in real-world operations.
