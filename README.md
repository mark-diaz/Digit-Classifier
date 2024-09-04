#### Motion Classification 
- This project utilizes Digital Signal Processing and Machine Learning techniques to classify motion patterns: in this specific use case: digits!
- For a more detailed overview my system design please see `APPENDIX.md`
- It utilizes the ARM-Based STM32 Microcontroller and its on-board accelerometer
	- This board had 2 megabytes of Flash memory with 786 Kilobytes of SRAM
- This project is written in C and utilizes the STM Cube IDE
- For an example console output through model training and classification please see `Console_Output.txt`

#### System Design:
<img width="868" alt="image" src="https://github.com/user-attachments/assets/5e1aa356-40eb-4e0f-9e4d-63b6bfb4b227">


#### Navigating the Code:
- The code I wrote is in `main.c` and `embedded_ML.c` utilizing the STM32 example design and an Embedded Machine Learning Library written by TA Charles Zaloom

`main.c`:

Contains the code for:
- STM32 setup code (Clock frequency, HAL Library, Instruction Cache, etc)
- The instantiation of the Neural Network with appropriate parameters and random number generation
- Infinite loop to start training and classification 

`embedded_ML.c`:

Contains the code for:
- Digital signal processing (velocity calculations, sampling, and filtering)
- Feature extraction and training loops for machine learning 
- Classification calculations taking max softmax output
- Helper functions to provide LED output to help user with performing motions
- Machine learning library code for gradient descent and back propagation


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
- I appreciate your time and thank you for reading this!
