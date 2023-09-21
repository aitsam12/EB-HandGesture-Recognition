# EB-HandGesture-Recognition
This is the code for our submission to ICRA2024.

### Title: Real-time Gesture Recognition with Event Cameras for Enhanced Robot Guidance

#### Authors: Muhammad Aitsam, Alessandro Di Nuovo

#### Institute: Sheffield Hallam University

### Project Objective:

In recent years, the field of event-based vision has undergone significant advancements, fueled by the emergence of high-resolution event cameras. These cameras offer an exceptional dynamic range, unlocking new possibilities for improving human-robot interactions under different environmental conditions. In this study, we harness the potential of event-based vision technology to create an intuitive robot guidance system capable of interpreting hand gestures for precise robot control. Additionally, we introduce a pioneering high-resolution hand-gesture dataset. Notably, our approach leverages the advantages of high-resolution event cameras, excelling not only in normal environments but also in low-light conditions. The implications of our work are profound, facilitating safer and more efficient collaboration between robots and human workers in shared workspaces by enabling robots to understand and respond in different lighting conditions.


### PreRequisite:

Install Metavision SDK or OpenEB.

Follow the installation guidelines from: https://docs.prophesee.ai/stable/installation/index.html

### Dataset Creation:

Number of Samples: 1500 

Classes: "wave",
        "point",
        "fist",
        "clap",
        "armroll"

Lightning Conditions: Low light, Normal Light

Hands: Right and Left Hand

Distance: near, normal, far

Time: 3sec

DATA SAMPLE image

### Data Training Algorithms

1. ConvRNN
2. MobileNetV2
3. SqueezeNet

Training video gif

### Results

##### ConvRNN

Training Accuracy: 95.23%

Validation Accuracy: 91.4%

Testing: 88.68%

### Final Model (TorchScript)

You can clone the final trained + converted model for deployment in real-world scenarios.

- model_classifier.ptjit
- info_classifier_jit.json






