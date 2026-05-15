# 🚦 Smart Intersection System - Fuzzy Logic

This project is a smart intersection simulation developed using **Fuzzy Logic** in **MATLAB** to prevent the time loss and inefficiency caused by traditional fixed-time traffic lights. The system analyzes the real-time vehicle density at the intersection and dynamically calculates the optimal green light duration.

## 📝 Project Overview
The system takes the vehicle queue waiting at the red light and the current traffic density of the approaching road (which will turn green) as input variables. By utilizing the **Mamdani** fuzzy inference system and the Centroid defuzzification method, it determines the most efficient green light duration (in seconds) for the intersection.

## ⚙️ System Architecture
The model is designed with a **MISO (Multiple-Input Single-Output)** architecture.

* **Input 1 (Queue):** Vehicle density waiting at the red light (0% - 100%)
  * *Membership Functions:* Low, Medium, High
* **Input 2 (Arrival):** Approaching vehicle density on the green light side (0% - 100%)
  * *Membership Functions:* Low, Medium, High
* **Output (Duration):** Green light duration (10 - 60 Seconds)
  * *Membership Functions:* Short, Normal, Long

**Decision Mechanism:** The system operates with 9 specifically defined *IF-THEN* rules to prevent intersection gridlocks and avoid keeping empty roads open unnecessarily.

## 🚀 Installation & Usage

### Requirements
* MATLAB (R2018b or newer recommended)
* Fuzzy Logic Toolbox

### How to Run
1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/your-username/fuzzy-logic-smart-intersection.git](https://github.com/your-username/fuzzy-logic-smart-intersection.git)
