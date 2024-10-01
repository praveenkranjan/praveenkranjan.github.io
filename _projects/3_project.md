---
layout: page
title: <h5>Self-organizing Mutlti-agent Target Enclosing.</h5>
description: #
img: assets/img/safe_enc/self_org_f1.gif
importance: 1
category: Distributed Multi-agents Systems
---

This paper introduces an approach to address the target enclosing problem using non-holonomic multiagent systems, where agents self-organize on the enclosing shape around a fixed target. In our approach, agents independently move toward the desired enclosing geometry when apart and activate the collision avoidance mechanism when a collision is imminent, thereby guaranteeing inter-agent safety. Our approach combines global enclosing behavior and local collision avoidance mechanisms by devising a special potential function and sliding manifold. We rigorously show that an agent does not need to ensure safety with every other agent and put forth a concept of the nearest colliding agent (for any arbitrary agent) with whom ensuring safety is sufficient to avoid collisions in the entire swarm. The proposed control eliminates the need for a fixed or pre-established agent arrangement around the target and requires only relative information between an agent and the target. This makes our design particularly appealing for scenarios with limited global information, hence significantly reducing communication requirements. We finally present simulation results to vindicate the efficacy of the proposed method.

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
