- Already spoke about this a while back - what feedback systems are
- so we got the manipulated variables - stuff you change to control the process variables, the load variables - the stuff that fluctuates outside of your control, requiring a control system and your target or objective - the process conditions
- ![[Pasted image 20250312175226.png]]
- components of a control system: process, sensors, transmission lines, controller, final control element
## Process
- we've already covered these in the [[First Order Systems]] and [[Second Order Systems]] and more on nth order systems
- Processes are constrained by physical laws and their engineering, causing them to end up as whatever order in differential equations.
- Whats funny is that these "first order" or "second order" systems mostly move up orders when a controller is added to the mix (the entire system).
- The process itself is first order, but since the controller interacts with it, we get something of a higher order. Unless you have a proportional controller of course
- Someday I might write more on this
## Sensors
- This is needed to input to the comparator (this is actually included in the controller, but we'll talk about it here anyways)
- The comparator basically gets the difference between the setpoint (what you want) and what you have. It gets the "error" ($\epsilon$)
- The sensor is sometimes first order, since it takes some time for the sensor itself to change it's conditions to measure. Unless specified in the near future though, we will be considering it an instantaneous process
- A bunch of sensors exist, made in a very creative way for a number of use cases:
- Flow sensors: orifice plate, venturi meter, turbine flow meter
- ![[Pasted image 20250312180649.png]]
- Pressure sensors: differential pressure cells. They all use a diaphragm and measure the change in some physical property of it when it deforms because of a pressure differential across it. The most popular one uses capacitance as the physical property. It's a second order system
- Temperature sensors: thermocouples, RTDs, and thermistors. These have a temperature sensing element inside a casing. If there is only one big thermal resistance between the process and the temperature sensing element, the system is modeled as a first order model. If there are two resistances, we can have something that can interact and we get a second order system. Thus (obviously) having a first order is faster and we want that over two resistances
- ![[Pasted image 20250312181324.png]]
- There are many more I unfortunately have to memorize :/
## Transmission Lines
- There are two types - pneumatic or electrical
- Pneumatic is composed of compressed fluids
- Pneumatic only holds (can be modeled as instantaneous) when the line is short and process doesnt change too fast
## Final Control Elements
- This is the actuator
- You have pneumatically controlled valves to control flow
- A nice little tip when you're designing for such systems, if the process simulation using this antiquated method or laplace or time domain shows you the manipulation required by the sensor is beyond the valve you have, you need an on/off valve, dont use a valve that can throttle for on/off
- The reason for the above is because throttling valves tend to have a stickiness property - if you push them to their limits, they become difficult to push back to normal operation
- These are called "sticky valves"
- We only use valves as actuators until now in the book. Even for heating systems, just adjust the flow rates of the thermal fluids