* Control systems are called for 3 general classes of problems: suppressing the influence of external disturbances, ensuring the stability of chemical processes, and optimizing the performance of a chemical process
## Design aspects of a process control system
*  ![[Pasted image 20250121172447.png]]
* I *would* explain what each variable means but I assume our reader has half a brain to comprehend
* The above diagram is how variables in a chemical process control system are classified
### How to design a system:
* Define the control objectives - "what are the operational objectives a control system is called upon to achieve?" -> the answer lies in the three type of problems the control system is called to solve
* Select measurements - "what variables should we measure in order to monitor the operational performance of a plant?" -> so these are the measurements you need to be able to make regarding the control objectives of your system. The output variables. The ones that are classified as "measured" are "primary measurements" and "unmeasured" are "secondary measurements"
* Select the manipulated variables - "What are the manipulated variables that can be used to control a process?" -> input variables you can change to make a control loop
* Select the control configuration
* Design the controller - no question here, no selection here, just straight up get programming and soldering
## A little on control configurations
* A control configuration is the information structure that is used to connect the available measurements to the available manipulated variables
* Depending on number of inputs and outputs, we can distinguish control configurations as single input single output (SISO) or multiple input multiple output (MIMO)
* Three general types of control configurations exist:
* Feedback control configuration: uses direct measurements of controlled variables to adjust manipulated variables
* Inferential control configuration: uses secondary measurements(the controlled variables can't be measured) to adjust the values of manipulated variables. An estimator uses the inputs and outputs to make an estimation of where the controlled variable is at. Sort of like how an inertial navigation machine in airplanes works
* Feedforward control configuration: direct measurement of the disturbances to adjust values of manipulated variables
## Hardware
* In process control, the hardware used is: process equipment, sensors, transducers (convert signals between analog and digital), transmission lines [[Intro to CPC]], controller, final control element, recording elements
* the final control element is the hardware that can manipulate a variable
[[Problems on intro to CPC]]