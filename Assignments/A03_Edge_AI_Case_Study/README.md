# A03 – Edge AI Case Study (Smart Traffic Monitoring)

## Overview

The goal of this assignment was to analyze a real-world edge AI system used for traffic monitoring. The case study focused on a smart city project that used edge computing and video analytics to track pedestrians, vehicles, and cyclists in real time.

The system used existing CCTV cameras and processed data locally to reduce latency and improve privacy.

---

## Problem

Modern cities face challenges such as:
- Increasing traffic congestion  
- Growing population density  
- Need for real-time data for urban planning  

Traditional systems rely heavily on cloud processing, which can introduce delays and raise privacy concerns.

---

## Approach

The system used edge computing to process video data directly on local devices instead of sending everything to the cloud.

Key components included:

- **Hardware:** NVIDIA Jetson TX2  
- **Model:** YOLOv3 (object detection)  
- **Tracking:** SORT algorithm  
- **Network:** LoRaWAN for communication  

The system detected and tracked:
- Pedestrians  
- Vehicles  
- Cyclists  

All processing was done locally, and only metadata (not raw video) was transmitted.

---

## Results

- Achieved around **69% detection accuracy**  
- Processed video at approximately **20 frames per second**  
- Maintained stable system performance under real-world conditions  

However, performance dropped in crowded environments due to object occlusion.

---

## Lesson to be Learned

This assignment helps one understand how AI systems are deployed in real-world environments.

Some key takeaways:

- Edge computing reduces latency and improves privacy  
- Real-world performance is often limited by environmental conditions  
- Hardware constraints play a big role in system design  
- AI systems must balance accuracy, speed, and resource usage  

---

## Challenges

- Understanding how different system components work together  
- Interpreting performance results in a real-world context  
- Connecting theoretical models to practical deployment  

---

## Real-World Relevance

This type of system can be used for:

- Urban planning  
- Traffic management  
- Pedestrian safety  
- Smart city development  

It shows how AI can be integrated into existing infrastructure without requiring major upgrades.

---

## Conclusion

This case study demonstrated how edge AI can be used to solve real-world problems efficiently.

It highlighted the importance of system design, hardware selection, and privacy considerations when deploying AI solutions.
