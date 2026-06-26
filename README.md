# CV_byeonguk
about CV 
# 안병욱 CV

## Profile
- Name: 안병욱
- Major: 시스템경영공학과
- Email: llnm0412@skku.edu
- GitHub: ...

## Education
- 성균관대학교 시스템경영공학과

## Research Interests
- AMR/AGV Simulation
- Manufacturing System Optimization
- Bottleneck Analysis
- Discrete-Event Simulation
- Design of Experiments / Quality Engineering

## Capstone Design Project
### Gripper-Aware Mobile Manipulator Dispatching Simulation for Semiconductor Packaging Process
### Seoul Semiconductor Industry-Academic Capstone Design
Developed a discrete-event simulation framework for optimizing Mobile Manipulator dispatching in a semiconductor packaging process. The project analyzed how dispatching rules, robot fleet size, layout constraints, and gripper performance affect equipment starvation and throughput.

* **Target Process:** Semiconductor packaging material handling process
* **Main Problem:** Inefficient dispatching and gripper failure can increase robot occupation time, cause equipment starvation, and reduce throughput.
* **Methods:** Discrete-event simulation, layout graph modeling, dispatching rule comparison, scenario-based experiment design
* **Dispatching Rules:** FIFO, NN, LQF, RTT, ATCS
* **Scenario Design:** 5 dispatching rules × 2 gripper conditions × 3 robot fleet sizes = 30 scenarios
* **KPIs:** Throughput, total starve time, robot utilization, corridor waiting frequency, re-grasp count, required robot count
* **My Role:** Simulation experiment design, KPI analysis, dispatching rule comparison, and optimization-oriented interpretation
* **Contribution:** Connected gripper-level hardware improvement with system-level manufacturing performance, providing a decision-support framework for AMR/Mobile Manipulator deployment and fleet-size planning.


## Research Achievements
...
## 1. Research Paper / Report List

### 1. Individual Paper Implementation & Open-source Analysis
1. **Open-source Paper Implementation Report: Domain Randomization for Sim-to-Real Transfer**

   * **Target Paper:** Tobin, J., Fong, R., Ray, A., Schneider, J., Zaremba, W., & Abbeel, P. (2017). *Domain Randomization for Transferring Deep Neural Networks from Simulation to the Real World*. IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS).
   * **Open-source Repository:** `matwilso/domrand`
   * **Project Type:** Individual open-source paper implementation and analysis
   * **Summary:**
     This project analyzed the concept of domain randomization for sim-to-real transfer in robotics. The original open-source implementation was reviewed and execution was attempted in a local Docker environment. Due to the aging dependencies of the original repository, including deprecated MuJoCo-related packages and Python version incompatibilities, the final implementation was reconstructed using PyBullet in Google Colab.
   * **Implementation Result:**
     The core idea of domain randomization was reproduced by generating randomized camera-view images of a simulated object. Camera distance, yaw, and pitch were randomly sampled, and multiple randomized simulation images were successfully generated.
   * **Key Learning Points:**

     * Understood the role of simulation in robotics and sim-to-real transfer.
     * Analyzed the limitations of outdated open-source research code.
     * Reproduced the core concept of camera randomization using PyBullet.
     * Documented implementation errors, causes, and resolution process.
   * **Submitted Materials:**

     * Analysis report slides
     * Source code notebook
     * Execution result screenshots
     * GitHub source code link

### 2. Team Open-source Research Paper Analysis

1. **SoftGrasp: Adaptive Grasping for Dexterous Hand Based on Multimodal Imitation Learning — Team Paper Analysis & Implementation**

   * **Target Paper:** Li, Y., Guo, C., Ren, J., Chen, B., Cheng, C., Zhang, H., & Lu, H. (2025). *SoftGrasp: Adaptive grasping for dexterous hand based on multimodal imitation learning*. Biomimetic Intelligence and Robotics, 5(1), Article 100217.
   * **Project Type:** Team-based open-source research paper analysis and model implementation
   * **Team:** Team 3, Smart Factory Capstone Design
   * **Team Members:** 양병호, 김강민, 김승우, 안병욱
   * **Summary:**
     This team project analyzed SoftGrasp, a multimodal imitation learning framework for adaptive robotic grasping. The paper addresses the limitations of conventional rigid-object grasping methods by integrating visual, joint-angle, and torque information to support stable grasping of deformable and irregular objects.
   * **Methodology Reviewed:**

     * Multimodal data collection using vision, joint angles, and torque signals
     * Feature extraction using ResNet-18 and MLP-based state encoders
     * Multimodal fusion through multi-head self-attention
     * Action prediction using angle and torque outputs
     * Model training using Huber Loss and Adam optimizer
   * **Implementation Result:**
     A simplified SoftGrasp-inspired model was implemented and tested using virtual training samples. The model structure included visual feature extraction, kinematic state encoding, attention-based multimodal fusion, and final action prediction. Training was conducted for 15 epochs, and the decreasing loss trend confirmed that the implemented model was able to learn from the constructed dataset.
   * **Key Learning Points:**

     * Understood the importance of multimodal sensing in robotic grasping.
     * Analyzed how attention mechanisms dynamically assign importance to vision, angle, and torque data across grasping stages.
     * Implemented a simplified multimodal learning pipeline inspired by the target paper.
     * Connected robotic grasping research with smart factory automation and flexible manufacturing applications.
   * **Submitted Materials:**

     * Team paper analysis slides
     * Model implementation and validation results
     * Training process and loss trend analysis
    
