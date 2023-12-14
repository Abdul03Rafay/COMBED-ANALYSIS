# COMBED-ANALYSIS

---

### **RUST GRAPHICAL ANALYSIS IMPLEMENTATION PROJECT**

**DS 210 /  NOV - DEC 2023 / ABDUL RAFAY** 

---

**DATA SET OF CHOICE : Commercial Building Energy Dataset (COMBED)**

> [https://combed.github.io/](https://combed.github.io/)
> 

---

**GOAL OF THE PROJECT :**  Implement graphical analysis using RUST to deduce insights on various energy consumption parameters’ relationship in the context of well documented academic research building.

---

******WHY COMBED? → real world relevance, detailed energy consumption patterns and research paper context.******

Upon short listing the links containing various datasets, I was interested in seeing what, COMBED a commercial building energy dataset contained. It’s description was interesting, with dataset demonstrating some unique qualities, hence why I decided to include it. 

- COMBED is the first of it’s kind energy dataset, where commercial building energy data was sampled more than once per minute. → high frequency sampling, suitable for implementing higher grid separation which requires large dataset.
- There are **200 smart meters** recording various power related parameters every 30 seconds, in **IIITD’s academic building**. → smart meters, potentially can provide us with rich data with multiple dimensions of data. Also the academic setting of the building could yield interesting insights related to energy consumptions in academic settings.
- The meters are Schneider electric based and the data collection system consists of RaspberryPi based controller and sMAP for data visualization and archiving. → another technical hint of how versatile and richly the data is collected.
- On top of that there were some other perks, such as their entire analysis scripts being **open sourc**e and accessible on **Github**, potentially providing us with tools for much more in-depth analysis of our interest. → open Github dataset, a valuable resource which could potentially become foundation for my data analysis.
- Also, COMBED was released as a part of following paper : **A comparison of non-intrusive load monitoring methods for commercial and residential buildings** Nipun Batra, Oliver Parson, Mario Berges, Amarjeet Singh, Alex Rogers. → the fact that the dataset was published with research paper, adds further credibility to the dataset, on which we can build on top for analysis according to our goals.

So, overall the versatility and tools provided with the dataset, which allows to explore various aspects of energy consumption in a academic setting, became my main reason in choosing this dataset. I’m pretty hopeful in potentially finding trends, relationships between parameters or anomalies in the context of energy consumption of academic building.

---

**INSIGHTS OF INTEREST:** 

- Identify peak energy consumption periods.
- **Explore the relationships between different meters and power parameters.**
- Investigate patterns in energy consumption associated with specific building systems or areas.
- Assess the overall energy efficiency of the academic building.
- Try to find a relationship if present between 200 meters.

---

******************************IMPLEMENTATION:******************************

→ **DATA LOADING/PREPROCESSING**

- Confirm successful loading and explore sample of data to understand it’s structure.
- RUST libraries : `csv`, `serde`, etc

→ **GRAPHICAL REPRESENTATION**

- Define graph structure representing meters and power parameters.
    - define `enum` or `struct` to represent graph strcuture.
- Verify graph aligns with dataset.

→ **GRAPH ALGORITHM MODIFICATIONS (GRID SEARCH)**

- Modify graph’s algorithm to find paths with in (e.g. 60) steps between any pair of meters or power parameters.
- breadth first search
- sample scenario tests

→ **VISUALIZATION ENHANCEMENTS** 

- colors, path visualizations, labels, etc
- RUST graphic libraries : e.g. `plotters`, `nannou`, etc
- overall visual improvements

→ **AVERAGE DISTANCE CALCULATIONS**

- test with different pairs of connected nodes

→ **INSIGHTS/DOCUMENTATION**

- analyze results gathered so far, to find patterns in energy consumption.
- document findings and explain how grid search implemented on COMBED.

→ **FINAL REVIEW**

- git repository

→ **PROJECT DUE**

Any feedback, especially on implementation tools are appreciated.

> THANK YOU!
> 

---
