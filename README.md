# Alertix – Traffic Orchestration Engine (TOE) 🚑🚦

## 📌 Overview

This repository contains the **Traffic Orchestration Engine (TOE)** developed as part of *Alertix*, a smart emergency response system built during a **24-hour hackathon – InnovateYou at AISSMS**.

Alertix aims to **reduce emergency response time** during road accidents and SOS situations by eliminating delays in detection, dispatch, and transportation.

---

## 🚨 Problem Statement

Emergency response systems today suffer from:

- Delayed accident reporting  
- Manual ambulance dispatch  
- Traffic congestion blocking emergency vehicles  
- Lack of real-time coordination  

These inefficiencies directly impact **life-saving response time**.

---

## 💡 Our Solution – Alertix

We developed **Alertix**, a system that:

- Detects accidents and triggers alerts  
- Automatically assigns the nearest ambulance  
- Eliminates manual dispatch delays  
- Tracks ambulance movement in real-time  

---

## 🚦 My Contribution – Traffic Orchestration Engine (TOE)

Developed by:

- Latika Ray  
- Gauri Dere  

### 🎯 Purpose

While Alertix handled detection and dispatch, our mentor emphasized that:

> **Traffic congestion is the biggest real-world bottleneck in emergency response.**

To solve this, we designed the **Traffic Orchestration Engine (TOE)**.

---

## ⚙️ How TOE Works

### 1️⃣ Ambulance Assignment

- System searches for nearest ambulance:
  - First within **5 km**
  - Then expands to **10 km**, and so on  
- Automatically assigns driver  

---

### 2️⃣ Route Optimization

- Identifies **best possible route**  
- Uses **A*-like pathfinding algorithm**  
- Integrates map APIs (Overleaf API used for simulation)  

---

### 3️⃣ Smart Signal Control 🚦

TOE dynamically controls traffic signals:

- **S1 (First Signal)** → Turns Green normally  
- **S2** → Skips Yellow (Red → Green directly)  
- **S3 onwards** → Skips both Red & Yellow → Immediate Green  

👉 This staged approach:

- Prevents sudden chaos  
- Gradually clears traffic  
- Builds a smooth **Green Corridor**  

---

### 4️⃣ Vehicle Alert System 📢

Simultaneously sends alerts to nearby vehicles:

> "Ambulance at 500m – Please MOVE LEFT!"

This ensures:

- Lane clearance  
- Faster ambulance movement  
- Reduced human reaction delay  

---

### 5️⃣ Continuous Monitoring

- Tracks ambulance in real-time  
- Adjusts signals dynamically  
- Reassigns ambulance if driver unavailable  

---

### 6️⃣ Route Completion

- Once destination is reached:
  - Signals revert to normal  
- Same process applies for return journey  

---

## 🧠 System Responsibility Split

| Module          | Responsibility                                         |
|----------------|------------------------------------------------------|
| Alertix         | Detection, alerting, ambulance dispatch              |
| TOE (This Repo) | Traffic management, route optimization, green corridor |

---

## ⚠️ Simulation Note

- This implementation is a **simulation**  
- Real-world execution requires:
  - Smart traffic signal infrastructure  
  - Smart city APIs  

Despite limitations, this demonstrates a **scalable real-world solution**.

---

## 🛠️ Tech Stack

- Vanilla JavaScript (Simulation)  
- Map API (Overleaf-based)  
- A*-like Algorithm (Pathfinding)  

---

## 🏁 Impact

- Reduces ambulance delay significantly  
- Eliminates manual intervention  
- Introduces intelligent traffic control  
- Addresses a **critical life-and-death problem**  

---

## 🔗 Original Project

Full project repository:  
https://github.com/shantanuvhanmore/alertix

---

## ⚠️ Disclaimer

This repository contains only the **Traffic Orchestration Engine module** developed by me and @Gauri Dere during the hackathon.

All credits to the team for the complete system.
## 👥 Team Members

- **[Latika Ray](https://github.com/latikaray)** – Traffic Orchestration Engine (TOE)  
- **[Gauri Dere](https://github.com/)** – Traffic Orchestration Engine (TOE)  
- **[Shantanu Vhanmore](https://github.com/shantanuvhanmore)** – Core Development, Guidance in TOE  
- **[Bhagyashree](https://github.com/)** – API, Testing, Documentation  