### 3. AI Coding Tools Practice

* **Post-Coding Era: AI Coding Tools Practice**
  Conducted an AI-assisted coding practice project using **Gemini Code Assist in VS Code**. The project was based on the research paper *Learning to Dispatch for Job Shop Scheduling via Deep Reinforcement Learning* (NeurIPS 2020), which applies deep reinforcement learning to job shop scheduling and dispatching decision problems.

  * **Target Paper:** Zhang et al., *Learning to Dispatch for Job Shop Scheduling via Deep Reinforcement Learning*, NeurIPS 2020
  * **Tool Used:** Gemini Code Assist in Visual Studio Code
  * **Topic:** Job shop scheduling, dispatching rules, deep reinforcement learning, AI-assisted code implementation
  * **GitHub Repository:** https://github.com/ByeongUk-ux/scheduling-.git
  * **Summary:**
    This project explored how AI coding tools can support the implementation and understanding of research code in the post-coding era. Gemini Code Assist was used in VS Code to help analyze, modify, and implement scheduling-related code based on a deep reinforcement learning approach for job shop scheduling.


## 2. Conference Paper

* **Title:** 반도체 패키징 공정에서 그리퍼 성능 개선을 고려한 Mobile Manipulator 디스패칭 최적화 시뮬레이션 연구
* **Status:** Scheduled for conference publication/presentation in July 2026
* **Research Area:** Smart factory, semiconductor manufacturing logistics, mobile manipulator dispatching, discrete-event simulation
* **Summary:**
  This paper presents a simulation-based decision-support framework for optimizing Mobile Manipulator dispatching in a semiconductor packaging process. The study analyzes how dispatching rules, robot fleet size, layout constraints, and gripper performance affect equipment starvation, throughput, and robot utilization.

## 3. Software Registration

* **Software Title:** AMR 물류 반송 스케줄링 최적화 이산사건 시뮬레이션 소프트웨어

* **Status:** Software registration completed

* **Summary:**
  This software was developed to optimize autonomous mobile robot logistics scheduling in advanced manufacturing processes such as semiconductor and display production. It models manufacturing uncertainty by reflecting equipment processing time distributions, robot handling time, failure probability, and recovery time. The simulator supports graph-based factory layout modeling, Dijkstra-based shortest path search, dynamic task assignment, discrete-event simulation, KPI analysis, and result logging.

* **Main Functions:**

  * Factory layout modeling using node, edge, equipment, robot, and scenario data
  * Shortest path search based on Dijkstra’s algorithm
  * Discrete-event simulation using a priority queue
  * Dynamic task allocation based on dispatching rules
  * KPI calculation including throughput, equipment waiting time, robot utilization, and transport waiting time
  * Bottleneck analysis using path usage frequency and detailed simulation logs

## 4. Patent Registration

* **Patent Title:** 지능형 모바일 매니퓰레이터 시스템 및 디스패칭 최적화 방법

* **Status:** Patent registration completed

* **Summary:**
  The patent relates to an intelligent Mobile Manipulator system and dispatching optimization method for automated logistics in semiconductor packaging processes. The invention integrates AI vision sensing, multimodal tactile sensing, graph-based layout modeling, and ATCS-based dispatching logic to reduce equipment starvation and improve system throughput.

* **Key Technical Elements:**

  * AI vision-based recognition of non-standardized handling objects
  * Multimodal tactile sensing for pressure and slip detection
  * Directional graph modeling of the actual manufacturing layout
  * ATCS-based composite dispatching algorithm
  * Real-time task priority control considering robot travel time and equipment waiting time
  * Throughput improvement and equipment starve time reduction



## Skills
- Python
- Simulation Modeling
- Data Analysis
- Statistical Analysis
- GitHub
