# DEMO CENTER

> Catalog of projects, demos, simulators and platforms.

---

## Index

| # | Project | Main tags |
|---|---------|-----------|
| 1 | [CTE-Spazio](#1-cte-spazio) | `#training` `#seriousGaming` `#space` |
| 2 | [STEALTH](#2-stealth) | `#ROS` |
| 3 | [ACHILE](#3-achile) | `#DIS` `#gStreamer` `#digitalTwin` |
| 4 | [LATACC](#4-latacc) | `#DIS` `#SAPIENT` |
| 5 | [FEDERATES](#5-federates) | `#HLA` `#CrowdModeling` |
| 6 | [BEEYONDERS](#6-beeyonders) | `#PathPlanning` `#A*` |
| 7 | [EDI 4.0](#7-edi-40) | `#BIM` `#Asset` `#AIM` |
| 8 | [SBS](#8-sbs) | `#BIM` `#Asset` `#AIM` |
| 9 | [AIM SMARTARGETS](#9-aim-smartargets) | `#BIM` `#Asset` `#AIM` |
| 10 | [CTE](#10-cte) | `#VR` `#DigitalTwin` `#Robot` `#latency` |
| 11 | [EFESTO](#11-efesto) | `#BIM` `#Asset` `#Infrastructure` |
| 12 | [HealthyCity](#12-healthycity) | `#BIM` `#Asset` `#Health` `#Safety` |
| 13 | [BIM + VR (mobile/AR)](#13-bim--vr-mobilear) | `#BIM` `#AR` `#SIMULATION` |
| 14 | [PAVE-SCAN (AR)](#14-pave-scan-ar-thesis) | `#AR` `#SIMULATION` `#ROADMANAGEMENT` |
| 15 | [BIM + VR (web)](#15-bim--vr-web) | `#VR` `#SIMULATION` `#BIM` |
| 16 | [VR – Scenario Builder, Simulator & Training](#16-vr--scenario-builder-simulator--training) | `#VR` `#UNITY` `#SIMULATION` `#SCENARIOBUILDER` |

---

## 1. CTE-Spazio

**Description**
The application provides training for a Canadarm2 operator aboard the ISS.
The operator is located inside the ISS Cupola and has no freedom of movement. The goal of the training is to teach the operator the instrumentation related to the Canadarm and how to best use it to operate the arm.

Specifically, the task is to grab a small satellite with the End Effector. The simulator provides a simplified version of the instrumentation and controls, including:

- 10 selectable cameras
- Armstat screen for monitoring the arm joints
- frame (reference system) management
- 3 selectable speeds
- a per-joint control system (SHOULDER, ELBOW, WRIST) via a single joystick (rather than a dual one as in reality)

The simulator aims to be as immersive as possible, using the headset alone. The hands are automatically recognized by the headset cameras, so no joysticks are needed. To increase immersion, the simulation features accurate sound design of the cupola and high-realism 3D models for the cupola itself and outer space.

**Tags:** `#training` `#seriousGaming` `#space`

**Images**

| | | |
|---|---|---|
| ![](images/cte-spazio-iss-training-hub.png) | ![](images/cte-spazio-armstat.png) | ![](images/cte-spazio-cockpit-camere.png) |

**Videos**
- ▶️ [Intro_lowQuality_30fps.mp4](videos/Intro_lowQuality_30fps.mp4)
- ▶️ [DemoCenter_CTESpazioDemoVideo_Cut.mp4](videos/DemoCenter_CTESpazioDemoVideo_Cut.mp4) (1:46) — click the preview to play:

[![CTE-Spazio demo video](images/cte-spazio-dashboard.png)](videos/DemoCenter_CTESpazioDemoVideo_Cut.mp4)

---

## 2. STEALTH

**Description**
The STEALTH project aims to simulate drone swarms in GPS-denied situations. A set of real and simulated drones moves within the same simulated scenario and computes its path based on inputs of various kinds (mainly images).

**Tags:** `#ROS`

**Images**

| | |
|---|---|
| ![](images/stealth-login.png) | ![](images/stealth-airfield.png) |

**Video**
- ▶️ [DemoCenter_StealthDemoVideo_Cut.mp4](videos/DemoCenter_StealthDemoVideo_Cut.mp4) — click the preview to play:

[![STEALTH demo video](images/stealth-video-thumb.png)](videos/DemoCenter_StealthDemoVideo_Cut.mp4)

---

## 3. ACHILE

**Description**
The ACHILE project splits into two separate tasks:

- The first aims to develop digital twins of objects and maps to be used in a military context.
- The second uses the SBS tool to simulate the movement of a platoon in a real scenario, then communicates the position via the DIS protocol. The scenario includes a drone streaming video via gStreamer.

**Tags:** `#DIS` `#gStreamer` `#digitalTwin`

![](images/achile-logo.png)

**Videos**
- ▶️ [Low_Quality_DemoVideo.mp4](videos/Low_Quality_DemoVideo.mp4) — task **T5.4**
- ▶️ [DemoCenter_AchileT83Demo.mp4](videos/DemoCenter_AchileT83Demo.mp4) — task **T8.3**

| T5.4 | T8.3 |
|---|---|
| [![ACHILE T5.4](images/achile-t5-4-video-thumb.png)](videos/Low_Quality_DemoVideo.mp4) | [![ACHILE T8.3](images/achile-t8-3-video-thumb.png)](videos/DemoCenter_AchileT83Demo.mp4) |

---

## 4. LATACC

**Description**
The LATACC project aims to simulate the detection processes of a radar. An a-priori-undefined number of entities is communicated to the application via the DIS protocol, and as soon as the radar recognizes one of them it sends a SAPIENT message to a third-party application.

**Tags:** `#DIS` `#SAPIENT`

**Images**

| | |
|---|---|
| ![](images/latacc-dis-objects.png) | ![](images/latacc-area-markers.png) |

---

## 5. FEDERATES

**Description**
The FEDERATES project simulates a hypothetical military operation scenario in the Grosseto area. Specifically, a small crowd of 50 people is simulated as three military vehicles approach. The vehicle simulation runs on a third-party application, and the data is received via the HLA protocol. The same protocol is used to publish the crowd data.

**Tags:** `#HLA` `#CrowdModeling`

**Images**

| | |
|---|---|
| ![](images/federates-scenario-militare.png) | ![](images/federates-landscape.png) |

**Video**
- ▶️ [FederatesSimulationLowQuality.mp4](videos/FederatesSimulationLowQuality.mp4) (0:50)

---

## 6. BEEYONDERS

**Description**
The BEEYONDERS project models the trajectory of autonomous vehicles on a construction site. Based on the movement data of people in the environment, a trajectory is created that strikes a compromise between the probability of crossing an agent on its path and the total distance traveled. To do this, a "weighted" variant of the A* algorithm is used.

**Tags:** `#PathPlanning` `#A*`

**Images**

| | | |
|---|---|---|
| ![](images/beeyonders-cantiere.png) | ![](images/beeyonders-cantiere-aereo.png) | ![](images/beeyonders-rover-mappa.png) |

**Video**
- ▶️ [BeeyondersVideoOctober2024_LowQuality.mp4](videos/BeeyondersVideoOctober2024_LowQuality.mp4) (1:25) — click the preview to play:

[![BEEYONDERS October 2024 video](images/beeyonders-video-oct2024.png)](videos/BeeyondersVideoOctober2024_LowQuality.mp4)

---

## 7. EDI 4.0

**Description**
EDI 4.0 is a platform for the digitalization of the entire construction supply chain that integrates BIM and the management of the functions and processes of the companies in the supply chain, with an operational-cooperation logic.

**Client:** Upgrading Services
**Tags:** `#BIM` `#Asset` `#AIM`

---

## 8. SBS

**Description**
Extension of the EDI application with 5D BIM management and the import of budget and schedule data, also via xls. BIA (Business Impact Analyzer) management and integration of BIM with GIS.

**Client:** Upgrading Services
**Tags:** `#BIM` `#Asset` `#AIM`

---

## 9. AIM SMARTARGETS

**Description**
An innovative digital platform aimed at facilitating and automating the integrated management of information (digital information and models, so-called BIM) in ST's operational context, i.e. in architectural construction and infrastructure projects.

Prototype features:

- upload, visualization and navigation of the BIM model;
- archiving and exposure of the metadata representing the informational content of the BIM model;
- design of integration with field devices at the single-model level for monitoring the asset in the operational phase;
- design of asset visualization features in a VR environment (e.g. integration with VR development frameworks such as Unity).

**Client:** SmarTargets
**Tags:** `#BIM` `#Asset` `#AIM`

---

## 10. CTE

**Description**
The project aims to evaluate the performance of the communication network between a simulator developed in Unity and a real robot operating in a physical environment. The interaction takes place in virtual reality (VR), where a digital replica of the robot (digital twin) is displayed. Communication latency is measured by comparing the movement of the virtual model in the simulator with the actual response of the robot in real time.

The project aims to test communication quality within a 5G network. The scenario features a UR10 industrial robot controlled via a Unity application, with communication specifically occurring between the Unity terminal and a Python controller connected to the robot via cable.

The Unity application includes both the "virtual" and the "real" version of the robot: the latter is based on the robot's real-time data and is represented as a *ghost* (a version identical to the virtual one but semi-transparent). The discrepancy between the "virtual" version (zero latency) and the "real" version (latency dependent on the 5G connection) lets you visually understand the latency provided by the network. A 3D dashboard within the application also allows the precise history of the data to be displayed.

**Tags:** `#VR` `#DigitalTwin` `#Robot` `#latency`

**Videos**
- ▶️ [CTE_Video2.mp4](videos/CTE_Video2.mp4)

---

## 11. EFESTO

**Description**
An innovative Asset Management digital platform aimed at facilitating and automating the management of information for infrastructure (e.g. the construction and building sector) and the individual elements that compose it (assets).

Current features:

- census of contexts (e.g. construction sites, contracts, etc.) and of assets (elements within a context);
- upload, visualization and navigation of the BIM model;
- document management associated with each context.

Future directions: budget management, scheduling, access to budget and schedule information via IFC files (5D BIM).

**Client:** US
**Tags:** `#BIM` `#Asset` `#Infrastructure`
**Possible future features:** LCA, BIA (Business Impact Analyzer), VR/AR

---

## 12. HealthyCity

**Description**
A digital platform for visualizing infrastructure in the healthcare sector and accessing the 3D BIM visualization of infrastructure with the related details of specific assets. The platform allows project users to view the 3D models of the infrastructure and to access individual assets, through a zoom-in feature, to the model and visualize it on the model itself. Moreover, from the BIM viewer, it is possible to see the asset's data and the related associated documents.

**Client:** LASIA
**Tags:** `#BIM` `#Asset` `#Infrastructure` `#Health` `#Safety`

---

## 13. BIM + VR (mobile/AR)

**Description**
The project produced a mobile application dedicated to visualizing BIM models in augmented reality, to localizing and navigating the model in AR via positioning based on a QR-code reference system, and to viewing, editing, saving and versioning the data contained in the displayed BIM.

**Tags:** `#BIM` `#AR` `#SIMULATION`

**Videos**
- ▶️ [Demo-AR-BIM-lowRes.mp4](videos/Demo-AR-BIM-lowRes.mp4)

---

## 14. PAVE-SCAN (AR)

**Description**
The project produced a mobile application dedicated to identifying potholes on the road surface in augmented reality. It allows you to add a pothole, edit it and view it in AR. First prototype for the PAVE-SCAN project.

**Tags:** `#AR` `#SIMULATION` `#ROADMANAGEMENT`

**Videos**
- ▶️ [Video-anomalia-in-strada-e-modifiche.mp4](videos/Video-anomalia-in-strada-e-modifiche.mp4)

---

## 15. BIM + VR (web)

**Description**
The project produced a web application dedicated to visualizing BIM models in virtual reality (3D), to localizing and navigating the model in VR via positioning within the scene, and to viewing the data contained in the displayed BIM. It also allows headless upload of BIM models.

**Tags:** `#VR` `#SIMULATION` `#BIM`

**Videos**
- ▶️ [Video-Rebecca-2.mp4](videos/Video-Rebecca-2.mp4)

---

## 16. VR – Scenario Builder, Simulator & Training

**Description**
The solution aims first and foremost to be a tool for analyzing and assessing the vulnerabilities of public spaces and for identifying potential response strategies. Furthermore, it aims to enable training and experimentation services for security procedures, for designing responses to attacks. The target users of the solution are everyone who manages security in any type of public space.

The solution offers several features absent from competitors' solutions, in particular: the creation of VR/AR models of the built environment, the dynamic design of a scenario's security assets, the creation of scenarios concerning threats and attack plans with dynamic configurations, the ability to create complex crowding dynamics within the public space under analysis, the dynamic simulation of crowd behaviors and designed attack plans, the simulation of alternative configurations of the same scenarios and plans, and multiplayer serious-gaming features to practice security procedures and experience simulated scenarios first-hand.

This solution is used to design scenarios in public spaces and the so-called built environment (such as music festivals, train stations, religious sites), to create multiple and customized configurations of attack plans and of static security elements, to dynamically simulate the behavior of the crowd modeled within the designed scenarios, and to experiment with and train security trainees within the simulated scenarios.

**Tags:** `#VR` `#UNITY` `#SIMULATION` `#SCENARIOBUILDER`

**Videos**
- ▶️ Scenario Builder — [SBS_Spirit.mp4](videos/SBS_Spirit.mp4)
- ▶️ Simulation — [SIM_Spirit.mp4](videos/SIM_Spirit.mp4)

---
