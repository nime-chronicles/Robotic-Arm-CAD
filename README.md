# 🤖 Robotic Arm CAD

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![CAD: Fusion 360 / SolidWorks](https://img.shields.io/badge/CAD-Parametric-blue.svg)](#software--compatibility)
[![Hardware: 6-DOF](https://img.shields.io/badge/Hardware-6--DOF-orange.svg)](#technical-specifications)

A comprehensive mechanical design and 3D CAD repository for an open-source [6]-Degree-of-Freedom (DoF) Robotic Arm This repository contains parametric source files, exported STEP/IGES assemblies, 3D-printable STL meshes, and a complete mechanical Bill of Materials (BOM).

---

## 📌 Overview

The **Robotic Arm CAD** project is engineered for [pick one: educational research]. The architecture focuses on high mechanical rigidity, accessible fabrication (3D printing and off-the-shelf fasteners), and straightforward integration with standard servo and stepper motor drivers.

### ✨ Key Features
* **Multi-Axis Articulation:** **[e.g., 6-DOF articulation with a rotating base, dual-arm shoulder, elbow, and 3-axis spherical wrist]**.
* **Optimized for 3D Printing:** Designed without requiring complex support structures where possible; flat orientation planes included for FDM printing.
* **Standardized Hardware:** Relies on metric hardware (**[e.g., M3/M4 fasteners and 608ZZ bearings]**) for ease of sourcing.
* **Modularity:** Interchangeable end-effector mount (**[e.g., parallel gripper, vacuum cup, or pen holder]**).

---

## ⚙️ Technical Specifications

| Parameter | Specification | Notes |
| :--- | :--- | :--- |
| **Degrees of Freedom** | **[6 DoF + Gripper]** | Rotational joints throughout |
| **Maximum Reach** | **[450 mm]** | From base center to wrist flange |
| **Max Payload** | **[500 g]** | At full horizontal extension |
| **Primary Actuators** | **[NEMA 17 Steppers & MG996R Servos]** | Closed-loop / Open-loop |
| **Structural Material** | **[PLA+ / PETG / Aluminum Extrusion]** | Recommended minimum 30% infill |
| **Total Weight** | **[1.8 kg]** | Including motors and fasteners |

---

## 📂 Repository Structure

```text
├── CAD/
│   ├── Source/             # Native CAD files (.f3d, .sldprt, .iam)
│   ├── STEP/               # Universal CAD export (.step / .stp)
│   └── Drawings/           # 2D engineering drawings and tolerances (.pdf)
├── Production/
│   ├── STL/                # High-resolution meshes ready for slicing (.stl)
│   └── 3MF/                # Pre-oriented manufacturing files (.3mf)
├── Docs/
│   ├── Assembly_Guide.md   # Step-by-step mechanical assembly instructions
│   └── Schematics/         # Wiring diagrams and motor pinouts
├── URDF/                   # Unified Robot Description Format for ROS/Gazebo simulation
├── BOM.md                  # Detailed Bill of Materials
└── README.md
