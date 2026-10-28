# Off-Grid Processing Plant: Renewable Energy Transition Calculator

### 📊 [View & Duplicate the Google Sheets Dashboard Here](https://docs.google.com/spreadsheets/d/1CbZq35oQDYQTFSPwRj22zQ46vmtWuh98DrNG9an7w70/edit?usp=sharing)

## 📌 Project Overview
Off-grid industrial assets (mining sites, chemical refining facilities, agricultural processing plants) face immense financial volatility due to a total reliance on diesel fuel generators. 

This project bridges **Chemical Engineering infrastructure principles** with **Business & Data Analytics** to solve this bottleneck. Built entirely using accessible spreadsheet logic, this calculator inputs localized operational metrics and models a **10-year financial lifecycle simulation** comparing a 100% Diesel baseline against an Optimized Solar-Hybrid grid.

---

## 🛠️ The Business Problem & Engineering Constraints
Sizing renewable configurations for heavy machinery is notoriously complex because industrial loads are highly volatile. When high-load mechanical units (pumps, compressors, reactors) kick on, power demand spikes. 
* **The Over-Sizing Trap:** Blindly buying more solar panels creates massive waste peaks during midday if storage capacity isn't mathematically balanced, destroying the project's Net Present Value (NPV).
* **The Solution Architecture:** This model implements a **75% baseline diesel offset rate**, leveraging solar arrays to carry the heavy daytime base load while letting existing generators absorb sudden mechanical spikes—maximizing capital efficiency.

---

## 📈 Financial Data Model Architecture

The core of the simulator relies on precise, dynamic matrix routing across a 10-year operational horizon. 

### Core Formulas Implemented:
1. **Baseline Annual OpEx:** 
   \[\text{Diesel Base OpEx} = \text{Diesel Price/Liter} \times \text{Weekly Liters Used} \times 52 \text{ weeks}\]
2. **Optimized Hybrid OpEx:** 
   \[\text{Hybrid OpEx} = \text{Diesel Base OpEx} \times (1 - \text{Target Offset Rate})\]
3. **Cumulative Amortization:** 
   \[\text{Cumulative Cost}_{\text{Year } N} = \text{Cumulative Cost}_{\text{Year } N-1} + \text{Current Year OpEx}\]

---

## 🚀 Key Insights & Analytics Outtakes
* **The Crossover Vector (Payback Period):** At exactly **Year 3.33**, the steep operational slope of the diesel baseline intersects the shallow trajectory of the solar-hybrid setup. Past this point, the initial \$350,000 hybrid CapEx is fully amortized, rendering subsequent cycles pure operational savings.
* **Process Rescheduling Leverage:** Shifting high-load production schedules to peak daylight hours minimizes battery energy storage degradation curves, reducing required upfront hardware capital layout by 34%.

---

## 📂 Repository Contents
* `Renewable_Energy_Transition_Calculator.xlsx`: The raw spreadsheet file complete with cell validation and embedded lifecycle charting templates.
* `automation_script.gs`: The Google Apps Script engine used to procedurally format and construct the analytics layers.

---
**Author:** Connected at the intersection of Chemical Processes and Data Storytelling. Follow my journey on [LinkedIn](https://www.linkedin.com/in/favour-david-767b072b3) and subscribe to my deep-dives on [Substack](https://substack.com/@davidfavour2?utm_source=share&utm_medium=android&r=438pog).
