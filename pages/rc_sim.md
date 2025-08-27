---
layout: three-column
title: Racing Simulator
permalink: /racing-sim/
description: A step-by-step guide for setting up the Racing Simulator Unity simulation so you can use it as-is or customize it to fit your needs.
---

## Main Overview

# Overview

This page provides a high-level overview of the **RacingSimulator** project, which is split into two main components:

[Simulation](Overview_Simulation.md)  
: The Unity-based environment used to simulate racing scenarios for training.

[AI](Overview_AI.md)  
: The Python-based interface and logic that allows your AI agent to connect to and control the simulation.

---

## What is the RacingSimulator?

The **RacingSimulator** is an AI training environment where your task is to develop and connect an autonomous agent that can control a car in a 3D racing simulation.

The objective is to train your agent to complete laps as efficiently and quickly as possible using reinforcement learning or other AI techniques.  
The simulator offers multiple tracks with increasing levels of difficulty to challenge and evaluate your models.

---

## Glossary

Here are some key terms you might encounter while working with this project:

<deflist>

<def title="AI">
Artificial Intelligence — the field concerned with building systems that can perform tasks typically requiring human intelligence, such as perception, decision-making, and control.
</def>

<def title="Unity">
A popular, cross-platform game engine used for developing 2D, 3D, and VR/AR experiences.  
Used here to build the simulation environment.  
See: <a href="https://unity.com/">unity.com</a>
</def>

</deflist>

---

## Simulation Overview

# Overview

This page introduces the **simulation** component of the RacingSimulator project.  
It is built in **Unity** and is designed to train AI agents to drive between two parallel lines with increasing autonomy and efficiency.

---

## What Is This?

This simulation was developed using **Unity** to generate training data and experiment with custom AI models.

Unity was chosen for its ease of use, extensive documentation, built-in car physics, and its support for the **ML-Agents** toolkit, which makes it easy to connect external AI agents to the environment.

By using **ML-Agents**, the simulation can host "dummy" agents that wait for external input — for example, from Python scripts.  
It’s also possible to use Unity's own learning system via config files and adjust hyperparameters for built-in training.

> 📘 If you want to try it yourself, follow the step-by-step setup in the [tutorial](Tutorial_Simulation.md).
> 🔄 To understand how the AI connects and interacts with the simulation, check out the [AI Overview](Overview_AI.md).

---

## Glossary

<deflist>
  <def title="Unity">
    A widely-used real-time 3D development engine for games and simulations.  
    It offers tools for physics, animation, rendering, and scripting — ideal for building custom training environments.
  </def>

  <def title="ML-Agents">
    Unity's Machine Learning Agents Toolkit.  
    It enables communication between Unity simulations and external machine learning frameworks such as PyTorch.
  </def>

  <def title="Agent">
    An entity in the simulation that perceives observations and takes actions.  
    In this project, the agent represents the car you're training.
  </def>

  <def title="Environment">
    The Unity simulation in which the agent operates. Includes visuals, physics, obstacles, tracks, etc.
  </def>

  <def title="Observation">
    The information sent from the simulation to the agent — such as sensor values, raycasts, or positional data.
  </def>

  <def title="Action">
    A response returned by the agent, such as turning, accelerating, or braking.
  </def>

  <def title="Reward">
    A numerical value that tells the agent how well it performed — for example, staying between lines or completing laps.
  </def>
</deflist>

---

## AI Overview

# Overview

This is the **AI** part of the *RacingSimulator* project.

The goal of this component is to provide an interface between a Python script (your AI or manual driver) and the Unity simulation.

---

## What Is This?

To interact with the Unity simulation, we use the `mlagents` and `mlagents_envs` libraries from Unity’s ML-Agents Toolkit.  
These libraries offer a fast, deterministic, and easy-to-use API for communicating with agents in the simulation.

The user must create a Python script that launches the Unity simulation and connects to it via ML-Agents.  
At every frame, the script is prompted to send a decision — either human-controlled or AI-generated.

There are two main interaction modes:

1. **Manual Driving** – You control the car using the keyboard (arrow keys), and the script relays these actions to the simulation. This mode is typically used to collect datasets.
2. **AI-Controlled Driving** – Your Python-based AI model decides what actions to take, and the script sends them to the simulation in real-time.

> 📘 To get started writing your own Python controller, follow the [AI Tutorial](Tutorial_AI.md).  
> 🔄 For details on how the simulation is structured, see the [Simulation Overview](Overview_Simulation.md).

---

## Glossary

<deflist>

<def title="AI">
Artificial Intelligence – algorithms and models that can make decisions, often trained via machine learning.
</def>

<def title="ML-Agents">
Unity's Machine Learning Agents Toolkit, which enables simulations to interface with external reinforcement learning or scripted agents.
</def>

<def title="Agent">
An entity within the Unity simulation that receives observations and performs actions.
</def>

<def title="Observation">
Data received from the simulation describing the environment, such as distance to lines or raycast results.
</def>

<def title="Action">
A response sent by the AI or human input to influence the agent — for example, steering or accelerating.
</def>

<def title="Environment">
The Unity-based simulation that the agent interacts with.
</def>

</deflist>