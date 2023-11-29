>Begin work on this target only after you've completed the rest of the course.

### Aim:

The main goal of this exercise is to let us know what you have understood from this course.

### Brief:
To do that, you will need to upgrade your current model using the knowledge that you have gathered from the entire course. 

First, you will need to build a better model of the motor controller from what you have learnt in Phase 2 and Phase 3 of Level 3, i.e., combine the working knowledge of MOSFETs and the motor controller working principle from Phase 3 and build a Motor controller that consists of 6 MOSFETs (Instead of 6 relays) and make the motor run. _(Instructions given below)_

Then, you will move on to upgrading the communication aspect of the powertrain, which means, you will change and add more parameters in the BMS PCB to send more data to the motor controller to behave accordingly. _(Instructions given below)_

For example, the BMS collects voltage, current and temperature data from the batteries, you can send temperature or current data to the motor controller and program the controller to slow down or speed up the motor or act in a specific way depending on the BMS data. 

Once the upgraded model is built, you will build a flow diagram to show the working of the entire powertrain, and also share a video of the working prototype. 

> Make sure to make a presentable video that showcases the powertrain clearly, as this video can help in the hiring process, students in the previous batches have been hired directly based on this video.

------------

### 1. Instructions to upgrade the Level 3 Phase 3 Motor controller model.

**Components required**
 
- **3** x IRF9530 / IRF9540 MOSFET  (P channel)
- **3** x IRFZ44N MOSFET (N channel)
- **3** x Motor controller PCB (Purple PCBs)
- **2** x 20Pin Male Header pins
- **3** x 330 ohm resistors (2 watt)
- **2** x meters Multistrand Wire 
- **1** x soldering iron kit
- **6** x BC558 Transistor (P channel)
- **6** x 100 ohm resistors

#### Step 1 : Organising the components,

- Each Purple PCB board needs 
    - 1 IRF9540 MOSFET
    - 1 IRFZ44N MOSFET
    - 2 BC 558 Transistor
    - 2 10k ohm Resistors
    - 2 330 Ohm resistors
    - 1 470 Ohm resistor.

#### Step 2 : Soldering all the components.

https://do7js0tdxrds1.cloudfront.net/4efa0e6br0cne2tmwd4jrvg4liv2?response-content-disposition=inline%3B+filename%3D%22WhatsApp+Image+2023-05-02+at+6.52.36+PM.jpeg%22%3B&response-content-type=image%2Fjpeg&Expires=1701255710&Signature=sZXWEmIfxTL44xWlvIx2qAR--B1WObMyTGG9e1LTHDgpj6fq~-QDwKYuctmQbxVGqHORlGfH5Castu9ZeDgbH1GO-YaQEpYvajzBDDUbhy~~P7H4UDK0SAPvBC9SoT57Ny5dU2-iP4b0AZaTtuRrho1CgN0LbGeTe6wCxj4EkUTLRFTtBo6TIzx3h83HzlCtokV~Ub87n8eNJjak0Cc5cUcqkuwmqYmlLdgoY83tkFfbtCNkwmGkTcEQ3oQacC5JPJiBgdh8IEJs5MIGBoX8HLrtSBHXlPQPTpXrTFoS0qCe1OjNm5KecLhbG3S5OKSEjZppQIlzHCLikg3WdTQihw__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Use the Markings on the Given PCB to place all the components required. For example, 

 - Place the corresponding MOSFET (Ex IRFZ44N) on the marked spot on the PCB with the same name.
 - Once done, flip the PCB and solder the MOSFET in place.
 - Do the same for all the components.

 #### Step 3. Assembling

Use what you learned in Level 3 Phase 3, where you used 6 relays to run a motor and apply the same circuit here.

Instead of 6 relays, we now have 6 MOSFETs. 

>If you have trouble figuring out the correct circuit connections, create a Forum post on Discord and we'll help guide you

----------

### Instructions for the Flow Diagram

#### 1. BMS Algorithm used for charging

https://do7js0tdxrds1.cloudfront.net/iicrz1k7zuq253ls8o6m24tfqcp7?response-content-disposition=inline%3B+filename%3D%22capstone+flowcharts.png%22%3B&response-content-type=image%2Fpng&Expires=1701255710&Signature=NGTHnkWRRrrhVD1G1N0sni9A9JnHFOS5kVtVGUlRHpUkvB4FOBdEz~iWZ2gZaeX12sVSxP3osEVYPBwVWHycmCNnB67GgGcmYqtvED225Jw4sMiEoD3a~aHzmg4vSZgBggBFZsnuHPiGjj48a3-5GHvse~PsPbG2MqYF0IoIptqBVb1mZRKWQTtwVuNgNMe05LGcrmcDcup8uetMH~v~ePXcXDKLUVOhAGduIM~qqVIG5WHEzHxRtTImPZEmQV1geeU9VAYOMcafR9bJhwAapqHJtzBZ9ldO4GZqvvGMazs-RC~5Qjqlrt9xNx0McauFLghOQJ4iNvFxafLw1QynaQ__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

