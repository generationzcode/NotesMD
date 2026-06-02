- So - I purposefully kept controllers out of [[Control Systems Intro]], we'll discuss them here
- There are three fundamental types of controllers, which can then be mixed and matched however you want: Proportional, Integral and Differential (PID)
- Controllers basically use the difference between the real value of the output and the objective to generate a signal for the final control element to actuate and change the manipulated variable
## Closed Loop Response
> How a controller used the error to generate an action, how that action closes the error and how that keeps the system going

![[Pasted image 20250312184719.png]]
- All the Gs are the transfer functions between the inputs and outputs of the block, d is the disturbance for the load, m is the change in the manipulated variable
- The process dynamics are:
- ![[Pasted image 20250312184849.png]]
- The control action:
- ![[Pasted image 20250312184933.png]]
- The error: 
- ![[Pasted image 20250312184944.png]]
- finally, m:
- ![[Pasted image 20250312185003.png]]
- to sum everything up, we can write the output as a function of the setpoint ($y_{sp}$) and disturbance:
- ![[Pasted image 20250312185111.png]]
- This formula works for every type of controller and each of those transfer functions can be tuned exactly for whatever process you're using 
- For every controller, there are two basic tasks:
- Servo Problem - when you change the setpoint (objective), you want the controller to cause the process to move
- Regulator Problem - when there's a disturbance and you want the controller to cause the process to come back to the objective
- We can easily see that the controller only depends on the function of error between the target variable and the objective. 
- I'd really like to write more about this but it's all self evident
## Proportional Controller
- The controller depends entirely on the absolute error to calculate the signal to correct
- This is way too easy to do the math for, the G_c is just a constant K_c
- Literally: 
- ![[Pasted image 20250312185712.png]]
## Integral Controller
- This is also known as a reset controller
- This can be understood by thinking of it as adding to the response a proportional controller would have given every time constant, so if there's no change, or little change, it will keep increasing the manipulation
- ![[Pasted image 20250313134450.png]]
- converting the above to a transfer function: 
- ![[Pasted image 20250313134911.png]]
- the rest of the math is pretty simple, just use what I wrote above
## Derivative
- used the derivative to "predict" the error in the near future and respond accordingly
- ![[Pasted image 20250313135024.png]]
