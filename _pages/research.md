---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

### Quick Links
1. [Skid-steered wheel mobile robots](#learning-enhanced-system-idendtification-and-control-for-kid-steer-wheel-mobile-robots)
2. [Stabilization on bumpy terrain](#stabilization-of-vehicles-on-bumpy-terrain)
3. [Articulated Robotics](#articulated-robotics)
4. [Containerization for robotics](#containerization-approach-towards-robotics-code-development-and-deployment)

<hr style="border:2px solid gray">

# Learning enhanced system idendtification and control for skid-steer wheel mobile robots
Skid-steered wheeled mobile robots (SSWMRs) find utility in a wide range of outdoor application arenas owing to their design simplicity, high maneuverability and relative ease for human control. Complete or partial autonomy for SSWMRs can thus be of significant benefit for the dull, dirty and dangerous environments which these robots operate within. The followin research investigation entails leveraging contemporary machine learning methods for renvisioning the motion characteristics and off-road control strategies for SSWMRs. 

## Learning for control

<style>
.responsive-iframe-container {
  position: relative;
  width: 100%;
  padding-bottom: 50%; /* 16:9 aspect ratio: 9/16 = 56.25%, 2:1 = 50% */
  height: 0;
  overflow: hidden;
}

.responsive-iframe-container iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 0;
}
</style>

<div class="responsive-iframe-container">
  <iframe src="https://drive.google.com/file/d/16S25WQNtAdzdsIEUFzd2tlVRqSk3fsKO/preview" allow="autoplay"></iframe>
</div>


A low-perception frequency control policy trained using deep reinforcement learning for combining the concepts of path look-ahead based motion planing, trajectory generation and control for skid-steer vehicles. Here, a proximal policy optimization (PPO) policy was trained using CoppeliaSim simulator as a gym environment coupled with the StableBaselines3 libraries for visual navigation under perception uncertainty for Clearpath Husky robot.

## Learning for System Idenitification

<style>
.responsive-iframe-container {
  position: relative;
  width: 100%;
  padding-bottom: 50%; /* 16:9 aspect ratio: 9/16 = 56.25%, 2:1 = 50% */
  height: 0;
  overflow: hidden;
}

.responsive-iframe-container iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 0;
}
</style>

<div class="responsive-iframe-container">
  <iframe src="https://drive.google.com/file/d/1H1IiMRArH_sOqK1w_919cNtoDNWUzFtz/preview" allow="autoplay"></iframe>
</div>


Skid-steered wheel mobile robots (SSWMRs) operate in a variety of outdoor environments exhibiting motion behaviors dominated by the effects of complex wheel-ground interactions. Characterizing these interactions is crucial both from the immediate robot autonomy perspective (for motion prediction and control) as well as a long-term predictive maintenance and diagnostics perspective. An ideal solution entails capturing precise state measurements for decisions and controls, which is considerably difficult, especially in increasingly unstructured outdoor regimes of operations for these robots. In this milieu, a framework to identify pre-determined discrete modes of operation can considerably simplify the motion model identification process. To this end, we propose an interactive multiple model (IMM) based filtering framework to probabilistically identify predefined robot operation modes that could arise due to traversal in different terrains or loss of wheel traction.

## Autonomy oriented digital twins using HPC

![HPC_Autonomy](https://github.com/ameyarsalvi/ameyarsalvi.github.io/assets/54649022/d79ec39c-a8f5-4ea0-9e66-1eb8ae16d67f)

Leveraging high performance compute clusters for photrealistic rendering of outdoor environments for systematic verification and validation of autonomy algorithms. In this work, NVIDIA ISAAC Sim was utilized to setup a visual navigation framework in outdoor simulation environments using the Palmetto cluster at Clemson University.

**Associated research products**

Code : <br />
[Pose informed Reinforcement Learning](https://github.com/ameyarsalvi/PoseEnhancedSSVN) |
[Behavior Cloning](https://github.com/ClemsonFA1p1/SummitXL_BehaviourCloning) | 
[Lane Keeping:Sim](https://github.com/ClemsonFA1p1/SummitXL_ReinforcementLearning) | 
[Skid-steer Visual Servoing](https://github.com/ARMLabCUICAR/SkidSteerVisualNavigation) |
[IMM based mode identification](https://github.com/ameyarsalvi/2025_ICRA_HuskyIMM)

Publications : 
1. [Virtual Evaluation of Deep Learning Techniques for Vision-Based Trajectory Tracking](/publication/2022_SAE_WCX)
2. [Online identification of skidding modes with interactive multiple model estimation](https://arxiv.org/abs/2409.20554)
3. [Experimental investigation of pose informed reinforcement learning for skid-steered visual navigation](https://arxiv.org/abs/2506.21732)
4. [Characterizing gaussian mixture of motion modes for skid-steer state estimation](https://arxiv.org/abs/2505.00200)

<hr style="border:2px solid gray">

# Stabilization of vehicles on bumpy terrain

Stabilizing vertical dynamics for on-road and off-road vehicles is an important research area that has been looked at mostly from the point of view of ride comfort. The advent of autonomous vehicles now shifts the focus more towards developing stabilizing techniques from the point of view of onboard proprioceptive and exteroceptive sensors whose real-time measurements influence the performance of an autonomous vehicle. The current solutions to this problem of managing the vertical oscillations usually limit themselves to the realm of active suspension systems without much consideration to modulating the vehicle velocity, which plays an important role by the virtue of the fact that vertical and longitudinal dynamics of a ground vehicle are coupled. The task of stabilizing vertical oscillations for military ground vehicles becomes even more challenging due lack of structured environments, like city roads or highways, in off-road scenarios. Moreover, changes in structural parameters of the vehicle, such as mass (due to changes in vehicle loading), suspension stiffness and damping values can have significant effect on the controller's performance. This demands the need for developing deep learning based control policies, that can take into account an extremely large number of input features and approximate a near optimal control action. In this work, these problems are addressed by training a deep reinforcement learning agent to minimize the vertical acceleration of a scaled vehicle travelling over bumps by controlling its velocity. 

<style>
.responsive-iframe-container {
  position: relative;
  width: 100%;
  padding-bottom: 50%; /* 16:9 aspect ratio: 9/16 = 56.25%, 2:1 = 50% */
  height: 0;
  overflow: hidden;
}

.responsive-iframe-container iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border: 0;
}
</style>

<div class="responsive-iframe-container">
  <iframe src="https://drive.google.com/file/d/1NlVM-7oufR6W0oXX-_F-P897iKylaFEW/preview" allow="autoplay"></iframe>
</div>


**Associated research products**

Code :  <br />
[Scaled Vehicle Stabilization](https://github.com/ClemsonFA1p1/Krovi_Tallapragada_qcar_stabilization) |
[Quater-car Stabilization](https://github.com/ClemsonFA1p1/GVSETS_RL_QuarterCar)

Publications : 
1. [Stabilization of vertical motion of a vehicle on bumpy terrain using deep reinforcement learning](/publication/2022_MECC)
2. [Deep Reinforcement Learning for Simultaneous Path Planning and stabilization of Off-road Vehicles](/publication/2021_GVSETS)
   
<hr style="border:2px solid gray">

# Articulated Robotics

## Cable driven parallel robots
Cable driven parallel robots (CDPRs) are often challenging to model and to dynamically control due to the inherent flexibility and elasticity of the cables. The additional inclusion of online geometric reconfigurability to a CDPR results in a complex underdetermined system with highly non-linear dynamics. The necessary (numerical) redundancy resolution requires multiple layers of optimization rendering its application computationally prohibitive for real-time control. Here, deep reinforcement learning approaches can offer a model-free framework to overcome these challenges and can provide a real-time capable dynamic control. This study discusses three settings for a model-free DRL implementation in dynamic trajectory tracking: (i) for a standard non-redundant CDPR with a fixed workspace; (ii) in an end-to-end setting with redundancy resolution on a reconfigurable CDPR; and (iii) in a decoupled approach resolving kinematic and actuation redundancies individually.

<iframe width="640" height="320" src="https://www.youtube.com/embed/IOs0d03G12g?si=8OYsWJkjWPaClFyx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**Associated research products**

Code:  <br />
[GitHub](https://github.com/ameyarsalvi/CDPR_ICRA)

Publications :
1. [Reinforcement Learning Control of a Reconfigurable Planar Cable Driven Parallel Manipulator](/publication/2023_ICRA)

<hr style="border:2px solid gray">

# Containerization approach towards robotics code development and deployment

Over the decades, robotics deployments have leveraging synergies with rapid in-parallel research and developmental advances in sensing, actuation, simulation, algorithmic control, communication, and high-performance computing among others. Collectively, their integration within a cyber-physical-systems framework has supercharged the increasingly complex realization of the real-time ‘sense-think-act’ robotics paradigm. Successful functioning of modern-day robots relies on seamless integration of increasingly complex systems (coming together at the component-, subsystem-, system- and system-of-system levels) as well as their systematic treatment throughout the life-cycle (from cradle to grave). As a consequence, ‘dependency management’ between the physical/algorithmic inter-dependencies of the multiple system elements is crucial for enabling synergistic (or managing adversarial) outcomes. In this work, we explore various facets of these challenges for autonomous operations with a simulated/physical Clearpath Husky robot by developing Robot Operating System (ROS) based Docker containers, that isolate different functions of the robot operations and yet interact with each other in  real-time for a synergistic deployment.


<p float="left">
  <img src="https://github.com/ameyarsalvi/ameyarsalvi.github.io/assets/54649022/4c198ac6-c88a-4f6f-b7dd-94dc1fe13fd5" width="450" height="250" />
  <img src="https://github.com/ameyarsalvi/ameyarsalvi.github.io/assets/54649022/75410e93-5ba3-45dd-98f9-1f843b63758c" width="450" height="250" /> 
</p>

**Associated research products**

Code:  <br />
[Containerized Parallel Simulations](https://github.com/ClemsonFA1p1/Containerization_terramechanics) |
[Containerized Module Integration](https://github.com/ClemsonFA1p1/Husky_motion_plan)

Publications:
1. [Containerization Approach for High-Fidelity Terramechanics Simulations](/publications/2023_SAE_WCX)
