There is a fundamental relationship between the Velocity constant (K~v~), the armature current (I~a~), and torque (τ) in BLDC motors. 

`τ = (8.3 x Ia)/Kv `

* τ is in N.m
* K~V~ is in A 
* I~a~ is in RPM/V.

### Fundamental torque production

All the complexity of an electric motor ultimately boils down to the "BIL" Lorentz force law:

`Force = Magnetic field  × Current ×  Conductor length`

Increase one of the above terms without negatively impacting another, and you have increased the torque output of your system.

[Here is a great resource for understanding Torque constant, make sure to go through it.](https://things-in-motion.blogspot.com/2018/12/how-to-estimate-torque-of-bldc-pmsm.html)

### Watch this video to understand Motor Velocity constant (K~V~) better.

https://www.youtube.com/watch?v=zv_BrN60JTo

Now that you know what K~v~ and K~t~ are, let's calculate the velocity constant of our motor and compare it with the actual K~v~ as stated by the manufacturer.


![CodeCogsEqn (3).png](https://www.pupilfirst.school/markdown_attachments/4526/pa7h3i-Yep1MinYHRDsNag)


If we add in the calculated torque values to the equation below, we get 540 K~v~ as the velocity constant of our motor. 

![CodeCogsEqn (4).png](https://www.pupilfirst.school/markdown_attachments/4527/1KEibTyd7vRrCLN1G-IeDA)

The listed K~v~ of this motor was 640 K~v~ and so we are only off around 15%.

>In order to estimate the shape of the back EMF we need to do a series of simulations at different rotor angles and plot the torque output. This torque output can then be converted to K~v~ in the same way as shown in the equation above.

Below is a great resource to understand the powertrain design of efficient electric vehicles.

*Effects of number of turns of armature winding*