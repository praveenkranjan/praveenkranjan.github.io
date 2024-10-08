---
layout: page
title: <h5>Guidance and Control for Autonomous Robots</h5>
description: another without an image
img: assets/img/guide_ctrl/self_org.gif
importance: 3
category: Robotics
---

In the realm of distributed multi-agent systems, achieving effective coordination among agents while minimizing information exchange is paramount. This research focuses on innovative control strategies that allow agents to maintain flexible formations without relying on predetermined structures. By leveraging decentralized decision-making processes, our approach empowers agents to adapt their positions and orientations in response to dynamic environments and varying mission requirements. This flexibility enhances the system's robustness, enabling agents to operate efficiently even in the face of uncertainties and limited global information. Through our work, we aim to redefine the possibilities of multi-agent coordination, paving the way for more resilient and adaptable autonomous systems.

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;">Self-organising Multi-agent Target enclosing</span>

This research presents an innovative approach to solving the target enclosing problem using non-holonomic multi-agent systems. Our method enables agents to self-organize around a fixed target, independently moving toward the desired formation while activating collision avoidance mechanisms when necessary. By combining global formation behavior with local collision avoidance, we ensure safe, coordinated movement among agents. The approach simplifies safety management by requiring each agent to focus only on its nearest potential collision, reducing the complexity of the system. This method is particularly effective in scenarios with limited global information, offering a robust solution that minimizes communication needs.

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
    <div class="col-sm-5 mt-3 mt-md-0">
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
  {% bibliography -f papers -q @*[key=new_4]* %}
  {% bibliography -f papers -q @*[key=new_2]* %}  
</div>
