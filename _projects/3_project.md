---
layout: page
title: Learning for Dynamics and Control
description: #
img: assets/img/safe_enc/self_org_f1.gif
importance: 4
category: Distributed Multi-agents Systems
---

Mobile robots often operate in dynamic, uncertain environments, requiring adaptive and precise control strategies. Traditional control methods rely on precise mathematical models, which can be difficult to derive for complex or unpredictable environments. This work focuses on leveraging learning-based approaches to improve the understanding of robot dynamics, allowing for more flexible and accurate control. By integrating data-driven models with control algorithms, the study aims to enable mobile robots to perform tasks more efficiently and autonomously in real-world scenarios.

<hr> <!-- Adding a line to separate sections -->

### <span style="font-weight: bold; font-size: 24px;">Deep Reinforcement learning for generalized motion planning of non-holonomic agents.</span>

In this work, we focus on the application of deep reinforcement learning (DRL) to develop robust and adaptable motion planning strategies for non-holonomic agents, such as wheeled robots and autonomous vehicles. Non-holonomic agents face constraints on their motion, making traditional planning techniques less effective. This work leverages the ability of DRL to learn complex policies through interaction with the environment, enabling generalized, efficient, and collision-free path planning in dynamic or complex environments, even with limited maneuverability. The study aims to enhance autonomous navigation by integrating learning-based approaches with classical motion planning concepts.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/self_org_f1.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/self_org_f2.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/self_org_f3.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/safe_enc/self_org.gif" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
## Related Publications
<div class="publications">
  {% bibliography -f papers -q @*[key=new_4]* %}  
</div>
