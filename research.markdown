---
layout: page
title: Research
permalink: /research/
order: 1
---

<style>
.section {
  margin: 5px auto;
  display: flex;
  flex-direction: row;
  }

  img {
    width: 200px;
    height: 120px;
    object-fit: contain;
}

/* .contain {
  object-fit: contain;
} */
  
  .content {
    vertical-align:middle;
    padding: 10px;
  }

</style>

I've been working on a bunch of topics, mostly related to network control and multi-agent systems.
More recently, I've started to work on fault detection and safety of control systems.

Curious to learn more? Have a look at the items below!

<h2> Fault Detection </h2>

Sometimes, faults happen, be it because of missed maintenance of actuators or even cyber-attacks.
Faulty dynamics may be difficult to control but, even more crucial, there's serious risk they go undetected until it's too late, compromising <b>safety</b> of the system.

How can you know if your system has broken down when you can only look at sampled measurements?
<b>Fault detection</b>, or fault diagnosis, tries to answer this precise question by devising smart strategies that can tell that something's going wrong based on input and outputs of the system.

More coming soon. Stay tuned!

<h2> Resilient consensus and distributed control </h2>

<b><i>Disclaimer:</i></b> Resilience is arguably one of the most (ab)used keywords recently. Not my fault, though, so I'll just use it to be consistent with the literature.

In the context of multi-agent control, 
<b>resilient consensus</b> refers to "normal" agents trying to agree on a common value while interacting with "misbehaving" agents that, well, just do what they want. Consensus is widely used for distributed control (e.g., via distributed estimation or dstributed optimization),
and making it robust/resilient to faulty agents or cyber-attacks is key to effective deployment of several multi-agent control techniques.

My research works along two directions.
The first is to design resilient algorithms with <b>flexible performance guarantees</b>: that is,
they should not only drive normal agents to some desired behavior,
but also quantify how good (or bad) the situation is going to be,
without relying on too strict assumptions.
The second is to leverage physical communication to obtain <b>trustworthiness information</b> about transmitting agents
and in turn perform detection of possible adversaries.

{% capture details %}
<br>
<section class="section">
  <img src="/assets/deviation.jpg" />
  <div class="content">
    <p class="paragraph">
      L. Ballotta, M. Yemini, 
      "The Role of Confidence for Trust-based Resilient Consensus," 
      in <i>American Control Conference</i>, 2024 [to appear]
      [<a href="https://arxiv.org/abs/2404.07838" target="_blank">arxiv</a>]
    </p>
  </div>
</section>
<section class="section">
  <img src="/assets/trade-off-comp-coll.jpg" />
  <div class="content">
    <p class="paragraph">
      L. Ballotta, G. Como, J. S. Shamma and L. Schenato, "Can Competition Outperform Collaboration? The Role of Misbehaving Agents,"
      in <i>IEEE Transactions on Automatic Control</i>, 2024 
      [<a href="https://ieeexplore.ieee.org/abstract/document/10306277" target="_blank">online</a>]
    </p>
  </div>
</section>
{% endcapture %}
{% capture summary %}<b>Selected publications</b>{% endcapture %}{% include details.html %}

<h2> Distributed smart sensing design </h2>

Smart sensors broadly denote devices equipped with both sensing and compute capabilities,
such as smart cameras for surveillance,
environmental sensors for wildlife monitoring,
or even robots in cloud robotics settings.
Smart sensors typically have limited resources,
such as low computational or transmission power,
which need to be allocated wisely to enhance performance and lifespan.
This challenge is even more exhancerbated when dealing with networks of heterogeneous smart sensors. 

My research addresses optimal sensing (co-)desing under resource constraints such as nontrivial computation and transmission delays and limited power consumption,
with a twofold focus:
to develop suitable control-oriented models and problems that address realistic smart sensing,
and to devise effective algorithms for design.

My next step will be to add TinyML to the picture: if you happen to have ideas, shoot me an email!

{% capture details %}
<br>
<section class="section">
  <img src="/assets/fig-compute-not-compute.jpg" />
  <div class="content">
    <p class="paragraph">
      L. Ballotta, G. Peserico, F. Zanini, P. Dini, 
      "To Compute or Not to Compute? Adaptive Smart Sensing in Resource-Constrained Edge Computing," 
      in <i> IEEE Transactions on Network Science and Engineering</i>, 2024
      [<a href="https://ieeexplore.ieee.org/abstract/document/10225419" target="_blank">online</a>]
      [<a href="https://arxiv.org/abs/2209.02166" target="_blank">arxiv</a>]
    </p>
  </div>
</section>
<section class="section">
  <img src="/assets/fig-comp-comm-codesign.jpg" />
  <div class="content">
    <p class="paragraph">
      V. Tripathi, L. Ballotta, L. Carlone, E. Modiano,
      "Computation and communication co-design for real-time monitoring and control in multi-agent systems," 
      in <i>International Symposium on Modeling and Optimization in Mobile, Ad hoc, and Wireless Networks (WiOpt)</i>, 2021
      [<a href="https://ieeexplore.ieee.org/abstract/document/9589966" target="_blank">online</a>]
      [<a href="https://arxiv.org/abs/2108.03122" target="_blank">arxiv</a>]
    </p>
  </div>
</section>
<section class="section">
  <img src="/assets/fig-sensing-tradeoffs.jpg" />
  <div class="content">
    <p class="paragraph">
      L. Ballotta, L. Schenato, L. Carlone,
      "Computation-communication trade-offs and sensor selection in real-time estimation for processing networks," 
      in <i>IEEE on Network Science and Engineering</i>, 2020
      [<a href="https://ieeexplore.ieee.org/abstract/document/9137405" target="_blank">online</a>]
      [<a href="https://arxiv.org/abs/1911.05859" target="_blank">arxiv</a>]
    </p>
  </div>
</section>
{% endcapture %}
{% capture summary %}<b>Selected publications</b>{% endcapture %}{% include details.html %}