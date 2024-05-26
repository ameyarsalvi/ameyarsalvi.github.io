---
title: "Containerization Approach for High-Fidelity Terramechanic Simulations"
collection: publications
permalink: /publication/2023_SAE_WCX
excerpt: 'Sanskruti Deepak Jadhav, Ameya Salvi, Krishna Chaitanya Kosaraju, Jonathon Smereka, Mark Brudnak, Venkat N Krovi, David Gorsich.'
date: 2023-04-10
venue: 'SAE Technical Paper'
#slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
#paperurl: 'http://gvsets.ndia-mich.org/documents/AAIR/2021/AAIR%20140PM%20Deep%20Reinforcement%20Learning%20for%20Simultaneous%20Path%20Planning%20and%20Stabilization%20of%20Offroad%20Vehicles.pdf'

---
Integrated modeling of vehicle, tire and terrain is a fundamental challenge to be addressed for off-road autonomous navigation. The complexities arise due to lack of tools and techniques to predict the continuously varying terrain and environmental conditions and the resultant non-linearities. The solution to this challenge can now be found in the plethora of data driven modeling and control techniques that have gained traction in the last decade. Data driven modeling and control techniques rely on the system’s repeated interaction with the environment to generate a lot of data and then use a function approximator to fit a model for the physical system with the data. Getting good quality and quantity of data may involve extensive experimentation with the physical system impacting developer’s resource. The process is computationally expensive, and the overhead time required is high.
High-fidelity simulators coupled with cloud-based containers can help ease the challenge of data ‘quality’ and ‘quantity’. Project Chrono is a multi-physics simulation engine that provides high-fidelity simulation capabilities with emphasis on flow and terrain modeling. With a host of libraries and APIs for industry accepted tools like MATLAB, Simulink and TensorFlow, Project Chrono proves to be a powerful research bed for data-driven modeling and control development for off-road navigation. Containers are lightweight virtual machines that take away repetitive configurations by setting up a computational environment, including all necessary dependencies and libraries. Docker encapsulates an end-to-end platform solution for heavy computation challenges of deep learning applications and allows fast development and testing. The synergy between the high-fidelity simulator and the compute outsourcing capabilities of cloud-based containers proves to be extremely beneficial for continuous integration and continuous deployment (CI/CD) for data driven modeling and control tasks. In the following work, we containerize a high-fidelity simulator (Project Chrono) to develop and validate data driven modeling and control algorithms for off-road autonomous navigation.

**Citation** : *Jadhav, S. D., Salvi, A., Kosaraju, K. C., Smereka, J., Brudnak, M., Krovi, V. N., & Gorsich, D. (2023). Containerization Approach for High-Fidelity Terramechanics Simulations (No. 2023-01-0105). SAE Technical Paper.*

[**Preprint**](https://par.nsf.gov/servlets/purl/10489454)