#### 2. Upgrading the Communications

Your current communications system from Level 8 only transmits if the battery voltage is high or low, which in turn controls the status of the motor in terms of Switched on or switched off.

This needs to be upgraded to transmit a lot more data to the motor, than in turn the motor needs to behave accordingly.

Example 1. With change in battery temperature, the motor speeds need to be reduced, or power needs to be restricted.

Example 2. With change in battery Voltage, Instead of switching off the motor, you need to write code to change the speed of the motor. (You have learnt how to change speed in Level 3)

The parameter that are available to you are, 

   - Battery temperature
        - Cell 1 temperature
        - Cell 2 temperature
   - Battery voltage
        - Cell 1 Voltage
        - Cell 2 Voltage
   - Discharge Current
   - Power consumption
 
You can see one example of how the parameters interact from the flow chart below.

Once you have a working communications code ready, you will need to build a flow chart to show exactly how the flow of information takes place between the 2 Arduinos

https://do7js0tdxrds1.cloudfront.net/rubacot32jhemj7qhmjod4za3vmc?response-content-disposition=inline%3B+filename%3D%22capstone+flowcharts+%28powertrain%29.png%22%3B&response-content-type=image%2Fpng&Expires=1701255710&Signature=QL0YfKFFpE5fisZ5o7VwU6kTw9iCXJ~H9cZsT8LvZIoh9fQ4LOj6mdGwhk~vNcVu7KLvPJKEOozq2WNJ95RRJNAZX-Q20~hJkizsm-rLYvGTHHl2fJYRoXq~gDL2HziFZEQ3KqUfqyf-ZU058MU-UlfgTjfmDyHVLtF5CKB5-d1MCwsR-HVuQmBwq2yRpm4Pqi5ZF9lILsLCl-ON6oFCmI4z3cz8z2Ctw-gGx0QhZDVZ4KMDpe7Yr2GJ~jLtwmNIFIPXrbo1RJlnzcjau3CJ7skx0QUyl7aT1wHh4wLg1MLYpqHJ4kU13Vv5DWdOHCHzESfaXQv2brpQMleKw0c2dg__&Key-Pair-Id=K2Q3HDJ6ZAQGFF

Report Template

## Instructions for the Video 

From level 3, you will explain how the signals coming from an Arduino effect the MOSFETs or Relays, which in turn rotate the motors.

Explain, briefly, how switching the MOSFETs or RELAYS `off` and `on` at certain intervals has the capacity to make the motor rotate.

For Level 8, explain what the 2 Arduinos are communicating, and how they are responding to each signal, and what are those signals as shown in the flowchart doing to the motor. 

You will need to explain everything you have done to make the motor run using the rubric given below.

## Rubric

1. Rebuild your projects/assemble your projects such that they are in working condition.
2. Once they are in working condition, record a small 5-10 minute video explaining how each component works, starting with Level 2.
3. Explain how the motor was built-in Level 2, and give out a brief of what difficulties you faced and how you fixed it.
4. Same as above for Level 3, explain how the circuit works to make the motor run and give a brief idea of all the problems you faced and what you did to solve them.
5. Briefly explain what the circuit is doing in Level 6 BMS,
6. Explain what the 2 Arduinos are communicating in Level 8 and how these communications affect the running of the motor.

## Video Layout

1. Start by introducing yourself. 
2. Pan your camera towards your model. Start with the Motor. 
3. Explain how the motor works without the controller.

    1. Explain why the coils are placed in a circle 120 degrees apart, and how does this arrangement make the rotor rotate.
    2. Why is the magnet placed so close to the coil? How does the distance between the coil and the rotor magnet effect the rotation?

4. Now, Pan towards the motor controller and explain how the signals travel through the controller to make the motor work. 

    1. Name each component used in the motor controller.
    2. What is the function of the MOSFETs in the circuit?
    3. What happens when a 5 volt signal is sent from the Arduino to the MOSFET?
    4. How does this 5 volt signal make the motor rotate?
    5. Can you increase the speed of the motor by changing the code? If yes, how? (Demonstrate the speed changing part)
   
5. Pan to the Battery management system circuit and explain briefly how it works. 
6. Highlight which communication BUS is used and what signals are sent between the motor controller and the battery management system. 
7. Explain briefly how these signals affect the working of the motor controller. 
8. Pan outward such that the full working model is visible in the frame. 
9. End video. 

>Once done, upload the video and wait for review. All the Best!

>Make sure the video is under 10 mins long. You can keep all the explanations brief to stay within this duration.