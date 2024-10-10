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

System identification in the frequency domain plays a crucial role in developing accurate models for small UAVs, offering significant advantages over other modeling techniques. One of the key strengths of this approach is its ability to provide detailed insights into the UAV’s dynamic behavior across a wide range of frequencies, which is essential for understanding how the system responds to different inputs. By analyzing the frequency response of the UAV, engineers can capture the influence of aerodynamic forces, actuator dynamics, and structural flexibilities that affect the vehicle's performance during flight. This method allows for precise characterization of the UAV's transfer functions, making it easier to design and refine control algorithms tailored to the vehicle's specific dynamics. Frequency domain system identification can also help identify and mitigate resonance or instability issues, which are particularly important in small UAVs that may operate in environments with turbulence or other external disturbances. An additional advantage of this approach is its robustness to noise and modeling errors. Frequency domain techniques can isolate specific dynamics and reduce the impact of unmodeled phenomena, resulting in more reliable models. This, in turn, allows for the design of more effective control systems that can adapt to changes in the UAV’s operating environment and performance, leading to better overall flight stability and robustness.

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

Physics-based flight dynamics modeling is essential for understanding how UAVs behave under different flight regimes. In this subtopic, we focus on developing high-fidelity models that simulate the forces and moments acting on UAVs. By incorporating physical principles such as aerodynamics, propulsion, and control surface deflections, these models enable accurate predictions of UAV performance, paving the way for more effective control system design and optimization. This approach also facilitates simulations that closely mirror real-world flight conditions, which are critical for testing and validation before deployment.

<div class="publications">
  {% bibliography -f papers -q @*[key=new_5]* %}  
</div>
