# Smart Traffic Management for Ambulance Priority

An AI and IoT-based system to create a "green corridor" for ambulances by automatically detecting the vehicle and its siren, then controlling the traffic signal.

## About
This project, "Smart Traffic Management for Ambulance Priority," is designed to address the critical delays ambulances face at urban intersections. Traditional fixed-timer traffic systems are rigid and cannot adapt to real-time emergencies, leading to increased response times and potential loss of life. Our solution integrates advanced Artificial Intelligence and Internet of Things technologies to create an autonomous system that detects approaching ambulances using a multi-modal approach and dynamically adjusts traffic signals to ensure unimpeded passage. This aims to streamline emergency response and significantly improve patient outcomes.

## Features
- Implements a **multi-modal AI approach** for robust ambulance detection (combining visual and acoustic analysis).
- Utilizes **YOLOv5** for efficient real-time object detection of ambulances in video streams.
- Employs **MFCC + MLP** for accurate siren recognition from audio inputs.
- Features **decision fusion logic** to prevent false positives by requiring dual confirmation (sight + sound).
- Integrates with a **NodeMCU (ESP8266)** microcontroller for real-time traffic signal override via relays.
- Designed for **low-cost and high scalability**, suitable for deployment in urban environments.
- Enhances emergency response by minimizing ambulance transit time at intersections.

## Requirements
* **Operating System:** Requires a 64-bit OS (Windows 10/11 or Ubuntu Linux) for compatibility with deep learning frameworks and real-time processing.
* **Development Environment:** Python 3.9 or later is necessary for coding the AI models and the master fusion script. Arduino IDE is required for NodeMCU programming.
* **Deep Learning Frameworks:** PyTorch (for YOLOv5) and TensorFlow/Keras (for MLP model training) are essential.
* **Image & Audio Processing Libraries:** OpenCV is crucial for efficient video capture and processing, while Librosa is used for advanced audio feature extraction (MFCCs).
* **Version Control:** Git for collaborative development and effective code management.
* **IDE:** VSCode or a similar Integrated Development Environment for coding, debugging, and version control integration.
* **Hardware Dependencies:** Webcam, Microphone, NodeMCU (ESP8266), 4-channel or 8-channel Relay Module, and LEDs/prototype traffic lights for actuation.

## System Architecture
The system's architecture is a multi-modal, three-tier framework designed for real-time edge processing and IoT-based actuation.

![System Architecture Diagram](https://github.com/user-attachments/assets/2f9d3686-5e1c-44f8-9959-5ff2ba101022) 
*(Note: Replace the placeholder image URL with your actual diagram's URL once uploaded to your repo)*

## Output

### Output 1 - Idle State (Monitoring)
This image shows the system's operational dashboard when no ambulance is detected. It represents the "normal operation" state of the intersection, displaying live video feed with system status indicators.



### Output 2 - Detection State (Override Active)
This image illustrates the system's dynamic response during a successful multi-modal detection event. An ambulance is detected visually (YOLOv5 bounding box) and acoustically (siren confirmation), leading to the activation of the "green corridor."

![Detection State Output](Gemini_Generated_Image_b3r2s9b3r2s9b3r2.png) 
*(Note: Replace the placeholder image URL with your actual diagram's URL once uploaded to your repo)*

### Sample Video:
This video demonstrates the real-time functionality of the system, showing the dynamic detection and traffic light override in action.

[https://github.com/user-attachments/assets/2f9d3686-5e1c-44f8-9959-5ff2ba101022](https://github.com/user-attachments/assets/2f9d3686-5e1c-44f8-9959-5ff2ba101022)

## Results and Impact
The "Smart Traffic Management for Ambulance Priority" system significantly enhances emergency response capabilities in urban environments. By accurately and autonomously prioritizing ambulances, it directly contributes to reducing critical transit times, which can lead to improved patient outcomes and a reduction in preventable loss of life. The project's multi-modal AI approach ensures high reliability and minimizes false triggers, making it a practical and trustworthy solution for real-world deployment.

This low-cost, scalable, and reproducible framework serves as a foundational step towards more intelligent and adaptive urban infrastructures. It showcases the immense potential of integrating cutting-edge AI (YOLOv5, MFCC+MLP) with IoT (NodeMCU, relays) to solve critical societal challenges, fostering a safer and more efficient environment for emergency services.

## Articles published / References
1.  M. Usaid, et al., "Ambulance Siren Detection using Artificial Intelligence in Urban Scenarios," *Sir Syed University Research Journal of Engineering & Technology*, vol. 12, no. 1, pp. 92-97, 2022.
2.  S. Amrutasagar, et al., "Enhanced Emergency Response: YOLOv7-Based Ambulance Detection and Distance Estimation," in *Proceedings of the 2024 International Conference on Intelligent Systems and Co-design (ICISC)*, 2024, pp. 1-6.
3.  M. Mohsin, et al., "Automatic Priority Analysis of Emergency Response Systems using Internet of Things (IoT) and Machine Learning (ML)," *Transportation Engineering*, vol. 19, no. 3, 2025.

## Document Link:
[https://docs.google.com/document/d/1UdO7VFjHVId9TRDj_AVljd5JN-Sg7w-w8oKDZ3ip7xk/edit?usp=sharing](https://docs.google.com/document/d/1UdO7VFjHVId9TRDj_AVljd5JN-Sg7w-w8oKDZ3ip7xk/edit?usp=sharing)
