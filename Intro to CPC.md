
![[Pasted image 20241203111120.png]]
* Major process variables - temperature, flow, pressure, level, composition
* This course is dynamic and thus we must move past steady state
## Analysing a system
* Identify the objective of any process
* The first letter of a signal is what its detecting and the second is for what it's being used for
* If the second letter is "I", then it's an indicator, for display. If the second letter is "T", its transmittance, for control system feedback
* signal transmission is done through electrical or pneumatic
* Pneumatic signals are for short distances, electrical through normal distance and for very long signals, digital
* ![[Pasted image 20241203115609.png]]
* "A signal is a flow of information"
## Thermocouple
![[Pasted image 20241203120655.png]]
* A voltage is created between T1 and T2 because of their temperatures and is in the microvolt level
* This is because of the seabeck effect - two junctions, at different temperatures cause a voltage 
* Peltier effect is when you put a voltage, one junction becomes hot and the other becomes cold
* The voltage does not vary linearly with temperature and thus a calibration polynomial must be used
* Thompson effect - voltage generated due to temperature gradient between two points
* The smallest change in temperature for which a change in voltage takes place is the resolution of the sensor.
>[!Important]
>* Resolution is the smallest change in the variable for which a change can be detected
>* Sensitivity is how big of a change in signal is caused due to a unit change in a variable
>* Note the difference 

* Accuracy - how close the measurement is to the true value. Error = Actual Value - Measured Value
* The time a sensor takes to give the measurement is called the dynamic lag. Like when you put a thermometer in your mouth, it takes some time to give the temperature. The time this takes is called the dynamic lag. *How fast my system responds to the change*
* Precision is the reproducibility of your measurement 
* ![[Pasted image 20241203122252.png]]
>[!todo]
>Assignment - Resistance Thermometer
>This is based on a principle that the resistance of a conductor varies with temperature

* Pressure sensor - strain gauge > simplest type of pressure sensor
* A differential pressure sensor has two pressures at two different sides with a diaphragm in the middle which deforms an element with properties that vary with deformation in the conductivity
![[Pasted image 20241210122645.png]]
One control loop costs not less than a few lakhs