---
title: "Deep Reinforcement Learning For Simultaneous Path
Planning and Stabilization of Offroad Vehicles"
collection: publications
permalink: /publication/2021_GVSETS
excerpt: 'Ameya Salvi, Jake Buzhardt, Phanindra Tallapragada, Venkat Krovi, Mark Brudnak, Jonathon M. Smereka'
date: 2021-08-10
venue: '2021 NDIA GROUND VEHICLE SYSTEM ENGINEERING AND TECHNOLOGY
SYMPOSIUM'
#slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
#paperurl: 'http://gvsets.ndia-mich.org/documents/AAIR/2021/AAIR%20140PM%20Deep%20Reinforcement%20Learning%20for%20Simultaneous%20Path%20Planning%20and%20Stabilization%20of%20Offroad%20Vehicles.pdf'
#citation: 'A. Salvi, J. Buzhardt, P. Tallapragada, V. Krovi, M. Brudnak, J. M. Smereka, “Deep reinforcement
#learning for simultaneous path planning and stabilization of offroad vehicles”, In Proceedings of the Ground
#Vehicle Systems Engineering and Technology Symposium (GVSETS), NDIA, Novi, MI, Aug. 10-12, 2021'
---

Motion planning algorithms for vehicles in an offroad environment have to contend with the significant vertical motion induced by the uneven terrain. Besides the obvious problems related to driver comfort, for autonomous vehicles, such “bumpy” vertical motion can induce significant mechanical noise in the real time data acquired from onboard sensors such as cameras to the point that perception becomes especially challenging. This paper advances a framework to address the problem of vertical motion in offroad autonomous motion control for vehicular systems. This framework is first developed to demonstrate the stabilization of the sprung mass in a modified quarter-car tracking a desired velocity while traversing a terrain with changing height. Even for an idealized model such as the quarter-car the dynamics turn out to be nonlinear and a model-based controller is not obvious. We therefore formulate this control problem as a Markov decision process and solve it using deep reinforcement learning. The control inputs that are learned are the torque on the wheel and the stiffness of the active suspension. It is demonstrated here that a time-varying velocity can be tracked with reduced chassis oscillations using these control inputs. We anticipate that reducing such oscillations will lead to sensor stabilization, which will improve perception and reduce the required frequency of recalibration. The deep reinforcement learning approach advanced in this paper remains useful for offroad motion planning when complex terramechanics and uncertain model parameters are introduced or the vehicle model increases in complexity.

**Citation** : *A. Salvi, J. Buzhardt, P. Tallapragada, V. Krovi, M. Brudnak, J. M. Smereka, “Deep reinforcement learning for simultaneous path planning and stabilization of offroad vehicles”, In Proceedings of the Ground Vehicle Systems Engineering and Technology Symposium (GVSETS), NDIA, Novi, MI, Aug. 10-12, 2021*

[**Preprint**](http://gvsets.ndia-mich.org/documents/AAIR/2021/AAIR%20140PM%20Deep%20Reinforcement%20Learning%20for%20Simultaneous%20Path%20Planning%20and%20Stabilization%20of%20Offroad%20Vehicles.pdf) 
