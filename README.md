# Implementing Natural Language Control (NLC) Framework in Webots
Watch Demo Video: https://canva.link/24ucb50t14p52yz
<img width="782" height="508" alt="image" src="https://github.com/user-attachments/assets/a32316c6-2103-45c3-8e6c-f9690921ff51" />


## Overview
This project demonstrates the implementation of a **Natural Language Control (NLC)** framework in the **Webots** robotics simulation environment.

The system enables a **Leader robot** to receive human text commands (e.g., *"Find target in the west"*) and coordinate **three follower robots** in a **star-topology multi-agent architecture** to execute the task autonomously.

Each follower robot is capable of:
- GPS-based navigation
- Compass-based heading correction
- Obstacle avoidance
- Colour-based visual target detection
- Status reporting back to the leader

---

## Project Objectives
The aim of this project was to design and simulate a multi-robot system capable of translating natural language instructions into coordinated robotic actions.

The project combines concepts from:
- Natural Language Processing (NLP)
- Multi-agent systems
- Robotics navigation
- Computer vision
- Fault-tolerant autonomous control

---

## System Architecture
The system follows a **star topology architecture**:

- **1 Leader Robot**
  - Receives and interprets human commands
  - Extracts task intent using keyword-based NLP
  - Sends structured commands to followers

- **3 Follower Robots**
  - Receive instructions from the leader
  - Navigate toward assigned targets
  - Search for visual objects
  - Report completion status

Example command:

```text
Find chai in the east
