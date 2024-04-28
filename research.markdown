---
layout: page
title: Research
permalink: /research/
order: 1
---

<style>
.section {
    display: flex;
    flex-direction: row;
  }

  img {
    max-width: 25%;
    max-height:10%;
    float: left;
  }
  
  .content {
    padding: 20px;
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
  <img src="/assets/deviation.jpg" class="image" />
  <div class="content">
    <p class="paragraph">
      L. Ballotta, M. Yemini, "The Role of Confidence for Trust-based Resilient Consensus," in <i>Proc. American Control Conference</i>, 2024 [to appear]
      [<a href="https://arxiv.org/abs/2404.07838" target="_blank">online</a>]
    </p>
  </div>
</section>
<br>
<section class="section">
  <img src="/assets/trade-off-comp-coll.jpg" class="image" />
  <div class="content">
    <p class="paragraph">
      L. Ballotta, G. Como, J. S. Shamma and L. Schenato, "Can Competition Outperform Collaboration? The Role of Misbehaving Agents," in <i>IEEE Transactions on Automatic Control</i>, 2024 
      [<a href="https://ieeexplore.ieee.org/abstract/document/10306277" target="_blank">online</a>]
    </p>
  </div>
</section>
{% endcapture %}
{% capture summary %}<b>Selected publications</b>{% endcapture %}{% include details.html %}

