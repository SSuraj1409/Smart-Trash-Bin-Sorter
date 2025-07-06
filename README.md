<h1 align="center">🔌 Smart Trash Bin Sorter</h1>
<p align="center"><i>A group project combining machine learning and Arduino hardware for automated waste classification</i></p>

---
## ♻️ Introduction

Waste is a major contributor to climate change due to the greenhouse gases emitted during its decomposition and handling. While recycling was introduced to reduce this impact by sorting and reprocessing reusable materials, many regions still struggle with poor recycling practices due to lack of infrastructure and awareness.

To address this challenge, our team at **JARCS Inc.** developed the **Smart Trash Bin Sorter**, an automated system that classifies waste as either **Recyclable** or **Biodegradable**. This intelligent solution eliminates the need for manual sorting in recycling facilities, thereby reducing operational costs and promoting environmentally responsible waste management.

The system is built within a **cuboid-shaped enclosure** and features a platform where users can place an item of trash. A **camera mounted on the front** scans the object using a **custom-trained Machine Learning model** developed with **Google Teachable Machine**. Based on the model's prediction, the trash is categorized as either recyclable or biodegradable.

Once classified:
- A **rotating cylinder mechanism** aligns with the appropriate internal bin.
- Two **automated push flaps** then guide the trash into the selected compartment.

The status of the machine is communicated using:
- **LED indicators**:
  - 🟥 **Red** – Resetting to default position  
  - 🟦 **Blue** – Processing the item  
  - 🟩 **Green** – Ready for next input
- An **LCD display** that provides real-time feedback on the system's current state.

This solution enhances efficiency and encourages cleaner waste separation at the source — directly where disposal happens — making recycling more accessible, automatic, and effective.

---

## 🙋‍♂️ My Contribution – Suraj Srinivasan

I was in charge of the **Teachable Machine integration** and **Python programming**. These components were the fastest to be completed, allowing me to contribute further by:

- Assisting in the **physical assembly and wiring**
- Supporting **Arduino code troubleshooting**
- Helping with **overall system integration and testing**

---

## 👥 Team Members

- AV J. Madrigalejos  
- Chris Edappady 
- Suraj Srinivasan 
- Joan John Mbunda

## 🛠️ PROGRAM AND CROSS-INTEGRATIONS

In this project, we utilized three different programs to allow the machine to perform its task effectively: **Teachable Machine by Google**, **Python**, and **Arduino**.

**Teachable Machine** is the analyzing tool in our machine. It examines the image of the trash item and determines whether it falls into the category of **Recyclable** or **Biodegradable**. Once classified, the result is displayed in the browser and picked up by the Python program.

The **Python program** continuously monitors the classification output from Teachable Machine and acts as a **communication bridge** between the web-based machine learning model and the Arduino microcontroller. It reads the classification result and sends the appropriate command through serial communication.

**Arduino** receives the command sent from Python and executes the corresponding action. This involves rotating the internal cylinder to the correct bin section and activating push flaps to dispose of the item into the appropriate compartment.

<div align="center">
<img src="https://i.imgur.com/Ls6KMM5.png" alt="Home page after logging in"/>
</div>

All three components work together in real-time to deliver fast, accurate, and automated waste sorting — without the need for any manual input.

---



## 📺 Project Demo
[![Watch the Demo](https://i.imgur.com/WHi7U0s.png)](https://youtu.be/EZBboQ9rwXk)




---

## 🖼️ System Flow Diagram

