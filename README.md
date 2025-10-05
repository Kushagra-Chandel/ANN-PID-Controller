<h1 align="center">⚡ ANN–PID Controller for DC Motor Speed Control</h1>

<p align="center">
  <b>Comparative Design of Optimal PID vs ANN Controller using MATLAB & Simulink</b><br>
  <img src="https://img.shields.io/badge/MATLAB-Simulink-orange?logo=mathworks" alt="MATLAB">
  <img src="https://img.shields.io/badge/AI-Artificial%20Neural%20Networks-blue" alt="ANN">
  <img src="https://img.shields.io/badge/Control%20Systems-DC%20Motor-green" alt="Control Systems">
</p>

---

## 🧠 Abstract

This project focuses on designing and analyzing a **neural network–based PID controller** to optimize the **speed control of a Brushless DC (BLDC) motor**.  
We develop both a **conventional PID controller** and an **Artificial Neural Network (ANN) controller** in MATLAB–Simulink and evaluate their performance against an ideal reference control model.

> 🟢 ANN-based control significantly reduces **overshoot**, improves **settling time**, and closely follows the ideal response curve — outperforming traditional PID controllers.

---

## 🎯 Motivation & Objective

Conventional linear controllers often struggle with nonlinear, parameter-varying systems like BLDC motors. Neural Networks offer adaptive learning capabilities, allowing controllers to:  
- Learn system dynamics without explicit parameter calculation.  
- Handle non-linearities and disturbances effectively.  
- Adapt to changing motor characteristics during operation.

👉 This work aims to design, train, and evaluate an **ANN-based adaptive controller** and compare its response to a **classical PID** for DC motor speed regulation.

---

## 🧱 Project Outline

1. 📐 Derive the **mathematical models** of BLDC motor and PID controller.  
2. ⚡ Implement a **conventional PID controller** in MATLAB for baseline data collection.  
3. 🧠 Design a **supervised ANN controller** for adaptive control.  
4. 🧪 Train the ANN using **80 % collected data** via back-propagation.  
5. ✅ Test and refine using the remaining dataset until optimal accuracy is achieved.  
6. 🔄 Replace PID with trained ANN in real-time simulation.  
7. 📊 Compare PID vs ANN performance against the reference model.

---

## 🧰 Purpose, Scope & Applicability

### 📝 Purpose
- Replace conventional tuning and sensor dependency with **ANN-based adaptive speed control**.  
- Maintain accurate control even under **parameter variations** or **dynamic loads**.  
- Leverage ANN learning to enhance **response accuracy** and **robustness**.

### 🌐 Scope
- Explore optimal **hidden layer configurations** and **adaptive learning rates**.  
- Investigate ANN’s ability to **self-tune** for real-time motor dynamics.  
- Identify pathways for improving performance during transient states.

### 🚀 Applicability
- Industrial motor control systems  
- Robotics & autonomous systems requiring precise speed regulation  
- Adaptive controllers for non-linear, parameter-varying environments

---

## 🧠 Neural Network Controller Design

- **Architecture**: Feed-forward ANN with two inputs (error & error rate), one output (controller gain), single hidden layer  
- **Training Algorithm**: Backpropagation (Supervised Learning)  
- **Training Data**: PID controlled response logs (80 % train / 20 % test)  
- **Implementation**: MATLAB Neural Network Toolbox & Simulink block integration

<p align="center">
  <img src="https://github.com/Kushagra-Chandel/ANN-PID-Controller/blob/main/assets/architecture.png" alt="ANN Architecture Diagram" width="500">
</p>

---

## 📊 Results & Comparative Analysis

| Parameter              | PID Controller | ANN Controller |
|-------------------------|----------------|----------------|
| Overshoot              | High          | **Low / Eliminated** |
| Settling Time          | Longer        | **Reduced** |
| Steady-State Error     | Moderate     | **Closer to Reference** |
| Adaptability          | Fixed tuning | **Adaptive to variations** |

> The ANN controller shows a **faster response**, **better stability**, and **closer match to the reference model** than the conventional PID controller.

<p align="center">
  <img src="https://github.com/Kushagra-Chandel/ANN-PID-Controller/blob/main/assets/comparison_plot.png" alt="PID vs ANN Graph" width="600">
</p>

---

## 🧠 Tech Stack

- 🧪 **MATLAB & Simulink** – Plant modeling & control simulation  
- 🧠 **Neural Network Toolbox** – ANN controller design & training  
- 📊 **Backpropagation** – Supervised learning algorithm  
- 📝 **Custom Scripts** – Data preprocessing & training automation

---

## 📚 References & Inspiration

- MATLAB Documentation – Neural Network Toolbox  
- Control Systems Engineering by Norman S. Nise  
- Research papers on ANN-based BLDC control systems

---

## 🙏 Acknowledgements

This project was completed under the guidance of mentors & faculty. Special thanks to MATLAB & Simulink resources and documentation that enabled efficient model building and integration.

---

### 👤 Author

### ✅ What This Version Achieves:

* **Research paper + GitHub project** hybrid look
* Recruiter, professor, and developer **sabko samajh aata hai instantly**
* Proper visual structure, icons, and comparison table make it *premium quality*
* Abstract, Motivation, Outline → convey academic clarity
* Architecture diagram & graph placeholders ready (add `.png` to `/assets` folder)

