---
layout: single
title: "UNC Real Time Systems Group — EV battery simulation"
excerpt: "+2% battery lifespan by integrating LSTM driving models."
thumb: /assets/images/headshot.jpg
weight: 5
permalink: /projects/unc-rtsg/
---

Link to Github coming soon!
[![Read the Report](https://img.shields.io/badge/Read_Paper-FF6F61?style=for-the-badge)](/assets/docs/Driving_Pattern_Prediction_for_the_Optimization_of_Wear_Leveling_Aware_Cell_Balancing.pdf)

# Goal
The goal of this project is to extend the lifespan of **electric vehicle (EV) batteries** by optimizing wear level-aware cell balancing. Traditional active balancing transfers charge between cells during idle periods but accelerates aging due to frequent transfers. This work explores predictive strategies that anticipate **future driving missions**, enabling smarter scheduling of balancing activities that minimize unnecessary wear while ensuring the vehicle remains operational.

# Methodology
## Data Generation
Because real-world EV driving data with the required features was unavailable, we built a **simulated dataset** using a graph-based approach:

- **Graph structure:** Watts–Strogatz digraph with 12 nodes (locations) and degree 4 connectivity  
- **Edges:** Assigned probabilities, random travel durations, and currents  
- **Home/charging station:** Randomly designated node  
- **Driving missions:** Generated as random walks across the graph, alternating between driving and idle states  

This setup allowed us to model realistic driving sequences and their impact on battery behavior.

## Prediction Strategies
We designed both **static** and **dynamic** prediction frameworks to estimate future driving missions.

- **Static Simulation:**  
  - **Average Mission** — derived from 1,000 simulated missions by averaging time and current values  
  - **Most Likely Mission** — path composed of the highest-probability edges  
  - **LSTM Prediction** — trained to predict the next node based on previous *k* nodes, then extended using a shifting strategy  

- **Dynamic Simulation:**  
  Predictions were updated throughout the day. If the predicted next node diverged from the actual trip, the system re-predicted the mission using:  
  - LSTM node-sequence shifting  
  - Recalculated most-likely path  

## Modeling
The core optimization problem was **balancing schedule generation**, where predicted missions informed when and how balancing occurred.  
We simulated multiple scenarios and measured:  
- **Battery lifespan (days until failure)**  
- **Error margin (deepest dip below charge threshold)**  

# Results
Across 34 six-month simulations:  

- All predictive strategies **extended battery lifespan by ~100 days** compared to no balancing  
- **LSTM-based predictions** and **most-likely missions** showed the best trade-off between extending lifespan and avoiding charge dips  
- Results highlight the balance between **longevity** and **risk of error**, which can be further mitigated by adjusting thresholds  

![Battery Lifespan](assets/images/battery_lifespan.png)  
*Simulation results comparing lifespan across balancing strategies.*

![Charge Error](assets/images/simulation_error.png)  
*Maximum charge dips below safe threshold for each method.*

# Future Work
- **Real-world data integration:** Collect trip and charging behavior from EV users to refine graph models  
- **Simpler modeling:** Explore using simpler models such as Markov models as they may better fit our use case
- **Adaptive mission length:** Remove the assumption of knowing daily mission length in advance  
- **Scenario generation:** Develop algorithms to create varied, realistic test graphs  
