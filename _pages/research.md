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

---

# Learning enhanced system idendtification and control for skid-steer wheel mobile robots
Skid-steered wheeled mobile robots (SSWMRs) find utility in a wide range of outdoor application arenas owing to their design simplicity, high maneuverability and relative ease for human control. Complete or partial autonomy for SSWMRs can thus be of significant benefit for the dull, dirty and dangerous environments which these robots operate within. The followin research investigation entails leveraging contemporary machine learning methods for renvisioning the motion characteristics and off-road control strategies for SSWMRs. 

## Deep reinforcement learning control
<iframe src="https://drive.google.com/file/d/15OgLxI7fIti-KspaqmniIypnsGHWD6w9/preview" width="900" height="480" allow="autoplay"></iframe>

A low-perception frequency control policy trained using deep reinforcement learning for combining the concepts of path look-ahead based motion planing, trajectory generation and control for skid-steer vehicles. Here, a proximal policy optimization (PPO) policy was trained using CoppeliaSim simulator as a gym environment coupled with the StableBaselines3 libraries for visual navigation under perception uncertainty for Clearpath Husky robot.

## Autonomy oriented digital twins using HPC

![HPC_Autonomy](https://github.com/ameyarsalvi/ameyarsalvi.github.io/assets/54649022/d79ec39c-a8f5-4ea0-9e66-1eb8ae16d67f)

Leveraging high performance compute clusters for photrealistic rendering of outdoor environments for systematic verification and validation of autonomy algorithms. In this work, NVIDIA ISAAC Sim was utilized to setup a visual navigation framework in outdoor simulation environments using the Palmetto cluster at Clemson University.

**Associated research products**

Code : <br />
[Behavior Cloning](https://github.com/ClemsonFA1p1/SummitXL_BehaviourCloning) | 
[Lane Keeping:Sim](https://github.com/ClemsonFA1p1/SummitXL_ReinforcementLearning) | 
[Skid-steer Visual Servoing](https://github.com/ARMLabCUICAR/SkidSteerVisualNavigation)

Publications : 
1. [Virtual Evaluation of Deep Learning Techniques for Vision-Based Trajectory Tracking](/publication/2022_SAE_WCX)

 --- 

# Stabilization of vehicles on bumpy terrain

Stabilizing vertical dynamics for on-road and off-road vehicles is an important research area that has been looked at mostly from the point of view of ride comfort. The advent of autonomous vehicles now shifts the focus more towards developing stabilizing techniques from the point of view of onboard proprioceptive and exteroceptive sensors whose real-time measurements influence the performance of an autonomous vehicle. The current solutions to this problem of managing the vertical oscillations usually limit themselves to the realm of active suspension systems without much consideration to modulating the vehicle velocity, which plays an important role by the virtue of the fact that vertical and longitudinal dynamics of a ground vehicle are coupled. The task of stabilizing vertical oscillations for military ground vehicles becomes even more challenging due lack of structured environments, like city roads or highways, in off-road scenarios. Moreover, changes in structural parameters of the vehicle, such as mass (due to changes in vehicle loading), suspension stiffness and damping values can have significant effect on the controller's performance. This demands the need for developing deep learning based control policies, that can take into account an extremely large number of input features and approximate a near optimal control action. In this work, these problems are addressed by training a deep reinforcement learning agent to minimize the vertical acceleration of a scaled vehicle travelling over bumps by controlling its velocity. 

<iframe src="https://drive.google.com/file/d/1NlVM-7oufR6W0oXX-_F-P897iKylaFEW/preview" width="900" height="480" allow="autoplay"></iframe>

**Associated research products**

Code :  <br />
[Scaled Vehicle Stabilization](https://github.com/ClemsonFA1p1/Krovi_Tallapragada_qcar_stabilization) |
[Quater-car Stabilization](https://github.com/ClemsonFA1p1/GVSETS_RL_QuarterCar)

Publications : 
1. [Stabilization of vertical motion of a vehicle on bumpy terrain using deep reinforcement learning](/publication/2022_MECC)
2. [Deep Reinforcement Learning for Simultaneous Path Planning and stabilization of Off-road Vehicles](/publication/2021_GVSETS)
   
--- 

# Articulated Robotics

## Cable driven parallel robots
Cable driven parallel robots (CDPRs) are often challenging to model and to dynamically control due to the inherent flexibility and elasticity of the cables. The additional inclusion of online geometric reconfigurability to a CDPR results in a complex underdetermined system with highly non-linear dynamics. The necessary (numerical) redundancy resolution requires multiple layers of optimization rendering its application computationally prohibitive for real-time control. Here, deep reinforcement learning approaches can offer a model-free framework to overcome these challenges and can provide a real-time capable dynamic control. This study discusses three settings for a model-free DRL implementation in dynamic trajectory tracking: (i) for a standard non-redundant CDPR with a fixed workspace; (ii) in an end-to-end setting with redundancy resolution on a reconfigurable CDPR; and (iii) in a decoupled approach resolving kinematic and actuation redundancies individually.

<iframe width="900" height="480" src="https://www.youtube.com/embed/IOs0d03G12g?si=8OYsWJkjWPaClFyx" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

**Associated research products**

Code:  <br />
[GitHub](https://github.com/ameyarsalvi/CDPR_ICRA)

Publications :
1. [Reinforcement Learning Control of a Reconfigurable Planar Cable Driven Parallel Manipulator](/publication/2023_ICRA)

--- 

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
