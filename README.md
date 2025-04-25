# Road Lane Detection using Computer Vision

This project explores road lane detection from dashcam video using two approaches:

1. **Classical image processing** (thresholding, morphological operations)
2. **Pre-trained deep learning models** (e.g. YOLOv5 or segmentation networks)

The goal is to compare the robustness of both pipelines and explore optional Model Predictive Control integration, where lane estimation dynamically updates lateral constraint boundaries.

## Relation to Previous Work:

This project builds upon my prior MPC work, available here:  
[Model Predictive Control for a Pneumatic Artificial Muscle](https://github.com/leonardmiksa1/Model-Predictive-Control)

While the controlled system is different, the MPC structure is fundamentally the same:
- In both cases, the **main state of interest is displacement** (actuator extension vs. vehicle lane offset)
- The only significant change is the state-space model used:
  - Pneumatic actuator dynamics for the PAM
  - Vehicle lateral dynamics for this project

This allows me to apply the same MPC logic to a completely different context — robotic exoskeleton vs. lane-keeping vehicle.

> *Project currently in development.*
