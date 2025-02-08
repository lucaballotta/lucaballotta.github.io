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
Recently, I've started to work on fault detection and safety of control systems.

Curious to learn more? Have a look at the items below!

<h2> Multi-robot collaboration </h2>

{% capture details %}
<br>
<section class="section">
  <img src="/assets/paper_figs/dcbf.jpg" />
  <div class="content">
    <p class="paragraph">
      L. Ballotta, R. Talak,
      "Safe Distributed Control of Multi-Robot Systems with Communication Delays", 
      2024
      [<a href="https://arxiv.org/abs/2402.09382" target="_blank">arxiv</a>]
    </p>
  </div>
</section>
<section class="section">
  <img src="/assets/paper_figs/dlite.jpg" />
  <div class="content">
    <p class="paragraph">
      Y. Chang, L. Ballotta, L. Carlone,
      "D-Lite: navigation-oriented compression of 3D scene graphs for multi-robot collaboration," 
      <i> IEEE Robotics and Automation Letters</i>, 2023
      [<a href="https://ieeexplore.ieee.org/document/10265226" target="_blank">online</a>]
    </p>
  </div>
</section>
<section class="section">
  <img src="/assets/paper_figs/trajectoryTrackingSampled.png" />
  <div class="content">
    <p class="paragraph">
      E. Rossi, M. Tognon, L. Ballotta, R. Carli, J. Cortés, A. Franchi, L. Schenato,
      "Coordinated multi-robot trajectory tracking control over sampled communication," 
      <i>Automatica</i>, 2023
      [<a href="https://www.sciencedirect.com/science/article/pii/S0005109823000924" target="_blank">online</a>]
    </p>
  </div>
</section>
{% endcapture %}
{% capture summary %}<b>Selected publications</b>{% endcapture %}{% include details.html %}

<h2> Resilient multi-agent systems </h2>

<b><i>Disclaimer:</i></b> Resilience is arguably one of the most (ab)used keywords recently. Not my fault, though, so I'll just be consistent with the literature.

In multi-agent systems, 
<b>resilient control</b> makes "normal" agents cooperate and collaborate while interacting with "misbehaving" agents that, well, just do what they want.

My research works along two directions.
The first is to design resilient algorithms with <b>flexible performance guarantees</b>: that is,
they should not only drive normal agents to some desired behavior,
but also quantify how good (or bad) the situation is going to be,
without relying on strict assumptions.
The second is to leverage physics-based sources of information,
such as the wireless channel,
to obtain <b>trustworthiness indications</b> of agents based on their transmitted data and in turn to detect adversaries.

{% capture details %}
<br>
<section class="section">
  <img src="/assets/paper_figs/trustConfidence.jpg" />
  <div class="content">
    <p class="paragraph">
      L. Ballotta, M. Yemini, 
      "The Role of Confidence for Trust-based Resilient Consensus," 
      <i>American Control Conference</i>, 2024
      [<a href="https://arxiv.org/abs/2404.07838" target="_blank">arxiv</a>]
      [<a href="https://ieeexplore.ieee.org/document/10644459" target="_blank">online</a>]
    </p>
  </div>
</section>
<section class="section">
  <img src="/assets/paper_figs/compColl.jpg" />
  <div class="content">
    <p class="paragraph">
      L. Ballotta, G. Como, J. S. Shamma and L. Schenato, "Can Competition Outperform Collaboration? The Role of Misbehaving Agents,"
       <i>IEEE Transactions on Automatic Control</i>, 2024 
      [<a href="https://ieeexplore.ieee.org/document/10306277" target="_blank">online</a>]
    </p>
  </div>
</section>
{% endcapture %}
{% capture summary %}<b>Selected publications</b>{% endcapture %}{% include details.html %}

<h2> Processing networks </h2>

Processing networks are wonderful beasts where interconnected smart sensors collect, process, and exchange data to fulfill a task.
Prominents examples are <b>smart cameras for surveillance,
environmental sensors for pollution monitoring,
teams of mobile robots,
Internet-of-Things devices,
and autonomous vehicles</b>.
Smart sensors have limited computation and communication resources which need to be wisely allocated to optimize performance.
This challenge is exhancerbated when dealing with networks of heterogeneous smart sensors.

My research investigates <b>optimal codesing under resource constraints</b> such as computation and transmission delays and limited power consumption,
with a twofold focus:
to develop <b>tailored models</b> of smart sensors under realistic conditions,
and to devise <b>codesign algorithms</b> for optimal performance and resource allocation.

My next step will be to add TinyML to the picture: if you'd like to collaborate, shoot me an email!

{% capture details %}
<br>
<section class="section">
  <img src="/assets/paper_figs/vremfl.png" />
  <div class="content">
    <p class="paragraph">
      L. Ballotta, N. Dal Fabbro, G. Perin, L. Schenato, M. Rossi, G. Piro,
      "VREM-FL: Mobility-Aware Computation-Scheduling Co-Design for Vehicular Federated Learning,"
      <i>IEEE Transactions on Vehicular Technology</i>, 2024
      [<a href="https://ieeexplore.ieee.org/document/10715716" target="_blank">online</a>]
    </p>
  </div>
</section>
<section class="section">
  <img src="/assets/paper_figs/processingNetworkAdaptive.jpg" />
  <div class="content">
    <p class="paragraph">
      L. Ballotta, G. Peserico, F. Zanini, P. Dini, 
      "To Compute or Not to Compute? Adaptive Smart Sensing in Resource-Constrained Edge Computing," 
      <i> IEEE Transactions on Network Science and Engineering</i>, 2024
      [<a href="https://ieeexplore.ieee.org/document/10225419" target="_blank">online</a>]
    </p>
  </div>
</section>
<section class="section">
  <img src="/assets/paper_figs/processingNetwork.jpg" />
  <div class="content">
    <p class="paragraph">
      L. Ballotta, L. Schenato, L. Carlone,
      "Computation-communication trade-offs and sensor selection in real-time estimation for processing networks," 
      <i>IEEE on Network Science and Engineering</i>, 2020
      [<a href="https://ieeexplore.ieee.org/abstract/document/9137405" target="_blank">online</a>]
      [<a href="https://arxiv.org/abs/1911.05859" target="_blank">arxiv</a>]
    </p>
  </div>
</section>
{% endcapture %}
{% capture summary %}<b>Selected publications</b>{% endcapture %}{% include details.html %}