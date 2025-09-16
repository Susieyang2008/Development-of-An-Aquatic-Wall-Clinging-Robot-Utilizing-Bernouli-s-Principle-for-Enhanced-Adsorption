# Aquatic Wall-Clinging Robot with Photogrammetry Capability  

## Overview  
This repository documents the design, development, and testing of a small **underwater wall-clinging robot** that uses **Bernoulli’s principle for negative pressure adsorption** and is capable of capturing images for **3D photogrammetric modeling**.  

The project was developed to address challenges in underwater inspection, pipeline maintenance, and marine research, where traditional ROVs often face instability, limited mobility, and insufficient imaging capabilities.  

Key innovations include:  
- **Negative pressure adhesion system** based on Bernoulli’s principle  
- **Remote-controlled thrusters, wheels, and propellers** for wall-clinging and omnidirectional movement  
- **Integrated ESP32-CAM module** for systematic image capture  
- **Photogrammetry pipeline** to reconstruct 3D models from overlapping underwater images  
- **Iterative hardware improvements** across first and second-generation prototypes  

---

## Features  
- **Adhesion Mechanism**: Negative pressure adsorption using ROV thrusters and acrylic plates.  
- **Mobility**: Rubber wheels with friction patterns and multiple propellers for rotation and angular control (60°–300° range).  
- **Imaging**: ESP32-CAM with waterproof casing, flashlight for illumination, and SD card storage.  
- **Control**: Arduino Mega2560 + HC-12 Bluetooth module, with a self-built PS2 joystick remote.  
- **Sensors**: Humidity sensor and buzzer for leak detection, MPU6050 gyroscope for balance.  
- **Waterproofing**: Dual protective casing with rubber seals and reinforced screw system.  

---

## Results  
- **Clinging & Movement**: Stable adhesion achieved on smooth and rough underwater surfaces.  
- **Rotation & Accuracy**: Improved from 83.79% (1st gen) to **84.72%** (2nd gen).  
- **Force Testing**: Withstood **12.0N (plane)** and **11.0N (side)** tension while adhered.  
- **Photogrammetry Tests**: Successful 3D alignment on patterned objects (e.g., keyboard), though limited by reflections, low camera resolution, and lighting conditions.  

---

## Project Structure  
- **docs** – Research paper and poster (PDFs).  
- **hardware** – CAD designs, component diagrams, and schematics.  
- **software** – Arduino code for robot and controller.  
- **tests** – Experiment data (tension, waterproofing, rotation, movement, photogrammetry).  

---

## Installation & Usage  
1. Upload Arduino code from `/software` to **Arduino Mega2560**.  
2. Connect hardware components (ROV thrusters, motors, ESP32-CAM, sensors).  
3. Power the robot and operate using the custom PS2 remote.  
4. For photogrammetry, capture overlapping images and process with **Agisoft Metashape** or similar software.  

---

## Future Work  
- Upgrade to **higher-resolution cameras** for sharper image reconstruction.  
- Implement **diffused lighting strategies** to reduce underwater reflections.  
- Add **AI/ML integration** for automated crack detection and adaptive navigation.  
- Explore **robotic arm attachments** for underwater maintenance tasks.  
- Enhance **waterproofing** and **battery replacement efficiency**.  

---

## References  
- Yang, C. *Development of an Aquatic Wall-Clinging Robot with Photogrammetry Capability*. 2025.  
- Yang, C. *ISEF Poster – Development of an Aquatic Wall-Clinging Robot Utilizing Bernoulli’s Principle for Enhanced Adsorption*. 2025.  

---

## License  
MIT License – see [LICENSE](LICENSE) for details.  
