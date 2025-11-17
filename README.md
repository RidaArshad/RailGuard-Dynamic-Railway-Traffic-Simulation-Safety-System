# 🚉 Dynamic–AI Rail Signalling

![Status](https://img.shields.io/badge/Status-Ongoing-blue)
![Python](https://img.shields.io/badge/Python-3.10%2B-yellow)
![Frontend](https://img.shields.io/badge/Frontend-HTML%2C%20CSS%2C%20JS-orange)
![AI](https://img.shields.io/badge/AI%20Module-Enabled-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

### **AI-Powered Railway Signalling and Platform Management System**  
_Reimagining train operations with adaptive signalling, real-time intelligence, and automated station assistance._

---

## 🧭 Overview

**Dynamic–AI Rail Signalling** is an ongoing research-driven project that integrates **Artificial Intelligence (AI)** with **Dynamic Moving Block Signalling** to revolutionize railway operations and enhance safety, speed, and efficiency.

## Key Challenges in Conventional Railway Operations

### Manual Decision-Making
- Highly subjective and slow response times, prone to human error.

### Fixed-Block Signalling
- Poor track utilization and inflexible block lengths, causing delays.

### Passenger-Freight Conflicts
- Congestion and scheduling inefficiencies reduce overall throughput.

### Rigid Safety Margins
- Overly conservative spacing reduces train density and network capacity.

### Optimized Operations (Goal)
- Addressing these challenges enables increased capacity, higher safety, and improved service quality.


<img width="1813" height="832" alt="Screenshot 2025-10-10 152458" src="https://github.com/user-attachments/assets/9f11cf7e-535d-4c4b-93a3-d58a9eb5b0a9" />
<img width="1812" height="833" alt="Screenshot 2025-10-10 152405" src="https://github.com/user-attachments/assets/9ee7db94-3eed-4fe4-859a-84a9c50722f1" />

# Our Solution: AI-Powered Junction & Mainline Management

## AI-Powered Junction Management
- **A* Pathfinding Engine:** Calculates optimal real-time routes for trains.  
- **Intelligent Train Prioritization:** Dynamically prioritizes trains based on operational characteristics.  
- **Intelligent Routing:** Efficiently manages passenger and goods train movement.  
- **Conflict-Free Allocation:** Ensures safe, collision-free operations at busy junctions.  
- **AI-Driven Suggestions:** Provides actionable guidance to station masters in real time.  

## Dynamic Moving Block for Mainline
- **Dynamic Moving Block Concept:** Replaces rigid blocks with AI-driven adaptive spacing.  
- **Safety Block Concept:** Real-time moving safety blocks adjust to train speed and braking distance.  
- **Closer Yet Safer Spacing:** Enables higher train density without compromising safety.  
- **Maximized Track Utilization:** Increases track capacity and throughput.  
- **Throughput Boost:** Minimizes delays and enhances overall mainline efficiency.

  
<img width="1234" height="625" alt="Screenshot 2025-09-25 103124" src="https://github.com/user-attachments/assets/b0592d7a-0158-4d66-9e1f-a0dacbb7f51d" />
<img width="1233" height="622" alt="Screenshot 2025-09-25 103143" src="https://github.com/user-attachments/assets/ea60e7dc-ab7b-4cde-a2d5-c5b010fba252" />


This project overcomes that limitation by implementing **Dynamic Moving Blocks**, where block lengths vary continuously in real time based on:
- Train **speed**
- **Braking distance**
- **Track occupancy**
- **Congestion level**

The system also introduces an **AI Decision Support Engine** that assists **Station Masters** by offering intelligent recommendations for:
- 🚉 Platform allotment  
- 🚦 Signal control decisions  
- 🕒 Train sequencing and prioritization  
- ⚡ Conflict resolution during high traffic  

---

## 🚀 Key Features

🟦 1. Real-time Train Simulation
1-second tick engine
+10 km/h acceleration per tick
Continuous speed-limit recalculation
Accurate longitudinal motion using physics equations
🟥 2. Braking Envelope & Safety Simulation
Computes braking distance using ( v^2 / 2a )
Adds fixed 200 m safety buffer
Calculates dynamic safe speed for every train
Automatic bubble-breach detection
Emergency braking triggers
🟩 3. Dynamic Block Control
Each track edge gets inflated time cost (9999) when occupied
A* naturally avoids occupied segments
Ensures conflict-free routing without manual detection
🟧 4. Interactive Frontend (Browser UI)
Dynamic simulation view
Train markers
Speed indicators
Route visualization
Safety bubble warnings
🟪 5. Backend (Flask)
Real-time state management
Thread-safe locks for train updates
REST endpoints for:
Fetching simulation state
Resetting simulation
Dispatching trains
📁 Project Structure
RailGuard/
│
├── Dynamic/
│   ├── app.py
│   ├── dynamic_simulation.html
│   │
│   ├── static/
│   │   ├── css/
│   │   │   ├── style.css
│   │   │   ├── style.css (login version)
│   │   │
│   │   ├── js/
│   │   │   ├── simulation.js
│   │   │   ├── script.js
│   │   │   ├── simulation.js (login version)
│   │   │
│   │   └── videos/
│   │       └── train.mp4
│   │
│   ├── templates/
│   │   └── index.html
│   │
│   ├── fixed_simulation.html
│   ├── TestingTracks2.json
│   └── TestRailway2.html
│
├── login/
│   ├── index.html
│   ├── style.css
│   └── images/
│       └── background.jpg
│
└── README.md
✔ This matches your GitHub Desktop screenshot exactly.
✔ No missing files.
✔ No extra folders.

▶️ How to Run RailGuard
1️⃣ Install dependencies
pip install flask networkx
2️⃣ Run the backend
python app.py
3️⃣ Open the browser
http://127.0.0.1:5000/
⚙️ Core Technologies
Python (Flask)
HTML, CSS, JavaScript
NetworkX (track graph modelling)
Threading (real-time simulation)
Physics-based braking model
A pathfinding*
⭐ Purpose of RailGuard
RailGuard is designed as:

a digital twin for railway movement
a research prototype for moving-block signalling
a visualization of braking envelopes
a conflict-free routing demonstration
a portfolio project showcasing simulation + backend + frontend engineering
It helps understand modern traffic supervision concepts such as:

ETCS Level 3 / CBTC
continuous monitoring
safe-speed determination
headway optimisation
📌 Notes
Some browser animations use video overlays.
Large file sizes (videos, images) require uploading via GitHub Desktop (not website).
App is built for demonstration — not an official signalling tool.
📜 License
This project is open for learning and research use.




---

## 🧩 Project Structure

<img width="1052" height="470" alt="image" src="https://github.com/user-attachments/assets/da7239a4-df05-49e7-bb5c-e0e5b04104ff" />


## Prototype

![WhatsApp Image 2025-10-06 at 11 48 23_e44f493d](https://github.com/user-attachments/assets/d0c0b1f5-760c-4a3d-9d0d-5a0fe807de89)

![WhatsApp Image 2025-10-06 at 11 48 22_6eb3f815](https://github.com/user-attachments/assets/c6a26f76-5a7e-43e5-82ec-bad7ac692ec1)

![WhatsApp Image 2025-10-06 at 11 48 21_f6111105](https://github.com/user-attachments/assets/6c9f24cd-90ba-4342-8763-e1b05bf583ba)

![WhatsApp Image 2025-10-06 at 11 48 23_ad850aed](https://github.com/user-attachments/assets/15d95e2a-a176-4a13-8de7-abac17491904)


