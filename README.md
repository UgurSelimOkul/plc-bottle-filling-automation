# 🏭 Industrial Bottle Filling & Packaging Automation

**An end-to-end industrial automation project designed for a 6-bottle filling, capping, and packaging line.**

This project encompasses the complete engineering lifecycle: from mechanical 3D design and cost analysis to system architecture using **Siemens S7-1200 PLC** and **TIA Portal**.

---

## 📖 Table of Contents
1. [Project Overview](#-project-overview)
2. [System Architecture](#-system-architecture)
3. [Hardware & Components](#-hardware--components)
4. [Process Flow](#-process-flow)
5. [3D Design & Mechanical Layout](#-3d-design--mechanical-layout)
6. [Technical Documentation](#-technical-documentation)
7. [Budget Analysis](#-budget-analysis)

---

## 🎯 Project Overview

The goal of this project is to automate the liquid filling and packaging process to increase efficiency, hygiene, and traceability in industrial sectors such as food, beverage, and pharmaceuticals.

**Key Features:**
* **Dual Conveyor System:** Continuous flow management.
* **Station-Based Processing:** Filling, Capping, and Wrapping stations.
* **Smart Sensing:** IR/Optical sensors for precise positioning and counting.
* **Human-Machine Collaboration:** Semi-automatic design allowing operator intervention for quality control.

---

## ⚙️ System Architecture

The system operates on a cyclic logic controlled by a **Siemens S7-1214C PLC**.

1.  **Input Stage:** Empty bottles are fed into Conveyor 1 and counted (Batch size: 6).
2.  **Filling Station:** Bottles are clamped, and the filling robot dispenses liquid (Time-controlled).
3.  **Capping Station:** Caps are placed and tightened using a rotary actuator.
4.  **Transfer:** Operators inspect and move bottles to Conveyor 2.
5.  **Wrapping Station:** Bottles are detected, wrapped with stretch film, and counted as a finished package.

---

## 🛠 Hardware & Components

| Component | Quantity | Function |
| :--- | :--- | :--- |
| **PLC** | 1 | Siemens S7-1214C DC/DC/DC |
| **Expansion Module** | 2 | SM1222 – 16 DO Module |
| **HMI** | 1 | Siemens HMI Panel |
| **Servo Motors** | 18 | Siemens V90 (Conveyors & Robotic Arms) |
| **Sensors** | 4 | Sick GRL18S (Reflective Optical Sensor) |
| **Contactors** | 18 | Siemens 3TF40-10 |

---

## 🔄 Process Flow

The automation logic is time-window based, ensuring synchronized operations without complex interlocks.

* **T = 0-2s:** Gripper arms lock the bottles.
* **T = 2-4s:** Robot arm descends.
* **T = 4-8s:** Process execution (Filling / Capping / Wrapping).
* **T = 8-10s:** Robot arm ascends.
* **T = 10-12s:** Grippers release, conveyor moves.

---

## 🎨 3D Design & Mechanical Layout

The physical layout was modeled to ensure ergonomic operation and spatial efficiency.

### System Overview (Isometric View)
![Isometric Main](3D-Design/isometric-view-main.jpg)

### Front View
![Front View](3D-Design/front-view.jpg)

### Top View (Layout)
![Top View](3D-Design/top-view.jpg)

### Additional Angles
| Angle 1 | Angle 2 |
| :---: | :---: |
| ![Left 1](3D-Design/isometric-view-left-1.jpg) | ![Left 2](3D-Design/isometric-view-left-2.jpg) |

---

## 📄 Technical Documentation

Detailed wiring diagrams, power circuit schematics, and PLC ladder logic diagrams are available in the full project report attached to this repository.

**The full report includes:**
* Detailed PLC Logic & Algorithms (LAD)
* Electrical Power Circuit Diagrams
* I/O Wiring Schematics

📥 **[Download Full Project Report (DOCX)](project-report.docx)**

---

## 💰 Budget Analysis

A comprehensive cost analysis was conducted for industrial feasibility.

| Item | Total Cost (Est.) |
| :--- | :--- |
| **PLC & Modules** | 33,600 TL |
| **HMI Panel** | 83,000 TL |
| **Servo Motors (x18)** | 248,400 TL |
| **Total System Cost** | **~415,638 TL** |

---

### 👨‍💻 Author
**Uğur Selim Okul**
*Electrical & Electronics Engineering Student*
* [GitHub Profile](https://github.com/UgurSelimOkul)
