# A07 – AoI vs PLP Analysis in IIoT Networks

## Overview

The goal of this assignment was to analyze how different network conditions affect the trade-off between data freshness and reliability in an IIoT system.

Two key metrics were used:

- **Age of Information (AoI):** measures how fresh the data is  
- **Packet Loss Probability (PLP):** measures how reliable the communication is  

The main idea is that improving one of these usually makes the other worse, so the system needs to be balanced.

---

## Problem

In IIoT systems, devices constantly send updates over a shared network.

The challenge is:
- Sending updates more frequently improves freshness (lower AoI)
- But too many transmissions cause collisions, increasing packet loss (higher PLP)

So the goal was to understand how different factors impact this trade-off.

---

## Approach

The analysis included:

- Exploring key variables:
  - Transmission probability  
  - Number of nodes  
  - Channel quality  
  - Capture threshold  

- Applying feature engineering:
  - Created **network load** feature (combining nodes + transmission rate)  
  - Added interaction and non-linear features  

- Building models:
  - Random Forest model (baseline)
  - Deep learning model (multi-output prediction for AoI and PLP)

---

## Results

- Random Forest model achieved:
  - R² ≈ 0.27 for AoI  

- Deep Learning model achieved:
  - R² ≈ 0.34 for AoI  
  - R² ≈ 0.78 for PLP  

The deep learning model performed better overall, especially for PLP, because it was able to capture more complex relationships.

---

## What I Learned

This assignment showed that IIoT systems are highly interconnected, and variables do not work independently.

Some key takeaways:

- Increasing transmission rate improves AoI but increases collisions  
- More nodes increase congestion and worsen performance  
- Feature engineering is critical for representing real system behavior  
- Predicting AoI and PLP together gives better results  

---

## Challenges

- Understanding interactions between multiple network variables  
- Representing system behavior using features  
- Improving model performance beyond basic inputs  

---

## Real-World Relevance

This type of analysis is important in systems such as:

- Smart factories  
- Healthcare monitoring systems  
- Sensor networks  

These systems need data that is both:
- **fast (fresh)**  
- **reliable**

---

## Conclusion

This assignment showed that optimizing IIoT systems is not just about improving one metric. It requires balancing multiple factors and understanding how they interact.

It also showed that combining feature engineering with more advanced models can significantly improve results.
