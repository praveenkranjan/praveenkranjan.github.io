---
layout: page
title: <h5>Guidance and Control for Autonomous Robots</h5>
description: ""
img: assets/img/guide_ctrl/sta_sitl.gif
importance: 3
category: Robotics
---

In the realm of distributed multi-agent systems, achieving effective coordination among agents while minimizing information exchange is paramount. This research focuses on innovative control strategies that allow agents to maintain flexible formations without relying on predetermined structures. By leveraging decentralized decision-making processes, our approach empowers agents to adapt their positions and orientations in response to dynamic environments and varying mission requirements. This flexibility enhances the system's robustness, enabling agents to operate efficiently even in the face of uncertainties and limited global information. Through our work, we aim to redefine the possibilities of multi-agent coordination, paving the way for more resilient and adaptable autonomous systems.

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;">Rapid prototyping for guidance algorithms for Unmanned aerial vehicles via Software in the Loop (SITL) and Hardware in the loop (HITL) simulations. </span>

This paper presents a novel approach to addressing the challenges of safe target enclosing by a single unmanned aerial vehicle (UAV) with limited information and autopilot lag considerations. Autopilot lag can cause delays in the response of the UAV, leading to potential safety risks. Therefore, the proposed guidance law takes into account the autopilot lag and aims to mitigate its effect on the UAVs' trajectory. We propose a robust guidance law that optimizes the UAV's trajectory to stay within safe proximity from the target in the presence of autopilot lag while also ensuring that the target always remains enclosed/contained. Moreover, since the UAV may have limited information available, the guidance law is designed to be robust and able to perform optimally with minimum information. Our approach thus enables the UAV to make intelligent decisions to execute corrective maneuvers based on the given safety requirements that could enhance situational awareness in complex and dynamic environments. We show through extensive simulations that our proposed guidance law significantly improves the UAV's performance while adhering to the constraints imposed on its trajectory.

<div class="row justify-content-sm-center">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/flex_form/flex_form_web_2.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Software-in-the-loop simulation used for testing the flexible formation guidance algorithms, ensuring readiness for real flight. 
        </div>
    </div>
</div>

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;"> Guidance of mobile-manipulator for waste mangement in GPS-Denied Environments</span>

This paper presents a novel approach to addressing the challenges of safe target enclosing by a single unmanned aerial vehicle (UAV) with limited information and autopilot lag considerations. Autopilot lag can cause delays in the response of the UAV, leading to potential safety risks. Therefore, the proposed guidance law takes into account the autopilot lag and aims to mitigate its effect on the UAVs' trajectory. We propose a robust guidance law that optimizes the UAV's trajectory to stay within safe proximity from the target in the presence of autopilot lag while also ensuring that the target always remains enclosed/contained. Moreover, since the UAV may have limited information available, the guidance law is designed to be robust and able to perform optimally with minimum information. Our approach thus enables the UAV to make intelligent decisions to execute corrective maneuvers based on the given safety requirements that could enhance situational awareness in complex and dynamic environments. We show through extensive simulations that our proposed guidance law significantly improves the UAV's performance while adhering to the constraints imposed on its trajectory.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/guide_ctrl/mob_mani.gif" title="example image" class="img-fluid rounded z-depth-1" %}
        <div class="caption">
            Flight experiments showcasing the practical implementation of flexible leader-follower formation control strategies.
        </div>
    </div>
</div>

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;">Robust UAV Guidance Law for Safe Target Circumnavigation with Limited Information and Autopilot Lag Considerations</span>

This paper presents a novel approach to addressing the challenges of safe target enclosing by a single unmanned aerial vehicle (UAV) with limited information and autopilot lag considerations. Autopilot lag can cause delays in the response of the UAV, leading to potential safety risks. Therefore, the proposed guidance law takes into account the autopilot lag and aims to mitigate its effect on the UAVs' trajectory. We propose a robust guidance law that optimizes the UAV's trajectory to stay within safe proximity from the target in the presence of autopilot lag while also ensuring that the target always remains enclosed/contained. Moreover, since the UAV may have limited information available, the guidance law is designed to be robust and able to perform optimally with minimum information. Our approach thus enables the UAV to make intelligent decisions to execute corrective maneuvers based on the given safety requirements that could enhance situational awareness in complex and dynamic environments. We show through extensive simulations that our proposed guidance law significantly improves the UAV's performance while adhering to the constraints imposed on its trajectory.

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

<hr> <!-- Adding a line to separate sections -->

## Related Publications

<div class="publications">
  {% bibliography -f papers -q @*[key=doi:10.2514/6.2024-0124]* %}
</div>
