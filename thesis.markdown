---
layout: page
title: Thesis proposals
permalink: /thesis/
order: 2
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

I offer thesis projects for both Bachelor's and Master's degrees.
Topics are broadly related to control systems over networks, safety and security, machine learning, and resource allocation.
Below you'll find a succinct summary of research topics I am interested in. For more details, please head to [Research](research.markdown). Also, you'll find specific thesis project proposals (Master's level) at [my thesis elearning webpage](https://elearning.dei.unipd.it/tesi/proposte-tesi/?relatore=417&corso=&selected_tags=){:target="_blank"}.

Bachelor's theses will typically involve control applications and/or critical review of relevant literature, and serve as an entry point to specific research topics, application domains, or control-oriented software development.
Master's theses are expected to address open research problems in control applications or methodology.

If you are interested in doing a thesis on any of the topics below, please [send me an email](emailto:luca.ballotta@unipd.it) with "[Thesis]" in the subject line attaching you CV (coursework and any relevant experience) and specify what you would like to study in the email body. I'm happy to discuss alternative topics you may be interested in. Also, I'm open to multi-disciplinary thesis projects related to telecommunications, mathematics, operation research, computer science, etc.

<!-- processing networks -->
{% capture details %}

A processing network is a multi-agent network system where agents are equipped with sensing, compute, communication, and possibly actuation/decision-making. It models a broad spectrum of systems such as wireless sensor networks, multi-robot systems, or Industrial Internet-of-Things.

Since agents are lightweight, their collective operations must be carefully managed to ensure high performance under energy, hardware, and bandwidth constraints. For example, when can a robot reduce local computations and rely on information sent by neighboring robots?

An interesting setting is edge-cloud architecture, where an agent (i.e., an edge device) can offload execution of computationally intensive tasks to a powerful edge or cloud server to save energy, for instance in autonomous driving. In this scenario, optimally balancing computation and communication latency and energy is key to ensure high performance and safety.

Specific problems in this area include (but are not limited to):
- policies for computation allocation and cloud offloading
- TinyML vs. cloud offloading for edge devices
- distributed event-triggered estimation
- federated learning and distributed federated learning 
- control of multi-robot systems
- time- and/or frequency-based scheduling of smart sensors
- sensor and actuator selection
- cloud offloading for autonomous driving
{% endcapture %}
{% capture summary %}<b> Processing networks and Edge Computing </b>{% endcapture %}{% include details.html %}

<!-- resilient multi-agent systems -->
{% capture details %}

In multi-agent systems connected over wireless networks, cyberattacks can intrude the system through the network itself to compromise nominal system behavior and, in the worst case, disrupt safety and performance.

I am interested in designing resilient distributed algorithms that, without centralized coordination or detection, can cope with unknown adversarial agents. This problem has relevant applications in federated learning, multi-robot systems, and smart power networks, to name a few.

A particularly attractive opportunity is represented by recent research in physical layer security, a cybersecurity approach based on detecting variations of physical communication signals. How to efficiently interface this security approach with higher-level control and learning objective is an active line of research.

Specific problems in this area include (but are not limited to):
- robust aggregation algorithms for distributed optimization and learning
- resilient multi-agent reinforcement learning
- physical layer authentication (PLA) for multi-agent and distributed algorithms
- data-driven filters for detection of adversarial neighbors
{% endcapture %}
{% capture summary %}<b>Resilient multi-agent systems</b>{% endcapture %}{% include details.html %}

<!-- vehicular federated learning -->
{% capture details %}

Federated learning is a machine learning framework where the dataset is split into many pieces, each assigned to an independent machine, or client. Due to privacy concerns, but also communication constraints, aggregating all individual datasets is not an option, requiring appropriate techniques whereby each client locally trains a model and all models are periodically aggregated to enhance performance.

Recently, federated learning on vehicles has been proposed as a promising solution to efficiently use sensory data generated while traveling, such as from cars' cameras and lidars. However, this scenario brings in several challenges: vehicles are mobile and thus network connectivity may change overtime; computation resources are limited; data collected online cannot be manually labeled by humans.

Specific problems in this area include (but are not limited to):
- time-based scheduling of vehicles
- self-supervised and unsupervised federated learning
- energy-efficient allocation of vehicular computing resources
- active learning
- joint resource allocation and path planning of vehicles
{% endcapture %}
{% capture summary %}<b>Vehicular federated learning</b>{% endcapture %}{% include details.html %}

<!-- safe control and learning -->
{% capture details %}

Physical control systems are subject to more or less stringent safety requirements, from collision avoidance in robot navigation and autonomous driving to current balancing in power networks. Such requirements can typically be expressed as set-membership hard constraints on the state of the system; in other words, the state must always remain inside a set, usually called <i>safe set</i>. This requirement is particularly challenging with learning-based models, e.g., reinforcement learning in the control loop, as they cannot generally learn hard constraints and therefore must be tweaked appropriately.

One powerful way to meet hard safety constraints uses control barrier functions (CBF), which are control Lyapunov-like functions that ensure forward invariance of a set. However, finding an appropriate control barrier functions is computationally challenging in general and requires careful evaluation of unmodeled dynamics and noises. In addition, the integration of barrier functions with learning-based models is still an open research area.

Specific problems in this area include (but are not limited to):
- control barrier functions with noisy dynamics and/or measurements
- control barrier functions for multi-agent systems
- safe reinforcement learning with control barrier functions
- learning-based construction of control barrier functions
- formal verification of control barrier functions
- codesign of sensors and control barrier functions

{% endcapture %}
{% capture summary %}<b>Safe control and learning</b>{% endcapture %}{% include details.html %}

<!-- sparse control and learning -->
{% capture details %}

Large-scale systems impose restrictions on the control inputs. Even if many inputs are theoretically available, practical constraints typically require to select few of those inputs. This situation occurs in, for example, large-scale network systems with limited bandwidth, social media management through influencers, or control of biological networks for drug development.
For a linear systems, the problem of sparse control can be seen as the selection of few columns of the input-state matrix <b><i>B</i></b>, typically subject to controllability constraints and/or minimization of control energy.

Specific problems in this area include (but are not limited to):
  - energy-efficient actuator selection and scheduling (i.e., time-varying selection)
  - structural controllability under actuator selection or scheduling
  - sparse control of large-scale networks and multi-agent systems
  - sparse attacks and defense strategies for cybersecurity
  - energy-efficient sparse reinforcement learning

{% endcapture %}
{% capture summary %}<b>Sparse control and learning</b>{% endcapture %}{% include details.html %}