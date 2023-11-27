The Motor controller is involved in several jobs, but its main function is to regulate the speed and direction of the electric motor by controlling and changing the voltage applied to the phases. But what is a Phase? Let's have a look.

## What is a Phase, and what are 3 phase motors?

To explain it in simple terms, consider an alternating current (AC) from your household socket providing a voltage that varies with time, reversing in direction then going back again. On a 2-wire system, this means that the voltage between them varies from maximum to zero during each cycle, but in opposite directions. Because of the speed of 50 or 60 times per second, this variation is not noticeable in heating applications and is acceptable for many lighting systems.

A 3-phase electric supply gives three wires giving the same cycle, but each a little later, as shown in the diagram below. (More phases are possible, but 3 is enough and is the usual.) A fourth wire is also often used as a neutral wire, corresponding to the zero line in the diagram. Taking any phase and the neutral wire would give a standard AC system, e.g. Phase 1.

https://do7js0tdxrds1.cloudfront.net/xcc6cld63hj9e7o50b62c3icgvtl?response-content-disposition=inline%3B+filename%3D%22ezgif-2-dfe4333f7199.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701084636&Signature=ta9x5z~OgfWKAVlZPdLQ07ue-1JgGqPQNaLpqSShl2nxeJyEK-OvNxV13xkm983lwawbYbhSYCsXcQS0BPs~Rgzy~JcBJ6dtuEpF23itBmi2oHtIfjO2CBZKmM6g7jmcTU3LHjmCXaMRF9-ELm4KBvJjfy8hVLCeUQtOqH~Ut6MfXli90YpH7MvCutILxKcf5-mv9bDUuVwO29dwThpx6PP5WF63oaYPnq1~5nHoFkuoJinipuzOwiBQoknR~HLWAHjl-AAwLKROXjwLqkDOyccI5ZXfyFpvda~hrDhF52eZAQkXwDjKCeVWJK9KUthAqICApFnTelGLU-hPAULOHQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

-=- [3 phase waveform](https://commons.wikimedia.org/wiki/File:3_phase_AC_waveform.svg) | License: [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)

There are a number of advantages. Firstly, it is possible to deliver three times as much power as with 2 wires of the same size. Secondly, it is possible to deliver a higher voltage by taking the difference between two wires (instead of the difference between neutral and the maximum positive or negative). On the diagram, the maximum voltage from Phase 1 would be 1.0 (positive or negative). However, the maximum voltage between Phase 1 and Phase 2 is 1.5.

The third advantage is that it can be used to power a 3-phase motor, also known as an induction motor. By powering fixed electromagnets (as done in our Motor model), the different phases mean that a magnetic field is effectively rotating, which causes a rotor to be dragged around and thus rotate the shaft of the motor.

https://do7js0tdxrds1.cloudfront.net/9llppv3w9axb2jqbevs40e8lcrln?response-content-disposition=inline%3B+filename%3D%22ezgif-2-e6f399d7961b.jpg%22%3B&response-content-type=image%2Fjpeg&Expires=1701084636&Signature=hFE8qMQRZRbtRSPVE8Vy0upADndrx1zRAc8gxdHLTKbupugEdi~9N16-55rsoqINbd3t7Hh24hF7L3CqCVeNzvSXqLeKSoDfEY~7XmogDJUmP0R7K79sqJANtZXbzejWgmo4GJLd4PAslCvnyzAz959SBadJDWgfqhcEjVbfrZWtGjktHSY-hI~NpqAfSW33QbZhKCHLMtokp3lLbeBsOiAmxKhI7D9Om0lAQuLvPjziG89NJQoCxhHuiDxDHIHBFYIvxqtROf7a5u~tqcGK~VI9-lTUp8pQdq7bj-y1DANsawqCvghIy7e7XSq6VM3E2SVHr~agzglGPVS3syCVQA__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

-=- [*Rotating 3-phase magnetic field*](https://commons.wikimedia.org/wiki/File:Rotatingfield.png) | License:
[CC0 1.0 Universal Public Domain Dedication](https://creativecommons.org/publicdomain/zero/1.0/deed.en)

These motors are compact and cheap compared with the equivalent single-phase ones. 

--------------------------

## Motor controller

Functions of a typical motor controller include:

1. Regulating motor speed, torque, or power output.

2. Control startups and soft starts.

3. Protect against circuit faults.

4. Smooth motor acceleration and deceleration.

5. Protect against overloads.

To accomplish all of this, motor controllers must be much more intelligent than previously made controllers. For example, quality motor controllers increase efficiency by monitoring the load and controlling/adjusting the torque to match. The increased efficiency also reduces motor heat, overall noise, and vibrations. 

A BLDC motor or PMSM motor is usually controlled by various complicated systems consisting of multiple ICs (Integrated circuits) to provide various motor control functions. 

These circuits usually include 
* A microcontroller.
* Pre-driver power stages to drive power MOSFETs.
* Differential amplifiers for amplifying sensed motor currents. 
* Comparators to extract back-electromotive force (BEMF) information. 
* Switching and linear regulators to step down voltages.