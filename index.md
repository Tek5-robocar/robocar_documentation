---
layout: three-column
title: Project Overview
---

# Robocar: Autonomous Racing Project

Welcome to the **Robocar** project — an open educational and research-ready platform for developing and testing autonomous navigation systems.

## 📌 Project Overview

**Robocar** is designed as a modular robotics platform that combines:
- High-precision navigation using **GNSS RTK GPS**
- Advanced motor control with **VESC (Vedder Electronic Speed Controller)**
- AI-driven decision-making trained via **simulation environments**

It’s ideal for university research, student projects, and robotics competitions.

## 🧭 Project Goals & Architecture

The **Robocar** project aims to develop a modular, autonomous racing platform capable of navigating complex circuits, processing real-time sensor data, and learning from simulation. It’s designed for hands-on education, AI research, and robotics competitions.

To achieve this, the system combines the following core components:

| Module            | Purpose |
|--------------------|---------|
| **AI Control**       | Python-based control logic trained via simulation |
| **Simulation**       | Unity-based racing environment for model testing and training |
| **GNSS RTK GPS + IMU** | Centimeter-level localization and motion sensing using the Point One Dev Kit |
| **Motor Control**    | High-efficiency motor management via VESC (Vedder ESC) |
| **Embedded Platform**| Real-time inference and control using Jetson Nano |
| **Computer Vision**  | Object tracking and depth perception with OAK-D Lite and DepthAI |

This architecture supports the project's objectives of real-world autonomy, AI validation in simulation, and integration of multiple perception and control technologies.



## 🚀 Getting Started

To explore this project:
1. Read the [Read the GNSS Guide]({{ '/gnss-rtk-gps/' | relative_url }})
2. Follow the [VESC Calibration Instructions]({{ '/vesc-calibration/' | relative_url }})

## 🏁 UTAC 2025 Tournament

In 2025, our Robocar team took part in the **UTAC autonomous vehicle tournament**, a national competition that brought together student-led robotics projects from across the country. It was an incredible opportunity to test our system in real-world conditions and benchmark our AI against others on a professional-grade circuit.

📖 Check out the full article to read about our experience, results, and technical challenges:  
👉 [Read the UTAC 2025 Recap](https://www.epitech.eu/2025/07/08/robocar-au-challenge-utac-2025/)

📹 And watch the highlight video from the event on YouTube:  
<iframe width="560" height="315"
  src="https://www.youtube.com/embed/BvDePUn8-f0"
  title="YouTube video player"
  frameborder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowfullscreen>
</iframe>


## 🧠 Acknowledgements

This project is supported by [Epitech](https://www.epitech.eu/) and contributions from robotics enthusiasts and students.

## 📬 Contact

For questions, feature requests, or collaboration proposals, feel free to [open an issue](https://github.com/tek5-robocar/robocar_documentation/issues) or reach out via email.