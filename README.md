#### Motion Classification 
- This project utilizes Digital Signal Processing and Machine Learning techniques to classify motion patterns: in this specific use case: digits!
- It utilizes the ARM-Based STM32 Microcontroller and its on-board accelerometer
	- This board had 2 megabytes of Flash memory with 786 Kilobytes of SRAM
- This project is written in C and utilizes the STM Cube IDE 
#### System Design:
```mermaid
flowchart LR
    A[Sensor Input] --> B[ADC]
    B --> C[DSP]
    C --> D[ML]
    D -->  E[Classifier Output]
    style A fill:#4a86e8,stroke:#333,stroke-width:2px
    style B fill:#4a86e8,stroke:#333,stroke-width:2px
    style C fill:#4a86e8,stroke:#333,stroke-width:2px
    style D fill:#4a86e8,stroke:#333,stroke-width:2px
    style E fill:#4a86e8,stroke:#333,stroke-width:2px
``` 
#### Project Results and Evaluation
- Sampling results across fifty different classifications this system predicted 47 of them to be the correct digit: 94% Accuracy!
	- The wrong predictions were likely to have been introduced by human error in data collection
- This project is a dynamic system that can train on changing data depending on what we want to classify in the field and Embedded ML is very flexible and dynamic 
	- In this case we are simply detecting digits and can recognize different letters and digits 
- I enjoyed this project because Internet of Things (IoT) requires many disciplines of engineering including: Transducers and Sensors, Digital Signal Processing, Embedded Systems, and Machine Learning!
**Product use and Application**: Education and Accessibilty
- This product can be used to teach young children how to correctly draw numbers and provide feedback
- This product can also be used to aid those who do not have the dexterity to draw numbers but can move a box to draw digits

#### Thank you for reading this
- Please see my presentation slides for a more detailed report of my design process!
