Some motors only require one speed, so they need only a constant DC voltage into the inverter or the controller. However, many products today, including many power and gardening tools, and electric vehicles require variable motor speeds. Such motors use pulse width modulation (PWM) to vary the motor speeds. PWM offers precise control over the motor’s speed and torque and allows for variable speeds.

PWM is a square wave signal with a constant frequency, 

PWM converts the inverter DC voltage into a modulated effective voltage. For example, a 3.3V battery can be used to apply any voltage from 0V to 3.3V to the motor by using a PWM control signal that’s between a 0 percent and 100 percent duty cycle. Algorithms take advantage of this control methodology to efficiently limit the startup current and to regulate motor speed and torque.

https://do7js0tdxrds1.cloudfront.net/5k7nk2ibtwvasne94etpiul71khk?response-content-disposition=inline%3B+filename%3D%22Duty_Cycle_Examples.png%22%3B&response-content-type=image%2Fpng&Expires=1701084980&Signature=Cgif9nGVGX8dH~yO52CG-RRuMDr7T3wBTy1lg-EKv36yJTrtMVpazTujhKSsMkXaF523v0pz2yHwWzsVgcaMIg99~9dD0uovBjrc-KylWIHXFyUSlc14asvdV4AYgYduw-iTwLCvLwdyPmZyBd8gREzQncLLGeq9LX2advjAbd-QXHMFzgDDQ-Fg3uSFevfA3pN-eCSgaI7cpYCA8l82Nwm~3dM~-S46obN3~AS5g5SZp4Ds3OPfvj3NAoveufZq8nZ7Lb2y2QIhTn0B8VuwdhFoUOypjV-h3kod8oNY0dBNWAEMAv-Gf5MOtcT7TlWXEEq2DSDLddSApeLRwjYM5A__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

-=- PWM duty cycle
-=- *Source: [Thewrightstuff](https://commons.wikimedia.org/wiki/File:Duty_Cycle_Examples.png) | License [(CC BY-SA 3.0)](https://creativecommons.org/licenses/by-sa/3.0/deed.en)*

https://do7js0tdxrds1.cloudfront.net/hyf1a232l32w1lf2s1jeff2s5fhr?response-content-disposition=inline%3B+filename%3D%22PWM%2C_3-level.png%22%3B&response-content-type=image%2Fpng&Expires=1701084980&Signature=iESpnLCipqiC590mDP6MFoP~iVaem-MZDLTSdx8H4fVnWTzRH0Ucsz5zWx3RR2ZpMfpCnXqClokNzSs8C2qEr9-r-6BHfXZ8gnqbLaNeZWiULD06SZUPMYtkNYFtJpxG0JJocLe6-aD5WIZyRtOBxuGcH4dg5TgchzaiZ5rcrUHfRfqE7KUNJ15X0rWTTUjcwczfDlqeYWLxUA9dA18H1N8tamT2ndMFo~vnPuwsj3I5Hjo1O3qnVHWGpG4CN8zUKondZZDqmbdZ3sT5GhDEMybTRdSfhpNUseHogSD2FJd7lhVCo7SjfXaneJlCnnVmbU2tSrCkokIZsPYKQGxU7w__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

-=- (Image 3) PWM duty cycle
-=- *Source: [Zureks](https://commons.wikimedia.org/wiki/File:PWM,_3-level.svg) | License [(CC BY-SA 3.0)](https://creativecommons.org/licenses/by-sa/3.0/deed.en)*

An example of PWM in an idealized inductor driven by a (Blue) voltage source modulated as a series of pulses, resulting in a (Red)  sine-like current in the inductor. The rectangular voltage pulses nonetheless result in a more and more smooth current waveform, as the switching frequency increases. 

>Note that the current waveform is the integral of the voltage waveform.

PWM switching frequency is an important design factor to keep in mind during power stage development. 

Raising the switching frequency increases switching losses but improves current regulation in low-inductance motors. Lowering the switching frequency increases current ripple, which translates into torque ripple (for example, vibrations). 


Application voltage and motor inductance will steer the designer into choosing the correct PWM switching frequency. As a rule of thumb, the higher the voltage or current, the lower the switching frequency will need to be. Continuing to change the PWM signal changes the duty cycle, as shown in Figure 4. It gives a range of voltage values, which in turn changes the speed of the motor. You can use these PWM duty cycle changes to vary the voltage into the motor winding.

https://do7js0tdxrds1.cloudfront.net/bkdqjq5gvra6n6me910w3bim63ro?response-content-disposition=inline%3B+filename%3D%220021.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701084980&Signature=NXkJco-XIFZB8u6qs7dWo4Xyh8XJHfPr0RfuvM~36DLYz1fDReQpaZ4P5Fr9cBQFo7xpclWoRzTkvyzoe1QZAqFqPIOzy6sjkwFiuJ8lOT~lTU0k2kvW2ArZt2KP~6McLNTK91sE~T9jJdrhLlpB5xgLQEMVi5bQ8GcA7BQ-kdsmVJ1O6gK0MHKbDriS4pKfJ12FoZxoxq5cbX4uUUoZepb2hog2fGmYdguXyg8SuUg2Sg3T54gC4d-6c3oC3SnTyIpIj0ZUbjKodRge~HTIqdW0m40ngXNskTSem5ODEue0~spH4j-nlnOdozTtadMrbD~vY3Lw-5c1Cwr-KpRdkA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Figure 4 : A block diagram of commutation logic functionality with PWM applied.

Further reading : 
* https://www.youtube.com/watch?v=5nwNKPs2gco
* https://www.youtube.com/watch?v=90g6RpvXBYY
* https://www.youtube.com/watch?v=GQLED3gmONg


In the next section, we will be learning how to build our own motor controllers.